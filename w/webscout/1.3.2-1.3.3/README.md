# Comparing `tmp/webscout-1.3.2.tar.gz` & `tmp/webscout-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-1.3.2.tar", last modified: Fri Apr 19 10:46:01 2024, max compression
+gzip compressed data, was "webscout-1.3.3.tar", last modified: Fri Apr 19 14:50:58 2024, max compression
```

## Comparing `webscout-1.3.2.tar` & `webscout-1.3.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 10:46:01.674465 webscout-1.3.2/
-drwxrwxrwx   0        0        0        0 2024-04-19 10:46:01.008720 webscout-1.3.2/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 10:46:01.024723 webscout-1.3.2/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-04-19 10:46:01.053714 webscout-1.3.2/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3846 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-04-19 10:46:01.073717 webscout-1.3.2/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     1754 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-04-11 08:32:30.000000 webscout-1.3.2/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-04-11 08:32:30.000000 webscout-1.3.2/LICENSE.md
--rw-rw-rw-   0        0        0    30426 2024-04-19 10:46:01.669462 webscout-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0    28235 2024-04-19 10:44:32.000000 webscout-1.3.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-19 10:46:01.675459 webscout-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     2725 2024-04-19 08:30:45.000000 webscout-1.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 10:46:01.634425 webscout-1.3.2/webscout/
--rw-rw-rw-   0        0        0    93054 2024-04-19 10:20:12.000000 webscout-1.3.2/webscout/AI.py
--rw-rw-rw-   0        0        0     2343 2024-04-11 08:32:30.000000 webscout-1.3.2/webscout/AIbase.py
--rw-rw-rw-   0        0        0    24126 2024-04-19 10:31:02.000000 webscout-1.3.2/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-04-11 08:32:30.000000 webscout-1.3.2/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     8103 2024-04-11 08:32:30.000000 webscout-1.3.2/webscout/HelpingAI.py
--rw-rw-rw-   0        0        0     1910 2024-04-19 05:15:07.000000 webscout-1.3.2/webscout/LLM.py
--rw-rw-rw-   0        0        0      977 2024-04-19 10:22:02.000000 webscout-1.3.2/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-04-11 08:32:30.000000 webscout-1.3.2/webscout/__main__.py
--rw-rw-rw-   0        0        0    17059 2024-04-11 08:32:30.000000 webscout-1.3.2/webscout/cli.py
--rw-rw-rw-   0        0        0      276 2024-04-11 08:32:30.000000 webscout-1.3.2/webscout/exceptions.py
--rw-rw-rw-   0        0        0    16358 2024-04-19 06:46:37.000000 webscout-1.3.2/webscout/g4f.py
--rw-rw-rw-   0        0        0      692 2024-04-11 08:32:30.000000 webscout-1.3.2/webscout/models.py
--rw-rw-rw-   0        0        0    20622 2024-04-11 08:35:51.000000 webscout-1.3.2/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2605 2024-04-11 08:32:30.000000 webscout-1.3.2/webscout/utils.py
--rw-rw-rw-   0        0        0       25 2024-04-19 08:30:29.000000 webscout-1.3.2/webscout/version.py
--rw-rw-rw-   0        0        0      941 2024-04-16 06:00:31.000000 webscout-1.3.2/webscout/voice.py
--rw-rw-rw-   0        0        0    74262 2024-04-19 10:21:11.000000 webscout-1.3.2/webscout/webai.py
--rw-rw-rw-   0        0        0     3085 2024-04-11 08:32:30.000000 webscout-1.3.2/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    40670 2024-04-11 08:32:30.000000 webscout-1.3.2/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-04-19 10:46:01.664465 webscout-1.3.2/webscout.egg-info/
--rw-rw-rw-   0        0        0    30426 2024-04-19 10:46:00.000000 webscout-1.3.2/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2024-04-19 10:46:00.000000 webscout-1.3.2/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 10:46:00.000000 webscout-1.3.2/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2024-04-19 10:46:00.000000 webscout-1.3.2/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      334 2024-04-19 10:46:00.000000 webscout-1.3.2/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-19 10:46:00.000000 webscout-1.3.2/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 14:50:58.146413 webscout-1.3.3/
+drwxrwxrwx   0        0        0        0 2024-04-19 14:50:57.647622 webscout-1.3.3/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:50:57.668654 webscout-1.3.3/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:50:57.705004 webscout-1.3.3/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3846 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:50:57.722002 webscout-1.3.3/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     1754 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-04-11 08:32:30.000000 webscout-1.3.3/LICENSE.md
+-rw-rw-rw-   0        0        0    30426 2024-04-19 14:50:58.140426 webscout-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0    28235 2024-04-19 10:44:32.000000 webscout-1.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 14:50:58.146413 webscout-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     2725 2024-04-19 14:23:06.000000 webscout-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:50:58.080942 webscout-1.3.3/webscout/
+-rw-rw-rw-   0        0        0    93054 2024-04-19 10:20:12.000000 webscout-1.3.3/webscout/AI.py
+-rw-rw-rw-   0        0        0     2343 2024-04-11 08:32:30.000000 webscout-1.3.3/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    24126 2024-04-19 10:31:02.000000 webscout-1.3.3/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-04-11 08:32:30.000000 webscout-1.3.3/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     8103 2024-04-11 08:32:30.000000 webscout-1.3.3/webscout/HelpingAI.py
+-rw-rw-rw-   0        0        0     1910 2024-04-19 05:15:07.000000 webscout-1.3.3/webscout/LLM.py
+-rw-rw-rw-   0        0        0      957 2024-04-19 14:19:46.000000 webscout-1.3.3/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-04-11 08:32:30.000000 webscout-1.3.3/webscout/__main__.py
+-rw-rw-rw-   0        0        0    17059 2024-04-11 08:32:30.000000 webscout-1.3.3/webscout/cli.py
+-rw-rw-rw-   0        0        0      276 2024-04-11 08:32:30.000000 webscout-1.3.3/webscout/exceptions.py
+-rw-rw-rw-   0        0        0    16358 2024-04-19 06:46:37.000000 webscout-1.3.3/webscout/g4f.py
+-rw-rw-rw-   0        0        0      692 2024-04-11 08:32:30.000000 webscout-1.3.3/webscout/models.py
+-rw-rw-rw-   0        0        0    20622 2024-04-11 08:35:51.000000 webscout-1.3.3/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2605 2024-04-11 08:32:30.000000 webscout-1.3.3/webscout/utils.py
+-rw-rw-rw-   0        0        0       25 2024-04-19 14:23:23.000000 webscout-1.3.3/webscout/version.py
+-rw-rw-rw-   0        0        0      941 2024-04-16 06:00:31.000000 webscout-1.3.3/webscout/voice.py
+-rw-rw-rw-   0        0        0    73868 2024-04-19 14:19:11.000000 webscout-1.3.3/webscout/webai.py
+-rw-rw-rw-   0        0        0     3085 2024-04-11 08:32:30.000000 webscout-1.3.3/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    40670 2024-04-11 08:32:30.000000 webscout-1.3.3/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:50:58.129912 webscout-1.3.3/webscout.egg-info/
+-rw-rw-rw-   0        0        0    30426 2024-04-19 14:50:56.000000 webscout-1.3.3/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2024-04-19 14:50:57.000000 webscout-1.3.3/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 14:50:56.000000 webscout-1.3.3/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2024-04-19 14:50:56.000000 webscout-1.3.3/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      334 2024-04-19 14:50:56.000000 webscout-1.3.3/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-19 14:50:56.000000 webscout-1.3.3/webscout.egg-info/top_level.txt
```

### Comparing `webscout-1.3.2/DeepWEBS/documents/query_results_extractor.py` & `webscout-1.3.3/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-1.3.3/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/DeepWEBS/networks/filepath_converter.py` & `webscout-1.3.3/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/DeepWEBS/networks/google_searcher.py` & `webscout-1.3.3/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/DeepWEBS/networks/network_configs.py` & `webscout-1.3.3/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/DeepWEBS/networks/webpage_fetcher.py` & `webscout-1.3.3/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/DeepWEBS/utilsdw/enver.py` & `webscout-1.3.3/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/DeepWEBS/utilsdw/logger.py` & `webscout-1.3.3/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/LICENSE.md` & `webscout-1.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/PKG-INFO` & `webscout-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.3.2
+Version: 1.3.3
 Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos and have TTS support
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.3.2 Summary: Search for words,
+Metadata-Version: 2.1 Name: webscout Version: 1.3.3 Summary: Search for words,
 documents, images, videos, news, maps and text translation using the Google,
 DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can
 transcribe yt videos and have TTS support Author: OEvortex Author-email:
 helpingai5@gmail.com License: HelpingAI Simplified Universal License Project-
 URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki Project-URL:
 Source, https://github.com/OE-LUCIFER/Webscout Project-URL: Tracker, https://
 github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube, https://
