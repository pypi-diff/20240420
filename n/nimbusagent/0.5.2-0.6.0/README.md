# Comparing `tmp/nimbusagent-0.5.2.tar.gz` & `tmp/nimbusagent-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nimbusagent-0.5.2.tar", last modified: Wed Apr 17 11:36:55 2024, max compression
+gzip compressed data, was "nimbusagent-0.6.0.tar", last modified: Sat Apr 20 10:59:27 2024, max compression
```

## Comparing `nimbusagent-0.5.2.tar` & `nimbusagent-0.6.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-17 11:36:55.865181 nimbusagent-0.5.2/
--rw-r--r--   0 Lee        (501) staff       (20)     3101 2023-12-04 18:36:26.000000 nimbusagent-0.5.2/.gitignore
--rw-r--r--   0 Lee        (501) staff       (20)     1073 2023-12-06 18:57:23.000000 nimbusagent-0.5.2/LICENSE.txt
--rw-r--r--   0 Lee        (501) staff       (20)       48 2023-11-18 23:57:46.000000 nimbusagent-0.5.2/MANIFEST.in
--rw-r--r--   0 Lee        (501) staff       (20)    10527 2024-04-17 11:36:55.864630 nimbusagent-0.5.2/PKG-INFO
--rw-r--r--   0 Lee        (501) staff       (20)     7992 2024-04-16 23:09:24.000000 nimbusagent-0.5.2/README.md
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-17 11:36:55.771738 nimbusagent-0.5.2/bin/
--rwxr-xr-x   0 Lee        (501) staff       (20)      384 2023-12-26 20:55:01.000000 nimbusagent-0.5.2/bin/build.sh
--rwxr-xr-x   0 Lee        (501) staff       (20)      209 2023-12-22 17:10:13.000000 nimbusagent-0.5.2/bin/publish-pypi.sh
--rwxr-xr-x   0 Lee        (501) staff       (20)      240 2023-12-22 17:34:16.000000 nimbusagent-0.5.2/bin/run_tests.sh
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-17 11:36:55.787150 nimbusagent-0.5.2/examples/
--rw-r--r--   0 Lee        (501) staff       (20)      277 2023-12-04 21:15:51.000000 nimbusagent-0.5.2/examples/completion_agent_basic_example.py
--rw-r--r--   0 Lee        (501) staff       (20)     1532 2023-12-26 21:17:23.000000 nimbusagent-0.5.2/examples/completion_agent_function_example.py
--rw-r--r--   0 Lee        (501) staff       (20)      427 2023-12-04 21:15:51.000000 nimbusagent-0.5.2/examples/completion_agent_history_example.py
--rw-r--r--   0 Lee        (501) staff       (20)      362 2023-12-04 21:15:51.000000 nimbusagent-0.5.2/examples/streaming_agent_basic_example.py
--rw-r--r--   0 Lee        (501) staff       (20)     1620 2023-12-26 21:17:23.000000 nimbusagent-0.5.2/examples/streaming_agent_function_example.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-17 11:36:55.794411 nimbusagent-0.5.2/examples/streaming_cli_chatbot/
--rw-r--r--   0 Lee        (501) staff       (20)     2376 2023-12-04 18:36:26.000000 nimbusagent-0.5.2/examples/streaming_cli_chatbot/simple_spinner.py
--rw-r--r--   0 Lee        (501) staff       (20)     2999 2023-12-04 21:15:51.000000 nimbusagent-0.5.2/examples/streaming_cli_chatbot/streaming_cli_chatbot.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-17 11:36:55.794867 nimbusagent-0.5.2/nimbusagent/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.5.2/nimbusagent/__init__.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-17 11:36:55.814901 nimbusagent-0.5.2/nimbusagent/agent/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.5.2/nimbusagent/agent/__init__.py
--rw-r--r--   0 Lee        (501) staff       (20)    13679 2024-04-17 11:35:54.000000 nimbusagent-0.5.2/nimbusagent/agent/base.py
--rw-r--r--   0 Lee        (501) staff       (20)     5140 2024-04-05 21:23:21.000000 nimbusagent-0.5.2/nimbusagent/agent/completion.py
--rw-r--r--   0 Lee        (501) staff       (20)    12853 2024-04-16 22:49:59.000000 nimbusagent-0.5.2/nimbusagent/agent/streaming.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-17 11:36:55.833495 nimbusagent-0.5.2/nimbusagent/functions/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.5.2/nimbusagent/functions/__init__.py
--rw-r--r--   0 Lee        (501) staff       (20)    17923 2024-01-26 20:49:40.000000 nimbusagent-0.5.2/nimbusagent/functions/handler.py
--rw-r--r--   0 Lee        (501) staff       (20)     9997 2023-12-04 21:15:51.000000 nimbusagent-0.5.2/nimbusagent/functions/parser.py
--rw-r--r--   0 Lee        (501) staff       (20)     2293 2023-12-26 21:17:23.000000 nimbusagent-0.5.2/nimbusagent/functions/responses.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-17 11:36:55.837447 nimbusagent-0.5.2/nimbusagent/memory/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.5.2/nimbusagent/memory/__init__.py
--rw-r--r--   0 Lee        (501) staff       (20)     5417 2023-12-04 21:15:51.000000 nimbusagent-0.5.2/nimbusagent/memory/base.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-17 11:36:55.842953 nimbusagent-0.5.2/nimbusagent/utils/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.5.2/nimbusagent/utils/__init__.py
--rw-r--r--   0 Lee        (501) staff       (20)     4246 2024-01-26 21:46:54.000000 nimbusagent-0.5.2/nimbusagent/utils/helper.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-17 11:36:55.863686 nimbusagent-0.5.2/nimbusagent.egg-info/
--rw-r--r--   0 Lee        (501) staff       (20)    10527 2024-04-17 11:36:55.000000 nimbusagent-0.5.2/nimbusagent.egg-info/PKG-INFO
--rw-r--r--   0 Lee        (501) staff       (20)     1259 2024-04-17 11:36:55.000000 nimbusagent-0.5.2/nimbusagent.egg-info/SOURCES.txt
--rw-r--r--   0 Lee        (501) staff       (20)        1 2024-04-17 11:36:55.000000 nimbusagent-0.5.2/nimbusagent.egg-info/dependency_links.txt
--rw-r--r--   0 Lee        (501) staff       (20)       60 2024-04-17 11:36:55.000000 nimbusagent-0.5.2/nimbusagent.egg-info/requires.txt
--rw-r--r--   0 Lee        (501) staff       (20)       12 2024-04-17 11:36:55.000000 nimbusagent-0.5.2/nimbusagent.egg-info/top_level.txt
--rw-r--r--   0 Lee        (501) staff       (20)     1365 2024-04-17 11:36:09.000000 nimbusagent-0.5.2/pyproject.toml
--rw-r--r--   0 Lee        (501) staff       (20)       38 2024-04-17 11:36:55.865245 nimbusagent-0.5.2/setup.cfg
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-17 11:36:55.863039 nimbusagent-0.5.2/tests/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 18:36:26.000000 nimbusagent-0.5.2/tests/__init__.py
--rw-r--r--   0 Lee        (501) staff       (20)     1962 2024-04-17 11:36:39.000000 nimbusagent-0.5.2/tests/test_nimbusagent_agent_base.py
--rw-r--r--   0 Lee        (501) staff       (20)     1012 2023-12-26 21:17:23.000000 nimbusagent-0.5.2/tests/test_nimbusagent_functions_handler.py
--rw-r--r--   0 Lee        (501) staff       (20)     1874 2023-12-04 21:15:51.000000 nimbusagent-0.5.2/tests/test_nimbusagent_functions_parser.py
--rw-r--r--   0 Lee        (501) staff       (20)      607 2023-12-26 21:17:23.000000 nimbusagent-0.5.2/tests/test_nimbusagent_functions_response.py
--rw-r--r--   0 Lee        (501) staff       (20)     4619 2023-12-04 21:15:51.000000 nimbusagent-0.5.2/tests/test_nimbusagent_memory_base.py
--rw-r--r--   0 Lee        (501) staff       (20)     6772 2024-01-05 19:48:38.000000 nimbusagent-0.5.2/tests/test_nimbusagent_utils.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.919646 nimbusagent-0.6.0/
+-rw-r--r--   0 Lee        (501) staff       (20)     3101 2023-12-04 18:36:26.000000 nimbusagent-0.6.0/.gitignore
+-rw-r--r--   0 Lee        (501) staff       (20)     1073 2023-12-06 18:57:23.000000 nimbusagent-0.6.0/LICENSE.txt
+-rw-r--r--   0 Lee        (501) staff       (20)       48 2023-11-18 23:57:46.000000 nimbusagent-0.6.0/MANIFEST.in
+-rw-r--r--   0 Lee        (501) staff       (20)    10527 2024-04-20 10:59:27.918787 nimbusagent-0.6.0/PKG-INFO
+-rw-r--r--   0 Lee        (501) staff       (20)     7992 2024-04-16 23:09:24.000000 nimbusagent-0.6.0/README.md
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.829045 nimbusagent-0.6.0/bin/
+-rwxr-xr-x   0 Lee        (501) staff       (20)      384 2023-12-26 20:55:01.000000 nimbusagent-0.6.0/bin/build.sh
+-rwxr-xr-x   0 Lee        (501) staff       (20)      209 2023-12-22 17:10:13.000000 nimbusagent-0.6.0/bin/publish-pypi.sh
+-rwxr-xr-x   0 Lee        (501) staff       (20)      240 2023-12-22 17:34:16.000000 nimbusagent-0.6.0/bin/run_tests.sh
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.845623 nimbusagent-0.6.0/examples/
+-rw-r--r--   0 Lee        (501) staff       (20)      277 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/examples/completion_agent_basic_example.py
+-rw-r--r--   0 Lee        (501) staff       (20)     1532 2023-12-26 21:17:23.000000 nimbusagent-0.6.0/examples/completion_agent_function_example.py
+-rw-r--r--   0 Lee        (501) staff       (20)      427 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/examples/completion_agent_history_example.py
+-rw-r--r--   0 Lee        (501) staff       (20)      362 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/examples/streaming_agent_basic_example.py
+-rw-r--r--   0 Lee        (501) staff       (20)     1620 2023-12-26 21:17:23.000000 nimbusagent-0.6.0/examples/streaming_agent_function_example.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.851482 nimbusagent-0.6.0/examples/streaming_cli_chatbot/
+-rw-r--r--   0 Lee        (501) staff       (20)     2376 2023-12-04 18:36:26.000000 nimbusagent-0.6.0/examples/streaming_cli_chatbot/simple_spinner.py
+-rw-r--r--   0 Lee        (501) staff       (20)     2999 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/examples/streaming_cli_chatbot/streaming_cli_chatbot.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.852094 nimbusagent-0.6.0/nimbusagent/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/nimbusagent/__init__.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.870413 nimbusagent-0.6.0/nimbusagent/agent/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/nimbusagent/agent/__init__.py
+-rw-r--r--   0 Lee        (501) staff       (20)    14119 2024-04-20 10:50:08.000000 nimbusagent-0.6.0/nimbusagent/agent/base.py
+-rw-r--r--   0 Lee        (501) staff       (20)     5140 2024-04-05 21:23:21.000000 nimbusagent-0.6.0/nimbusagent/agent/completion.py
+-rw-r--r--   0 Lee        (501) staff       (20)    12853 2024-04-16 22:49:59.000000 nimbusagent-0.6.0/nimbusagent/agent/streaming.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.884684 nimbusagent-0.6.0/nimbusagent/functions/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/nimbusagent/functions/__init__.py
+-rw-r--r--   0 Lee        (501) staff       (20)    18224 2024-04-20 10:54:04.000000 nimbusagent-0.6.0/nimbusagent/functions/handler.py
+-rw-r--r--   0 Lee        (501) staff       (20)     9997 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/nimbusagent/functions/parser.py
+-rw-r--r--   0 Lee        (501) staff       (20)     2293 2023-12-26 21:17:23.000000 nimbusagent-0.6.0/nimbusagent/functions/responses.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.888450 nimbusagent-0.6.0/nimbusagent/memory/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/nimbusagent/memory/__init__.py
+-rw-r--r--   0 Lee        (501) staff       (20)     5417 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/nimbusagent/memory/base.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.893131 nimbusagent-0.6.0/nimbusagent/utils/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/nimbusagent/utils/__init__.py
+-rw-r--r--   0 Lee        (501) staff       (20)     4246 2024-01-26 21:46:54.000000 nimbusagent-0.6.0/nimbusagent/utils/helper.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.918128 nimbusagent-0.6.0/nimbusagent.egg-info/
+-rw-r--r--   0 Lee        (501) staff       (20)    10527 2024-04-20 10:59:27.000000 nimbusagent-0.6.0/nimbusagent.egg-info/PKG-INFO
+-rw-r--r--   0 Lee        (501) staff       (20)     1259 2024-04-20 10:59:27.000000 nimbusagent-0.6.0/nimbusagent.egg-info/SOURCES.txt
+-rw-r--r--   0 Lee        (501) staff       (20)        1 2024-04-20 10:59:27.000000 nimbusagent-0.6.0/nimbusagent.egg-info/dependency_links.txt
+-rw-r--r--   0 Lee        (501) staff       (20)       60 2024-04-20 10:59:27.000000 nimbusagent-0.6.0/nimbusagent.egg-info/requires.txt
+-rw-r--r--   0 Lee        (501) staff       (20)       12 2024-04-20 10:59:27.000000 nimbusagent-0.6.0/nimbusagent.egg-info/top_level.txt
+-rw-r--r--   0 Lee        (501) staff       (20)     1365 2024-04-20 10:54:04.000000 nimbusagent-0.6.0/pyproject.toml
+-rw-r--r--   0 Lee        (501) staff       (20)       38 2024-04-20 10:59:27.919729 nimbusagent-0.6.0/setup.cfg
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.917451 nimbusagent-0.6.0/tests/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 18:36:26.000000 nimbusagent-0.6.0/tests/__init__.py
+-rw-r--r--   0 Lee        (501) staff       (20)     1962 2024-04-17 11:36:39.000000 nimbusagent-0.6.0/tests/test_nimbusagent_agent_base.py
+-rw-r--r--   0 Lee        (501) staff       (20)     1012 2023-12-26 21:17:23.000000 nimbusagent-0.6.0/tests/test_nimbusagent_functions_handler.py
+-rw-r--r--   0 Lee        (501) staff       (20)     1874 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/tests/test_nimbusagent_functions_parser.py
+-rw-r--r--   0 Lee        (501) staff       (20)      607 2023-12-26 21:17:23.000000 nimbusagent-0.6.0/tests/test_nimbusagent_functions_response.py
+-rw-r--r--   0 Lee        (501) staff       (20)     4619 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/tests/test_nimbusagent_memory_base.py
+-rw-r--r--   0 Lee        (501) staff       (20)     6772 2024-01-05 19:48:38.000000 nimbusagent-0.6.0/tests/test_nimbusagent_utils.py
```

### Comparing `nimbusagent-0.5.2/.gitignore` & `nimbusagent-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.2/LICENSE.txt` & `nimbusagent-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.2/PKG-INFO` & `nimbusagent-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nimbusagent
-Version: 0.5.2
+Version: 0.6.0
 Summary: An OpenAI agent with basic memory, functions, and moderation support
 Author: Lee Huffman
 License: MIT License
         
         Copyright (c) 2023 Vaisala Xweather
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nimbusagent-0.5.2/README.md` & `nimbusagent-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.2/examples/completion_agent_function_example.py` & `nimbusagent-0.6.0/examples/completion_agent_function_example.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.2/examples/streaming_agent_function_example.py` & `nimbusagent-0.6.0/examples/streaming_agent_function_example.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.2/examples/streaming_cli_chatbot/simple_spinner.py` & `nimbusagent-0.6.0/examples/streaming_cli_chatbot/simple_spinner.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.2/examples/streaming_cli_chatbot/streaming_cli_chatbot.py` & `nimbusagent-0.6.0/examples/streaming_cli_chatbot/streaming_cli_chatbot.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.2/nimbusagent/agent/base.py` & `nimbusagent-0.6.0/nimbusagent/agent/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
             max_tokens: int = 500,
 
             functions: Optional[list] = None,
             functions_embeddings: Optional[List[dict]] = None,
             functions_embeddings_model: str = FUNCTIONS_EMBEDDING_MODEL,
             functions_always_use: Optional[List[str]] = None,
             functions_pattern_groups: Optional[List[dict]] = None,
