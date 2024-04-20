# Comparing `tmp/ai_microcore-3.4.0.tar.gz` & `tmp/ai_microcore-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_microcore-3.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ai_microcore-3.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ai_microcore-3.4.0.tar` & `ai_microcore-3.5.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rwxr-xr-x   0        0        0     1091 2023-11-04 16:00:47.197704 ai_microcore-3.4.0/LICENSE
--rwxr-xr-x   0        0        0    11116 2024-04-04 12:54:33.488412 ai_microcore-3.4.0/README.md
--rwxr-xr-x   0        0        0     3887 2024-04-20 14:21:46.683015 ai_microcore-3.4.0/microcore/__init__.py
--rwxr-xr-x   0        0        0     6544 2024-04-20 12:26:13.641652 ai_microcore-3.4.0/microcore/_env.py
--rwxr-xr-x   0        0        0     3311 2024-04-18 13:13:30.363208 ai_microcore-3.4.0/microcore/_llm_functions.py
--rwxr-xr-x   0        0        0      786 2024-04-20 12:35:24.174582 ai_microcore-3.4.0/microcore/_prepare_llm_args.py
--rwxr-xr-x   0        0        0     2319 2024-03-08 00:49:48.900573 ai_microcore-3.4.0/microcore/ai_func/__init__.py
--rwxr-xr-x   0        0        0      314 2023-11-04 16:00:47.368478 ai_microcore-3.4.0/microcore/ai_func/python_ai_func.j2
--rwxr-xr-x   0        0        0      576 2023-11-04 19:26:33.244252 ai_microcore-3.4.0/microcore/ai_modules.py
--rwxr-xr-x   0        0        0    11541 2024-04-18 16:30:03.398309 ai_microcore-3.4.0/microcore/configuration.py
--rwxr-xr-x   0        0        0     3133 2024-02-15 20:01:36.859722 ai_microcore-3.4.0/microcore/embedding_db/__init__.py
--rwxr-xr-x   0        0        0     4565 2024-02-15 19:46:15.503154 ai_microcore-3.4.0/microcore/embedding_db/chromadb.py
--rwxr-xr-x   0        0        0     8369 2024-03-08 00:49:49.038994 ai_microcore-3.4.0/microcore/file_storage.py
--rwxr-xr-x   0        0        0     4725 2024-04-20 12:35:24.223611 ai_microcore-3.4.0/microcore/json_parsing.py
--rwxr-xr-x   0        0        0       16 2023-11-06 23:41:28.213361 ai_microcore-3.4.0/microcore/llm/__init__.py
--rwxr-xr-x   0        0        0     4708 2024-04-16 08:56:56.272317 ai_microcore-3.4.0/microcore/llm/_openai_llm_v0.py
--rwxr-xr-x   0        0        0     5120 2024-04-18 17:18:22.746984 ai_microcore-3.4.0/microcore/llm/_openai_llm_v1.py
--rwxr-xr-x   0        0        0     3655 2024-04-16 13:59:52.503374 ai_microcore-3.4.0/microcore/llm/anthropic.py
--rwxr-xr-x   0        0        0     4479 2024-04-16 09:04:29.151454 ai_microcore-3.4.0/microcore/llm/google_genai.py
--rwxr-xr-x   0        0        0     5801 2024-04-18 13:00:32.311278 ai_microcore-3.4.0/microcore/llm/google_vertex_ai.py
--rwxr-xr-x   0        0        0     3229 2024-04-16 14:08:39.822867 ai_microcore-3.4.0/microcore/llm/local_llm.py
--rwxr-xr-x   0        0        0     4812 2024-04-20 14:21:18.005758 ai_microcore-3.4.0/microcore/llm/local_transformers.py
--rwxr-xr-x   0        0        0      272 2023-11-06 23:49:42.323932 ai_microcore-3.4.0/microcore/llm/openai_llm.py
--rwxr-xr-x   0        0        0     2466 2024-04-16 08:13:17.036046 ai_microcore-3.4.0/microcore/logging.py
--rwxr-xr-x   0        0        0      642 2024-03-08 00:49:48.881046 ai_microcore-3.4.0/microcore/message_types.py
--rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.559200 ai_microcore-3.4.0/microcore/templating/__init__.py
--rwxr-xr-x   0        0        0      525 2023-11-12 15:43:10.028753 ai_microcore-3.4.0/microcore/templating/jinja2.py
--rwxr-xr-x   0        0        0     1455 2024-03-31 01:09:15.566074 ai_microcore-3.4.0/microcore/text2speech/elevenlabs.py
--rwxr-xr-x   0        0        0     1046 2024-03-11 12:20:49.086082 ai_microcore-3.4.0/microcore/types.py
--rwxr-xr-x   0        0        0     1601 2024-04-19 09:12:25.103139 ai_microcore-3.4.0/microcore/ui.py
--rwxr-xr-x   0        0        0     8767 2024-04-18 17:18:22.797985 ai_microcore-3.4.0/microcore/utils.py
--rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.618937 ai_microcore-3.4.0/microcore/wrappers/__init__.py
--rwxr-xr-x   0        0        0     1559 2024-04-18 13:05:21.831255 ai_microcore-3.4.0/microcore/wrappers/llm_response_wrapper.py
--rwxr-xr-x   0        0        0      480 2024-04-02 14:01:24.033112 ai_microcore-3.4.0/microcore/wrappers/prompt_wrapper.py
--rwxr-xr-x   0        0        0     1450 2024-04-18 14:27:33.934530 ai_microcore-3.4.0/pyproject.toml
--rw-r--r--   0        0        0    11811 1970-01-01 00:00:00.000000 ai_microcore-3.4.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1091 2023-11-04 16:00:47.197704 ai_microcore-3.5.0/LICENSE
+-rwxr-xr-x   0        0        0    11116 2024-04-04 12:54:33.488412 ai_microcore-3.5.0/README.md
+-rwxr-xr-x   0        0        0     3922 2024-04-20 15:03:54.996749 ai_microcore-3.5.0/microcore/__init__.py
+-rwxr-xr-x   0        0        0     6544 2024-04-20 12:26:13.641652 ai_microcore-3.5.0/microcore/_env.py
+-rwxr-xr-x   0        0        0     3790 2024-04-20 15:07:06.612137 ai_microcore-3.5.0/microcore/_llm_functions.py
+-rwxr-xr-x   0        0        0      786 2024-04-20 12:35:24.174582 ai_microcore-3.5.0/microcore/_prepare_llm_args.py
+-rwxr-xr-x   0        0        0     2319 2024-03-08 00:49:48.900573 ai_microcore-3.5.0/microcore/ai_func/__init__.py
+-rwxr-xr-x   0        0        0      314 2023-11-04 16:00:47.368478 ai_microcore-3.5.0/microcore/ai_func/python_ai_func.j2
+-rwxr-xr-x   0        0        0      576 2023-11-04 19:26:33.244252 ai_microcore-3.5.0/microcore/ai_modules.py
+-rwxr-xr-x   0        0        0    11591 2024-04-20 14:59:40.736447 ai_microcore-3.5.0/microcore/configuration.py
+-rwxr-xr-x   0        0        0     3133 2024-02-15 20:01:36.859722 ai_microcore-3.5.0/microcore/embedding_db/__init__.py
+-rwxr-xr-x   0        0        0     4565 2024-02-15 19:46:15.503154 ai_microcore-3.5.0/microcore/embedding_db/chromadb.py
+-rwxr-xr-x   0        0        0     8369 2024-03-08 00:49:49.038994 ai_microcore-3.5.0/microcore/file_storage.py
+-rwxr-xr-x   0        0        0     4725 2024-04-20 12:35:24.223611 ai_microcore-3.5.0/microcore/json_parsing.py
+-rwxr-xr-x   0        0        0       16 2023-11-06 23:41:28.213361 ai_microcore-3.5.0/microcore/llm/__init__.py
+-rwxr-xr-x   0        0        0     4708 2024-04-16 08:56:56.272317 ai_microcore-3.5.0/microcore/llm/_openai_llm_v0.py
+-rwxr-xr-x   0        0        0     5120 2024-04-18 17:18:22.746984 ai_microcore-3.5.0/microcore/llm/_openai_llm_v1.py
+-rwxr-xr-x   0        0        0     3655 2024-04-16 13:59:52.503374 ai_microcore-3.5.0/microcore/llm/anthropic.py
+-rwxr-xr-x   0        0        0     4479 2024-04-16 09:04:29.151454 ai_microcore-3.5.0/microcore/llm/google_genai.py
+-rwxr-xr-x   0        0        0     5801 2024-04-18 13:00:32.311278 ai_microcore-3.5.0/microcore/llm/google_vertex_ai.py
+-rwxr-xr-x   0        0        0     3229 2024-04-16 14:08:39.822867 ai_microcore-3.5.0/microcore/llm/local_llm.py
+-rwxr-xr-x   0        0        0     4812 2024-04-20 14:21:18.005758 ai_microcore-3.5.0/microcore/llm/local_transformers.py
+-rwxr-xr-x   0        0        0      272 2023-11-06 23:49:42.323932 ai_microcore-3.5.0/microcore/llm/openai_llm.py
+-rwxr-xr-x   0        0        0     2466 2024-04-16 08:13:17.036046 ai_microcore-3.5.0/microcore/logging.py
+-rwxr-xr-x   0        0        0      642 2024-03-08 00:49:48.881046 ai_microcore-3.5.0/microcore/message_types.py
+-rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.559200 ai_microcore-3.5.0/microcore/templating/__init__.py
+-rwxr-xr-x   0        0        0      525 2023-11-12 15:43:10.028753 ai_microcore-3.5.0/microcore/templating/jinja2.py
+-rwxr-xr-x   0        0        0     1455 2024-03-31 01:09:15.566074 ai_microcore-3.5.0/microcore/text2speech/elevenlabs.py
+-rwxr-xr-x   0        0        0     1046 2024-03-11 12:20:49.086082 ai_microcore-3.5.0/microcore/types.py
+-rwxr-xr-x   0        0        0     1601 2024-04-19 09:12:25.103139 ai_microcore-3.5.0/microcore/ui.py
+-rwxr-xr-x   0        0        0     9072 2024-04-20 14:50:05.806382 ai_microcore-3.5.0/microcore/utils.py
+-rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.618937 ai_microcore-3.5.0/microcore/wrappers/__init__.py
+-rwxr-xr-x   0        0        0     1559 2024-04-18 13:05:21.831255 ai_microcore-3.5.0/microcore/wrappers/llm_response_wrapper.py
+-rwxr-xr-x   0        0        0      480 2024-04-02 14:01:24.033112 ai_microcore-3.5.0/microcore/wrappers/prompt_wrapper.py
+-rwxr-xr-x   0        0        0     1450 2024-04-18 14:27:33.934530 ai_microcore-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0    11811 1970-01-01 00:00:00.000000 ai_microcore-3.5.0/PKG-INFO
```

### Comparing `ai_microcore-3.4.0/LICENSE` & `ai_microcore-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/README.md` & `ai_microcore-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/__init__.py` & `ai_microcore-3.5.0/microcore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from ._env import configure, env, config
 from .logging import use_logging
 from .message_types import UserMsg, AssistantMsg, SysMsg, Msg
 from .configuration import ApiType, LLMConfigError, Config
 from .types import BadAIJsonAnswer, BadAIAnswer
 from .wrappers.prompt_wrapper import PromptWrapper
 from .wrappers.llm_response_wrapper import LLMResponse
