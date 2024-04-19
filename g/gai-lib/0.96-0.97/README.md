# Comparing `tmp/gai-lib-0.96.tar.gz` & `tmp/gai-lib-0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gai-lib-0.96.tar", last modified: Tue Apr  2 15:38:08 2024, max compression
+gzip compressed data, was "gai-lib-0.97.tar", last modified: Fri Apr 19 22:08:43 2024, max compression
```

## Comparing `gai-lib-0.96.tar` & `gai-lib-0.97.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-02 15:38:08.922034 gai-lib-0.96/
--rw-r--r--   0 roylai    (1000) roylai    (1000)       57 2024-02-20 05:11:48.000000 gai-lib-0.96/MANIFEST.in
--rw-r--r--   0 roylai    (1000) roylai    (1000)      921 2024-04-02 15:38:08.922034 gai-lib-0.96/PKG-INFO
--rw-r--r--   0 roylai    (1000) roylai    (1000)        4 2024-04-02 15:38:04.000000 gai-lib-0.96/VERSION
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-02 15:38:08.922034 gai-lib-0.96/gai/
--rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.96/gai/__init__.py
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-02 15:38:08.922034 gai-lib-0.96/gai/common/
--rw-r--r--   0 roylai    (1000) roylai    (1000)      930 2024-02-20 08:56:16.000000 gai-lib-0.96/gai/common/StatusListener.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1842 2024-02-20 08:56:16.000000 gai-lib-0.96/gai/common/StatusUpdater.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-20 08:56:16.000000 gai-lib-0.96/gai/common/__init__.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)       20 2024-02-20 08:56:16.000000 gai-lib-0.96/gai/common/constants.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     3188 2024-02-24 08:29:07.000000 gai-lib-0.96/gai/common/errors.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     4222 2024-02-22 17:41:30.000000 gai-lib-0.96/gai/common/file_utils.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     5369 2024-04-02 15:12:34.000000 gai-lib-0.96/gai/common/generators_utils.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     7950 2024-03-17 16:20:07.000000 gai-lib-0.96/gai/common/http_utils.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1131 2024-02-20 09:56:37.000000 gai-lib-0.96/gai/common/image_utils.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1417 2024-03-25 15:14:40.000000 gai-lib-0.96/gai/common/logging.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     2712 2024-02-20 09:56:46.000000 gai-lib-0.96/gai/common/overlap_splitter.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1244 2024-02-20 09:56:53.000000 gai-lib-0.96/gai/common/sound_utils.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     3192 2024-02-20 08:56:16.000000 gai-lib-0.96/gai/common/utils.py
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-02 15:38:08.922034 gai-lib-0.96/gai/lib/
--rw-r--r--   0 roylai    (1000) roylai    (1000)      479 2024-02-20 10:00:58.000000 gai-lib-0.96/gai/lib/ClientBase.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     4158 2024-02-23 13:22:53.000000 gai-lib-0.96/gai/lib/GGG.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     2631 2024-02-20 09:54:00.000000 gai-lib-0.96/gai/lib/ITTClient.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     5600 2024-02-23 16:05:13.000000 gai-lib-0.96/gai/lib/RAGClientAsync.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     8481 2024-02-25 05:19:13.000000 gai-lib-0.96/gai/lib/RAGClientSync.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     2518 2024-02-20 09:55:02.000000 gai-lib-0.96/gai/lib/STTClient.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1724 2024-02-20 09:55:02.000000 gai-lib-0.96/gai/lib/TTSClient.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.96/gai/lib/__init__.py
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-02 15:38:08.922034 gai-lib-0.96/gai/lib/ttt/
--rw-r--r--   0 roylai    (1000) roylai    (1000)      211 2024-02-19 19:45:33.000000 gai-lib-0.96/gai/lib/ttt/AnthropicChunkWrapper.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1260 2024-02-19 19:45:33.000000 gai-lib-0.96/gai/lib/ttt/ChunkWrapper.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)      222 2024-02-19 19:45:33.000000 gai-lib-0.96/gai/lib/ttt/OpenAIChunkWrapper.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     6896 2024-04-02 15:36:56.000000 gai-lib-0.96/gai/lib/ttt/TTTClient.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.96/gai/lib/ttt/__init__.py
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-02 15:38:08.922034 gai-lib-0.96/gai/tools/
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1013 2024-02-22 17:41:40.000000 gai-lib-0.96/gai/tools/Chunker.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1619 2024-03-14 05:24:24.000000 gai-lib-0.96/gai/tools/Googler.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)      388 2024-02-19 19:45:33.000000 gai-lib-0.96/gai/tools/PDFConvert.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     2513 2024-02-19 19:45:33.000000 gai-lib-0.96/gai/tools/Scraper.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.96/gai/tools/__init__.py
--rw-r--r--   0 roylai    (1000) roylai    (1000)     3150 2024-03-17 16:29:06.000000 gai-lib-0.96/gai.yml
-drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-02 15:38:08.922034 gai-lib-0.96/gai_lib.egg-info/
--rw-r--r--   0 roylai    (1000) roylai    (1000)      921 2024-04-02 15:38:08.000000 gai-lib-0.96/gai_lib.egg-info/PKG-INFO
--rw-r--r--   0 roylai    (1000) roylai    (1000)     1016 2024-04-02 15:38:08.000000 gai-lib-0.96/gai_lib.egg-info/SOURCES.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)        1 2024-04-02 15:38:08.000000 gai-lib-0.96/gai_lib.egg-info/dependency_links.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)      265 2024-04-02 15:38:08.000000 gai-lib-0.96/gai_lib.egg-info/entry_points.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)       88 2024-04-02 15:38:08.000000 gai-lib-0.96/gai_lib.egg-info/requires.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)        4 2024-04-02 15:38:08.000000 gai-lib-0.96/gai_lib.egg-info/top_level.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)      120 2024-03-25 14:35:24.000000 gai-lib-0.96/requirements.txt
--rw-r--r--   0 roylai    (1000) roylai    (1000)       38 2024-04-02 15:38:08.922034 gai-lib-0.96/setup.cfg
--rw-r--r--   0 roylai    (1000) roylai    (1000)     2881 2024-03-25 14:35:01.000000 gai-lib-0.96/setup.py
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-19 22:08:43.367512 gai-lib-0.97/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)       57 2024-02-20 05:11:48.000000 gai-lib-0.97/MANIFEST.in
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      921 2024-04-19 22:08:43.367512 gai-lib-0.97/PKG-INFO
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        4 2024-04-19 22:04:19.000000 gai-lib-0.97/VERSION
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-19 22:08:43.367512 gai-lib-0.97/gai/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.97/gai/__init__.py
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-19 22:08:43.367512 gai-lib-0.97/gai/common/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1040 2024-04-19 21:38:04.000000 gai-lib-0.97/gai/common/StatusListener.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1842 2024-02-20 08:56:16.000000 gai-lib-0.97/gai/common/StatusUpdater.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-20 08:56:16.000000 gai-lib-0.97/gai/common/__init__.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)       20 2024-02-20 08:56:16.000000 gai-lib-0.97/gai/common/constants.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     3188 2024-02-24 08:29:07.000000 gai-lib-0.97/gai/common/errors.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     4222 2024-02-22 17:41:30.000000 gai-lib-0.97/gai/common/file_utils.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     5369 2024-04-02 15:12:34.000000 gai-lib-0.97/gai/common/generators_utils.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     8401 2024-04-19 21:57:05.000000 gai-lib-0.97/gai/common/http_utils.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1131 2024-02-20 09:56:37.000000 gai-lib-0.97/gai/common/image_utils.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1417 2024-03-25 15:14:40.000000 gai-lib-0.97/gai/common/logging.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     2712 2024-02-20 09:56:46.000000 gai-lib-0.97/gai/common/overlap_splitter.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1244 2024-02-20 09:56:53.000000 gai-lib-0.97/gai/common/sound_utils.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     3192 2024-02-20 08:56:16.000000 gai-lib-0.97/gai/common/utils.py
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-19 22:08:43.367512 gai-lib-0.97/gai/lib/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      479 2024-02-20 10:00:58.000000 gai-lib-0.97/gai/lib/ClientBase.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     4158 2024-02-23 13:22:53.000000 gai-lib-0.97/gai/lib/GGG.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     2631 2024-02-20 09:54:00.000000 gai-lib-0.97/gai/lib/ITTClient.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     4382 2024-04-19 21:59:14.000000 gai-lib-0.97/gai/lib/RAGClientAsync.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     7499 2024-04-19 21:19:32.000000 gai-lib-0.97/gai/lib/RAGClientSync.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     2518 2024-02-20 09:55:02.000000 gai-lib-0.97/gai/lib/STTClient.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1724 2024-02-20 09:55:02.000000 gai-lib-0.97/gai/lib/TTSClient.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.97/gai/lib/__init__.py
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-19 22:08:43.367512 gai-lib-0.97/gai/lib/ttt/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      211 2024-02-19 19:45:33.000000 gai-lib-0.97/gai/lib/ttt/AnthropicChunkWrapper.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1260 2024-02-19 19:45:33.000000 gai-lib-0.97/gai/lib/ttt/ChunkWrapper.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      222 2024-02-19 19:45:33.000000 gai-lib-0.97/gai/lib/ttt/OpenAIChunkWrapper.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     7026 2024-04-16 11:50:57.000000 gai-lib-0.97/gai/lib/ttt/TTTClient.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.97/gai/lib/ttt/__init__.py
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-19 22:08:43.367512 gai-lib-0.97/gai/tools/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1013 2024-02-22 17:41:40.000000 gai-lib-0.97/gai/tools/Chunker.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1619 2024-03-14 05:24:24.000000 gai-lib-0.97/gai/tools/Googler.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      388 2024-02-19 19:45:33.000000 gai-lib-0.97/gai/tools/PDFConvert.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     2513 2024-02-19 19:45:33.000000 gai-lib-0.97/gai/tools/Scraper.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        0 2024-02-19 19:45:33.000000 gai-lib-0.97/gai/tools/__init__.py
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     3178 2024-04-19 22:01:42.000000 gai-lib-0.97/gai.yml
+drwxr-xr-x   0 roylai    (1000) roylai    (1000)        0 2024-04-19 22:08:43.367512 gai-lib-0.97/gai_lib.egg-info/
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      921 2024-04-19 22:08:43.000000 gai-lib-0.97/gai_lib.egg-info/PKG-INFO
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     1016 2024-04-19 22:08:43.000000 gai-lib-0.97/gai_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        1 2024-04-19 22:08:43.000000 gai-lib-0.97/gai_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      265 2024-04-19 22:08:43.000000 gai-lib-0.97/gai_lib.egg-info/entry_points.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)       88 2024-04-19 22:08:43.000000 gai-lib-0.97/gai_lib.egg-info/requires.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)        4 2024-04-19 22:08:43.000000 gai-lib-0.97/gai_lib.egg-info/top_level.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)      120 2024-03-25 14:35:24.000000 gai-lib-0.97/requirements.txt
+-rw-r--r--   0 roylai    (1000) roylai    (1000)       38 2024-04-19 22:08:43.367512 gai-lib-0.97/setup.cfg
+-rw-r--r--   0 roylai    (1000) roylai    (1000)     2881 2024-03-25 14:35:01.000000 gai-lib-0.97/setup.py
```

### Comparing `gai-lib-0.96/PKG-INFO` & `gai-lib-0.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gai-lib
-Version: 0.96
+Version: 0.97
 Author: kakkoii1337
 Author-email: kakkoii1337@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `gai-lib-0.96/gai/common/StatusListener.py` & `gai-lib-0.97/gai/common/StatusListener.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import websockets
 import json
-
+from gai.common.logging import getLogger
+logger = getLogger(__name__)
+logger.setLevel("INFO")
 
 class StatusListener:
 
     def __init__(self, uri):
         self.uri = uri
         self.cancellation_token = None
 
     async def listen(self, callback=None):
         async with websockets.connect(self.uri) as websocket:
-            print(f"Connected to {self.uri}")
+            logger.info(f"Connected to {self.uri}")
             try:
                 while self.cancellation_token is None:
                     message = await websocket.recv()
                     if callback:
                         callback(message)
-                    print(f"Received status update: {message}")
+                    logger.info(f"Received status update: {message}")
 
                     if message == "<stop>":
                         self.cancellation_token = message
 
             except websockets.exceptions.ConnectionClosed as e:
-                print(f"Connection closed: {e}")
+                logger.error(f"Connection closed: {e}")
 
     def stop(self):
         self.cancellation_token = "<stop>"
-        print("Stopping listener")
+        logger.info("Stopping listener")
         return self.cancellation_token
     
-
```

