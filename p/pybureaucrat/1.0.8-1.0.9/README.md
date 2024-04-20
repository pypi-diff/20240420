# Comparing `tmp/pybureaucrat-1.0.8.tar.gz` & `tmp/pybureaucrat-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybureaucrat-1.0.8.tar", last modified: Sat Apr 13 13:15:48 2024, max compression
+gzip compressed data, was "pybureaucrat-1.0.9.tar", last modified: Thu Apr 18 18:04:06 2024, max compression
```

## Comparing `pybureaucrat-1.0.8.tar` & `pybureaucrat-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-13 13:15:48.552255 pybureaucrat-1.0.8/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2024-04-06 03:57:44.000000 pybureaucrat-1.0.8/LICENSE
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       37 2024-04-06 03:57:44.000000 pybureaucrat-1.0.8/MANIFEST.in
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      787 2024-04-13 13:15:48.552255 pybureaucrat-1.0.8/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-06 03:57:44.000000 pybureaucrat-1.0.8/README.MD
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-13 13:15:48.540255 pybureaucrat-1.0.8/client/
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-13 13:15:48.548255 pybureaucrat-1.0.8/client/pybureaucrat/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-10 15:11:05.000000 pybureaucrat-1.0.8/client/pybureaucrat/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2634 2024-04-10 15:11:05.000000 pybureaucrat-1.0.8/client/pybureaucrat/base.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1244 2024-04-10 15:11:05.000000 pybureaucrat-1.0.8/client/pybureaucrat/blobs.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      432 2024-04-13 13:13:31.000000 pybureaucrat-1.0.8/client/pybureaucrat/bureaucrat_connection.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      186 2024-04-10 15:11:05.000000 pybureaucrat-1.0.8/client/pybureaucrat/deserializers.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      813 2024-04-10 15:11:05.000000 pybureaucrat-1.0.8/client/pybureaucrat/queues.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1795 2024-04-10 15:11:05.000000 pybureaucrat-1.0.8/client/pybureaucrat/tables.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      860 2024-04-13 04:38:14.000000 pybureaucrat-1.0.8/client/pybureaucrat/trees.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-13 13:15:48.548255 pybureaucrat-1.0.8/client/pybureaucrat.egg-info/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      787 2024-04-13 13:15:48.000000 pybureaucrat-1.0.8/client/pybureaucrat.egg-info/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      497 2024-04-13 13:15:48.000000 pybureaucrat-1.0.8/client/pybureaucrat.egg-info/SOURCES.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2024-04-13 13:15:48.000000 pybureaucrat-1.0.8/client/pybureaucrat.egg-info/dependency_links.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       13 2024-04-13 13:15:48.000000 pybureaucrat-1.0.8/client/pybureaucrat.egg-info/top_level.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2024-04-06 03:57:44.000000 pybureaucrat-1.0.8/pyproject.toml
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2024-04-13 13:15:48.552255 pybureaucrat-1.0.8/setup.cfg
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1163 2024-04-10 15:11:05.000000 pybureaucrat-1.0.8/setup.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        5 2024-04-13 13:13:31.000000 pybureaucrat-1.0.8/version.txt
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-18 18:04:06.085151 pybureaucrat-1.0.9/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2024-04-06 03:57:44.000000 pybureaucrat-1.0.9/LICENSE
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       37 2024-04-06 03:57:44.000000 pybureaucrat-1.0.9/MANIFEST.in
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      787 2024-04-18 18:04:06.081151 pybureaucrat-1.0.9/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-06 03:57:44.000000 pybureaucrat-1.0.9/README.MD
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-18 18:04:06.069151 pybureaucrat-1.0.9/client/
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-18 18:04:06.081151 pybureaucrat-1.0.9/client/pybureaucrat/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-10 15:11:05.000000 pybureaucrat-1.0.9/client/pybureaucrat/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2847 2024-04-18 18:01:56.000000 pybureaucrat-1.0.9/client/pybureaucrat/base.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1316 2024-04-18 18:01:56.000000 pybureaucrat-1.0.9/client/pybureaucrat/blobs.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      432 2024-04-13 13:13:31.000000 pybureaucrat-1.0.9/client/pybureaucrat/bureaucrat_connection.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      186 2024-04-10 15:11:05.000000 pybureaucrat-1.0.9/client/pybureaucrat/deserializers.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      861 2024-04-18 18:01:56.000000 pybureaucrat-1.0.9/client/pybureaucrat/queues.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1891 2024-04-18 18:01:56.000000 pybureaucrat-1.0.9/client/pybureaucrat/tables.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      932 2024-04-18 18:01:56.000000 pybureaucrat-1.0.9/client/pybureaucrat/trees.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-18 18:04:06.081151 pybureaucrat-1.0.9/client/pybureaucrat.egg-info/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      787 2024-04-18 18:04:06.000000 pybureaucrat-1.0.9/client/pybureaucrat.egg-info/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      497 2024-04-18 18:04:06.000000 pybureaucrat-1.0.9/client/pybureaucrat.egg-info/SOURCES.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2024-04-18 18:04:06.000000 pybureaucrat-1.0.9/client/pybureaucrat.egg-info/dependency_links.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       13 2024-04-18 18:04:06.000000 pybureaucrat-1.0.9/client/pybureaucrat.egg-info/top_level.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2024-04-06 03:57:44.000000 pybureaucrat-1.0.9/pyproject.toml
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2024-04-18 18:04:06.085151 pybureaucrat-1.0.9/setup.cfg
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1163 2024-04-10 15:11:05.000000 pybureaucrat-1.0.9/setup.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        5 2024-04-18 18:01:56.000000 pybureaucrat-1.0.9/version.txt
```

### Comparing `pybureaucrat-1.0.8/LICENSE` & `pybureaucrat-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pybureaucrat-1.0.8/PKG-INFO` & `pybureaucrat-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybureaucrat
-Version: 1.0.8
+Version: 1.0.9
 Summary: A python client for bureaucrat server
 Home-page: https://github.com/LostSavannah/bureaucrat/tree/main/lib
 Author: Erick Fernando Mora Ramirez
 Author-email: erickfernandomoraramirez@gmail.com
 Project-URL: Bug Tracker, https://dev.moradev.dev/pybureaucrat/issues
 Project-URL: Documentation, https://dev.moradev.dev/pybureaucrat/documentation
 Project-URL: Examples, https://dev.moradev.dev/pybureaucrat/examples
