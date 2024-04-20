# Comparing `tmp/kv_fs-0.1.6.tar.gz` & `tmp/kv_fs-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv_fs-0.1.6.tar", last modified: Thu Apr 18 07:01:56 2024, max compression
+gzip compressed data, was "kv_fs-0.1.7.tar", last modified: Sat Apr 20 18:04:21 2024, max compression
```

## Comparing `kv_fs-0.1.6.tar` & `kv_fs-0.1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:56.916112 kv_fs-0.1.6/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1191 2024-04-18 07:01:56.916112 kv_fs-0.1.6/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      773 2024-04-05 13:29:50.000000 kv_fs-0.1.6/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      620 2024-04-18 07:01:47.000000 kv_fs-0.1.6/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-18 07:01:56.916112 kv_fs-0.1.6/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:56.906112 kv_fs-0.1.6/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:56.896112 kv_fs-0.1.6/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:56.906112 kv_fs-0.1.6/src/kv/fs/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-05 13:16:34.000000 kv_fs-0.1.6/src/kv/fs/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:56.906112 kv_fs-0.1.6/src/kv/fs/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       29 2024-04-05 13:16:34.000000 kv_fs-0.1.6/src/kv/fs/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3520 2024-04-18 06:52:28.000000 kv_fs-0.1.6/src/kv/fs/api/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:56.906112 kv_fs-0.1.6/src/kv/fs/append/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-15 16:51:53.000000 kv_fs-0.1.6/src/kv/fs/append/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1109 2024-04-15 17:43:37.000000 kv_fs-0.1.6/src/kv/fs/append/append.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      563 2024-04-15 16:09:48.000000 kv_fs-0.1.6/src/kv/fs/append/ndjson.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:56.906112 kv_fs-0.1.6/src/kv/fs/ops/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       84 2024-04-15 15:13:10.000000 kv_fs-0.1.6/src/kv/fs/ops/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2274 2024-04-15 15:48:34.000000 kv_fs-0.1.6/src/kv/fs/ops/ops.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:56.906112 kv_fs-0.1.6/src/kv_fs.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1191 2024-04-18 07:01:56.000000 kv_fs-0.1.6/src/kv_fs.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      387 2024-04-18 07:01:56.000000 kv_fs-0.1.6/src/kv_fs.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-18 07:01:56.000000 kv_fs-0.1.6/src/kv_fs.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       31 2024-04-18 07:01:56.000000 kv_fs-0.1.6/src/kv_fs.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-18 07:01:56.000000 kv_fs-0.1.6/src/kv_fs.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:21.481025 kv_fs-0.1.7/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1191 2024-04-20 18:04:21.481025 kv_fs-0.1.7/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      773 2024-04-05 13:29:50.000000 kv_fs-0.1.7/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      620 2024-04-20 18:04:19.000000 kv_fs-0.1.7/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-20 18:04:21.481025 kv_fs-0.1.7/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:21.471025 kv_fs-0.1.7/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:21.471025 kv_fs-0.1.7/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:21.471025 kv_fs-0.1.7/src/kv/fs/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-05 13:16:34.000000 kv_fs-0.1.7/src/kv/fs/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:21.471025 kv_fs-0.1.7/src/kv/fs/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       29 2024-04-05 13:16:34.000000 kv_fs-0.1.7/src/kv/fs/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     5017 2024-04-20 18:03:41.000000 kv_fs-0.1.7/src/kv/fs/api/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:21.471025 kv_fs-0.1.7/src/kv/fs/append/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-15 16:51:53.000000 kv_fs-0.1.7/src/kv/fs/append/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1108 2024-04-20 17:35:38.000000 kv_fs-0.1.7/src/kv/fs/append/append.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      563 2024-04-15 16:09:48.000000 kv_fs-0.1.7/src/kv/fs/append/ndjson.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:21.481025 kv_fs-0.1.7/src/kv/fs/ops/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       96 2024-04-20 17:53:13.000000 kv_fs-0.1.7/src/kv/fs/ops/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2719 2024-04-20 17:53:05.000000 kv_fs-0.1.7/src/kv/fs/ops/ops.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-20 18:04:21.481025 kv_fs-0.1.7/src/kv_fs.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1191 2024-04-20 18:04:21.000000 kv_fs-0.1.7/src/kv_fs.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      387 2024-04-20 18:04:21.000000 kv_fs-0.1.7/src/kv_fs.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-20 18:04:21.000000 kv_fs-0.1.7/src/kv_fs.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       31 2024-04-20 18:04:21.000000 kv_fs-0.1.7/src/kv_fs.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-20 18:04:21.000000 kv_fs-0.1.7/src/kv_fs.egg-info/top_level.txt
```

### Comparing `kv_fs-0.1.6/PKG-INFO` & `kv_fs-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kv-fs
-Version: 0.1.6
+Version: 0.1.7
 Summary: Key-Value DB API on the filesystem
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-kv
 Project-URL: home, https://github.com/moveread/python-kv/tree/main/kv-fs
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
```

### Comparing `kv_fs-0.1.6/README.md` & `kv_fs-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `kv_fs-0.1.6/pyproject.toml` & `kv_fs-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kv-fs"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Key-Value DB API on the filesystem"
 dependencies = [
   "kv-api", "ramda", "haskellian-either"
 ]
```

