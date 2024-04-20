# Comparing `tmp/llama_index_llms_fireworks-0.1.4.tar.gz` & `tmp/llama_index_llms_fireworks-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_fireworks-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_llms_fireworks-0.1.5.tar", max compression
```

## Comparing `llama_index_llms_fireworks-0.1.4.tar` & `llama_index_llms_fireworks-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       41 2024-02-26 03:20:40.032355 llama_index_llms_fireworks-0.1.4/README.md
--rw-r--r--   0        0        0       17 2024-02-26 03:20:40.032355 llama_index_llms_fireworks-0.1.4/llama_index/llms/fireworks/BUILD
--rw-r--r--   0        0        0       79 2024-02-26 03:20:40.032355 llama_index_llms_fireworks-0.1.4/llama_index/llms/fireworks/__init__.py
--rw-r--r--   0        0        0     2901 2024-02-26 18:26:06.578583 llama_index_llms_fireworks-0.1.4/llama_index/llms/fireworks/base.py
--rw-r--r--   0        0        0     3767 2024-02-26 18:26:06.578583 llama_index_llms_fireworks-0.1.4/llama_index/llms/fireworks/utils.py
--rw-r--r--   0        0        0     1422 2024-02-26 19:00:55.160691 llama_index_llms_fireworks-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 llama_index_llms_fireworks-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       41 2024-04-20 18:08:19.156844 llama_index_llms_fireworks-0.1.5/README.md
+-rw-r--r--   0        0        0       17 2024-04-20 18:08:19.156844 llama_index_llms_fireworks-0.1.5/llama_index/llms/fireworks/BUILD
+-rw-r--r--   0        0        0       79 2024-04-20 18:08:19.156844 llama_index_llms_fireworks-0.1.5/llama_index/llms/fireworks/__init__.py
+-rw-r--r--   0        0        0     3390 2024-04-20 18:08:19.156844 llama_index_llms_fireworks-0.1.5/llama_index/llms/fireworks/base.py
+-rw-r--r--   0        0        0     3951 2024-04-20 18:08:19.156844 llama_index_llms_fireworks-0.1.5/llama_index/llms/fireworks/utils.py
+-rw-r--r--   0        0        0     1422 2024-04-20 18:08:19.156844 llama_index_llms_fireworks-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 llama_index_llms_fireworks-0.1.5/PKG-INFO
```

### Comparing `llama_index_llms_fireworks-0.1.4/llama_index/llms/fireworks/base.py` & `llama_index_llms_fireworks-0.1.5/llama_index/llms/fireworks/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,34 @@
 from llama_index.llms.openai import OpenAI
 
 DEFAULT_API_BASE = "https://api.fireworks.ai/inference/v1"
 DEFAULT_MODEL = "accounts/fireworks/models/mixtral-8x7b-instruct"
 
 
 class Fireworks(OpenAI):
+    """Fireworks LLM.
+
+    Examples:
+        `pip install llama-index-llms-fireworks`
+
+        ```python
+        from llama_index.llms.fireworks import Fireworks
+
+        # Create an instance of the Fireworks class
+        llm = Fireworks(
+            model="accounts/fireworks/models/mixtral-8x7b-instruct",
+            api_key="YOUR_API_KEY"
+        )
+
+        # Call the complete method with a prompt
+        resp = llm.complete("Hello world!")
+        print(resp)
+        ```
+    """
+
     def __init__(
         self,
         model: str = DEFAULT_MODEL,
         temperature: float = DEFAULT_TEMPERATURE,
         max_tokens: int = DEFAULT_NUM_OUTPUTS,
         additional_kwargs: Optional[Dict[str, Any]] = None,
         max_retries: int = 10,
```

### Comparing `llama_index_llms_fireworks-0.1.4/llama_index/llms/fireworks/utils.py` & `llama_index_llms_fireworks-0.1.5/llama_index/llms/fireworks/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,23 @@
 
 LLAMA_MODELS = {
     "accounts/fireworks/models/llama-v2-7b-chat": 4096,
     "accounts/fireworks/models/llama-v2-13b-chat": 4096,
     "accounts/fireworks/models/llama-v2-70b-chat": 4096,
     "accounts/fireworks/models/llama-v2-34b-code-instruct": 16384,
     "accounts/fireworks/models/llamaguard-7b": 4096,
+    "accounts/fireworks/models/llama-v3-8b-instruct": 8192,
+    "accounts/fireworks/models/llama-v3-70b-instruct": 8192,
 }
 
 MISTRAL_MODELS = {
     "accounts/fireworks/models/mistral-7b-instruct-4k": 16384,
     "accounts/fireworks/models/mixtral-8x7b-instruct": 32768,
     "accounts/fireworks/models/firefunction-v1": 32768,
+    "accounts/fireworks/models/mixtral-8x22b-instruct": 65536,
 }
 
 ALL_AVAILABLE_MODELS = {
     **LLAMA_MODELS,
     **MISTRAL_MODELS,
 }
```

### Comparing `llama_index_llms_fireworks-0.1.4/pyproject.toml` & `llama_index_llms_fireworks-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 [tool.poetry]
 authors = ["benjibc"]
 description = "llama-index llms fireworks integration"
 license = "MIT"
 name = "llama-index-llms-fireworks"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 llama-index-core = "^0.10.1"
 llama-index-llms-openai = "^0.1.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_llms_fireworks-0.1.4/PKG-INFO` & `llama_index_llms_fireworks-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-fireworks
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index llms fireworks integration
 License: MIT
 Author: benjibc
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