+            function_pattern_mode: Literal['all','first'] = 'all',
             functions_k_closest: int = 3,
             function_min_similarity: float = 0.5,
 
             function_max_tokens: int = 2000,
             use_tool_calls: bool = True,
 
             system_message: str = SYS_MSG,
@@ -66,14 +67,16 @@
             model_name: The name of the model to use (default: 'gpt-4-0613')
             secondary_model_name: The name of the secondary model to use (default: 'gpt-3.5-turbo')
             temperature: The temperature for the response sampling (default: 0.1)
             functions: The list of functions to use (default: None)
             functions_embeddings: The list of function embeddings to use (default: None)
             functions_embeddings_model: The model to use for function embeddings (default: 'text-embedding-ada-002')
             functions_pattern_groups: The list of function pattern groups to use (default: None)
+            function_pattern_mode: The mode to use for function patterns (default: 'all') step through all patterns
+                            or 'first' to stop at the first match
             functions_k_closest: The number of closest embedding functions to use (default: 3)
             function_min_similarity: The minimum similarity to use for embedding functions (default: 0.5)
             functions_always_use: The list of functions to always use (default: None)
             function_max_tokens: The maximum number of tokens to allow for function call. (default: 2500) 0 = unlimited
             use_tool_calls: True if parallel functions should be allowed (default: True). Functions are being
                             deprecated though tool_calls are still a bit beta, so for now this can be set to
                             False to continue using function calls.
