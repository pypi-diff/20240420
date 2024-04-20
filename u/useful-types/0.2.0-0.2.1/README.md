# Comparing `tmp/useful_types-0.2.0.tar.gz` & `tmp/useful_types-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "useful_types-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "useful_types-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `useful_types-0.2.0.tar` & `useful_types-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1056 2023-06-18 22:23:38.935104 useful_types-0.2.0/LICENSE
--rw-r--r--   0        0        0      509 2023-06-19 00:39:07.860788 useful_types-0.2.0/README.md
--rw-r--r--   0        0        0     1043 2023-09-23 21:33:56.607109 useful_types-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7923 2023-09-23 21:29:12.717252 useful_types-0.2.0/useful_types/__init__.py
--rw-r--r--   0        0        0     1766 2023-07-23 02:04:01.297352 useful_types-0.2.0/useful_types/experimental.py
--rw-r--r--   0        0        0        0 2023-03-11 23:36:05.335457 useful_types-0.2.0/useful_types/py.typed
--rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 useful_types-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-06-18 22:23:38.935104 useful_types-0.2.1/LICENSE
+-rw-r--r--   0        0        0      509 2023-06-19 00:39:07.860788 useful_types-0.2.1/README.md
+-rw-r--r--   0        0        0     1043 2024-04-20 08:56:46.209082 useful_types-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7923 2024-04-20 08:36:52.389490 useful_types-0.2.1/useful_types/__init__.py
+-rw-r--r--   0        0        0     1766 2023-07-23 02:04:01.297352 useful_types-0.2.1/useful_types/experimental.py
+-rw-r--r--   0        0        0        0 2023-03-11 23:36:05.335457 useful_types-0.2.1/useful_types/py.typed
+-rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 useful_types-0.2.1/PKG-INFO
```

### Comparing `useful_types-0.2.0/LICENSE` & `useful_types-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `useful_types-0.2.0/pyproject.toml` & `useful_types-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "useful_types"
-version = "0.2.0"
+version = "0.2.1"
 authors = [{name = "The Python typing community"}]
 description = "A collection of useful types."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
 dependencies = ["typing_extensions >= 4.7"]
```

### Comparing `useful_types-0.2.0/useful_types/__init__.py` & `useful_types-0.2.1/useful_types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,10 +286,10 @@
     @overload
     def __getitem__(self, index: SupportsIndex, /) -> _T_co: ...
     @overload
     def __getitem__(self, index: slice, /) -> Sequence[_T_co]: ...
     def __contains__(self, value: object, /) -> bool: ...
     def __len__(self) -> int: ...
     def __iter__(self) -> Iterator[_T_co]: ...
-    def index(self, value: Any, /, start: int = 0, stop: int = ...) -> int: ...
+    def index(self, value: Any, start: int = 0, stop: int = ..., /) -> int: ...
     def count(self, value: Any, /) -> int: ...
     def __reversed__(self) -> Iterator[_T_co]: ...
```

### Comparing `useful_types-0.2.0/useful_types/experimental.py` & `useful_types-0.2.1/useful_types/experimental.py`

 * *Files identical despite different names*

### Comparing `useful_types-0.2.0/PKG-INFO` & `useful_types-0.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: useful_types
-Version: 0.2.0
+Version: 0.2.1
 Summary: A collection of useful types.
 Author: The Python typing community
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: typing_extensions >= 4.7
 Project-URL: changelog, https://github.com/hauntsaninja/useful_types/blob/main/CHANGELOG.md
 Project-URL: homepage, https://github.com/hauntsaninja/useful_types
```

