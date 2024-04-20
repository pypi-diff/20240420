# Comparing `tmp/webscout-1.3.3.tar.gz` & `tmp/webscout-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-1.3.3.tar", last modified: Fri Apr 19 14:50:58 2024, max compression
+gzip compressed data, was "webscout-1.3.4.tar", last modified: Sat Apr 20 05:46:03 2024, max compression
```

## Comparing `webscout-1.3.3.tar` & `webscout-1.3.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 14:50:58.146413 webscout-1.3.3/
-drwxrwxrwx   0        0        0        0 2024-04-19 14:50:57.647622 webscout-1.3.3/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:50:57.668654 webscout-1.3.3/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:50:57.705004 webscout-1.3.3/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3846 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:50:57.722002 webscout-1.3.3/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     1754 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-04-11 08:32:30.000000 webscout-1.3.3/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-04-11 08:32:30.000000 webscout-1.3.3/LICENSE.md
--rw-rw-rw-   0        0        0    30426 2024-04-19 14:50:58.140426 webscout-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0    28235 2024-04-19 10:44:32.000000 webscout-1.3.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-19 14:50:58.146413 webscout-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     2725 2024-04-19 14:23:06.000000 webscout-1.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:50:58.080942 webscout-1.3.3/webscout/
--rw-rw-rw-   0        0        0    93054 2024-04-19 10:20:12.000000 webscout-1.3.3/webscout/AI.py
--rw-rw-rw-   0        0        0     2343 2024-04-11 08:32:30.000000 webscout-1.3.3/webscout/AIbase.py
--rw-rw-rw-   0        0        0    24126 2024-04-19 10:31:02.000000 webscout-1.3.3/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-04-11 08:32:30.000000 webscout-1.3.3/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     8103 2024-04-11 08:32:30.000000 webscout-1.3.3/webscout/HelpingAI.py
--rw-rw-rw-   0        0        0     1910 2024-04-19 05:15:07.000000 webscout-1.3.3/webscout/LLM.py
--rw-rw-rw-   0        0        0      957 2024-04-19 14:19:46.000000 webscout-1.3.3/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-04-11 08:32:30.000000 webscout-1.3.3/webscout/__main__.py
--rw-rw-rw-   0        0        0    17059 2024-04-11 08:32:30.000000 webscout-1.3.3/webscout/cli.py
--rw-rw-rw-   0        0        0      276 2024-04-11 08:32:30.000000 webscout-1.3.3/webscout/exceptions.py
--rw-rw-rw-   0        0        0    16358 2024-04-19 06:46:37.000000 webscout-1.3.3/webscout/g4f.py
--rw-rw-rw-   0        0        0      692 2024-04-11 08:32:30.000000 webscout-1.3.3/webscout/models.py
--rw-rw-rw-   0        0        0    20622 2024-04-11 08:35:51.000000 webscout-1.3.3/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2605 2024-04-11 08:32:30.000000 webscout-1.3.3/webscout/utils.py
--rw-rw-rw-   0        0        0       25 2024-04-19 14:23:23.000000 webscout-1.3.3/webscout/version.py
--rw-rw-rw-   0        0        0      941 2024-04-16 06:00:31.000000 webscout-1.3.3/webscout/voice.py
--rw-rw-rw-   0        0        0    73868 2024-04-19 14:19:11.000000 webscout-1.3.3/webscout/webai.py
--rw-rw-rw-   0        0        0     3085 2024-04-11 08:32:30.000000 webscout-1.3.3/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    40670 2024-04-11 08:32:30.000000 webscout-1.3.3/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:50:58.129912 webscout-1.3.3/webscout.egg-info/
--rw-rw-rw-   0        0        0    30426 2024-04-19 14:50:56.000000 webscout-1.3.3/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2024-04-19 14:50:57.000000 webscout-1.3.3/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 14:50:56.000000 webscout-1.3.3/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2024-04-19 14:50:56.000000 webscout-1.3.3/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      334 2024-04-19 14:50:56.000000 webscout-1.3.3/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-19 14:50:56.000000 webscout-1.3.3/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 05:46:03.027856 webscout-1.3.4/
+drwxrwxrwx   0        0        0        0 2024-04-20 05:46:02.730104 webscout-1.3.4/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.4/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 05:46:02.760478 webscout-1.3.4/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.4/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-04-11 08:32:30.000000 webscout-1.3.4/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-04-11 08:32:30.000000 webscout-1.3.4/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-04-20 05:46:02.792037 webscout-1.3.4/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.4/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-04-11 08:32:30.000000 webscout-1.3.4/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-04-20 05:31:46.000000 webscout-1.3.4/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-04-11 08:32:30.000000 webscout-1.3.4/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3590 2024-04-20 05:30:03.000000 webscout-1.3.4/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-04-20 05:46:02.811037 webscout-1.3.4/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.3.4/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     2472 2024-04-20 05:24:28.000000 webscout-1.3.4/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-04-11 08:32:30.000000 webscout-1.3.4/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-04-11 08:32:30.000000 webscout-1.3.4/LICENSE.md
+-rw-rw-rw-   0        0        0    31947 2024-04-20 05:46:03.016859 webscout-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    29756 2024-04-20 05:34:00.000000 webscout-1.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-20 05:46:03.028858 webscout-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     2725 2024-04-20 05:11:59.000000 webscout-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 05:46:02.947868 webscout-1.3.4/webscout/
+-rw-rw-rw-   0        0        0    93054 2024-04-19 10:20:12.000000 webscout-1.3.4/webscout/AI.py
+-rw-rw-rw-   0        0        0     2343 2024-04-11 08:32:30.000000 webscout-1.3.4/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    24413 2024-04-20 03:51:32.000000 webscout-1.3.4/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-04-20 05:41:28.000000 webscout-1.3.4/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     8103 2024-04-11 08:32:30.000000 webscout-1.3.4/webscout/HelpingAI.py
+-rw-rw-rw-   0        0        0     1910 2024-04-19 05:15:07.000000 webscout-1.3.4/webscout/LLM.py
+-rw-rw-rw-   0        0        0     1002 2024-04-20 05:14:03.000000 webscout-1.3.4/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-04-11 08:32:30.000000 webscout-1.3.4/webscout/__main__.py
+-rw-rw-rw-   0        0        0    17059 2024-04-11 08:32:30.000000 webscout-1.3.4/webscout/cli.py
+-rw-rw-rw-   0        0        0      276 2024-04-11 08:32:30.000000 webscout-1.3.4/webscout/exceptions.py
+-rw-rw-rw-   0        0        0    16358 2024-04-19 17:15:45.000000 webscout-1.3.4/webscout/g4f.py
+-rw-rw-rw-   0        0        0      692 2024-04-11 08:32:30.000000 webscout-1.3.4/webscout/models.py
+-rw-rw-rw-   0        0        0    20622 2024-04-20 05:41:28.000000 webscout-1.3.4/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2605 2024-04-11 08:32:30.000000 webscout-1.3.4/webscout/utils.py
+-rw-rw-rw-   0        0        0       25 2024-04-20 05:13:34.000000 webscout-1.3.4/webscout/version.py
+-rw-rw-rw-   0        0        0      941 2024-04-16 06:00:31.000000 webscout-1.3.4/webscout/voice.py
+-rw-rw-rw-   0        0        0    73868 2024-04-20 05:16:14.000000 webscout-1.3.4/webscout/webai.py
+-rw-rw-rw-   0        0        0     3085 2024-04-11 08:32:30.000000 webscout-1.3.4/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    40670 2024-04-11 08:32:30.000000 webscout-1.3.4/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-04-20 05:46:03.010857 webscout-1.3.4/webscout.egg-info/
+-rw-rw-rw-   0        0        0    31947 2024-04-20 05:46:01.000000 webscout-1.3.4/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2024-04-20 05:46:02.000000 webscout-1.3.4/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 05:46:01.000000 webscout-1.3.4/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2024-04-20 05:46:01.000000 webscout-1.3.4/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      334 2024-04-20 05:46:01.000000 webscout-1.3.4/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-20 05:46:01.000000 webscout-1.3.4/webscout.egg-info/top_level.txt
```

### Comparing `webscout-1.3.3/DeepWEBS/documents/query_results_extractor.py` & `webscout-1.3.4/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.3/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-1.3.4/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.3/DeepWEBS/networks/filepath_converter.py` & `webscout-1.3.4/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.3/DeepWEBS/networks/google_searcher.py` & `webscout-1.3.4/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.3/DeepWEBS/networks/network_configs.py` & `webscout-1.3.4/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.3/DeepWEBS/networks/webpage_fetcher.py` & `webscout-1.3.4/DeepWEBS/networks/webpage_fetcher.py`

 * *Files 11% similar despite different names*

```diff
@@ -74,24 +74,22 @@
         logger.success(f"> [{self.done_count}/{self.total_count}] Fetched: {url}")
         return url, html_path
 
     def fetch(self, urls: List[str], overwrite: bool = False, output_parent: str = None) -> List[Dict[str, str]]:
         self.urls = urls
         self.total_count = len(self.urls)
 
