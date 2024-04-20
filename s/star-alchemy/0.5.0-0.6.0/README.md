# Comparing `tmp/star_alchemy-0.5.0.tar.gz` & `tmp/star_alchemy-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "star_alchemy-0.5.0.tar", max compression
+gzip compressed data, was "star_alchemy-0.6.0.tar", max compression
```

## Comparing `star_alchemy-0.5.0.tar` & `star_alchemy-0.6.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1072 2024-04-20 08:54:38.862902 star_alchemy-0.5.0/LICENSE
--rw-r--r--   0        0        0      583 2024-04-20 09:11:43.098941 star_alchemy-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       81 2024-04-20 09:00:01.825574 star_alchemy-0.5.0/star_alchemy/__init__.py
--rw-r--r--   0        0        0     8523 2024-04-20 09:09:52.190925 star_alchemy-0.5.0/star_alchemy/_star_schema.py
--rw-r--r--   0        0        0      527 1970-01-01 00:00:00.000000 star_alchemy-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-20 08:54:38.862902 star_alchemy-0.6.0/LICENSE
+-rw-r--r--   0        0        0      583 2024-04-20 12:54:47.016060 star_alchemy-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       81 2024-04-20 09:00:01.825574 star_alchemy-0.6.0/star_alchemy/__init__.py
+-rw-r--r--   0        0        0     8563 2024-04-20 12:53:30.464055 star_alchemy-0.6.0/star_alchemy/_star_schema.py
+-rw-r--r--   0        0        0      527 1970-01-01 00:00:00.000000 star_alchemy-0.6.0/PKG-INFO
```

### Comparing `star_alchemy-0.5.0/LICENSE` & `star_alchemy-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `star_alchemy-0.5.0/pyproject.toml` & `star_alchemy-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "star-alchemy"
-version = "0.5.0"
+version = "0.6.0"
 description = ""
 authors = ["Daniel Bradburn <moagstar@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 sqlalchemy = "^2"
 toolz = "^0.12.0"
```

### Comparing `star_alchemy-0.5.0/star_alchemy/_star_schema.py` & `star_alchemy-0.6.0/star_alchemy/_star_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,17 @@
     """
     if select.select_from_override:
         compiled = compiler.process(super(Schema._Select, select), **kw)
         return compiled
 
     # get the columns (and thus the tables) from the sub-expressions involved in this query
     tables = {
-        x.table for x in visitors.iterate(select, {}) if isinstance(x, ColumnClause)
+        x.table
+        for x in visitors.iterate(select, {})
+        if isinstance(x, ColumnClause) and x.table is not None
     }
 
     # TODO: Perhaps only join to lowest common root rather than root? For example
     #  if there are no expressions coming directly from job, do we always need to
     #  join to job?
     # use paths to generate the joins based on the tables present in this query
     joins = unique(
```

### Comparing `star_alchemy-0.5.0/PKG-INFO` & `star_alchemy-0.6.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: star-alchemy
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 Author: Daniel Bradburn
 Author-email: moagstar@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

