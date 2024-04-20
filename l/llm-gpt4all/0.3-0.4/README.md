# Comparing `tmp/llm-gpt4all-0.3.tar.gz` & `tmp/llm_gpt4all-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-gpt4all-0.3.tar", last modified: Wed Jan 24 03:18:19 2024, max compression
+gzip compressed data, was "llm_gpt4all-0.4.tar", last modified: Sat Apr 20 00:33:40 2024, max compression
```

## Comparing `llm-gpt4all-0.3.tar` & `llm_gpt4all-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 03:18:19.981918 llm-gpt4all-0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-24 03:18:07.000000 llm-gpt4all-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-01-24 03:18:19.981918 llm-gpt4all-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-01-24 03:18:07.000000 llm-gpt4all-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 03:18:19.981918 llm-gpt4all-0.3/llm_gpt4all.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-01-24 03:18:19.000000 llm-gpt4all-0.3/llm_gpt4all.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-24 03:18:19.000000 llm-gpt4all-0.3/llm_gpt4all.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 03:18:19.000000 llm-gpt4all-0.3/llm_gpt4all.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-24 03:18:19.000000 llm-gpt4all-0.3/llm_gpt4all.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-24 03:18:19.000000 llm-gpt4all-0.3/llm_gpt4all.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-24 03:18:19.000000 llm-gpt4all-0.3/llm_gpt4all.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-01-24 03:18:07.000000 llm-gpt4all-0.3/llm_gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-24 03:18:19.981918 llm-gpt4all-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-01-24 03:18:07.000000 llm-gpt4all-0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 03:18:19.981918 llm-gpt4all-0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-01-24 03:18:07.000000 llm-gpt4all-0.3/tests/test_llm_gpt4all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:33:40.654027 llm_gpt4all-0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-20 00:33:30.000000 llm_gpt4all-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-04-20 00:33:40.654027 llm_gpt4all-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-04-20 00:33:30.000000 llm_gpt4all-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:33:40.654027 llm_gpt4all-0.4/llm_gpt4all.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-04-20 00:33:40.000000 llm_gpt4all-0.4/llm_gpt4all.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-20 00:33:40.000000 llm_gpt4all-0.4/llm_gpt4all.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 00:33:40.000000 llm_gpt4all-0.4/llm_gpt4all.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-20 00:33:40.000000 llm_gpt4all-0.4/llm_gpt4all.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-20 00:33:40.000000 llm_gpt4all-0.4/llm_gpt4all.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-20 00:33:40.000000 llm_gpt4all-0.4/llm_gpt4all.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9829 2024-04-20 00:33:30.000000 llm_gpt4all-0.4/llm_gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 00:33:40.654027 llm_gpt4all-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-20 00:33:30.000000 llm_gpt4all-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:33:40.654027 llm_gpt4all-0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-20 00:33:30.000000 llm_gpt4all-0.4/tests/test_llm_gpt4all.py
```

### Comparing `llm-gpt4all-0.3/LICENSE` & `llm_gpt4all-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-gpt4all-0.3/PKG-INFO` & `llm_gpt4all-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: llm-gpt4all
-Version: 0.3
+Version: 0.4
 Summary: Plugin for LLM adding support for GPT4ALL models
 Home-page: https://github.com/simonw/llm-gpt4all
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/llm-gpt4all/issues
 Project-URL: CI, https://github.com/simonw/llm-gpt4all/actions
 Project-URL: Changelog, https://github.com/simonw/llm-gpt4all/releases
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: llm>=0.11
-Requires-Dist: gpt4all>=2.0.1
+Requires-Dist: gpt4all>=2.5.1
 Requires-Dist: httpx
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # llm-gpt4all
 
 [![PyPI](https://img.shields.io/pypi/v/llm-gpt4all.svg)](https://pypi.org/project/llm-gpt4all/)
```

### Comparing `llm-gpt4all-0.3/README.md` & `llm_gpt4all-0.4/README.md`

 * *Files identical despite different names*

### Comparing `llm-gpt4all-0.3/llm_gpt4all.egg-info/PKG-INFO` & `llm_gpt4all-0.4/llm_gpt4all.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: llm-gpt4all
-Version: 0.3
+Version: 0.4
 Summary: Plugin for LLM adding support for GPT4ALL models
 Home-page: https://github.com/simonw/llm-gpt4all
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/llm-gpt4all/issues
 Project-URL: CI, https://github.com/simonw/llm-gpt4all/actions
 Project-URL: Changelog, https://github.com/simonw/llm-gpt4all/releases
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: llm>=0.11
-Requires-Dist: gpt4all>=2.0.1
+Requires-Dist: gpt4all>=2.5.1
 Requires-Dist: httpx
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # llm-gpt4all
 
 [![PyPI](https://img.shields.io/pypi/v/llm-gpt4all.svg)](https://pypi.org/project/llm-gpt4all/)
```

### Comparing `llm-gpt4all-0.3/llm_gpt4all.py` & `llm_gpt4all-0.4/llm_gpt4all.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,24 +31,27 @@
     def retrieve_model(
         model_name: str,
         model_path: Optional[str] = None,
         allow_download: bool = True,
         verbose: bool = False,
     ) -> str:
         try:
-            return _GPT4All.retrieve_model(model_name, model_path, allow_download, verbose)
+            return _GPT4All.retrieve_model(
+                model_name, model_path, allow_download, verbose
+            )
         except requests.exceptions.ConnectionError:
-            return _GPT4All.retrieve_model(model_name, model_path, allow_download=False, verbose=verbose)
-
+            return _GPT4All.retrieve_model(
+                model_name, model_path, allow_download=False, verbose=verbose
+            )
 
 
 def get_gpt4all_models():
     return fetch_cached_json(
-        url="https://gpt4all.io/models/models2.json",
-        path=llm.user_dir() / "gpt4all_models2.json",
+        url="https://gpt4all.io/models/models3.json",
+        path=llm.user_dir() / "gpt4all_models3.json",
         cache_timeout=3600,
     )
 
 
 @llm.hookimpl
 def register_models(register):
     raw_models = get_gpt4all_models()
@@ -69,30 +72,36 @@
     can_stream = True
 
     class Options(llm.Options):
         max_tokens: int = Field(
             description="The maximum number of tokens to generate.", default=200
         )
         temp: float = Field(
-            description="The model temperature. Larger values increase creativity but decrease factuality.", default=0.7
+            description="The model temperature. Larger values increase creativity but decrease factuality.",
+            default=0.7,
         )
         top_k: int = Field(
-            description="Randomly sample from the top_k most likely tokens at each generation step. Set this to 1 for greedy decoding.", default=40
+            description="Randomly sample from the top_k most likely tokens at each generation step. Set this to 1 for greedy decoding.",
+            default=40,
         )
         top_p: float = Field(
-            description="Randomly sample at each generation step from the top most likely tokens whose probabilities add up to top_p.", default=0.4
+            description="Randomly sample at each generation step from the top most likely tokens whose probabilities add up to top_p.",
+            default=0.4,
         )
         repeat_penalty: float = Field(
-            description="Penalize the model for repetition. Higher values result in less repetition.", default=1.18
+            description="Penalize the model for repetition. Higher values result in less repetition.",
+            default=1.18,
         )
         repeat_last_n: int = Field(
-            description="How far in the models generation history to apply the repeat penalty.", default=64
+            description="How far in the models generation history to apply the repeat penalty.",
+            default=64,
         )
         n_batch: int = Field(
-            description="Number of prompt tokens processed in parallel. Larger values decrease latency but increase resource requirements.", default=8
+            description="Number of prompt tokens processed in parallel. Larger values decrease latency but increase resource requirements.",
+            default=8,
         )
 
     def __init__(self, details):
         self._details = details
         self.model_id = details["filename"].split(".")[0]
 
     def prompt_template(self):
@@ -154,21 +163,21 @@
             model_name = self.filename()
             model_exists_locally = Path(GPT4ALL_MODEL_DIRECTORY / model_name).exists()
             allow_download = not model_exists_locally
             gpt_model = GPT4All(model_name, allow_download=allow_download)
             output = gpt_model.generate(
                 text_prompt,
                 streaming=True,
-                max_tokens = prompt.options.max_tokens or 400,
-                temp = prompt.options.temp,
-                top_k = prompt.options.top_k,
-                top_p = prompt.options.top_p,
-                repeat_penalty = prompt.options.repeat_penalty,
-                repeat_last_n = prompt.options.repeat_last_n,
-                n_batch = prompt.options.n_batch,
+                max_tokens=prompt.options.max_tokens or 400,
+                temp=prompt.options.temp,
+                top_k=prompt.options.top_k,
+                top_p=prompt.options.top_p,
+                repeat_penalty=prompt.options.repeat_penalty,
+                repeat_last_n=prompt.options.repeat_last_n,
+                n_batch=prompt.options.n_batch,
             )
             yield from output
 
     def filename(self):
         return self._details["filename"]
 
     def filesize_bytes(self):
@@ -176,15 +185,15 @@
 
     def is_installed(self):
         try:
             GPT4All.retrieve_model(
                 self._details["filename"], allow_download=False, verbose=False
             )
             return True
-        except ValueError:
+        except (FileNotFoundError, ValueError):
             return False
 
     def __str__(self):
         installed = " (installed)" if self.is_installed() else ""
         return "gpt4all: {} - {}, {} download, needs {}GB RAM{}".format(
             self.model_id,
             self._details["name"],
```

### Comparing `llm-gpt4all-0.3/setup.py` & `llm_gpt4all-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.3"
+VERSION = "0.4"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -27,13 +27,13 @@
     license="Apache License, Version 2.0",
     classifiers=["License :: OSI Approved :: Apache Software License"],
     version=VERSION,
     modules=["llm_gpt4all"],
     entry_points={"llm": ["gpt4all = llm_gpt4all"]},
     install_requires=[
         "llm>=0.11",
-        "gpt4all>=2.0.1",
+        "gpt4all>=2.5.1",
         "httpx",
     ],
     extras_require={"test": ["pytest"]},
     python_requires=">=3.9",
 )
```

### Comparing `llm-gpt4all-0.3/tests/test_llm_gpt4all.py` & `llm_gpt4all-0.4/tests/test_llm_gpt4all.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,59 +14,41 @@
 
 
 def test_llm_models():
     runner = CliRunner()
     result = runner.invoke(cli, ["models", "list"])
     assert result.exit_code == 0, result.output
     for fragment in (
-        "gpt4all: ggml-gpt4all-j-v1 - Groovy, 3.53GB download, needs 8GB RAM",
-        "gpt4all: orca-mini-7b - Orca, 3.53GB download, needs 8GB RAM",
-        "gpt4all: ggml-model-gpt4all-falcon-q4_0 - GPT4All Falcon, 3.78GB download, needs 8GB RAM",
-        "gpt4all: ggml-mpt-7b-chat - MPT Chat, 4.52GB download, needs 8GB RAM",
+        "gpt4all: Meta-Llama-3-8B-Instruct - Llama 3 Instruct, 4.34GB download, needs 8GB RAM",
+        "gpt4all: mistral-7b-instruct-v0 - Mistral Instruct, 3.83GB download, needs 8GB RAM",
     ):
         assert fragment in result.output
 
 
 @pytest.mark.parametrize(
     "model_id,expected_blocks",
     (
         (
-            "ggml-gpt4all-j-v1",
-            # This has no promptTemplate, so default display
+            "Meta-Llama-3-8B-Instruct",
             [
-                "### Human: \ninput 1\n### Assistant:\n",
+                "<|start_header_id|>user<|end_header_id|>\n\ninput 1<|eot_id|><|start_header_id|>assistant<|end_header_id|>\n\n%2<|eot_id|>",
                 "response 1",
-                "### Human: \ninput 2\n### Assistant:\n",
+                "<|start_header_id|>user<|end_header_id|>\n\ninput 2<|eot_id|><|start_header_id|>assistant<|end_header_id|>\n\n%2<|eot_id|>",
             ],
         ),
         (
-            "orca-mini-7b",
-            # This has no promptTemplate, so default display
-            [
-                "### User:\ninput 1\n### Response:\n",
-                "response 1",
-                "### User:\ninput 2\n### Response:\n",
-            ],
-        ),
-        (
-            "ggml-mpt-7b-chat",
-            # This has no promptTemplate, so default display
-            [
-                "<|im_start|>user\ninput 1<|im_end|><|im_start|>assistant\n",
-                "response 1<|im_end|>",
-                "<|im_start|>user\ninput 2<|im_end|><|im_start|>assistant\n",
-            ],
+            "mistral-7b-instruct-v0",
+            ["[INST] input 1 [/INST]", "response 1", "[INST] input 2 [/INST]"],
         ),
         (
-            "ggml-model-gpt4all-falcon-q4_0",
-            # This has no promptTemplate, so default display
+            "orca-mini-3b-gguf2-q4_0",
             [
-                "### Instruction:\ninput 1\n### Response:\n",
+                "### User:\ninput 1\n\n### Response:\n",
                 "response 1",
-                "### Instruction:\ninput 2\n### Response:\n",
+                "### User:\ninput 2\n\n### Response:\n",
             ],
         ),
     ),
 )
 def test_conversation_prompt_blocks(model_id, expected_blocks):
     model = llm.get_model(model_id)
     conversation = model.conversation()
```