-        with concurrent.futures.ThreadPoolExecutor() as executor:
+        with concurrent.futures.ProcessPoolExecutor() as executor:
             futures = [
-                executor.submit(self.fetch_single_webpage, url, overwrite, output_parent)
+                executor.submit(WebpageFetcher().fetch, url, overwrite, output_parent)
                 for url in urls
             ]
             concurrent.futures.wait(futures)
 
+        self.url_and_html_path_list = [
+            {"url": future.result().url, "html_path": str(future.result().html_path)}
+            for future in futures
+        ]
+
         return self.url_and_html_path_list
 
-if __name__ == "__main__":
-    urls = [
-        "https://stackoverflow.com/questions/295135/turn-a-string-into-a-valid-filename",
-        "https://www.liaoxuefeng.com/wiki/1016959663602400/1017495723838528",
-        "https://docs.python.org/zh-cn/3/tutorial/interpreter.html",
-    ]
-    batch_webpage_fetcher = BatchWebpageFetcher()
-    batch_webpage_fetcher.fetch(urls=urls, overwrite=True, output_parent="python tutorials")
+
```

### Comparing `webscout-1.3.3/DeepWEBS/utilsdw/logger.py` & `webscout-1.3.4/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.3/LICENSE.md` & `webscout-1.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-1.3.3/PKG-INFO` & `webscout-1.3.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,66 +1,14 @@
-Metadata-Version: 2.1
-Name: webscout
-Version: 1.3.3
-Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos and have TTS support
-Author: OEvortex
-Author-email: helpingai5@gmail.com
-License: HelpingAI Simplified Universal License
-Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
-Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
-Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
-Project-URL: YouTube, https://youtube.com/@OEvortex
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: docstring_inheritance>=2.1.2
-Requires-Dist: click>=8.1.7
-Requires-Dist: curl_cffi>=0.6.0b7
-Requires-Dist: lxml>=5.1.0
-Requires-Dist: nest-asyncio>=1.6.0
-Requires-Dist: selenium>=4.1.3
-Requires-Dist: tqdm>=4.64.0
-Requires-Dist: webdriver-manager>=3.5.4
-Requires-Dist: halo>=0.0.31
-Requires-Dist: g4f>=0.2.2.3
-Requires-Dist: rich
-Requires-Dist: python-dotenv
-Requires-Dist: Helpingai-T2
-Requires-Dist: beautifulsoup4
-Requires-Dist: markdownify
-Requires-Dist: pydantic
-Requires-Dist: requests
-Requires-Dist: sse_starlette
-Requires-Dist: termcolor
-Requires-Dist: tiktoken
-Requires-Dist: tldextract
-Requires-Dist: orjson
-Provides-Extra: dev
-Requires-Dist: ruff>=0.1.6; extra == "dev"
-Requires-Dist: pytest>=7.4.2; extra == "dev"
-
 #  webscout
 <p align="center">
 
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/webscout"/></a>
 <a href="https://pepy.tech/project/webscout"><img alt="Downloads" src="https://static.pepy.tech/badge/webscout"></a>
 
-Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos
+Search for anything using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos, have TTS support and now has webai(terminal gpt and open interpeter) support
 
 
 ## Table of Contents
 - [webscout](#webscout)
   - [Table of Contents](#table-of-contents)
   - [Install](#install)
   - [CLI version](#cli-version)
@@ -96,14 +44,16 @@
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDIA` -](#9-koboldia--)
     - [10. `Sean` - chat With Sean](#10-sean---chat-with-sean)
   - [usage of special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
     - [`LLM`](#llm)
     - [`LLM` with internet](#llm-with-internet)
+  - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
+    - [for using as terminal gpt](#for-using-as-terminal-gpt)
 
 ## Install
 ```python
 pip install -U webscout
 ```
 ## CLI version
 
@@ -797,7 +747,53 @@
 
         # Print the response
         if response:
             print("AI:", response)
         else:
             print("No response")
 ```
+## `Webai` - terminal gpt and a open interpeter
+
+```python
+from webscout.webai import Main
+
+def use_rawdog_with_webai(prompt):
+    """
+    Wrap the webscout default method in a try-except block to catch any unhandled
+    exceptions and print a helpful message.
+    """
+    try:
+        webai_bot = Main(
+            max_tokens=500, 
+            provider="phind",
+            temperature=0.7,  
+            top_k=40,          
+            top_p=0.95,        
+            model="Phind Model",  # Replace with your desired model
+            auth=None,       # Replace with your auth key/value (if needed)
+            timeout=30,
+            disable_conversation=True,
+            filepath=None,
+            update_file=True,
+            intro=None,
+            rawdog=True,
+            history_offset=10250,
+            awesome_prompt=None,
+            proxy_path=None,
+            quiet=True
+        )
+        webai_response = webai_bot.default(prompt) 
+    except Exception as e:
+        print("Unexpected error:", e)
+
+
+if __name__ == "__main__":
+    user_prompt = input("Enter your prompt: ")
+    use_rawdog_with_webai(user_prompt)
+```
+```shell
+python -m webscout.webai webai --provider "phind" --rawdog
+```
+### for using as terminal gpt
+```python
+python -m webscout.webai webai --provider "sean"
+```
```

#### html2text {}

```diff
@@ -1,114 +1,89 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.3.3 Summary: Search for words,
-documents, images, videos, news, maps and text translation using the Google,
-DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can
-transcribe yt videos and have TTS support Author: OEvortex Author-email:
-helpingai5@gmail.com License: HelpingAI Simplified Universal License Project-
-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki Project-URL:
-Source, https://github.com/OE-LUCIFER/Webscout Project-URL: Tracker, https://
-github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube, https://
-youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers Classifier: License :: Other/
-Proprietary License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
-Programming Language :: Python :: Implementation :: CPython Classifier: Topic
-:: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Description-Content-Type: text/
-markdown License-File: LICENSE.md Requires-Dist: docstring_inheritance>=2.1.2
-Requires-Dist: click>=8.1.7 Requires-Dist: curl_cffi>=0.6.0b7 Requires-Dist:
-lxml>=5.1.0 Requires-Dist: nest-asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3
-Requires-Dist: tqdm>=4.64.0 Requires-Dist: webdriver-manager>=3.5.4 Requires-
-Dist: halo>=0.0.31 Requires-Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-
-Dist: python-dotenv Requires-Dist: Helpingai-T2 Requires-Dist: beautifulsoup4
-Requires-Dist: markdownify Requires-Dist: pydantic Requires-Dist: requests
-Requires-Dist: sse_starlette Requires-Dist: termcolor Requires-Dist: tiktoken
-Requires-Dist: tldextract Requires-Dist: orjson Provides-Extra: dev Requires-
-Dist: ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra == "dev"
 # webscout
- _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for words, documents, images, videos, news,
-maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com,
-you.com, etc Also containes AI models and now can transcribe yt videos ## Table
-of Contents - [webscout](#webscout) - [Table of Contents](#table-of-contents) -
- [Install](#install) - [CLI version](#cli-version) - [CLI to use LLM](#cli-to-
-   use-llm) - [Regions](#regions) - [Transcriber](#transcriber) - [DeepWEBS:
-Advanced Web Searches](#deepwebs-advanced-web-searches) - [Activating DeepWEBS]
-(#activating-deepwebs) - [Point to remember before using `DeepWEBS`](#point-to-
- remember-before-using-deepwebs) - [Usage Example](#usage-example) - [Text-to-
- Speech:](#text-to-speech) - [Available TTS Voices:](#available-tts-voices) -
-[ALL voices:](#all-voices) - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-
-classes) - [Exceptions](#exceptions) - [usage of webscout](#usage-of-webscout)
-  - [1. `text()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-
-  search-by-duckduckgocom-and-yepcom) - [2. `answers()` - instant answers by
-DuckDuckGo.com and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-
-  yepcom) - [3. `images()` - image search by DuckDuckGo.com and Yep.com](#3-
-  images---image-search-by-duckduckgocom-and-yepcom) - [4. `videos()` - video
-  search by DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom) - [5.
-`news()` - news search by DuckDuckGo.com and yep.com](#5-news---news-search-by-
- duckduckgocom-and-yepcom) - [6. `maps()` - map search by DuckDuckGo.com and]
- (#6-maps---map-search-by-duckduckgocom-and) - [7. `translate()` - translation
-by DuckDuckGo.com and Yep.com](#7-translate---translation-by-duckduckgocom-and-
-yepcom) - [8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-
-suggestions---suggestions-by-duckduckgocom-and-yepcom) - [usage of webscout.AI]
-   (#usage-of-webscoutai) - [1. `PhindSearch` - Search using Phind.com](#1-
- phindsearch---search-using-phindcom) - [2. `YepChat` - Chat with mistral 8x7b
-powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat) -
-  [3. `You.com` - search with you.com](#3-youcom---search-with-youcom) - [4.
-`Gemini` - search with google gemini](#4-gemini---search-with-google-gemini) -
-  [usage of image generator from Webscout.AI](#usage-of-image-generator-from-
- webscoutai) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-
-  using-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
-  searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
- perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
-opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Sean` -
- chat With Sean](#10-sean---chat-with-sean) - [usage of special .LLM file from
-webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
-    - [`LLM`](#llm) - [`LLM` with internet](#llm-with-internet) ## Install
-   ```python pip install -U webscout ``` ## CLI version ```python3 python -
-m webscout --help ``` | Command | Description | |------------------------------
--------------|-----------------------------------------------------------------
---------------------------------------| | python -m webscout answers -k Text |
-    CLI function to perform an answers search using Webscout. | | python -
-  m webscout images -k Text | CLI function to perform an images search using
-Webscout. | | python -m webscout maps -k Text | CLI function to perform a maps
- search using Webscout. | | python -m webscout news -k Text | CLI function to
-  perform a news search using Webscout. | | python -m webscout suggestions -
-   k Text | CLI function to perform a suggestions search using Webscout. | |
- python -m webscout text -k Text | CLI function to perform a text search using
- Webscout. | | python -m webscout translate -k Text | CLI function to perform
-   translate using Webscout. | | python -m webscout version | A command-line
-   interface command that prints and returns the version of the program. | |
-  python -m webscout videos -k Text | CLI function to perform a videos search
-  using DuckDuckGo API. | ## CLI to use LLM ```python python -m webscout.LLM
- model_name ``` [Go To TOP](#TOP) ## Regions expand xa-ar for Arabia xa-en for
-Arabia (en) ar-es for Argentina au-en for Australia at-de for Austria be-fr for
- Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg for Bulgaria ca-en
- for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for Chile cn-zh for
- China co-es for Colombia hr-hr for Croatia cz-cs for Czech Republic dk-da for
-Denmark ee-et for Estonia fi-fi for Finland fr-fr for France de-de for Germany
- gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en for India id-id
-for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he for Israel it-it
-for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-lt for Lithuania
- xl-es for Latin America my-ms for Malaysia my-en for Malaysia (en) mx-es for
- Mexico nl-nl for Netherlands nz-en for New Zealand no-no for Norway pe-es for
- Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl for Poland pt-pt
- for Portugal ro-ro for Romania ru-ru for Russia sg-en for Singapore sk-sk for
-Slovak Republic sl-sl for Slovenia za-en for South Africa es-es for Spain se-sv
-  for Sweden ch-de for Switzerland (de) ch-fr for Switzerland (fr) ch-it for
- Switzerland (it) tw-tzh for Taiwan th-th for Thailand tr-tr for Turkey ua-uk
- for Ukraine uk-en for United Kingdom us-en for United States ue-es for United
- States (es) ve-es for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go
- To TOP](#TOP) ## Transcriber The transcriber function in webscout is a handy
-tool that transcribes YouTube videos. Here's an example code demonstrating its
-       usage: ```python import sys from webscout import transcriber def
-    extract_transcript(video_id): """Extracts the transcript from a YouTube
-  video.""" try: transcript_list = transcriber.list_transcripts(video_id) for
-transcript in transcript_list: transcript_data_list = transcript.fetch() lang =
+       _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using the Google,
+DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can
+transcribe yt videos, have TTS support and now has webai(terminal gpt and open
+ interpeter) support ## Table of Contents - [webscout](#webscout) - [Table of
+   Contents](#table-of-contents) - [Install](#install) - [CLI version](#cli-
+     version) - [CLI to use LLM](#cli-to-use-llm) - [Regions](#regions) -
+  [Transcriber](#transcriber) - [DeepWEBS: Advanced Web Searches](#deepwebs-
+ advanced-web-searches) - [Activating DeepWEBS](#activating-deepwebs) - [Point
+to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
+   - [Usage Example](#usage-example) - [Text-to-Speech:](#text-to-speech) -
+[Available TTS Voices:](#available-tts-voices) - [ALL voices:](#all-voices) -
+   [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-classes) - [Exceptions]
+ (#exceptions) - [usage of webscout](#usage-of-webscout) - [1. `text()` - text
+ search by DuckDuckGo.com and Yep.com](#1-text---text-search-by-duckduckgocom-
+and-yepcom) - [2. `answers()` - instant answers by DuckDuckGo.com and Yep.com]
+ (#2-answers---instant-answers-by-duckduckgocom-and-yepcom) - [3. `images()` -
+   image search by DuckDuckGo.com and Yep.com](#3-images---image-search-by-
+ duckduckgocom-and-yepcom) - [4. `videos()` - video search by DuckDuckGo.com]
+  (#4-videos---video-search-by-duckduckgocom) - [5. `news()` - news search by
+DuckDuckGo.com and yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom)
+  - [6. `maps()` - map search by DuckDuckGo.com and](#6-maps---map-search-by-
+  duckduckgocom-and) - [7. `translate()` - translation by DuckDuckGo.com and
+    Yep.com](#7-translate---translation-by-duckduckgocom-and-yepcom) - [8.
+`suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-suggestions---
+ suggestions-by-duckduckgocom-and-yepcom) - [usage of webscout.AI](#usage-of-
+  webscoutai) - [1. `PhindSearch` - Search using Phind.com](#1-phindsearch---
+  search-using-phindcom) - [2. `YepChat` - Chat with mistral 8x7b powered by
+    yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat) - [3.
+`You.com` - search with you.com](#3-youcom---search-with-youcom) - [4. `Gemini`
+- search with google gemini](#4-gemini---search-with-google-gemini) - [usage of
+image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai) -
+[5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia) -
+  [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-
+blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-
+ with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-
+  opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Sean` - chat With Sean]
+   (#10-sean---chat-with-sean) - [usage of special .LLM file from webscout
+(webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm) - [`LLM`]
+ (#llm) - [`LLM` with internet](#llm-with-internet) - [`Webai` - terminal gpt
+  and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter) - [for
+  using as terminal gpt](#for-using-as-terminal-gpt) ## Install ```python pip
+install -U webscout ``` ## CLI version ```python3 python -m webscout --help ```
+| Command | Description | |-------------------------------------------|--------
+-------------------------------------------------------------------------------
+   ----------------| | python -m webscout answers -k Text | CLI function to
+perform an answers search using Webscout. | | python -m webscout images -k Text
+    | CLI function to perform an images search using Webscout. | | python -
+m webscout maps -k Text | CLI function to perform a maps search using Webscout.
+  | | python -m webscout news -k Text | CLI function to perform a news search
+ using Webscout. | | python -m webscout suggestions -k Text | CLI function to
+  perform a suggestions search using Webscout. | | python -m webscout text -
+  k Text | CLI function to perform a text search using Webscout. | | python -
+    m webscout translate -k Text | CLI function to perform translate using
+  Webscout. | | python -m webscout version | A command-line interface command
+  that prints and returns the version of the program. | | python -m webscout
+videos -k Text | CLI function to perform a videos search using DuckDuckGo API.
+| ## CLI to use LLM ```python python -m webscout.LLM model_name ``` [Go To TOP]
+   (#TOP) ## Regions expand xa-ar for Arabia xa-en for Arabia (en) ar-es for
+ Argentina au-en for Australia at-de for Austria be-fr for Belgium (fr) be-nl
+for Belgium (nl) br-pt for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for
+    Canada (fr) ct-ca for Catalan cl-es for Chile cn-zh for China co-es for
+Colombia hr-hr for Croatia cz-cs for Czech Republic dk-da for Denmark ee-et for
+ Estonia fi-fi for Finland fr-fr for France de-de for Germany gr-el for Greece
+hk-tzh for Hong Kong hu-hu for Hungary in-en for India id-id for Indonesia id-
+en for Indonesia (en) ie-en for Ireland il-he for Israel it-it for Italy jp-jp
+for Japan kr-kr for Korea lv-lv for Latvia lt-lt for Lithuania xl-es for Latin
+ America my-ms for Malaysia my-en for Malaysia (en) mx-es for Mexico nl-nl for
+  Netherlands nz-en for New Zealand no-no for Norway pe-es for Peru ph-en for
+Philippines ph-tl for Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-
+ ro for Romania ru-ru for Russia sg-en for Singapore sk-sk for Slovak Republic
+sl-sl for Slovenia za-en for South Africa es-es for Spain se-sv for Sweden ch-
+ de for Switzerland (de) ch-fr for Switzerland (fr) ch-it for Switzerland (it)
+ tw-tzh for Taiwan th-th for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en
+ for United Kingdom us-en for United States ue-es for United States (es) ve-es
+ for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ##
+     Transcriber The transcriber function in webscout is a handy tool that
+  transcribes YouTube videos. Here's an example code demonstrating its usage:
+ ```python import sys from webscout import transcriber def extract_transcript
+     (video_id): """Extracts the transcript from a YouTube video.""" try:
+  transcript_list = transcriber.list_transcripts(video_id) for transcript in
+       transcript_list: transcript_data_list = transcript.fetch() lang =
  transcript.language transcript_text = "" if transcript.language_code == 'en':
     for line in transcript_data_list: start_time = line['start'] end_time =
      start_time + line['duration'] formatted_line = f"{start_time:.2f} -
   {end_time:.2f}: {line['text']}\n" transcript_text += formatted_line return
   transcript_text elif transcript.is_translatable: english_transcript_list =
     transcript.translate('en').fetch() for line in english_transcript_list:
       start_time = line['start'] end_time = start_time + line['duration']
@@ -346,8 +321,21 @@
    messages to be sent, including the user input, search results, and system
 message messages = [ {"role": "user", "content": user_input + "\n" + "websearch
 results are:" + "\n".join(search_results)}, ] # Use the chat method to get the
      response response = LLM.chat(messages) return response if __name__ ==
   "__main__": while True: # Get the user input user_input = input("User: ") #
  Perform a web search based on the user input with WEBS() as webs: response =
 chat(user_input, webs) # Print the response if response: print("AI:", response)
-                        else: print("No response") ```
+else: print("No response") ``` ## `Webai` - terminal gpt and a open interpeter
+ ```python from webscout.webai import Main def use_rawdog_with_webai(prompt):
+    """ Wrap the webscout default method in a try-except block to catch any
+  unhandled exceptions and print a helpful message. """ try: webai_bot = Main
+  ( max_tokens=500, provider="phind", temperature=0.7, top_k=40, top_p=0.95,
+  model="Phind Model", # Replace with your desired model auth=None, # Replace
+  with your auth key/value (if needed) timeout=30, disable_conversation=True,
+filepath=None, update_file=True, intro=None, rawdog=True, history_offset=10250,
+      awesome_prompt=None, proxy_path=None, quiet=True ) webai_response =
+webai_bot.default(prompt) except Exception as e: print("Unexpected error:", e)
+     if __name__ == "__main__": user_prompt = input("Enter your prompt: ")
+use_rawdog_with_webai(user_prompt) ``` ```shell python -m webscout.webai webai
+--provider "phind" --rawdog ``` ### for using as terminal gpt ```python python
+                 -m webscout.webai webai --provider "sean" ```
```

### Comparing `webscout-1.3.3/README.md` & `webscout-1.3.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,66 @@
+Metadata-Version: 2.1
+Name: webscout
+Version: 1.3.4
+Summary: Search for anything using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos, have TTS support and now has webai(terminal gpt and open interpeter) support
+Author: OEvortex
+Author-email: helpingai5@gmail.com
+License: HelpingAI Simplified Universal License
+Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
+Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
+Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
+Project-URL: YouTube, https://youtube.com/@OEvortex
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: docstring_inheritance>=2.1.2
+Requires-Dist: click>=8.1.7
+Requires-Dist: curl_cffi>=0.6.0b7
+Requires-Dist: lxml>=5.1.0
+Requires-Dist: nest-asyncio>=1.6.0
+Requires-Dist: selenium>=4.1.3
+Requires-Dist: tqdm>=4.64.0
+Requires-Dist: webdriver-manager>=3.5.4
+Requires-Dist: halo>=0.0.31
+Requires-Dist: g4f>=0.2.2.3
+Requires-Dist: rich
+Requires-Dist: python-dotenv
+Requires-Dist: Helpingai-T2
+Requires-Dist: beautifulsoup4
+Requires-Dist: markdownify
+Requires-Dist: pydantic
+Requires-Dist: requests
+Requires-Dist: sse_starlette
+Requires-Dist: termcolor
+Requires-Dist: tiktoken
+Requires-Dist: tldextract
+Requires-Dist: orjson
+Provides-Extra: dev
+Requires-Dist: ruff>=0.1.6; extra == "dev"
+Requires-Dist: pytest>=7.4.2; extra == "dev"
+
 #  webscout
 <p align="center">
 
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/webscout"/></a>
 <a href="https://pepy.tech/project/webscout"><img alt="Downloads" src="https://static.pepy.tech/badge/webscout"></a>
 
-Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos
+Search for anything using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos, have TTS support and now has webai(terminal gpt and open interpeter) support
 
 
 ## Table of Contents
 - [webscout](#webscout)
   - [Table of Contents](#table-of-contents)
   - [Install](#install)
   - [CLI version](#cli-version)
@@ -44,14 +96,16 @@
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDIA` -](#9-koboldia--)
     - [10. `Sean` - chat With Sean](#10-sean---chat-with-sean)
   - [usage of special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
     - [`LLM`](#llm)
     - [`LLM` with internet](#llm-with-internet)
+  - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
+    - [for using as terminal gpt](#for-using-as-terminal-gpt)
 
 ## Install
 ```python
 pip install -U webscout
 ```
 ## CLI version
 
@@ -744,8 +798,54 @@
             response = chat(user_input, webs)
 
         # Print the response
         if response:
             print("AI:", response)
         else:
             print("No response")
-```
+```
+## `Webai` - terminal gpt and a open interpeter
+
+```python
+from webscout.webai import Main
+
+def use_rawdog_with_webai(prompt):
+    """
+    Wrap the webscout default method in a try-except block to catch any unhandled
+    exceptions and print a helpful message.
+    """
+    try:
+        webai_bot = Main(
+            max_tokens=500, 
+            provider="phind",
+            temperature=0.7,  
+            top_k=40,          
+            top_p=0.95,        
+            model="Phind Model",  # Replace with your desired model
+            auth=None,       # Replace with your auth key/value (if needed)
+            timeout=30,
+            disable_conversation=True,
+            filepath=None,
+            update_file=True,
+            intro=None,
+            rawdog=True,
+            history_offset=10250,
+            awesome_prompt=None,
+            proxy_path=None,
+            quiet=True
+        )
+        webai_response = webai_bot.default(prompt) 
+    except Exception as e:
+        print("Unexpected error:", e)
+
+
+if __name__ == "__main__":
+    user_prompt = input("Enter your prompt: ")
+    use_rawdog_with_webai(user_prompt)
+```
+```shell
+python -m webscout.webai webai --provider "phind" --rawdog
+```
+### for using as terminal gpt
+```python
+python -m webscout.webai webai --provider "sean"
+```
```

#### html2text {}

```diff
@@ -1,86 +1,117 @@
-# webscout
- _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for words, documents, images, videos, news,
-maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com,
-you.com, etc Also containes AI models and now can transcribe yt videos ## Table
-of Contents - [webscout](#webscout) - [Table of Contents](#table-of-contents) -
- [Install](#install) - [CLI version](#cli-version) - [CLI to use LLM](#cli-to-
-   use-llm) - [Regions](#regions) - [Transcriber](#transcriber) - [DeepWEBS:
-Advanced Web Searches](#deepwebs-advanced-web-searches) - [Activating DeepWEBS]
-(#activating-deepwebs) - [Point to remember before using `DeepWEBS`](#point-to-
- remember-before-using-deepwebs) - [Usage Example](#usage-example) - [Text-to-
- Speech:](#text-to-speech) - [Available TTS Voices:](#available-tts-voices) -
-[ALL voices:](#all-voices) - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-
-classes) - [Exceptions](#exceptions) - [usage of webscout](#usage-of-webscout)
-  - [1. `text()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-
-  search-by-duckduckgocom-and-yepcom) - [2. `answers()` - instant answers by
-DuckDuckGo.com and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-
-  yepcom) - [3. `images()` - image search by DuckDuckGo.com and Yep.com](#3-
-  images---image-search-by-duckduckgocom-and-yepcom) - [4. `videos()` - video
-  search by DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom) - [5.
-`news()` - news search by DuckDuckGo.com and yep.com](#5-news---news-search-by-
- duckduckgocom-and-yepcom) - [6. `maps()` - map search by DuckDuckGo.com and]
- (#6-maps---map-search-by-duckduckgocom-and) - [7. `translate()` - translation
-by DuckDuckGo.com and Yep.com](#7-translate---translation-by-duckduckgocom-and-
-yepcom) - [8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-
-suggestions---suggestions-by-duckduckgocom-and-yepcom) - [usage of webscout.AI]
-   (#usage-of-webscoutai) - [1. `PhindSearch` - Search using Phind.com](#1-
- phindsearch---search-using-phindcom) - [2. `YepChat` - Chat with mistral 8x7b
-powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat) -
-  [3. `You.com` - search with you.com](#3-youcom---search-with-youcom) - [4.
-`Gemini` - search with google gemini](#4-gemini---search-with-google-gemini) -
-  [usage of image generator from Webscout.AI](#usage-of-image-generator-from-
- webscoutai) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-
-  using-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
-  searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
- perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
-opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Sean` -
- chat With Sean](#10-sean---chat-with-sean) - [usage of special .LLM file from
-webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
-    - [`LLM`](#llm) - [`LLM` with internet](#llm-with-internet) ## Install
-   ```python pip install -U webscout ``` ## CLI version ```python3 python -
-m webscout --help ``` | Command | Description | |------------------------------
--------------|-----------------------------------------------------------------
---------------------------------------| | python -m webscout answers -k Text |
-    CLI function to perform an answers search using Webscout. | | python -
-  m webscout images -k Text | CLI function to perform an images search using
-Webscout. | | python -m webscout maps -k Text | CLI function to perform a maps
- search using Webscout. | | python -m webscout news -k Text | CLI function to
-  perform a news search using Webscout. | | python -m webscout suggestions -
-   k Text | CLI function to perform a suggestions search using Webscout. | |
- python -m webscout text -k Text | CLI function to perform a text search using
- Webscout. | | python -m webscout translate -k Text | CLI function to perform
-   translate using Webscout. | | python -m webscout version | A command-line
-   interface command that prints and returns the version of the program. | |
-  python -m webscout videos -k Text | CLI function to perform a videos search
-  using DuckDuckGo API. | ## CLI to use LLM ```python python -m webscout.LLM
- model_name ``` [Go To TOP](#TOP) ## Regions expand xa-ar for Arabia xa-en for
-Arabia (en) ar-es for Argentina au-en for Australia at-de for Austria be-fr for
- Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg for Bulgaria ca-en
- for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for Chile cn-zh for
- China co-es for Colombia hr-hr for Croatia cz-cs for Czech Republic dk-da for
-Denmark ee-et for Estonia fi-fi for Finland fr-fr for France de-de for Germany
- gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en for India id-id
-for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he for Israel it-it
-for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-lt for Lithuania
- xl-es for Latin America my-ms for Malaysia my-en for Malaysia (en) mx-es for
- Mexico nl-nl for Netherlands nz-en for New Zealand no-no for Norway pe-es for
- Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl for Poland pt-pt
- for Portugal ro-ro for Romania ru-ru for Russia sg-en for Singapore sk-sk for
-Slovak Republic sl-sl for Slovenia za-en for South Africa es-es for Spain se-sv
-  for Sweden ch-de for Switzerland (de) ch-fr for Switzerland (fr) ch-it for
- Switzerland (it) tw-tzh for Taiwan th-th for Thailand tr-tr for Turkey ua-uk
- for Ukraine uk-en for United Kingdom us-en for United States ue-es for United
- States (es) ve-es for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go
- To TOP](#TOP) ## Transcriber The transcriber function in webscout is a handy
-tool that transcribes YouTube videos. Here's an example code demonstrating its
-       usage: ```python import sys from webscout import transcriber def
-    extract_transcript(video_id): """Extracts the transcript from a YouTube
-  video.""" try: transcript_list = transcriber.list_transcripts(video_id) for
-transcript in transcript_list: transcript_data_list = transcript.fetch() lang =
+Metadata-Version: 2.1 Name: webscout Version: 1.3.4 Summary: Search for
+anything using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc
+Also containes AI models, can transcribe yt videos, have TTS support and now
+has webai(terminal gpt and open interpeter) support Author: OEvortex Author-
+email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
+Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
+Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
+Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
+https://youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/
+Stable Classifier: Intended Audience :: Developers Classifier: License ::
+Other/Proprietary License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic
+:: Software Development :: Libraries :: Python Modules Description-Content-
+Type: text/markdown License-File: LICENSE.md Requires-Dist:
+docstring_inheritance>=2.1.2 Requires-Dist: click>=8.1.7 Requires-Dist:
+curl_cffi>=0.6.0b7 Requires-Dist: lxml>=5.1.0 Requires-Dist: nest-
+asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3 Requires-Dist: tqdm>=4.64.0
+Requires-Dist: webdriver-manager>=3.5.4 Requires-Dist: halo>=0.0.31 Requires-
+Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
+Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
+Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
+Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
+Requires-Dist: orjson Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra ==
+"dev" Requires-Dist: pytest>=7.4.2; extra == "dev" # webscout
+       _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using the Google,
+DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can
+transcribe yt videos, have TTS support and now has webai(terminal gpt and open
+ interpeter) support ## Table of Contents - [webscout](#webscout) - [Table of
+   Contents](#table-of-contents) - [Install](#install) - [CLI version](#cli-
+     version) - [CLI to use LLM](#cli-to-use-llm) - [Regions](#regions) -
+  [Transcriber](#transcriber) - [DeepWEBS: Advanced Web Searches](#deepwebs-
+ advanced-web-searches) - [Activating DeepWEBS](#activating-deepwebs) - [Point
+to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
+   - [Usage Example](#usage-example) - [Text-to-Speech:](#text-to-speech) -
+[Available TTS Voices:](#available-tts-voices) - [ALL voices:](#all-voices) -
+   [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-classes) - [Exceptions]
+ (#exceptions) - [usage of webscout](#usage-of-webscout) - [1. `text()` - text
+ search by DuckDuckGo.com and Yep.com](#1-text---text-search-by-duckduckgocom-
+and-yepcom) - [2. `answers()` - instant answers by DuckDuckGo.com and Yep.com]
+ (#2-answers---instant-answers-by-duckduckgocom-and-yepcom) - [3. `images()` -
+   image search by DuckDuckGo.com and Yep.com](#3-images---image-search-by-
+ duckduckgocom-and-yepcom) - [4. `videos()` - video search by DuckDuckGo.com]
+  (#4-videos---video-search-by-duckduckgocom) - [5. `news()` - news search by
+DuckDuckGo.com and yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom)
+  - [6. `maps()` - map search by DuckDuckGo.com and](#6-maps---map-search-by-
+  duckduckgocom-and) - [7. `translate()` - translation by DuckDuckGo.com and
+    Yep.com](#7-translate---translation-by-duckduckgocom-and-yepcom) - [8.
+`suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-suggestions---
+ suggestions-by-duckduckgocom-and-yepcom) - [usage of webscout.AI](#usage-of-
+  webscoutai) - [1. `PhindSearch` - Search using Phind.com](#1-phindsearch---
+  search-using-phindcom) - [2. `YepChat` - Chat with mistral 8x7b powered by
+    yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat) - [3.
+`You.com` - search with you.com](#3-youcom---search-with-youcom) - [4. `Gemini`
+- search with google gemini](#4-gemini---search-with-google-gemini) - [usage of
+image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai) -
+[5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia) -
+  [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-
+blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-
+ with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-
+  opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Sean` - chat With Sean]
+   (#10-sean---chat-with-sean) - [usage of special .LLM file from webscout
+(webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm) - [`LLM`]
+ (#llm) - [`LLM` with internet](#llm-with-internet) - [`Webai` - terminal gpt
+  and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter) - [for
+  using as terminal gpt](#for-using-as-terminal-gpt) ## Install ```python pip
+install -U webscout ``` ## CLI version ```python3 python -m webscout --help ```
+| Command | Description | |-------------------------------------------|--------
+-------------------------------------------------------------------------------
+   ----------------| | python -m webscout answers -k Text | CLI function to
+perform an answers search using Webscout. | | python -m webscout images -k Text
+    | CLI function to perform an images search using Webscout. | | python -
+m webscout maps -k Text | CLI function to perform a maps search using Webscout.
+  | | python -m webscout news -k Text | CLI function to perform a news search
+ using Webscout. | | python -m webscout suggestions -k Text | CLI function to
+  perform a suggestions search using Webscout. | | python -m webscout text -
+  k Text | CLI function to perform a text search using Webscout. | | python -
+    m webscout translate -k Text | CLI function to perform translate using
+  Webscout. | | python -m webscout version | A command-line interface command
+  that prints and returns the version of the program. | | python -m webscout
+videos -k Text | CLI function to perform a videos search using DuckDuckGo API.
+| ## CLI to use LLM ```python python -m webscout.LLM model_name ``` [Go To TOP]
+   (#TOP) ## Regions expand xa-ar for Arabia xa-en for Arabia (en) ar-es for
+ Argentina au-en for Australia at-de for Austria be-fr for Belgium (fr) be-nl
+for Belgium (nl) br-pt for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for
+    Canada (fr) ct-ca for Catalan cl-es for Chile cn-zh for China co-es for
+Colombia hr-hr for Croatia cz-cs for Czech Republic dk-da for Denmark ee-et for
+ Estonia fi-fi for Finland fr-fr for France de-de for Germany gr-el for Greece
+hk-tzh for Hong Kong hu-hu for Hungary in-en for India id-id for Indonesia id-
+en for Indonesia (en) ie-en for Ireland il-he for Israel it-it for Italy jp-jp
+for Japan kr-kr for Korea lv-lv for Latvia lt-lt for Lithuania xl-es for Latin
+ America my-ms for Malaysia my-en for Malaysia (en) mx-es for Mexico nl-nl for
+  Netherlands nz-en for New Zealand no-no for Norway pe-es for Peru ph-en for
+Philippines ph-tl for Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-
+ ro for Romania ru-ru for Russia sg-en for Singapore sk-sk for Slovak Republic
+sl-sl for Slovenia za-en for South Africa es-es for Spain se-sv for Sweden ch-
+ de for Switzerland (de) ch-fr for Switzerland (fr) ch-it for Switzerland (it)
+ tw-tzh for Taiwan th-th for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en
+ for United Kingdom us-en for United States ue-es for United States (es) ve-es
+ for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ##
+     Transcriber The transcriber function in webscout is a handy tool that
+  transcribes YouTube videos. Here's an example code demonstrating its usage:
+ ```python import sys from webscout import transcriber def extract_transcript
+     (video_id): """Extracts the transcript from a YouTube video.""" try:
+  transcript_list = transcriber.list_transcripts(video_id) for transcript in
+       transcript_list: transcript_data_list = transcript.fetch() lang =
  transcript.language transcript_text = "" if transcript.language_code == 'en':
     for line in transcript_data_list: start_time = line['start'] end_time =
      start_time + line['duration'] formatted_line = f"{start_time:.2f} -
   {end_time:.2f}: {line['text']}\n" transcript_text += formatted_line return
   transcript_text elif transcript.is_translatable: english_transcript_list =
     transcript.translate('en').fetch() for line in english_transcript_list:
       start_time = line['start'] end_time = start_time + line['duration']
@@ -318,8 +349,21 @@
    messages to be sent, including the user input, search results, and system
 message messages = [ {"role": "user", "content": user_input + "\n" + "websearch
 results are:" + "\n".join(search_results)}, ] # Use the chat method to get the
      response response = LLM.chat(messages) return response if __name__ ==
   "__main__": while True: # Get the user input user_input = input("User: ") #
  Perform a web search based on the user input with WEBS() as webs: response =
 chat(user_input, webs) # Print the response if response: print("AI:", response)
-                        else: print("No response") ```
+else: print("No response") ``` ## `Webai` - terminal gpt and a open interpeter
+ ```python from webscout.webai import Main def use_rawdog_with_webai(prompt):
+    """ Wrap the webscout default method in a try-except block to catch any
+  unhandled exceptions and print a helpful message. """ try: webai_bot = Main
+  ( max_tokens=500, provider="phind", temperature=0.7, top_k=40, top_p=0.95,
+  model="Phind Model", # Replace with your desired model auth=None, # Replace
+  with your auth key/value (if needed) timeout=30, disable_conversation=True,
+filepath=None, update_file=True, intro=None, rawdog=True, history_offset=10250,
+      awesome_prompt=None, proxy_path=None, quiet=True ) webai_response =
+webai_bot.default(prompt) except Exception as e: print("Unexpected error:", e)
+     if __name__ == "__main__": user_prompt = input("Enter your prompt: ")
+use_rawdog_with_webai(user_prompt) ``` ```shell python -m webscout.webai webai
+--provider "phind" --rawdog ``` ### for using as terminal gpt ```python python
+                 -m webscout.webai webai --provider "sean" ```
```

### Comparing `webscout-1.3.3/setup.py` & `webscout-1.3.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="1.3.3", 
-    description="Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos and have TTS support",
+    version="1.3.4", 
+    description="Search for anything using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos, have TTS support and now has webai(terminal gpt and open interpeter) support",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

### Comparing `webscout-1.3.3/webscout/AI.py` & `webscout-1.3.4/webscout/AI.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.3/webscout/AIbase.py` & `webscout-1.3.4/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.3/webscout/AIutel.py` & `webscout-1.3.4/webscout/AIutel.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,39 @@
 import appdirs
 import datetime
 import re
 import sys
 import click
 from rich.markdown import Markdown
 from rich.console import Console
-
+import g4f
 appdir = appdirs.AppDirs("AIWEBS", "vortex")
 
 default_path = appdir.user_cache_dir
 
 if not os.path.exists(default_path):
     os.makedirs(default_path)
+webai = [
+    "leo",
+    "openai",
+    "opengpt",
+    "koboldai",
+    "gemini",
+    "phind",
+    "blackboxai",
+    "g4fauto",
+    "perplexity",
+    "sean",
+]
+
+gpt4free_providers = [
+    provider.__name__ for provider in g4f.Provider.__providers__  # if provider.working
+]
 
+available_providers = webai + gpt4free_providers
 
 def run_system_command(
     command: str,
     exit_on_error: bool = True,
     stdout_error: bool = True,
     help: str = None,
 ):
@@ -464,15 +481,14 @@
 
 LLM:
 ```python
 print("The essay is about...")
 ```
 """
 
-    # Idea borrowed from https://github.com/AbanteAI/rawdog
 
     def __init__(
         self,
         quiet: bool = False,
         internal_exec: bool = False,
         confirm_script: bool = False,
         interpreter: str = "python",
```

### Comparing `webscout-1.3.3/webscout/DWEBS.py` & `webscout-1.3.4/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.3/webscout/HelpingAI.py` & `webscout-1.3.4/webscout/HelpingAI.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.3/webscout/LLM.py` & `webscout-1.3.4/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.3/webscout/__init__.py` & `webscout-1.3.4/webscout/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Webscout.
 
-Search for words, documents, images, videos, news, maps and text translation 
-using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
+Search for anything using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos, have TTS support and now has webai(terminal gpt and open interpeter) support
 """
 import g4f
 import logging
 from .webscout_search import WEBS
 from .webscout_search_async import AsyncWEBS
 from .version import __version__
 from .DWEBS import DeepWEBS
```

### Comparing `webscout-1.3.3/webscout/cli.py` & `webscout-1.3.4/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.3/webscout/g4f.py` & `webscout-1.3.4/webscout/g4f.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import g4f
 from webscout.AIutel import Optimizers
 from webscout.AIutel import Conversation
 from webscout.AIutel import AwesomePrompts
-from webscout.AIutel import Provider
+from webscout.AIbase import Provider
 from webscout.AIutel import available_providers
 
 
 g4f.debug.version_check = False
 
 working_providers = available_providers
```

### Comparing `webscout-1.3.3/webscout/models.py` & `webscout-1.3.4/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.3/webscout/transcriber.py` & `webscout-1.3.4/webscout/transcriber.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.3/webscout/utils.py` & `webscout-1.3.4/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.3/webscout/voice.py` & `webscout-1.3.4/webscout/voice.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.3/webscout/webai.py` & `webscout-1.3.4/webscout/webai.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,27 +25,28 @@
 from rich.prompt import Prompt
 from rich.progress import Progress
 from typing import Iterator
 from webscout.AIutel import Optimizers
 from webscout.AIutel import default_path
 from webscout.AIutel import AwesomePrompts
 from webscout.AIutel import RawDog
+from webscout import available_providers
 from colorama import Fore
 from colorama import init as init_colorama
 from dotenv import load_dotenv
 import g4f
 
 import webscout.AIutel
 
 init_colorama(autoreset=True)
 
 load_dotenv()  # loads .env variables
 
 logging.basicConfig(
-    format="%(asctime)s - %(levelname)s : %(message)s ",  # [%(module)s,%(lineno)s]", # for debug purposes
+    format="%(asctime)s - %(levelname)s : %(message)s ",  
     datefmt="%H:%M:%S",
     level=logging.INFO,
 )
 
 try:
     clipman.init()
 except Exception as e:
@@ -57,15 +58,15 @@
 
 
 class this:
     """Console's common variables"""
 
     rich_code_themes = ["monokai", "paraiso-dark", "igor", "vs", "fruity", "xcode"]
 
-    default_provider = "sean"
+    default_provider = "phind"
 
     getExc = lambda e: e.args[1] if len(e.args) > 1 else str(e)
 
     context_settings = dict(auto_envvar_prefix="Webscout")
 
     """Console utils"""
 
@@ -1073,15 +1074,15 @@
     @webai_.group()  
     @click.help_option("-h", "--help")
     def awesome():
         """Perform CRUD operations on awesome-prompts"""
         pass
 
 
-
+import webscout
 class Chatwebai:
     """webai command"""
 
     @staticmethod
     @click.command(context_settings=this.context_settings)
     @click.option(
         "-m",
@@ -1190,15 +1191,15 @@
         "--proxy-path",
         type=click.Path(exists=True),
         help="Path to .json file containing proxies",
     )
     @click.option(
         "-p",
         "--provider",
-        type=click.Choice(webscout.available_providers),
+        type=click.Choice(available_providers),
         default=this.default_provider,
         help="Name of LLM provider.",
         metavar=(
             f"[{'|'.join(webscout.webai)}] etc, "
             "run 'webscout gpt4free list providers -w' to "
             "view more providers and 'webscout gpt4free test -y' "
             "for advanced g4f providers test"
```

### Comparing `webscout-1.3.3/webscout/webscout_search.py` & `webscout-1.3.4/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.3/webscout/webscout_search_async.py` & `webscout-1.3.4/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.3/webscout.egg-info/PKG-INFO` & `webscout-1.3.4/webscout.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.3.3
-Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos and have TTS support
+Version: 1.3.4
+Summary: Search for anything using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos, have TTS support and now has webai(terminal gpt and open interpeter) support
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
 Project-URL: YouTube, https://youtube.com/@OEvortex
@@ -52,15 +52,15 @@
 
 #  webscout
 <p align="center">
 
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/webscout"/></a>
 <a href="https://pepy.tech/project/webscout"><img alt="Downloads" src="https://static.pepy.tech/badge/webscout"></a>
 
-Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos
+Search for anything using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos, have TTS support and now has webai(terminal gpt and open interpeter) support
 
 
 ## Table of Contents
 - [webscout](#webscout)
   - [Table of Contents](#table-of-contents)
   - [Install](#install)
   - [CLI version](#cli-version)
@@ -96,14 +96,16 @@
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDIA` -](#9-koboldia--)
     - [10. `Sean` - chat With Sean](#10-sean---chat-with-sean)
   - [usage of special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
     - [`LLM`](#llm)
     - [`LLM` with internet](#llm-with-internet)
+  - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
+    - [for using as terminal gpt](#for-using-as-terminal-gpt)
 
 ## Install
 ```python
 pip install -U webscout
 ```
 ## CLI version
 
@@ -797,7 +799,53 @@
 
         # Print the response
         if response:
             print("AI:", response)
         else:
             print("No response")
 ```
+## `Webai` - terminal gpt and a open interpeter
+
+```python
+from webscout.webai import Main
+
+def use_rawdog_with_webai(prompt):
+    """
+    Wrap the webscout default method in a try-except block to catch any unhandled
+    exceptions and print a helpful message.
+    """
+    try:
+        webai_bot = Main(
+            max_tokens=500, 
+            provider="phind",
+            temperature=0.7,  
+            top_k=40,          
+            top_p=0.95,        
+            model="Phind Model",  # Replace with your desired model
+            auth=None,       # Replace with your auth key/value (if needed)
+            timeout=30,
+            disable_conversation=True,
+            filepath=None,
+            update_file=True,
+            intro=None,
+            rawdog=True,
+            history_offset=10250,
+            awesome_prompt=None,
+            proxy_path=None,
+            quiet=True
+        )
+        webai_response = webai_bot.default(prompt) 
+    except Exception as e:
+        print("Unexpected error:", e)
+
+
+if __name__ == "__main__":
+    user_prompt = input("Enter your prompt: ")
+    use_rawdog_with_webai(user_prompt)
+```
+```shell
+python -m webscout.webai webai --provider "phind" --rawdog
+```
+### for using as terminal gpt
+```python
+python -m webscout.webai webai --provider "sean"
+```
```

#### html2text {}

```diff
@@ -1,114 +1,117 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.3.3 Summary: Search for words,
-documents, images, videos, news, maps and text translation using the Google,
+Metadata-Version: 2.1 Name: webscout Version: 1.3.4 Summary: Search for
+anything using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc
+Also containes AI models, can transcribe yt videos, have TTS support and now
+has webai(terminal gpt and open interpeter) support Author: OEvortex Author-
+email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
+Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
+Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
+Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
+https://youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/
+Stable Classifier: Intended Audience :: Developers Classifier: License ::
+Other/Proprietary License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic
+:: Software Development :: Libraries :: Python Modules Description-Content-
+Type: text/markdown License-File: LICENSE.md Requires-Dist:
+docstring_inheritance>=2.1.2 Requires-Dist: click>=8.1.7 Requires-Dist:
+curl_cffi>=0.6.0b7 Requires-Dist: lxml>=5.1.0 Requires-Dist: nest-
+asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3 Requires-Dist: tqdm>=4.64.0
+Requires-Dist: webdriver-manager>=3.5.4 Requires-Dist: halo>=0.0.31 Requires-
+Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
+Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
+Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
+Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
+Requires-Dist: orjson Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra ==
+"dev" Requires-Dist: pytest>=7.4.2; extra == "dev" # webscout
+       _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using the Google,
 DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can
-transcribe yt videos and have TTS support Author: OEvortex Author-email:
-helpingai5@gmail.com License: HelpingAI Simplified Universal License Project-
-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki Project-URL:
-Source, https://github.com/OE-LUCIFER/Webscout Project-URL: Tracker, https://
-github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube, https://
-youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers Classifier: License :: Other/
-Proprietary License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
-Programming Language :: Python :: Implementation :: CPython Classifier: Topic
-:: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Description-Content-Type: text/
-markdown License-File: LICENSE.md Requires-Dist: docstring_inheritance>=2.1.2
-Requires-Dist: click>=8.1.7 Requires-Dist: curl_cffi>=0.6.0b7 Requires-Dist:
-lxml>=5.1.0 Requires-Dist: nest-asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3
-Requires-Dist: tqdm>=4.64.0 Requires-Dist: webdriver-manager>=3.5.4 Requires-
-Dist: halo>=0.0.31 Requires-Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-
-Dist: python-dotenv Requires-Dist: Helpingai-T2 Requires-Dist: beautifulsoup4
-Requires-Dist: markdownify Requires-Dist: pydantic Requires-Dist: requests
-Requires-Dist: sse_starlette Requires-Dist: termcolor Requires-Dist: tiktoken
-Requires-Dist: tldextract Requires-Dist: orjson Provides-Extra: dev Requires-
-Dist: ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra == "dev"
-# webscout
- _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for words, documents, images, videos, news,
-maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com,
-you.com, etc Also containes AI models and now can transcribe yt videos ## Table
-of Contents - [webscout](#webscout) - [Table of Contents](#table-of-contents) -
- [Install](#install) - [CLI version](#cli-version) - [CLI to use LLM](#cli-to-
-   use-llm) - [Regions](#regions) - [Transcriber](#transcriber) - [DeepWEBS:
-Advanced Web Searches](#deepwebs-advanced-web-searches) - [Activating DeepWEBS]
-(#activating-deepwebs) - [Point to remember before using `DeepWEBS`](#point-to-
- remember-before-using-deepwebs) - [Usage Example](#usage-example) - [Text-to-
- Speech:](#text-to-speech) - [Available TTS Voices:](#available-tts-voices) -
-[ALL voices:](#all-voices) - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-
-classes) - [Exceptions](#exceptions) - [usage of webscout](#usage-of-webscout)
-  - [1. `text()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-
-  search-by-duckduckgocom-and-yepcom) - [2. `answers()` - instant answers by
-DuckDuckGo.com and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-
-  yepcom) - [3. `images()` - image search by DuckDuckGo.com and Yep.com](#3-
-  images---image-search-by-duckduckgocom-and-yepcom) - [4. `videos()` - video
-  search by DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom) - [5.
-`news()` - news search by DuckDuckGo.com and yep.com](#5-news---news-search-by-
- duckduckgocom-and-yepcom) - [6. `maps()` - map search by DuckDuckGo.com and]
- (#6-maps---map-search-by-duckduckgocom-and) - [7. `translate()` - translation
-by DuckDuckGo.com and Yep.com](#7-translate---translation-by-duckduckgocom-and-
-yepcom) - [8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-
-suggestions---suggestions-by-duckduckgocom-and-yepcom) - [usage of webscout.AI]
-   (#usage-of-webscoutai) - [1. `PhindSearch` - Search using Phind.com](#1-
- phindsearch---search-using-phindcom) - [2. `YepChat` - Chat with mistral 8x7b
-powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat) -
-  [3. `You.com` - search with you.com](#3-youcom---search-with-youcom) - [4.
-`Gemini` - search with google gemini](#4-gemini---search-with-google-gemini) -
-  [usage of image generator from Webscout.AI](#usage-of-image-generator-from-
- webscoutai) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-
-  using-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
-  searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
- perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
-opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Sean` -
- chat With Sean](#10-sean---chat-with-sean) - [usage of special .LLM file from
-webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
-    - [`LLM`](#llm) - [`LLM` with internet](#llm-with-internet) ## Install
-   ```python pip install -U webscout ``` ## CLI version ```python3 python -
-m webscout --help ``` | Command | Description | |------------------------------
--------------|-----------------------------------------------------------------
---------------------------------------| | python -m webscout answers -k Text |
-    CLI function to perform an answers search using Webscout. | | python -
-  m webscout images -k Text | CLI function to perform an images search using
-Webscout. | | python -m webscout maps -k Text | CLI function to perform a maps
- search using Webscout. | | python -m webscout news -k Text | CLI function to
-  perform a news search using Webscout. | | python -m webscout suggestions -
-   k Text | CLI function to perform a suggestions search using Webscout. | |
- python -m webscout text -k Text | CLI function to perform a text search using
- Webscout. | | python -m webscout translate -k Text | CLI function to perform
-   translate using Webscout. | | python -m webscout version | A command-line
-   interface command that prints and returns the version of the program. | |
-  python -m webscout videos -k Text | CLI function to perform a videos search
-  using DuckDuckGo API. | ## CLI to use LLM ```python python -m webscout.LLM
- model_name ``` [Go To TOP](#TOP) ## Regions expand xa-ar for Arabia xa-en for
-Arabia (en) ar-es for Argentina au-en for Australia at-de for Austria be-fr for
- Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg for Bulgaria ca-en
- for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for Chile cn-zh for
- China co-es for Colombia hr-hr for Croatia cz-cs for Czech Republic dk-da for
-Denmark ee-et for Estonia fi-fi for Finland fr-fr for France de-de for Germany
- gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en for India id-id
-for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he for Israel it-it
-for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-lt for Lithuania
- xl-es for Latin America my-ms for Malaysia my-en for Malaysia (en) mx-es for
- Mexico nl-nl for Netherlands nz-en for New Zealand no-no for Norway pe-es for
- Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl for Poland pt-pt
- for Portugal ro-ro for Romania ru-ru for Russia sg-en for Singapore sk-sk for
-Slovak Republic sl-sl for Slovenia za-en for South Africa es-es for Spain se-sv
-  for Sweden ch-de for Switzerland (de) ch-fr for Switzerland (fr) ch-it for
- Switzerland (it) tw-tzh for Taiwan th-th for Thailand tr-tr for Turkey ua-uk
- for Ukraine uk-en for United Kingdom us-en for United States ue-es for United
- States (es) ve-es for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go
- To TOP](#TOP) ## Transcriber The transcriber function in webscout is a handy
-tool that transcribes YouTube videos. Here's an example code demonstrating its
-       usage: ```python import sys from webscout import transcriber def
-    extract_transcript(video_id): """Extracts the transcript from a YouTube
-  video.""" try: transcript_list = transcriber.list_transcripts(video_id) for
-transcript in transcript_list: transcript_data_list = transcript.fetch() lang =
+transcribe yt videos, have TTS support and now has webai(terminal gpt and open
+ interpeter) support ## Table of Contents - [webscout](#webscout) - [Table of
+   Contents](#table-of-contents) - [Install](#install) - [CLI version](#cli-
+     version) - [CLI to use LLM](#cli-to-use-llm) - [Regions](#regions) -
+  [Transcriber](#transcriber) - [DeepWEBS: Advanced Web Searches](#deepwebs-
+ advanced-web-searches) - [Activating DeepWEBS](#activating-deepwebs) - [Point
+to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
+   - [Usage Example](#usage-example) - [Text-to-Speech:](#text-to-speech) -
+[Available TTS Voices:](#available-tts-voices) - [ALL voices:](#all-voices) -
+   [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-classes) - [Exceptions]
+ (#exceptions) - [usage of webscout](#usage-of-webscout) - [1. `text()` - text
+ search by DuckDuckGo.com and Yep.com](#1-text---text-search-by-duckduckgocom-
+and-yepcom) - [2. `answers()` - instant answers by DuckDuckGo.com and Yep.com]
+ (#2-answers---instant-answers-by-duckduckgocom-and-yepcom) - [3. `images()` -
+   image search by DuckDuckGo.com and Yep.com](#3-images---image-search-by-
+ duckduckgocom-and-yepcom) - [4. `videos()` - video search by DuckDuckGo.com]
+  (#4-videos---video-search-by-duckduckgocom) - [5. `news()` - news search by
+DuckDuckGo.com and yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom)
+  - [6. `maps()` - map search by DuckDuckGo.com and](#6-maps---map-search-by-
+  duckduckgocom-and) - [7. `translate()` - translation by DuckDuckGo.com and
+    Yep.com](#7-translate---translation-by-duckduckgocom-and-yepcom) - [8.
+`suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-suggestions---
+ suggestions-by-duckduckgocom-and-yepcom) - [usage of webscout.AI](#usage-of-
+  webscoutai) - [1. `PhindSearch` - Search using Phind.com](#1-phindsearch---
+  search-using-phindcom) - [2. `YepChat` - Chat with mistral 8x7b powered by
+    yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat) - [3.
+`You.com` - search with you.com](#3-youcom---search-with-youcom) - [4. `Gemini`
+- search with google gemini](#4-gemini---search-with-google-gemini) - [usage of
+image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai) -
+[5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia) -
+  [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-
+blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-
+ with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-
+  opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Sean` - chat With Sean]
+   (#10-sean---chat-with-sean) - [usage of special .LLM file from webscout
+(webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm) - [`LLM`]
+ (#llm) - [`LLM` with internet](#llm-with-internet) - [`Webai` - terminal gpt
+  and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter) - [for
+  using as terminal gpt](#for-using-as-terminal-gpt) ## Install ```python pip
+install -U webscout ``` ## CLI version ```python3 python -m webscout --help ```
+| Command | Description | |-------------------------------------------|--------
+-------------------------------------------------------------------------------
+   ----------------| | python -m webscout answers -k Text | CLI function to
+perform an answers search using Webscout. | | python -m webscout images -k Text
+    | CLI function to perform an images search using Webscout. | | python -
+m webscout maps -k Text | CLI function to perform a maps search using Webscout.
+  | | python -m webscout news -k Text | CLI function to perform a news search
+ using Webscout. | | python -m webscout suggestions -k Text | CLI function to
+  perform a suggestions search using Webscout. | | python -m webscout text -
+  k Text | CLI function to perform a text search using Webscout. | | python -
+    m webscout translate -k Text | CLI function to perform translate using
+  Webscout. | | python -m webscout version | A command-line interface command
+  that prints and returns the version of the program. | | python -m webscout
+videos -k Text | CLI function to perform a videos search using DuckDuckGo API.
+| ## CLI to use LLM ```python python -m webscout.LLM model_name ``` [Go To TOP]
+   (#TOP) ## Regions expand xa-ar for Arabia xa-en for Arabia (en) ar-es for
+ Argentina au-en for Australia at-de for Austria be-fr for Belgium (fr) be-nl
+for Belgium (nl) br-pt for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for
+    Canada (fr) ct-ca for Catalan cl-es for Chile cn-zh for China co-es for
+Colombia hr-hr for Croatia cz-cs for Czech Republic dk-da for Denmark ee-et for
+ Estonia fi-fi for Finland fr-fr for France de-de for Germany gr-el for Greece
+hk-tzh for Hong Kong hu-hu for Hungary in-en for India id-id for Indonesia id-
+en for Indonesia (en) ie-en for Ireland il-he for Israel it-it for Italy jp-jp
+for Japan kr-kr for Korea lv-lv for Latvia lt-lt for Lithuania xl-es for Latin
+ America my-ms for Malaysia my-en for Malaysia (en) mx-es for Mexico nl-nl for
+  Netherlands nz-en for New Zealand no-no for Norway pe-es for Peru ph-en for
+Philippines ph-tl for Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-
+ ro for Romania ru-ru for Russia sg-en for Singapore sk-sk for Slovak Republic
+sl-sl for Slovenia za-en for South Africa es-es for Spain se-sv for Sweden ch-
+ de for Switzerland (de) ch-fr for Switzerland (fr) ch-it for Switzerland (it)
+ tw-tzh for Taiwan th-th for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en
+ for United Kingdom us-en for United States ue-es for United States (es) ve-es
+ for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ##
+     Transcriber The transcriber function in webscout is a handy tool that
+  transcribes YouTube videos. Here's an example code demonstrating its usage:
+ ```python import sys from webscout import transcriber def extract_transcript
+     (video_id): """Extracts the transcript from a YouTube video.""" try:
+  transcript_list = transcriber.list_transcripts(video_id) for transcript in
+       transcript_list: transcript_data_list = transcript.fetch() lang =
  transcript.language transcript_text = "" if transcript.language_code == 'en':
     for line in transcript_data_list: start_time = line['start'] end_time =
      start_time + line['duration'] formatted_line = f"{start_time:.2f} -
   {end_time:.2f}: {line['text']}\n" transcript_text += formatted_line return
   transcript_text elif transcript.is_translatable: english_transcript_list =
     transcript.translate('en').fetch() for line in english_transcript_list:
       start_time = line['start'] end_time = start_time + line['duration']
@@ -346,8 +349,21 @@
    messages to be sent, including the user input, search results, and system
 message messages = [ {"role": "user", "content": user_input + "\n" + "websearch
 results are:" + "\n".join(search_results)}, ] # Use the chat method to get the
      response response = LLM.chat(messages) return response if __name__ ==
   "__main__": while True: # Get the user input user_input = input("User: ") #
  Perform a web search based on the user input with WEBS() as webs: response =
 chat(user_input, webs) # Print the response if response: print("AI:", response)
-                        else: print("No response") ```
+else: print("No response") ``` ## `Webai` - terminal gpt and a open interpeter
+ ```python from webscout.webai import Main def use_rawdog_with_webai(prompt):
+    """ Wrap the webscout default method in a try-except block to catch any
+  unhandled exceptions and print a helpful message. """ try: webai_bot = Main
+  ( max_tokens=500, provider="phind", temperature=0.7, top_k=40, top_p=0.95,
+  model="Phind Model", # Replace with your desired model auth=None, # Replace
+  with your auth key/value (if needed) timeout=30, disable_conversation=True,
+filepath=None, update_file=True, intro=None, rawdog=True, history_offset=10250,
+      awesome_prompt=None, proxy_path=None, quiet=True ) webai_response =
+webai_bot.default(prompt) except Exception as e: print("Unexpected error:", e)
+     if __name__ == "__main__": user_prompt = input("Enter your prompt: ")
+use_rawdog_with_webai(user_prompt) ``` ```shell python -m webscout.webai webai
+--provider "phind" --rawdog ``` ### for using as terminal gpt ```python python
+                 -m webscout.webai webai --provider "sean" ```
```

### Comparing `webscout-1.3.3/webscout.egg-info/SOURCES.txt` & `webscout-1.3.4/webscout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

