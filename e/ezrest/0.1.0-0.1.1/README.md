# Comparing `tmp/ezrest-0.1.0.tar.gz` & `tmp/ezrest-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezrest-0.1.0.tar", last modified: Thu Apr 18 21:49:50 2024, max compression
+gzip compressed data, was "ezrest-0.1.1.tar", last modified: Sat Apr 20 14:12:47 2024, max compression
```

## Comparing `ezrest-0.1.0.tar` & `ezrest-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-04-18 21:49:50.378758 ezrest-0.1.0/
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     1071 2024-04-08 18:35:44.000000 ezrest-0.1.0/LICENSE
--rw-r--r--   0 mrf0x     (1000) mrf0x     (1000)     4111 2024-04-18 21:49:50.378758 ezrest-0.1.0/PKG-INFO
-drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-04-18 21:49:50.374758 ezrest-0.1.0/docs/
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     1738 2024-04-18 20:20:47.000000 ezrest-0.1.0/docs/README.md
-drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-04-18 21:49:50.374758 ezrest-0.1.0/ezrest/
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)       22 2024-04-18 21:48:24.000000 ezrest-0.1.0/ezrest/__init__.py
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     9431 2024-04-17 22:49:06.000000 ezrest-0.1.0/ezrest/requests.py
-drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-04-18 21:49:50.374758 ezrest-0.1.0/ezrest.egg-info/
--rw-r--r--   0 mrf0x     (1000) mrf0x     (1000)     4111 2024-04-18 21:49:50.000000 ezrest-0.1.0/ezrest.egg-info/PKG-INFO
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)      224 2024-04-18 21:49:50.000000 ezrest-0.1.0/ezrest.egg-info/SOURCES.txt
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)        1 2024-04-18 21:49:50.000000 ezrest-0.1.0/ezrest.egg-info/dependency_links.txt
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)       63 2024-04-18 21:49:50.000000 ezrest-0.1.0/ezrest.egg-info/requires.txt
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)        7 2024-04-18 21:49:50.000000 ezrest-0.1.0/ezrest.egg-info/top_level.txt
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     1585 2024-04-17 21:49:47.000000 ezrest-0.1.0/pyproject.toml
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)       38 2024-04-18 21:49:50.378758 ezrest-0.1.0/setup.cfg
+drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-04-20 14:12:47.989097 ezrest-0.1.1/
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     1071 2024-04-08 18:35:44.000000 ezrest-0.1.1/LICENSE
+-rw-r--r--   0 mrf0x     (1000) mrf0x     (1000)     4147 2024-04-20 14:12:47.989097 ezrest-0.1.1/PKG-INFO
+drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-04-20 14:12:47.985097 ezrest-0.1.1/docs/
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     1738 2024-04-18 20:20:47.000000 ezrest-0.1.1/docs/README.md
+drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-04-20 14:12:47.985097 ezrest-0.1.1/ezrest/
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)       22 2024-04-20 13:35:49.000000 ezrest-0.1.1/ezrest/__init__.py
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     9776 2024-04-20 14:02:21.000000 ezrest-0.1.1/ezrest/requests.py
+drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-04-20 14:12:47.985097 ezrest-0.1.1/ezrest.egg-info/
+-rw-r--r--   0 mrf0x     (1000) mrf0x     (1000)     4147 2024-04-20 14:12:47.000000 ezrest-0.1.1/ezrest.egg-info/PKG-INFO
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)      224 2024-04-20 14:12:47.000000 ezrest-0.1.1/ezrest.egg-info/SOURCES.txt
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)        1 2024-04-20 14:12:47.000000 ezrest-0.1.1/ezrest.egg-info/dependency_links.txt
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)       68 2024-04-20 14:12:47.000000 ezrest-0.1.1/ezrest.egg-info/requires.txt
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)        7 2024-04-20 14:12:47.000000 ezrest-0.1.1/ezrest.egg-info/top_level.txt
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     1592 2024-04-20 14:01:52.000000 ezrest-0.1.1/pyproject.toml
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)       38 2024-04-20 14:12:47.989097 ezrest-0.1.1/setup.cfg
```

### Comparing `ezrest-0.1.0/LICENSE` & `ezrest-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ezrest-0.1.0/PKG-INFO` & `ezrest-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezrest
-Version: 0.1.0
+Version: 0.1.1
 Summary: Modular Python framework for implementing REST API clients
 Author: Jacek Lewański
 License: MIT License
         
         Copyright (c) 2024 Jacek Lewański
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,14 +38,15 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: httpx; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # ezrest
```

### Comparing `ezrest-0.1.0/docs/README.md` & `ezrest-0.1.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `ezrest-0.1.0/ezrest/requests.py` & `ezrest-0.1.1/ezrest/requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import AsyncIterator, Generic, Iterator, TypeVar
+from typing import Any, AsyncIterator, Generic, Iterator, TypeVar, Union
 from urllib.parse import urlparse, urlunparse
 
 # Represents the type of the REST API response
 # In most cases it will be a JSON response (ie. Dict[str, Any])
 _ResponseType = TypeVar("_ResponseType")
 
 
@@ -122,22 +122,23 @@
             while next_url:
                 response = await self.get(url, *args, **kwargs).json()
                 for item in response.get("items", []):
                     yield item
                 next_url = response.get("next")
         """
         raise NotImplementedError()
+        yield None  # pragma: no cover # supresses mypy error
 
 
 # Types that unify synchronous and asynchronous connector usage in
 # BaseEndpoint class.
-_ConnectorType = TypeVar("_ConnectorType", AsyncConnector, Connector)
+_ConnectorType = TypeVar("_ConnectorType", bound=Union[AsyncConnector, Connector])
 
 
-class BaseEndpoint(Generic[_ConnectorType]):
+class BaseEndpoint(Generic[_ConnectorType, _ResponseType]):
     """
     (Async)Endpoint [Builder]
 
     This class allows for generating endpoint URLs dynamically without
     hardcoding endpoint suffixes and uses (Async)Connector instance to
     perform requests.
 
@@ -153,15 +154,15 @@
 
     Examples:
 
     base_url = 'http://x.com/'
 
     connector = Connector[Dict[str, Any]] ()
 
-    api_root = Endpoint(base_url, connector)
+    api_root = Endpoint[Dict[str, Any]](base_url, connector)
 
     api_root                # http://x.com/
     api_root.posts          # http://x.com/posts
     api_root.comments[3]    # http://x.com/comments/3
     api_root["comments"][3] # http://x.com/comments/3
 
     api_root.comments.3     # Not allowed, 3 is not a string type
@@ -187,24 +188,24 @@
         path = parsed_url.path
         while path.endswith("/"):
             path = path[:-1]
         return urlunparse(
             parsed_url._replace(path=path, params="", query="", fragment="")
         )
 
-    def _generate_endpoint(self, name: str):
+    def _generate_endpoint(self, name: Any):
         """
         Creates new endpoint object (for subresources) with:
         - the same type as the parent endpoint object
         - the same instance of the connector
         - name of the resource appended at the end of the URL
         """
         return type(self)(self._get_sub_resource_url(name), self.connector)
 
-    def _get_sub_resource_url(self, name: str) -> str:
+    def _get_sub_resource_url(self, name: Any) -> str:
         """
         Generates new URL with the name of the resource appended at the end
         """
         return f"{self.url}/{str(name)}"
 
     __getattr__ = __getitem__ = _generate_endpoint
 
@@ -230,16 +231,22 @@
 
     def list(self, *args, **kwargs):
         """Runs connector's list method to retrieve items one-by-one"""
         return self.connector.list(self.url, *args, **kwargs)
 
 
 # Type aliases that are more convenient to use.
-# If the response type is Dict[str, Any] ,
-# then you can define them like this:
+# If the response type is Dict[str, Any],
+# instantiation will look like this:
 #
-# class MyEndpoint(Endpoint[Dict[str, Any]])
-# OR
-# class MyAsyncEndpoint(AsyncEndpoint[Dict[str, Any]])
+# endpoint = endpoint = Endpoint[Dict[str, Any]](url, Connector())
+# async_endpoint = AsyncEndpoint[Dict[str, Any]](url, AsyncConnector())
 #
-Endpoint = BaseEndpoint[Connector[_ResponseType]]
-AsyncEndpoint = BaseEndpoint[AsyncConnector[_ResponseType]]
+# and inheritance will look like this:
+#
+# class MyEndpoint(Endpoint[Dict[str, Any]]):
+#     ...
+# class MyAsyncEndpoint(AsyncEndpoint[Dict[str, Any]]):
+#     ...
+#
+Endpoint = BaseEndpoint[Connector[_ResponseType], _ResponseType]
+AsyncEndpoint = BaseEndpoint[AsyncConnector[_ResponseType], _ResponseType]
```

