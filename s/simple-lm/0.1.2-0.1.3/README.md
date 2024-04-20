# Comparing `tmp/simple_lm-0.1.2.tar.gz` & `tmp/simple_lm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_lm-0.1.2.tar", max compression
+gzip compressed data, was "simple_lm-0.1.3.tar", max compression
```

## Comparing `simple_lm-0.1.2.tar` & `simple_lm-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      665 2024-04-18 06:03:15.343416 simple_lm-0.1.2/README.md
--rw-r--r--   0        0        0      424 2024-04-18 18:37:24.025321 simple_lm-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       84 2024-04-18 06:27:42.611100 simple_lm-0.1.2/simple_lm/__init__.py
--rw-r--r--   0        0        0     1383 2024-04-18 18:37:16.770995 simple_lm-0.1.2/simple_lm/core.py
--rw-r--r--   0        0        0     1323 1970-01-01 00:00:00.000000 simple_lm-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      665 2024-04-18 06:03:15.343416 simple_lm-0.1.3/README.md
+-rw-r--r--   0        0        0      424 2024-04-20 05:00:09.996372 simple_lm-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       84 2024-04-18 06:27:42.611100 simple_lm-0.1.3/simple_lm/__init__.py
+-rw-r--r--   0        0        0     1794 2024-04-20 04:58:58.676716 simple_lm-0.1.3/simple_lm/core.py
+-rw-r--r--   0        0        0     1323 1970-01-01 00:00:00.000000 simple_lm-0.1.3/PKG-INFO
```

### Comparing `simple_lm-0.1.2/README.md` & `simple_lm-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `simple_lm-0.1.2/simple_lm/core.py` & `simple_lm-0.1.3/simple_lm/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 from instructor import from_openai, from_anthropic, Mode
 from anthropic import Anthropic
 from openai import OpenAI
 
 
+from instructor import from_openai, from_anthropic, Mode
+from anthropic import Anthropic
+from openai import OpenAI
+
+
 class SimpleLM:
     def __init__(self):
         self.clients = {}
         self.models = {}
 
     def setup_client(
         self,
         client_name,
         api_key=None,
+        mode=Mode.MD_JSON
     ):
+        
         client_creator = {
             "openai": lambda: from_openai(
                 OpenAI(api_key=api_key),
             ),
             "anthropic": lambda: from_anthropic(Anthropic(api_key=api_key)),
             "together": lambda: from_openai(
                 OpenAI(api_key=api_key, base_url="https://api.together.xyz/v1"),
-                mode=Mode.MD_JSON,
+                mode=mode
             ),
             "ollama": lambda: from_openai(
                 OpenAI(api_key=api_key, base_url="http://localhost:11434/v1"),
-                mode=Mode.TOOLS,
+                mode=mode
             ),
         }
 
         if client_name in client_creator:
             client = client_creator[client_name]()
         else:
             raise ValueError(f"Unsupported client type: {client_name}")
@@ -39,8 +46,17 @@
 
     def get_client(self, client_name):
         if client_name in self.clients:
             return self.clients[client_name]
         else:
             raise ValueError(
                 f"Client '{client_name}' not initialized. Please set up the client first."
+            )
+
+
+    def get_client(self, client_name):
+        if client_name in self.clients:
+            return self.clients[client_name]
+        else:
+            raise ValueError(
+                f"Client '{client_name}' not initialized. Please set up the client first."
             )
```

### Comparing `simple_lm-0.1.2/PKG-INFO` & `simple_lm-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-lm
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple abstraction over instructor for LLM apps
 License: MIT
 Author: Joe Petrantoni
 Author-email: 79169021+jpetrantoni@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