### Comparing `gai-lib-0.96/gai/common/StatusUpdater.py` & `gai-lib-0.97/gai/common/StatusUpdater.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.96/gai/common/errors.py` & `gai-lib-0.97/gai/common/errors.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.96/gai/common/file_utils.py` & `gai-lib-0.97/gai/common/file_utils.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.96/gai/common/generators_utils.py` & `gai-lib-0.97/gai/common/generators_utils.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.96/gai/common/http_utils.py` & `gai-lib-0.97/gai/common/http_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -100,29 +100,42 @@
     if 'code' in error_data:
         error_code = error_data['code']
         if 'message' in error_data:
             raise ApiException(status_code=response.status_code, code=error_code, message=error_data['message'] )
         
     raise ApiException(status_code=response.status_code, code=error_code, message=json.dumps(error_data) )
 
-async def http_post_async(url, data):
-    return httppost_async(url, data)
+async def http_post_async(url, data=None, files=None):
+    return await httppost_async(url, data, files)
+
+async def httppost_async(url, data=None,files=None):
+    if data == None and files == None:
+        raise Exception("No data or files provided")
+
+    logger.debug(f"httppost:url={url}")
+    logger.debug(f"httppost:data={pprint.pformat(data)}")
 
-async def httppost_async(url, data):
-    headers = {"Content-Type": "application/json"}
     async with httpx.AsyncClient() as client:
