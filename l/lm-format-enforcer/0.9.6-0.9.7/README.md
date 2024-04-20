# Comparing `tmp/lm_format_enforcer-0.9.6.tar.gz` & `tmp/lm_format_enforcer-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lm_format_enforcer-0.9.6.tar", max compression
+gzip compressed data, was "lm_format_enforcer-0.9.7.tar", max compression
```

## Comparing `lm_format_enforcer-0.9.6.tar` & `lm_format_enforcer-0.9.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1065 2024-04-19 07:43:38.737733 lm_format_enforcer-0.9.6/LICENSE
--rw-r--r--   0        0        0    12804 2024-04-19 07:43:38.737733 lm_format_enforcer-0.9.6/README.md
--rw-r--r--   0        0        0      850 2024-04-19 07:43:38.737733 lm_format_enforcer-0.9.6/lmformatenforcer/__init__.py
--rw-r--r--   0        0        0     3893 2024-04-19 07:43:38.737733 lm_format_enforcer-0.9.6/lmformatenforcer/analyzer.py
--rw-r--r--   0        0        0     6702 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/characterlevelparser.py
--rw-r--r--   0        0        0      341 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/consts.py
--rw-r--r--   0        0        0      104 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/external/__init__.py
--rw-r--r--   0        0        0    10566 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/external/jsonschemaobject.py
--rw-r--r--   0        0        0     7044 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/external/jsonschemaobjectutil.py
--rw-r--r--   0        0        0        0 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/integrations/__init__.py
--rw-r--r--   0        0        0     2595 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/integrations/exllamav2.py
--rw-r--r--   0        0        0     2820 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/integrations/haystackv1.py
--rw-r--r--   0        0        0     3518 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/integrations/haystackv2.py
--rw-r--r--   0        0        0     3572 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/integrations/llamacpp.py
--rw-r--r--   0        0        0     6769 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/integrations/transformers.py
--rw-r--r--   0        0        0     3538 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/integrations/trtllm.py
--rw-r--r--   0        0        0     2645 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/integrations/vllm.py
--rw-r--r--   0        0        0    29631 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/jsonschemaparser.py
--rw-r--r--   0        0        0     3926 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/regexparser.py
--rw-r--r--   0        0        0    10083 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/tokenenforcer.py
--rw-r--r--   0        0        0     6813 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/tokenizerprefixtree.py
--rw-r--r--   0        0        0     2664 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/pyproject.toml
--rw-r--r--   0        0        0    14137 1970-01-01 00:00:00.000000 lm_format_enforcer-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-20 06:28:51.746895 lm_format_enforcer-0.9.7/LICENSE
+-rw-r--r--   0        0        0    12804 2024-04-20 06:28:51.746895 lm_format_enforcer-0.9.7/README.md
+-rw-r--r--   0        0        0      850 2024-04-20 06:28:51.750895 lm_format_enforcer-0.9.7/lmformatenforcer/__init__.py
+-rw-r--r--   0        0        0     3893 2024-04-20 06:28:51.750895 lm_format_enforcer-0.9.7/lmformatenforcer/analyzer.py
+-rw-r--r--   0        0        0     6702 2024-04-20 06:28:51.750895 lm_format_enforcer-0.9.7/lmformatenforcer/characterlevelparser.py
+-rw-r--r--   0        0        0      341 2024-04-20 06:28:51.750895 lm_format_enforcer-0.9.7/lmformatenforcer/consts.py
+-rw-r--r--   0        0        0      104 2024-04-20 06:28:51.750895 lm_format_enforcer-0.9.7/lmformatenforcer/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-20 06:28:51.750895 lm_format_enforcer-0.9.7/lmformatenforcer/external/__init__.py
+-rw-r--r--   0        0        0    10566 2024-04-20 06:28:51.750895 lm_format_enforcer-0.9.7/lmformatenforcer/external/jsonschemaobject.py
+-rw-r--r--   0        0        0     7044 2024-04-20 06:28:51.750895 lm_format_enforcer-0.9.7/lmformatenforcer/external/jsonschemaobjectutil.py
+-rw-r--r--   0        0        0        0 2024-04-20 06:28:51.750895 lm_format_enforcer-0.9.7/lmformatenforcer/integrations/__init__.py
+-rw-r--r--   0        0        0     2595 2024-04-20 06:28:51.750895 lm_format_enforcer-0.9.7/lmformatenforcer/integrations/exllamav2.py
+-rw-r--r--   0        0        0     2820 2024-04-20 06:28:51.750895 lm_format_enforcer-0.9.7/lmformatenforcer/integrations/haystackv1.py
+-rw-r--r--   0        0        0     3518 2024-04-20 06:28:51.750895 lm_format_enforcer-0.9.7/lmformatenforcer/integrations/haystackv2.py
+-rw-r--r--   0        0        0     3572 2024-04-20 06:28:51.750895 lm_format_enforcer-0.9.7/lmformatenforcer/integrations/llamacpp.py
+-rw-r--r--   0        0        0     6769 2024-04-20 06:28:51.750895 lm_format_enforcer-0.9.7/lmformatenforcer/integrations/transformers.py
+-rw-r--r--   0        0        0     3538 2024-04-20 06:28:51.750895 lm_format_enforcer-0.9.7/lmformatenforcer/integrations/trtllm.py
+-rw-r--r--   0        0        0     2645 2024-04-20 06:28:51.750895 lm_format_enforcer-0.9.7/lmformatenforcer/integrations/vllm.py
+-rw-r--r--   0        0        0    30242 2024-04-20 06:28:51.750895 lm_format_enforcer-0.9.7/lmformatenforcer/jsonschemaparser.py
+-rw-r--r--   0        0        0     3926 2024-04-20 06:28:51.750895 lm_format_enforcer-0.9.7/lmformatenforcer/regexparser.py
+-rw-r--r--   0        0        0    10083 2024-04-20 06:28:51.750895 lm_format_enforcer-0.9.7/lmformatenforcer/tokenenforcer.py
+-rw-r--r--   0        0        0     6813 2024-04-20 06:28:51.750895 lm_format_enforcer-0.9.7/lmformatenforcer/tokenizerprefixtree.py
+-rw-r--r--   0        0        0     2664 2024-04-20 06:28:51.750895 lm_format_enforcer-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0    14137 1970-01-01 00:00:00.000000 lm_format_enforcer-0.9.7/PKG-INFO
```

### Comparing `lm_format_enforcer-0.9.6/LICENSE` & `lm_format_enforcer-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.6/README.md` & `lm_format_enforcer-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.6/lmformatenforcer/__init__.py` & `lm_format_enforcer-0.9.7/lmformatenforcer/__init__.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.6/lmformatenforcer/analyzer.py` & `lm_format_enforcer-0.9.7/lmformatenforcer/analyzer.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.6/lmformatenforcer/characterlevelparser.py` & `lm_format_enforcer-0.9.7/lmformatenforcer/characterlevelparser.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.6/lmformatenforcer/external/jsonschemaobject.py` & `lm_format_enforcer-0.9.7/lmformatenforcer/external/jsonschemaobject.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.6/lmformatenforcer/external/jsonschemaobjectutil.py` & `lm_format_enforcer-0.9.7/lmformatenforcer/external/jsonschemaobjectutil.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.6/lmformatenforcer/integrations/exllamav2.py` & `lm_format_enforcer-0.9.7/lmformatenforcer/integrations/exllamav2.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.6/lmformatenforcer/integrations/haystackv1.py` & `lm_format_enforcer-0.9.7/lmformatenforcer/integrations/haystackv1.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.6/lmformatenforcer/integrations/haystackv2.py` & `lm_format_enforcer-0.9.7/lmformatenforcer/integrations/haystackv2.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.6/lmformatenforcer/integrations/llamacpp.py` & `lm_format_enforcer-0.9.7/lmformatenforcer/integrations/llamacpp.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.6/lmformatenforcer/integrations/transformers.py` & `lm_format_enforcer-0.9.7/lmformatenforcer/integrations/transformers.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.6/lmformatenforcer/integrations/trtllm.py` & `lm_format_enforcer-0.9.7/lmformatenforcer/integrations/trtllm.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.6/lmformatenforcer/integrations/vllm.py` & `lm_format_enforcer-0.9.7/lmformatenforcer/integrations/vllm.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.6/lmformatenforcer/jsonschemaparser.py` & `lm_format_enforcer-0.9.7/lmformatenforcer/jsonschemaparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,23 @@
                 option_stack = updated_parser.object_stack[:-1] + [option_parser]
                 option_parser = JsonSchemaParser(self.context, self.config, option_stack, updated_parser.num_consecutive_whitespaces)
                 option_parser.context.active_parser = option_parser
                 option_parser.last_parsed_string = last_parsed_string
                 option_json_schema_parsers.append(option_parser)
             return UnionParser(option_json_schema_parsers)
 