```

### Comparing `pybureaucrat-1.0.8/client/pybureaucrat/base.py` & `pybureaucrat-1.0.9/client/pybureaucrat/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import TypeVar, Callable
 from enum import IntEnum
 import requests
+import asyncio
 
 from .deserializers import default_deserializer
 
 T = TypeVar("T")
 TResult = TypeVar("TResult")
 
 class ResultStatus(IntEnum):
@@ -35,41 +36,44 @@
         super().__init__(*args)
         self.status = status
 
 class BaseHttpService:
     def __init__(self, baseUrl:str) -> None:
         self.baseUrl = baseUrl
 
-    def get(self, url:str, headers:dict[str, str] = None, caster:Callable[[str,], T] = None, stream:bool = False) -> T:
+    async def get(self, url:str, headers:dict[str, str] = None, caster:Callable[[str,], T] = None, stream:bool = False) -> T:
         caster = caster or default_deserializer
-        response = requests.get(f"{self.baseUrl}/{url}", headers=headers, stream=stream)
+        request = lambda : requests.get(f"{self.baseUrl}/{url}", headers=headers, stream=stream)
+        response = await asyncio.to_thread(request)
         status = get_result_status(response.status_code)
         if status == ResultStatus.Success:
             return caster(response.text)
         else:
             raise ServiceError(status, response.text)
 
