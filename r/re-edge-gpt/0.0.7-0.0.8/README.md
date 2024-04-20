# Comparing `tmp/re_edge_gpt-0.0.7.tar.gz` & `tmp/re_edge_gpt-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "re_edge_gpt-0.0.7.tar", last modified: Fri Oct  6 06:15:06 2023, max compression
+gzip compressed data, was "re_edge_gpt-0.0.8.tar", last modified: Fri Oct  6 08:01:24 2023, max compression
```

## Comparing `re_edge_gpt-0.0.7.tar` & `re_edge_gpt-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-10-06 06:15:06.553043 re_edge_gpt-0.0.7/
--rw-rw-rw-   0        0        0     1085 2023-06-22 06:27:17.000000 re_edge_gpt-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     8894 2023-10-06 06:15:06.551789 re_edge_gpt-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     8001 2023-10-06 03:44:24.000000 re_edge_gpt-0.0.7/README.md
--rw-rw-rw-   0        0        0     1112 2023-10-06 06:14:46.000000 re_edge_gpt-0.0.7/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-10-06 06:15:06.513985 re_edge_gpt-0.0.7/re_edge_gpt/
--rw-rw-rw-   0        0        0      292 2023-08-19 11:32:10.000000 re_edge_gpt-0.0.7/re_edge_gpt/__init__.py
--rw-rw-rw-   0        0        0    10147 2023-10-06 06:12:15.000000 re_edge_gpt-0.0.7/re_edge_gpt/chathub.py
--rw-rw-rw-   0        0        0     2487 2023-09-01 08:50:44.000000 re_edge_gpt-0.0.7/re_edge_gpt/constants.py
--rw-rw-rw-   0        0        0     5222 2023-10-06 06:13:22.000000 re_edge_gpt-0.0.7/re_edge_gpt/conversation.py
--rw-rw-rw-   0        0        0     1256 2023-08-02 06:26:40.000000 re_edge_gpt-0.0.7/re_edge_gpt/conversation_style.py
--rw-rw-rw-   0        0        0       46 2023-08-02 06:26:40.000000 re_edge_gpt-0.0.7/re_edge_gpt/exceptions.py
--rw-rw-rw-   0        0        0    16537 2023-10-04 02:40:08.000000 re_edge_gpt-0.0.7/re_edge_gpt/image_genearation.py
--rw-rw-rw-   0        0        0     2247 2023-08-02 06:26:40.000000 re_edge_gpt-0.0.7/re_edge_gpt/locale.py
--rw-rw-rw-   0        0        0     7489 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.7/re_edge_gpt/main.py
--rw-rw-rw-   0        0        0     7755 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.7/re_edge_gpt/re_edge_gpt.py
--rw-rw-rw-   0        0        0     5948 2023-09-01 08:50:24.000000 re_edge_gpt-0.0.7/re_edge_gpt/request.py
--rw-rw-rw-   0        0        0      967 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.7/re_edge_gpt/utilities.py
-drwxrwxrwx   0        0        0        0 2023-10-06 06:15:06.550735 re_edge_gpt-0.0.7/re_edge_gpt.egg-info/
--rw-rw-rw-   0        0        0     8894 2023-10-06 06:15:06.000000 re_edge_gpt-0.0.7/re_edge_gpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2023-10-06 06:15:06.000000 re_edge_gpt-0.0.7/re_edge_gpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-06 06:15:06.000000 re_edge_gpt-0.0.7/re_edge_gpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-10-06 06:15:06.000000 re_edge_gpt-0.0.7/re_edge_gpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-10-06 06:15:06.000000 re_edge_gpt-0.0.7/re_edge_gpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-06 06:15:06.553043 re_edge_gpt-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-10-06 08:01:24.777412 re_edge_gpt-0.0.8/
+-rw-rw-rw-   0        0        0     1085 2023-06-22 06:27:17.000000 re_edge_gpt-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     8968 2023-10-06 08:01:24.776231 re_edge_gpt-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     8075 2023-10-06 06:20:08.000000 re_edge_gpt-0.0.8/README.md
+-rw-rw-rw-   0        0        0     1112 2023-10-06 08:01:12.000000 re_edge_gpt-0.0.8/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-10-06 08:01:24.754150 re_edge_gpt-0.0.8/re_edge_gpt/
+-rw-rw-rw-   0        0        0      292 2023-08-19 11:32:10.000000 re_edge_gpt-0.0.8/re_edge_gpt/__init__.py
+-rw-rw-rw-   0        0        0    10147 2023-10-06 06:12:15.000000 re_edge_gpt-0.0.8/re_edge_gpt/chathub.py
+-rw-rw-rw-   0        0        0     2487 2023-09-01 08:50:44.000000 re_edge_gpt-0.0.8/re_edge_gpt/constants.py
+-rw-rw-rw-   0        0        0     5222 2023-10-06 06:13:22.000000 re_edge_gpt-0.0.8/re_edge_gpt/conversation.py
+-rw-rw-rw-   0        0        0     1256 2023-08-02 06:26:40.000000 re_edge_gpt-0.0.8/re_edge_gpt/conversation_style.py
+-rw-rw-rw-   0        0        0       46 2023-08-02 06:26:40.000000 re_edge_gpt-0.0.8/re_edge_gpt/exceptions.py
+-rw-rw-rw-   0        0        0    16578 2023-10-06 07:54:24.000000 re_edge_gpt-0.0.8/re_edge_gpt/image_genearation.py
+-rw-rw-rw-   0        0        0     2247 2023-08-02 06:26:40.000000 re_edge_gpt-0.0.8/re_edge_gpt/locale.py
+-rw-rw-rw-   0        0        0     7489 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.8/re_edge_gpt/main.py
+-rw-rw-rw-   0        0        0     7755 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.8/re_edge_gpt/re_edge_gpt.py
+-rw-rw-rw-   0        0        0     5948 2023-09-01 08:50:24.000000 re_edge_gpt-0.0.8/re_edge_gpt/request.py
+-rw-rw-rw-   0        0        0      967 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.8/re_edge_gpt/utilities.py
+drwxrwxrwx   0        0        0        0 2023-10-06 08:01:24.775726 re_edge_gpt-0.0.8/re_edge_gpt.egg-info/
+-rw-rw-rw-   0        0        0     8968 2023-10-06 08:01:24.000000 re_edge_gpt-0.0.8/re_edge_gpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2023-10-06 08:01:24.000000 re_edge_gpt-0.0.8/re_edge_gpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-06 08:01:24.000000 re_edge_gpt-0.0.8/re_edge_gpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-10-06 08:01:24.000000 re_edge_gpt-0.0.8/re_edge_gpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-10-06 08:01:24.000000 re_edge_gpt-0.0.8/re_edge_gpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-10-06 08:01:24.777412 re_edge_gpt-0.0.8/setup.cfg
```

### Comparing `re_edge_gpt-0.0.7/LICENSE` & `re_edge_gpt-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.7/PKG-INFO` & `re_edge_gpt-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re_edge_gpt
-Version: 0.0.7
+Version: 0.0.8
 Summary: Microsoft's Bing Chat AI
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Integration-Automation/ReEdgeGPT
 Project-URL: Code, https://github.com/Integration-Automation/ReEdgeGPT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -258,14 +258,15 @@
 
 > * Q: Exception: UnauthorizedRequest: Cannot retrieve user status.
 > * A: Renew your cookie file.
 
 > * Q: Exception: conversationSignature
 > * A: Clear all your bing cookie and renew your cookie file.
 >   * Like : https://github.com/Integration-Automation/ReEdgeGPT/issues/17
