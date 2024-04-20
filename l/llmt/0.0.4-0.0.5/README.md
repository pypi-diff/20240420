# Comparing `tmp/llmt-0.0.4.tar.gz` & `tmp/llmt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmt-0.0.4.tar", last modified: Sun Apr 14 17:02:26 2024, max compression
+gzip compressed data, was "llmt-0.0.5.tar", last modified: Sat Apr 20 19:31:44 2024, max compression
```

## Comparing `llmt-0.0.4.tar` & `llmt-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:02:26.962675 llmt-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-04-14 17:02:22.000000 llmt-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-14 17:02:26.962675 llmt-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-14 17:02:22.000000 llmt-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:02:26.962675 llmt-0.0.4/llmt/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/assistants.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/json_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/openai_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7263 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/response.txt.j2
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:02:26.962675 llmt-0.0.4/llmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-14 17:02:26.000000 llmt-0.0.4/llmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-14 17:02:26.000000 llmt-0.0.4/llmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 17:02:26.000000 llmt-0.0.4/llmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-14 17:02:26.000000 llmt-0.0.4/llmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-14 17:02:26.000000 llmt-0.0.4/llmt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-14 17:02:22.000000 llmt-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-14 17:02:22.000000 llmt-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 17:02:26.962675 llmt-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:31:44.103417 llmt-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-04-20 19:31:40.000000 llmt-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-20 19:31:44.103417 llmt-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-20 19:31:40.000000 llmt-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:31:44.103417 llmt-0.0.5/llmt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-20 19:31:40.000000 llmt-0.0.5/llmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-20 19:31:40.000000 llmt-0.0.5/llmt/assistants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-20 19:31:40.000000 llmt-0.0.5/llmt/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-20 19:31:40.000000 llmt-0.0.5/llmt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-20 19:31:40.000000 llmt-0.0.5/llmt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-20 19:31:40.000000 llmt-0.0.5/llmt/json_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10292 2024-04-20 19:31:40.000000 llmt-0.0.5/llmt/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-04-20 19:31:40.000000 llmt-0.0.5/llmt/openai_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-04-20 19:31:40.000000 llmt-0.0.5/llmt/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-20 19:31:40.000000 llmt-0.0.5/llmt/response.txt.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-20 19:31:40.000000 llmt-0.0.5/llmt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:31:44.103417 llmt-0.0.5/llmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-20 19:31:44.000000 llmt-0.0.5/llmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-20 19:31:44.000000 llmt-0.0.5/llmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 19:31:44.000000 llmt-0.0.5/llmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-20 19:31:44.000000 llmt-0.0.5/llmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-20 19:31:44.000000 llmt-0.0.5/llmt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-20 19:31:40.000000 llmt-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-20 19:31:40.000000 llmt-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 19:31:44.103417 llmt-0.0.5/setup.cfg
```

### Comparing `llmt-0.0.4/LICENSE` & `llmt-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llmt-0.0.4/PKG-INFO` & `llmt-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: llmt
-Version: 0.0.4
-Summary: Convenient LLM chat wrapper for data pipelines, CI/CD, or personal workspaces.
+Version: 0.0.5
+Summary: LLMT aims to make it easy to programatically connect OpenAI and HuggingFace models to your data pipelines, CI/CD, or personal workspaces.
 Author-email: Artem Golub <artem@outermeasure.com>
 Project-URL: Homepage, https://github.com/omhq/llmt
 Project-URL: Bug Tracker, https://github.com/omhq/llmt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai==1.14.1
+Requires-Dist: requests==2.31.0
 Requires-Dist: watchdog==4.0.0
 Requires-Dist: halo==0.0.31
 Requires-Dist: inquirer==3.2.4
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: docstring-parser==0.16
 Requires-Dist: typing-extensions==4.10.0