-        if not isinstance(data, str):
-            data = json.dumps(data)
         try:
-            response = await client.post(url, data=data, headers=headers)
-            if response.status == 200:
+            if files:
+                if data and "stream" in data:
+                    files["stream"] = (None, data["stream"])
+                response = await client.post(url, files=files)
+            else:
+                if "stream" in data:
+                    response = await client.post(url, json=data, stream=data["stream"])
+                else:
+                    response = await client.post(url, json=data)
+
+            if response.status_code == 200:
                 return response
             else:
-                await _handle_failed_response_async(response)
-        except httpx.HTTPStatusError as e:
+                _handle_failed_response(response)
+
+        except httpx.ConnectError as e:
             raise Exception("Connection Error. Is the service Running?")
 
 
 def http_post(url, data=None, files=None):
     return httppost(url, data, files)
 
 
@@ -161,24 +174,24 @@
             return response
         else:
             _handle_failed_response(response)
     except requests.exceptions.ConnectionError as e:
         raise Exception("Connection Error. Is the service Running?")
 
 async def http_get_async(url):
-    return httpget_async(url)
+    return await httpget_async(url)
 
 async def httpget_async(url):
-    async with httpx.AsyncClient() as session:
+    async with httpx.AsyncClient() as client:
         try:
-            async with session.get(url) as response:
-                if response.status == 200:
-                    return response                      # Returning the data
-                else:
-                    await _handle_failed_response_async(response)
+            response = await client.get(url)
+            if response.status_code == 200:
+                return response                      # Returning the data
+            else:
+                await _handle_failed_response_async(response)
         except httpx.HTTPStatusError as e:
             raise Exception("Connection Error. Is the service Running?")
 
 ### DELETE method
 
 def http_delete(url):
     return httpdelete(url)