### Comparing `ezrest-0.1.0/ezrest.egg-info/PKG-INFO` & `ezrest-0.1.1/ezrest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezrest
-Version: 0.1.0
+Version: 0.1.1
 Summary: Modular Python framework for implementing REST API clients
 Author: Jacek Lewański
 License: MIT License
         
         Copyright (c) 2024 Jacek Lewański
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,14 +38,15 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: httpx; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # ezrest
```

### Comparing `ezrest-0.1.0/pyproject.toml` & `ezrest-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 [project.urls]
 Homepage = "https://github.com/nullJaX/ezrest"
 Documentation = "https://nullJaX.github.io/ezrest"
 Issues = "https://github.com/nullJaX/ezrest/issues"
 "Release notes" = "https://github.com/nullJaX/ezrest/releases"
 
 [project.optional-dependencies]
-dev = ["build", "httpx", "pytest", "pytest-asyncio", "pytest-cov", "ruff", "twine"]
+dev = ["build", "httpx", "mypy", "pytest", "pytest-asyncio", "pytest-cov", "ruff", "twine"]
 
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools >= 61.0"]
 
 [tool.setuptools]
 packages = ["ezrest"]
 
 [tool.setuptools.dynamic]
 version = {attr = "ezrest.__version__"}
 
 [tool.coverage.report]
-exclude_lines = ["pass"]
+exclude_also = ["pass"]
 fail_under = 90
 show_missing = true
 skip_covered = true
 skip_empty = true
 
 [tool.coverage.run]
 branch = true
```