```

### Comparing `webscout-1.3.2/README.md` & `webscout-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/setup.py` & `webscout-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="1.3.2", 
+    version="1.3.3", 
     description="Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos and have TTS support",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
```

### Comparing `webscout-1.3.2/webscout/AI.py` & `webscout-1.3.3/webscout/AI.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/webscout/AIbase.py` & `webscout-1.3.3/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/webscout/AIutel.py` & `webscout-1.3.3/webscout/AIutel.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/webscout/DWEBS.py` & `webscout-1.3.3/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/webscout/HelpingAI.py` & `webscout-1.3.3/webscout/HelpingAI.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/webscout/LLM.py` & `webscout-1.3.3/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/webscout/__init__.py` & `webscout-1.3.3/webscout/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import logging
 from .webscout_search import WEBS
 from .webscout_search_async import AsyncWEBS
 from .version import __version__
 from .DWEBS import DeepWEBS
 from .transcriber import transcriber
 from .voice import play_audio
-from .LLM import LLM
+
 
 __repo__ = "https://github.com/OE-LUCIFER/Webscout"
 
 webai = [
     "leo",
     "openai",
     "opengpt",
```

### Comparing `webscout-1.3.2/webscout/cli.py` & `webscout-1.3.3/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/webscout/g4f.py` & `webscout-1.3.3/webscout/g4f.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/webscout/models.py` & `webscout-1.3.3/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/webscout/transcriber.py` & `webscout-1.3.3/webscout/transcriber.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/webscout/utils.py` & `webscout-1.3.3/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/webscout/voice.py` & `webscout-1.3.3/webscout/voice.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/webscout/webai.py` & `webscout-1.3.3/webscout/webai.py`

 * *Files 0% similar despite different names*

```diff
@@ -2180,23 +2180,15 @@
         """Generate images with pollinations.ai"""
         with Progress() as progress:
             task = progress.add_task(
                 f"[cyan]Generating ...[{amount}]",
                 total=amount,
                 visible=quiet == False,
             )
-            imager = Imager(timeout=timeout, proxies=proxy if proxy else {})
-            for image in imager.generate(
-                prompt=prompt,
-                amount=amount,
-                additives=no_additives == False,
-                stream=True,
-            ):
-                imager.save([image], name=name, dir=directory)
-                progress.update(task, advance=1)
+
 
 
 class Utils:
     """Utilities command"""
 
     @staticmethod
     @click.command(context_settings=this.context_settings)
@@ -2213,24 +2205,24 @@
     )
     @click.help_option("-h", "--help")
     @busy_bar.run(index=1, immediate=True)
     def update(source, dev, sudo):
         """Install latest version of webscout"""
         if dev:
             source = "git+" + webscout.__repo__ + ".git"