@@ -128,14 +131,15 @@
         self.function_handler = self._init_function_handler(
             functions=functions,
             functions_embeddings=functions_embeddings,
             functions_embeddings_model=functions_embeddings_model,
             functions_k_closest=functions_k_closest,
             functions_always_use=functions_always_use,
             functions_pattern_groups=functions_pattern_groups,
+            function_pattern_mode=function_pattern_mode,
             function_max_tokens=function_max_tokens,
             function_min_similarity=function_min_similarity)
         self.use_tool_calls = use_tool_calls
 
     def set_system_message(self, message: str) -> None:
         """Sets the system message.
         :param message: The system message to set
@@ -146,14 +150,15 @@
                                functions: Optional[List],
                                functions_embeddings: Optional[List],
                                functions_embeddings_model: str = FUNCTIONS_EMBEDDING_MODEL,
                                functions_k_closest: int = 3,
                                function_min_similarity: float = 0.5,
                                functions_always_use: Optional[List[str]] = None,
                                functions_pattern_groups: Optional[List[dict]] = None,
+                               function_pattern_mode: Literal['all','first'] = 'all',
                                function_max_tokens: int = 0) -> FunctionHandler:
         """Initializes the function handler.
         Returns a FunctionHandler instance.
 
         :param functions: The list of functions to use
         :param functions_embeddings: The list of function embeddings to use
         :param functions_k_closest: The number of closest functions to use
