# Comparing `tmp/sqlrepo-1.2.1.tar.gz` & `tmp/sqlrepo-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlrepo-1.2.1.tar", last modified: Fri Apr 19 14:09:09 2024, max compression
+gzip compressed data, was "sqlrepo-1.3.0.tar", last modified: Sat Apr 20 18:29:02 2024, max compression
```

## Comparing `sqlrepo-1.2.1.tar` & `sqlrepo-1.3.0.tar`

### file list

```diff
@@ -1,26 +1,22 @@
--rw-r--r--   0        0        0     9580 2024-04-19 13:48:52.688101 sqlrepo-1.2.1/README.md
--rw-r--r--   0        0        0     3039 2024-04-19 14:09:09.193136 sqlrepo-1.2.1/pyproject.toml
--rw-r--r--   0        0        0       37 2024-01-16 08:47:35.121506 sqlrepo-1.2.1/sqlrepo/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2024-01-16 08:47:35.121506 sqlrepo-1.2.1/sqlrepo/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2024-01-16 08:47:35.121506 sqlrepo-1.2.1/sqlrepo/.pytest_cache/README.md
--rw-r--r--   0        0        0      130 2024-01-16 08:47:35.121506 sqlrepo-1.2.1/sqlrepo/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2024-01-16 08:47:35.121506 sqlrepo-1.2.1/sqlrepo/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      463 2024-04-15 09:56:07.307086 sqlrepo-1.2.1/sqlrepo/__init__.py
--rw-r--r--   0        0        0      491 2024-04-15 09:17:35.411159 sqlrepo-1.2.1/sqlrepo/exc.py
--rw-r--r--   0        0        0      798 2024-04-15 09:17:49.278046 sqlrepo-1.2.1/sqlrepo/logging.py
--rw-r--r--   0        0        0        0 2024-04-16 08:40:42.695391 sqlrepo-1.2.1/sqlrepo/py.typed
--rw-r--r--   0        0        0    32857 2024-04-19 14:00:18.076644 sqlrepo-1.2.1/sqlrepo/queries.py
--rw-r--r--   0        0        0    22638 2024-04-19 13:36:14.622268 sqlrepo-1.2.1/sqlrepo/repositories.py
--rw-r--r--   0        0        0     3540 2024-04-16 08:43:46.475848 sqlrepo-1.2.1/sqlrepo/uow.py
--rw-r--r--   0        0        0        0 2023-12-29 20:17:14.670751 sqlrepo-1.2.1/tests/__init__.py
--rw-r--r--   0        0        0     8306 2024-04-18 09:54:19.867457 sqlrepo-1.2.1/tests/conftest.py
--rw-r--r--   0        0        0    14662 2024-04-19 14:00:47.946165 sqlrepo-1.2.1/tests/test_async_queries.py
--rw-r--r--   0        0        0    11193 2024-04-19 13:59:20.466566 sqlrepo-1.2.1/tests/test_async_repositories.py
--rw-r--r--   0        0        0    17011 2024-04-18 08:27:43.006148 sqlrepo-1.2.1/tests/test_base_queries.py
--rw-r--r--   0        0        0     2825 2024-04-18 13:50:35.586184 sqlrepo-1.2.1/tests/test_base_repositories.py
--rw-r--r--   0        0        0    13863 2024-04-19 13:47:29.322240 sqlrepo-1.2.1/tests/test_sync_queries.py
--rw-r--r--   0        0        0    10428 2024-04-19 13:50:29.889774 sqlrepo-1.2.1/tests/test_sync_repositories.py
--rw-r--r--   0        0        0        0 2024-04-05 11:56:33.229687 sqlrepo-1.2.1/tests/test_uow.py
--rw-r--r--   0        0        0      804 2024-04-15 06:16:49.991950 sqlrepo-1.2.1/tests/types.py
--rw-r--r--   0        0        0     7155 2024-04-19 14:04:27.333651 sqlrepo-1.2.1/tests/utils.py
--rw-r--r--   0        0        0     9933 1970-01-01 00:00:00.000000 sqlrepo-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    10214 2024-04-20 17:27:11.031406 sqlrepo-1.3.0/README.md
+-rw-r--r--   0        0        0     3039 2024-04-20 18:29:02.978908 sqlrepo-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      463 2024-04-20 13:22:39.767049 sqlrepo-1.3.0/sqlrepo/__init__.py
+-rw-r--r--   0        0        0      828 2024-04-20 18:17:10.137553 sqlrepo-1.3.0/sqlrepo/exc.py
+-rw-r--r--   0        0        0      798 2024-04-20 13:22:39.767049 sqlrepo-1.3.0/sqlrepo/logging.py
+-rw-r--r--   0        0        0        0 2024-04-20 13:22:39.767049 sqlrepo-1.3.0/sqlrepo/py.typed
+-rw-r--r--   0        0        0    32857 2024-04-20 13:22:39.767049 sqlrepo-1.3.0/sqlrepo/queries.py
+-rw-r--r--   0        0        0    22638 2024-04-20 17:56:19.449223 sqlrepo-1.3.0/sqlrepo/repositories.py
+-rw-r--r--   0        0        0     4650 2024-04-20 18:19:28.090308 sqlrepo-1.3.0/sqlrepo/uow.py
+-rw-r--r--   0        0        0        0 2024-02-23 13:08:38.602420 sqlrepo-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     8306 2024-04-20 13:22:39.767049 sqlrepo-1.3.0/tests/conftest.py
+-rw-r--r--   0        0        0    14662 2024-04-20 13:22:39.767049 sqlrepo-1.3.0/tests/test_async_queries.py
+-rw-r--r--   0        0        0    11193 2024-04-20 17:56:35.948763 sqlrepo-1.3.0/tests/test_async_repositories.py
+-rw-r--r--   0        0        0     1296 2024-04-20 18:23:19.878013 sqlrepo-1.3.0/tests/test_async_uow.py
+-rw-r--r--   0        0        0    17001 2024-04-20 18:27:20.234117 sqlrepo-1.3.0/tests/test_base_queries.py
+-rw-r--r--   0        0        0     2983 2024-04-20 18:26:07.232625 sqlrepo-1.3.0/tests/test_base_repositories.py
+-rw-r--r--   0        0        0    13863 2024-04-20 13:22:39.767049 sqlrepo-1.3.0/tests/test_sync_queries.py
+-rw-r--r--   0        0        0    10428 2024-04-20 13:22:39.767049 sqlrepo-1.3.0/tests/test_sync_repositories.py
+-rw-r--r--   0        0        0     1124 2024-04-20 18:21:28.054970 sqlrepo-1.3.0/tests/test_sync_uow.py
+-rw-r--r--   0        0        0      804 2024-04-14 11:07:16.846888 sqlrepo-1.3.0/tests/types.py
+-rw-r--r--   0        0        0     7155 2024-04-20 13:22:39.767049 sqlrepo-1.3.0/tests/utils.py
+-rw-r--r--   0        0        0    10567 1970-01-01 00:00:00.000000 sqlrepo-1.3.0/PKG-INFO
```

### Comparing `sqlrepo-1.2.1/README.md` & `sqlrepo-1.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 # sqlrepo
 
 ![coverage](./coverage.svg)
 