-        source = "python-tgpt" if source is None else source
+        source = "webscout" if source is None else source
         assert (
             "tgpt" in source or source == "."
         ), f"Cannot update webscout from the source '{source}'"
         click.secho(
-            f"[*] Updating from '{'pip' if source=='python-tgpt' else source}'",
+            f"[*] Updating from '{'pip' if source=='webscout' else source}'",
             fg="yellow",
         )
         this.run_system_command(f"{sudo or ''}pip install --upgrade {source}")
-        response = this.run_system_command("pip show python-tgpt")[1]
+        response = this.run_system_command("pip show webscout")[1]
         click.secho(response.stdout)
         click.secho("Congratulations! webscout updated successfully.", fg="cyan")
 
     @staticmethod
     @click.command(context_settings=this.context_settings)
     @click.option("-w", "--whole", is_flag=True, help="Stdout whole json info")
     @click.option(
```

### Comparing `webscout-1.3.2/webscout/webscout_search.py` & `webscout-1.3.3/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/webscout/webscout_search_async.py` & `webscout-1.3.3/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.2/webscout.egg-info/PKG-INFO` & `webscout-1.3.3/webscout.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.3.2
+Version: 1.3.3
 Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos and have TTS support
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.3.2 Summary: Search for words,
+Metadata-Version: 2.1 Name: webscout Version: 1.3.3 Summary: Search for words,
 documents, images, videos, news, maps and text translation using the Google,
 DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can
 transcribe yt videos and have TTS support Author: OEvortex Author-email:
 helpingai5@gmail.com License: HelpingAI Simplified Universal License Project-
 URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki Project-URL:
 Source, https://github.com/OE-LUCIFER/Webscout Project-URL: Tracker, https://
 github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube, https://
```

### Comparing `webscout-1.3.2/webscout.egg-info/SOURCES.txt` & `webscout-1.3.3/webscout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