@@ -166,14 +171,15 @@
             functions=functions,
             embeddings=functions_embeddings,
             embeddings_model=functions_embeddings_model,
             k_nearest=functions_k_closest,
             min_similarity=function_min_similarity,
             always_use=functions_always_use,
             pattern_groups=functions_pattern_groups,
+            pattern_mode=function_pattern_mode,
             calling_function_start_callback=self.calling_function_start_callback,
             calling_function_stop_callback=self.calling_function_stop_callback,
             max_tokens=function_max_tokens,
             chat_history=self.chat_history
         )
 
     # noinspection PyUnresolvedReferences
```

### Comparing `nimbusagent-0.5.2/nimbusagent/agent/completion.py` & `nimbusagent-0.6.0/nimbusagent/agent/completion.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.2/nimbusagent/agent/streaming.py` & `nimbusagent-0.6.0/nimbusagent/agent/streaming.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.2/nimbusagent/functions/handler.py` & `nimbusagent-0.6.0/nimbusagent/functions/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ast
 import inspect
 import json
 import logging
 import re
 from dataclasses import dataclass
-from typing import Optional, List, Dict, Any, Union, Callable, Type, Tuple
+from typing import Optional, List, Dict, Any, Union, Callable, Type, Tuple, Literal
 
 import tiktoken
 from openai.types.chat import ChatCompletionToolParam
 
 from nimbusagent.functions import parser
 from nimbusagent.functions.responses import FuncResponse, DictFuncResponse
 from nimbusagent.memory.base import AgentMemory