-from ._llm_functions import llm, allm
+from ._llm_functions import llm, allm, llm_parallel
 from .utils import parse, dedent
 
 
 def tpl(file: os.PathLike[str] | str, **kwargs) -> str | PromptWrapper:
     """Renders a prompt template using the provided parameters."""
     return PromptWrapper(env().tpl_function(file, **kwargs))
 
@@ -97,14 +97,15 @@
 
 texts = _EmbeddingDBProxy()
 """Embedding database, see `microcore.embedding_db.AbstractEmbeddingDB`"""
 
 __all__ = [
     "llm",
     "allm",
+    "llm_parallel",
     "tpl",
     "prompt",
     "fmt",
     "texts",
     "configure",
     "validate_config",
     "storage",
@@ -132,8 +133,8 @@
     "configuration",
     "Config",
     "types",
     "ui",
     # "wrappers",
 ]
 
-__version__ = "3.4.0"
+__version__ = "3.5.0"
```

### Comparing `ai_microcore-3.4.0/microcore/_env.py` & `ai_microcore-3.5.0/microcore/_env.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/_llm_functions.py` & `ai_microcore-3.5.0/microcore/_llm_functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime
 
 from .message_types import Msg
+from .utils import run_parallel
 from .wrappers.llm_response_wrapper import LLMResponse
 from ._env import env
 
 
 def llm(prompt: str | Msg | list[str] | list[Msg], **kwargs) -> str | LLMResponse:
     """
     Request Large Language Model synchronously
@@ -89,7 +90,20 @@
     response = await env().llm_async_function(prompt, **kwargs)
     try:
         response.gen_duration = (datetime.now() - start).total_seconds()
     except AttributeError:
         ...
     [h(response) for h in env().llm_after_handlers]
     return response
+
+
+async def llm_parallel(
+    prompts: list, max_concurrent_tasks: int = None, **kwargs
+) -> list[str] | list[LLMResponse]:
+    tasks = [allm(prompt, **kwargs) for prompt in prompts]
+
+    if max_concurrent_tasks is None:
+        max_concurrent_tasks = int(env().config.MAX_CONCURRENT_TASKS)
+    if not max_concurrent_tasks:
+        max_concurrent_tasks = len(tasks)
+
+    return await run_parallel(tasks, max_concurrent_tasks=max_concurrent_tasks)
```

### Comparing `ai_microcore-3.4.0/microcore/_prepare_llm_args.py` & `ai_microcore-3.5.0/microcore/_prepare_llm_args.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/ai_func/__init__.py` & `ai_microcore-3.5.0/microcore/ai_func/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/ai_modules.py` & `ai_microcore-3.5.0/microcore/ai_modules.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/configuration.py` & `ai_microcore-3.5.0/microcore/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,13 +307,15 @@
     JINJA2_AUTO_ESCAPE: bool = None
 
     ELEVENLABS_API_KEY: str = from_env()
 
     TEXT_TO_SPEECH_PATH: str | Path = from_env()
     """Path to the folder with generated voice files"""
 
+    MAX_CONCURRENT_TASKS: int = from_env(None)
+
     def __post_init__(self):
         if self.JINJA2_AUTO_ESCAPE is None:
             self.JINJA2_AUTO_ESCAPE = get_bool_from_env("JINJA2_AUTO_ESCAPE", False)
         super().__post_init__()
         if self.TEXT_TO_SPEECH_PATH is None:
             self.TEXT_TO_SPEECH_PATH = Path(self.STORAGE_PATH) / "voicing"
```

### Comparing `ai_microcore-3.4.0/microcore/embedding_db/__init__.py` & `ai_microcore-3.5.0/microcore/embedding_db/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/embedding_db/chromadb.py` & `ai_microcore-3.5.0/microcore/embedding_db/chromadb.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/file_storage.py` & `ai_microcore-3.5.0/microcore/file_storage.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/json_parsing.py` & `ai_microcore-3.5.0/microcore/json_parsing.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/llm/_openai_llm_v0.py` & `ai_microcore-3.5.0/microcore/llm/_openai_llm_v0.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/llm/_openai_llm_v1.py` & `ai_microcore-3.5.0/microcore/llm/_openai_llm_v1.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/llm/anthropic.py` & `ai_microcore-3.5.0/microcore/llm/anthropic.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/llm/google_genai.py` & `ai_microcore-3.5.0/microcore/llm/google_genai.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/llm/google_vertex_ai.py` & `ai_microcore-3.5.0/microcore/llm/google_vertex_ai.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/llm/local_llm.py` & `ai_microcore-3.5.0/microcore/llm/local_llm.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/llm/local_transformers.py` & `ai_microcore-3.5.0/microcore/llm/local_transformers.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/logging.py` & `ai_microcore-3.5.0/microcore/logging.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/message_types.py` & `ai_microcore-3.5.0/microcore/message_types.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/templating/jinja2.py` & `ai_microcore-3.5.0/microcore/templating/jinja2.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/text2speech/elevenlabs.py` & `ai_microcore-3.5.0/microcore/text2speech/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/types.py` & `ai_microcore-3.5.0/microcore/types.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/ui.py` & `ai_microcore-3.5.0/microcore/ui.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/microcore/utils.py` & `ai_microcore-3.5.0/microcore/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import builtins
 import dataclasses
 import inspect
 import json
 import os
 import sys
 import re
@@ -272,7 +273,17 @@
         dedented_lines = [
             line[min_indent:] if line and len(line) >= min_indent else line
             for line in lines
         ]
     else:
         dedented_lines = lines
     return "\n".join(dedented_lines)
+
+
+async def run_parallel(tasks: list, max_concurrent_tasks: int):
+    semaphore = asyncio.Semaphore(max_concurrent_tasks)
+
+    async def worker(task):
+        async with semaphore:
+            return await task
+
+    return await asyncio.gather(*[worker(task) for task in tasks])
```

### Comparing `ai_microcore-3.4.0/microcore/wrappers/llm_response_wrapper.py` & `ai_microcore-3.5.0/microcore/wrappers/llm_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/pyproject.toml` & `ai_microcore-3.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.4.0/PKG-INFO` & `ai_microcore-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-microcore
-Version: 3.4.0
+Version: 3.5.0
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
-Metadata-Version: 2.1 Name: ai-microcore Version: 3.4.0 Summary: # Minimalistic
+Metadata-Version: 2.1 Name: ai-microcore Version: 3.5.0 Summary: # Minimalistic
 Foundation for AI Applications Keywords: llm,large language
 models,ai,similarity search,ai search,gpt,openai Author-email: Vitalii
 Stepanenko
 vitalii.in> Maintainer-email: Vitalii Stepanenko
 vitalii.in> Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
```

