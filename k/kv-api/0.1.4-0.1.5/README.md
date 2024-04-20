# Comparing `tmp/kv_api-0.1.4.tar.gz` & `tmp/kv_api-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv_api-0.1.4.tar", last modified: Thu Apr 18 07:01:32 2024, max compression
+gzip compressed data, was "kv_api-0.1.5.tar", last modified: Sat Apr 20 18:04:02 2024, max compression
```

## Comparing `kv_api-0.1.4.tar` & `kv_api-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:32.716112 kv_api-0.1.4/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      423 2024-04-18 07:01:32.716112 kv_api-0.1.4/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       46 2024-04-05 12:42:30.000000 kv_api-0.1.4/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      603 2024-04-18 07:01:28.000000 kv_api-0.1.4/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-18 07:01:32.716112 kv_api-0.1.4/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:32.716112 kv_api-0.1.4/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:32.706112 kv_api-0.1.4/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:32.716112 kv_api-0.1.4/src/kv/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      172 2024-04-18 06:51:44.000000 kv_api-0.1.4/src/kv/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1327 2024-04-18 06:51:39.000000 kv_api-0.1.4/src/kv/api/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:32.716112 kv_api-0.1.4/src/kv/api/append/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       45 2024-04-15 16:52:22.000000 kv_api-0.1.4/src/kv/api/append/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      762 2024-04-18 06:52:15.000000 kv_api-0.1.4/src/kv/api/append/append.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:32.716112 kv_api-0.1.4/src/kv/api/errors/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       81 2024-04-10 05:52:43.000000 kv_api-0.1.4/src/kv/api/errors/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      679 2024-04-10 09:04:29.000000 kv_api-0.1.4/src/kv/api/errors/errors.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      118 2024-04-15 16:21:13.000000 kv_api-0.1.4/src/kv/api/locatable.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:32.716112 kv_api-0.1.4/src/kv_api.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      423 2024-04-18 07:01:32.000000 kv_api-0.1.4/src/kv_api.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      374 2024-04-18 07:01:32.000000 kv_api-0.1.4/src/kv_api.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-18 07:01:32.000000 kv_api-0.1.4/src/kv_api.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-04-18 07:01:32.000000 kv_api-0.1.4/src/kv_api.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-18 07:01:32.000000 kv_api-0.1.4/src/kv_api.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:02.820967 kv_api-0.1.5/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      423 2024-04-20 18:04:02.820967 kv_api-0.1.5/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       46 2024-04-05 12:42:30.000000 kv_api-0.1.5/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      603 2024-04-20 18:04:00.000000 kv_api-0.1.5/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-20 18:04:02.820967 kv_api-0.1.5/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:02.810967 kv_api-0.1.5/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:02.810967 kv_api-0.1.5/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:02.810967 kv_api-0.1.5/src/kv/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      122 2024-04-20 17:32:30.000000 kv_api-0.1.5/src/kv/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2491 2024-04-20 17:54:31.000000 kv_api-0.1.5/src/kv/api/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:02.810967 kv_api-0.1.5/src/kv/api/append/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       79 2024-04-20 17:37:34.000000 kv_api-0.1.5/src/kv/api/append/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      818 2024-04-20 17:34:19.000000 kv_api-0.1.5/src/kv/api/append/append.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      646 2024-04-20 17:38:48.000000 kv_api-0.1.5/src/kv/api/append/simple.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:02.810967 kv_api-0.1.5/src/kv/api/errors/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       81 2024-04-10 05:52:43.000000 kv_api-0.1.5/src/kv/api/errors/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      791 2024-04-20 05:01:50.000000 kv_api-0.1.5/src/kv/api/errors/errors.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1598 2024-04-20 17:32:02.000000 kv_api-0.1.5/src/kv/api/simple.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:02.820967 kv_api-0.1.5/src/kv_api.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      423 2024-04-20 18:04:02.000000 kv_api-0.1.5/src/kv_api.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      399 2024-04-20 18:04:02.000000 kv_api-0.1.5/src/kv_api.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-20 18:04:02.000000 kv_api-0.1.5/src/kv_api.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-04-20 18:04:02.000000 kv_api-0.1.5/src/kv_api.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-20 18:04:02.000000 kv_api-0.1.5/src/kv_api.egg-info/top_level.txt
```

### Comparing `kv_api-0.1.4/pyproject.toml` & `kv_api-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kv-api"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "API spec for an async Key-Value DB"
 dependencies = [
   "haskellian-either"
 ]
```

### Comparing `kv_api-0.1.4/src/kv/api/append/append.py` & `kv_api-0.1.5/src/kv/api/append/append.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import Generic, TypeVar, overload, Literal
 from abc import ABC, abstractmethod
 from haskellian.either import Either
+from haskellian.asyn.promises import Promise
 from ..errors import DBError, InexistentItem
 from ..api import KV
 
 T = TypeVar('T')
 
 class Appendable(ABC, Generic[T]):
   @overload
   @abstractmethod
-  async def append(self, id: str, values: list[T], *, create: Literal[False]) -> Either[DBError|InexistentItem, None]:
+  def append(self, id: str, values: list[T], *, create: Literal[False]) -> Promise[Either[DBError|InexistentItem, None]]:
     """Appends `values` if it already existed. Otherwise doesn't append, and returns `Left[ExistentItem]`"""
   @overload
   @abstractmethod
-  async def append(self, id: str, values: list[T], *, create: bool = True) -> Either[DBError, None]:
+  def append(self, id: str, values: list[T], *, create: bool = True) -> Promise[Either[DBError, None]]:
     """Appends `values` to `id`, creating the item if needed"""
 
-class AppendableAPI(KV[T], Appendable, Generic[T]):
+class AppendableKV(KV[list[T]], Appendable, Generic[T]):
   ...
```

### Comparing `kv_api-0.1.4/src/kv/api/errors/errors.py` & `kv_api-0.1.5/src/kv/api/errors/errors.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from typing import Literal, Any
 from dataclasses import dataclass
 
+class StrMixin:
+  def __str__(self) -> str:
+    return self.__repr__()
+
 @dataclass(eq=False)
-class InexistentItem(BaseException):
+class InexistentItem(StrMixin, BaseException):
   key: str | None = None
   detail: Any | None = None
   reason: Literal['inexistent-item'] = 'inexistent-item'
 
 @dataclass(eq=False)
-class ExistentItem(BaseException):
+class ExistentItem(StrMixin, BaseException):
   key: str
   detail: Any | None = None
   reason: Literal['existent-item'] = 'existent-item'
 
 @dataclass(eq=False)
-class DBError(BaseException):
+class DBError(StrMixin, BaseException):
   detail: Any = None
   reason: Literal['db-error'] = 'db-error'
 
 @dataclass(eq=False)
-class InvalidData(BaseException):
+class InvalidData(StrMixin, BaseException):
   detail: Any = None
   reason: Literal['invalid-data'] = 'invalid-data'
 
 ReadError = DBError | InvalidData | InexistentItem
```

