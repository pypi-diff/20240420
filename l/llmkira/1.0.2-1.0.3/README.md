# Comparing `tmp/llmkira-1.0.2.tar.gz` & `tmp/llmkira-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmkira-1.0.2.tar", last modified: Thu Apr 18 15:06:55 2024, max compression
+gzip compressed data, was "llmkira-1.0.3.tar", last modified: Sat Apr 20 05:32:17 2024, max compression
```

## Comparing `llmkira-1.0.2.tar` & `llmkira-1.0.3.tar`

### file list

```diff
@@ -1,60 +1,61 @@
--rw-r--r--   0        0        0    11357 2024-04-18 15:06:42.707143 llmkira-1.0.2/LICENSE
--rw-r--r--   0        0        0     1030 2024-04-18 15:06:42.707143 llmkira-1.0.2/NOTICE.MD
--rw-r--r--   0        0        0     7780 2024-04-18 15:06:42.707143 llmkira-1.0.2/README.md
--rw-r--r--   0        0        0      730 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/__init__.py
--rw-r--r--   0        0        0      209 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/_exception.py
--rw-r--r--   0        0        0     5346 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/cache/__init__.py
--rw-r--r--   0        0        0     1266 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/cache/elara_runtime.py
--rw-r--r--   0        0        0     2299 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/cache/lmdb_runtime.py
--rw-r--r--   0        0        0     1451 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/cache/redis_runtime.py
--rw-r--r--   0        0        0     1159 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/cache/runtime_schema.py
--rw-r--r--   0        0        0     4711 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/doc_manager/__init__.py
--rw-r--r--   0        0        0      127 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/extra/plugins/__init__.py
--rw-r--r--   0        0        0     6768 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/extra/plugins/alarm/__init__.py
--rw-r--r--   0        0        0     6005 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/extra/plugins/search/__init__.py
--rw-r--r--   0        0        0     1774 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/extra/plugins/search/engine.py
--rw-r--r--   0        0        0     5527 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/extra/voice/__init__.py
--rw-r--r--   0        0        0     3247 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/extra/voice_hook.py
--rw-r--r--   0        0        0        0 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/kv_manager/__init__.py
--rw-r--r--   0        0        0      626 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/kv_manager/_base.py
--rw-r--r--   0        0        0     2323 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/kv_manager/env.py
--rw-r--r--   0        0        0     4419 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/kv_manager/file.py
--rw-r--r--   0        0        0     1015 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/kv_manager/instruction.py
--rw-r--r--   0        0        0     1512 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/kv_manager/time.py
--rw-r--r--   0        0        0     1070 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/kv_manager/tool_call.py
--rw-r--r--   0        0        0      637 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/memory/__init__.py
--rw-r--r--   0        0        0      733 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/memory/_base.py
--rw-r--r--   0        0        0     2381 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/memory/local_storage.py
--rw-r--r--   0        0        0     1070 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/memory/redis_storage/LICENSE
--rw-r--r--   0        0        0     2819 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/memory/redis_storage/__init__.py
--rw-r--r--   0        0        0     6192 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/memory/redis_storage/utils.py
--rw-r--r--   0        0        0      522 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/openai/__init__.py
--rw-r--r--   0        0        0     3431 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/openai/_excption.py
--rw-r--r--   0        0        0    10293 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/openai/cell.py
--rw-r--r--   0        0        0     8546 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/openai/request.py
--rw-r--r--   0        0        0     1968 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/openai/utils.py
--rw-r--r--   0        0        0      130 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/openapi/__init__.py
--rw-r--r--   0        0        0     2729 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/openapi/fuse/__init__.py
--rw-r--r--   0        0        0     1610 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/openapi/hook/__init__.py
--rw-r--r--   0        0        0     4285 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/openapi/transducer/__init__.py
--rw-r--r--   0        0        0      799 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/openapi/transducer/default_factory.py
--rw-r--r--   0        0        0     1229 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/openapi/transducer/schema.py
--rw-r--r--   0        0        0     2143 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/openapi/trigger/__init__.py
--rw-r--r--   0        0        0      419 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/openapi/trigger/default_trigger.py
--rw-r--r--   0        0        0      321 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/sdk/__init__.py
--rw-r--r--   0        0        0     1069 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/sdk/tools/LICENSE
--rw-r--r--   0        0        0     4501 2024-04-18 15:06:42.727143 llmkira-1.0.2/llmkira/sdk/tools/__init__.py
--rw-r--r--   0        0        0      496 2024-04-18 15:06:42.731143 llmkira-1.0.2/llmkira/sdk/tools/error.py
--rw-r--r--   0        0        0     3373 2024-04-18 15:06:42.731143 llmkira-1.0.2/llmkira/sdk/tools/loader.py
--rw-r--r--   0        0        0     9551 2024-04-18 15:06:42.731143 llmkira-1.0.2/llmkira/sdk/tools/model.py
--rw-r--r--   0        0        0     3286 2024-04-18 15:06:42.731143 llmkira-1.0.2/llmkira/sdk/tools/register.py
--rw-r--r--   0        0        0    10610 2024-04-18 15:06:42.731143 llmkira-1.0.2/llmkira/sdk/tools/schema.py
--rw-r--r--   0        0        0     4233 2024-04-18 15:06:42.731143 llmkira-1.0.2/llmkira/sdk/utils.py
--rw-r--r--   0        0        0     4848 2024-04-18 15:06:42.731143 llmkira-1.0.2/llmkira/task/__init__.py
--rw-r--r--   0        0        0    16588 2024-04-18 15:06:42.731143 llmkira-1.0.2/llmkira/task/schema.py
--rw-r--r--   0        0        0      219 2024-04-18 15:06:42.731143 llmkira-1.0.2/llmkira/task/snapshot/__init__.py
--rw-r--r--   0        0        0      422 2024-04-18 15:06:42.731143 llmkira-1.0.2/llmkira/task/snapshot/_base.py
--rw-r--r--   0        0        0     1237 2024-04-18 15:06:42.731143 llmkira-1.0.2/llmkira/task/snapshot/local.py
--rw-r--r--   0        0        0     2898 2024-04-18 15:06:55.610990 llmkira-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1485 2024-04-18 15:06:42.731143 llmkira-1.0.2/tests/pydantic_error.py
--rw-r--r--   0        0        0    11094 1970-01-01 00:00:00.000000 llmkira-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-20 05:32:02.352945 llmkira-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1030 2024-04-20 05:32:02.352945 llmkira-1.0.3/NOTICE.MD
+-rw-r--r--   0        0        0     8422 2024-04-20 05:32:02.352945 llmkira-1.0.3/README.md
+-rw-r--r--   0        0        0      730 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/__init__.py
+-rw-r--r--   0        0        0      209 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/_exception.py
+-rw-r--r--   0        0        0     5346 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/cache/__init__.py
+-rw-r--r--   0        0        0     1266 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/cache/elara_runtime.py
+-rw-r--r--   0        0        0     2299 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/cache/lmdb_runtime.py
+-rw-r--r--   0        0        0     1451 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/cache/redis_runtime.py
+-rw-r--r--   0        0        0     1159 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/cache/runtime_schema.py
+-rw-r--r--   0        0        0     4711 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/doc_manager/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/extra/plugins/__init__.py
+-rw-r--r--   0        0        0     6886 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/extra/plugins/alarm/__init__.py
+-rw-r--r--   0        0        0     8269 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/extra/plugins/e2b_code_interpreter/__init__.py
+-rw-r--r--   0        0        0     5950 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/extra/plugins/search/__init__.py
+-rw-r--r--   0        0        0     1774 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/extra/plugins/search/engine.py
+-rw-r--r--   0        0        0     5527 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/extra/voice/__init__.py
+-rw-r--r--   0        0        0     3247 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/extra/voice_hook.py
+-rw-r--r--   0        0        0        0 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/kv_manager/__init__.py
+-rw-r--r--   0        0        0      626 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/kv_manager/_base.py
+-rw-r--r--   0        0        0     2323 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/kv_manager/env.py
+-rw-r--r--   0        0        0     4419 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/kv_manager/file.py
+-rw-r--r--   0        0        0     1025 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/kv_manager/instruction.py
+-rw-r--r--   0        0        0     1512 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/kv_manager/time.py
+-rw-r--r--   0        0        0     1158 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/kv_manager/tool_call.py
+-rw-r--r--   0        0        0      637 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/memory/__init__.py
+-rw-r--r--   0        0        0      733 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/memory/_base.py
+-rw-r--r--   0        0        0     2381 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/memory/local_storage.py
+-rw-r--r--   0        0        0     1070 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/memory/redis_storage/LICENSE
+-rw-r--r--   0        0        0     2819 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/memory/redis_storage/__init__.py
+-rw-r--r--   0        0        0     6192 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/memory/redis_storage/utils.py
+-rw-r--r--   0        0        0      522 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openai/__init__.py
+-rw-r--r--   0        0        0     3431 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openai/_excption.py
+-rw-r--r--   0        0        0    10731 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openai/cell.py
+-rw-r--r--   0        0        0     8553 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openai/request.py
+-rw-r--r--   0        0        0     1968 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openai/utils.py
+-rw-r--r--   0        0        0      130 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openapi/__init__.py
+-rw-r--r--   0        0        0     2729 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openapi/fuse/__init__.py
+-rw-r--r--   0        0        0     1610 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openapi/hook/__init__.py
+-rw-r--r--   0        0        0     4285 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openapi/transducer/__init__.py
+-rw-r--r--   0        0        0      799 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openapi/transducer/default_factory.py
+-rw-r--r--   0        0        0     1229 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openapi/transducer/schema.py
+-rw-r--r--   0        0        0     2143 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openapi/trigger/__init__.py
+-rw-r--r--   0        0        0      419 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openapi/trigger/default_trigger.py
+-rw-r--r--   0        0        0      321 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/sdk/__init__.py
+-rw-r--r--   0        0        0     1069 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/sdk/tools/LICENSE
+-rw-r--r--   0        0        0     4501 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/sdk/tools/__init__.py
+-rw-r--r--   0        0        0      496 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/sdk/tools/error.py
+-rw-r--r--   0        0        0     3373 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/sdk/tools/loader.py
+-rw-r--r--   0        0        0     9551 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/sdk/tools/model.py
+-rw-r--r--   0        0        0     3286 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/sdk/tools/register.py
+-rw-r--r--   0        0        0    10609 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/sdk/tools/schema.py
+-rw-r--r--   0        0        0     4238 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/sdk/utils.py
+-rw-r--r--   0        0        0     4848 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/task/__init__.py
+-rw-r--r--   0        0        0    16694 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/task/schema.py
+-rw-r--r--   0        0        0      219 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/task/snapshot/__init__.py
+-rw-r--r--   0        0        0      422 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/task/snapshot/_base.py
+-rw-r--r--   0        0        0     1237 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/task/snapshot/local.py
+-rw-r--r--   0        0        0     2919 2024-04-20 05:32:17.048968 llmkira-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1485 2024-04-20 05:32:02.380945 llmkira-1.0.3/tests/pydantic_error.py
+-rw-r--r--   0        0        0    11765 1970-01-01 00:00:00.000000 llmkira-1.0.3/PKG-INFO
```

### Comparing `llmkira-1.0.2/LICENSE` & `llmkira-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/NOTICE.MD` & `llmkira-1.0.3/NOTICE.MD`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/README.md` & `llmkira-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -38,23 +38,25 @@
 > Python>=3.9
 
 This project uses the ToolCall feature.
 
 It integrates a message queuing and snapshot system, offering plugin mechanisms and authentication prior to plugin
 execution.
 
-The model adheres to the Openai Format Schema. Please adapt using [gateway](https://github.com/Portkey-AI/gateway)
+The bot adheres to the **Openai Format Schema**. Please adapt using [gateway](https://github.com/Portkey-AI/gateway)
 or [one-api](https://github.com/songquanpeng/one-api) independently.
 
-| Demo                              | Vision With Voice            |
-|-----------------------------------|------------------------------|
-| ![sticker](./docs/chain_chat.gif) | ![vision](./docs/vision.gif) |
+| Demo                                                                          | Vision With Voice                                                        | Code Interpreter                                                                      |
+|-------------------------------------------------------------------------------|--------------------------------------------------------------------------|---------------------------------------------------------------------------------------|
+| ![sticker](https://github.com/LlmKira/Openaibot/raw/main/docs/chain_chat.gif) | ![vision](https://github.com/LlmKira/Openaibot/raw/main/docs/vision.gif) | ![code](https://github.com/LlmKira/Openaibot/raw/main/docs/code_interpreter_func.gif) |
 
 ## 🔨 Roadmap
 
+> The program has iterated to its fourth generation.
+
 - [x] Removal of legacy code
 - [x] Deletion of metric system
 - [x] Deletion of model selection system, unified to OpenAI Schema
 - [x] Implementation of a more robust plugin system
 - [x] Project structure simplification
 - [x] Elimination of the Provider system
 - [x] Hook support
@@ -73,22 +75,23 @@
 - 🍟 Multi-platform support – extend new platforms by inheriting the base class
 - 🍔 Plugins can determine their appearance in new sessions dynamically, preventing performance degradation despite large
   amounts of plugins
 
 ### 🍔 Login Modes
 
 - `Login via url`: Use `/login token$https://provider.com` to Login. The program posts the token to the interface to
