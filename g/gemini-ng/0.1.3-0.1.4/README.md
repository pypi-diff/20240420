# Comparing `tmp/gemini_ng-0.1.3.tar.gz` & `tmp/gemini_ng-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini_ng-0.1.3.tar", last modified: Wed Apr 17 17:04:36 2024, max compression
+gzip compressed data, was "gemini_ng-0.1.4.tar", last modified: Sat Apr 20 17:21:03 2024, max compression
```

## Comparing `gemini_ng-0.1.3.tar` & `gemini_ng-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-17 17:04:36.996065 gemini_ng-0.1.3/
--rw-r--r--   0 viv        (501) staff       (20)     1053 2024-04-15 16:41:45.000000 gemini_ng-0.1.3/LICENSE
--rw-r--r--   0 viv        (501) staff       (20)     3128 2024-04-17 17:04:36.995677 gemini_ng-0.1.3/PKG-INFO
--rw-r--r--   0 viv        (501) staff       (20)     1019 2024-04-15 16:43:10.000000 gemini_ng-0.1.3/README.md
--rw-r--r--   0 viv        (501) staff       (20)     1012 2024-04-15 16:16:28.000000 gemini_ng-0.1.3/pyproject.toml
--rw-r--r--   0 viv        (501) staff       (20)       38 2024-04-17 17:04:36.996124 gemini_ng-0.1.3/setup.cfg
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-17 17:04:36.987503 gemini_ng-0.1.3/src/
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-17 17:04:36.989158 gemini_ng-0.1.3/src/gemini_ng/
--rw-r--r--   0 viv        (501) staff       (20)       56 2024-04-17 17:03:58.000000 gemini_ng-0.1.3/src/gemini_ng/__init__.py
--rw-r--r--   0 viv        (501) staff       (20)     1693 2024-04-17 12:11:24.000000 gemini_ng-0.1.3/src/gemini_ng/chat.py
--rw-r--r--   0 viv        (501) staff       (20)     8172 2024-04-17 12:11:51.000000 gemini_ng-0.1.3/src/gemini_ng/client.py
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-17 17:04:36.993202 gemini_ng-0.1.3/src/gemini_ng/schemas/
--rw-r--r--   0 viv        (501) staff       (20)      385 2024-04-17 12:08:05.000000 gemini_ng-0.1.3/src/gemini_ng/schemas/__init__.py
--rw-r--r--   0 viv        (501) staff       (20)      140 2024-04-14 15:18:05.000000 gemini_ng-0.1.3/src/gemini_ng/schemas/base.py
--rw-r--r--   0 viv        (501) staff       (20)     1134 2024-04-14 16:13:55.000000 gemini_ng-0.1.3/src/gemini_ng/schemas/harm.py
--rw-r--r--   0 viv        (501) staff       (20)      922 2024-04-14 19:14:33.000000 gemini_ng-0.1.3/src/gemini_ng/schemas/part.py
--rw-r--r--   0 viv        (501) staff       (20)     2842 2024-04-17 12:11:02.000000 gemini_ng-0.1.3/src/gemini_ng/schemas/request.py
--rw-r--r--   0 viv        (501) staff       (20)     1441 2024-04-15 16:14:16.000000 gemini_ng-0.1.3/src/gemini_ng/schemas/response.py
--rw-r--r--   0 viv        (501) staff       (20)     1636 2024-04-14 18:15:51.000000 gemini_ng-0.1.3/src/gemini_ng/schemas/upload.py
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-17 17:04:36.994521 gemini_ng-0.1.3/src/gemini_ng/utils/
--rw-r--r--   0 viv        (501) staff       (20)        0 2024-04-14 19:17:31.000000 gemini_ng-0.1.3/src/gemini_ng/utils/__init__.py
--rw-r--r--   0 viv        (501) staff       (20)      509 2024-04-15 16:23:14.000000 gemini_ng-0.1.3/src/gemini_ng/utils/cache.py
--rw-r--r--   0 viv        (501) staff       (20)     1435 2024-04-15 15:33:21.000000 gemini_ng-0.1.3/src/gemini_ng/utils/error.py
--rw-r--r--   0 viv        (501) staff       (20)     2027 2024-04-17 17:03:54.000000 gemini_ng-0.1.3/src/gemini_ng/utils/video.py
-drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-17 17:04:36.995262 gemini_ng-0.1.3/src/gemini_ng.egg-info/
--rw-r--r--   0 viv        (501) staff       (20)     3128 2024-04-17 17:04:36.000000 gemini_ng-0.1.3/src/gemini_ng.egg-info/PKG-INFO
--rw-r--r--   0 viv        (501) staff       (20)      640 2024-04-17 17:04:36.000000 gemini_ng-0.1.3/src/gemini_ng.egg-info/SOURCES.txt
--rw-r--r--   0 viv        (501) staff       (20)        1 2024-04-17 17:04:36.000000 gemini_ng-0.1.3/src/gemini_ng.egg-info/dependency_links.txt
--rw-r--r--   0 viv        (501) staff       (20)      137 2024-04-17 17:04:36.000000 gemini_ng-0.1.3/src/gemini_ng.egg-info/requires.txt
--rw-r--r--   0 viv        (501) staff       (20)       10 2024-04-17 17:04:36.000000 gemini_ng-0.1.3/src/gemini_ng.egg-info/top_level.txt
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-20 17:21:03.661605 gemini_ng-0.1.4/
+-rw-r--r--   0 viv        (501) staff       (20)     1053 2024-04-15 16:41:45.000000 gemini_ng-0.1.4/LICENSE
+-rw-r--r--   0 viv        (501) staff       (20)     3128 2024-04-20 17:21:03.661352 gemini_ng-0.1.4/PKG-INFO
+-rw-r--r--   0 viv        (501) staff       (20)     1019 2024-04-15 16:43:10.000000 gemini_ng-0.1.4/README.md
+-rw-r--r--   0 viv        (501) staff       (20)     1012 2024-04-15 16:16:28.000000 gemini_ng-0.1.4/pyproject.toml
+-rw-r--r--   0 viv        (501) staff       (20)       38 2024-04-20 17:21:03.661645 gemini_ng-0.1.4/setup.cfg
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-20 17:21:03.654183 gemini_ng-0.1.4/src/
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-20 17:21:03.656815 gemini_ng-0.1.4/src/gemini_ng/
+-rw-r--r--   0 viv        (501) staff       (20)       56 2024-04-20 17:12:31.000000 gemini_ng-0.1.4/src/gemini_ng/__init__.py
+-rw-r--r--   0 viv        (501) staff       (20)     1693 2024-04-17 12:11:24.000000 gemini_ng-0.1.4/src/gemini_ng/chat.py
+-rw-r--r--   0 viv        (501) staff       (20)     8590 2024-04-20 17:19:47.000000 gemini_ng-0.1.4/src/gemini_ng/client.py
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-20 17:21:03.659755 gemini_ng-0.1.4/src/gemini_ng/schemas/
+-rw-r--r--   0 viv        (501) staff       (20)      414 2024-04-20 17:09:53.000000 gemini_ng-0.1.4/src/gemini_ng/schemas/__init__.py
+-rw-r--r--   0 viv        (501) staff       (20)      140 2024-04-14 15:18:05.000000 gemini_ng-0.1.4/src/gemini_ng/schemas/base.py
+-rw-r--r--   0 viv        (501) staff       (20)     1134 2024-04-14 16:13:55.000000 gemini_ng-0.1.4/src/gemini_ng/schemas/harm.py
+-rw-r--r--   0 viv        (501) staff       (20)      922 2024-04-14 19:14:33.000000 gemini_ng-0.1.4/src/gemini_ng/schemas/part.py
+-rw-r--r--   0 viv        (501) staff       (20)     1265 2024-04-20 17:14:13.000000 gemini_ng-0.1.4/src/gemini_ng/schemas/proxy.py
+-rw-r--r--   0 viv        (501) staff       (20)     2842 2024-04-17 12:11:02.000000 gemini_ng-0.1.4/src/gemini_ng/schemas/request.py
+-rw-r--r--   0 viv        (501) staff       (20)     1441 2024-04-15 16:14:16.000000 gemini_ng-0.1.4/src/gemini_ng/schemas/response.py
+-rw-r--r--   0 viv        (501) staff       (20)     1636 2024-04-14 18:15:51.000000 gemini_ng-0.1.4/src/gemini_ng/schemas/upload.py
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-20 17:21:03.660661 gemini_ng-0.1.4/src/gemini_ng/utils/
+-rw-r--r--   0 viv        (501) staff       (20)        0 2024-04-14 19:17:31.000000 gemini_ng-0.1.4/src/gemini_ng/utils/__init__.py
+-rw-r--r--   0 viv        (501) staff       (20)      509 2024-04-15 16:23:14.000000 gemini_ng-0.1.4/src/gemini_ng/utils/cache.py
+-rw-r--r--   0 viv        (501) staff       (20)     1435 2024-04-15 15:33:21.000000 gemini_ng-0.1.4/src/gemini_ng/utils/error.py
+-rw-r--r--   0 viv        (501) staff       (20)     2027 2024-04-17 17:03:54.000000 gemini_ng-0.1.4/src/gemini_ng/utils/video.py
+drwxr-xr-x   0 viv        (501) staff       (20)        0 2024-04-20 17:21:03.660959 gemini_ng-0.1.4/src/gemini_ng.egg-info/
+-rw-r--r--   0 viv        (501) staff       (20)     3128 2024-04-20 17:21:03.000000 gemini_ng-0.1.4/src/gemini_ng.egg-info/PKG-INFO
+-rw-r--r--   0 viv        (501) staff       (20)      671 2024-04-20 17:21:03.000000 gemini_ng-0.1.4/src/gemini_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 viv        (501) staff       (20)        1 2024-04-20 17:21:03.000000 gemini_ng-0.1.4/src/gemini_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 viv        (501) staff       (20)      137 2024-04-20 17:21:03.000000 gemini_ng-0.1.4/src/gemini_ng.egg-info/requires.txt
+-rw-r--r--   0 viv        (501) staff       (20)       10 2024-04-20 17:21:03.000000 gemini_ng-0.1.4/src/gemini_ng.egg-info/top_level.txt
```

### Comparing `gemini_ng-0.1.3/LICENSE` & `gemini_ng-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.1.3/PKG-INFO` & `gemini_ng-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini-ng
-Version: 0.1.3
+Version: 0.1.4
 Summary: Next-generation Gemini API Client
 Author-email: Ming Yang <ymviv@qq.com>
 License: Copyright (c) 2024 Ming Yang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `gemini_ng-0.1.3/README.md` & `gemini_ng-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.1.3/pyproject.toml` & `gemini_ng-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.1.3/src/gemini_ng/chat.py` & `gemini_ng-0.1.4/src/gemini_ng/chat.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.1.3/src/gemini_ng/client.py` & `gemini_ng-0.1.4/src/gemini_ng/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import hashlib
 import os
 import tempfile
 
+import httplib2
 import requests
 import googleapiclient.discovery as g_discovery
 from tqdm import tqdm
 
 from .chat import ChatSession
 from .schemas import (
     ChatMessage,
@@ -17,41 +18,52 @@
     SafetySetting,
     TextPart,
     ImagePart,
     FilePart,
     VideoPart,
     UploadFile,
     UploadedFile,
+    ProxyInfo,
 )
 from .utils.cache import get_cache_instance
 from .utils.error import handle_http_exception
 from .utils.video import extract_video_frames
 
 
 class GeminiClient:
     def __init__(
         self,
         api_key: str | None = None,
         version: str = "v1beta",
+        proxy_info: ProxyInfo | dict | None = None,
+        timeout: int | None = None,
     ):
         api_key = api_key or os.getenv("GEMINI_NG_API_KEY")
 
         if api_key is None:
             raise ValueError("Gemini API (`GEMINI_NG_API_KEY`) key must be provided")
 
         self.api_key = api_key
 
         rsp = requests.get(
             "https://generativelanguage.googleapis.com/$discovery/rest",
             params={"version": version, "key": api_key},
         )
         rsp.raise_for_status()
 
+        if proxy_info is not None:
+            if not isinstance(proxy_info, ProxyInfo):
+                proxy_info = ProxyInfo.model_validate(proxy_info)
+
+            proxy_info = proxy_info.to_httplib2_proxy_info()
+
+        http = httplib2.Http(timeout=timeout, proxy_info=proxy_info)
+
         self.genai_service = g_discovery.build_from_document(
-            rsp.content, developerKey=api_key
+            rsp.content, developerKey=api_key, http=http
         )
 
     @staticmethod
     def normalize_prompt(prompt: list | str) -> list:
         parts = []
 
         if isinstance(prompt, str):
```