### Comparing `kv_fs-0.1.6/src/kv/fs/api/api.py` & `kv_fs-0.1.7/src/kv/fs/api/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 from typing import TypeVar, Generic, Callable, AsyncIterable
 from dataclasses import dataclass
 import os
+from shutil import SameFileError
 from ramda import curry
 import haskellian.either as E
 import haskellian.asyn.promises as P
 import haskellian.asyn.iter as AI
 from pydantic import RootModel
-from kv.api import KV, Locatable
+from kv.api import KV
 from kv.api.errors import InexistentItem, InvalidData, ExistentItem, DBError
 from .. import ops
 
 A = TypeVar('A')
 T = TypeVar('T')
 
 @dataclass
-class FilesystemKV(KV[T], Locatable, Generic[T]):
+class FilesystemKV(KV[T], Generic[T]):
 
   @classmethod
   def validated(cls, Type: type[A], base_path: str) -> 'FilesystemKV[A]':
     Model = RootModel[Type]
     return FilesystemKV(
       base_path=base_path, extension='.json',
       parse=lambda b: E.validate_json(b, Model).fmap(lambda x: x.root).mapl(InvalidData),
       dump=lambda x: Model(x).model_dump_json(exclude_none=True)
     )
 
   base_path: str
   extension: str = ''
   parse: Callable[[bytes], E.Either[InvalidData, T]] = lambda x: E.Right(x) # type: ignore
   dump: Callable[[T], bytes|str] = lambda x: x # type: ignore
+  
+  def __post_init__(self):
+    os.makedirs(self.base_path, exist_ok=True)
 
   def _path(self, key: str) -> str:
     return os.path.abspath(os.path.join(self.base_path, f'{key}{self.extension}'))
   
   @curry
   def _parse_err(self, err: OSError, key: str) -> DBError | ExistentItem | InexistentItem:
     match err:
@@ -44,18 +48,18 @@
         return DBError(str(err))
   
   @P.lift
   async def insert(self, key: str, value: T, *, replace: bool = False) -> E.Either[ExistentItem|DBError, None]:
     return ops.insert(self._path(key), self.dump(value), exists_ok=replace) \
       .mapl(self._parse_err(key=key)) # type: ignore
   
-  @P.lift
-  async def update(self, key: str, value: T) -> E.Either[DBError | InexistentItem, None]:
-    return ops.update(self._path(key), self.dump(value)) \
-      .mapl(self._parse_err(key=key)) # type: ignore
+  # @P.lift
+  # async def update(self, key: str, value: T) -> E.Either[DBError | InexistentItem, None]:
+  #   return ops.update(self._path(key), self.dump(value)) \
+  #     .mapl(self._parse_err(key=key)) # type: ignore
 
   @P.lift
   async def read(self, key: str) -> E.Either[DBError | InvalidData | InexistentItem, T]:
     either = ops.read(self._path(key)) \
       .mapl(self._parse_err(key=key)) # type: ignore
     return either & self.parse
   
@@ -81,18 +85,47 @@
         yield E.Right((name, value))
       except E.IsLeft as e:
         if isinstance(e.value, OSError):
           yield E.Left(DBError(str(e)))
         else:
           yield E.Left(e.value)
 
-  def url(self, id: str) -> str:
-    return self._path(id)
-      
   @P.lift
   async def commit(self) -> E.Either[DBError, None]:
     return E.Right(None)
   
   @P.lift
   async def rollback(self) -> E.Either[DBError, None]:
     return E.Left(DBError('Rollback not implemented in filesystem KV'))
