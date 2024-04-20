# Comparing `tmp/star-alchemy-0.4.0.tar.gz` & `tmp/star_alchemy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "star-alchemy-0.4.0.tar", max compression
+gzip compressed data, was "star_alchemy-0.5.0.tar", max compression
```

## Comparing `star-alchemy-0.4.0.tar` & `star_alchemy-0.5.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1072 2022-09-08 16:09:54.411296 star-alchemy-0.4.0/LICENSE
--rw-r--r--   0        0        0      583 2023-02-02 12:26:40.459628 star-alchemy-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       67 2023-02-02 10:12:39.695050 star-alchemy-0.4.0/star_alchemy/__init__.py
--rw-r--r--   0        0        0     7642 2023-02-02 10:12:39.695050 star-alchemy-0.4.0/star_alchemy/_star_schema.py
--rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 star-alchemy-0.4.0/setup.py
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 star-alchemy-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-20 08:54:38.862902 star_alchemy-0.5.0/LICENSE
+-rw-r--r--   0        0        0      583 2024-04-20 09:11:43.098941 star_alchemy-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       81 2024-04-20 09:00:01.825574 star_alchemy-0.5.0/star_alchemy/__init__.py
+-rw-r--r--   0        0        0     8523 2024-04-20 09:09:52.190925 star_alchemy-0.5.0/star_alchemy/_star_schema.py
+-rw-r--r--   0        0        0      527 1970-01-01 00:00:00.000000 star_alchemy-0.5.0/PKG-INFO
```

### Comparing `star-alchemy-0.4.0/LICENSE` & `star_alchemy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `star-alchemy-0.4.0/pyproject.toml` & `star_alchemy-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "star-alchemy"
-version = "0.4.0"
+version = "0.5.0"
 description = ""
 authors = ["Daniel Bradburn <moagstar@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 sqlalchemy = "^2"
 toolz = "^0.12.0"
```

### Comparing `star-alchemy-0.4.0/star_alchemy/_star_schema.py` & `star_alchemy-0.5.0/star_alchemy/_star_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,33 @@
 import dataclasses
+import typing
 from functools import cached_property, partial
 
-from sqlalchemy import Column
 from sqlalchemy.ext.compiler import compiles
 from sqlalchemy.sql import ClauseElement, FromClause, Select, Selectable, visitors
+from sqlalchemy.sql.elements import ColumnClause
 from toolz import first, sliding_window, unique
 
+LeftRight = tuple[Selectable, Selectable]
+OnClause = typing.Callable[[Selectable, Selectable], ClauseElement]
+
+
+@dataclasses.dataclass
+class Join:
+    on_clause_func: OnClause | None = None
+    isouter: bool = True
+    full: bool = False
+
+    def __post_init__(self):
+        if not self.isouter and self.full:
+            raise ValueError("Cannot specify full=True unless isouter is also True")
+
+
+JoinDict = dict[LeftRight, Join | OnClause]
+
 
 @dataclasses.dataclass(frozen=True)
 class Schema:
     """
     Defines a star-alchemy schema. This defines how tables are attached
     together and is used to automatically detect the joins that are
     needed for a particular query. There are 3 main parts to the API...
@@ -25,15 +43,15 @@
     ... })
 
     2. The tables can be inspected `Schema.tables`
     3. Queries can be generated using `Schema.select`
     """
 
     definition: dict
-    on_clauses: dict = dataclasses.field(default_factory=dict)
+    joins: JoinDict = dataclasses.field(default_factory=dict)
 
     @property
     def root(self):
         return self.table_paths[0][0]
 
     @cached_property
     def tables(self):
@@ -79,30 +97,46 @@
         def _paths(obj, path=()):
             for table, value in (obj if isinstance(obj, dict) else {}).items():
                 yield table, (table_path := tuple([*path, table.name]))
                 yield from _paths(value, table_path)
 
         return list(_paths(self.definition))
 
-    def on_clause(self, left: Selectable, right: Selectable) -> ClauseElement:
+    def join(
+        self, left: Selectable, right: Selectable
+    ) -> tuple[ClauseElement, bool, bool]:
         """
         Generate the on_clause for joining two tables. If there is a
         simple foreign key relationship between the tables then it is
         possible to automatically generate this clause, otherwise an
         explicit join needs to be specified in the constructor, for
         example...
 
         :param left: Left selectable.
         :param right: Right selectable.
 
         :return: Expression which is used to join the two tables.
         """
-        on_clause_func = self.on_clauses.get((left, right), self._default_on_clause)
-        on_clause = on_clause_func(left, right)
-        return on_clause
+        join = self.joins.get((left, right), self._default_on_clause)
+
+        if isinstance(join, Join):
+            on_clause_func = (
+                self._default_on_clause
+                if join.on_clause_func is None
+                else join.on_clause_func
+            )
+            on_clause = on_clause_func(left, right)
+            isouter = join.isouter
+            full = join.full
+        else:
+            on_clause = join(left, right)
+            isouter = True
+            full = False
+
+        return on_clause, isouter, full
 
     class _Select(Select):
         """
         Special sqlalchemy select that stores the `Schema` which
         generated it. This can then be used to automatically generate
         the `select_from` for the query.
         """
@@ -153,15 +187,17 @@
     be joined.
     """
     if select.select_from_override:
         compiled = compiler.process(super(Schema._Select, select), **kw)
         return compiled
 
     # get the columns (and thus the tables) from the sub-expressions involved in this query
-    tables = {x.table for x in visitors.iterate(select, {}) if isinstance(x, Column)}
+    tables = {
+        x.table for x in visitors.iterate(select, {}) if isinstance(x, ColumnClause)
+    }
 
     # TODO: Perhaps only join to lowest common root rather than root? For example
     #  if there are no expressions coming directly from job, do we always need to
     #  join to job?
     # use paths to generate the joins based on the tables present in this query
     joins = unique(
         join
@@ -174,21 +210,21 @@
     for join in joins:
 
         # get the left and right tables of the join
         get_table = partial(getattr, select._schema.tables)
         left_table, right_table = map(get_table, join)
 
         # get the on clause which should be used to join the two tables
-        on_clause = select._schema.on_clause(left_table, right_table)
+        join = select._schema.join(left_table, right_table)
 
         # generate the select_from, because we are performing this in a loop
         # the select_from is built from the previous iteration, iteratively
         # building the joins needed for this selecct_from
         select_from = left_table if select_from is None else select_from
-        select_from = select_from.join(right_table, on_clause, isouter=True)
+        select_from = select_from.join(right_table, *join)
 
     # Add the select_from to the select, if there are no joins, we still might
     # need to select from the root table in the schema
     if select_from is not None:
         select = super(Schema._Select, select).select_from(select_from)
     elif select._schema.root in tables:
         select_from = select._schema.root
```

