# Comparing `tmp/hltv_async_api-0.6.1.tar.gz` & `tmp/hltv_async_api-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.6.1.tar", max compression
+gzip compressed data, was "hltv_async_api-0.6.2.tar", max compression
```

## Comparing `hltv_async_api-0.6.1.tar` & `hltv_async_api-0.6.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      124 2024-04-18 21:30:05.353310 hltv_async_api-0.6.1/hltv_async_api/__init__.py
--rw-r--r--   0        0        0    38550 2024-04-18 21:51:53.449078 hltv_async_api-0.6.1/hltv_async_api/aiohltv.py
--rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.6.1/LICENSE
--rw-r--r--   0        0        0      648 2024-04-18 21:30:05.359311 hltv_async_api-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    15314 2024-04-18 21:50:02.092187 hltv_async_api-0.6.1/README.md
--rw-r--r--   0        0        0    15827 1970-01-01 00:00:00.000000 hltv_async_api-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      124 2024-04-18 21:30:05.353310 hltv_async_api-0.6.2/hltv_async_api/__init__.py
+-rw-r--r--   0        0        0    38547 2024-04-20 14:54:15.471310 hltv_async_api-0.6.2/hltv_async_api/aiohltv.py
+-rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.6.2/LICENSE
+-rw-r--r--   0        0        0      648 2024-04-20 14:55:02.780232 hltv_async_api-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0    15314 2024-04-18 21:50:02.092187 hltv_async_api-0.6.2/README.md
+-rw-r--r--   0        0        0    15827 1970-01-01 00:00:00.000000 hltv_async_api-0.6.2/PKG-INFO
```

### Comparing `hltv_async_api-0.6.1/hltv_async_api/aiohltv.py` & `hltv_async_api-0.6.2/hltv_async_api/aiohltv.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         self.PROXY_ONCE = proxy_one_time
 
         if self.PROXY_PATH:
             with open(self.PROXY_PATH, "r") as file:
                     self.PROXY_LIST = [line.strip() for line in file.readlines()]
 
         if self.PROXY_PROTOCOL:
-            self.PROXY_LIST = [self.PROXY_PROTOCOL + '://' + proxy[i] for i, proxy in enumerate(self.PROXY_LIST, start=0)]
+            self.PROXY_LIST = [self.PROXY_PROTOCOL + '://' + proxy for i, proxy in enumerate(self.PROXY_LIST, start=0)]
 
         if proxy_path or proxy_list:
             self.USE_PROXY = True
         else:
             self.USE_PROXY = False
 
         self.session = None
```

### Comparing `hltv_async_api-0.6.1/LICENSE` & `hltv_async_api-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.6.1/pyproject.toml` & `hltv_async_api-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hltv_async_api"
-version = "0.6.1"
+version = "0.6.2"
 authors = ["Akim Slys <akimslys2003@gmail.com>"]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `hltv_async_api-0.6.1/README.md` & `hltv_async_api-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.6.1/PKG-INFO` & `hltv_async_api-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.6.1
+Version: 0.6.2
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Author: Akim Slys
 Author-email: akimslys2003@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