+>   * And: https://github.com/Integration-Automation/ReEdgeGPT/issues/22
 
 > * Q: ValueError: Invalid header value b'_U=***\n'
 > * A: Renew your image cookie.
 
 </details>
 
 ---
```

### Comparing `re_edge_gpt-0.0.7/README.md` & `re_edge_gpt-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -232,14 +232,15 @@
 
 > * Q: Exception: UnauthorizedRequest: Cannot retrieve user status.
 > * A: Renew your cookie file.
 
 > * Q: Exception: conversationSignature
 > * A: Clear all your bing cookie and renew your cookie file.
 >   * Like : https://github.com/Integration-Automation/ReEdgeGPT/issues/17
+>   * And: https://github.com/Integration-Automation/ReEdgeGPT/issues/22
 
 > * Q: ValueError: Invalid header value b'_U=***\n'
 > * A: Renew your image cookie.
 
 </details>
 
 ---
```

### Comparing `re_edge_gpt-0.0.7/pyproject.toml` & `re_edge_gpt-0.0.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "re_edge_gpt"
-version = "0.0.07"
+version = "0.0.08"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 dependencies = [
     "aiohttp", "certifi", "httpx", "prompt_toolkit", "requests", "rich", "regex"
 ]
 description = "Microsoft's Bing Chat AI"
