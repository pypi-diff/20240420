# Comparing `tmp/ParendumLib-0.2.1.tar.gz` & `tmp/ParendumLib-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ParendumLib-0.2.1.tar", last modified: Fri Apr 19 11:15:58 2024, max compression
+gzip compressed data, was "ParendumLib-0.2.2.tar", last modified: Sat Apr 20 11:46:47 2024, max compression
```

## Comparing `ParendumLib-0.2.1.tar` & `ParendumLib-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 11:15:58.161274 ParendumLib-0.2.1/
--rw-rw-rw-   0        0        0       41 2024-04-19 11:15:21.000000 ParendumLib-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      233 2024-04-19 11:15:58.161274 ParendumLib-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-19 11:15:58.148883 ParendumLib-0.2.1/ParendumLib.egg-info/
--rw-rw-rw-   0        0        0      233 2024-04-19 11:15:58.000000 ParendumLib-0.2.1/ParendumLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      480 2024-04-19 11:15:58.000000 ParendumLib-0.2.1/ParendumLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 11:15:58.000000 ParendumLib-0.2.1/ParendumLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2024-04-19 11:15:58.000000 ParendumLib-0.2.1/ParendumLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-19 11:15:58.000000 ParendumLib-0.2.1/ParendumLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1323 2024-04-19 11:10:14.000000 ParendumLib-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 11:15:58.158275 ParendumLib-0.2.1/parendumlib/
--rw-rw-rw-   0        0        0      222 2023-12-27 22:30:57.000000 ParendumLib-0.2.1/parendumlib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 11:15:58.159266 ParendumLib-0.2.1/parendumlib/database/
--rw-rw-rw-   0        0        0        0 2023-12-27 20:05:10.000000 ParendumLib-0.2.1/parendumlib/database/__init__.py
--rw-rw-rw-   0        0        0     3458 2023-12-27 20:21:09.000000 ParendumLib-0.2.1/parendumlib/database/mongodb.py
--rw-rw-rw-   0        0        0       55 2023-10-10 13:03:24.000000 ParendumLib-0.2.1/parendumlib/exceptions.py
--rw-rw-rw-   0        0        0     6215 2024-04-19 11:08:15.000000 ParendumLib-0.2.1/parendumlib/logger.py
--rw-rw-rw-   0        0        0     4897 2024-04-19 11:02:59.000000 ParendumLib-0.2.1/parendumlib/mailer.py
-drwxrwxrwx   0        0        0        0 2024-04-19 11:15:58.160281 ParendumLib-0.2.1/parendumlib/permissions/
--rw-rw-rw-   0        0        0        0 2023-12-27 22:27:26.000000 ParendumLib-0.2.1/parendumlib/permissions/__init__.py
--rw-rw-rw-   0        0        0     3273 2023-12-27 22:35:03.000000 ParendumLib-0.2.1/parendumlib/permissions/mongodb.py
--rw-rw-rw-   0        0        0     1483 2023-12-27 22:31:06.000000 ParendumLib-0.2.1/parendumlib/responses.py
--rw-rw-rw-   0        0        0     2089 2023-12-28 22:19:08.000000 ParendumLib-0.2.1/parendumlib/utils.py
--rw-rw-rw-   0        0        0       42 2024-04-19 11:15:58.161274 ParendumLib-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      522 2024-04-19 11:15:44.000000 ParendumLib-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 11:46:47.402623 ParendumLib-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      220 2024-04-20 11:46:47.402623 ParendumLib-0.2.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 11:46:47.400622 ParendumLib-0.2.2/ParendumLib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      220 2024-04-20 11:46:47.000000 ParendumLib-0.2.2/ParendumLib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2024-04-20 11:46:47.000000 ParendumLib-0.2.2/ParendumLib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 11:46:47.000000 ParendumLib-0.2.2/ParendumLib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-20 11:46:47.000000 ParendumLib-0.2.2/ParendumLib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-20 11:46:47.000000 ParendumLib-0.2.2/ParendumLib.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 11:46:47.401622 ParendumLib-0.2.2/parendumlib/
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/parendumlib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 11:46:47.401622 ParendumLib-0.2.2/parendumlib/database/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/parendumlib/database/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3375 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/parendumlib/database/mongodb.py
+-rw-rw-rw-   0 root         (0) root         (0)       53 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/parendumlib/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6063 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/parendumlib/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     4773 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/parendumlib/mailer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 11:46:47.402623 ParendumLib-0.2.2/parendumlib/permissions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/parendumlib/permissions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3179 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/parendumlib/permissions/mongodb.py
+-rw-rw-rw-   0 root         (0) root         (0)     1447 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/parendumlib/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)     2133 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/parendumlib/utils.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 11:46:47.402623 ParendumLib-0.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/setup.py
```

### Comparing `ParendumLib-0.2.1/parendumlib/database/mongodb.py` & `ParendumLib-0.2.2/parendumlib/database/mongodb.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-import motor.motor_asyncio
-from bson.objectid import ObjectId
-
-
-class Mongo:
-
-    def __init__(self, db_name: str, user: str = None, password: str = None, host: str = "127.0.0.1", port: int = 27017):
-        if not user and not password:
-            mongo_uri = f'mongodb://{host}:{port}/{db_name}?authSource=admin'
-        else:
-            mongo_uri = f'mongodb://{user}:{password}@{host}:{port}/{db_name}?authSource=admin'
-        self.db_name = db_name
-        self.client = motor.motor_asyncio.AsyncIOMotorClient(mongo_uri)
-
-    def collection(self, collection_name: str):
-        return getattr(self.client, self.db_name).astra.get_collection(collection_name)
-
-    @staticmethod
-    def parse_helper(result) -> dict:
-        result['_id'] = str(result['_id'])
-        return dict(result)
-
-    async def retrieve_all(self,
-                           collection_name: str,
-                           query: dict = None,
-                           filter_fields: dict = None) -> list:
-        results = []
-        async for result in self.collection(collection_name).find(
-                query, filter_fields):
-            results.append(self.parse_helper(result))
-        return results
-
-    async def retrieve_last(self, collection_name: str, order_field: str) -> dict:
-        result = await self.collection(collection_name).find_one(
-            {}, sort=[(order_field, -1)]
-        )
-        if result:
-            return self.parse_helper(result)
-
-    async def retrieve_one(self, collection_name: str, id_obj: str) -> dict:
-        result = await self.collection(collection_name).find_one(
-            {"_id": ObjectId(id_obj)})
-        if result:
-            return self.parse_helper(result)
-
-    async def add(self, collection_name: str, data: dict) -> dict:
-        result = await self.collection(collection_name).insert_one(data)
-        new_result = await self.collection(collection_name).find_one(
-            {"_id": result.inserted_id})
-        return self.parse_helper(new_result)
-
-    async def update(self, collection_name: str, id_obj: str,
-                     data: dict) -> bool:
-        if len(data) < 1:
-            return False
-        result = await self.collection(collection_name).find_one(
-            {"_id": ObjectId(id_obj)})
-        if result:
-            updated_result = await self.collection(collection_name).update_one(
-                {"_id": ObjectId(id_obj)}, {"$set": data})
-            if updated_result:
-                return True
-            return False
-
-    async def delete(self, collection_name: str, id_obj: str) -> bool:
-        result = await self.collection(collection_name).find_one(
-            {"_id": ObjectId(id_obj)})
-        if result:
-            await self.collection(collection_name).delete_one(
-                {"_id": ObjectId(id_obj)})
-            return True
-
-    async def create_index(self, collection_name: str, field_name: str, seconds: int = 60):
-        await self.collection(collection_name).create_index(
-            [(field_name, 1)],
-            expireAfterSeconds=seconds
-        )
-
-    async def find_limit(self, collection_name: str, start: int = 1, limit: int = 10, query: dict = None):
-        _logs = (await self.retrieve_all(collection_name, query))[::-1]
-        _start_index = (start - 1) * limit
-        _end_index = _start_index + limit
-        return _logs[_start_index:_end_index]
+import motor.motor_asyncio
+from bson.objectid import ObjectId
+
+
+class Mongo:
+
+    def __init__(self, db_name: str, user: str = None, password: str = None, host: str = "127.0.0.1", port: int = 27017):
+        if not user and not password:
+            mongo_uri = f'mongodb://{host}:{port}/{db_name}?authSource=admin'
+        else:
+            mongo_uri = f'mongodb://{user}:{password}@{host}:{port}/{db_name}?authSource=admin'
+        self.db_name = db_name
+        self.client = motor.motor_asyncio.AsyncIOMotorClient(mongo_uri)
+
+    def collection(self, collection_name: str):
+        return getattr(self.client, self.db_name).astra.get_collection(collection_name)
+
+    @staticmethod
+    def parse_helper(result) -> dict:
+        result['_id'] = str(result['_id'])
+        return dict(result)
+
+    async def retrieve_all(self,
+                           collection_name: str,
+                           query: dict = None,
+                           filter_fields: dict = None) -> list:
+        results = []
+        async for result in self.collection(collection_name).find(
+                query, filter_fields):
+            results.append(self.parse_helper(result))
+        return results
+
+    async def retrieve_last(self, collection_name: str, order_field: str) -> dict:
+        result = await self.collection(collection_name).find_one(
+            {}, sort=[(order_field, -1)]
+        )
+        if result:
+            return self.parse_helper(result)
+
+    async def retrieve_one(self, collection_name: str, id_obj: str) -> dict:
+        result = await self.collection(collection_name).find_one(
+            {"_id": ObjectId(id_obj)})
+        if result:
+            return self.parse_helper(result)
+
+    async def add(self, collection_name: str, data: dict) -> dict:
+        result = await self.collection(collection_name).insert_one(data)
+        new_result = await self.collection(collection_name).find_one(
+            {"_id": result.inserted_id})
+        return self.parse_helper(new_result)
+
+    async def update(self, collection_name: str, id_obj: str,
+                     data: dict) -> bool:
+        if len(data) < 1:
+            return False
+        result = await self.collection(collection_name).find_one(
+            {"_id": ObjectId(id_obj)})
+        if result:
+            updated_result = await self.collection(collection_name).update_one(
+                {"_id": ObjectId(id_obj)}, {"$set": data})
+            if updated_result:
+                return True
+            return False
+
+    async def delete(self, collection_name: str, id_obj: str) -> bool:
+        result = await self.collection(collection_name).find_one(
+            {"_id": ObjectId(id_obj)})
+        if result:
+            await self.collection(collection_name).delete_one(
+                {"_id": ObjectId(id_obj)})
+            return True
+
+    async def create_index(self, collection_name: str, field_name: str, seconds: int = 60):
+        await self.collection(collection_name).create_index(
+            [(field_name, 1)],
+            expireAfterSeconds=seconds
+        )
+
+    async def find_limit(self, collection_name: str, start: int = 1, limit: int = 10, query: dict = None):
+        _logs = (await self.retrieve_all(collection_name, query))[::-1]
+        _start_index = (start - 1) * limit
+        _end_index = _start_index + limit
+        return _logs[_start_index:_end_index]
```

### Comparing `ParendumLib-0.2.1/parendumlib/logger.py` & `ParendumLib-0.2.2/parendumlib/logger.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-import threading
-import requests
-import logging
-import hashlib
-import inspect
-import hmac
-import time
-
-
-class Logger:
-
-    def __init__(self, domain: str, api_key: str, api_secret: str, port: int = 443, log_file: str = None):
-        self.protocol = "https" if port == 443 else "http"
-        self.endpoint = f"{self.protocol}://{domain}:{port}"
-        self.api_key = api_key
-        self.api_secret = api_secret.encode()
-
-        self.logger = logging.getLogger()
-        self.logger.setLevel(logging.INFO)
-
-        self.formatter = logging.Formatter('[%(asctime)s] [%(levelname)s] %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
-
-        if log_file:
-            self.file_handler = logging.FileHandler(log_file)
-            self.file_handler.setFormatter(self.formatter)
-            self.logger.addHandler(self.file_handler)
-
-        self.console_handler = logging.StreamHandler()
-        self.console_handler.setFormatter(self.formatter)
-        self.logger.addHandler(self.console_handler)
-
-    def _generate_signature(self, timestamp: str) -> str:
-        """
-        Generate HMAC signature using the provided timestamp.
-
-        Args:
-            timestamp (str): The timestamp to be used in signature generation.
-
-        Returns:
-            str: The generated HMAC signature.
-        """
-        return hmac.new(self.api_secret, timestamp.encode(), digestmod=hashlib.sha256).hexdigest()
-
-    def _get_hmac_headers(self) -> dict:
-        """
-        Generate the HMAC headers required for API requests.
-
-        Returns:
-            dict: A dictionary containing the required headers.
-        """
-        timestamp = str(int(time.time()))
-        return {
-            "X-Signature": self._generate_signature(timestamp),
-            "X-Timestamp": timestamp,
-            "Authorization": f"Bearer {self.api_key}",
-            "Content-Type": "application/json"
-        }
-
-    def _do_post(self, url: str, body: dict = None) -> dict:
-        """
-        Make a POST request to the specified URL.
-
-        Args:
-            url (str): The URL to make the request to.
-            body (dict, optional): The body of the request. Defaults to None.
-
-        Returns:
-            dict: The API response.
-        """
-        try:
-            response = requests.request("POST", url, headers=self._get_hmac_headers(), json=body, timeout=2)
-            if response.status_code == 200:
-                return response.json()
-            return dict(code=response.status_code, error=response.json())
-        except Exception as e:
-            return dict(code=500, error=str(e))
-
-    def _log(self, level: str, function: str, message: str, status_code: int, elapsed_time: int = 1,
-             arguments: list = None, content: dict = None, save: bool = False):
-        _new_log = dict(
-            function=function,
-            message=message,
-            level=level.lower(),
-            status_code=status_code or 0,
-            elapsed_time=elapsed_time
-        )
-        if arguments:
-            _new_log["arguments"] = arguments
-        if content:
-            _new_log["content"] = content
-        if hasattr(self.logger, level):
-            getattr(self.logger, level)(f"[{function}] {message}")
-        else:
-            self.logger.info(f"[{level}:{function}] {message}")
-        if save:
-            self._do_post(f"{self.endpoint}/api/logs/new", _new_log)
-
-    def _do_log(self, level: str, function: str, message: str, status_code: int, elapsed_time: int = 1,
-                arguments: list = None, content: dict = None, save: bool = False):
-        thread = threading.Thread(target=self._log, args=(
-            level, function, message, status_code, elapsed_time, arguments, content, save,
-        ))
-        thread.start()
-
-    def log(self, level: str, message: str, status_code: int = 0, save: bool = False):
-        stack = inspect.stack()
-        caller_info = stack[1]
-        caller_name = caller_info.function
-        caller_line_no = caller_info.lineno
-        self._do_log(level, f"{caller_name}():{caller_line_no}", message, status_code, save=save)
-
-    def success(self, message: str, status_code: int = 0, save: bool = False):
-        stack = inspect.stack()
-        caller_info = stack[1]
-        caller_name = caller_info.function
-        caller_line_no = caller_info.lineno
-        self._do_log('success', f"{caller_name}():{caller_line_no}", message, status_code, save=save)
-
-    def debug(self, message: str, status_code: int = 100, save: bool = False):
-        stack = inspect.stack()
-        caller_info = stack[1]
-        caller_name = caller_info.function
-        caller_line_no = caller_info.lineno
-        self._do_log('debug', f"{caller_name}():{caller_line_no}", message, status_code, save=save)
-
-    def info(self, message: str, status_code: int = 200, save: bool = False):
-        stack = inspect.stack()
-        caller_info = stack[1]
-        caller_name = caller_info.function
-        caller_line_no = caller_info.lineno
-        self._do_log('info', f"{caller_name}():{caller_line_no}", message, status_code, save=save)
-
-    def warning(self, message: str, status_code: int = 400, save: bool = False):
-        stack = inspect.stack()
-        caller_info = stack[1]
-        caller_name = caller_info.function
-        caller_line_no = caller_info.lineno
-        self._do_log('warning', f"{caller_name}():{caller_line_no}", message, status_code, save=save)
-
-    def error(self, message: str, status_code: int = 500, save: bool = False):
-        stack = inspect.stack()
-        caller_info = stack[1]
-        caller_name = caller_info.function
-        caller_line_no = caller_info.lineno
-        self._do_log('error', f"{caller_name}():{caller_line_no}", message, status_code, save=save)
-
-    def exception(self, message: str, status_code: int = 600, save: bool = False):
-        stack = inspect.stack()
-        caller_info = stack[1]
-        caller_name = caller_info.function
-        caller_line_no = caller_info.lineno
-        self._do_log('exception', f"{caller_name}():{caller_line_no}", message, status_code, save=save)
+import threading
+import requests
+import logging
+import hashlib
+import inspect
+import hmac
+import time
+
+
+class Logger:
+
+    def __init__(self, domain: str, api_key: str, api_secret: str, port: int = 443, log_file: str = None):
+        self.protocol = "https" if port == 443 else "http"
+        self.endpoint = f"{self.protocol}://{domain}:{port}"
+        self.api_key = api_key
+        self.api_secret = api_secret.encode()
+
+        self.logger = logging.getLogger()
+        self.logger.setLevel(logging.INFO)
+
+        self.formatter = logging.Formatter('[%(asctime)s] [%(levelname)s] %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+
+        if log_file:
+            self.file_handler = logging.FileHandler(log_file)
+            self.file_handler.setFormatter(self.formatter)
+            self.logger.addHandler(self.file_handler)
+
+        self.console_handler = logging.StreamHandler()
+        self.console_handler.setFormatter(self.formatter)
+        self.logger.addHandler(self.console_handler)
+
+    def _generate_signature(self, timestamp: str) -> str:
+        """
+        Generate HMAC signature using the provided timestamp.
+
+        Args:
+            timestamp (str): The timestamp to be used in signature generation.
+
+        Returns:
+            str: The generated HMAC signature.
+        """
+        return hmac.new(self.api_secret, timestamp.encode(), digestmod=hashlib.sha256).hexdigest()
+
+    def _get_hmac_headers(self) -> dict:
+        """
+        Generate the HMAC headers required for API requests.
+
+        Returns:
+            dict: A dictionary containing the required headers.
+        """
+        timestamp = str(int(time.time()))
+        return {
+            "X-Signature": self._generate_signature(timestamp),
+            "X-Timestamp": timestamp,
+            "Authorization": f"Bearer {self.api_key}",
+            "Content-Type": "application/json"
+        }
+
+    def _do_post(self, url: str, body: dict = None) -> dict:
+        """
+        Make a POST request to the specified URL.
+
+        Args:
+            url (str): The URL to make the request to.
+            body (dict, optional): The body of the request. Defaults to None.
+
+        Returns:
+            dict: The API response.
+        """
+        try:
+            response = requests.request("POST", url, headers=self._get_hmac_headers(), json=body, timeout=2)
+            if response.status_code == 200:
+                return response.json()
+            return dict(code=response.status_code, error=response.json())
+        except Exception as e:
+            return dict(code=500, error=str(e))
+
+    def _log(self, level: str, function: str, message: str, status_code: int, elapsed_time: int = 1,
+             arguments: list = None, content: dict = None, save: bool = False):
+        _new_log = dict(
+            function=function,
+            message=message,
+            level=level.lower(),
+            status_code=status_code or 0,
+            elapsed_time=elapsed_time
+        )
+        if arguments:
+            _new_log["arguments"] = arguments
+        if content:
+            _new_log["content"] = content
+        if hasattr(self.logger, level):
+            getattr(self.logger, level)(f"[{function}] {message}")
+        else:
+            self.logger.info(f"[{level}:{function}] {message}")
+        if save:
+            self._do_post(f"{self.endpoint}/api/logs/new", _new_log)
+
+    def _do_log(self, level: str, function: str, message: str, status_code: int, elapsed_time: int = 1,
+                arguments: list = None, content: dict = None, save: bool = False):
+        thread = threading.Thread(target=self._log, args=(
+            level, function, message, status_code, elapsed_time, arguments, content, save,
+        ))
+        thread.start()
+
+    def log(self, level: str, message: str, status_code: int = 0, save: bool = False):
+        stack = inspect.stack()
+        caller_info = stack[1]
+        caller_name = caller_info.function
+        caller_line_no = caller_info.lineno
+        self._do_log(level, f"{caller_name}():{caller_line_no}", message, status_code, save=save)
+
+    def success(self, message: str, status_code: int = 0, save: bool = False):
+        stack = inspect.stack()
+        caller_info = stack[1]
+        caller_name = caller_info.function
+        caller_line_no = caller_info.lineno
+        self._do_log('success', f"{caller_name}():{caller_line_no}", message, status_code, save=save)
+
+    def debug(self, message: str, status_code: int = 100, save: bool = False):
+        stack = inspect.stack()
+        caller_info = stack[1]
+        caller_name = caller_info.function
+        caller_line_no = caller_info.lineno
+        self._do_log('debug', f"{caller_name}():{caller_line_no}", message, status_code, save=save)
+
+    def info(self, message: str, status_code: int = 200, save: bool = False):
+        stack = inspect.stack()
+        caller_info = stack[1]
+        caller_name = caller_info.function
+        caller_line_no = caller_info.lineno
+        self._do_log('info', f"{caller_name}():{caller_line_no}", message, status_code, save=save)
+
+    def warning(self, message: str, status_code: int = 400, save: bool = False):
+        stack = inspect.stack()
+        caller_info = stack[1]
+        caller_name = caller_info.function
+        caller_line_no = caller_info.lineno
+        self._do_log('warning', f"{caller_name}():{caller_line_no}", message, status_code, save=save)
+
+    def error(self, message: str, status_code: int = 500, save: bool = False):
+        stack = inspect.stack()
+        caller_info = stack[1]
+        caller_name = caller_info.function
+        caller_line_no = caller_info.lineno
+        self._do_log('error', f"{caller_name}():{caller_line_no}", message, status_code, save=save)
+
+    def exception(self, message: str, status_code: int = 600, save: bool = False):
+        stack = inspect.stack()
+        caller_info = stack[1]
+        caller_name = caller_info.function
+        caller_line_no = caller_info.lineno
+        self._do_log('exception', f"{caller_name}():{caller_line_no}", message, status_code, save=save)
```

### Comparing `ParendumLib-0.2.1/parendumlib/permissions/mongodb.py` & `ParendumLib-0.2.2/parendumlib/permissions/mongodb.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-from datetime import datetime, timedelta
-from fastapi import Request
-import socket
-
-from ..utils import format_user_agent
-from ..exceptions import NotAuthenticatedException
-
-
-class Permissions:
-    def __init__(self, db, config: dict):
-        self.db = db
-        self.config = config
-
-    async def get_user_session(self, request: Request):
-        if not (user_session := await self.get_user(request)):
-            raise NotAuthenticatedException()
-        return user_session
-
-    async def get_user(self, request: Request) -> object | None:
-        """
-        Retrieve the user based on the session token from the request.
-        Also updates the last session time for the user's device.
-        """
-        session_token = request.session.get("session_token")
-        if not session_token:
-            return None
-
-        user = await self.__get_user_by_session_token(session_token)
-        if not user:
-            return None
-
-        if self.__is_session_expired(user.get('last_session')):
-            return None
-
-        client_ip = request.client.host
-        proxy_ip = None
-        if forwarded_for := request.headers.get("X-Forwarded-For"):
-            proxy_ip = client_ip
-            client_ip = forwarded_for.split(",")[0].strip()
-        user_agent = format_user_agent(request.headers.get("User-Agent"))
-
-        if proxy_ip and (proxy_ip != self.config.get('endpoint', dict()).get('proxy', '') and proxy_ip != socket.gethostbyname("parendum.com")):
-            print(f"Not authorized proxy tried to connect ({proxy_ip} != {self.config.get('endpoint', dict()).get('proxy', '')})")
-            return None
-
-        if not self.__is_device_valid(user, client_ip, user_agent):
-            return None
-
-        await self.__update_user_last_session(user, client_ip, user_agent)
-        return user
-
-    async def __get_user_by_session_token(self, session_token):
-        """Retrieve a user from the database using the session token."""
-        users = await self.db.retrieve_all('users', dict(session_token=session_token))
-        return users[0] if users else None
-
-    def __is_device_valid(self, user, client_ip, user_agent):
-        """Check if the device is valid for the user."""
-        devices = user.get('devices', [])
-        return any(self.__is_device_match(device, client_ip, user_agent) for device in devices)
-
-    async def __update_user_last_session(self, user, client_ip, user_agent):
-        """Update the last session time for the user's device."""
-        devices = user.get('devices', [])
-        for device in devices:
-            if self.__is_device_match(device, client_ip, user_agent):
-                device['last_session'] = datetime.utcnow()
-        await self.db.update('users', user.get('_id'), dict(last_session=datetime.utcnow(), devices=devices))
-
-    @staticmethod
-    def __is_session_expired(last_session):
-        """Check if the session has expired."""
-        return last_session and datetime.utcnow() - last_session > timedelta(hours=24)
-
-    @staticmethod
-    def __is_device_match(device, client_ip, user_agent):
-        return device.get('client_ip') == client_ip and device.get('user_agent') == user_agent and device.get('is_active')
+from datetime import datetime, timedelta
+from fastapi import Request
+import socket
+
+from ..utils import format_user_agent
+from ..exceptions import NotAuthenticatedException
+
+
+class Permissions:
+    def __init__(self, db, config: dict):
+        self.db = db
+        self.config = config
+
+    async def get_user_session(self, request: Request):
+        if not (user_session := await self.get_user(request)):
+            raise NotAuthenticatedException()
+        return user_session
+
+    async def get_user(self, request: Request):
+        """
+        Retrieve the user based on the session token from the request.
+        Also updates the last session time for the user's device.
+        """
+        session_token = request.session.get("session_token")
+        if not session_token:
+            return None
+
+        user = await self.__get_user_by_session_token(session_token)
+        if not user:
+            return None
+
+        if self.__is_session_expired(user.get('last_session')):
+            return None
+
+        client_ip = request.client.host
+        proxy_ip = None
+        if forwarded_for := request.headers.get("X-Forwarded-For"):
+            proxy_ip = client_ip
+            client_ip = forwarded_for.split(",")[0].strip()
+        user_agent = format_user_agent(request.headers.get("User-Agent"))
+
+        if proxy_ip and (proxy_ip != self.config.get('endpoint', dict()).get('proxy', '') and proxy_ip != socket.gethostbyname("parendum.com")):
+            print(f"Not authorized proxy tried to connect ({proxy_ip} != {self.config.get('endpoint', dict()).get('proxy', '')})")
+            return None
+
+        if not self.__is_device_valid(user, client_ip, user_agent):
+            return None
+
+        await self.__update_user_last_session(user, client_ip, user_agent)
+        return user
+
+    async def __get_user_by_session_token(self, session_token):
+        """Retrieve a user from the database using the session token."""
+        users = await self.db.retrieve_all('users', dict(session_token=session_token))
+        return users[0] if users else None
+
+    def __is_device_valid(self, user, client_ip, user_agent):
+        """Check if the device is valid for the user."""
+        devices = user.get('devices', [])
+        return any(self.__is_device_match(device, client_ip, user_agent) for device in devices)
+
+    async def __update_user_last_session(self, user, client_ip, user_agent):
+        """Update the last session time for the user's device."""
+        devices = user.get('devices', [])
+        for device in devices:
+            if self.__is_device_match(device, client_ip, user_agent):
+                device['last_session'] = datetime.utcnow()
+        await self.db.update('users', user.get('_id'), dict(last_session=datetime.utcnow(), devices=devices))
+
+    @staticmethod
+    def __is_session_expired(last_session):
+        """Check if the session has expired."""
+        return last_session and datetime.utcnow() - last_session > timedelta(hours=24)
+
+    @staticmethod
+    def __is_device_match(device, client_ip, user_agent):
+        return device.get('client_ip') == client_ip and device.get('user_agent') == user_agent and device.get('is_active')
```

### Comparing `ParendumLib-0.2.1/parendumlib/responses.py` & `ParendumLib-0.2.2/parendumlib/responses.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from fastapi.templating import Jinja2Templates
-from fastapi.responses import JSONResponse
-
-
-class Response:
-
-    def __init__(self, config: dict = None, templates_directory: str = None):
-        self.templates = None if not templates_directory else Jinja2Templates(directory=templates_directory)
-        self.config = config or dict()
-
-    def message(self, data, msg, extra: dict = None):
-        return JSONResponse(self.__response_model__(data, msg, extra))
-
-    def render_template(self, file_name: str, context: dict):
-        return self.templates.TemplateResponse(file_name, context)
-
-    def error_message(self, key: str, error_key: str):
-        _msg_data = self.config.get('messages', dict()).get(key, dict())
-        _title = _msg_data.get('title', '<No title defined>')
-        _msg = _msg_data.get('errors', dict()).get(error_key, dict(code=999, message="<No message defined>"))
-        return JSONResponse(self.__error_response_model__(_title, _msg.get('code', 500), _msg.get('message')))
-
-    @staticmethod
-    def __response_model__(data, msg: str = None, extra: dict = None):
-        if not isinstance(data, list):
-            data = [data]
-        res = dict(data=data, code=200)
-        if msg:
-            res["message"] = msg
-        if extra:
-            res.update(extra)
-        return res
-
-    @staticmethod
-    def __error_response_model__(error, code: int, msg):
-        return dict(error=error, code=code, message=msg)
+from fastapi.templating import Jinja2Templates
+from fastapi.responses import JSONResponse
+
+
+class Response:
+
+    def __init__(self, config: dict = None, templates_directory: str = None):
+        self.templates = None if not templates_directory else Jinja2Templates(directory=templates_directory)
+        self.config = config or dict()
+
+    def message(self, data, msg, extra: dict = None):
+        return JSONResponse(self.__response_model__(data, msg, extra))
+
+    def render_template(self, file_name: str, context: dict):
+        return self.templates.TemplateResponse(file_name, context)
+
+    def error_message(self, key: str, error_key: str):
+        _msg_data = self.config.get('messages', dict()).get(key, dict())
+        _title = _msg_data.get('title', '<No title defined>')
+        _msg = _msg_data.get('errors', dict()).get(error_key, dict(code=999, message="<No message defined>"))
+        return JSONResponse(self.__error_response_model__(_title, _msg.get('code', 500), _msg.get('message')))
+
+    @staticmethod
+    def __response_model__(data, msg: str = None, extra: dict = None):
+        if not isinstance(data, list):
+            data = [data]
+        res = dict(data=data, code=200)
+        if msg:
+            res["message"] = msg
+        if extra:
+            res.update(extra)
+        return res
+
+    @staticmethod
+    def __error_response_model__(error, code: int, msg):
+        return dict(error=error, code=code, message=msg)
```

### Comparing `ParendumLib-0.2.1/parendumlib/utils.py` & `ParendumLib-0.2.2/parendumlib/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,71 @@
-import random
-import re
-
-
-def all_required(model: dict, required_args: list):
-    for _req_arg in required_args:
-        if model.get(_req_arg) is None:
-            return False, _req_arg
-    return True, None
-
-
-def detect_browser(user_agent: str):
-    browsers = {
-        'brave': r'Brave',
-        'firefox': r'Firefox',
-        'edge': r'Edg',
-        'safari': r'Safari',
-        'opera': r'Opera|OPR',
-        'internet_explorer': r'MSIE|Trident',
-        'chrome': r'Chrome',
-    }
-
-    for browser, pattern in browsers.items():
-        if re.search(pattern, user_agent):
-            if browser == 'chrome':
-                if 'Edg' not in user_agent and 'Brave' not in user_agent:
-                    return browser
-            elif browser == 'safari':
-                if 'Chrome' not in user_agent and 'Brave' not in user_agent:
-                    return browser
-            else:
-                return browser
-    return 'unknown'
-
-
-def format_user_agent(user_agent: str):
-    _browser = detect_browser(user_agent).capitalize()
-    return " - ".join(user_agent.split('(')[1].split(')')[0].split('; '))
-
-
-def create_string(length: int = 32, lowercase: bool = True, uppercase: bool = True,
-                  numbers: bool = True, symbols: bool = True):
-    if not any([lowercase, uppercase, numbers, symbols]) or length <= 0:
-        return None
-
-    lowercase_set = "abcdefghijklmnopqrstuvwxyz"
-    uppercase_set = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
-    numbers_set = "0123456789"
-    symbols_set = "!@#$%^&*()_-+=<>?"
-
-    first_char_query = ""
-    if lowercase:
-        first_char_query += lowercase_set
-    if uppercase:
-        first_char_query += uppercase_set
-    if numbers:
-        first_char_query += numbers_set
-
-    if length == 1:
-        return random.choice(first_char_query)
-
-    rest_query = first_char_query
-    if symbols:
-        rest_query += symbols_set
-
-    result = random.choice(first_char_query)
-    result += ''.join(random.choice(rest_query) for _ in range(length - 1))
-    return result
+import random
+import re
+
+
+def all_required(model: dict, required_args: list):
+    if model is None:
+        return False, None
+    for _req_arg in required_args:
+        if model.get(_req_arg) is None:
+            return False, _req_arg
+    return True, None
+
+
+def detect_browser(user_agent: str):
+    browsers = {
+        'brave': r'Brave',
+        'firefox': r'Firefox',
+        'edge': r'Edg',
+        'safari': r'Safari',
+        'opera': r'Opera|OPR',
+        'internet_explorer': r'MSIE|Trident',
+        'chrome': r'Chrome',
+    }
+
+    for browser, pattern in browsers.items():
+        if re.search(pattern, user_agent):
+            if browser == 'chrome':
+                if 'Edg' not in user_agent and 'Brave' not in user_agent:
+                    return browser
+            elif browser == 'safari':
+                if 'Chrome' not in user_agent and 'Brave' not in user_agent:
+                    return browser
+            else:
+                return browser
+    return 'unknown'
+
+
+def format_user_agent(user_agent: str):
+    _browser = detect_browser(user_agent).capitalize()
+    return " - ".join(user_agent.split('(')[1].split(')')[0].split('; '))
+
+
+def create_string(length: int = 32, lowercase: bool = True, uppercase: bool = True,
+                  numbers: bool = True, symbols: bool = True):
+    if not any([lowercase, uppercase, numbers, symbols]) or length <= 0:
+        return None
+
+    lowercase_set = "abcdefghijklmnopqrstuvwxyz"
+    uppercase_set = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
+    numbers_set = "0123456789"
+    symbols_set = "!@#$%^&*()_-+=<>?"
+
+    first_char_query = ""
+    if lowercase:
+        first_char_query += lowercase_set
+    if uppercase:
+        first_char_query += uppercase_set
+    if numbers:
+        first_char_query += numbers_set
+
+    if length == 1:
+        return random.choice(first_char_query)
+
+    rest_query = first_char_query
+    if symbols:
+        rest_query += symbols_set
+
+    first_choice = first_char_query if not symbols else rest_query
+    result = random.choice(first_choice)
+    result += ''.join(random.choice(rest_query) for _ in range(length - 1))
+    return result
```

