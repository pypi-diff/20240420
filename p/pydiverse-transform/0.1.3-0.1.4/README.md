# Comparing `tmp/pydiverse_transform-0.1.3.tar.gz` & `tmp/pydiverse_transform-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiverse_transform-0.1.3.tar", max compression
+gzip compressed data, was "pydiverse_transform-0.1.4.tar", max compression
```

## Comparing `pydiverse_transform-0.1.3.tar` & `pydiverse_transform-0.1.4.tar`

### file list

```diff
@@ -1,40 +1,52 @@
--rw-r--r--   0        0        0     1517 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/LICENSE
--rw-r--r--   0        0        0     2331 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/docs/package/README.md
--rw-r--r--   0        0        0     1471 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       13 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/.gitignore
--rw-r--r--   0        0        0      387 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/transform/__init__.py
--rw-r--r--   0        0        0      108 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/__init__.py
--rw-r--r--   0        0        0     3470 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/alignment.py
--rw-r--r--   0        0        0     2797 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/column.py
--rw-r--r--   0        0        0     5082 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/dispatchers.py
--rw-r--r--   0        0        0      191 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/expressions/__init__.py
--rw-r--r--   0        0        0     1078 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/expressions/expressions.py
--rw-r--r--   0        0        0      682 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/expressions/lambda_getter.py
--rw-r--r--   0        0        0     4871 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/expressions/symbolic_expressions.py
--rw-r--r--   0        0        0     4881 2023-06-27 07:59:14.838718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/expressions/translator.py
--rw-r--r--   0        0        0     1708 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/expressions/util.py
--rw-r--r--   0        0        0      530 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/functions.py
--rw-r--r--   0        0        0      135 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/__init__.py
--rw-r--r--   0        0        0      903 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/aggregate.py
--rw-r--r--   0        0        0     3590 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/core.py
--rw-r--r--   0        0        0     1694 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/logical.py
--rw-r--r--   0        0        0     2341 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/numeric.py
--rw-r--r--   0        0        0    17847 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/registry.py
--rw-r--r--   0        0        0      518 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/string.py
--rw-r--r--   0        0        0      334 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/window.py
--rw-r--r--   0        0        0     3833 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/table.py
--rw-r--r--   0        0        0    16536 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/table_impl.py
--rw-r--r--   0        0        0       84 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/util/__init__.py
--rw-r--r--   0        0        0     2637 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/util/bidict.py
--rw-r--r--   0        0        0     1161 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/util/ordered_set.py
--rw-r--r--   0        0        0     1892 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/util/util.py
--rw-r--r--   0        0        0    14653 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/core/verbs.py
--rw-r--r--   0        0        0       42 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/eager/__init__.py
--rw-r--r--   0        0        0      265 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/eager/eager_table.py
--rw-r--r--   0        0        0    21015 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/eager/pandas_table.py
--rw-r--r--   0        0        0       36 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/lazy/__init__.py
--rw-r--r--   0        0        0      454 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/lazy/lazy_table.py
--rw-r--r--   0        0        0    26850 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/lazy/sql_table.py
--rw-r--r--   0        0        0        0 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/util/__init__.py
--rw-r--r--   0        0        0      730 2023-06-27 07:59:14.842718 pydiverse_transform-0.1.3/src/pydiverse/transform/util/testing.py
--rw-r--r--   0        0        0     3160 1970-01-01 00:00:00.000000 pydiverse_transform-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1517 2024-04-19 23:55:18.089497 pydiverse_transform-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2331 2024-04-19 23:55:18.089497 pydiverse_transform-0.1.4/docs/package/README.md
+-rw-r--r--   0        0        0     2238 2024-04-19 23:55:18.089497 pydiverse_transform-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       13 2024-04-19 23:55:18.089497 pydiverse_transform-0.1.4/src/pydiverse/.gitignore
+-rw-r--r--   0        0        0      423 2024-04-19 23:55:18.089497 pydiverse_transform-0.1.4/src/pydiverse/transform/__init__.py
+-rw-r--r--   0        0        0      297 2024-04-19 23:55:18.089497 pydiverse_transform-0.1.4/src/pydiverse/transform/_typing.py
+-rw-r--r--   0        0        0      152 2024-04-19 23:55:18.089497 pydiverse_transform-0.1.4/src/pydiverse/transform/core/__init__.py
+-rw-r--r--   0        0        0     3490 2024-04-19 23:55:18.089497 pydiverse_transform-0.1.4/src/pydiverse/transform/core/alignment.py
+-rw-r--r--   0        0        0     5229 2024-04-19 23:55:18.089497 pydiverse_transform-0.1.4/src/pydiverse/transform/core/dispatchers.py
+-rw-r--r--   0        0        0     4910 2024-04-19 23:55:18.089497 pydiverse_transform-0.1.4/src/pydiverse/transform/core/dtypes.py
+-rw-r--r--   0        0        0      332 2024-04-19 23:55:18.089497 pydiverse_transform-0.1.4/src/pydiverse/transform/core/expressions/__init__.py
+-rw-r--r--   0        0        0     8189 2024-04-19 23:55:18.089497 pydiverse_transform-0.1.4/src/pydiverse/transform/core/expressions/expressions.py
+-rw-r--r--   0        0        0      708 2024-04-19 23:55:18.089497 pydiverse_transform-0.1.4/src/pydiverse/transform/core/expressions/lambda_getter.py
+-rw-r--r--   0        0        0     5261 2024-04-19 23:55:18.089497 pydiverse_transform-0.1.4/src/pydiverse/transform/core/expressions/symbolic_expressions.py
+-rw-r--r--   0        0        0     6028 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/core/expressions/translator.py
+-rw-r--r--   0        0        0     1907 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/core/expressions/util.py
+-rw-r--r--   0        0        0     1003 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/core/functions.py
+-rw-r--r--   0        0        0    20636 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/core/registry.py
+-rw-r--r--   0        0        0     3845 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/core/table.py
+-rw-r--r--   0        0        0    20327 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/core/table_impl.py
+-rw-r--r--   0        0        0      120 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/core/util/__init__.py
+-rw-r--r--   0        0        0     2635 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/core/util/bidict.py
+-rw-r--r--   0        0        0     1159 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/core/util/ordered_set.py
+-rw-r--r--   0        0        0     2222 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/core/util/util.py
+-rw-r--r--   0        0        0    15548 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/core/verbs.py
+-rw-r--r--   0        0        0       78 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/eager/__init__.py
+-rw-r--r--   0        0        0      265 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/eager/eager_table.py
+-rw-r--r--   0        0        0    32535 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/eager/pandas_table.py
+-rw-r--r--   0        0        0      763 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/errors/__init__.py
+-rw-r--r--   0        0        0       72 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/lazy/__init__.py
+-rw-r--r--   0        0        0      440 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/lazy/lazy_table.py
+-rw-r--r--   0        0        0       72 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/lazy/sql_table/__init__.py
+-rw-r--r--   0        0        0      146 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/lazy/sql_table/dialects/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/lazy/sql_table/dialects/duckdb.py
+-rw-r--r--   0        0        0    10123 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/lazy/sql_table/dialects/mssql.py
+-rw-r--r--   0        0        0     3167 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/lazy/sql_table/dialects/postgres.py
+-rw-r--r--   0        0        0     3338 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/lazy/sql_table/dialects/sqlite.py
+-rw-r--r--   0        0        0    38447 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/lazy/sql_table/sql_table.py
+-rw-r--r--   0        0        0      241 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/ops/__init__.py
+-rw-r--r--   0        0        0     1212 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/ops/aggregate.py
+-rw-r--r--   0        0        0     3863 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/ops/core.py
+-rw-r--r--   0        0        0      899 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/ops/datetime.py
+-rw-r--r--   0        0        0      299 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/ops/generic.py
+-rw-r--r--   0        0        0     2464 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/ops/logical.py
+-rw-r--r--   0        0        0      425 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/ops/markers.py
+-rw-r--r--   0        0        0     2355 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/ops/numeric.py
+-rw-r--r--   0        0        0     1437 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/ops/string.py
+-rw-r--r--   0        0        0     1368 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/ops/window.py
+-rw-r--r--   0        0        0       65 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/util/__init__.py
+-rw-r--r--   0        0        0      865 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/util/reraise.py
+-rw-r--r--   0        0        0     1304 2024-04-19 23:55:18.093497 pydiverse_transform-0.1.4/src/pydiverse/transform/util/warnings.py
+-rw-r--r--   0        0        0     3290 1970-01-01 00:00:00.000000 pydiverse_transform-0.1.4/PKG-INFO
```

### Comparing `pydiverse_transform-0.1.3/LICENSE` & `pydiverse_transform-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.3/docs/package/README.md` & `pydiverse_transform-0.1.4/docs/package/README.md`

 * *Files identical despite different names*

### Comparing `pydiverse_transform-0.1.3/src/pydiverse/transform/core/alignment.py` & `pydiverse_transform-0.1.4/src/pydiverse/transform/core/alignment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,97 +1,101 @@
 from __future__ import annotations
 
 import inspect
+from typing import TYPE_CHECKING
 
-from pydiverse.transform.core import column, table, table_impl
-from pydiverse.transform.core.expressions import symbolic_expressions, util
+from pydiverse.transform.core.expressions import (
+    Column,
+    LiteralColumn,
+    SymbolicExpression,
+    util,
+)
+from pydiverse.transform.errors import AlignmentError
+
+if TYPE_CHECKING:
+    from pydiverse.transform.core import AbstractTableImpl, Table
 
 
 def aligned(*, with_: str):
     """Decorator for aligned functions."""
+    from pydiverse.transform.core import AbstractTableImpl, Table
+
     if callable(with_):
         raise ValueError("Decorator @aligned requires with_ argument.")
 
     def decorator(func):
         signature = inspect.signature(func)
         if not isinstance(with_, str):