-  
+  
+  @P.lift
+  async def copy(self, key: str, to: 'KV[T]', to_key: str, *, replace: bool = True) -> E.Either[DBError|InexistentItem|ExistentItem, None]:
+    if not isinstance(to, FilesystemKV):
+      return await super().copy(key, to, to_key, replace=replace)
+    
+    if not replace and os.path.exists(to._path(to_key)):
+      return E.Left(ExistentItem(to_key, detail=f'Path "{to._path(to_key)}" already exists, but replace is False'))
+
+    match ops.copy(self._path(key), to._path(to_key)):
+      case E.Right():
+        return E.Right(None)
+      case E.Left(FileNotFoundError()) as e:
+        return E.Left(InexistentItem(key, detail=str(e.value)))
+      case E.Left() as e:
+        return E.Left(DBError(detail=str(e.value)))
+ 
+  @P.lift
+  async def move(self, key: str, to: 'KV[T]', to_key: str, *, replace: bool = True) -> E.Either[DBError|InexistentItem|ExistentItem, None]:
+    if not isinstance(to, FilesystemKV):
+      return await super().move(key, to, to_key, replace=replace)
+    
+    if not replace and os.path.exists(to._path(to_key)):
+      return E.Left(ExistentItem(to_key, detail=f'Path "{to._path(to_key)}" already exists, but replace is False'))
+
+    match ops.move(self._path(key), to._path(to_key)):
+      case E.Right():
+        return E.Right(None)
+      case E.Left(FileNotFoundError()) as e:
+        return E.Left(InexistentItem(key, detail=str(e.value)))
+      case E.Left() as e:
+        return E.Left(DBError(detail=str(e.value)))
+
```

### Comparing `kv_fs-0.1.6/src/kv/fs/append/append.py` & `kv_fs-0.1.7/src/kv/fs/append/append.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Generic, TypeVar
 import os
 from pydantic import RootModel
 import haskellian.either as E
 import haskellian.asyn.promises as P
-from kv.api import AppendableAPI
+from kv.api.append import AppendableKV
 from kv.api.errors import InexistentItem, DBError, InvalidData
 from ..api import FilesystemKV
 from .. import ops
 from . import ndjson
 
 A = TypeVar('A')
 T = TypeVar('T')
 
-class FilesystemAppendKV(FilesystemKV[list[T]], AppendableAPI[list[T]], Generic[T]):
+class FilesystemAppendKV(FilesystemKV[list[T]], AppendableKV[T], Generic[T]):
 
   @P.lift
   async def append(self, id: str, values: list[T], *, create: bool = True) -> E.Either[DBError|InexistentItem, None]:
     if not create and not os.path.exists(self._path(id)):
       return E.Left(InexistentItem(id))
     either = ops.append(self._path(id), self.dump(values))
     return either.mapl(self._parse_err) # type: ignore
```

### Comparing `kv_fs-0.1.6/src/kv/fs/append/ndjson.py` & `kv_fs-0.1.7/src/kv/fs/append/ndjson.py`

 * *Files identical despite different names*

### Comparing `kv_fs-0.1.6/src/kv/fs/ops/ops.py` & `kv_fs-0.1.7/src/kv/fs/ops/ops.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 from typing import Iterable
 import os
+import shutil
 from haskellian.either import Either, Left, Right, safe
 
+def copy(src: str, dst: str) -> Either[FileNotFoundError|shutil.SameFileError|OSError, None]:
+  try:
+    shutil.copy(src, dst)
+    return Right(None)
+  except (shutil.SameFileError, FileNotFoundError, OSError) as e:
+    return Left(e)
+  
+def move(src: str, dst: str) -> Either[FileNotFoundError|OSError, None]:
+  try:
+    shutil.move(src, dst)
+    return Right(None)
+  except (FileNotFoundError, OSError) as e:
+    return Left(e)
+
 def ensure_path(file: str):
   dir = os.path.dirname(file)
   if dir != '':
     os.makedirs(dir, exist_ok=True)
 
 def append(path: str, data: str|bytes) -> Either[OSError, None]:
   mode = f'ab' if isinstance(data, bytes) else 'a'
```

### Comparing `kv_fs-0.1.6/src/kv_fs.egg-info/PKG-INFO` & `kv_fs-0.1.7/src/kv_fs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kv-fs
-Version: 0.1.6
+Version: 0.1.7
 Summary: Key-Value DB API on the filesystem
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-kv
 Project-URL: home, https://github.com/moveread/python-kv/tree/main/kv-fs
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
```