@@ -190,15 +203,15 @@
             return response
         else:
             _handle_failed_response(response)
     except requests.exceptions.ConnectionError as e:
         raise Exception("Connection Error. Is the service Running?")
 
 async def http_delete_async(url):
-    return httpdelete_async(url)
+    return await httpdelete_async(url)
 
 async def httpdelete_async(url):
     async with httpx.AsyncClient() as session:
         try:
             response = await session.delete(url)
             if response.status_code == 200:
                 return response
@@ -219,15 +232,15 @@
             return response
         else:
             _handle_failed_response(response)
     except requests.exceptions.ConnectionError as e:
         raise Exception("Connection Error. Is the service Running?")
 
 async def http_put_async(url):
-    return httpput_async(url)
+    return await httpput_async(url)
 
 async def httpput_async(url):
     async with httpx.AsyncClient() as session:
         try:
             response = await session.put(url)
             if response.status_code == 200:
                 return response
```

### Comparing `gai-lib-0.96/gai/common/image_utils.py` & `gai-lib-0.97/gai/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.96/gai/common/logging.py` & `gai-lib-0.97/gai/common/logging.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.96/gai/common/overlap_splitter.py` & `gai-lib-0.97/gai/common/overlap_splitter.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.96/gai/common/sound_utils.py` & `gai-lib-0.97/gai/common/sound_utils.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.96/gai/common/utils.py` & `gai-lib-0.97/gai/common/utils.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.96/gai/lib/GGG.py` & `gai-lib-0.97/gai/lib/GGG.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.96/gai/lib/ITTClient.py` & `gai-lib-0.97/gai/lib/ITTClient.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.96/gai/lib/RAGClientAsync.py` & `gai-lib-0.97/gai/lib/RAGClientSync.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,28 @@
 import os
 import json
 from fastapi import WebSocketDisconnect