@@ -45,37 +45,40 @@
     :param chat_history:  The chat history to use.  If None, no chat history will be used.
     """
     functions = None
     func_mapping = None
     always_use = None
     orig_functions: dict = None
     pattern_groups = None
+    pattern_mode = 'all'
     chat_history: AgentMemory = None
     processed_functions = None
     max_tokens = 0
 
     def __init__(self, functions: list = None,
                  embeddings: list = None,
                  embeddings_model: str = FUNCTIONS_EMBEDDING_MODEL,
                  k_nearest: int = 3,
                  min_similarity: float = 0.5,
                  always_use: list = None,
                  pattern_groups: list = None,
+                 pattern_mode: Literal['all', 'first'] = 'all',
                  calling_function_start_callback: callable = None,
                  calling_function_stop_callback: callable = None,
                  chat_history: AgentMemory = None,
                  max_tokens: int = 0
                  ):
 
         self.embeddings = embeddings
         self.embeddings_model = embeddings_model
         self.k_nearest = k_nearest
         self.min_similarity = min_similarity
         self.always_use = always_use
         self.pattern_groups = pattern_groups
+        self.pattern_mode = pattern_mode
         self.chat_history = chat_history
         self.encoding = tiktoken.get_encoding("cl100k_base")
         self.max_tokens = max_tokens
 
         self.orig_functions = {func.__name__: func for func in functions} if functions else None
         if not embeddings:
             self.functions = self.parse_functions(functions)
@@ -120,31 +123,33 @@
                             tokens=func_tokens,
                             mapping=mapping,
                             mapping_name=mapping_name)
 
     def _get_group_function(self, query: str) -> Optional[List[str]]:
         """
         Get the list of functions to use based on the pattern groups.