->SQLAlchemy repository pattern.
+> Repository pattern implementation for SQLAlchemy models.
+
+## About repository pattern
+
+Actually, I know, that my implementation is not good as repository pattern. I know, that
+repository must has abstract interface, which must be implemented for different backends. I have
+plans to make sqlrepo part of repository-pattern package, which will implements all possible
+backends.
 
 ## Current state
 
 Now, some features of repository pattern works incorrect or some parts of it is hard to understand
 or use. I want to simplify work with repositories, so this is TODO for my project:
 
+* [ ] Add more backends for repository pattern. Now, only SQLAlchemy adapter implemented. I want
+      to implement other backends to make this repository better to use in different situations.
+      NOTE: in future sqlrepo will be replaced with something like python-repository-pattern.
 * [ ] Add more test cases for main functionality. Now, tested only base cases of repository
     method use.
 * [ ] Add wrapper for all non sqlrepo exceptions. Now, some functionality could raise
       "raw" SQLAlchemy error. I want to avoid the situation, when developer make
       try-except with all possible exceptions, when works with my package.
 * [ ] Add more use-cases of `specific_column_mapping` option. Now it only works with
       `search_by` and `order_by` params. I want to add it for filters, joins and other
```

### Comparing `sqlrepo-1.2.1/pyproject.toml` & `sqlrepo-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     "httpx>=0.27.0",
     "pyment>=0.3.3",
     "ipython>=8.19.0",
 ]
 
 [project]
 name = "sqlrepo"