-  retrieve configuration information
+  retrieve configuration
+  information, [how to develop this](https://github.com/LlmKira/Openaibot/blob/81eddbff0f136697d5ad6e13ee1a7477b26624ed/app/components/credential.py#L20).
 - `Login`: Use `/login https://api.com/v1$key$model` to login
 
-### 🧀 Plugin Previews
+### 🧀 Plugin Can Do More
 
-| Sticker Converter                   | Timer Function                  | Translate Function                           |
-|-------------------------------------|---------------------------------|----------------------------------------------|
-| ![sticker](./docs/sticker_func.gif) | ![timer](./docs/timer_func.gif) | ![translate](./docs/translate_file_func.gif) |
+| Sticker Converter                   | Timer Function(built-in)        |
+|-------------------------------------|---------------------------------|
+| ![sticker](./docs/sticker_func.gif) | ![timer](./docs/timer_func.gif) |
 
 ### 🎬 Platform Support
 
 | Platform | Support | File System | Remarks                                |
 |----------|---------|-------------|----------------------------------------|
 | Telegram | ✅       | ✅           |                                        |
 | Discord  | ✅       | ✅           |                                        |
@@ -101,51 +104,57 @@
 | IRC      | ❌       |             |                                        |
 | ...      |         |             | Create Issue/PR                        |
 
 ## 📦 Quick Start
 
 Refer to the [🧀 Deployment Document](https://llmkira.github.io/Docs/) for more information.
 
+### 📦 One-click Deployment
+
+If you are using a brand-new server, you can use the following shell to automatically install this project.
+
+```shell
+curl -sSL https://raw.githubusercontent.com/LLMKira/Openaibot/main/deploy.sh | bash
+```
+
+### 📦 Manual Installation
+
 ```shell
-# Install Telegram Voice dependencies
+# Install Voice dependencies
 apt install ffmpeg
 # Install RabbitMQ
 docker pull rabbitmq:3.10-management
 docker run -d -p 5672:5672 -p 15672:15672 \
   -e RABBITMQ_DEFAULT_USER=admin \
   -e RABBITMQ_DEFAULT_PASS=8a8a8a \
   --hostname myRabbit \
   --name rabbitmq \
   rabbitmq:3.10-management
 docker ps -l
 # Install Project
+git clone https://github.com/LlmKira/Openaibot/
+cd Openaibot
 pip install pdm
 pdm install -G bot
 cp .env.exp .env && nano .env
 # Test
 pdm run python3 start_sender.py
 pdm run python3 start_receiver.py
 # Host
-pdm start pm2.json
+apt install npm
+npm install pm2 -g
+pm2 start pm2.json
 ```
 
 ### 🥣 Docker
 
 Build Hub: [sudoskys/llmbot](https://hub.docker.com/repository/docker/sudoskys/llmbot/general)
 
-#### Automatic Docker/Docker-compose Installation
-
-If you are using a brand new server, you can use the following shell to automatically install this project.
-
-This script automatically installs the required services and maps ports using Docker methods. If you have
-deployed `redis`, `rabbitmq`, `mongodb`, please modify the `docker-compose.yml` file accordingly.
-
-```shell
-curl -sSL https://raw.githubusercontent.com/LLMKira/Openaibot/main/deploy.sh | bash
-```
+> Note that if you run this project using Docker, you will start Redis, MongoDB, and RabbitMQ. But if you're running
+> locally, just RabbitMQ
 
 #### Manual Docker-compose Installation
 
 ```shell
 git clone https://github.com/LlmKira/Openaibot.git
 cd Openaibot
 cp .env.exp .env&&nano .env
@@ -181,16 +190,19 @@
 ### Hooks
 
 Hooks control the EventMessage in sender and receiver. For example, we have `voice_hook` in built-in hooks.
 
 you can enable it by setting `VOICE_REPLY_ME=true` in `.env`.
 
 ```shell
-/env VOICE_REPLY_ME=true
+/env VOICE_REPLY_ME=yes
+# must
+
 /env REECHO_VOICE_KEY=<key in dev.reecho.ai>
+# not must
 ```
 
 use `/env VOICE_REPLY_ME=NONE` to disable this env.
 
 check the source code in `llmkira/extra/voice_hook.py`, learn to write your own hooks.
 
 ## 🧀 Sponsor
```

#### html2text {}

```diff
@@ -3,81 +3,88 @@
                            _[_d_o_c_k_e_r_]_[_d_o_c_k_e_r_ _w_o_r_k_f_l_o_w_]
                               _[_t_e_l_e_g_r_a_m_]_[_d_i_s_c_o_r_d_]
                             _[_l_i_c_e_n_s_e_]_[_d_o_c_k_e_r_ _b_u_i_l_d_]
               _ð___©_ _D_e_p_l_o_y_ _D_o_c_s & _ð__§__ _D_e_v_ _D_o_c_s & _ð__¤__ _C_o_n_t_r_i_b_u_t_e
 > Don't hesitate to Star â­ï¸, Issue ð, and PR ð ï¸ > Python>=3.9 This
 project uses the ToolCall feature. It integrates a message queuing and snapshot
 system, offering plugin mechanisms and authentication prior to plugin
-execution. The model adheres to the Openai Format Schema. Please adapt using
+execution. The bot adheres to the **Openai Format Schema**. Please adapt using
 [gateway](https://github.com/Portkey-AI/gateway) or [one-api](https://
-github.com/songquanpeng/one-api) independently. | Demo | Vision With Voice | |-
-----------------------------------|------------------------------| | ![sticker]
-(./docs/chain_chat.gif) | ![vision](./docs/vision.gif) | ## ð¨ Roadmap - [x]
-Removal of legacy code - [x] Deletion of metric system - [x] Deletion of model
-selection system, unified to OpenAI Schema - [x] Implementation of a more
-robust plugin system - [x] Project structure simplification - [x] Elimination
-of the Provider system - [x] Hook support - [x] Access to TTS - [x] Add
-standalone support for gpt-4-turbo and vision - [ ] Add LLM reference support
-to the plugin environment. (extract && search in text) ## ð¦ Features - ðª
-A comprehensive plugin development ecosystem, adopting a classic design, and
-seamless integration with plugins through `pip` installation - ð Message
-system with no time or sender constraints, offering fully decoupled logics -
-ð¬ Offers Login via a URL mechanism, providing a flexible and expandable
-authentication development solution - ð° Empowers users to authorize plugin
-execution. Users can configure plugin environment variables at their discretion
-- ð¦ Support for plugins to access files - ð Multi-platform support â
-extend new platforms by inheriting the base class - ð Plugins can determine
-their appearance in new sessions dynamically, preventing performance
-degradation despite large amounts of plugins ### ð Login Modes - `Login via
-url`: Use `/login token$https://provider.com` to Login. The program posts the
-token to the interface to retrieve configuration information - `Login`: Use `/
-login https://api.com/v1$key$model` to login ### ð§ Plugin Previews | Sticker
-Converter | Timer Function | Translate Function | |----------------------------
----------|---------------------------------|-----------------------------------
------------| | ![sticker](./docs/sticker_func.gif) | ![timer](./docs/
-timer_func.gif) | ![translate](./docs/translate_file_func.gif) | ### ð¬
-Platform Support | Platform | Support | File System | Remarks | |----------|---
-------|-------------|----------------------------------------| | Telegram | â
-| â | | | Discord | â | â | | | Kook | â | â | Does not support
-`triggering by reply` | | Slack | â | â | Does not support `triggering by
-reply` | | QQ | â | | | | Wechat | â | | | | Twitter | â | | | | Matrix |
-â | | | | IRC | â | | | | ... | | | Create Issue/PR | ## ð¦ Quick Start
-Refer to the [ð§ Deployment Document](https://llmkira.github.io/Docs/) for
-more information. ```shell # Install Telegram Voice dependencies apt install
-ffmpeg # Install RabbitMQ docker pull rabbitmq:3.10-management docker run -d -
-p 5672:5672 -p 15672:15672 \ -e RABBITMQ_DEFAULT_USER=admin \ -
+github.com/songquanpeng/one-api) independently. | Demo | Vision With Voice |
+Code Interpreter | |-----------------------------------------------------------
+--------------------|----------------------------------------------------------
+----------------|--------------------------------------------------------------
+-------------------------| | ![sticker](https://github.com/LlmKira/Openaibot/
+raw/main/docs/chain_chat.gif) | ![vision](https://github.com/LlmKira/Openaibot/
+raw/main/docs/vision.gif) | ![code](https://github.com/LlmKira/Openaibot/raw/
+main/docs/code_interpreter_func.gif) | ## ð¨ Roadmap > The program has
+iterated to its fourth generation. - [x] Removal of legacy code - [x] Deletion
+of metric system - [x] Deletion of model selection system, unified to OpenAI
+Schema - [x] Implementation of a more robust plugin system - [x] Project
+structure simplification - [x] Elimination of the Provider system - [x] Hook
+support - [x] Access to TTS - [x] Add standalone support for gpt-4-turbo and
+vision - [ ] Add LLM reference support to the plugin environment. (extract &&
+search in text) ## ð¦ Features - ðª A comprehensive plugin development
+ecosystem, adopting a classic design, and seamless integration with plugins
+through `pip` installation - ð Message system with no time or sender
+constraints, offering fully decoupled logics - ð¬ Offers Login via a URL
+mechanism, providing a flexible and expandable authentication development
+solution - ð° Empowers users to authorize plugin execution. Users can
+configure plugin environment variables at their discretion - ð¦ Support for
+plugins to access files - ð Multi-platform support â extend new platforms
+by inheriting the base class - ð Plugins can determine their appearance in
+new sessions dynamically, preventing performance degradation despite large
+amounts of plugins ### ð Login Modes - `Login via url`: Use `/login
+token$https://provider.com` to Login. The program posts the token to the
+interface to retrieve configuration information, [how to develop this](https://
+github.com/LlmKira/Openaibot/blob/81eddbff0f136697d5ad6e13ee1a7477b26624ed/app/
+components/credential.py#L20). - `Login`: Use `/login https://api.com/
+v1$key$model` to login ### ð§ Plugin Can Do More | Sticker Converter | Timer
+Function(built-in) | |-------------------------------------|-------------------
+--------------| | ![sticker](./docs/sticker_func.gif) | ![timer](./docs/
+timer_func.gif) | ### ð¬ Platform Support | Platform | Support | File System
+| Remarks | |----------|---------|-------------|-------------------------------
+---------| | Telegram | â | â | | | Discord | â | â | | | Kook | â |
+â | Does not support `triggering by reply` | | Slack | â | â | Does not
+support `triggering by reply` | | QQ | â | | | | Wechat | â | | | | Twitter
+| â | | | | Matrix | â | | | | IRC | â | | | | ... | | | Create Issue/PR
+| ## ð¦ Quick Start Refer to the [ð§ Deployment Document](https://
+llmkira.github.io/Docs/) for more information. ### ð¦ One-click Deployment If
+you are using a brand-new server, you can use the following shell to
+automatically install this project. ```shell curl -sSL https://
+raw.githubusercontent.com/LLMKira/Openaibot/main/deploy.sh | bash ``` ### ð¦
+Manual Installation ```shell # Install Voice dependencies apt install ffmpeg #
+Install RabbitMQ docker pull rabbitmq:3.10-management docker run -d -p 5672:
+5672 -p 15672:15672 \ -e RABBITMQ_DEFAULT_USER=admin \ -
 e RABBITMQ_DEFAULT_PASS=8a8a8a \ --hostname myRabbit \ --name rabbitmq \
-rabbitmq:3.10-management docker ps -l # Install Project pip install pdm pdm
-install -G bot cp .env.exp .env && nano .env # Test pdm run python3
-start_sender.py pdm run python3 start_receiver.py # Host pdm start pm2.json ```
-### ð¥£ Docker Build Hub: [sudoskys/llmbot](https://hub.docker.com/repository/
-docker/sudoskys/llmbot/general) #### Automatic Docker/Docker-compose
-Installation If you are using a brand new server, you can use the following
-shell to automatically install this project. This script automatically installs
-the required services and maps ports using Docker methods. If you have deployed
-`redis`, `rabbitmq`, `mongodb`, please modify the `docker-compose.yml` file
-accordingly. ```shell curl -sSL https://raw.githubusercontent.com/LLMKira/
-Openaibot/main/deploy.sh | bash ``` #### Manual Docker-compose Installation
-```shell git clone https://github.com/LlmKira/Openaibot.git cd Openaibot cp
-.env.exp .env&&nano .env docker-compose -f docker-compose.yml up -d ``` The
-Docker configuration file `docker-compose.yml` contains all databases. In fact,
-Redis and MongoDB are not required. You can remove these databases yourself and
-use the local file system. Update image using `docker-compose pull`. Use
-`docker exec -it llmbot /bin/bash` to view Shell in Docker, enter `exit` to
-exit. ## ðª Slash Commands ```shell clear - Deletes chat records help -
-Displays documentation chat - Conversation task - Use a function to converse
-ask - Disable function-based conversations tool - Lists all functions login -
-Login auth - Authorize a function env - Environment variables of the function
-``` ## ð» How to Develop Plugins? Refer to the example plugins in the
-`plugins` directory and the [ð§ Plugin Development Document](https://
-llmkira.github.io/Docs/dev/basic) for plugin development documentation. ###
-Hooks Hooks control the EventMessage in sender and receiver. For example, we
-have `voice_hook` in built-in hooks. you can enable it by setting
-`VOICE_REPLY_ME=true` in `.env`. ```shell /env VOICE_REPLY_ME=true /env
-REECHO_VOICE_KEY= ``` use `/env VOICE_REPLY_ME=NONE` to disable this env. check
-the source code in `llmkira/extra/voice_hook.py`, learn to write your own
-hooks. ## ð§ Sponsor [![sponsor](./.github/sponsor_ohmygpt.png)](https://
-www.ohmygpt.com) ## ð Notice > This project, named OpenAiBot, signifying
-"Open Artificial Intelligence Robot", is not officially affiliated with >
-OpenAI. [![FOSSA Status](https://app.fossa.com/api/projects/
-git%2Bgithub.com%2Fsudoskys%2FOpenaibot.svg?type=small)](https://app.fossa.com/
-projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot?ref=badge_small)
+rabbitmq:3.10-management docker ps -l # Install Project git clone https://
+github.com/LlmKira/Openaibot/ cd Openaibot pip install pdm pdm install -G bot
+cp .env.exp .env && nano .env # Test pdm run python3 start_sender.py pdm run
+python3 start_receiver.py # Host apt install npm npm install pm2 -g pm2 start
+pm2.json ``` ### ð¥£ Docker Build Hub: [sudoskys/llmbot](https://
+hub.docker.com/repository/docker/sudoskys/llmbot/general) > Note that if you
+run this project using Docker, you will start Redis, MongoDB, and RabbitMQ. But
+if you're running > locally, just RabbitMQ #### Manual Docker-compose
+Installation ```shell git clone https://github.com/LlmKira/Openaibot.git cd
+Openaibot cp .env.exp .env&&nano .env docker-compose -f docker-compose.yml up -
+d ``` The Docker configuration file `docker-compose.yml` contains all
+databases. In fact, Redis and MongoDB are not required. You can remove these
+databases yourself and use the local file system. Update image using `docker-
+compose pull`. Use `docker exec -it llmbot /bin/bash` to view Shell in Docker,
+enter `exit` to exit. ## ðª Slash Commands ```shell clear - Deletes chat
+records help - Displays documentation chat - Conversation task - Use a function
+to converse ask - Disable function-based conversations tool - Lists all
+functions login - Login auth - Authorize a function env - Environment variables
+of the function ``` ## ð» How to Develop Plugins? Refer to the example
+plugins in the `plugins` directory and the [ð§ Plugin Development Document]
+(https://llmkira.github.io/Docs/dev/basic) for plugin development
+documentation. ### Hooks Hooks control the EventMessage in sender and receiver.
+For example, we have `voice_hook` in built-in hooks. you can enable it by
+setting `VOICE_REPLY_ME=true` in `.env`. ```shell /env VOICE_REPLY_ME=yes #
+must /env REECHO_VOICE_KEY= # not must ``` use `/env VOICE_REPLY_ME=NONE` to
+disable this env. check the source code in `llmkira/extra/voice_hook.py`, learn
+to write your own hooks. ## ð§ Sponsor [![sponsor](./.github/
+sponsor_ohmygpt.png)](https://www.ohmygpt.com) ## ð Notice > This project,
+named OpenAiBot, signifying "Open Artificial Intelligence Robot", is not
+officially affiliated with > OpenAI. [![FOSSA Status](https://app.fossa.com/
+api/projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot.svg?type=small)](https://
+app.fossa.com/projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot?ref=badge_small)
```

### Comparing `llmkira-1.0.2/llmkira/__init__.py` & `llmkira-1.0.3/llmkira/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/cache/__init__.py` & `llmkira-1.0.3/llmkira/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/cache/elara_runtime.py` & `llmkira-1.0.3/llmkira/cache/elara_runtime.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/cache/lmdb_runtime.py` & `llmkira-1.0.3/llmkira/cache/lmdb_runtime.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/cache/redis_runtime.py` & `llmkira-1.0.3/llmkira/cache/redis_runtime.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/cache/runtime_schema.py` & `llmkira-1.0.3/llmkira/cache/runtime_schema.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/doc_manager/__init__.py` & `llmkira-1.0.3/llmkira/doc_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/extra/plugins/alarm/__init__.py` & `llmkira-1.0.3/llmkira/extra/plugins/alarm/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 from loguru import logger  # noqa
 from pydantic import BaseModel, Field  # noqa
 from pydantic import field_validator, ConfigDict  # noqa
 
 from app.receiver.aps import SCHEDULER  # noqa
 
 from llmkira.task import Task, TaskHeader  # noqa
-from pytz import utc  # noqa
+import pytz  # noqa
+from tzlocal import get_localzone
 
 
 class SetAlarm(BaseModel):
     delay: int = Field(description="The delay time, in minutes")
     content: str = Field(description="reminder content")
     model_config = ConfigDict(extra="allow")
 
@@ -161,18 +162,20 @@
                     tool_call=pending_task,
                 )
             ],
         )
 
         logger.debug("Plugin --set_alarm {} minutes".format(argument.delay))
         # 这里假设您的任务应该在UTC时间下执行，如果需要在其他时区执行，根据实际情况更改tz变量