-        :param query:  The query to use.
-        :return:  The list of functions to use based on the pattern groups. If no pattern groups are found, None is
-                    returned.
+        :param query: The query to use.
+        :return: The list of functions to use based on the pattern groups. If no pattern groups are found, None is returned.
         """
         if not self.pattern_groups:
             return None
 
         function_names = []
 
         for group in self.pattern_groups:
             if re.search(group['pattern'], query):
                 for func in group['functions']:
                     func_name = func if isinstance(func, str) else func.__name__
                     if func_name not in function_names and func_name in self.orig_functions:
                         function_names.append(func_name)
+                # Break out of the loop after the first match if mode is 'first'
+                if self.pattern_mode == 'first':
+                    break
 
-        return function_names
+        return function_names if function_names else None
 
     def remove_functions_mappings(self, function_names: List[str]):
         """
         Remove the given functions from the function mappings.
         :param function_names:  The list of function names to remove.
         """
         if not self.processed_functions:
```

### Comparing `nimbusagent-0.5.2/nimbusagent/functions/parser.py` & `nimbusagent-0.6.0/nimbusagent/functions/parser.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.2/nimbusagent/functions/responses.py` & `nimbusagent-0.6.0/nimbusagent/functions/responses.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.2/nimbusagent/memory/base.py` & `nimbusagent-0.6.0/nimbusagent/memory/base.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.2/nimbusagent/utils/helper.py` & `nimbusagent-0.6.0/nimbusagent/utils/helper.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.2/nimbusagent.egg-info/PKG-INFO` & `nimbusagent-0.6.0/nimbusagent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nimbusagent
-Version: 0.5.2
+Version: 0.6.0
 Summary: An OpenAI agent with basic memory, functions, and moderation support
 Author: Lee Huffman
 License: MIT License
         
         Copyright (c) 2023 Vaisala Xweather
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nimbusagent-0.5.2/nimbusagent.egg-info/SOURCES.txt` & `nimbusagent-0.6.0/nimbusagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.2/pyproject.toml` & `nimbusagent-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nimbusagent"
-version = "0.5.2"
+version = "0.6.0"
 description = "An OpenAI agent with basic memory, functions, and moderation support"
 readme = "README.md"
 license = { file = "LICENSE.txt" }
 keywords = [
     "openai",
     "gpt3",
     "gpt3.5",
```

### Comparing `nimbusagent-0.5.2/tests/test_nimbusagent_agent_base.py` & `nimbusagent-0.6.0/tests/test_nimbusagent_agent_base.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.2/tests/test_nimbusagent_functions_handler.py` & `nimbusagent-0.6.0/tests/test_nimbusagent_functions_handler.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.2/tests/test_nimbusagent_functions_parser.py` & `nimbusagent-0.6.0/tests/test_nimbusagent_functions_parser.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.2/tests/test_nimbusagent_functions_response.py` & `nimbusagent-0.6.0/tests/test_nimbusagent_functions_response.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.2/tests/test_nimbusagent_memory_base.py` & `nimbusagent-0.6.0/tests/test_nimbusagent_memory_base.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.2/tests/test_nimbusagent_utils.py` & `nimbusagent-0.6.0/tests/test_nimbusagent_utils.py`

 * *Files identical despite different names*