@@ -25,42 +26,43 @@
 Requires-Dist: SQLAlchemy==2.0.28
 Requires-Dist: pydantic==2.6.4
 
 # LLMT
 
 [![PyPI version](https://badge.fury.io/py/llmt.svg)](https://badge.fury.io/py/llmt)
 
-## Overview
+## What is this good for?
 
-Convenient LLM chat wrapper for data pipelines, CI/CD, or personal workspaces.
+LLMT aims to make it easy to programatically connect OpenAI and HuggingFace models to your data pipelines, CI/CD, or personal workspaces.
 
-Supports local function calling, chat history retention, and can run anywhere. Chat using a terminal, input/output files, or directly through LLMT API.
+Supports function calling, chat and context history retention. Python 3.12 and up.
 
 ### Usage
 
 Use the package in directly in your python code (`pip install llmt`), or as a local workspace running a container to interact with ChatGPT.
 
 ### Module import
 
 ```python
 from llmt import LLMT
 
 
 llmt = LLMT()
 llmt.init_assistant(
-    "dataengineer",
+    "snowflake",
     api_key="...",
     model="gpt-3.5-turbo",
-    assistant_description="You are a data engineer, and a python expert.",)
-llmt.init_functions(["./my_functions.py"])
-llmt.init_chat("single_chat")
-
-response = llmt.run(
-    "What's the result of 22 plus 5 in decimal added to the hexadecimal number A?"
+    assistant_description="You are a snowflake expert. Answer questions briefly in a sentence or less."
 )
+
+llmt.init_functions(["./helper_functions.py"])
+llmt.init_context("snowflake")
+response = llmt.run("generate an example merge dml")
+
+print(response)
 ```
 
 ### Local workspace
 
 Install Docker and make command. Make is not required since you can use docker compose.
 
 - Clone this repo.
```

### Comparing `llmt-0.0.4/README.md` & `llmt-0.0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # LLMT
 
 [![PyPI version](https://badge.fury.io/py/llmt.svg)](https://badge.fury.io/py/llmt)
 
-## Overview
+## What is this good for?
 
-Convenient LLM chat wrapper for data pipelines, CI/CD, or personal workspaces.
+LLMT aims to make it easy to programatically connect OpenAI and HuggingFace models to your data pipelines, CI/CD, or personal workspaces.
 
-Supports local function calling, chat history retention, and can run anywhere. Chat using a terminal, input/output files, or directly through LLMT API.
+Supports function calling, chat and context history retention. Python 3.12 and up.
 
 ### Usage
 
 Use the package in directly in your python code (`pip install llmt`), or as a local workspace running a container to interact with ChatGPT.
 
 ### Module import
 
 ```python
 from llmt import LLMT
 
 
 llmt = LLMT()
 llmt.init_assistant(
-    "dataengineer",
+    "snowflake",
     api_key="...",
     model="gpt-3.5-turbo",
-    assistant_description="You are a data engineer, and a python expert.",)
-llmt.init_functions(["./my_functions.py"])
-llmt.init_chat("single_chat")
-
-response = llmt.run(
-    "What's the result of 22 plus 5 in decimal added to the hexadecimal number A?"
+    assistant_description="You are a snowflake expert. Answer questions briefly in a sentence or less."
 )
+
+llmt.init_functions(["./helper_functions.py"])
+llmt.init_context("snowflake")
+response = llmt.run("generate an example merge dml")
+
+print(response)
 ```
 
 ### Local workspace
 
 Install Docker and make command. Make is not required since you can use docker compose.
 
 - Clone this repo.
```

### Comparing `llmt-0.0.4/llmt/__init__.py` & `llmt-0.0.5/llmt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     OpenAIFunction,
     RawFunctionResult,
     WrapperConfig,
 )
 from .openai_types import FinalResponseMessage, FunctionCall, GenericMessage, Message
 from .parsers import ArgSchemaParser, defargparsers
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 __all__ = [
     "LLMT",
     "OpenAIAssistant",
     "ChatManager",
     "FileManager",
     "prompt_create_chat",
     "prompt_init",
```

### Comparing `llmt-0.0.4/llmt/assistants.py` & `llmt-0.0.5/llmt/assistants.py`

 * *Files identical despite different names*

### Comparing `llmt-0.0.4/llmt/core.py` & `llmt-0.0.5/llmt/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 import os
+import time
 
-from .managers import ChatManager, FileManager, FunctionManager
+from .managers import ChatManager, ContextManager, FileManager, FunctionManager
 from .utils import load_config
 from .assistants import OpenAIAssistant
-from .prompts import prompt_create_chat, prompt_init, ask, ask_once
+from .prompts import prompt_create_chat, prompt_init, ask, ask_once, get_usage_as_string
 
 
 class LLMT:
     def __init__(self, **kwargs):
         self.configs = None
         self.chat = None
         self.assistant = None
         self.file_manager = None
         self.function_manager = None
         self.config_file = kwargs.get("config_file", None)
         self.root_path = kwargs.get("root_path", os.getcwd())
         self.chat_manager = ChatManager(self.root_path)
+        self.context_manager = ContextManager(self.root_path)
 
         if self.config_file:
             self.configs = load_config(self.config_file)
 
         self.init_file_manager()
 
     def get_chats(self):
-        return list(self.chat_manager.list_chats())
+        return list(self.chat_manager.list())
 
     def prompt_create_chat(self):
         return prompt_create_chat()
 
     def init_prompt(self):
         if not self.configs:
             raise ValueError("No configuration file provided.")
 
-        return prompt_init(self.configs["assistants"], (["Create new chat file"] + self.get_chats()))
+        return prompt_init(
+            self.configs["assistants"], (["Create new chat file"] + self.get_chats())
+        )
 
     def find_assistant(self, assistant_name):
         return next(
             (x for x in self.configs["assistants"] if x["name"] == assistant_name),
             None,
         )
 
@@ -60,15 +64,19 @@
             )
 
     def init_functions(self, paths):
         self.function_manager = FunctionManager(paths)
 
     def init_chat(self, chat_name):
         self.chat = chat_name
-        self.chat_manager.init_chat(chat_name)
+        self.chat_manager.create(chat_name)
+
+    def init_context(self, chat_name):
+        self.chat = chat_name
+        self.context_manager.create(chat_name)
 
     def init_file_manager(self, **kwargs):
         if not self.configs:
             input_file = kwargs.get("input_file", None)
             output_file = kwargs.get("output_file", None)
 
         if self.configs:
@@ -80,29 +88,43 @@
 
     def init_first_messages(self):
         if not self.assistant:
             raise ValueError("No assistant initialized.")
         if not self.chat:
             raise ValueError("No chat initialized.")
 
-        if self.chat_manager.list_messages() == 0:
-            self.chat_manager.save_to_chat(
+        if self.context_manager.list_messages() == 0:
+            self.context_manager.save(
                 {"role": "system", "content": self.assistant.description}
             )
 
+    def init_chat_history(self):
+        messages = self.chat_manager.get_history()
+        for message in messages:
+            self.file_manager.prepend_to_output(message)
+
     def run_forever(self):
         self.init_first_messages()
+
+        if self.file_manager:
+            self.init_chat_history()
+
         yield from ask(
             self.chat_manager,
+            self.context_manager,
             self.file_manager,
             self.function_manager,
             self.assistant,
         )
 
-    def run(self, message, functions=None):
+    def run(self, message):
         self.init_first_messages()
+
+        if self.file_manager:
+            self.init_chat_history()
+
         return ask_once(
             message,
-            self.chat_manager,
+            self.context_manager,
             self.function_manager,
             self.assistant,
         )
```

### Comparing `llmt-0.0.4/llmt/exceptions.py` & `llmt-0.0.5/llmt/exceptions.py`

 * *Files identical despite different names*

### Comparing `llmt-0.0.4/llmt/managers.py` & `llmt-0.0.5/llmt/managers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,50 @@
 import os
 import sys
 import json
 import time
 import jinja2
 import importlib.util
+from abc import ABC, abstractmethod
 
 from typing import Any, Callable, overload
 from inspect import getmembers, isfunction
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler
 
 from .functions.functions import FunctionResult, OpenAIFunction
 from .functions.sets import OpenAIFunctionSet
 from .json_type import JsonType
 from .openai_types import FunctionCall
 from .utils import logger
 from .consts import RESPONSE_TEMPLATE
 
 
+class FileManagerInterface(ABC):
+    @abstractmethod
+    def create(self, context_name):
+        pass
+
+    @abstractmethod
+    def get_history(self):
+        pass
+
+    @abstractmethod
+    def list(self):
+        pass
+
+    @abstractmethod
+    def list_messages(self):
+        pass
+
+    @abstractmethod
+    def save(self, message):
+        pass
+
+
 class EventHandler(FileSystemEventHandler):
     """Event handler for the input file system events."""
 
     def __init__(self):
         super().__init__()
 
         self.contents = ""
@@ -63,98 +86,149 @@
         self.env = jinja2.Environment(
             trim_blocks=True,
             lstrip_blocks=True,
             loader=jinja2.FileSystemLoader(searchpath=os.path.join(root_path, "llmt")),
         )
 
     def init(self):
-        if not os.path.exists(self.input_file):
-            with open(self.input_file, "w") as f:
-                f.write("")
-
-        if not os.path.exists(self.output_file):
-            with open(self.output_file, "w") as f:
-                f.write("")
+        with open(self.input_file, "w") as f:
+            f.write("")
 
-    def output_file_contents(self):
+        with open(self.output_file, "w") as f:
+            f.write("")
+
+    def output_contents(self):
         with open(self.output_file, "r") as f:
             return f.read()
 
     def write_to_output(self, data):
+        with open(self.output_file, "w") as f:
+            f.write(data)
+
+    def prepend_to_output(self, data):
         template = self.env.get_template(RESPONSE_TEMPLATE)
-        file_contents = self.output_file_contents()
-        date = time.strftime("%Y-%m-%d %I:%M%p")
-        data["date"] = date
-    
+        file_contents = self.output_contents()
+
         with open(self.output_file, "w") as f:
             f.write(template.render(**data))
 
             if file_contents:
-                f.write("\n\n")
-                f.write("---")
-                f.write("\n\n")
                 f.write(file_contents)
 
     def events_generator(self):
         yield from self.event_handler.events_generator()
         self.observer.join()
 
     def __del__(self):
         self.observer.stop()
 
 
-class ChatManager:
+class ChatManager(FileManagerInterface):
     def __init__(self, path):
         self.path = f"{path}/chats"
 
         if not os.path.exists(self.path):
             os.makedirs(self.path)
 
-    def init_chat(self, chat_name):
+    def create(self, chat_name):
         self.chat_name = chat_name
         self.file_path = os.path.join(self.path, f"{self.chat_name}.json")
 
         if not os.path.exists(self.file_path):
             with open(self.file_path, "w") as f:
                 json.dump([], f)
 
-    def save_to_chat(self, message):
+    def get_history(self):
+        with open(self.file_path) as f:
+            return json.load(f)
+
+    def list(self):
+        return [x.split(".")[0] for x in os.listdir(self.path) if x.endswith(".json")]
+
+    def list_messages(self):
+        with open(os.path.join(self.path, f"{self.chat_name}.json")) as f:
+            try:
+                return len(json.load(f))
+            except json.JSONDecodeError:
+                return 0
+
+    def save(self, message):
         chat_list = []
 
         with open(self.file_path) as f:
-            chat_list = json.load(f)
+            try:
+                chat_list = json.load(f)
+            except json.JSONDecodeError:
+                chat_list = []
 
         chat_list.append(message)
 
         with open(self.file_path, "w") as f:
             json.dump(chat_list, f, indent=4)
 
-    def list_chats(self):
+
+class ContextManager(FileManagerInterface):
+    def __init__(self, path):
+        self.path = f"{path}/contexts"
+
+        if not os.path.exists(self.path):
+            os.makedirs(self.path)
+
+    def create(self, context_name):
+        self.context_name = context_name
+        self.file_path = os.path.join(self.path, f"{self.context_name}.json")
+
+        if not os.path.exists(self.file_path):
+            with open(self.file_path, "w") as f:
+                json.dump([], f)
+
+    def get_history(self):
+        with open(self.file_path) as f:
+            return json.load(f)
+
+    def list(self):
         return [x.split(".")[0] for x in os.listdir(self.path) if x.endswith(".json")]
 
     def list_messages(self):
-        with open(os.path.join(self.path, f"{self.chat_name}.json")) as f:
-            return len(json.load(f))
+        with open(os.path.join(self.path, f"{self.context_name}.json")) as f:
+            try:
+                return len(json.load(f))
+            except json.JSONDecodeError:
+                return 0
+
+    def save(self, message):
+        context_list = []
 
+        with open(self.file_path) as f:
+            try:
+                context_list = json.load(f)
+            except json.JSONDecodeError:
+                context_list = []
 
-class FunctionManager():
+        context_list.append(message)
+
+        with open(self.file_path, "w") as f:
+            json.dump(context_list, f, indent=4)
+
+
+class FunctionManager:
     def __init__(self, paths):
         self._paths = []
         self.functions = OpenAIFunctionSet(*([]))
 
         for path in paths:
             if not os.path.exists(path):
                 logger.warning(f"Path {path} does not exist.")
                 continue
             self._paths.append(path)
             self._init_functions(path)
-    
+
     def _path_exists(self, path):
         return os.path.exists(path)
-    
+
     def _module_functions(self, path):
         spec = importlib.util.spec_from_file_location("llmt.udfs", path)
         module = importlib.util.module_from_spec(spec)
         sys.modules["llmt.udfs"] = module
         spec.loader.exec_module(module)
         return getmembers(module, isfunction)
 
@@ -169,43 +243,40 @@
 
         Returns:
             list[JsonType]: The functions schema.
         """
         return self.functions.functions_schema
 
     @overload
-    def add_function(self, function: OpenAIFunction) -> OpenAIFunction:
-        ...
+    def add_function(self, function: OpenAIFunction) -> OpenAIFunction: ...
 
     @overload
     def add_function(
         self,
         function: Callable[..., Any],
         *,
         name: str | None = None,
         description: str | None = None,
         save_return: bool = True,
         serialize: bool = True,
         remove_call: bool = False,
         interpret_as_response: bool = False,
-    ) -> Callable[..., Any]:
-        ...
+    ) -> Callable[..., Any]: ...
 
     @overload
     def add_function(
         self,
         *,
         name: str | None = None,
         description: str | None = None,
         save_return: bool = True,
         serialize: bool = True,
         remove_call: bool = False,
         interpret_as_response: bool = False,
-    ) -> Callable[[Callable[..., Any]], Callable[..., Any]]:
-        ...
+    ) -> Callable[[Callable[..., Any]], Callable[..., Any]]: ...
 
     def add_function(
         self,
         function: OpenAIFunction | Callable[..., Any] | None = None,
         *,
         name: str | None = None,
         description: str | None = None,
```

### Comparing `llmt-0.0.4/llmt/openai_types.py` & `llmt-0.0.5/llmt/openai_types.py`

 * *Files identical despite different names*

### Comparing `llmt-0.0.4/llmt/prompts.py` & `llmt-0.0.5/llmt/prompts.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import time
 import inquirer
 
+from pydantic import BaseModel
 from typing import List
 from halo import Halo
 from llmt.openai_types import FunctionCall
 from openai.types import CompletionChoice, CompletionUsage
 from openai.types.chat import (
     ChatCompletion,
     ChatCompletionMessage,
@@ -16,14 +18,46 @@
 
 class Style:
     GREEN = "\033[32m"
     RESET = "\033[0m"
     YELLOW = "\033[33m"
 
 
+class ChatResponse(BaseModel):
+    role: str
+    content: str
+    function_calls: List[FunctionCall]
+    usage: dict
+    date: str
+
+
+def create_chat_message(role, content, function_calls=None, usage=None):
+    """Create a chat message.
+
+    Args:
+        role (str): Role name.
+        response (dict): The response.
+
+    Returns:
+        ChatResponse: The chat response.
+    """
+    if function_calls is None:
+        function_calls = []
+    if usage is None:
+        usage = {}
+
+    return ChatResponse(
+        role=role,
+        content=content,
+        function_calls=function_calls,
+        usage=usage,
+        date=time.strftime("%Y-%m-%d %I:%M%p"),
+    )
+
+
 def prompt_create_chat():
     """Prompt the user to create a new chat thread.
 
     Returns:
         str: Chat name.
     """
     questions = [inquirer.Text("chat_name", message="Enter a chat name")]
@@ -61,42 +95,42 @@
     """Get the usage information.
 
     Returns:
         str: The usage information.
     """
     return ", ".join(
         [
-            f'completion tokens: {usage["completion_tokens"]}',
-            f'prompt tokens: {usage["prompt_tokens"]}',
-            f'total tokens: {usage["total_tokens"]}',
+            f'completion tokens: {usage.get("completion_tokens", "")}',
+            f'prompt tokens: {usage.get("prompt_tokens", "")}',
+            f'total tokens: {usage.get("total_tokens", "")}',
         ]
     )
 
 
-def run_until_response(messages, assistant, chat_manager, function_manager):
+def run_until_response(context, assistant, function_manager):
     function_calls = []
 
     while True:
         function_schema = (
             function_manager.functions_schema if function_manager else None
         )
         chat_completion: ChatCompletion = assistant.generate_message(
-            messages, function_schema
+            context, function_schema
         )
         chat_completion_choice: CompletionChoice = chat_completion.choices[0]
         chat_completion_message: ChatCompletionMessage = chat_completion_choice.message
         usage: CompletionUsage = chat_completion.usage
         response: str = chat_completion_message.content
 
         if chat_completion_choice.finish_reason == "tool_calls":
             tool_calls: List[ChatCompletionMessageToolCall] = (
                 chat_completion_message.tool_calls
             )
             message = {"role": "assistant", "tool_calls": tool_calls}
-            messages.append(message)
+            context.append(message)
 
             for tool_call in tool_calls:
                 args = tool_call.function.arguments
                 fn_name = tool_call.function.name
                 function_call: FunctionCall = {
                     "name": fn_name,
                     "arguments": args,
@@ -105,99 +139,101 @@
                 message = {
                     "role": "tool",
                     "content": str(result.content),
                     "tool_call_id": tool_call.id,
                     "name": fn_name,
                 }
                 template_message = {**message, "arguments": args}
-                messages.append(message)
-                chat_manager.save_to_chat(message)
+                context.append(message)
                 function_calls.append(template_message)
 
             continue
 
         if chat_completion_choice.finish_reason == "stop":
             break
 
     return {
         "response": response,
-        "messages": messages,
+        "messages": context,
         "function_calls": function_calls,
         "usage": {
             "completion_tokens": usage.completion_tokens,
             "prompt_tokens": usage.prompt_tokens,
             "total_tokens": usage.total_tokens,
         },
     }
 
 
 def ask_once(
     input_text,
-    chat_manager,
+    context_manager,
     function_manager,
     assistant: OpenAIAssistant,
 ):
     """Chat with the assistant once.
 
     Args:
         input_text (str): The input text.
-        chat_manager (ChatManager): The chat manager.
+        context_manager (ContextManager): The context manager.
         function_manager (FunctionManager): The function manager.
         assistant (OpenAIAssistant): The assistant.
         functions (module): The functions module.
 
     Returns:
         dict: The assistant, response, function calls, and usage information.
     """
+    context = context_manager.get_history()
+
     message = {"role": "user", "content": input_text}
-    messages = [{"role": "system", "content": assistant.description}, message]
-    chat_manager.save_to_chat(message)
+    context_manager.save(message)
+    context.append(message)
 
     response = run_until_response(
-        messages,
+        context,
         assistant,
-        chat_manager,
         function_manager,
     )
-    messages = response["messages"]
+
+    # context becomes the response messages
+    context = response["messages"]
+
     message = {"role": "assistant", "content": response["response"]}
-    messages.append(message)
-    chat_manager.save_to_chat(message)
+    context_manager.save(message)
+    context.append(message)
 
-    return {
-        "assistant": assistant,
-        "response": response["response"],
-        "function_calls": response["function_calls"],
-        "info": get_usage_as_string(response["usage"]),
-    }
+    return create_chat_message(
+        "system", response["response"], response["function_calls"], response["usage"]
+    ).model_dump()
 
 
 def ask(
     chat_manager,
+    context_manager,
     file_manager,
     function_manager,
     assistant: OpenAIAssistant,
 ):
     """Chat with the assistant.
 
     Args:
         chat_manager (ChatManager): The chat manager.
+        context_manager (ContextManager): The context manager.
         file_manager (FileManager or None): The input file handler object or None.
         function_manager (FunctionManager): The function manager.
         assistant (OpenAIAssistant): The assistant.
 
     Returns:
         None
 
     Yields:
         str: The response.
     """
     input_text = ""
     response = ""
-    messages = [{"role": "system", "content": assistant.description}]
+    context = context_manager.get_history()
     spinner = Halo(text="Working...", spinner="dots")
 
     while True:
         if file_manager:
             print(f"{Style.GREEN}You{Style.RESET}: using {file_manager.input_file}")
 
             for event in file_manager.events_generator():
@@ -209,39 +245,47 @@
         if len(input_text) == 0:
             continue
 
         if input_text.lower() in EXIT_CODES:
             break
 
         message = {"role": "user", "content": input_text}
-        messages.append(message)
-        chat_manager.save_to_chat(message)
+        context.append(message)
+        context_manager.save(message)
+
+        chat_user_message = create_chat_message("user", input_text).model_dump()
+        chat_manager.save(chat_user_message)
 
         spinner.start()
+
         response = run_until_response(
-            messages,
+            context,
             assistant,
-            chat_manager,
             function_manager,
         )
-        messages = response["messages"]
+
+        # context becomes the response messages
+        context = response["messages"]
+
         spinner.stop()
 
         message = {"role": "assistant", "content": response["response"]}
-        messages.append(message)
-        chat_manager.save_to_chat(message)
-        to_user_response = {
-            "assistant": assistant,
-            "response": response["response"],
-            "function_calls": response["function_calls"],
-            "info": get_usage_as_string(response["usage"]),
-        }
+        context.append(message)
+        context_manager.save(message)
+
+        chat_response = create_chat_message(
+            "system",
+            response["response"],
+            response["function_calls"],
+            response["usage"],
+        ).model_dump()
+        chat_manager.save(chat_response)
 
         if file_manager:
-            file_manager.write_to_output(to_user_response)
+            file_manager.prepend_to_output(chat_response)
         else:
             yield " ".join(
                 [
                     f"{Style.GREEN}{assistant.name}{Style.RESET}:",
                     f"{response['response']}\n\n{Style.YELLOW}usage{Style.RESET}:",
                     f"{get_usage_as_string(response['usage'])}",
                 ]
```

### Comparing `llmt-0.0.4/llmt/utils.py` & `llmt-0.0.5/llmt/utils.py`

 * *Files identical despite different names*

### Comparing `llmt-0.0.4/llmt.egg-info/PKG-INFO` & `llmt-0.0.5/llmt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: llmt
-Version: 0.0.4
-Summary: Convenient LLM chat wrapper for data pipelines, CI/CD, or personal workspaces.
+Version: 0.0.5
+Summary: LLMT aims to make it easy to programatically connect OpenAI and HuggingFace models to your data pipelines, CI/CD, or personal workspaces.
 Author-email: Artem Golub <artem@outermeasure.com>
 Project-URL: Homepage, https://github.com/omhq/llmt
 Project-URL: Bug Tracker, https://github.com/omhq/llmt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai==1.14.1
+Requires-Dist: requests==2.31.0
 Requires-Dist: watchdog==4.0.0
 Requires-Dist: halo==0.0.31
 Requires-Dist: inquirer==3.2.4
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: docstring-parser==0.16
 Requires-Dist: typing-extensions==4.10.0
@@ -25,42 +26,43 @@
 Requires-Dist: SQLAlchemy==2.0.28
 Requires-Dist: pydantic==2.6.4
 
 # LLMT
 
 [![PyPI version](https://badge.fury.io/py/llmt.svg)](https://badge.fury.io/py/llmt)
 
-## Overview
+## What is this good for?
 
-Convenient LLM chat wrapper for data pipelines, CI/CD, or personal workspaces.
+LLMT aims to make it easy to programatically connect OpenAI and HuggingFace models to your data pipelines, CI/CD, or personal workspaces.
 
-Supports local function calling, chat history retention, and can run anywhere. Chat using a terminal, input/output files, or directly through LLMT API.
+Supports function calling, chat and context history retention. Python 3.12 and up.
 
 ### Usage
 
 Use the package in directly in your python code (`pip install llmt`), or as a local workspace running a container to interact with ChatGPT.
 
 ### Module import
 
 ```python
 from llmt import LLMT
 
 
 llmt = LLMT()
 llmt.init_assistant(
-    "dataengineer",
+    "snowflake",
     api_key="...",
     model="gpt-3.5-turbo",
-    assistant_description="You are a data engineer, and a python expert.",)
-llmt.init_functions(["./my_functions.py"])
-llmt.init_chat("single_chat")
-
-response = llmt.run(
-    "What's the result of 22 plus 5 in decimal added to the hexadecimal number A?"
+    assistant_description="You are a snowflake expert. Answer questions briefly in a sentence or less."
 )
+
+llmt.init_functions(["./helper_functions.py"])
+llmt.init_context("snowflake")
+response = llmt.run("generate an example merge dml")
+
+print(response)
 ```
 
 ### Local workspace
 
 Install Docker and make command. Make is not required since you can use docker compose.
 
 - Clone this repo.
```

### Comparing `llmt-0.0.4/pyproject.toml` & `llmt-0.0.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "llmt"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Artem Golub", email="artem @ outermeasure.com"}
 ]
-description = "Convenient LLM chat wrapper for data pipelines, CI/CD, or personal workspaces."
+description = "LLMT aims to make it easy to programatically connect OpenAI and HuggingFace models to your data pipelines, CI/CD, or personal workspaces."
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.12"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dynamic = ["dependencies"]
```