```

### Comparing `re_edge_gpt-0.0.7/re_edge_gpt/chathub.py` & `re_edge_gpt-0.0.8/re_edge_gpt/chathub.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.7/re_edge_gpt/constants.py` & `re_edge_gpt-0.0.8/re_edge_gpt/constants.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.7/re_edge_gpt/conversation.py` & `re_edge_gpt-0.0.8/re_edge_gpt/conversation.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.7/re_edge_gpt/conversation_style.py` & `re_edge_gpt-0.0.8/re_edge_gpt/conversation_style.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.7/re_edge_gpt/image_genearation.py` & `re_edge_gpt-0.0.8/re_edge_gpt/image_genearation.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import contextlib
 import json
 import os
 import socket
 import sys
 import time
 from functools import partial
-from typing import Dict
+from typing import Dict, Mapping
 from typing import List
 from typing import Union
 
 import httpx
 import pkg_resources
 import regex
 import requests
@@ -290,19 +290,19 @@
             prompt: str
         """
         if not self.quiet:
             print("Sending request...")
         url_encoded_prompt = requests.utils.quote(prompt)
         # https://www.bing.com/images/create?q=<PROMPT>&rt=3&FORM=GENCRE
         url = f"{BING_URL}/images/create?q={url_encoded_prompt}&rt=3&FORM=GENCRE"
-        payload = f"q={url_encoded_prompt}&qs=ds"
+        # payload = f"q={url_encoded_prompt}&qs=ds"
         response = await self.session.post(
             url,
             follow_redirects=False,
-            data=payload,
+            data={"q": url_encoded_prompt, "qs": "ds"},
         )
         content = response.text
         if "this prompt has been blocked" in content.lower():
             raise Exception(
                 "Your prompt has been blocked by Bing. Try to change any bad words and try again.",
             )
         if response.status_code != 302:
```

### Comparing `re_edge_gpt-0.0.7/re_edge_gpt/locale.py` & `re_edge_gpt-0.0.8/re_edge_gpt/locale.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.7/re_edge_gpt/main.py` & `re_edge_gpt-0.0.8/re_edge_gpt/main.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.7/re_edge_gpt/re_edge_gpt.py` & `re_edge_gpt-0.0.8/re_edge_gpt/re_edge_gpt.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.7/re_edge_gpt/request.py` & `re_edge_gpt-0.0.8/re_edge_gpt/request.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.7/re_edge_gpt/utilities.py` & `re_edge_gpt-0.0.8/re_edge_gpt/utilities.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.7/re_edge_gpt.egg-info/PKG-INFO` & `re_edge_gpt-0.0.8/re_edge_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-edge-gpt
-Version: 0.0.7
+Version: 0.0.8
 Summary: Microsoft's Bing Chat AI
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Integration-Automation/ReEdgeGPT
 Project-URL: Code, https://github.com/Integration-Automation/ReEdgeGPT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -258,14 +258,15 @@
 
 > * Q: Exception: UnauthorizedRequest: Cannot retrieve user status.
 > * A: Renew your cookie file.
 
 > * Q: Exception: conversationSignature
 > * A: Clear all your bing cookie and renew your cookie file.
 >   * Like : https://github.com/Integration-Automation/ReEdgeGPT/issues/17
+>   * And: https://github.com/Integration-Automation/ReEdgeGPT/issues/22
 
 > * Q: ValueError: Invalid header value b'_U=***\n'
 > * A: Renew your image cookie.
 
 </details>
 
 ---
```

### Comparing `re_edge_gpt-0.0.7/re_edge_gpt.egg-info/SOURCES.txt` & `re_edge_gpt-0.0.8/re_edge_gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