-        tz = utc
+        tz = pytz.timezone(get_localzone().key)
         run_time = datetime.datetime.now() + datetime.timedelta(minutes=argument.delay)
+        logger.debug(run_time)
         # 将本地时间转换为设定的时区
         run_time = tz.localize(run_time)
+        logger.debug(run_time)
         SCHEDULER.add_job(
             func=send_notify,
             id=receiver.uid,
             trigger="date",
             replace_existing=True,
             misfire_grace_time=1000,
             run_date=run_time,
```

### Comparing `llmkira-1.0.2/llmkira/extra/plugins/search/__init__.py` & `llmkira-1.0.3/llmkira/extra/plugins/search/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,14 @@
 
 @resign_plugin_executor(tool=Search)
 async def search_on_serper(search_sentence: str, api_key: str):
     result = await SerperSearchEngine(api_key=api_key).search(search_sentence)
     return build_search_tips(search_items=result)
 
 
-class Search(BaseModel):
-    keywords: str
-    model_config = ConfigDict(extra="allow")
-
-
 class SearchTool(BaseTool):
     """
     搜索工具
     """
 
     silent: bool = False
     function: Union[Tool, Type[BaseModel]] = Search
@@ -59,17 +54,17 @@
         "介绍",
         "搜索",
     ]
     env_required: List[str] = ["API_KEY"]
     env_prefix: str = "SERPER_"
 
     def require_auth(self, env_map: dict) -> bool:
