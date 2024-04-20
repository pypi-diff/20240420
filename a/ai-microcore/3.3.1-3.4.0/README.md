# Comparing `tmp/ai_microcore-3.3.1.tar.gz` & `tmp/ai_microcore-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_microcore-3.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ai_microcore-3.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ai_microcore-3.3.1.tar` & `ai_microcore-3.4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rwxr-xr-x   0        0        0     1091 2023-11-04 16:00:47.197704 ai_microcore-3.3.1/LICENSE
--rwxr-xr-x   0        0        0    11116 2024-04-04 12:54:33.488412 ai_microcore-3.3.1/README.md
--rwxr-xr-x   0        0        0     3887 2024-04-18 17:28:28.764089 ai_microcore-3.3.1/microcore/__init__.py
--rwxr-xr-x   0        0        0     6065 2024-04-18 16:11:44.822923 ai_microcore-3.3.1/microcore/_env.py
--rwxr-xr-x   0        0        0     3311 2024-04-18 13:13:30.363208 ai_microcore-3.3.1/microcore/_llm_functions.py
--rwxr-xr-x   0        0        0      786 2024-04-18 17:18:22.638592 ai_microcore-3.3.1/microcore/_prepare_llm_args.py
--rwxr-xr-x   0        0        0     2319 2024-03-08 00:49:48.900573 ai_microcore-3.3.1/microcore/ai_func/__init__.py
--rwxr-xr-x   0        0        0      314 2023-11-04 16:00:47.368478 ai_microcore-3.3.1/microcore/ai_func/python_ai_func.j2
--rwxr-xr-x   0        0        0      576 2023-11-04 19:26:33.244252 ai_microcore-3.3.1/microcore/ai_modules.py
--rwxr-xr-x   0        0        0    11541 2024-04-18 16:30:03.398309 ai_microcore-3.3.1/microcore/configuration.py
--rwxr-xr-x   0        0        0     3133 2024-02-15 20:01:36.859722 ai_microcore-3.3.1/microcore/embedding_db/__init__.py
--rwxr-xr-x   0        0        0     4565 2024-02-15 19:46:15.503154 ai_microcore-3.3.1/microcore/embedding_db/chromadb.py
--rwxr-xr-x   0        0        0     8369 2024-03-08 00:49:49.038994 ai_microcore-3.3.1/microcore/file_storage.py
--rwxr-xr-x   0        0        0     4725 2024-04-18 17:18:22.711937 ai_microcore-3.3.1/microcore/json_parsing.py
--rwxr-xr-x   0        0        0       16 2023-11-06 23:41:28.213361 ai_microcore-3.3.1/microcore/llm/__init__.py
--rwxr-xr-x   0        0        0     4708 2024-04-16 08:56:56.272317 ai_microcore-3.3.1/microcore/llm/_openai_llm_v0.py
--rwxr-xr-x   0        0        0     5120 2024-04-18 17:18:22.746984 ai_microcore-3.3.1/microcore/llm/_openai_llm_v1.py
--rwxr-xr-x   0        0        0     3655 2024-04-16 13:59:52.503374 ai_microcore-3.3.1/microcore/llm/anthropic.py
--rwxr-xr-x   0        0        0     4479 2024-04-16 09:04:29.151454 ai_microcore-3.3.1/microcore/llm/google_genai.py
--rwxr-xr-x   0        0        0     5801 2024-04-18 13:00:32.311278 ai_microcore-3.3.1/microcore/llm/google_vertex_ai.py
--rwxr-xr-x   0        0        0     3229 2024-04-16 14:08:39.822867 ai_microcore-3.3.1/microcore/llm/local_llm.py
--rwxr-xr-x   0        0        0     3052 2024-04-18 13:05:21.887990 ai_microcore-3.3.1/microcore/llm/local_transformers.py
--rwxr-xr-x   0        0        0      272 2023-11-06 23:49:42.323932 ai_microcore-3.3.1/microcore/llm/openai_llm.py
--rwxr-xr-x   0        0        0     2466 2024-04-16 08:13:17.036046 ai_microcore-3.3.1/microcore/logging.py
--rwxr-xr-x   0        0        0      642 2024-03-08 00:49:48.881046 ai_microcore-3.3.1/microcore/message_types.py
--rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.559200 ai_microcore-3.3.1/microcore/templating/__init__.py
--rwxr-xr-x   0        0        0      525 2023-11-12 15:43:10.028753 ai_microcore-3.3.1/microcore/templating/jinja2.py
--rwxr-xr-x   0        0        0     1455 2024-03-31 01:09:15.566074 ai_microcore-3.3.1/microcore/text2speech/elevenlabs.py
--rwxr-xr-x   0        0        0     1046 2024-03-11 12:20:49.086082 ai_microcore-3.3.1/microcore/types.py
--rwxr-xr-x   0        0        0     1535 2024-03-31 01:09:15.567119 ai_microcore-3.3.1/microcore/ui.py
--rwxr-xr-x   0        0        0     8767 2024-04-18 17:18:22.797985 ai_microcore-3.3.1/microcore/utils.py
--rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.618937 ai_microcore-3.3.1/microcore/wrappers/__init__.py
--rwxr-xr-x   0        0        0     1559 2024-04-18 13:05:21.831255 ai_microcore-3.3.1/microcore/wrappers/llm_response_wrapper.py
--rwxr-xr-x   0        0        0      480 2024-04-02 14:01:24.033112 ai_microcore-3.3.1/microcore/wrappers/prompt_wrapper.py
--rwxr-xr-x   0        0        0     1450 2024-04-18 14:27:33.934530 ai_microcore-3.3.1/pyproject.toml
--rw-r--r--   0        0        0    11811 1970-01-01 00:00:00.000000 ai_microcore-3.3.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1091 2023-11-04 16:00:47.197704 ai_microcore-3.4.0/LICENSE
+-rwxr-xr-x   0        0        0    11116 2024-04-04 12:54:33.488412 ai_microcore-3.4.0/README.md
+-rwxr-xr-x   0        0        0     3887 2024-04-20 14:21:46.683015 ai_microcore-3.4.0/microcore/__init__.py
+-rwxr-xr-x   0        0        0     6544 2024-04-20 12:26:13.641652 ai_microcore-3.4.0/microcore/_env.py
+-rwxr-xr-x   0        0        0     3311 2024-04-18 13:13:30.363208 ai_microcore-3.4.0/microcore/_llm_functions.py
+-rwxr-xr-x   0        0        0      786 2024-04-20 12:35:24.174582 ai_microcore-3.4.0/microcore/_prepare_llm_args.py
+-rwxr-xr-x   0        0        0     2319 2024-03-08 00:49:48.900573 ai_microcore-3.4.0/microcore/ai_func/__init__.py
+-rwxr-xr-x   0        0        0      314 2023-11-04 16:00:47.368478 ai_microcore-3.4.0/microcore/ai_func/python_ai_func.j2
+-rwxr-xr-x   0        0        0      576 2023-11-04 19:26:33.244252 ai_microcore-3.4.0/microcore/ai_modules.py
+-rwxr-xr-x   0        0        0    11541 2024-04-18 16:30:03.398309 ai_microcore-3.4.0/microcore/configuration.py
+-rwxr-xr-x   0        0        0     3133 2024-02-15 20:01:36.859722 ai_microcore-3.4.0/microcore/embedding_db/__init__.py
+-rwxr-xr-x   0        0        0     4565 2024-02-15 19:46:15.503154 ai_microcore-3.4.0/microcore/embedding_db/chromadb.py
+-rwxr-xr-x   0        0        0     8369 2024-03-08 00:49:49.038994 ai_microcore-3.4.0/microcore/file_storage.py
+-rwxr-xr-x   0        0        0     4725 2024-04-20 12:35:24.223611 ai_microcore-3.4.0/microcore/json_parsing.py
+-rwxr-xr-x   0        0        0       16 2023-11-06 23:41:28.213361 ai_microcore-3.4.0/microcore/llm/__init__.py
+-rwxr-xr-x   0        0        0     4708 2024-04-16 08:56:56.272317 ai_microcore-3.4.0/microcore/llm/_openai_llm_v0.py
+-rwxr-xr-x   0        0        0     5120 2024-04-18 17:18:22.746984 ai_microcore-3.4.0/microcore/llm/_openai_llm_v1.py
+-rwxr-xr-x   0        0        0     3655 2024-04-16 13:59:52.503374 ai_microcore-3.4.0/microcore/llm/anthropic.py
+-rwxr-xr-x   0        0        0     4479 2024-04-16 09:04:29.151454 ai_microcore-3.4.0/microcore/llm/google_genai.py
+-rwxr-xr-x   0        0        0     5801 2024-04-18 13:00:32.311278 ai_microcore-3.4.0/microcore/llm/google_vertex_ai.py
+-rwxr-xr-x   0        0        0     3229 2024-04-16 14:08:39.822867 ai_microcore-3.4.0/microcore/llm/local_llm.py
+-rwxr-xr-x   0        0        0     4812 2024-04-20 14:21:18.005758 ai_microcore-3.4.0/microcore/llm/local_transformers.py
+-rwxr-xr-x   0        0        0      272 2023-11-06 23:49:42.323932 ai_microcore-3.4.0/microcore/llm/openai_llm.py
+-rwxr-xr-x   0        0        0     2466 2024-04-16 08:13:17.036046 ai_microcore-3.4.0/microcore/logging.py
+-rwxr-xr-x   0        0        0      642 2024-03-08 00:49:48.881046 ai_microcore-3.4.0/microcore/message_types.py
+-rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.559200 ai_microcore-3.4.0/microcore/templating/__init__.py
+-rwxr-xr-x   0        0        0      525 2023-11-12 15:43:10.028753 ai_microcore-3.4.0/microcore/templating/jinja2.py
+-rwxr-xr-x   0        0        0     1455 2024-03-31 01:09:15.566074 ai_microcore-3.4.0/microcore/text2speech/elevenlabs.py
+-rwxr-xr-x   0        0        0     1046 2024-03-11 12:20:49.086082 ai_microcore-3.4.0/microcore/types.py
+-rwxr-xr-x   0        0        0     1601 2024-04-19 09:12:25.103139 ai_microcore-3.4.0/microcore/ui.py
+-rwxr-xr-x   0        0        0     8767 2024-04-18 17:18:22.797985 ai_microcore-3.4.0/microcore/utils.py
+-rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.618937 ai_microcore-3.4.0/microcore/wrappers/__init__.py
+-rwxr-xr-x   0        0        0     1559 2024-04-18 13:05:21.831255 ai_microcore-3.4.0/microcore/wrappers/llm_response_wrapper.py
+-rwxr-xr-x   0        0        0      480 2024-04-02 14:01:24.033112 ai_microcore-3.4.0/microcore/wrappers/prompt_wrapper.py
+-rwxr-xr-x   0        0        0     1450 2024-04-18 14:27:33.934530 ai_microcore-3.4.0/pyproject.toml
+-rw-r--r--   0        0        0    11811 1970-01-01 00:00:00.000000 ai_microcore-3.4.0/PKG-INFO
```

### Comparing `ai_microcore-3.3.1/LICENSE` & `ai_microcore-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/README.md` & `ai_microcore-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/__init__.py` & `ai_microcore-3.4.0/microcore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,8 +132,8 @@
     "configuration",
     "Config",
     "types",
     "ui",
     # "wrappers",
 ]
 