-version = "1.2.1"
+version = "1.3.0"
 description = "sqlalchemy repositories with crud operations and other utils for it."
 authors = [
     { name = "Dmitriy Lunev", email = "dima.lunev14@gmail.com" },
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dependencies = [
```

### Comparing `sqlrepo-1.2.1/sqlrepo/logging.py` & `sqlrepo-1.3.0/sqlrepo/logging.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.2.1/sqlrepo/queries.py` & `sqlrepo-1.3.0/sqlrepo/queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.2.1/sqlrepo/repositories.py` & `sqlrepo-1.3.0/sqlrepo/repositories.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.2.1/tests/conftest.py` & `sqlrepo-1.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.2.1/tests/test_async_queries.py` & `sqlrepo-1.3.0/tests/test_async_queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.2.1/tests/test_async_repositories.py` & `sqlrepo-1.3.0/tests/test_async_repositories.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.2.1/tests/test_base_queries.py` & `sqlrepo-1.3.0/tests/test_base_queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             {"other_model_id": OtherModel.id, "some_other_model_field": OtherModel.name},
             ["not_presented_field", "other_model_id"],
             ["not_presented_field", OtherModel.id],
         ),
     ],
 )
 def test_resolve_specific_columns(  # noqa
-    specific_column_mapping: dict[str, ColumnElement[Any]],
+    specific_column_mapping: Any,  # noqa: ANN401
     elements: list[str | ColumnElement[Any]],
     expected_result: list[str | ColumnElement[Any]],  # noqa
 ) -> None:
     query = BaseQuery(SimpleFilterConverter, specific_column_mapping)
     converted_columns = query._resolve_specific_columns(elements=elements)  # type: ignore
     assert converted_columns == expected_result
```

### Comparing `sqlrepo-1.2.1/tests/test_base_repositories.py` & `sqlrepo-1.3.0/tests/test_base_repositories.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,21 @@
 def test_cant_eval_forward_ref() -> None:
     with pytest.warns(RepositoryModelClassIncorrectUseWarning):
 
         class MyRepo(BaseRepository["OtherModel"]):  # type: ignore
             ...
 
 
+def test_eval_forward_ref() -> None:
+    class MyRepo(BaseRepository["MyModel"]):  # type: ignore
+        ...
+
+    assert MyRepo.model_class == MyModel  # type: ignore
+
+
 def test_generic_incorrect_type() -> None:
     with pytest.warns(
         RepositoryModelClassIncorrectUseWarning,
         match="Passed GenericType is not SQLAlchemy model declarative class.",
     ):
 
         class MyRepo(BaseRepository[int]):  # type: ignore
@@ -62,16 +69,16 @@
     class CorrectRepo(BaseRepository[MyModel]): ...
 
     assert CorrectRepo.model_class == MyModel  # type: ignore
 
 
 def test_validate_disable_attributes() -> None:
     class CorrectRepo(BaseRepository[MyModel]):
-        disable_id_field = MyModel.id
-        disable_field = MyModel.bl
+        disable_id_field = "id"
+        disable_field = "bl"
         disable_field_type = bool
 
     CorrectRepo._validate_disable_attributes()  # type: ignore
 
 
 def test_validate_disable_attributes_raise_error() -> None:
     class CorrectRepo(BaseRepository[MyModel]): ...
```

### Comparing `sqlrepo-1.2.1/tests/test_sync_queries.py` & `sqlrepo-1.3.0/tests/test_sync_queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.2.1/tests/test_sync_repositories.py` & `sqlrepo-1.3.0/tests/test_sync_repositories.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.2.1/tests/types.py` & `sqlrepo-1.3.0/tests/types.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.2.1/tests/utils.py` & `sqlrepo-1.3.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.2.1/PKG-INFO` & `sqlrepo-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 Metadata-Version: 2.1
 Name: sqlrepo
-Version: 1.2.1
+Version: 1.3.0
 Summary: sqlalchemy repositories with crud operations and other utils for it.
 Author-Email: Dmitriy Lunev <dima.lunev14@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: sqlalchemy>=2.0.29
 Requires-Dist: python-dev-utils[sqlalchemy_filters]>=1.3.1
 Description-Content-Type: text/markdown
 
 # sqlrepo
 
 ![coverage](./coverage.svg)
 
->SQLAlchemy repository pattern.
+> Repository pattern implementation for SQLAlchemy models.
+
+## About repository pattern
+
+Actually, I know, that my implementation is not good as repository pattern. I know, that
+repository must has abstract interface, which must be implemented for different backends. I have
+plans to make sqlrepo part of repository-pattern package, which will implements all possible
+backends.
 
 ## Current state
 
 Now, some features of repository pattern works incorrect or some parts of it is hard to understand
 or use. I want to simplify work with repositories, so this is TODO for my project:
 
+* [ ] Add more backends for repository pattern. Now, only SQLAlchemy adapter implemented. I want
+      to implement other backends to make this repository better to use in different situations.
+      NOTE: in future sqlrepo will be replaced with something like python-repository-pattern.
 * [ ] Add more test cases for main functionality. Now, tested only base cases of repository
     method use.
 * [ ] Add wrapper for all non sqlrepo exceptions. Now, some functionality could raise
       "raw" SQLAlchemy error. I want to avoid the situation, when developer make
       try-except with all possible exceptions, when works with my package.
 * [ ] Add more use-cases of `specific_column_mapping` option. Now it only works with
       `search_by` and `order_by` params. I want to add it for filters, joins and other
```