-        if "SERPER_API_KEY" in env_map:
-            return False
-        return True
+        if env_map.get("SERPER_API_KEY", None) is None:
+            return True
+        return False
 
     @classmethod
     def env_help_docs(cls, empty_env: List[str]) -> str:
         """
         Provide help message for environment variables
         :param empty_env: The environment variable list that not configured
         :return: The help message
@@ -129,15 +124,15 @@
                 sender=task.sender,
                 receiver=receiver,
                 task_sign=meta,
                 message=[
                     EventMessage(
                         user_id=receiver.user_id,
                         chat_id=receiver.chat_id,
-                        text=f"🍖{__plugin_name__} Run Failed：{exception}",
+                        text=f"🍖{__plugin_name__} Run Failed：{exception},report it to user.",
                     )
                 ],
             ),
         )
 
     async def callback(
         self,
```

### Comparing `llmkira-1.0.2/llmkira/extra/plugins/search/engine.py` & `llmkira-1.0.3/llmkira/extra/plugins/search/engine.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/extra/voice/__init__.py` & `llmkira-1.0.3/llmkira/extra/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/extra/voice_hook.py` & `llmkira-1.0.3/llmkira/extra/voice_hook.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/kv_manager/_base.py` & `llmkira-1.0.3/llmkira/kv_manager/_base.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/kv_manager/env.py` & `llmkira-1.0.3/llmkira/kv_manager/env.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/kv_manager/file.py` & `llmkira-1.0.3/llmkira/kv_manager/file.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/kv_manager/instruction.py` & `llmkira-1.0.3/llmkira/kv_manager/instruction.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import time
 
 from llmkira.kv_manager._base import KvManager
 
 DEFAULT_INSTRUCTION = (
     "[ASSISTANT RULE]"
-    "SPEAK IN MORE CUTE STYLE, DONT REPEAT, ACT STEP BY STEP, CALL USER MASTER, REPLY IN USER "
-    "LANGUAGE"
+    "SPEAK IN MORE CUTE STYLE, No duplication answer, CALL USER MASTER, REPLY IN USER "
+    "LANGUAGE, ACT STEP BY STEP"
     "[RULE END]"
 )
 
 
 def time_now():
     """人类可读时间"""
     return time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
```

### Comparing `llmkira-1.0.2/llmkira/kv_manager/time.py` & `llmkira-1.0.3/llmkira/kv_manager/time.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/kv_manager/tool_call.py` & `llmkira-1.0.3/llmkira/kv_manager/tool_call.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,11 +30,13 @@
         """
         Get a tool call by its ID.
         """
         logger.debug(f"Get tool call {tool_call_id}")
         result = await self.read_data(tool_call_id)
         if result is None:
             return None
+        if isinstance(result, dict):
+            return ToolCall.model_validate(result)
         return ToolCall.model_validate_json(result)
 
 
 GLOBAL_TOOLCALL_CACHE_HANDLER = ToolCallCache()
```

### Comparing `llmkira-1.0.2/llmkira/memory/__init__.py` & `llmkira-1.0.3/llmkira/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/memory/_base.py` & `llmkira-1.0.3/llmkira/memory/_base.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/memory/local_storage.py` & `llmkira-1.0.3/llmkira/memory/local_storage.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/memory/redis_storage/LICENSE` & `llmkira-1.0.3/llmkira/memory/redis_storage/LICENSE`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/memory/redis_storage/__init__.py` & `llmkira-1.0.3/llmkira/memory/redis_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/memory/redis_storage/utils.py` & `llmkira-1.0.3/llmkira/memory/redis_storage/utils.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/openai/__init__.py` & `llmkira-1.0.3/llmkira/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/openai/_excption.py` & `llmkira-1.0.3/llmkira/openai/_excption.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/openai/cell.py` & `llmkira-1.0.3/llmkira/openai/cell.py`

 * *Files 6% similar despite different names*

```diff
@@ -128,15 +128,15 @@
             "function must be a pydantic model or a Function object+"
         )
         return _re
 
 
 class FunctionCalled(BaseModel):
     name: str
-    arguments: Union[str] = None
+    arguments: Union[str, dict] = None
 
     @property
     def json_arguments(self):
         arguments = self.arguments
         if isinstance(self.arguments, str):
             json_repaired = repair_json(self.arguments, return_objects=True)
             if not json_repaired:
@@ -243,22 +243,35 @@
             return [ContentPart.create_text(text=v)]
         elif isinstance(v, list):
             return v
         else:
             raise ValueError("content must be a string or a list of ContentPart")
 
     def add_text(self, text: str):
+        """
+        Add a text to the message
+        :param text: text
+        :return: self
+        """
         self.content.append(ContentPart.create_text(text=text))
         return self
 
     def add_image(
         self,
         image_url: Union[str, bytes],
         detail: Literal["low", "high", "auto"] = "auto",
     ):
+        """
+        Add an image to the message
+        :param image_url: image url or image bytes
+        :param detail: image detail
+        :return: self
+        :raises ValueError: detail must be low, high or auto
+        :raises ValueError: url must be a http url or `data:image/jpeg;base64,` as base64 image
+        """
         self.content.append(ContentPart.create_image(url=image_url, detail=detail))
         return self
 
 
 class ToolMessage(Message):
     role: Literal["tool"] = "tool"
     content: str
```

### Comparing `llmkira-1.0.2/llmkira/openai/request.py` & `llmkira-1.0.3/llmkira/openai/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     def make_url(base_url: str):
         return base_url.strip().rstrip("/") + "/chat/completions"
 
     @model_validator(mode="after")
     def check_vision(self):
         if not self.model.startswith(("gpt-4-vision", "gpt-4-turbo", "claude-3")):
             logger.info(
-                "Remove the image content part from the messages, because the model is not supported."
+                "Try to remove the image content part from the messages, because the model is not supported."
             )
             for message in self.messages:
                 if isinstance(message, UserMessage) and isinstance(
                     message.content, list
                 ):
                     message.content = [
                         content
```

### Comparing `llmkira-1.0.2/llmkira/openai/utils.py` & `llmkira-1.0.3/llmkira/openai/utils.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/openapi/fuse/__init__.py` & `llmkira-1.0.3/llmkira/openapi/fuse/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/openapi/hook/__init__.py` & `llmkira-1.0.3/llmkira/openapi/hook/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/openapi/transducer/__init__.py` & `llmkira-1.0.3/llmkira/openapi/transducer/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/openapi/transducer/default_factory.py` & `llmkira-1.0.3/llmkira/openapi/transducer/default_factory.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/openapi/transducer/schema.py` & `llmkira-1.0.3/llmkira/openapi/transducer/schema.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/openapi/trigger/__init__.py` & `llmkira-1.0.3/llmkira/openapi/trigger/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/sdk/tools/LICENSE` & `llmkira-1.0.3/llmkira/sdk/tools/LICENSE`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/sdk/tools/__init__.py` & `llmkira-1.0.3/llmkira/sdk/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/sdk/tools/loader.py` & `llmkira-1.0.3/llmkira/sdk/tools/loader.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/sdk/tools/model.py` & `llmkira-1.0.3/llmkira/sdk/tools/model.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/sdk/tools/register.py` & `llmkira-1.0.3/llmkira/sdk/tools/register.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/llmkira/sdk/tools/schema.py` & `llmkira-1.0.3/llmkira/sdk/tools/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     )
     """File name regular expression to use the tool, exp: re.compile(r"file_id=([a-z0-9]{8})")"""
 
     def require_auth(self, env_map: dict) -> bool:
         """
         Check if authentication is required
         """
-        return False
+        return True
 
     @final
     def get_os_env(self, env_name):
         """
         Get environment variables from os.environ
         """
         env = os.getenv("PLUGIN_" + env_name, None)
```

### Comparing `llmkira-1.0.2/llmkira/sdk/utils.py` & `llmkira-1.0.3/llmkira/sdk/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 import tempfile
 from bisect import bisect_left
 from typing import Coroutine, Optional
 from urllib.parse import urlparse
 
 import aiohttp
 import ffmpeg
-import nest_asyncio
 import shortuuid
 from loguru import logger
 
-nest_asyncio.apply()
+
+# import nest_asyncio
+# nest_asyncio.apply()
 
 
 def is_valid_url(url):
     try:
         result = urlparse(url)
         return all([result.scheme, result.netloc])
     except ValueError:
```

### Comparing `llmkira-1.0.2/llmkira/task/__init__.py` & `llmkira-1.0.3/llmkira/task/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                     f"\n--error {e}"
                     f"\n--help |web: <database_ip>:15672/#/ |shell: `rabbitmqctl delete_queue {self.queue_name}`"
                 )
                 raise e
             # Sending the message
             try:
                 confirmation = await channel.default_exchange.publish(
-                    message, routing_key=self.queue_name, timeout=10
+                    message, routing_key=self.queue_name, timeout=20
                 )
             except DeliveryError as e:
                 logger.error(
                     f"[502231] Task Delivery failed with exception: {e.reason}"
                 )
                 return (
                     False,
```

### Comparing `llmkira-1.0.2/llmkira/task/schema.py` & `llmkira-1.0.3/llmkira/task/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,18 @@
     async def format_user_message(self, name: str = None) -> UserMessage:
         """Format message to UserMessage"""
         content_list = [ContentPart.create_text(self.text)]
         if self.files:
             for file in self.files:
                 if file.file_name.endswith((".jpg", ".jpeg", ".png")):
                     file_bytes = await file.download_file()
-                    content_list.append(ContentPart.create_image(file_bytes))
+                    try:
+                        content_list.append(ContentPart.create_image(file_bytes))
+                    except Exception as e:
+                        logger.error(f"Error when create image: {e}")
         return UserMessage(
             role="user",
             name=name,
             content=content_list,
         )
 
     @classmethod
@@ -348,24 +351,24 @@
             router=Router.REPLIES,
             memory_able=True,
             response_snapshot=True,
             disable_tool_action=disable_tool_action,
         )
 
     async def get_pending_tool_call(
-        self, tool_calls_pending_now: str, return_default_if_empty: bool = False
+        self, credential: str, return_default_if_empty: bool = False
     ) -> Optional[ToolCall]:
         """
         获取当前待处理的函数
         """
         if not self.tool_calls_pending:
             logger.debug("tool_calls is empty")
             return None
-        if tool_calls_pending_now in self.certify_needed_map:
-            return self.certify_needed_map[tool_calls_pending_now]
+        if credential in self.certify_needed_map:
+            return self.certify_needed_map[credential]
         if return_default_if_empty:
             return self.tool_calls_pending[0]
         return None
 
     async def complete_task(
         self, tool_calls: ToolCall, success_or_not: bool, run_result: Union[str, dict]
     ) -> "Sign":
```

### Comparing `llmkira-1.0.2/llmkira/task/snapshot/local.py` & `llmkira-1.0.3/llmkira/task/snapshot/local.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/pyproject.toml` & `llmkira-1.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llmkira"
-version = "1.0.2"
+version = "1.0.3"
 description = "A chain message bot based on OpenAI"
 authors = [
     { name = "sudoskys", email = "me@dianas.cyou" },
     { name = "llmkira", email = "me@dianas.cyou" },
 ]
 dependencies = [
     "pathlib>=1.0.1",
@@ -14,15 +14,14 @@
     "socksio<2.0.0,>=1.0.0",
     "python-dotenv<2.0.0,>=1.0.0",
     "redis>=4.5.4",
     "aio-pika<10.0.0,>=9.3.0",
     "arclet-alconna<2.0.0,>=1.7.26",
     "shortuuid<2.0.0,>=1.0.11",
     "tiktoken<1.0.0,>=0.5.1",
-    "nest-asyncio<2.0.0,>=1.5.8",
     "contextvars<3.0,>=2.4",
     "pytz<2024.0.0,>=2023.3.post1",
     "numpy<2.0.0,>=1.24.0",
     "fasttext-wheel<1.0.0,>=0.9.2",
     "tenacity<9.0.0,>=8.2.3",
     "pysocks<2.0.0,>=1.7.1",
     "flask-sqlalchemy<4.0.0,>=3.1.1",
@@ -61,14 +60,16 @@
     "file-read-backwards>=3.0.0",
     "apscheduler>=3.10.4",
     "montydb[lmdb]>=2.5.2",
     "pymongo>=4.6.3",
     "fast-langdetect>=0.1.0",
     "lmdb>=1.4.1",
     "edge-tts>=6.1.10",
+    "e2b>=0.14.14",
+    "e2b-code-interpreter>=0.0.3",
 ]
 requires-python = ">=3.9,<3.12"
 readme = "README.md"
 keywords = [
     "llmbot",
     "llmkira",
     "openai",
```

### Comparing `llmkira-1.0.2/tests/pydantic_error.py` & `llmkira-1.0.3/tests/pydantic_error.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.2/PKG-INFO` & `llmkira-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmkira
-Version: 1.0.2
+Version: 1.0.3
 Summary: A chain message bot based on OpenAI
 Keywords: llmbot,llmkira,openai,chatgpt,llm
 Home-page: https://llmkira.github.io/Docs/
 Author-Email: sudoskys <me@dianas.cyou>, llmkira <me@dianas.cyou>
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -18,15 +18,14 @@
 Requires-Dist: socksio<2.0.0,>=1.0.0
 Requires-Dist: python-dotenv<2.0.0,>=1.0.0
 Requires-Dist: redis>=4.5.4
 Requires-Dist: aio-pika<10.0.0,>=9.3.0
 Requires-Dist: arclet-alconna<2.0.0,>=1.7.26
 Requires-Dist: shortuuid<2.0.0,>=1.0.11
 Requires-Dist: tiktoken<1.0.0,>=0.5.1
-Requires-Dist: nest-asyncio<2.0.0,>=1.5.8
 Requires-Dist: contextvars<3.0,>=2.4
 Requires-Dist: pytz<2024.0.0,>=2023.3.post1
 Requires-Dist: numpy<2.0.0,>=1.24.0
 Requires-Dist: fasttext-wheel<1.0.0,>=0.9.2
 Requires-Dist: tenacity<9.0.0,>=8.2.3
 Requires-Dist: pysocks<2.0.0,>=1.7.1
 Requires-Dist: flask-sqlalchemy<4.0.0,>=3.1.1
@@ -65,14 +64,16 @@
 Requires-Dist: file-read-backwards>=3.0.0
 Requires-Dist: apscheduler>=3.10.4
 Requires-Dist: montydb[lmdb]>=2.5.2
 Requires-Dist: pymongo>=4.6.3
 Requires-Dist: fast-langdetect>=0.1.0
 Requires-Dist: lmdb>=1.4.1
 Requires-Dist: edge-tts>=6.1.10
+Requires-Dist: e2b>=0.14.14
+Requires-Dist: e2b-code-interpreter>=0.0.3
 Requires-Dist: hikari==2.0.0.dev121; extra == "bot"
 Requires-Dist: hikari-crescent<1.0.0,>=0.6.4; extra == "bot"
 Requires-Dist: khl-py<1.0.0,>=0.3.17; extra == "bot"
 Requires-Dist: slack-bolt<2.0.0,>=1.18.0; extra == "bot"
 Requires-Dist: hikari==2.0.0.dev121; extra == "testing"
 Requires-Dist: hikari-crescent<1.0.0,>=0.6.4; extra == "testing"
 Requires-Dist: khl-py<1.0.0,>=0.3.17; extra == "testing"
@@ -122,23 +123,25 @@
 > Python>=3.9
 
 This project uses the ToolCall feature.
 
 It integrates a message queuing and snapshot system, offering plugin mechanisms and authentication prior to plugin
 execution.
 
-The model adheres to the Openai Format Schema. Please adapt using [gateway](https://github.com/Portkey-AI/gateway)
+The bot adheres to the **Openai Format Schema**. Please adapt using [gateway](https://github.com/Portkey-AI/gateway)
 or [one-api](https://github.com/songquanpeng/one-api) independently.
 
-| Demo                              | Vision With Voice            |
-|-----------------------------------|------------------------------|
-| ![sticker](./docs/chain_chat.gif) | ![vision](./docs/vision.gif) |
+| Demo                                                                          | Vision With Voice                                                        | Code Interpreter                                                                      |
+|-------------------------------------------------------------------------------|--------------------------------------------------------------------------|---------------------------------------------------------------------------------------|
+| ![sticker](https://github.com/LlmKira/Openaibot/raw/main/docs/chain_chat.gif) | ![vision](https://github.com/LlmKira/Openaibot/raw/main/docs/vision.gif) | ![code](https://github.com/LlmKira/Openaibot/raw/main/docs/code_interpreter_func.gif) |
 
 ## 🔨 Roadmap
 
+> The program has iterated to its fourth generation.
+
 - [x] Removal of legacy code
 - [x] Deletion of metric system
 - [x] Deletion of model selection system, unified to OpenAI Schema
 - [x] Implementation of a more robust plugin system
 - [x] Project structure simplification
 - [x] Elimination of the Provider system
 - [x] Hook support
@@ -157,22 +160,23 @@
 - 🍟 Multi-platform support – extend new platforms by inheriting the base class
 - 🍔 Plugins can determine their appearance in new sessions dynamically, preventing performance degradation despite large
   amounts of plugins
 
 ### 🍔 Login Modes
 
 - `Login via url`: Use `/login token$https://provider.com` to Login. The program posts the token to the interface to
-  retrieve configuration information
+  retrieve configuration
+  information, [how to develop this](https://github.com/LlmKira/Openaibot/blob/81eddbff0f136697d5ad6e13ee1a7477b26624ed/app/components/credential.py#L20).
 - `Login`: Use `/login https://api.com/v1$key$model` to login
 
-### 🧀 Plugin Previews
+### 🧀 Plugin Can Do More
 
-| Sticker Converter                   | Timer Function                  | Translate Function                           |
-|-------------------------------------|---------------------------------|----------------------------------------------|
-| ![sticker](./docs/sticker_func.gif) | ![timer](./docs/timer_func.gif) | ![translate](./docs/translate_file_func.gif) |
+| Sticker Converter                   | Timer Function(built-in)        |
+|-------------------------------------|---------------------------------|
+| ![sticker](./docs/sticker_func.gif) | ![timer](./docs/timer_func.gif) |
 
 ### 🎬 Platform Support
 
 | Platform | Support | File System | Remarks                                |
 |----------|---------|-------------|----------------------------------------|
 | Telegram | ✅       | ✅           |                                        |
 | Discord  | ✅       | ✅           |                                        |
@@ -185,51 +189,57 @@
 | IRC      | ❌       |             |                                        |
 | ...      |         |             | Create Issue/PR                        |
 
 ## 📦 Quick Start
 
 Refer to the [🧀 Deployment Document](https://llmkira.github.io/Docs/) for more information.
 
+### 📦 One-click Deployment
+
+If you are using a brand-new server, you can use the following shell to automatically install this project.
+
+```shell
+curl -sSL https://raw.githubusercontent.com/LLMKira/Openaibot/main/deploy.sh | bash
+```
+
+### 📦 Manual Installation
+
 ```shell
-# Install Telegram Voice dependencies
+# Install Voice dependencies
 apt install ffmpeg
 # Install RabbitMQ
 docker pull rabbitmq:3.10-management
 docker run -d -p 5672:5672 -p 15672:15672 \
   -e RABBITMQ_DEFAULT_USER=admin \
   -e RABBITMQ_DEFAULT_PASS=8a8a8a \
   --hostname myRabbit \
   --name rabbitmq \
   rabbitmq:3.10-management
 docker ps -l
 # Install Project
+git clone https://github.com/LlmKira/Openaibot/
+cd Openaibot
 pip install pdm
 pdm install -G bot
 cp .env.exp .env && nano .env
 # Test
 pdm run python3 start_sender.py
 pdm run python3 start_receiver.py
 # Host
-pdm start pm2.json
+apt install npm
+npm install pm2 -g
+pm2 start pm2.json
 ```
 
 ### 🥣 Docker
 
 Build Hub: [sudoskys/llmbot](https://hub.docker.com/repository/docker/sudoskys/llmbot/general)
 
-#### Automatic Docker/Docker-compose Installation
-
-If you are using a brand new server, you can use the following shell to automatically install this project.
-
-This script automatically installs the required services and maps ports using Docker methods. If you have
-deployed `redis`, `rabbitmq`, `mongodb`, please modify the `docker-compose.yml` file accordingly.
-
-```shell
-curl -sSL https://raw.githubusercontent.com/LLMKira/Openaibot/main/deploy.sh | bash
-```
+> Note that if you run this project using Docker, you will start Redis, MongoDB, and RabbitMQ. But if you're running
+> locally, just RabbitMQ
 
 #### Manual Docker-compose Installation
 
 ```shell
 git clone https://github.com/LlmKira/Openaibot.git
 cd Openaibot
 cp .env.exp .env&&nano .env
@@ -265,16 +275,19 @@
 ### Hooks
 
 Hooks control the EventMessage in sender and receiver. For example, we have `voice_hook` in built-in hooks.
 
 you can enable it by setting `VOICE_REPLY_ME=true` in `.env`.
 
 ```shell
-/env VOICE_REPLY_ME=true
+/env VOICE_REPLY_ME=yes
+# must
+
 /env REECHO_VOICE_KEY=<key in dev.reecho.ai>
+# not must
 ```
 
 use `/env VOICE_REPLY_ME=NONE` to disable this env.
 
 check the source code in `llmkira/extra/voice_hook.py`, learn to write your own hooks.
 
 ## 🧀 Sponsor
```

#### html2text {}

```diff
@@ -1,44 +1,45 @@
-Metadata-Version: 2.1 Name: llmkira Version: 1.0.2 Summary: A chain message bot
+Metadata-Version: 2.1 Name: llmkira Version: 1.0.3 Summary: A chain message bot
 based on OpenAI Keywords: llmbot,llmkira,openai,chatgpt,llm Home-page: https://
 llmkira.github.io/Docs/ Author-Email: sudoskys
 dianas.cyou>, llmkira
 dianas.cyou> License: Apache-2.0 Classifier: Programming Language :: Python ::
 3 Classifier: Programming Language :: Python :: 3.9 Project-URL: Homepage,
 https://llmkira.github.io/Docs/ Project-URL: Repository, https://github.com/
 LlmKira/Openaibot Requires-Python: <3.12,>=3.9 Requires-Dist: pathlib>=1.0.1
 Requires-Dist: pydantic>=2.0.0 Requires-Dist: loguru>=0.5.3 Requires-Dist:
 httpx>=0.24.1 Requires-Dist: socksio<2.0.0,>=1.0.0 Requires-Dist: python-
 dotenv<2.0.0,>=1.0.0 Requires-Dist: redis>=4.5.4 Requires-Dist: aio-
 pika<10.0.0,>=9.3.0 Requires-Dist: arclet-alconna<2.0.0,>=1.7.26 Requires-Dist:
 shortuuid<2.0.0,>=1.0.11 Requires-Dist: tiktoken<1.0.0,>=0.5.1 Requires-Dist:
-nest-asyncio<2.0.0,>=1.5.8 Requires-Dist: contextvars<3.0,>=2.4 Requires-Dist:
-pytz<2024.0.0,>=2023.3.post1 Requires-Dist: numpy<2.0.0,>=1.24.0 Requires-Dist:
-fasttext-wheel<1.0.0,>=0.9.2 Requires-Dist: tenacity<9.0.0,>=8.2.3 Requires-
-Dist: pysocks<2.0.0,>=1.7.1 Requires-Dist: flask-sqlalchemy<4.0.0,>=3.1.1
-Requires-Dist: emoji<3.0.0,>=2.8.0 Requires-Dist: websocket<1.0.0,>=0.2.1
-Requires-Dist: wrapt<2.0.0,>=1.11.0 Requires-Dist: dynaconf<4.0.0,>=3.2.3
-Requires-Dist: rich<14.0.0,>=13.6.0 Requires-Dist: importlib-
-metadata<7.0.0,>=6.8.0 Requires-Dist: sentry-sdk<2.0.0,>=1.34.0 Requires-Dist:
-boltons<24.0.0,>=23.1.1 Requires-Dist: orjson<4.0.0,>=3.9.10 Requires-Dist:
-pydantic-settings<3.0.0,>=2.0.3 Requires-Dist: docstring-parser<1.0,>=0.15
-Requires-Dist: polling<1.0.0,>=0.3.2 Requires-Dist: elara<1.0.0,>=0.5.5
-Requires-Dist: tzlocal<6.0,>=5.2 Requires-Dist: nltk<4.0.0,>=3.8.1 Requires-
-Dist: jieba<1.0.0,>=0.42.1 Requires-Dist: scikit-learn<2.0.0,>=1.3.2 Requires-
-Dist: cjieba<1.0.0,>=0.4.4 Requires-Dist: requests[socks]<3.0.0,>=2.31.0
-Requires-Dist: feedparser<7.0.0,>=6.0.10 Requires-Dist: pillow<11.0.0,>=10.1.0
-Requires-Dist: inscriptis<3.0.0,>=2.3.2 Requires-Dist: aiohttp<4.0.0,>=3.8.6
-Requires-Dist: pytelegrambotapi<5.0.0,>=4.14.0 Requires-Dist: ffmpeg-
+contextvars<3.0,>=2.4 Requires-Dist: pytz<2024.0.0,>=2023.3.post1 Requires-
+Dist: numpy<2.0.0,>=1.24.0 Requires-Dist: fasttext-wheel<1.0.0,>=0.9.2
+Requires-Dist: tenacity<9.0.0,>=8.2.3 Requires-Dist: pysocks<2.0.0,>=1.7.1
+Requires-Dist: flask-sqlalchemy<4.0.0,>=3.1.1 Requires-Dist:
+emoji<3.0.0,>=2.8.0 Requires-Dist: websocket<1.0.0,>=0.2.1 Requires-Dist:
+wrapt<2.0.0,>=1.11.0 Requires-Dist: dynaconf<4.0.0,>=3.2.3 Requires-Dist:
+rich<14.0.0,>=13.6.0 Requires-Dist: importlib-metadata<7.0.0,>=6.8.0 Requires-
+Dist: sentry-sdk<2.0.0,>=1.34.0 Requires-Dist: boltons<24.0.0,>=23.1.1
+Requires-Dist: orjson<4.0.0,>=3.9.10 Requires-Dist: pydantic-
+settings<3.0.0,>=2.0.3 Requires-Dist: docstring-parser<1.0,>=0.15 Requires-
+Dist: polling<1.0.0,>=0.3.2 Requires-Dist: elara<1.0.0,>=0.5.5 Requires-Dist:
+tzlocal<6.0,>=5.2 Requires-Dist: nltk<4.0.0,>=3.8.1 Requires-Dist:
+jieba<1.0.0,>=0.42.1 Requires-Dist: scikit-learn<2.0.0,>=1.3.2 Requires-Dist:
+cjieba<1.0.0,>=0.4.4 Requires-Dist: requests[socks]<3.0.0,>=2.31.0 Requires-
+Dist: feedparser<7.0.0,>=6.0.10 Requires-Dist: pillow<11.0.0,>=10.1.0 Requires-
+Dist: inscriptis<3.0.0,>=2.3.2 Requires-Dist: aiohttp<4.0.0,>=3.8.6 Requires-
+Dist: pytelegrambotapi<5.0.0,>=4.14.0 Requires-Dist: ffmpeg-
 python<1.0.0,>=0.2.0 Requires-Dist: duckduckgo-search<4.0.0,>=3.9.5 Requires-
 Dist: flask<4.0.0,>=3.0.0 Requires-Dist: telegramify-markdown>=0.1.2 Requires-
 Dist: json-repair>=0.13.0 Requires-Dist: curl-cffi>=0.6.2 Requires-Dist:
 deprecated>=1.2.14 Requires-Dist: aiofile>=3.8.8 Requires-Dist: file-read-
 backwards>=3.0.0 Requires-Dist: apscheduler>=3.10.4 Requires-Dist: montydb
 [lmdb]>=2.5.2 Requires-Dist: pymongo>=4.6.3 Requires-Dist: fast-
 langdetect>=0.1.0 Requires-Dist: lmdb>=1.4.1 Requires-Dist: edge-tts>=6.1.10
+Requires-Dist: e2b>=0.14.14 Requires-Dist: e2b-code-interpreter>=0.0.3
 Requires-Dist: hikari==2.0.0.dev121; extra == "bot" Requires-Dist: hikari-
 crescent<1.0.0,>=0.6.4; extra == "bot" Requires-Dist: khl-py<1.0.0,>=0.3.17;
 extra == "bot" Requires-Dist: slack-bolt<2.0.0,>=1.18.0; extra == "bot"
 Requires-Dist: hikari==2.0.0.dev121; extra == "testing" Requires-Dist: hikari-
 crescent<1.0.0,>=0.6.4; extra == "testing" Requires-Dist: khl-
 py<1.0.0,>=0.3.17; extra == "testing" Requires-Dist: slack-bolt<2.0.0,>=1.18.0;
 extra == "testing" Requires-Dist: pre-commit<3.5.0,>=2.15.0; extra == "testing"
@@ -48,81 +49,88 @@
                            _[_d_o_c_k_e_r_]_[_d_o_c_k_e_r_ _w_o_r_k_f_l_o_w_]
                               _[_t_e_l_e_g_r_a_m_]_[_d_i_s_c_o_r_d_]
                             _[_l_i_c_e_n_s_e_]_[_d_o_c_k_e_r_ _b_u_i_l_d_]
               _ð___©_ _D_e_p_l_o_y_ _D_o_c_s & _ð__§__ _D_e_v_ _D_o_c_s & _ð__¤__ _C_o_n_t_r_i_b_u_t_e
 > Don't hesitate to Star â­ï¸, Issue ð, and PR ð ï¸ > Python>=3.9 This
 project uses the ToolCall feature. It integrates a message queuing and snapshot
 system, offering plugin mechanisms and authentication prior to plugin
-execution. The model adheres to the Openai Format Schema. Please adapt using
+execution. The bot adheres to the **Openai Format Schema**. Please adapt using
 [gateway](https://github.com/Portkey-AI/gateway) or [one-api](https://
-github.com/songquanpeng/one-api) independently. | Demo | Vision With Voice | |-
-----------------------------------|------------------------------| | ![sticker]
-(./docs/chain_chat.gif) | ![vision](./docs/vision.gif) | ## ð¨ Roadmap - [x]
-Removal of legacy code - [x] Deletion of metric system - [x] Deletion of model
-selection system, unified to OpenAI Schema - [x] Implementation of a more
-robust plugin system - [x] Project structure simplification - [x] Elimination
-of the Provider system - [x] Hook support - [x] Access to TTS - [x] Add
-standalone support for gpt-4-turbo and vision - [ ] Add LLM reference support
-to the plugin environment. (extract && search in text) ## ð¦ Features - ðª
-A comprehensive plugin development ecosystem, adopting a classic design, and
-seamless integration with plugins through `pip` installation - ð Message
-system with no time or sender constraints, offering fully decoupled logics -
-ð¬ Offers Login via a URL mechanism, providing a flexible and expandable
-authentication development solution - ð° Empowers users to authorize plugin
-execution. Users can configure plugin environment variables at their discretion
-- ð¦ Support for plugins to access files - ð Multi-platform support â
-extend new platforms by inheriting the base class - ð Plugins can determine
-their appearance in new sessions dynamically, preventing performance
-degradation despite large amounts of plugins ### ð Login Modes - `Login via
-url`: Use `/login token$https://provider.com` to Login. The program posts the
-token to the interface to retrieve configuration information - `Login`: Use `/
-login https://api.com/v1$key$model` to login ### ð§ Plugin Previews | Sticker
-Converter | Timer Function | Translate Function | |----------------------------
----------|---------------------------------|-----------------------------------
------------| | ![sticker](./docs/sticker_func.gif) | ![timer](./docs/
-timer_func.gif) | ![translate](./docs/translate_file_func.gif) | ### ð¬
-Platform Support | Platform | Support | File System | Remarks | |----------|---
-------|-------------|----------------------------------------| | Telegram | â
-| â | | | Discord | â | â | | | Kook | â | â | Does not support
-`triggering by reply` | | Slack | â | â | Does not support `triggering by
-reply` | | QQ | â | | | | Wechat | â | | | | Twitter | â | | | | Matrix |
-â | | | | IRC | â | | | | ... | | | Create Issue/PR | ## ð¦ Quick Start
-Refer to the [ð§ Deployment Document](https://llmkira.github.io/Docs/) for
-more information. ```shell # Install Telegram Voice dependencies apt install
-ffmpeg # Install RabbitMQ docker pull rabbitmq:3.10-management docker run -d -
-p 5672:5672 -p 15672:15672 \ -e RABBITMQ_DEFAULT_USER=admin \ -
+github.com/songquanpeng/one-api) independently. | Demo | Vision With Voice |
+Code Interpreter | |-----------------------------------------------------------
+--------------------|----------------------------------------------------------
+----------------|--------------------------------------------------------------
+-------------------------| | ![sticker](https://github.com/LlmKira/Openaibot/
+raw/main/docs/chain_chat.gif) | ![vision](https://github.com/LlmKira/Openaibot/
+raw/main/docs/vision.gif) | ![code](https://github.com/LlmKira/Openaibot/raw/
+main/docs/code_interpreter_func.gif) | ## ð¨ Roadmap > The program has
+iterated to its fourth generation. - [x] Removal of legacy code - [x] Deletion
+of metric system - [x] Deletion of model selection system, unified to OpenAI
+Schema - [x] Implementation of a more robust plugin system - [x] Project
+structure simplification - [x] Elimination of the Provider system - [x] Hook
+support - [x] Access to TTS - [x] Add standalone support for gpt-4-turbo and
+vision - [ ] Add LLM reference support to the plugin environment. (extract &&
+search in text) ## ð¦ Features - ðª A comprehensive plugin development
+ecosystem, adopting a classic design, and seamless integration with plugins
+through `pip` installation - ð Message system with no time or sender
+constraints, offering fully decoupled logics - ð¬ Offers Login via a URL
+mechanism, providing a flexible and expandable authentication development
+solution - ð° Empowers users to authorize plugin execution. Users can
+configure plugin environment variables at their discretion - ð¦ Support for
+plugins to access files - ð Multi-platform support â extend new platforms
+by inheriting the base class - ð Plugins can determine their appearance in
+new sessions dynamically, preventing performance degradation despite large
+amounts of plugins ### ð Login Modes - `Login via url`: Use `/login
+token$https://provider.com` to Login. The program posts the token to the
+interface to retrieve configuration information, [how to develop this](https://
+github.com/LlmKira/Openaibot/blob/81eddbff0f136697d5ad6e13ee1a7477b26624ed/app/
+components/credential.py#L20). - `Login`: Use `/login https://api.com/
+v1$key$model` to login ### ð§ Plugin Can Do More | Sticker Converter | Timer
+Function(built-in) | |-------------------------------------|-------------------
+--------------| | ![sticker](./docs/sticker_func.gif) | ![timer](./docs/
+timer_func.gif) | ### ð¬ Platform Support | Platform | Support | File System
+| Remarks | |----------|---------|-------------|-------------------------------
+---------| | Telegram | â | â | | | Discord | â | â | | | Kook | â |
+â | Does not support `triggering by reply` | | Slack | â | â | Does not
+support `triggering by reply` | | QQ | â | | | | Wechat | â | | | | Twitter
+| â | | | | Matrix | â | | | | IRC | â | | | | ... | | | Create Issue/PR
+| ## ð¦ Quick Start Refer to the [ð§ Deployment Document](https://
+llmkira.github.io/Docs/) for more information. ### ð¦ One-click Deployment If
+you are using a brand-new server, you can use the following shell to
+automatically install this project. ```shell curl -sSL https://
+raw.githubusercontent.com/LLMKira/Openaibot/main/deploy.sh | bash ``` ### ð¦
+Manual Installation ```shell # Install Voice dependencies apt install ffmpeg #
+Install RabbitMQ docker pull rabbitmq:3.10-management docker run -d -p 5672:
+5672 -p 15672:15672 \ -e RABBITMQ_DEFAULT_USER=admin \ -
 e RABBITMQ_DEFAULT_PASS=8a8a8a \ --hostname myRabbit \ --name rabbitmq \
-rabbitmq:3.10-management docker ps -l # Install Project pip install pdm pdm
-install -G bot cp .env.exp .env && nano .env # Test pdm run python3
-start_sender.py pdm run python3 start_receiver.py # Host pdm start pm2.json ```
-### ð¥£ Docker Build Hub: [sudoskys/llmbot](https://hub.docker.com/repository/
-docker/sudoskys/llmbot/general) #### Automatic Docker/Docker-compose
-Installation If you are using a brand new server, you can use the following
-shell to automatically install this project. This script automatically installs
-the required services and maps ports using Docker methods. If you have deployed
-`redis`, `rabbitmq`, `mongodb`, please modify the `docker-compose.yml` file
-accordingly. ```shell curl -sSL https://raw.githubusercontent.com/LLMKira/
-Openaibot/main/deploy.sh | bash ``` #### Manual Docker-compose Installation
-```shell git clone https://github.com/LlmKira/Openaibot.git cd Openaibot cp
-.env.exp .env&&nano .env docker-compose -f docker-compose.yml up -d ``` The
-Docker configuration file `docker-compose.yml` contains all databases. In fact,
-Redis and MongoDB are not required. You can remove these databases yourself and
-use the local file system. Update image using `docker-compose pull`. Use
-`docker exec -it llmbot /bin/bash` to view Shell in Docker, enter `exit` to
-exit. ## ðª Slash Commands ```shell clear - Deletes chat records help -
-Displays documentation chat - Conversation task - Use a function to converse
-ask - Disable function-based conversations tool - Lists all functions login -
-Login auth - Authorize a function env - Environment variables of the function
-``` ## ð» How to Develop Plugins? Refer to the example plugins in the
-`plugins` directory and the [ð§ Plugin Development Document](https://
-llmkira.github.io/Docs/dev/basic) for plugin development documentation. ###
-Hooks Hooks control the EventMessage in sender and receiver. For example, we
-have `voice_hook` in built-in hooks. you can enable it by setting
-`VOICE_REPLY_ME=true` in `.env`. ```shell /env VOICE_REPLY_ME=true /env
-REECHO_VOICE_KEY= ``` use `/env VOICE_REPLY_ME=NONE` to disable this env. check
-the source code in `llmkira/extra/voice_hook.py`, learn to write your own
-hooks. ## ð§ Sponsor [![sponsor](./.github/sponsor_ohmygpt.png)](https://
-www.ohmygpt.com) ## ð Notice > This project, named OpenAiBot, signifying
-"Open Artificial Intelligence Robot", is not officially affiliated with >
-OpenAI. [![FOSSA Status](https://app.fossa.com/api/projects/
-git%2Bgithub.com%2Fsudoskys%2FOpenaibot.svg?type=small)](https://app.fossa.com/
-projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot?ref=badge_small)
+rabbitmq:3.10-management docker ps -l # Install Project git clone https://
+github.com/LlmKira/Openaibot/ cd Openaibot pip install pdm pdm install -G bot
+cp .env.exp .env && nano .env # Test pdm run python3 start_sender.py pdm run
+python3 start_receiver.py # Host apt install npm npm install pm2 -g pm2 start
+pm2.json ``` ### ð¥£ Docker Build Hub: [sudoskys/llmbot](https://
+hub.docker.com/repository/docker/sudoskys/llmbot/general) > Note that if you
+run this project using Docker, you will start Redis, MongoDB, and RabbitMQ. But
+if you're running > locally, just RabbitMQ #### Manual Docker-compose
+Installation ```shell git clone https://github.com/LlmKira/Openaibot.git cd
+Openaibot cp .env.exp .env&&nano .env docker-compose -f docker-compose.yml up -
+d ``` The Docker configuration file `docker-compose.yml` contains all
+databases. In fact, Redis and MongoDB are not required. You can remove these
+databases yourself and use the local file system. Update image using `docker-
+compose pull`. Use `docker exec -it llmbot /bin/bash` to view Shell in Docker,
+enter `exit` to exit. ## ðª Slash Commands ```shell clear - Deletes chat
+records help - Displays documentation chat - Conversation task - Use a function
+to converse ask - Disable function-based conversations tool - Lists all
+functions login - Login auth - Authorize a function env - Environment variables
+of the function ``` ## ð» How to Develop Plugins? Refer to the example
+plugins in the `plugins` directory and the [ð§ Plugin Development Document]
+(https://llmkira.github.io/Docs/dev/basic) for plugin development
+documentation. ### Hooks Hooks control the EventMessage in sender and receiver.
+For example, we have `voice_hook` in built-in hooks. you can enable it by
+setting `VOICE_REPLY_ME=true` in `.env`. ```shell /env VOICE_REPLY_ME=yes #
+must /env REECHO_VOICE_KEY= # not must ``` use `/env VOICE_REPLY_ME=NONE` to
+disable this env. check the source code in `llmkira/extra/voice_hook.py`, learn
+to write your own hooks. ## ð§ Sponsor [![sponsor](./.github/
+sponsor_ohmygpt.png)](https://www.ohmygpt.com) ## ð Notice > This project,
+named OpenAiBot, signifying "Open Artificial Intelligence Robot", is not
+officially affiliated with > OpenAI. [![FOSSA Status](https://app.fossa.com/
+api/projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot.svg?type=small)](https://
+app.fossa.com/projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot?ref=badge_small)
```