-__version__ = "3.3.1"
+__version__ = "3.4.0"
```

### Comparing `ai_microcore-3.3.1/microcore/_env.py` & `ai_microcore-3.4.0/microcore/_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass, field, asdict
 from importlib.util import find_spec
 import jinja2
 
-from .configuration import Config, ApiType
+from .configuration import Config, ApiType, LLMConfigError
 from . import AbstractEmbeddingDB
 from .types import TplFunctionType, LLMAsyncFunctionType, LLMFunctionType
 from .templating.jinja2 import make_jinja2_env, make_tpl_function
 from .llm.openai_llm import make_llm_functions as make_openai_llm_functions
 from .llm.local_llm import make_llm_functions as make_local_llm_functions
 
 
@@ -33,15 +33,28 @@
         self.init_similarity_search()
 
     def init_templating(self):
         self.jinja_env = make_jinja2_env(self)
         self.tpl_function = make_tpl_function(self)
 
     def init_llm(self):
-        if self.config.LLM_API_TYPE == ApiType.FUNCTION:
+        if self.config.LLM_API_TYPE == ApiType.NONE:
+
+            def not_configured(*args, **kwargs):
+                raise LLMConfigError("Language model is not configured")
+
+            async def a_not_configured(*args, **kwargs):
+                raise LLMConfigError("Language model is not configured")
+
+            self.llm_function, self.llm_async_function = (
+                not_configured,
+                a_not_configured,
+            )
+
+        elif self.config.LLM_API_TYPE == ApiType.FUNCTION:
             self.llm_function, self.llm_async_function = make_local_llm_functions(
                 self.config
             )
         elif self.config.LLM_API_TYPE == ApiType.TRANSFORMERS:
             try:
                 from .llm.local_transformers import (
                     make_llm_functions as make_transformers_llm_functions,
```

### Comparing `ai_microcore-3.3.1/microcore/_llm_functions.py` & `ai_microcore-3.4.0/microcore/_llm_functions.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/_prepare_llm_args.py` & `ai_microcore-3.4.0/microcore/_prepare_llm_args.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/ai_func/__init__.py` & `ai_microcore-3.4.0/microcore/ai_func/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/ai_modules.py` & `ai_microcore-3.4.0/microcore/ai_modules.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/configuration.py` & `ai_microcore-3.4.0/microcore/configuration.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/embedding_db/__init__.py` & `ai_microcore-3.4.0/microcore/embedding_db/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/embedding_db/chromadb.py` & `ai_microcore-3.4.0/microcore/embedding_db/chromadb.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/file_storage.py` & `ai_microcore-3.4.0/microcore/file_storage.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/json_parsing.py` & `ai_microcore-3.4.0/microcore/json_parsing.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/llm/_openai_llm_v0.py` & `ai_microcore-3.4.0/microcore/llm/_openai_llm_v0.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/llm/_openai_llm_v1.py` & `ai_microcore-3.4.0/microcore/llm/_openai_llm_v1.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/llm/anthropic.py` & `ai_microcore-3.4.0/microcore/llm/anthropic.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/llm/google_genai.py` & `ai_microcore-3.4.0/microcore/llm/google_genai.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/llm/google_vertex_ai.py` & `ai_microcore-3.4.0/microcore/llm/google_vertex_ai.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/llm/local_llm.py` & `ai_microcore-3.4.0/microcore/llm/local_llm.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/logging.py` & `ai_microcore-3.4.0/microcore/logging.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/message_types.py` & `ai_microcore-3.4.0/microcore/message_types.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/templating/jinja2.py` & `ai_microcore-3.4.0/microcore/templating/jinja2.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/text2speech/elevenlabs.py` & `ai_microcore-3.4.0/microcore/text2speech/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/types.py` & `ai_microcore-3.4.0/microcore/types.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/ui.py` & `ai_microcore-3.4.0/microcore/ui.py`

 * *Files 20% similar despite different names*

```diff
@@ -68,7 +68,11 @@
 
 def white(msg):
     return f"{Fore.WHITE}{msg}{Fore.RESET}"
 
 
 def gray(msg):
     return f"\033[90m{msg}{Fore.RESET}"
+
+
+def black(msg):
+    return f"{Fore.BLACK}{msg}{Fore.RESET}"
```

### Comparing `ai_microcore-3.3.1/microcore/utils.py` & `ai_microcore-3.4.0/microcore/utils.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/microcore/wrappers/llm_response_wrapper.py` & `ai_microcore-3.4.0/microcore/wrappers/llm_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/pyproject.toml` & `ai_microcore-3.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.3.1/PKG-INFO` & `ai_microcore-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-microcore
-Version: 3.3.1
+Version: 3.4.0
 Summary: # Minimalistic Foundation for AI Applications
 Keywords: llm,large language models,ai,similarity search,ai search,gpt,openai
 Author-email: Vitalii Stepanenko <mail@vitalii.in>
 Maintainer-email: Vitalii Stepanenko <mail@vitalii.in>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ai-microcore Version: 3.3.1 Summary: # Minimalistic
+Metadata-Version: 2.1 Name: ai-microcore Version: 3.4.0 Summary: # Minimalistic
 Foundation for AI Applications Keywords: llm,large language
 models,ai,similarity search,ai search,gpt,openai Author-email: Vitalii
 Stepanenko
 vitalii.in> Maintainer-email: Vitalii Stepanenko
 vitalii.in> Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
```