-    def post(self, url:str, parameter:T, 
+    async def post(self, url:str, parameter:T, 
              headers:dict[str, str] = None, caster:Callable[[str,], TResult] = None,
              is_raw:bool = False
              ) -> TResult:
         caster = caster or default_deserializer
         params = {
             "headers": headers,
             "data" if is_raw else "json":parameter
         }
-        response = requests.post(f"{self.baseUrl}/{url}",  **params)
+        request = lambda : requests.post(f"{self.baseUrl}/{url}",  **params)
+        response = await asyncio.to_thread(request)
         status = get_result_status(response.status_code)
         if status == ResultStatus.Success:
             return caster(response.text)
         else:
             raise ServiceError(status, response.text)
         
-    def delete(self, url:str, headers:dict[str, str] = None, caster:Callable[[str,], T] = None) -> T:
+    async def delete(self, url:str, headers:dict[str, str] = None, caster:Callable[[str,], T] = None) -> T:
         caster = caster or default_deserializer
         print(f"{self.baseUrl}/{url}")
-        response = requests.delete(f"{self.baseUrl}/{url}", headers=headers)
+        request = lambda : requests.delete(f"{self.baseUrl}/{url}", headers=headers)
+        response = await asyncio.to_thread(request)
         status = get_result_status(response.status_code)
         if status == ResultStatus.Success:
             return caster(response.text)
         else:
             raise ServiceError(status, response.text)
```

### Comparing `pybureaucrat-1.0.8/client/pybureaucrat/blobs.py` & `pybureaucrat-1.0.9/client/pybureaucrat/blobs.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,27 +12,28 @@
         self.files:list[str] = files
         self.folders:list[str] = folders
 
 class BlobsService(BaseHttpService):
     def __init__(self, baseUrl: str) -> None:
         super().__init__(baseUrl)
 
-    def index(self, path:str) -> BlobsIndex:
-        return BlobsIndex(**self.get(f"blobs/{path}")["index"])
+    async def index(self, path:str) -> BlobsIndex:
+        index = (await self.get(f"blobs/{path}"))["index"]
+        return BlobsIndex(**index)
     
-    def read(self, path:str) -> str|None:
+    async def read(self, path:str) -> str|None:
         try:
-            b64content:str = self.get(f"blobs/raw:{path}", caster=raw_deserializer)
+            b64content:str = await self.get(f"blobs/raw:{path}", caster=raw_deserializer)
             return base64.b64decode(b64content).decode()
         except:
             return None
     
-    def write(self, path:str, content:str) -> str:
+    async def write(self, path:str, content:str) -> str:
         b64content =  base64.b64encode(content.encode()).decode()
-        return self.post(f"blobs/{path}", b64content)
+        return await self.post(f"blobs/{path}", b64content)
 
-    def delete_blob(self, path:str) -> bool:
+    async def delete_blob(self, path:str) -> bool:
         try:
-            self.delete(f"blobs/{path}")
+            await self.delete(f"blobs/{path}")
             return True
         except ServiceError as e:
             return False
```

### Comparing `pybureaucrat-1.0.8/client/pybureaucrat/trees.py` & `pybureaucrat-1.0.9/client/pybureaucrat/trees.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import TypeVar, Any
 from .base import BaseHttpService, ServiceError
 
 class TreeService(BaseHttpService):
     def __init__(self, baseUrl: str) -> None:
         super().__init__(baseUrl)
 
-    def get_forests(self) -> list[str]:
-        return self.get("trees/")
+    async def get_forests(self) -> list[str]:
+        return await self.get("trees/")
 
-    def get_trees(self, forest:str) -> list[str]:
-        return self.get(f"trees/{forest}")
+    async def get_trees(self, forest:str) -> list[str]:
+        return await self.get(f"trees/{forest}")
 
-    def index(self, forest:str, tree:str, path:str = "$"):
-        return self.get(f"trees/{forest}/{tree}/index:{path}")
+    async def index(self, forest:str, tree:str, path:str = "$"):
+        return await self.get(f"trees/{forest}/{tree}/index:{path}")
 
-    def get_value(self, forest:str, tree:str, path:str = "$"):
-        return self.get(f"trees/{forest}/{tree}/{path}")
+    async def get_value(self, forest:str, tree:str, path:str = "$"):
+        return await self.get(f"trees/{forest}/{tree}/{path}")
 
-    def set_value(self, forest:str, tree:str, path:str, value):
-        return self.post(f"trees/{forest}/{tree}/{path}", value)
+    async def set_value(self, forest:str, tree:str, path:str, value):
+        return await self.post(f"trees/{forest}/{tree}/{path}", value)
 
-    def remove_value(self, forest:str, tree:str, path:str):
-        return self.delete(f"trees/{forest}/{tree}/{path}")
+    async def remove_value(self, forest:str, tree:str, path:str):
+        return await self.delete(f"trees/{forest}/{tree}/{path}")
```

### Comparing `pybureaucrat-1.0.8/client/pybureaucrat.egg-info/PKG-INFO` & `pybureaucrat-1.0.9/client/pybureaucrat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybureaucrat
-Version: 1.0.8
+Version: 1.0.9
 Summary: A python client for bureaucrat server
 Home-page: https://github.com/LostSavannah/bureaucrat/tree/main/lib
 Author: Erick Fernando Mora Ramirez
 Author-email: erickfernandomoraramirez@gmail.com
 Project-URL: Bug Tracker, https://dev.moradev.dev/pybureaucrat/issues
 Project-URL: Documentation, https://dev.moradev.dev/pybureaucrat/documentation
 Project-URL: Examples, https://dev.moradev.dev/pybureaucrat/examples
```

### Comparing `pybureaucrat-1.0.8/setup.py` & `pybureaucrat-1.0.9/setup.py`

 * *Files identical despite different names*