### Comparing `gemini_ng-0.1.3/src/gemini_ng/schemas/harm.py` & `gemini_ng-0.1.4/src/gemini_ng/schemas/harm.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.1.3/src/gemini_ng/schemas/part.py` & `gemini_ng-0.1.4/src/gemini_ng/schemas/part.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.1.3/src/gemini_ng/schemas/request.py` & `gemini_ng-0.1.4/src/gemini_ng/schemas/request.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.1.3/src/gemini_ng/schemas/response.py` & `gemini_ng-0.1.4/src/gemini_ng/schemas/response.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.1.3/src/gemini_ng/schemas/upload.py` & `gemini_ng-0.1.4/src/gemini_ng/schemas/upload.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.1.3/src/gemini_ng/utils/error.py` & `gemini_ng-0.1.4/src/gemini_ng/utils/error.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.1.3/src/gemini_ng/utils/video.py` & `gemini_ng-0.1.4/src/gemini_ng/utils/video.py`

 * *Files identical despite different names*

### Comparing `gemini_ng-0.1.3/src/gemini_ng.egg-info/PKG-INFO` & `gemini_ng-0.1.4/src/gemini_ng.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini-ng
-Version: 0.1.3
+Version: 0.1.4
 Summary: Next-generation Gemini API Client
 Author-email: Ming Yang <ymviv@qq.com>
 License: Copyright (c) 2024 Ming Yang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `gemini_ng-0.1.3/src/gemini_ng.egg-info/SOURCES.txt` & `gemini_ng-0.1.4/src/gemini_ng.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/gemini_ng.egg-info/dependency_links.txt
 src/gemini_ng.egg-info/requires.txt
 src/gemini_ng.egg-info/top_level.txt
 src/gemini_ng/schemas/__init__.py
 src/gemini_ng/schemas/base.py
 src/gemini_ng/schemas/harm.py
 src/gemini_ng/schemas/part.py
+src/gemini_ng/schemas/proxy.py
 src/gemini_ng/schemas/request.py
 src/gemini_ng/schemas/response.py
 src/gemini_ng/schemas/upload.py
 src/gemini_ng/utils/__init__.py
 src/gemini_ng/utils/cache.py
 src/gemini_ng/utils/error.py
 src/gemini_ng/utils/video.py
```