-from gai.common.http_utils import http_post_async, http_get_async,http_delete_async
+from gai.common.http_utils import http_post, http_delete,http_get
 from gai.common.logging import getLogger
-from gai.common.errors import ApiException
 logger = getLogger(__name__)
+from gai.common.errors import ApiException
+import asyncio
 from gai.lib.ClientBase import ClientBase
+import threading
+import websockets
+import time
+from threading import Thread
+
+import asyncio
+from urllib.parse import urlsplit
+
+from gai.common.StatusListener import StatusListener
+async def run_listener(server_uri, progress_updater):
+    listener = StatusListener(server_uri)
+    await listener.listen(callback=progress_updater)
 
 class RAGClientBase(ClientBase):
     
     def __init__(self,config_path=None):
         super().__init__(config_path)
         self.base_url = os.path.join(
             self.config["gai_url"], 
@@ -22,123 +35,162 @@
             files = {
                 "file": (os.path.basename(file_path), f if mode == 'rb' else f.read(), "application/pdf"),
                 "metadata": (None, json.dumps(metadata), "application/json"),
                 "collection_name": (None, collection_name, "text/plain")
             }
             return files
 
-class RAGClientAsync(RAGClientBase):
+class RAGClientSync(RAGClientBase):
 
     def __init__(self,config_path=None):
         super().__init__(config_path)
 
-### ----------------- INDEXING ----------------- ###
+# Indexing Transaction -------------------------------------------------------------------------------------------------------------------------------------------
 
-    # Provides an updater to get chunk indexing status
-    # NOTE: The update is only relevant if this library is used in a FastAPI application with a websocket connection
-    async def index_file_async(
-        self, 
+
+    # synchronous version of index_file_async
+    def index_file(self, 
         collection_name, 
         file_path, 
         title="",
         source="",
         authors="",
         publisher="",
         published_date="",
         comments="",
-        keywords="", 
-        progress_updater=None):
-        url=os.path.join(self.base_url,"index-file")
+        keywords=""):
+        url = os.path.join(self.base_url,"index-file")
         metadata = {
             "title": title,
             "source": source,
             "authors": authors,
             "publisher": publisher,
             "published_date": published_date,
             "comments": comments,
             "keywords": keywords
         }
-       # We will assume file ending with *.pdf to be PDF but this check should be done before the call.
+
+        # We will assume file ending with *.pdf to be PDF but this check should be done before the call.
         mode = 'rb' if file_path.endswith('.pdf') else 'r'
         with open(file_path, mode) as f:
             files = {
-                "file": (os.path.basename(file_path), f, "application/pdf"),
+                "file": (os.path.basename(file_path), f.read(), "application/pdf"),
                 "metadata": (None, json.dumps(metadata), "application/json"),
                 "collection_name": (None, collection_name, "text/plain")
             }
-            response = await http_post_async(url=url, files=files)
-
-        # Callback for progress update (returns a number between 0 and 100)
-        if progress_updater:
-            # Exception should not disrupt the indexing process
-            try:
-                # progress = int((i + 1) / len(chunks) * 100)
-                progress = 100
-                await progress_updater(progress)
-                logger.debug(
-                    f"RAGClient: progress={progress}")
-                # await send_progress(websocket, progress)
-            except WebSocketDisconnect as e:
-                if e.code == 1000:
-                    # Normal closure, perhaps log it as info and continue gracefully
-                    logger.info(
-                        f"RAGClient: WebSocket closed normally with code {e.code}")
-                    pass
-                else:
-                    # Handle other codes as actual errors
-                    logger.error(
-                        f"RAGClient: WebSocket disconnected with error code {e.code}")
-                    pass
-            except Exception as e:
-                logger.error(
-                    f"RetrievalGeneration.index_async: Update websocket progress failed. Error={str(e)}")
-                pass
-
+            logger.info(f"RAGClient.index_file: {url}")            
+            response = http_post(url=url, files=files)
+        
+        # {document_id: "document_id"}
         return json.loads(response.text)
 
-
-    async def retrieve_async(self, collection_name, query_texts, n_results=None):
+    def retrieve(self, collection_name, query_texts, n_results=None):
         url = os.path.join(self.base_url,"retrieve")
+        logger.info(f"RAGClient.retrieve: {url}")
         data = {
             "collection_name": collection_name,
             "query_texts": query_texts
         }
         if n_results:
             data["n_results"] = n_results
 
-        response = await http_post_async(url, data=data)
+        response = http_post(url, data=data)
         return response
 
-    # Database Management
+#Collections-------------------------------------------------------------------------------------------------------------------------------------------
+
+    def list_collections(self):
+        url = os.path.join(self.base_url,"collections")
+        logger.info(f"RAGClient.list_collections: {url}")
+        response = http_get(url)
+        return json.loads(response.text)
+
+    def purge_all(self):
+        url = os.path.join(self.base_url,"purge")
+        logger.info(f"RAGClient.purge_all: {url}")
+        response = http_delete(url)
+        return json.loads(response.text)
 
-    async def delete_collection_async(self, collection_name):
+    def delete_collection(self, collection_name):
         url = os.path.join(self.base_url,"collection",collection_name)
-        logger.info(f"RAGClient.delete_collection: Deleting collection {url}")
+        logger.info(f"RAGClient.delete_collection: {url}")
         try:
-            response = await http_delete_async(url)
+            response = http_delete(url)
         except ApiException as e:
             if e.code == 'collection_not_found':
                 return {"count":0}
             logger.error(e)
             raise e
         return json.loads(response.text)
 
-    async def list_collections(self):
-        url = os.path.join(self.base_url,"collections")
-        response = await http_get_async(url)
+#Documents-------------------------------------------------------------------------------------------------------------------------------------------
+
+    def list_documents(self):
+        url = os.path.join(self.base_url,"documents")
+        logger.info(f"RAGClient.list_documents: {url}")
+        response = http_get(url)
         return json.loads(response.text)
 
-    async def list_documents(self,collection_name):
-        url = os.path.join(self.base_url,"collection",collection_name)
-        response = await http_get_async(url)
+    def list_documents_by_collection(self,collection_name):
+        url = os.path.join(self.base_url,f"documents/{collection_name}")
+        logger.info(f"RAGClient.list_documents_by_collection: {url}")
+        response = http_get(url)
         return json.loads(response.text)
-    
-    async def get_document_async(self,collection_name,doc_id):
+
+    def get_document_header(self,collection_name,doc_id):
         url = os.path.join(self.base_url,f"document/{collection_name}/{doc_id}")
-        response = await http_get_async(url)
+        logger.info(f"RAGClient.get_documents: {url}")
+        response = http_get(url)
         return json.loads(response.text)
 
-    async def delete_document_async(self,collection_name,doc_id):
+    def delete_document(self,collection_name,doc_id):
         url = os.path.join(self.base_url,f"document/{collection_name}/{doc_id}")
-        response = await http_delete_async(url)
+        logger.info(f"RAGClient.delete_documents: {url}")
+        response = http_delete(url)
         return json.loads(response.text)
 
+    def get_document_id(self,collection_name, file_path):
+        url = os.path.join(self.base_url,f"document/exists/{collection_name}")
+        logger.info(f"RAGClient.document_exists: {url}")
+        with open(file_path, "r") as f:
+            text = f.read()        
+        files = {
+            "file": (file_path, text, "text/plain"),
+            "collection_name": (None, collection_name, "text/plain")
+        }        
+        response = http_post(url, files=files)
+        return json.loads(response.text)    
+
+
+#chunks-------------------------------------------------------------------------------------------------------------------------------------------
+
+    def list_chunks(self,collection_name=None,doc_id=None):
+
+        if collection_name and not doc_id or doc_id and not collection_name:
+            raise Exception("Both collection_name and doc_id must be provided or neither.")
+        
+        if not collection_name and not doc_id:
+            url = os.path.join(self.base_url,"chunks")
+            logger.info(f"RAGClient.list_chunks: {url}")
+            try:
+                response = http_get(url)
+                return json.loads(response.text)
+            except Exception as e:
+                if e.detail['code'] == 'collections_not_found':
+                    return []
+                raise e
+
+        url = os.path.join(self.base_url,f"chunks/by_document/{collection_name}/{doc_id}")
+        logger.info(f"RAGClient.list_chunks: {url}")
+        response = http_get(url)
+        if response.status_code == 404:
+            return []
+
+        return json.loads(response.text)
+
+    
+    def get_chunk(self,collection_name, chunk_id):
+
+        url = os.path.join(self.base_url,f"chunk/{collection_name}/{chunk_id}")
+        logger.info(f"RAGClient.get_chunk: {url}")
+        response = http_get(url)
+        return json.loads(response.text)
```

### Comparing `gai-lib-0.96/gai/lib/STTClient.py` & `gai-lib-0.97/gai/lib/STTClient.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.96/gai/lib/TTSClient.py` & `gai-lib-0.97/gai/lib/TTSClient.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.96/gai/lib/ttt/ChunkWrapper.py` & `gai-lib-0.97/gai/lib/ttt/ChunkWrapper.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.96/gai/lib/ttt/TTTClient.py` & `gai-lib-0.97/gai/lib/ttt/TTTClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,18 +49,20 @@
             if he.code == "context_length_exceeded":
                 try:
                     generator = "mistral7b_128k-exllama"
                     data["model"] = generator
                     url = self._gen_url(generator)
                     response = http_post(url, data)
                 except Exception as e:
+                    logger.error(f"TTTClient.api: gaigen error={e}")
                     raise e
             else:
                 raise he
         except Exception as e:
+            logger.error(f"TTTClient.api: gaigen error={e}")
             raise e
 
         if not stream:
             if response.json()["choices"][0]["message"]["tool_calls"]:
                 response.decode = lambda: {
                     "type":"function",
                     "name": response.json()["choices"][0]["message"]["tool_calls"][0]["function"]["name"],
```

### Comparing `gai-lib-0.96/gai/tools/Chunker.py` & `gai-lib-0.97/gai/tools/Chunker.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.96/gai/tools/Googler.py` & `gai-lib-0.97/gai/tools/Googler.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.96/gai/tools/Scraper.py` & `gai-lib-0.97/gai/tools/Scraper.py`

 * *Files identical despite different names*

### Comparing `gai-lib-0.96/gai.yml` & `gai-lib-0.97/gai.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 default_generator: mistral7b-exllama
 #gai_url: "http://localhost:12031"
 gai_url: "https://gaiaio.ai/api/gen"
 generators:
     mistral7b-exllama:
         type: ttt
-        url: "/v1/chat/completions"
         #url: "/gen/v1/chat/completions"
+        url: "/v1/chat/completions"
         whitelist:
             - temperature
             - top_p
             - min_p
             - top_k
             - max_new_tokens
             - typical
@@ -109,10 +109,11 @@
         env:
             gai_api_key: "gai_api_key"
     llava-transformers:
         type: itt
         url: "/v1/vision/completions"
     rag:
         type: rag
-        url: "/v1/rag"
+        url: "/gen/v1/rag"
+        #url: "/v1/rag"
         env:
             gai_api_key: "gai_api_key"
```

### Comparing `gai-lib-0.96/gai_lib.egg-info/PKG-INFO` & `gai-lib-0.97/gai_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gai-lib
-Version: 0.96
+Version: 0.97
 Author: kakkoii1337
 Author-email: kakkoii1337@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `gai-lib-0.96/gai_lib.egg-info/SOURCES.txt` & `gai-lib-0.97/gai_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gai-lib-0.96/setup.py` & `gai-lib-0.97/setup.py`

 * *Files identical despite different names*

