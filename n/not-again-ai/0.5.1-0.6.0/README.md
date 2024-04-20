# Comparing `tmp/not_again_ai-0.5.1.tar.gz` & `tmp/not_again_ai-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not_again_ai-0.5.1.tar", max compression
+gzip compressed data, was "not_again_ai-0.6.0.tar", max compression
```

## Comparing `not_again_ai-0.5.1.tar` & `not_again_ai-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0     1071 2024-01-28 17:31:42.037063 not_again_ai-0.5.1/LICENSE
--rw-r--r--   0        0        0    14407 2024-04-06 17:00:39.883880 not_again_ai-0.5.1/README.md
--rw-r--r--   0        0        0     4151 2024-04-06 17:02:08.449047 not_again_ai-0.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-20 15:38:49.234719 not_again_ai-0.5.1/src/not_again_ai/__init__.py
--rw-r--r--   0        0        0        0 2023-10-22 01:25:46.292824 not_again_ai-0.5.1/src/not_again_ai/base/__init__.py
--rw-r--r--   0        0        0      344 2023-10-22 01:25:46.292824 not_again_ai-0.5.1/src/not_again_ai/base/file_system.py
--rw-r--r--   0        0        0     3448 2023-10-22 01:25:46.292824 not_again_ai-0.5.1/src/not_again_ai/base/parallel.py
--rw-r--r--   0        0        0      451 2024-03-31 23:12:37.684279 not_again_ai-0.5.1/src/not_again_ai/llm/__init__.py
--rw-r--r--   0        0        0     8269 2024-04-06 16:45:02.127390 not_again_ai-0.5.1/src/not_again_ai/llm/chat_completion.py
--rw-r--r--   0        0        0     4125 2024-04-06 16:44:56.735321 not_again_ai-0.5.1/src/not_again_ai/llm/chat_completion_vision.py
--rw-r--r--   0        0        0     3424 2024-02-04 00:26:08.346905 not_again_ai-0.5.1/src/not_again_ai/llm/context_management.py
--rw-r--r--   0        0        0     2500 2024-01-29 00:33:04.305624 not_again_ai-0.5.1/src/not_again_ai/llm/embeddings.py
--rw-r--r--   0        0        0     2470 2024-01-28 00:29:53.278594 not_again_ai-0.5.1/src/not_again_ai/llm/openai_client.py
--rw-r--r--   0        0        0     9498 2024-04-06 16:57:24.213284 not_again_ai-0.5.1/src/not_again_ai/llm/prompts.py
--rw-r--r--   0        0        0     4244 2024-02-04 00:27:48.412079 not_again_ai-0.5.1/src/not_again_ai/llm/tokens.py
--rw-r--r--   0        0        0       93 2022-11-20 15:38:49.234719 not_again_ai-0.5.1/src/not_again_ai/py.typed
--rw-r--r--   0        0        0      466 2024-03-31 23:13:12.512750 not_again_ai-0.5.1/src/not_again_ai/statistics/__init__.py
--rw-r--r--   0        0        0     4429 2024-01-28 00:06:13.617140 not_again_ai-0.5.1/src/not_again_ai/statistics/dependence.py
--rw-r--r--   0        0        0      447 2024-03-31 23:13:45.949200 not_again_ai-0.5.1/src/not_again_ai/viz/__init__.py
--rw-r--r--   0        0        0     3382 2023-11-19 21:07:35.038071 not_again_ai-0.5.1/src/not_again_ai/viz/barplots.py
--rw-r--r--   0        0        0     4354 2023-10-22 01:25:46.292824 not_again_ai-0.5.1/src/not_again_ai/viz/distributions.py
--rw-r--r--   0        0        0     2290 2023-10-22 01:25:46.292824 not_again_ai-0.5.1/src/not_again_ai/viz/scatterplot.py
--rw-r--r--   0        0        0     5212 2024-01-27 23:36:54.323725 not_again_ai-0.5.1/src/not_again_ai/viz/time_series.py
--rw-r--r--   0        0        0      238 2022-11-20 15:38:49.234719 not_again_ai-0.5.1/src/not_again_ai/viz/utils.py
--rw-r--r--   0        0        0    15972 1970-01-01 00:00:00.000000 not_again_ai-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-01-28 17:31:42.037063 not_again_ai-0.6.0/LICENSE
+-rw-r--r--   0        0        0    14407 2024-04-20 17:53:46.881490 not_again_ai-0.6.0/README.md
+-rw-r--r--   0        0        0     4145 2024-04-20 19:07:12.112393 not_again_ai-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-20 15:38:49.234719 not_again_ai-0.6.0/src/not_again_ai/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-22 01:25:46.292824 not_again_ai-0.6.0/src/not_again_ai/base/__init__.py
+-rw-r--r--   0        0        0      344 2023-10-22 01:25:46.292824 not_again_ai-0.6.0/src/not_again_ai/base/file_system.py
+-rw-r--r--   0        0        0     3448 2023-10-22 01:25:46.292824 not_again_ai-0.6.0/src/not_again_ai/base/parallel.py
+-rw-r--r--   0        0        0      451 2024-04-20 17:53:46.881490 not_again_ai-0.6.0/src/not_again_ai/llm/__init__.py
+-rw-r--r--   0        0        0     8528 2024-04-20 18:00:17.873978 not_again_ai-0.6.0/src/not_again_ai/llm/chat_completion.py
+-rw-r--r--   0        0        0     3424 2024-02-04 00:26:08.346905 not_again_ai-0.6.0/src/not_again_ai/llm/context_management.py
+-rw-r--r--   0        0        0     2500 2024-01-29 00:33:04.305624 not_again_ai-0.6.0/src/not_again_ai/llm/embeddings.py
+-rw-r--r--   0        0        0     2470 2024-01-28 00:29:53.278594 not_again_ai-0.6.0/src/not_again_ai/llm/openai_client.py
+-rw-r--r--   0        0        0     7094 2024-04-20 19:17:25.528556 not_again_ai-0.6.0/src/not_again_ai/llm/prompts.py
+-rw-r--r--   0        0        0     4301 2024-04-20 19:20:27.986968 not_again_ai-0.6.0/src/not_again_ai/llm/tokens.py
+-rw-r--r--   0        0        0       93 2022-11-20 15:38:49.234719 not_again_ai-0.6.0/src/not_again_ai/py.typed
+-rw-r--r--   0        0        0      466 2024-04-20 17:53:46.881490 not_again_ai-0.6.0/src/not_again_ai/statistics/__init__.py
+-rw-r--r--   0        0        0     4429 2024-01-28 00:06:13.617140 not_again_ai-0.6.0/src/not_again_ai/statistics/dependence.py
+-rw-r--r--   0        0        0      447 2024-04-20 17:53:46.881490 not_again_ai-0.6.0/src/not_again_ai/viz/__init__.py
+-rw-r--r--   0        0        0     3382 2023-11-19 21:07:35.038071 not_again_ai-0.6.0/src/not_again_ai/viz/barplots.py
+-rw-r--r--   0        0        0     4354 2023-10-22 01:25:46.292824 not_again_ai-0.6.0/src/not_again_ai/viz/distributions.py
+-rw-r--r--   0        0        0     2290 2023-10-22 01:25:46.292824 not_again_ai-0.6.0/src/not_again_ai/viz/scatterplot.py
+-rw-r--r--   0        0        0     5212 2024-01-27 23:36:54.323725 not_again_ai-0.6.0/src/not_again_ai/viz/time_series.py
+-rw-r--r--   0        0        0      238 2022-11-20 15:38:49.234719 not_again_ai-0.6.0/src/not_again_ai/viz/utils.py
+-rw-r--r--   0        0        0    15966 1970-01-01 00:00:00.000000 not_again_ai-0.6.0/PKG-INFO
```

### Comparing `not_again_ai-0.5.1/LICENSE` & `not_again_ai-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.5.1/README.md` & `not_again_ai-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.5.1/pyproject.toml` & `not_again_ai-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "not-again-ai"
-version = "0.5.1"
+version = "0.6.0"
 description = "Designed to once and for all collect all the little things that come up over and over again in AI projects and put them in one place."
 authors = ["DaveCoDev <dave.co.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/DaveCoDev/not-again-ai"
 documentation = "https://github.com/DaveCoDev/not-again-ai"
 classifiers = [
@@ -24,19 +24,19 @@
 # Some packages, such as scipy, constrain their upper bound of Python versions they support.
 # Without also constraining the upper bound here, Poetry will not select those versions and will
 # result in an old version being resolved/locked.
 python = "^3.11, <3.13"
 
 # Optional dependencies are defined here, and groupings are defined below.
 numpy = { version = "^1.26.4", optional = true }
-openai = { version = "^1.16.2", optional = true }
-pandas = { version = "^2.2.1", optional = true }
+openai = { version = "^1.23.2", optional = true }
+pandas = { version = "^2.2.2", optional = true }
 python-liquid = { version = "^1.12.1", optional = true }
 scipy = { version = "^1.13.0", optional = true }
-scikit-learn = { version = "^1.4.1.post1", optional = true }
+scikit-learn = { version = "^1.4.2", optional = true }
 seaborn = { version = "^0.13.2", optional = true }
 tiktoken = { version = "^0.6.0", optional = true }
 
 [tool.poetry.extras]
 llm = ["openai", "python-liquid", "tiktoken"]
 statistics = ["numpy", "scikit-learn", "scipy"]
 viz = ["numpy", "pandas", "seaborn"]
```

### Comparing `not_again_ai-0.5.1/src/not_again_ai/base/parallel.py` & `not_again_ai-0.6.0/src/not_again_ai/base/parallel.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.5.1/src/not_again_ai/llm/chat_completion.py` & `not_again_ai-0.6.0/src/not_again_ai/llm/chat_completion.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,18 @@
     seed: int | None = None,
     logprobs: tuple[bool, int | None] | None = None,
     n: int = 1,
     **kwargs: Any,
 ) -> dict[str, Any]:
     """Get an OpenAI chat completion response: https://platform.openai.com/docs/api-reference/chat/create
 
+    NOTE: Depending on the model, certain parameters may not be supported,
+    particularly for older vision-enabled models like gpt-4-1106-vision-preview.
+    Be sure to check the documentation: https://platform.openai.com/docs/models/gpt-4-turbo-and-gpt-4
+
     Args:
         messages (list): A list of messages comprising the conversation so far.
         model (str): ID of the model to use. See the model endpoint compatibility table:
             https://platform.openai.com/docs/models/model-endpoint-compatibility
             for details on which models work with the Chat API.
         client (OpenAI): An instance of the OpenAI client.
         tools (list[dict[str, Any]], optional): A list of tools the model may generate JSON inputs for.
```

### Comparing `not_again_ai-0.5.1/src/not_again_ai/llm/context_management.py` & `not_again_ai-0.6.0/src/not_again_ai/llm/context_management.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.5.1/src/not_again_ai/llm/embeddings.py` & `not_again_ai-0.6.0/src/not_again_ai/llm/embeddings.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.5.1/src/not_again_ai/llm/openai_client.py` & `not_again_ai-0.6.0/src/not_again_ai/llm/openai_client.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.5.1/src/not_again_ai/llm/prompts.py` & `not_again_ai-0.6.0/src/not_again_ai/llm/prompts.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,77 +3,21 @@
 import mimetypes
 from pathlib import Path
 from typing import Any
 
 from liquid import Template
 
 
-def _validate_message(message: dict[str, str]) -> bool:
-    """Valides that a message has valid fields and if the role is valid.
-    See https://platform.openai.com/docs/api-reference/chat/create#chat-create-messages
-    """
-    valid_fields = ["role", "content", "name", "tool_call_id", "tool_calls"]
-    # Check if the only keys in the message are in valid_fields
-    if not all(key in valid_fields for key in message):
-        raise ValueError(f"Message contains invalid fields: {message.keys()}")
-
-    # Check if the only roles in the message are in valid_fields
-    valid_roles = ["system", "user", "assistant", "tool"]
-    if message["role"] not in valid_roles:
-        raise ValueError(f"Message contains invalid role: {message['role']}")
-
-    return True
-
-
-def chat_prompt(messages_unformatted: list[dict[str, str]], variables: dict[str, str]) -> list[dict[str, str]]:
-    """
-    Formats a list of messages for OpenAI's chat completion API using Liquid templating.
-
-    Args:
-        messages_unformatted: A list of dictionaries where each dictionary
-            represents a message. Each message must have 'role' and 'content'
-            keys with string values, where content is a Liquid template.
-        variables: A dictionary where each key-value pair represents a variable
-            name and its value for template rendering.
-
-    Returns:
-        A list of dictionaries with the same structure as `messages_unformatted`,
-        but with the 'content' of each message with the provided `variables`.
-
-    Examples:
-        >>> messages = [
-        ...     {"role": "system", "content": "You are a helpful assistant."},
-        ...     {"role": "user", "content": "Help me {{task}}"}
-        ... ]
-        >>> vars = {"task": "write Python code for the fibonnaci sequence"}
-        >>> chat_prompt(messages, vars)
-        [
-            {"role": "system", "content": "You are a helpful assistant."},
-            {"role": "user", "content": "Help me write Python code for the fibonnaci sequence"}
-        ]
-    """
-
-    messages_formatted = deepcopy(messages_unformatted)
-    for message in messages_formatted:
-        if not _validate_message(message):
-            raise ValueError()
-
-        liquid_template = Template(message["content"])
-        message["content"] = liquid_template.render(**variables)
-
-    return messages_formatted
-
-
 def _validate_message_vision(message: dict[str, list[dict[str, Path | str]] | str]) -> bool:
     """Validates that a message for a vision model is valid"""
-    valid_fields = ["role", "content"]
+    valid_fields = ["role", "content", "name", "tool_call_id", "tool_calls"]
     if not all(key in valid_fields for key in message):
         raise ValueError(f"Message contains invalid fields: {message.keys()}")
 
-    valid_roles = ["system", "user", "assistant"]
+    valid_roles = ["system", "user", "assistant", "tool"]
     if message["role"] not in valid_roles:
         raise ValueError(f"Message contains invalid role: {message['role']}")
 
     if not isinstance(message["content"], list) and not isinstance(message["content"], str):
         raise ValueError(f"content must be a list of dictionaries or a string: {message['content']}")
 
     if isinstance(message["content"], list):
@@ -122,21 +66,21 @@
     # List of valid types is here: https://platform.openai.com/docs/guides/vision/what-type-of-files-can-i-upload
     if mime_type not in valid_mime_types:
         raise ValueError(f"Invalid MIME type for image: {mime_type}")
 
     return f"data:{mime_type};base64,{image_data}"
 
 
-def chat_prompt_vision(messages_unformatted: list[dict[str, Any]], variables: dict[str, str]) -> list[dict[str, Any]]:
-    """Formats a list of messages for OpenAI's chat completion API, for vision models only, using Liquid templating.
+def chat_prompt(messages_unformatted: list[dict[str, Any]], variables: dict[str, str]) -> list[dict[str, Any]]:
+    """Formats a list of messages for OpenAI's chat completion API,
+    including special syntax for vision models, using Liquid templating.
 
     Args:
         messages_unformatted (list[dict[str, list[dict[str, Path | str]] | str]]):
             A list of dictionaries where each dictionary represents a message.
-            Each message must have 'role' and 'content' keys. `role` must be 'system', 'user', or 'assistant'.
             `content` can be a Liquid template string or a list of dictionaries where each dictionary
             represents a content part. Each content part can be a string or a dictionary with 'image' and 'detail' keys.
             The 'image' key must be a Path or a string representing a URL. The 'detail' key is optional and must be 'low' or 'high'.
         variables: A dictionary where each key-value pair represents a variable
             name and its value for template rendering.
 
     Returns:
```

### Comparing `not_again_ai-0.5.1/src/not_again_ai/llm/tokens.py` & `not_again_ai-0.6.0/src/not_again_ai/llm/tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,16 @@
         "gpt-4-0314",
         "gpt-4-32k-0314",
         "gpt-4-0613",
         "gpt-4-32k-0613",
         "gpt-4-1106-preview",
         "gpt-4-turbo-preview",
         "gpt-4-0125-preview",
+        "gpt-4-turbo",
+        "gpt-4-turbo-2024-04-09",
     }:
         tokens_per_message = 3  # every message follows <|start|>{role/name}\n{content}<|end|>\n
         tokens_per_name = 1  # if there's a name, the role is omitted
     elif model == "gpt-3.5-turbo-0301":
         tokens_per_message = 4
         tokens_per_name = -1
     # Approximate catch-all. Assumes future versions of 3.5 and 4 will have the same token counts as the 0613 versions.
```

### Comparing `not_again_ai-0.5.1/src/not_again_ai/statistics/dependence.py` & `not_again_ai-0.6.0/src/not_again_ai/statistics/dependence.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.5.1/src/not_again_ai/viz/barplots.py` & `not_again_ai-0.6.0/src/not_again_ai/viz/barplots.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.5.1/src/not_again_ai/viz/distributions.py` & `not_again_ai-0.6.0/src/not_again_ai/viz/distributions.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.5.1/src/not_again_ai/viz/scatterplot.py` & `not_again_ai-0.6.0/src/not_again_ai/viz/scatterplot.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.5.1/src/not_again_ai/viz/time_series.py` & `not_again_ai-0.6.0/src/not_again_ai/viz/time_series.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.5.1/PKG-INFO` & `not_again_ai-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not-again-ai
-Version: 0.5.1
+Version: 0.6.0
 Summary: Designed to once and for all collect all the little things that come up over and over again in AI projects and put them in one place.
 Home-page: https://github.com/DaveCoDev/not-again-ai
 License: MIT
 Author: DaveCoDev
 Author-email: dave.co.dev@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: Development Status :: 3 - Alpha
@@ -17,18 +17,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Provides-Extra: llm
 Provides-Extra: statistics
 Provides-Extra: viz
 Requires-Dist: numpy (>=1.26.4,<2.0.0) ; extra == "statistics" or extra == "viz"
-Requires-Dist: openai (>=1.16.2,<2.0.0) ; extra == "llm"
-Requires-Dist: pandas (>=2.2.1,<3.0.0) ; extra == "viz"
+Requires-Dist: openai (>=1.23.2,<2.0.0) ; extra == "llm"
+Requires-Dist: pandas (>=2.2.2,<3.0.0) ; extra == "viz"
 Requires-Dist: python-liquid (>=1.12.1,<2.0.0) ; extra == "llm"
-Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0) ; extra == "statistics"
+Requires-Dist: scikit-learn (>=1.4.2,<2.0.0) ; extra == "statistics"
 Requires-Dist: scipy (>=1.13.0,<2.0.0) ; extra == "statistics"
 Requires-Dist: seaborn (>=0.13.2,<0.14.0) ; extra == "viz"
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0) ; extra == "llm"
 Project-URL: Documentation, https://github.com/DaveCoDev/not-again-ai
 Project-URL: Repository, https://github.com/DaveCoDev/not-again-ai
 Description-Content-Type: text/markdown
```