+        # For some performance optimizations to work, we want to make sure we don't leave irrelevant
+        # objects at the top of the stack, which we know will be passed over next timestep
+        new_object_stack = updated_parser.object_stack
+        while new_object_stack and new_object_stack[-1].can_end() and new_object_stack[-1].get_allowed_characters() == '':
+            finished_receiver = new_object_stack[-1]
+            if isinstance(finished_receiver, StringParsingState):
+                updated_parser.last_parsed_string = finished_receiver.parsed_string
+            del new_object_stack[-1]
+
         return updated_parser
 
     def get_allowed_characters(self) -> str:
         self.context.active_parser = self
         
         allowed_character_strs = []
         for parser in reversed(self.object_stack):
```

### Comparing `lm_format_enforcer-0.9.6/lmformatenforcer/regexparser.py` & `lm_format_enforcer-0.9.7/lmformatenforcer/regexparser.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.6/lmformatenforcer/tokenenforcer.py` & `lm_format_enforcer-0.9.7/lmformatenforcer/tokenenforcer.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.6/lmformatenforcer/tokenizerprefixtree.py` & `lm_format_enforcer-0.9.7/lmformatenforcer/tokenizerprefixtree.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.6/pyproject.toml` & `lm_format_enforcer-0.9.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lm-format-enforcer"
-version = "0.9.6"
+version = "0.9.7"
 description = "Enforce the output format (JSON Schema, Regex etc) of a language model"
 authors = ["Noam Gat <noamgat@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noamgat/lm-format-enforcer"
 repository = "https://github.com/noamgat/lm-format-enforcer"
 documentation = "https://github.com/noamgat/lm-format-enforcer"
```

### Comparing `lm_format_enforcer-0.9.6/PKG-INFO` & `lm_format_enforcer-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lm-format-enforcer
-Version: 0.9.6
+Version: 0.9.7
 Summary: Enforce the output format (JSON Schema, Regex etc) of a language model
 Home-page: https://github.com/noamgat/lm-format-enforcer
 License: MIT
 Author: Noam Gat
 Author-email: noamgat@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