-            raise Exception(
+            raise TypeError(
                 f"Argument 'with_' must be of type str, not '{type(with_).__name__}'."
             )
         if with_ not in signature.parameters:
-            raise Exception(f"Function has no argument named '{with_}'")
+            raise ValueError(f"Function has no argument named '{with_}'")
 
         def wrapper(*args, **kwargs):
             # Execute func
             result = func(*args, **kwargs)
-            if not isinstance(result, symbolic_expressions.SymbolicExpression):
-                raise ValueError(
+            if not isinstance(result, SymbolicExpression):
+                raise TypeError(
                     "Aligned function must return a symbolic expression not"
                     f" '{result}'."
                 )
 
             # Extract the correct `with_` argument for eval_aligned
             bound_sig = signature.bind(*args, **kwargs)
             bound_sig.apply_defaults()
 
             alignment_param = bound_sig.arguments[with_]
-            if isinstance(alignment_param, symbolic_expressions.SymbolicExpression):
+            if isinstance(alignment_param, SymbolicExpression):
                 alignment_param = alignment_param._
 
-            if isinstance(alignment_param, column.Column):
+            if isinstance(alignment_param, Column):
                 aligned_with = alignment_param.table
-            elif isinstance(
-                alignment_param, (table.Table, table_impl.AbstractTableImpl)
-            ):
+            elif isinstance(alignment_param, (Table, AbstractTableImpl)):
                 aligned_with = alignment_param
             else:
                 raise NotImplementedError
 
             # Evaluate aligned
             return eval_aligned(result, with_=aligned_with)
 
         return wrapper
 
     return decorator
 
 
 def eval_aligned(
-    sexpr: symbolic_expressions.SymbolicExpression,
-    with_: table_impl.AbstractTableImpl | table.Table = None,
-    **kwargs,
-) -> symbolic_expressions.SymbolicExpression[column.LiteralColumn]:
+    sexpr: SymbolicExpression, with_: AbstractTableImpl | Table = None, **kwargs
+) -> SymbolicExpression[LiteralColumn]:
     """Evaluates an expression using the AlignedExpressionEvaluator."""
+    from pydiverse.transform.core import AbstractTableImpl, Table
 
-    expr = (
-        sexpr._ if isinstance(sexpr, symbolic_expressions.SymbolicExpression) else sexpr
-    )
+    expr = sexpr._ if isinstance(sexpr, SymbolicExpression) else sexpr
 
     # Determine Backend
     backend = util.determine_expr_backend(expr)
     if backend is None:
         # TODO: Handle this case. Should return some value...
         raise NotImplementedError
 
     # Evaluate the function calls on the shared backend
     alignedEvaluator = backend.AlignedExpressionEvaluator(backend.operator_registry)
     result = alignedEvaluator.translate(expr, **kwargs)
 
-    literal_column = column.LiteralColumn(
-        typed_value=result, expr=expr, backend=backend
-    )
+    literal_column = LiteralColumn(typed_value=result, expr=expr, backend=backend)
 
     # Check if alignment condition holds
     if with_ is not None:
-        if isinstance(with_, table.Table):
+        if isinstance(with_, Table):
             with_ = with_._impl
-        if not isinstance(with_, table_impl.AbstractTableImpl):
-            raise ValueError(
+        if not isinstance(with_, AbstractTableImpl):
+            raise TypeError(
                 "'with_' must either be an instance of a Table or TableImpl. Not"
                 f" '{with_}'."
             )
 
         if not with_.is_aligned_with(literal_column):
-            raise ValueError(f"Result of eval_aligned isn't aligned with {with_}.")
+            raise AlignmentError(f"Result of eval_aligned isn't aligned with {with_}.")
 
     # Convert to sexpr so that the user can easily continue transforming
     # it symbolically.
-    return symbolic_expressions.SymbolicExpression(literal_column)
+    return SymbolicExpression(literal_column)
```

### Comparing `pydiverse_transform-0.1.3/src/pydiverse/transform/core/dispatchers.py` & `pydiverse_transform-0.1.4/src/pydiverse/transform/core/dispatchers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
 import copy
 from functools import partial, reduce, wraps
 from typing import Any
 
-from pydiverse.transform.core import column, table, verbs
-from pydiverse.transform.core.expressions import unwrap_symbolic_expressions
-from pydiverse.transform.core.table_impl import AbstractTableImpl
+from pydiverse.transform.core.expressions import (
+    Column,
+    LambdaColumn,
+    unwrap_symbolic_expressions,
+)
 from pydiverse.transform.core.util import bidict, traverse
 
 
 class Pipeable:
     def __init__(self, f=None, calls=None):
         if f is not None:
             if calls is not None:
@@ -25,15 +27,15 @@
         -> Lazy. Extend pipe.
         """
         if isinstance(other, Pipeable):
             return Pipeable(calls=self.calls + other.calls)
         elif callable(other):
             return Pipeable(calls=self.calls + [other])
 
-        raise Exception
+        raise RuntimeError
 
     def __rrshift__(self, other):
         """
         other >> Pipeable
         -> Eager.
         """
         if callable(other):
@@ -55,18 +57,18 @@
     def __call__(self, /, *args, **keywords):
         keywords = {**self.keywords, **keywords}
         #                   ↙ *args moved to front.
         return self.func(*args, *self.args, **keywords)
 
 
 def verb(func):
+    from pydiverse.transform.core.table import Table
+
     def copy_tables(arg: Any = None):
-        return traverse(
-            arg, lambda x: copy.copy(x) if isinstance(x, table.Table) else x
-        )
+        return traverse(arg, lambda x: copy.copy(x) if isinstance(x, Table) else x)
 
     @wraps(func)
     def wrapper(*args, **kwargs):
         # Copy Table objects to prevent mutating them
         # This can be the case if the user uses __setitem__ inside the verb
         def f(*args, **kwargs):
             args = copy_tables(args)
@@ -137,37 +139,41 @@
 
         def get_c(b, tB):
             tC = b >> left_join(tB, b == tB.b)
             return tC[tB.c]
         feature_col = get_c(tblA.b, tblB)
 
     """
+    from pydiverse.transform.core.verbs import select
 
-    if isinstance(arg, column.Column):
-        tbl = (arg.table >> verbs.select(arg))._impl  # type: AbstractTableImpl
+    if isinstance(arg, Column):
+        tbl = (arg.table >> select(arg))._impl
         col = tbl.get_col(arg)
 
         tbl.available_cols = {col.uuid}
         tbl.named_cols = bidict({col.name: col.uuid})
         return tbl
-    elif isinstance(arg, column.LambdaColumn):
-        raise ValueError
+    elif isinstance(arg, LambdaColumn):
+        raise ValueError("Can't start a pipe with a lambda column.")
 
     return arg
 
 
 def unwrap_tables(arg: Any = None):
     """
     Takes an instance or collection of `Table` objects and replaces them with
     their implementation.
     """
-    return traverse(arg, lambda x: x._impl if isinstance(x, table.Table) else x)
+    from pydiverse.transform.core.table import Table
+
+    return traverse(arg, lambda x: x._impl if isinstance(x, Table) else x)
 
 
 def wrap_tables(arg: Any = None):
     """
     Takes an instance or collection of `AbstractTableImpl` objects and wraps
     them in a `Table` object. This is an inverse to the `unwrap_tables` function.
     """
-    return traverse(
-        arg, lambda x: table.Table(x) if isinstance(x, AbstractTableImpl) else x
-    )
+    from pydiverse.transform.core.table import Table
+    from pydiverse.transform.core.table_impl import AbstractTableImpl
+
+    return traverse(arg, lambda x: Table(x) if isinstance(x, AbstractTableImpl) else x)
```

### Comparing `pydiverse_transform-0.1.3/src/pydiverse/transform/core/expressions/lambda_getter.py` & `pydiverse_transform-0.1.4/src/pydiverse/transform/core/expressions/lambda_getter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
-from pydiverse.transform.core.column import LambdaColumn
-from pydiverse.transform.core.expressions import SymbolicExpression
+from pydiverse.transform.core.expressions import LambdaColumn
+from pydiverse.transform.core.expressions.symbolic_expressions import SymbolicExpression
 
 
 class LambdaColumnGetter:
     """
     An instance of this object can be used to instantiate a LambdaColumn.
     """
```

### Comparing `pydiverse_transform-0.1.3/src/pydiverse/transform/core/expressions/symbolic_expressions.py` & `pydiverse_transform-0.1.4/src/pydiverse/transform/core/expressions/symbolic_expressions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 from __future__ import annotations
 
 from html import escape
-from typing import Any, Generic, TypeVar
+from typing import Any, Generic
 
-from pydiverse.transform.core import alignment
+from pydiverse.transform._typing import T
+from pydiverse.transform.core.expressions import CaseExpression, FunctionCall, util
+from pydiverse.transform.core.registry import OperatorRegistry
 from pydiverse.transform.core.util import traverse
 
-from ..ops import registry
-from . import expressions, util
-
-T = TypeVar("T")
-
 
 class SymbolicExpression(Generic[T]):
     """
     Base class to represent a symbolic expression. It can be manipulated using
     standard python operators (for example you can add them) or by calling
     attributes of it.
 
@@ -36,35 +33,46 @@
             raise AttributeError(
                 f"Invalid attribute {item}. Attributes can't begin and end with an"
                 " underscore."
             )
         return SymbolAttribute(item, self)
 
     def __getitem__(self, item):
-        return SymbolicExpression(expressions.FunctionCall("__getitem__", self, item))
+        return SymbolicExpression(FunctionCall("__getitem__", self, item))
+
+    def case(self, *cases: tuple[Any, Any], default: Any = None):
+        case_expression = CaseExpression(
+            switching_on=self,
+            cases=cases,
+            default=default,
+        )
+
+        return SymbolicExpression(case_expression)
 
     def __dir__(self):
         # TODO: Instead of displaying all available operators, translate the
         #       expression and according to the dtype and backend only display
         #       the operators that actually are available.
-        return sorted(registry.OperatorRegistry.ALL_REGISTERED_OPS)
+        return sorted(OperatorRegistry.ALL_REGISTERED_OPS)
 
     # __contains__, __iter__ and __bool__ are all invalid on s-expressions
     __contains__ = None
     __iter__ = None
 
     def __bool__(self):
         raise TypeError(
             "Symbolic expressions can't be converted to True/False, "
             "or used with these keywords: not, and, or."
         )
 
     def __str__(self):
+        from pydiverse.transform.core.alignment import eval_aligned
+
         try:
-            result = alignment.eval_aligned(self._, check_alignment=False)._
+            result = eval_aligned(self._, check_alignment=False)._
 
             dtype = result.typed_value.dtype
             value = result.typed_value.value
             return (
                 f"Symbolic Expression: {repr(self._)}\ndtype: {dtype}\n\n{str(value)}"
             )
         except Exception as e:
@@ -74,22 +82,26 @@
                 f"{type(e).__name__}: {str(e)}"
             )
 
     def __repr__(self):
         return f"<Sym: {self._}>"
 
     def _repr_html_(self):
+        from pydiverse.transform.core.alignment import eval_aligned
+
         html = f"<pre>Symbolic Expression:\n{escape(repr(self._))}</pre>"
 
         try:
-            result = alignment.eval_aligned(self._, check_alignment=False)._
+            result = eval_aligned(self._, check_alignment=False)._
             backend = util.determine_expr_backend(self._)
 
             value_repr = backend._html_repr_expr(result.typed_value.value)
-            html += f"dtype: <code>{escape(result.typed_value.dtype)}</code></br></br>"
+            html += (
+                f"dtype: <code>{escape(str(result.typed_value.dtype))}</code></br></br>"
+            )
             html += f"<pre>{escape(value_repr)}</pre>"
         except Exception as e:
             html += (
                 "</br><pre>Failed to get evaluate due to an exception:\n"
                 f"{escape(e.__class__.__name__)}: {escape(str(e))}</pre>"
             )
 
@@ -104,17 +116,15 @@
         self.__name = name
         self.__on = on
 
     def __getattr__(self, item) -> SymbolAttribute:
         return SymbolAttribute(self.__name + "." + item, self.__on)
 
     def __call__(self, *args, **kwargs) -> SymbolicExpression:
-        return SymbolicExpression(
-            expressions.FunctionCall(self.__name, self.__on, *args, **kwargs)
-        )
+        return SymbolicExpression(FunctionCall(self.__name, self.__on, *args, **kwargs))
 
     def __hash__(self):
         raise Exception(
             "Nope... You probably didn't want to do this. Did you misspell the"
             f" attribute name '{self.__name}' of '{self.__on}'? Maybe you forgot a"
             " leading underscore."
         )
@@ -128,15 +138,15 @@
 
 
 # Add all supported dunder methods to `SymbolicExpression`.
 # This has to be done, because Python doesn't call __getattr__ for
 # dunder methods.
 def create_operator(op):
     def impl(*args, **kwargs):
-        return SymbolicExpression(expressions.FunctionCall(op, *args, **kwargs))
+        return SymbolicExpression(FunctionCall(op, *args, **kwargs))
 
     return impl
 
 
-for dunder in registry.OperatorRegistry.SUPPORTED_DUNDER:
+for dunder in OperatorRegistry.SUPPORTED_DUNDER:
     setattr(SymbolicExpression, dunder, create_operator(dunder))
 del create_operator
```

### Comparing `pydiverse_transform-0.1.3/src/pydiverse/transform/core/expressions/translator.py` & `pydiverse_transform-0.1.4/src/pydiverse/transform/core/expressions/translator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,85 +1,85 @@
 from __future__ import annotations
 
 import dataclasses
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, Generic, TypeVar
-from collections.abc import Iterable
+from typing import TYPE_CHECKING, Any, Generic
 
-from pydiverse.transform.core import column
-from pydiverse.transform.core.expressions import expressions
-from pydiverse.transform.core.ops import Operator, OPType, registry
+from pydiverse.transform._typing import T
+from pydiverse.transform.core import registry
+from pydiverse.transform.core.expressions import (
+    CaseExpression,
+    Column,
+    FunctionCall,
+    LiteralColumn,
+)
+from pydiverse.transform.ops.core import Operator, OPType
+from pydiverse.transform.util import reraise
 
 if TYPE_CHECKING:
-    # noinspection PyUnresolvedReferences
-    from pydiverse.transform.core.table_impl import AbstractTableImpl
-
-ImplT = TypeVar("ImplT", bound="AbstractTableImpl")
-T = TypeVar("T")
+    from pydiverse.transform.core.dtypes import DType
 
 
 # Basic container to store value and associated type metadata
 @dataclass
 class TypedValue(Generic[T]):
     value: T
-    dtype: str
+    dtype: DType
     ftype: OPType = dataclasses.field(default=OPType.EWISE)
 
     def __iter__(self):
         return iter((self.value, self.dtype))
 
 
 class Translator(Generic[T]):
     def translate(self, expr, **kwargs) -> T:
         """Translate an expression recursively."""
         try:
             return bottom_up_replace(expr, lambda e: self._translate(e, **kwargs))
         except Exception as e:
-            raise ValueError(
-                "An exception occured while trying to translate the expression"
-                f" '{expr}':\n{e}"
-            ) from e
+            msg = f"This exception occurred while translating the expression: {expr}"
+            reraise(e, suffix=msg)
 
     def _translate(self, expr, **kwargs) -> T:
         """Translate an expression non recursively."""
         raise NotImplementedError
 
 
-class DelegatingTranslator(Generic[T], Translator[T]):
+class DelegatingTranslator(Translator[T], Generic[T]):
     """
     Translator that dispatches to different translate functions based on
     the type of the expression.
     """
 
     def __init__(self, operator_registry: registry.OperatorRegistry):
         self.operator_registry = operator_registry
 
     def translate(self, expr, **kwargs):
         """Translate an expression recursively."""
         try:
             return self._translate(expr, **kwargs)
         except Exception as e:
-            raise ValueError(
-                "An exception occured while trying to translate the expression"
-                f" '{expr}':\n{e}"
-            ) from e
+            msg = f"This exception occurred while translating the expression: {expr}"
+            reraise(e, suffix=msg)
 
-    def _translate(self, expr, accept_literal_col=True, **kwargs):
-        if isinstance(expr, column.Column):
+    def _translate(self, expr, **kwargs):
+        if isinstance(expr, Column):
             return self._translate_col(expr, **kwargs)
 
-        if isinstance(expr, column.LiteralColumn):
-            if accept_literal_col:
-                return self._translate_literal_col(expr, **kwargs)
-            else:
-                raise ValueError("Literal columns aren't allowed in this context.")
+        if isinstance(expr, LiteralColumn):
+            return self._translate_literal_col(expr, **kwargs)
 
-        if isinstance(expr, expressions.FunctionCall):
+        if isinstance(expr, FunctionCall):
             operator = self.operator_registry.get_operator(expr.name)
-            op_args, op_kwargs, context_kwargs = self.__translate_function_arguments(
+
+            # Mutate function call arguments using operator
+            expr_args, expr_kwargs = operator.mutate_args(expr.args, expr.kwargs)
+            expr = FunctionCall(expr.name, *expr_args, **expr_kwargs)
+
+            op_args, op_kwargs, context_kwargs = self._translate_function_arguments(
                 expr, operator, **kwargs
             )
 
             if op_kwargs:
                 raise NotImplementedError
 
             signature = tuple(arg.dtype for arg in op_args)
@@ -87,44 +87,73 @@
                 expr.name, signature
             )
 
             return self._translate_function(
                 expr, implementation, op_args, context_kwargs, **kwargs
             )
 
+        if isinstance(expr, CaseExpression):
+            switching_on = (
+                self._translate(expr.switching_on, **{**kwargs, "context": "case_val"})
+                if expr.switching_on is not None
+                else None
+            )
+
+            cases = []
+            for cond, value in expr.cases:
+                cases.append(
+                    (
+                        self._translate(cond, **{**kwargs, "context": "case_cond"}),
+                        self._translate(value, **{**kwargs, "context": "case_val"}),
+                    )
+                )
+
+            default = self._translate(expr.default, **{**kwargs, "context": "case_val"})
+            return self._translate_case(expr, switching_on, cases, default, **kwargs)
+
         if literal_result := self._translate_literal(expr, **kwargs):
             return literal_result
 
         raise NotImplementedError(
             f"Couldn't find a way to translate object of type {type(expr)} with value"
             f" {expr}."
         )
 
-    def _translate_col(self, expr: column.Column, **kwargs) -> T:
+    def _translate_col(self, expr: Column, **kwargs) -> T:
         raise NotImplementedError
 
-    def _translate_literal_col(self, expr: column.LiteralColumn, **kwargs) -> T:
+    def _translate_literal_col(self, expr: LiteralColumn, **kwargs) -> T:
         raise NotImplementedError
 
     def _translate_function(
         self,
-        expr: expressions.FunctionCall,
+        expr: FunctionCall,
         implementation: registry.TypedOperatorImpl,
-        op_args: Iterable[T],
+        op_args: list[T],
         context_kwargs: dict[str, Any],
         **kwargs,
     ) -> T:
         raise NotImplementedError
 
+    def _translate_case(
+        self,
+        expr: CaseExpression,
+        switching_on: T | None,
+        cases: list[tuple[T, T]],
+        default: T,
+        **kwargs,
+    ) -> T:
+        raise NotImplementedError
+
     def _translate_literal(self, expr, **kwargs) -> T:
         raise NotImplementedError
 
-    def __translate_function_arguments(
-        self, expr: expressions.FunctionCall, operator: Operator, **kwargs
-    ):
+    def _translate_function_arguments(
+        self, expr: FunctionCall, operator: Operator, **kwargs
+    ) -> tuple[list[T], dict[str, T], dict[str, Any]]:
         op_args = [self._translate(arg, **kwargs) for arg in expr.args]
         op_kwargs = {}
         context_kwargs = {}
 
         for k, v in expr.kwargs.items():
             if k in operator.context_kwargs:
                 context_kwargs[k] = v
@@ -132,18 +161,26 @@
                 op_kwargs[k] = self._translate(v, **kwargs)
 
         return op_args, op_kwargs, context_kwargs
 
 
 def bottom_up_replace(expr, replace):
     def transform(expr):
-        if isinstance(expr, expressions.FunctionCall):
-            f = expressions.FunctionCall(
+        if isinstance(expr, FunctionCall):
+            f = FunctionCall(
                 expr.name,
                 *(transform(arg) for arg in expr.args),
                 **{k: transform(v) for k, v in expr.kwargs.items()},
             )
             return replace(f)
-        else:
-            return replace(expr)
+
+        if isinstance(expr, CaseExpression):
+            c = CaseExpression(
+                switching_on=transform(expr.switching_on),
+                cases=[(transform(k), transform(v)) for k, v in expr.cases],
+                default=transform(expr.default),
+            )
+            return replace(c)
+
+        return replace(expr)
 
     return transform(expr)
```

### Comparing `pydiverse_transform-0.1.3/src/pydiverse/transform/core/expressions/util.py` & `pydiverse_transform-0.1.4/src/pydiverse/transform/core/expressions/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Type
+from typing import TYPE_CHECKING
 
-from pydiverse.transform.core import column
-
-from . import expressions
+from pydiverse.transform.core.expressions import (
+    CaseExpression,
+    Column,
+    FunctionCall,
+    LiteralColumn,
+)
 
 if TYPE_CHECKING:
     # noinspection PyUnresolvedReferences
     from pydiverse.transform.core.table_impl import AbstractTableImpl
 
 
 def iterate_over_expr(expr, expand_literal_col=False):
     """
     Iterate in depth-first preorder over the expression and yield all components.
     """
 
     yield expr
 
-    if isinstance(expr, expressions.FunctionCall):
+    if isinstance(expr, FunctionCall):
+        for child in expr.iter_children():
+            yield from iterate_over_expr(child, expand_literal_col=expand_literal_col)
+        return
+
+    if isinstance(expr, CaseExpression):
         for child in expr.iter_children():
             yield from iterate_over_expr(child, expand_literal_col=expand_literal_col)
         return
 
-    if expand_literal_col and isinstance(expr, column.LiteralColumn):
+    if expand_literal_col and isinstance(expr, LiteralColumn):
         yield from iterate_over_expr(expr.expr, expand_literal_col=expand_literal_col)
         return
 
 
 def determine_expr_backend(expr) -> type[AbstractTableImpl] | None:
     """Returns the backend used in an expression.
 
@@ -35,17 +43,17 @@
     If no backend can be determined (because the expression doesn't contain a
     column), None is returned instead. If different backends are being used,
     throws an exception.
     """
 
     backends = set()
     for atom in iterate_over_expr(expr):
-        if isinstance(atom, column.Column):
+        if isinstance(atom, Column):
             backends.add(type(atom.table))
-        if isinstance(atom, column.LiteralColumn):
+        if isinstance(atom, LiteralColumn):
             backends.add(atom.backend)
 
     if len(backends) == 1:
         return backends.pop()
     if len(backends) >= 2:
         raise ValueError(
             "Expression contains different backends "
```

### Comparing `pydiverse_transform-0.1.3/src/pydiverse/transform/core/functions.py` & `pydiverse_transform-0.1.4/src/pydiverse/transform/core/functions.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 from __future__ import annotations
 
-from .expressions import FunctionCall, SymbolicExpression
+from typing import Any
+
+from pydiverse.transform.core.expressions import (
+    CaseExpression,
+    FunctionCall,
+    SymbolicExpression,
+)
 
 __all__ = [
     "count",
     "row_number",
 ]
 
 
@@ -17,7 +23,25 @@
         return _sym_f_call("count")
     else:
         return _sym_f_call("count", expr)
 
 
 def row_number(*, arrange: list):
     return _sym_f_call("row_number", arrange=arrange)
+
+
+def case(*cases: tuple[Any, Any], default: Any = None):
+    case_expression = CaseExpression(
+        switching_on=None,
+        cases=cases,
+        default=default,
+    )
+
+    return SymbolicExpression(case_expression)
+
+
+def min(first: Any, *expr: Any):
+    return _sym_f_call("__least", first, *expr)
+
+
+def max(first: Any, *expr: Any):
+    return _sym_f_call("__greatest", first, *expr)
```

### Comparing `pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/aggregate.py` & `pydiverse_transform-0.1.4/src/pydiverse/transform/ops/aggregate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 from __future__ import annotations
 
-from .core import Aggregate, Unary
+from pydiverse.transform.ops.core import Aggregate, Unary
 
 __all__ = [
     "Min",
     "Max",
     "Mean",
     "Sum",
+    "Any",
+    "All",
     "StringJoin",
     "Count",
 ]
 
 
 class Min(Aggregate, Unary):
     name = "min"
     signatures = [
         "int -> int",
         "float -> float",
         "str -> str",
+        "datetime -> datetime",
     ]
 
 
 class Max(Aggregate, Unary):
     name = "max"
     signatures = [
         "int -> int",
         "float -> float",
         "str -> str",
+        "datetime -> datetime",
     ]
 
 
 class Mean(Aggregate, Unary):
     name = "mean"
     signatures = [
         "int -> float",
@@ -42,18 +46,32 @@
     name = "sum"
     signatures = [
         "int -> int",
         "float -> float",
     ]
 
 
+class Any(Aggregate, Unary):
+    name = "any"
+    signatures = [
+        "bool -> bool",
+    ]
+
+
+class All(Aggregate, Unary):
+    name = "all"
+    signatures = [
+        "bool -> bool",
+    ]
+
+
 class StringJoin(Aggregate):
     name = "join"
     signatures = [
-        "str, str -> str",
+        "str, const str -> str",
     ]
 
 
 class Count(Aggregate):
     name = "count"
     signatures = [
         "-> int",
```

### Comparing `pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/core.py` & `pydiverse_transform-0.1.4/src/pydiverse/transform/ops/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 import enum
-import typing
 from collections import ChainMap
+from typing import TYPE_CHECKING
 
-from pydiverse.transform.core.ops import registry
+if TYPE_CHECKING:
+    from pydiverse.transform.core.registry import OperatorSignature
 
 __all__ = [
     "OPType",
     "Operator",
     "OperatorExtension",
     "Arity",
     "Nullary",
     "Unary",
     "Binary",
     "ElementWise",
     "Aggregate",
     "Window",
+    "Marker",
 ]
 
 
 class OPType(enum.IntEnum):
     EWISE = 1
     AGGREGATE = 2
     WINDOW = 3
@@ -76,17 +78,23 @@
 
     def __eq__(self, other):
         return type(self) == type(other)
 
     def __hash__(self):
         return hash(type(self))
 
-    def validate_signature(self, signature: registry.OperatorSignature) -> bool:
+    def validate_signature(self, signature: OperatorSignature):
         pass
 
+    def mutate_args(self, args, kwargs):
+        """
+        Allows the operator to modify the arguments passed to it before translation
+        """
+        return args, kwargs
+
 
 class OperatorExtension:
     """
     An extension to an operator. Provides additional signatures.
     """
 
     operator: type[Operator] = NotImplemented
@@ -140,7 +148,11 @@
 
 
 class Window(Operator):
     ftype = OPType.WINDOW
     context_kwargs = {
         "arrange",  # List[Column | LambdaColumn]
     }
+
+
+class Marker(Operator):
+    ftype = None
```

### Comparing `pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/logical.py` & `pydiverse_transform-0.1.4/src/pydiverse/transform/ops/logical.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,65 @@
 from __future__ import annotations
 
-from .core import Binary, ElementWise, Unary
+from pydiverse.transform.core import dtypes
+from pydiverse.transform.ops.core import Binary, ElementWise, Operator, Unary
 
 __all__ = [
     "Equal",
     "NotEqual",
     "Less",
     "LessEqual",
     "Greater",
     "GreaterEqual",
+    "IsIn",
     "And",
     "RAnd",
     "Or",
     "ROr",
     "Xor",
     "RXor",
     "Invert",
 ]
 
 
+class Logical(Operator):
+    # Operator that returns a "REAL" boolean.
+    # This is mostly relevant for mssql
+    pass
+
+
 #### Comparison Operators ####
 
 
-class Comparison(ElementWise, Binary):
+class Comparison(ElementWise, Binary, Logical):
     signatures = [
         "int, int -> bool",
-        "int, float -> bool",
-        "float, int -> bool",
         "float, float -> bool",
         "str, str -> bool",
         "bool, bool -> bool",
+        "datetime, datetime -> bool",
     ]
 
     def validate_signature(self, signature):
-        assert signature.rtype == "bool"
+        assert isinstance(signature.rtype, dtypes.Bool)
         super().validate_signature(signature)
 
 
 class Equal(Comparison):
     name = "__eq__"
+    signatures = Comparison.signatures + [
+        "T, const none -> bool",
+    ]
 
 
 class NotEqual(Comparison):
     name = "__ne__"
+    signatures = Comparison.signatures + [
+        "T, const none -> bool",
+    ]
 
 
 class Less(Comparison):
     name = "__lt__"
 
 
 class LessEqual(Comparison):
@@ -57,25 +70,39 @@
     name = "__gt__"
 
 
 class GreaterEqual(Comparison):
     name = "__ge__"
 
 
+class IsIn(ElementWise, Logical):
+    name = "isin"
+    signatures = [
+        # TODO: A signature like "T, const list[const T] -> bool" would be better
+        "T, const T... -> bool",
+    ]
+
+
 #### Boolean Operators ####
 
 
-class BooleanBinary(ElementWise, Binary):
+class BooleanBinary(ElementWise, Binary, Logical):
     signatures = [
         "bool, bool -> bool",
     ]
 
     def validate_signature(self, signature):
-        assert signature.args == ("bool", "bool")
-        assert signature.rtype == "bool"
+        assert len(signature.args) == 2
+
+        for arg_dtype in signature.args:
+            assert isinstance(arg_dtype, dtypes.Bool)
+            assert not arg_dtype.vararg
+            assert not arg_dtype.const
+
+        assert isinstance(signature.rtype, dtypes.Bool)
         super().validate_signature(signature)
 
 
 class And(BooleanBinary):
     name = "__and__"
 
 
@@ -95,12 +122,12 @@
     name = "__xor__"
 
 
 class RXor(BooleanBinary):
     name = "__rxor__"
 
 
-class Invert(ElementWise, Unary):
+class Invert(ElementWise, Unary, Logical):
     name = "__invert__"
     signatures = [
         "bool -> bool",
     ]
```

### Comparing `pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/numeric.py` & `pydiverse_transform-0.1.4/src/pydiverse/transform/ops/numeric.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from . import Binary, ElementWise, Unary
+from pydiverse.transform.ops.core import Binary, ElementWise, Unary
 
 __all__ = [
     "Add",
     "RAdd",
     "Sub",
     "RSub",
     "Mul",
@@ -66,16 +66,14 @@
     name = "__rmul__"
 
 
 class TrueDiv(ElementWise, Binary):
     name = "__truediv__"
     signatures = [
         "int, int -> float",
-        "int, float -> float",
-        "float, int -> float",
         "float, float -> float",
     ]
 
 
 class RTrueDiv(TrueDiv):
     name = "__rtruediv__"
 
@@ -90,15 +88,16 @@
 class RFloorDiv(FloorDiv):
     name = "__rfloordiv__"
 
 
 class Pow(ElementWise, Binary):
     name = "__pow__"
     signatures = [
-        "int, int -> int",
+        "int, int -> float",
+        "float, float -> float",
     ]
 
 
 class RPow(Pow):
     name = "__rpow__"
 
 
@@ -137,11 +136,11 @@
     ]
 
 
 class Round(ElementWise):
     name = "__round__"
     signatures = [
         "int -> int",
-        "int, int -> int",
-        "float -> int",
-        "float, int -> float",
+        "int, const int -> int",
+        "float -> float",
+        "float, const int -> float",
     ]
```

### Comparing `pydiverse_transform-0.1.3/src/pydiverse/transform/core/ops/registry.py` & `pydiverse_transform-0.1.4/src/pydiverse/transform/core/registry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,133 +1,157 @@
 from __future__ import annotations
 
 import dataclasses
 import functools
 import inspect
 import itertools
-import typing
+import textwrap
+from collections.abc import Iterable
 from functools import partial
+from typing import TYPE_CHECKING, Callable
 
-if typing.TYPE_CHECKING:
-    from pydiverse.transform.core.ops import Operator, OperatorExtension
+from pydiverse.transform.core import dtypes
+from pydiverse.transform.errors import ExpressionTypeError
+
+if TYPE_CHECKING:
+    from pydiverse.transform.ops import Operator, OperatorExtension
 
 
 class OperatorImpl:
     """
     Internal type to store the implementation of an operator and all associated
     metadata.
 
     If the function (`impl`) provided as the underlying parameter has keyword
     only arguments that start with an underscore, they get added to the
     `self.internal_kwargs` list.
     """
 
-    id = itertools.count()
+    id_ = itertools.count()
 
     def __init__(
         self,
         operator: Operator,
-        impl: typing.Callable,
+        impl: Callable,
         signature: OperatorSignature,
     ):
         self.operator = operator
         self.impl = impl
         self.signature = signature
-        self.variants: dict[str, typing.Callable] = {}
+        self.variants: dict[str, Callable] = {}
 
-        self.__id = next(OperatorImpl.id)
+        self.__id = next(OperatorImpl.id_)
 
         # Inspect impl signature to get internal kwargs
-        self.internal_kwargs = []
-
-        try:
-            impl_signature = inspect.signature(impl)
-            for name, param in impl_signature.parameters.items():
-                if param.kind == inspect.Parameter.KEYWORD_ONLY and name.startswith(
-                    "_"
-                ):
-                    self.internal_kwargs.append(name)
-        except (TypeError, ValueError):
-            pass
+        self.internal_kwargs = self._compute_internal_kwargs(impl)
+        self.variant_internal_kwargs = {}
 
         # Calculate Ordering Key
         # - Find match with the least number templates in the signature
         # - From those take the one with the least number of different templates
         # - From those take the one where the first template appears latest
+        # - From those take the one where the const modifiers match better
         # - From those take the one that isn't a vararg or has the most arguments.
         # - From those take the one that was defined first
 
         num_templates = 0
         templates_set = set()
-        first_template_index = len(signature.args)
+        template_indices = []
+        const_modifiers = []
         for i, dtype in enumerate(signature.args):
-            if is_template_type(dtype):
+            if isinstance(dtype, dtypes.Template):
                 num_templates += 1
-                templates_set.add(dtype)
-                first_template_index = min(first_template_index, i)
+                templates_set.add(dtype.name)
+                template_indices.append(-i)
+            if dtype.const:
+                const_modifiers.append(i)
         num_different_templates = len(templates_set)
         is_vararg = int(self.signature.is_vararg)
 
         self._precedence = (
             num_templates,
             num_different_templates,
-            -first_template_index,
+            tuple(template_indices),
+            tuple(const_modifiers),
             is_vararg,
             -len(signature.args),
             self.__id,
         )
 
-    def add_variant(self, name: str, impl: typing.Callable):
+    def add_variant(self, name: str, impl: Callable):
         if name in self.variants:
             raise ValueError(
                 f"Already added a variant with name '{name}'"
                 f" to operator {self.operator}."
             )
         self.variants[name] = impl
+        self.variant_internal_kwargs[name] = self._compute_internal_kwargs(impl)
+
+    @staticmethod
+    def _compute_internal_kwargs(impl: Callable):
+        internal_kwargs = []
+        try:
+            impl_signature = inspect.signature(impl)
+            for name, param in impl_signature.parameters.items():
+                if param.kind == inspect.Parameter.KEYWORD_ONLY and name.startswith(
+                    "_"
+                ):
+                    internal_kwargs.append(name)
+        except (TypeError, ValueError):
+            pass
+
+        return internal_kwargs
 
 
 @dataclasses.dataclass
 class TypedOperatorImpl:
     """
     Operator Implementation with a non-templated return type.
     Unlike `OperatorImpl`, this class is intended to be the return type of
     the OperatorRegistry.
     """
 
     operator: Operator
     impl: OperatorImpl
-    rtype: str
+    rtype: dtypes.DType
 
     @classmethod
-    def from_operator_impl(cls, impl: OperatorImpl, rtype: str):
+    def from_operator_impl(cls, impl: OperatorImpl, rtype: dtypes.DType):
         return cls(
             operator=impl.operator,
             impl=impl,
             rtype=rtype,
         )
 
     def __call__(self, *args, **kwargs):
         return self.impl.impl(*args, **self.__clean_kwargs(kwargs))
 
-    def get_variant(self, name: str) -> typing.Callable | None:
+    def has_variant(self, name: str) -> bool:
+        return name in self.impl.variants
+
+    def get_variant(self, name: str) -> Callable | None:
         variant = self.impl.variants.get(name)
         if variant is None:
             return None
 
         @functools.wraps(variant)
         def variant_wrapper(*args, **kwargs):
-            return variant(*args, **self.__clean_kwargs(kwargs))
+            return variant(*args, **self.__clean_kwargs(kwargs, variant=name))
 
         return variant_wrapper
 
-    def __clean_kwargs(self, kwargs):
+    def __clean_kwargs(self, kwargs, variant=None):
+        internal_kwargs = self.impl.internal_kwargs
+        if variant:
+            internal_kwargs = self.impl.variant_internal_kwargs[variant]
+
         return {
             k: v
             for k, v in kwargs.items()
-            if not k.startswith("_") or k in self.impl.internal_kwargs
+            if not k.startswith("_") or k in internal_kwargs
         }
 
 
 class OperatorRegistry:
     # It only makes sense to define some dunder methods.
     # These are the ones which can be registered.
     SUPPORTED_DUNDER = {
@@ -162,15 +186,15 @@
         "__ne__",
         "__gt__",
         "__ge__",
     }
 
     # Set containing all operator names that have been defined across all registries.
     # Used for __dir__ method of SymbolicExpression
-    ALL_REGISTERED_OPS = set()  # type: set[str]
+    ALL_REGISTERED_OPS: set[str] = set()
 
     def __init__(self, name, super_registry=None):
         self.name = name
         self.super_registry = super_registry
         self.registered_ops = set()  # type: set[Operator]
         self.implementations = dict()  # type: dict[str, OperatorImplementationStore]
         self.check_super = dict()  # type: dict[str, bool]
@@ -203,20 +227,25 @@
 
         self.registered_ops.add(operator)
         self.ALL_REGISTERED_OPS.add(name)
 
     def get_operator(self, name: str) -> Operator | None:
         if impl_store := self.implementations.get(name, None):
             return impl_store.operator
-        return None
+
+        # If operation hasn't been defined in this registry, go to the parent
+        # registry and check if it has been defined there.
+        if self.super_registry is None or not self.check_super.get(name, True):
+            raise ValueError(f"No implementation for operator '{name}' found")
+        return self.super_registry.get_operator(name)
 
     def add_implementation(
         self,
         operator: Operator,
-        impl: typing.Callable,
+        impl: Callable,
         signature: str,
         variant: str | None = None,
     ):
         if operator not in self.registered_ops:
             raise ValueError(
                 f"Operator {operator} ({operator.name}) hasn't been registered in this"
                 f" operator registry '{self.name}'"
@@ -233,14 +262,21 @@
         else:
             implementation_store.add_implementation(op_impl)
 
     def get_implementation(self, name, args_signature) -> TypedOperatorImpl:
         if name not in self.ALL_REGISTERED_OPS:
             raise ValueError(f"No operator named '{name}'.")
 
+        for dtype in args_signature:
+            if not isinstance(dtype, dtypes.DType):
+                raise TypeError(
+                    "Expected elements of `args_signature` to be of type DType,"
+                    f" but found element of type {type(dtype).__name__} instead."
+                )
+
         if store := self.implementations.get(name):
             if impl := store.find_best_match(args_signature):
                 return impl
 
         # If operation hasn't been defined in this registry, go to the parent
         # registry and check if it has been defined there.
         if self.super_registry is None or not self.check_super.get(name, True):
@@ -252,19 +288,20 @@
 
 
 class OperatorSignature:
     """
     Specification:
 
         signature ::= arguments "->" rtype
-        arguments ::= (dtype ",")* terminal_arg
-        terminal_arg ::= dtype | vararg
+        arguments ::= (modifiers dtype ",")* terminal_arg
+        terminal_arg ::= modifiers (dtype | vararg)
         vararg ::= dtype "..."
         rtype ::= dtype
         dtype ::= template | "int" | "float" | "str" | "bool" | and others...
+        modifiers ::= "const"?
         template ::= single uppercase character
 
     Examples:
 
         Function that takes two integers and returns an integer:
             int, int -> int
 
@@ -273,29 +310,29 @@
             T, U -> bool
 
         Variable number of arguments:
             int... -> int
 
     """
 
-    def __init__(self, args: tuple[str], rtype: str):
+    def __init__(self, args: list[dtypes.DType], rtype: dtypes.DType):
         """
         :param args: Tuple of argument types.
         :param rtype: The return type.
         """
         self.args = args
         self.rtype = rtype
 
     @classmethod
     def parse(cls, signature: str) -> OperatorSignature:
         def parse_cstypes(cst: str):
             # cstypes = comma seperated types
             types = cst.split(",")
             types = [t.strip() for t in types]
-            types = [t for t in types if t]
+            types = [dtypes.dtype_from_string(t) for t in types if t]
             return types
 
         if "->" not in signature:
             raise ValueError("Invalid signature: arrow (->) missing.")
 
         arg_sig, r_sig = signature.split("->")
         args = parse_cstypes(arg_sig)
@@ -306,251 +343,269 @@
             raise ValueError(
                 f"Invalid operator signature '{signature}'. Expected exactly one return"
                 " type."
             )
 
         rtype = rtype[0]
 
-        base_args_types = [get_base_type(arg) for arg in args]
-        base_rtype = get_base_type(rtype)
-
-        for type in (*base_args_types, base_rtype):
-            if not type.isalnum():
-                raise ValueError(f"Invalid type '{type}'. Types must be alphanumeric.")
-
         # Validate Template
         # Output template must also occur in signature
-
-        if is_template_type(base_rtype):
-            if base_rtype not in base_args_types:
+        if isinstance(rtype, dtypes.Template):
+            if rtype.name not in [arg.name for arg in args]:
                 raise ValueError(
-                    f"Template return type '{base_rtype}' must also occur in the"
+                    f"Template return type '{rtype}' must also occur in the"
                     " argument signature."
                 )
 
         # Validate vararg
         # Vararg can only occur for the very last element
-
         for arg in args[:-1]:
-            if arg.endswith("..."):
-                raise ValueError(f"Only last argument can be a vararg.")
+            if arg.vararg:
+                raise ValueError("Only last argument can be a vararg.")
 
-        if rtype.endswith("..."):
-            raise ValueError(f"Return value can't be a vararg.")
+        if rtype.vararg:
+            raise ValueError("Return value can't be a vararg.")
 
         return OperatorSignature(
-            args=tuple(args),
+            args=args,
             rtype=rtype,
         )
 
     def __repr__(self):
-        return f"{ ', '.join(self.args)} -> {self.rtype}"
+        args_str = ", ".join(str(arg) for arg in self.args)
+        return args_str + " -> " + str(self.rtype)
 
     def __hash__(self):
         return hash((self.args, self.rtype))
 
     def __eq__(self, other):
         if not isinstance(other, OperatorSignature):
             return False
         return self.args == other.args and self.rtype == other.rtype
 
     @property
     def is_vararg(self) -> bool:
         if len(self.args) == 0:
             return False
-        return is_vararg_type(self.args[-1])
-
-
-def is_template_type(s: str) -> bool:
-    # Singe upper case ASCII character
-    return len(s) == 1 and 65 <= ord(s) <= 90
-
-
-def is_vararg_type(s: str) -> bool:
-    return s.endswith("...")
-
-
-def get_base_type(s: str) -> str:
-    """Get base type from imput string without any decorators.
-    -> Trims varargs ellipsis (...) from input.
-    """
-    if s.endswith("..."):
-        return s[:-3]
-    return s
+        return self.args[-1].vararg
 
 
 class OperatorImplementationStore:
     """
     Stores all implementations for a specific operation in a trie according to
     their signature. This enables us to easily find the best matching
     operator implementation for a given set of input argument types.
     """
 
     @dataclasses.dataclass
     class TrieNode:
-        __slots__ = ("value", "operator", "children", "is_vararg")
-        value: str
+        __slots__ = ("value", "operator", "children")
+        value: dtypes.DType
         operator: OperatorImpl | None
         children: list[OperatorImplementationStore.TrieNode]
-        is_vararg: bool
+
+        def __repr__(self):
+            self_text = f"({self.value} - {self.operator})"
+            if self.children:
+                children_text = "\n".join(repr(c) for c in self.children)
+                children_text = textwrap.indent(children_text, "  ")
+                return self_text + "\n" + children_text
+            return self_text
 
     def __init__(self, operator: Operator):
         self.operator = operator
-        self.root = self.TrieNode("ROOT", None, [], False)
+        self.root = self.TrieNode("ROOT", None, [])  # type: ignore
 
     def add_implementation(self, operator: OperatorImpl):
         node = self.get_node(operator.signature, create_missing=True)
         if node.operator is not None:
             raise ValueError(
                 f"Implementation for signature {operator.signature} already defined."
             )
 
         node.operator = operator
-        node.is_vararg |= operator.signature.is_vararg
 
     def add_variant(self, name: str, operator: OperatorImpl):
         node = self.get_node(operator.signature, create_missing=False)
         if node is None or node.operator is None:
             raise ValueError(
                 f"No implementation for signature {operator.signature} found."
                 " Make sure there is an exact match to add a variant."
             )
 
-        assert node.operator.signature.rtype == operator.signature.rtype
+        assert node.operator.signature.rtype.same_kind(operator.signature.rtype)
         node.operator.add_variant(name, operator.impl)
 
     def get_node(self, signature: OperatorSignature, create_missing: bool = True):
         node = self.root
         for dtype in signature.args:
-            dtype = get_base_type(dtype)
             for child in node.children:
-                if dtype == child.value:
+                if child.value == dtype:
                     node = child
                     break
             else:
                 if create_missing:
-                    new_node = self.TrieNode(dtype, None, [], False)
+                    new_node = self.TrieNode(dtype, None, [])
                     node.children.append(new_node)
                     node = new_node
                 else:
                     return None
 
         return node
 
-    def find_best_match(self, signature: tuple[str]) -> TypedOperatorImpl | None:
+    def find_best_match(
+        self, signature: tuple[dtypes.DType]
+    ) -> TypedOperatorImpl | None:
         matches = list(self._find_matches(signature))
 
         if not matches:
             return None
 
         # Find best matching template.
         best_match = None
-        best_score = (0xFFFF,)
+        best_score = ((0x7FFFFFFF,), (0x7FFFFFFF,))
 
-        for match, templates in matches:
-            if match.operator._precedence < best_score:
+        for match, templates, type_promotion_indices in matches:
+            score = (
+                # Prefer operators that didn't need any type promotion
+                tuple(-i for i in type_promotion_indices),
+                # And then match according to signature
+                match.operator._precedence,
+            )
+            if score < best_score:
                 best_match = (match, templates)
-                best_score = match.operator._precedence
+                best_score = score
 
         rtype = best_match[0].operator.signature.rtype
-        rtype = best_match[1].get(rtype, rtype)  # If it is a template -> Translate
+        if isinstance(rtype, dtypes.Template):
+            # If rtype is a template -> Translate
+            rtype = best_match[1][rtype.name]
 
         return TypedOperatorImpl.from_operator_impl(best_match[0].operator, rtype)
 
-    def _find_matches(self, signature: tuple[str]):
+    def _find_matches(
+        self, signature: tuple[dtypes.DType]
+    ) -> Iterable[TrieNode, dict[str, dtypes.DType, tuple[int, ...]]]:
         """Yield all operators that match the input signature"""
 
         # Case 0 arguments:
         if len(signature) == 0:
-            yield (self.root, dict())
+            yield self.root, dict(), tuple()
             return
 
         # Case 1+ args:
-
         def does_match(
-            dtype: str,
+            dtype: dtypes.DType,
             node: OperatorImplementationStore.TrieNode,
-            templates: dict[str, str],
         ) -> bool:
-            if is_template_type(node.value):
-                t = templates.get(node.value)
-                return t is None or dtype == t
-            return dtype == node.value
-
-        # Store tuple of (Node, index in signature, templates)
-        stack = [(child, 0, dict()) for child in self.root.children]
+            if isinstance(node.value, dtypes.Template):
+                return node.value.modifiers_compatible(dtype)
+            return dtype.can_promote_to(node.value)
+
+        stack: list[
+            tuple[OperatorImplementationStore.TrieNode, int, dict, tuple[int, ...]]
+        ] = [(child, 0, dict(), tuple()) for child in self.root.children]
 
         while stack:
-            node, s_i, templates = stack.pop()
+            node, s_i, templates, type_promotion_indices = stack.pop()
             dtype = signature[s_i]
 
-            if not does_match(dtype, node, templates):
+            if not does_match(dtype, node):
                 continue
 
-            if is_template_type(node.value) and node.value not in templates:
-                # Insert dtype into templates dict
+            if isinstance(node.value, dtypes.Template):
                 templates = templates.copy()
-                templates[node.value] = dtype
+                if node.value.name not in templates:
+                    templates[node.value.name] = [dtype.without_modifiers()]
+                else:
+                    templates[node.value.name] = templates[node.value.name] + [
+                        dtype.without_modifiers()
+                    ]
+            elif not node.value.same_kind(dtype):
+                # Needs type promotion
+                # This only works when types can be promoted once
+                # -> (uint > int) wouldn't be preferred over (uint > int > float)
+                type_promotion_indices = (*type_promotion_indices, s_i)
 
             if s_i + 1 == len(signature):
                 if node.operator is not None:
-                    yield (node, templates)
+                    # Find compatible type for templates
+                    try:
+                        templates = {
+                            name: dtypes.promote_dtypes(types_)
+                            for name, types_ in templates.items()
+                        }
+                        yield node, templates, type_promotion_indices
+                    except ExpressionTypeError:
+                        print(f"Can't promote: {templates}")
+                        pass
+
                 continue
 
             children = iter(node.children)
-            if node.is_vararg:
+            if node.value.vararg:
                 children = itertools.chain(children, iter((node,)))
 
             for child in children:
-                stack.append((child, s_i + 1, templates))
+                stack.append((child, s_i + 1, templates, type_promotion_indices))
 
 
 class OperatorRegistrationContextManager:
     def __init__(
         self,
         registry: OperatorRegistry,
         operator: Operator,
-        # Options
+        *,
         check_super=True,
     ):
         self.registry = registry
         self.operator = operator
 
         self.registry.register_op(operator, check_super=check_super)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         pass
 
-    def __call__(self, signature: str, variant: str = None):
+    def __call__(self, signature: str, *, variant: str = None):
         if not isinstance(signature, str):
-            raise TypeError(f"Signature must be of type str.")
+            raise TypeError("Signature must be of type str.")
 
         def decorator(func):
-            self.registry.add_implementation(self.operator, func, signature, variant)
+            self.registry.add_implementation(
+                self.operator,
+                func,
+                signature,
+                variant,
+            )
             return func
 
         return decorator
 
-    def auto(self, func=None, *, variant: str = None):
+    def auto(self, func: Callable = None, *, variant: str = None):
         if func is None:
             return partial(self.auto, variant=variant)
 
         if not self.operator.signatures:
             raise ValueError(f"Operator {self.operator} has not default signatures.")
 
-        for sig in self.operator.signatures:
-            self.registry.add_implementation(self.operator, func, sig, variant)
+        for signature in self.operator.signatures:
+            self.registry.add_implementation(
+                self.operator,
+                func,
+                signature,
+                variant,
+            )
 
         return func
 
     def extension(self, extension: type[OperatorExtension], variant: str = None):
-        if extension.operator != type(self.operator):
+        if extension.operator != type(self.operator):  # noqa: E721
             raise ValueError(
                 f"Operator extension for '{extension.operator.__name__}' can't "
                 f"be applied to operator of type '{type(self.operator).__name__}'."
             )
 
         def decorator(func):
             for sig in extension.signatures:
```

### Comparing `pydiverse_transform-0.1.3/src/pydiverse/transform/core/table.py` & `pydiverse_transform-0.1.4/src/pydiverse/transform/core/table.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
-from html import escape
-from typing import Generic, TypeVar
 from collections.abc import Iterable
+from html import escape
+from typing import Generic
 
-from pydiverse.transform.core import verbs
-from pydiverse.transform.core.column import Column, LambdaColumn
-from pydiverse.transform.core.expressions import SymbolicExpression
-from pydiverse.transform.core.table_impl import AbstractTableImpl
-
-ImplT = TypeVar("ImplT", bound=AbstractTableImpl)
+from pydiverse.transform._typing import ImplT
+from pydiverse.transform.core.expressions import (
+    Column,
+    LambdaColumn,
+    SymbolicExpression,
+)
 
 
 class Table(Generic[ImplT]):
     """
     All attributes of a table are columns except for the `_impl` attribute
     which is a reference to the underlying table implementation.
     """
@@ -26,28 +26,30 @@
             key = key._
         return SymbolicExpression(self._impl.get_col(key))
 
     def __setitem__(self, col, expr):
         """Mutate a column
         :param col: Either a str or SymbolicColumn
         """
+        from pydiverse.transform.core.verbs import mutate
+
         col_name = None
 
         if isinstance(col, SymbolicExpression):
             underlying = col._
             if isinstance(underlying, (Column, LambdaColumn)):
                 col_name = underlying.name
         elif isinstance(col, str):
             col_name = col
 
         if not col_name:
             raise KeyError(
                 f"Invalid key {col}. Must be either a string, Column or LambdaColumn."
             )
-        self._impl = (self >> verbs.mutate(**{col_name: expr}))._impl
+        self._impl = (self >> mutate(**{col_name: expr}))._impl
 
     def __getattr__(self, name) -> SymbolicExpression[Column]:
         return SymbolicExpression(self._impl.get_col(name))
 
     def __iter__(self) -> Iterable[SymbolicExpression[Column]]:
         # Capture current state (this allows modifying the table inside a loop)
         cols = [
@@ -78,34 +80,38 @@
         return False
 
     def __copy__(self):
         impl_copy = self._impl.copy()
         return self.__class__(impl_copy)
 
     def __str__(self):
+        from pydiverse.transform.core.verbs import collect
+
         try:
             return (
                 f"Table: {self._impl.name}, backend: {type(self._impl).__name__}\n"
-                f"{self >> verbs.collect()}"
+                f"{self >> collect()}"
             )
         except Exception as e:
             return (
                 f"Table: {self._impl.name}, backend: {type(self._impl).__name__}\n"
                 "Failed to collect table due to an exception:\n"
                 f"{type(e).__name__}: {str(e)}"
             )
 
     def _repr_html_(self) -> str | None:
+        from pydiverse.transform.core.verbs import collect
+
         html = (
             f"Table <code>{self._impl.name}</code> using"
             f" <code>{type(self._impl).__name__}</code> backend:</br>"
         )
         try:
             # TODO: For lazy backend only show preview (eg. take first 20 rows)
-            html += (self >> verbs.collect())._repr_html_()
+            html += (self >> collect())._repr_html_()
         except Exception as e:
             html += (
                 "</br><pre>Failed to collect table due to an exception:\n"
                 f"{escape(e.__class__.__name__)}: {escape(str(e))}</pre>"
             )
         return html
```

### Comparing `pydiverse_transform-0.1.3/src/pydiverse/transform/core/table_impl.py` & `pydiverse_transform-0.1.4/src/pydiverse/transform/core/table_impl.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,49 @@
 from __future__ import annotations
 
 import copy
 import dataclasses
+import datetime
 import uuid
 import warnings
-from typing import TYPE_CHECKING, Any, Callable, Generic, TypeVar
 from collections.abc import Iterable
+from typing import TYPE_CHECKING, Any, Callable, Generic, TypeVar
 
-from pydiverse.transform.core.ops.registry import (
+from pydiverse.transform import ops
+from pydiverse.transform._typing import ImplT
+from pydiverse.transform.core import dtypes
+from pydiverse.transform.core.expressions import (
+    CaseExpression,
+    Column,
+    LambdaColumn,
+    LiteralColumn,
+)
+from pydiverse.transform.core.expressions.translator import (
+    DelegatingTranslator,
+    Translator,
+    TypedValue,
+)
+from pydiverse.transform.core.registry import (
     OperatorRegistrationContextManager,
     OperatorRegistry,
 )
 from pydiverse.transform.core.util import bidict, ordered_set
-
-from .column import Column, LambdaColumn, LiteralColumn
-from .expressions.translator import DelegatingTranslator, Translator, TypedValue
-from .ops import Operator, OPType
-from .util import OrderingDescriptor
+from pydiverse.transform.errors import ExpressionTypeError, FunctionTypeError
+from pydiverse.transform.ops import OPType
 
 if TYPE_CHECKING:
-    # noinspection PyUnresolvedReferences
-    from pydiverse.transform.core.expressions import SymbolicExpression
-
+    from pydiverse.transform.core.util import OrderingDescriptor
+    from pydiverse.transform.ops import Operator
 
-class _TableImplMeta(type):
-    """
-    Metaclass that adds an appropriate operator_registry attribute to each class
-    in the table implementation class hierarchy.
-    """
-
-    def __new__(cls, name, bases, attrs, **kwargs):
-        c = super().__new__(cls, name, bases, attrs, **kwargs)
-
-        # By using `super` to get the super_registry, we can check for potential
-        # operation definitions in order of the MRO.
-        super_reg = (
-            super(c, c).operator_registry
-            if hasattr(super(c, c), "operator_registry")
-            else None
-        )
-        setattr(c, "operator_registry", OperatorRegistry(name, super_reg))
-        return c
 
-
-ImplT = TypeVar("ImplT", bound="AbstractTableImpl")
 ExprCompT = TypeVar("ExprCompT", bound="TypedValue")
 AlignedT = TypeVar("AlignedT", bound="TypedValue")
 
 
-class AbstractTableImpl(metaclass=_TableImplMeta):
+class AbstractTableImpl:
     """
     Base class from which all table backend implementations are derived from.
     It tracks various metadata that is relevant for all backends.
 
     Attributes:
         name: The name of the table.
 
@@ -71,15 +62,15 @@
 
         grouped_by: Ordered set of columns by which the table is grouped by.
         intrinsic_grouped_by: Ordered set of columns representing the underlying
             grouping level of the table. This gets set when performing a
             summarising operation.
     """
 
-    operator_registry: OperatorRegistry
+    operator_registry = OperatorRegistry("AbstractTableImpl")
 
     def __init__(
         self,
         name: str,
         columns: dict[str, Column],
     ):
         self.name = name
@@ -97,14 +88,27 @@
         # Init Values
         for name, col in columns.items():
             self.selects.add(name)
             self.named_cols.fwd[name] = col.uuid
             self.available_cols.add(col.uuid)
             self.cols[col.uuid] = ColumnMetaData.from_expr(col.uuid, col, self)
 
+    def __init_subclass__(cls, **kwargs):
+        super().__init_subclass__(**kwargs)
+
+        # Add new `operator_registry` class variable to subclass.
+        # We define the super registry by walking up the MRO. This allows us
+        # to check for potential operation definitions in the parent classes.
+        super_reg = None
+        for super_cls in cls.__mro__:
+            if hasattr(super_cls, "operator_registry"):
+                super_reg = super_cls.operator_registry
+                break
+        cls.operator_registry = OperatorRegistry(cls.__name__, super_reg)
+
     def copy(self):
         c = copy.copy(self)
         # Copy containers
         for k, v in self.__dict__.items():
             if isinstance(v, (list, dict, set, bidict, ordered_set)):
                 c.__dict__[k] = copy.copy(v)
 
@@ -118,15 +122,15 @@
 
         if isinstance(key, LambdaColumn):
             key = key.name
 
         if isinstance(key, str):
             if uuid := self.named_cols.fwd.get(key, None):
                 return self.cols[uuid].as_column(key, self)
-            # Must return AttributeError, else `hasattr` doesn't work on Table instances.
+            # Must return AttributeError, else `hasattr` doesn't work on Table instances
             raise AttributeError(f"Table '{self.name}' has not column named '{key}'.")
 
         if isinstance(key, Column):
             uuid = key.uuid
             if uuid in self.available_cols:
                 name = self.named_cols.bwd[uuid]
                 return self.cols[uuid].as_column(name, self)
@@ -214,57 +218,135 @@
         return OperatorRegistrationContextManager(
             cls.operator_registry, operator, **kwargs
         )
 
     #### Expressions ####
 
     class ExpressionCompiler(
-        Generic[ImplT, ExprCompT], DelegatingTranslator[ExprCompT]
+        DelegatingTranslator[ExprCompT], Generic[ImplT, ExprCompT]
     ):
         """
         Class convert an expression into a function that, when provided with
         the appropriate arguments, evaluates the expression.
 
         The reason we can't just eagerly evaluate the expression is because for
         grouped data we often have to use the split-apply-combine strategy.
         """
 
         def __init__(self, backend: ImplT):
             self.backend = backend
             super().__init__(backend.operator_registry)
 
         def _translate_literal(self, expr, **kwargs):
-            def literal_func(*args, **kwargs):
-                return expr
+            literal = self._translate_literal_value(expr)
 
+            if isinstance(expr, bool):
+                return TypedValue(literal, dtypes.Bool(const=True))
             if isinstance(expr, int):
-                return TypedValue(literal_func, "int")
+                return TypedValue(literal, dtypes.Int(const=True))
             if isinstance(expr, float):
-                return TypedValue(literal_func, "float")
+                return TypedValue(literal, dtypes.Float(const=True))
             if isinstance(expr, str):
-                return TypedValue(literal_func, "str")
-            if isinstance(expr, bool):
-                return TypedValue(literal_func, "bool")
+                return TypedValue(literal, dtypes.String(const=True))
+            if isinstance(expr, datetime.datetime):
+                return TypedValue(literal, dtypes.DateTime(const=True))
+
+            if expr is None:
+                return TypedValue(literal, dtypes.NoneDType(const=True))
+
+        def _translate_literal_value(self, expr):
+            def literal_func(*args, **kwargs):
+                return expr
 
-    class AlignedExpressionEvaluator(Generic[AlignedT], DelegatingTranslator[AlignedT]):
+            return literal_func
+
+        def _translate_case_common(
+            self,
+            expr: CaseExpression,
+            switching_on: ExprCompT | None,
+            cases: list[tuple[ExprCompT, ExprCompT]],
+            default: ExprCompT,
+            **kwargs,
+        ) -> tuple[dtypes.DType, OPType]:
+            # Determine dtype of result
+            val_dtypes = [default.dtype.without_modifiers()]
+            for _, val in cases:
+                val_dtypes.append(val.dtype.without_modifiers())
+
+            result_dtype = dtypes.promote_dtypes(val_dtypes)
+
+            # Determine ftype of result
+            val_ftypes = set()
+            if not default.dtype.const:
+                val_ftypes.add(default.ftype)
+
+            for _, val in cases:
+                if not val.dtype.const:
+                    val_ftypes.add(val.ftype)
+
+            if len(val_ftypes) == 0:
+                result_ftype = OPType.EWISE
+            elif len(val_ftypes) == 1:
+                (result_ftype,) = val_ftypes
+            elif OPType.WINDOW in val_ftypes:
+                result_ftype = OPType.WINDOW
+            else:
+                # AGGREGATE and EWISE are incompatible
+                raise FunctionTypeError(
+                    "Incompatible function types found in case statement: "
+                    ", ".join(val_ftypes)
+                )
+
+            if result_ftype is OPType.EWISE and switching_on is not None:
+                result_ftype = switching_on.ftype
+
+            # Type check conditions
+            if switching_on is None:
+                # All conditions must be boolean
+                for cond, _ in cases:
+                    if not dtypes.Bool().same_kind(cond.dtype):
+                        raise ExpressionTypeError(
+                            "All conditions in a case statement return booleans. "
+                            f"{cond} is of type {cond.dtype}."
+                        )
+            else:
+                # All conditions must be of the same type as switching_on
+                for cond, _ in cases:
+                    if not cond.dtype.can_promote_to(
+                        switching_on.dtype.without_modifiers()
+                    ):
+                        # Can't compare
+                        raise ExpressionTypeError(
+                            f"Condition value {cond} (dtype: {cond.dtype}) "
+                            f"is incompatible with switch dtype {switching_on.dtype}."
+                        )
+
+            return result_dtype, result_ftype
+
+    class AlignedExpressionEvaluator(DelegatingTranslator[AlignedT], Generic[AlignedT]):
         """
         Used for evaluating an expression in a typical eager style where, as
         long as two columns have the same alignment / length, we can perform
         operations on them without first having to join them.
         """
 
         def _translate_literal(self, expr, **kwargs):
+            if isinstance(expr, bool):
+                return TypedValue(expr, dtypes.Bool(const=True))
             if isinstance(expr, int):
-                return TypedValue(expr, "int")
+                return TypedValue(expr, dtypes.Int(const=True))
             if isinstance(expr, float):
-                return TypedValue(expr, "float")
+                return TypedValue(expr, dtypes.Float(const=True))
             if isinstance(expr, str):
-                return TypedValue(expr, "str")
-            if isinstance(expr, bool):
-                return TypedValue(expr, "bool")
+                return TypedValue(expr, dtypes.String(const=True))
+            if isinstance(expr, datetime.datetime):
+                return TypedValue(expr, dtypes.DateTime(const=True))
+
+            if expr is None:
+                return TypedValue(expr, dtypes.NoneDType(const=True))
 
     class LambdaTranslator(Translator):
         """
         Translator that takes an expression and replaces all LambdaColumns
         inside it with the corresponding Column instance.
         """
 
@@ -273,16 +355,16 @@
             super().__init__()
 
         def _translate(self, expr, **kwargs):
             # Resolve lambda and return Column object
             if isinstance(expr, LambdaColumn):
                 if expr.name not in self.backend.named_cols.fwd:
                     raise ValueError(
-                        f"Invalid lambda column '{expr.name}. No column with this name"
-                        f" found for table '{self.backend.name}'.'"
+                        f"Invalid lambda column '{expr.name}'. No column with this name"
+                        f" found for table '{self.backend.name}'."
                     )
                 uuid = self.backend.named_cols.fwd[expr.name]
                 return self.backend.cols[uuid].as_column(expr.name, self.backend)
             return expr
 
     #### Helpers ####
 
@@ -310,76 +392,91 @@
             if OPType.AGGREGATE in ftypes:
                 return OPType.AGGREGATE
             return op_ftype
 
         if op_ftype == OPType.AGGREGATE:
             if OPType.WINDOW in ftypes:
                 if strict:
-                    raise ValueError(
+                    raise FunctionTypeError(
                         "Can't nest a window function inside an aggregate function"
                         f" ({operator.name})."
                     )
                 else:
                     # TODO: Replace with logger
                     warnings.warn(
-                        f"Nesting a window function inside an aggregate function is not"
-                        f" supported by SQL backend."
+                        "Nesting a window function inside an aggregate function is not"
+                        " supported by SQL backend."
                     )
             if OPType.AGGREGATE in ftypes:
-                raise ValueError(
+                raise FunctionTypeError(
                     "Can't nest an aggregate function inside an aggregate function"
                     f" ({operator.name})."
                 )
             return op_ftype
 
         if op_ftype == OPType.WINDOW:
             if OPType.WINDOW in ftypes:
                 if strict:
-                    raise ValueError(
+                    raise FunctionTypeError(
                         "Can't nest a window function inside a window function"
                         f" ({operator.name})."
                     )
                 else:
                     warnings.warn(
-                        f"Nesting a window function inside a window function is not"
-                        f" supported by SQL backend."
+                        "Nesting a window function inside a window function is not"
+                        " supported by SQL backend."
                     )
             return op_ftype
 
 
 @dataclasses.dataclass
 class ColumnMetaData:
     uuid: uuid.UUID
     expr: Any
     compiled: Callable[[Any], TypedValue]
-    dtype: str
-    ftype: str
+    dtype: dtypes.DType
+    ftype: OPType
 
     @classmethod
     def from_expr(cls, uuid, expr, table: AbstractTableImpl, **kwargs):
         v = table.compiler.translate(expr, **kwargs)
         return cls(
             uuid=uuid,
             expr=expr,
             compiled=v.value,
-            dtype=v.dtype,
+            dtype=v.dtype.without_modifiers(),
             ftype=v.ftype,
         )
 
     def __hash__(self):
         return hash(self.uuid)
 
     def as_column(self, name, table: AbstractTableImpl):
         return Column(name, table, self.dtype, self.uuid)
 
 
-#### ARITHMETIC OPERATORS ######################################################
+#### MARKER OPERATIONS #########################################################
+
+
+with AbstractTableImpl.op(ops.NullsFirst()) as op:
+
+    @op.auto
+    def _nulls_first(_):
+        raise RuntimeError("This is just a marker that never should get called")
+
 
+with AbstractTableImpl.op(ops.NullsLast()) as op:
+
+    @op.auto
+    def _nulls_last(_):
+        raise RuntimeError("This is just a marker that never should get called")
+
+
+#### ARITHMETIC OPERATORS ######################################################
 
-from pydiverse.transform.core import ops
 
 with AbstractTableImpl.op(ops.Add()) as op:
 
     @op.auto
     def _add(lhs, rhs):
         return lhs + rhs
```

### Comparing `pydiverse_transform-0.1.3/src/pydiverse/transform/core/util/bidict.py` & `pydiverse_transform-0.1.4/src/pydiverse/transform/core/util/bidict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
-from typing import (
-    Generic,
-    TypeVar,
-)
 from collections.abc import (
     ItemsView,
     Iterable,
     KeysView,
     Mapping,
     MutableMapping,
     ValuesView,
 )
+from typing import (
+    Generic,
+    TypeVar,
+)
 
 KT = TypeVar("KT")
 VT = TypeVar("VT")
 
 
 class bidict(Generic[KT, VT]):
     """
@@ -32,16 +32,16 @@
             self.__bwd = bwd
         else:
             self.__fwd = dict(seq) if seq is not None else dict()
             self.__bwd = {v: k for k, v in self.__fwd.items()}
 
         if len(self.__fwd) != len(self.__bwd) != len(seq):
             raise ValueError(
-                f"Input sequence contains duplicate key value pairs. Mapping must be"
-                f" unique."
+                "Input sequence contains duplicate key value pairs. Mapping must be"
+                " unique."
             )
 
         self.fwd = _BidictInterface(
             self.__fwd, self.__bwd
         )  # type: _BidictInterface[KT, VT]
         self.bwd = _BidictInterface(
             self.__bwd, self.__fwd
```

### Comparing `pydiverse_transform-0.1.3/src/pydiverse/transform/core/util/ordered_set.py` & `pydiverse_transform-0.1.4/src/pydiverse/transform/core/util/ordered_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
-from typing import TypeVar
 from collections.abc import Iterable, MutableSet
 
-T = TypeVar("T")
+from pydiverse.transform._typing import T
 
 
 class ordered_set(MutableSet[T]):
     def __init__(self, values: Iterable[T] = tuple()):
         self.__data = {v: None for v in values}
 
     def __contains__(self, item: T) -> bool:
```

### Comparing `pydiverse_transform-0.1.3/src/pydiverse/transform/core/util/util.py` & `pydiverse_transform-0.1.4/src/pydiverse/transform/core/util/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from __future__ import annotations
 
 import typing
 from dataclasses import dataclass
 
-from pydiverse.transform.core import column
-from pydiverse.transform.core.expressions import expressions
+from pydiverse.transform._typing import T
+from pydiverse.transform.core.expressions import FunctionCall
 
 __all__ = (
     "traverse",
     "sign_peeler",
     "OrderingDescriptor",
     "translate_ordering",
 )
 
-T = typing.TypeVar("T")
-
 
 def traverse(obj: T, callback: typing.Callable) -> T:
     if isinstance(obj, list):
         return [traverse(elem, callback) for elem in obj]
     if isinstance(obj, dict):
         return {k: traverse(v, callback) for k, v in obj.items()}
     if isinstance(obj, tuple):
@@ -26,30 +24,54 @@
             # Named tuples cause problems
             raise Exception
         return tuple(traverse(elem, callback) for elem in obj)
 
     return callback(obj)
 
 
-def sign_peeler(expr):
-    """Remove unary - and + prefix and return the sign
-    :return: `True` for `+` and `False` for `-`
-    """
-    num_neg = 0
-    while isinstance(expr, expressions.FunctionCall):
-        if expr.name == "__neg__":
-            num_neg += 1
-            expr = expr.args[0]
-        elif expr.name == "__pos__":
+def peel_markers(expr, markers):
+    found_markers = []
+    while isinstance(expr, FunctionCall):
+        if expr.name in markers:
+            found_markers.append(expr.name)
+            assert len(expr.args) == 1
             expr = expr.args[0]
         else:
             break
+    return expr, found_markers
+
+
+def sign_peeler(expr):
+    """
+    Remove unary - and + prefix and return the sign
+    :return: `True` for `+` and `False` for `-`
+    """
+
+    expr, markers = peel_markers(expr, {"__neg__", "__pos__"})
+    num_neg = markers.count("__neg__")
     return expr, num_neg % 2 == 0
 
 
+def ordering_peeler(expr):
+    expr, markers = peel_markers(
+        expr, {"__neg__", "__pos__", "nulls_first", "nulls_last"}
+    )
+
+    ascending = markers.count("__neg__") % 2 == 0
+    nulls_first = False
+    for marker in markers:
+        if marker == "nulls_first":
+            nulls_first = True
+            break
+        if marker == "nulls_last":
+            break
+
+    return expr, ascending, nulls_first
+
+
 ####
 
 
 @dataclass
 class OrderingDescriptor:
     __slots__ = ("order", "asc", "nulls_first")
 
@@ -57,17 +79,12 @@
     asc: bool
     nulls_first: bool
 
 
 def translate_ordering(tbl, order_list) -> list[OrderingDescriptor]:
     ordering = []
     for arg in order_list:
-        col, ascending = sign_peeler(arg)
-        if not isinstance(col, (column.Column, column.LambdaColumn)):
-            raise ValueError(
-                "Arguments to arrange must be of type 'Column' or 'LambdaColumn' and"
-                f" not '{type(col)}'."
-            )
+        col, ascending, nulls_first = ordering_peeler(arg)
         col = tbl.resolve_lambda_cols(col)
-        ordering.append(OrderingDescriptor(col, ascending, False))
+        ordering.append(OrderingDescriptor(col, ascending, nulls_first))
 
     return ordering
```

### Comparing `pydiverse_transform-0.1.3/src/pydiverse/transform/core/verbs.py` & `pydiverse_transform-0.1.4/src/pydiverse/transform/core/verbs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 from __future__ import annotations
 
 import functools
 from collections import ChainMap
-from typing import Dict
 from collections.abc import Iterable
+from typing import Literal
 
-from .column import Column, LambdaColumn, generate_col_uuid
-from .dispatchers import builtin_verb
-from .expressions import SymbolicExpression
-from .expressions.util import iterate_over_expr
-from .table_impl import AbstractTableImpl, ColumnMetaData
-from .util import bidict, ordered_set, sign_peeler, translate_ordering
+from pydiverse.transform.core import dtypes
+from pydiverse.transform.core.dispatchers import builtin_verb
+from pydiverse.transform.core.expressions import (
+    Column,
+    LambdaColumn,
+    SymbolicExpression,
+)
+from pydiverse.transform.core.expressions.util import iterate_over_expr
+from pydiverse.transform.core.table_impl import AbstractTableImpl, ColumnMetaData
+from pydiverse.transform.core.util import (
+    bidict,
+    ordered_set,
+    sign_peeler,
+    translate_ordering,
+)
+from pydiverse.transform.errors import ExpressionTypeError, FunctionTypeError
+from pydiverse.transform.ops import OPType
 
 __all__ = [
     "alias",
     "collect",
     "build_query",
     "show_query",
     "select",
@@ -53,17 +64,17 @@
         )
 
 
 def check_lambdas_valid(tbl: AbstractTableImpl, *expressions):
     lambdas = []
     for expression in expressions:
         lambdas.extend(
-            l for l in iterate_over_expr(expression) if isinstance(l, LambdaColumn)
+            lc for lc in iterate_over_expr(expression) if isinstance(lc, LambdaColumn)
         )
-    missing_lambdas = {l for l in lambdas if l.name not in tbl.named_cols.fwd}
+    missing_lambdas = {lc for lc in lambdas if lc.name not in tbl.named_cols.fwd}
     if missing_lambdas:
         missing_lambdas_str = ", ".join(map(lambda x: str(x), missing_lambdas))
         raise ValueError(f"Invalid lambda column(s) {missing_lambdas_str}.")
 
 
 def cols_in_expression(expression) -> set[Column]:
     return {c for c in iterate_over_expr(expression) if isinstance(c, Column)}
@@ -77,15 +88,15 @@
 
 def validate_table_args(*tables):
     if len(tables) == 0:
         return
 
     for table in tables:
         if not isinstance(table, AbstractTableImpl):
-            raise ValueError(f"Expected a TableImpl but got {type(table)} instead.")
+            raise TypeError(f"Expected a TableImpl but got {type(table)} instead.")
 
     backend = type(tables[0])
     for table in tables:
         if type(table) != backend:
             raise ValueError(
                 f"Can't mix tables with different backends. Expected '{backend}' but"
                 f" found '{type(table)}'."
@@ -184,15 +195,15 @@
         if not isinstance(k, str) or not isinstance(v, str):
             raise TypeError(
                 f"Key and Value of `name_map` must both be strings: ({k!r}, {v!r})"
             )
 
     # Reference col that doesn't exist
     if missing_cols := name_map.keys() - tbl.named_cols.fwd.keys():
-        raise KeyError(f"Table has no columns named: " + ", ".join(missing_cols))
+        raise KeyError("Table has no columns named: " + ", ".join(missing_cols))
 
     # Can't rename two cols to the same name
     _seen = set()
     if duplicate_names := {
         name for name in name_map.values() if name in _seen or _seen.add(name)
     }:
         raise ValueError(
@@ -226,37 +237,44 @@
     check_cols_available(tbl, cols_in_expressions(kwargs.values()), "mutate")
 
     new_tbl = tbl.copy()
     new_tbl.preverb_hook("mutate", **kwargs)
     kwargs = {k: new_tbl.resolve_lambda_cols(v) for k, v in kwargs.items()}
 
     for name, expr in kwargs.items():
-        uid = generate_col_uuid()
+        uid = Column.generate_col_uuid()
+        col = ColumnMetaData.from_expr(uid, expr, new_tbl, verb="mutate")
+
+        if dtypes.NoneDType().same_kind(col.dtype):
+            raise ExpressionTypeError(
+                f"Column '{name}' has an invalid type: {col.dtype}"
+            )
+
         new_tbl.selects.add(name)
         new_tbl.named_cols.fwd[name] = uid
         new_tbl.available_cols.add(uid)
-        new_tbl.cols[uid] = ColumnMetaData.from_expr(uid, expr, new_tbl, verb="mutate")
+        new_tbl.cols[uid] = col
 
     new_tbl.mutate(**kwargs)
     return new_tbl
 
 
 @builtin_verb()
 def join(
     left: AbstractTableImpl,
     right: AbstractTableImpl,
     on: SymbolicExpression,
     how: str,
     *,
-    validate: str = None,
+    validate: Literal["1:?", None] = None,
 ):
     validate_table_args(left, right)
 
     if left.grouped_by or right.grouped_by:
-        raise ValueError(f"Can't join grouped tables. You first have to ungroup them.")
+        raise ValueError("Can't join grouped tables. You first have to ungroup them.")
 
     # Check args only contains valid columns
     check_cols_available((left, right), cols_in_expression(on), "join")
 
     if how not in ("inner", "left", "outer"):
         raise ValueError(
             "Join type must be one of 'inner', 'left' or 'outer' (value provided:"
@@ -352,23 +370,24 @@
 @builtin_verb()
 def group_by(tbl: AbstractTableImpl, *args: Column | LambdaColumn, add=False):
     # Validate Input
     validate_table_args(tbl)
     check_cols_available(tbl, cols_in_expressions(args), "group_by")
     check_lambdas_valid(tbl, *args)
 
-    # WARNING: Depending on the SQL backend, you might only be allowed to reference columns
+    # WARNING: Depending on the SQL backend, you might
+    #          only be allowed to reference columns
     if not args:
         raise ValueError(
             "Expected columns to group by, but none were specified. To remove the"
             " grouping use the ungroup verb instead."
         )
     for col in args:
         if not isinstance(col, (Column, LambdaColumn)):
-            raise ValueError(
+            raise TypeError(
                 "Arguments to group_by verb must be of type 'Column' or 'LambdaColumn'"
                 f" and not '{type(col)}'."
             )
 
     args = [tbl.resolve_lambda_cols(arg) for arg in args]
 
     new_tbl = tbl.copy()
@@ -421,19 +440,30 @@
     # Add summarizing cols to the end of the select.
     for name, expr in kwargs.items():
         if name in selects:
             raise ValueError(
                 f"Column with name '{name}' already in select. The new summarised"
                 " columns must have a different name than the grouping columns."
             )
-        uid = generate_col_uuid()
+        uid = Column.generate_col_uuid()
+        col = ColumnMetaData.from_expr(uid, expr, new_tbl, verb="summarise")
+
+        if dtypes.NoneDType().same_kind(col.dtype):
+            raise ExpressionTypeError(
+                f"Column '{name}' has an invalid type: {col.dtype}"
+            )
+        if col.ftype != OPType.AGGREGATE:
+            raise FunctionTypeError(
+                f"Expression for column '{name}' doesn't summarise any values."
+            )
+
         selects.add(name)
         named_cols.fwd[name] = uid
         available_cols.add(uid)
-        cols[uid] = ColumnMetaData.from_expr(uid, expr, new_tbl, verb="summarise")
+        cols[uid] = col
 
     # Update new_tbl
     new_tbl.selects = ordered_set(selects)
     new_tbl.named_cols = named_cols
     new_tbl.available_cols = available_cols
     new_tbl.cols.update(cols)
     new_tbl.intrinsic_grouped_by = new_tbl.grouped_by.copy()
```

### Comparing `pydiverse_transform-0.1.3/PKG-INFO` & `pydiverse_transform-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: pydiverse-transform
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pipe based dataframe manipulation library that can also transform data on SQL databases
 License: BSD-3-Clause
 Author: QuantCo, Inc.
 Requires-Python: >=3.9
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database
+Provides-Extra: pyarrow
 Requires-Dist: SQLAlchemy (>=1.4.27)
 Requires-Dist: numpy (>=1.23.1)
 Requires-Dist: pandas (>=1.4.3)
+Requires-Dist: pyarrow (>=11.0.0) ; extra == "pyarrow"
 Description-Content-Type: text/markdown
 
 # pydiverse.transform
 
 [![CI](https://github.com/pydiverse/pydiverse.transform/actions/workflows/tests.yml/badge.svg)](https://github.com/pydiverse/pydiverse.transform/actions/workflows/tests.yml)
 
 Pipe based dataframe manipulation library that can also transform data on SQL databases
```

