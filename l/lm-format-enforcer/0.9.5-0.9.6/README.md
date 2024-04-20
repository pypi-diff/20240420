# Comparing `tmp/lm_format_enforcer-0.9.5.tar.gz` & `tmp/lm_format_enforcer-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lm_format_enforcer-0.9.5.tar", max compression
+gzip compressed data, was "lm_format_enforcer-0.9.6.tar", max compression
```

## Comparing `lm_format_enforcer-0.9.5.tar` & `lm_format_enforcer-0.9.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1065 2024-04-12 20:19:20.208109 lm_format_enforcer-0.9.5/LICENSE
--rw-r--r--   0        0        0    12804 2024-04-12 20:19:20.208109 lm_format_enforcer-0.9.5/README.md
--rw-r--r--   0        0        0      850 2024-04-12 20:19:20.208109 lm_format_enforcer-0.9.5/lmformatenforcer/__init__.py
--rw-r--r--   0        0        0     3893 2024-04-12 20:19:20.208109 lm_format_enforcer-0.9.5/lmformatenforcer/analyzer.py
--rw-r--r--   0        0        0     6702 2024-04-12 20:19:20.208109 lm_format_enforcer-0.9.5/lmformatenforcer/characterlevelparser.py
--rw-r--r--   0        0        0      341 2024-04-12 20:19:20.208109 lm_format_enforcer-0.9.5/lmformatenforcer/consts.py
--rw-r--r--   0        0        0      104 2024-04-12 20:19:20.208109 lm_format_enforcer-0.9.5/lmformatenforcer/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-12 20:19:20.208109 lm_format_enforcer-0.9.5/lmformatenforcer/external/__init__.py
--rw-r--r--   0        0        0    10566 2024-04-12 20:19:20.212109 lm_format_enforcer-0.9.5/lmformatenforcer/external/jsonschemaobject.py
--rw-r--r--   0        0        0     7044 2024-04-12 20:19:20.212109 lm_format_enforcer-0.9.5/lmformatenforcer/external/jsonschemaobjectutil.py
--rw-r--r--   0        0        0        0 2024-04-12 20:19:20.212109 lm_format_enforcer-0.9.5/lmformatenforcer/integrations/__init__.py
--rw-r--r--   0        0        0     2798 2024-04-12 20:19:20.212109 lm_format_enforcer-0.9.5/lmformatenforcer/integrations/exllamav2.py
--rw-r--r--   0        0        0     2820 2024-04-12 20:19:20.212109 lm_format_enforcer-0.9.5/lmformatenforcer/integrations/haystackv1.py
--rw-r--r--   0        0        0     3518 2024-04-12 20:19:20.212109 lm_format_enforcer-0.9.5/lmformatenforcer/integrations/haystackv2.py
--rw-r--r--   0        0        0     3572 2024-04-12 20:19:20.212109 lm_format_enforcer-0.9.5/lmformatenforcer/integrations/llamacpp.py
--rw-r--r--   0        0        0     6769 2024-04-12 20:19:20.212109 lm_format_enforcer-0.9.5/lmformatenforcer/integrations/transformers.py
--rw-r--r--   0        0        0     3538 2024-04-12 20:19:20.212109 lm_format_enforcer-0.9.5/lmformatenforcer/integrations/trtllm.py
--rw-r--r--   0        0        0     2645 2024-04-12 20:19:20.212109 lm_format_enforcer-0.9.5/lmformatenforcer/integrations/vllm.py
--rw-r--r--   0        0        0    29631 2024-04-12 20:19:20.212109 lm_format_enforcer-0.9.5/lmformatenforcer/jsonschemaparser.py
--rw-r--r--   0        0        0     3926 2024-04-12 20:19:20.212109 lm_format_enforcer-0.9.5/lmformatenforcer/regexparser.py
--rw-r--r--   0        0        0    10083 2024-04-12 20:19:20.212109 lm_format_enforcer-0.9.5/lmformatenforcer/tokenenforcer.py
--rw-r--r--   0        0        0     6813 2024-04-12 20:19:20.212109 lm_format_enforcer-0.9.5/lmformatenforcer/tokenizerprefixtree.py
--rw-r--r--   0        0        0     2664 2024-04-12 20:19:20.212109 lm_format_enforcer-0.9.5/pyproject.toml
--rw-r--r--   0        0        0    14137 1970-01-01 00:00:00.000000 lm_format_enforcer-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-19 07:43:38.737733 lm_format_enforcer-0.9.6/LICENSE
+-rw-r--r--   0        0        0    12804 2024-04-19 07:43:38.737733 lm_format_enforcer-0.9.6/README.md
+-rw-r--r--   0        0        0      850 2024-04-19 07:43:38.737733 lm_format_enforcer-0.9.6/lmformatenforcer/__init__.py
+-rw-r--r--   0        0        0     3893 2024-04-19 07:43:38.737733 lm_format_enforcer-0.9.6/lmformatenforcer/analyzer.py
+-rw-r--r--   0        0        0     6702 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/characterlevelparser.py
+-rw-r--r--   0        0        0      341 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/consts.py
+-rw-r--r--   0        0        0      104 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/external/__init__.py
+-rw-r--r--   0        0        0    10566 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/external/jsonschemaobject.py
+-rw-r--r--   0        0        0     7044 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/external/jsonschemaobjectutil.py
+-rw-r--r--   0        0        0        0 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/integrations/__init__.py
+-rw-r--r--   0        0        0     2595 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/integrations/exllamav2.py
+-rw-r--r--   0        0        0     2820 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/integrations/haystackv1.py
+-rw-r--r--   0        0        0     3518 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/integrations/haystackv2.py
+-rw-r--r--   0        0        0     3572 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/integrations/llamacpp.py
+-rw-r--r--   0        0        0     6769 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/integrations/transformers.py
+-rw-r--r--   0        0        0     3538 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/integrations/trtllm.py
+-rw-r--r--   0        0        0     2645 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/integrations/vllm.py
+-rw-r--r--   0        0        0    29631 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/jsonschemaparser.py
+-rw-r--r--   0        0        0     3926 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/regexparser.py
+-rw-r--r--   0        0        0    10083 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/tokenenforcer.py
+-rw-r--r--   0        0        0     6813 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/lmformatenforcer/tokenizerprefixtree.py
+-rw-r--r--   0        0        0     2664 2024-04-19 07:43:38.741732 lm_format_enforcer-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0    14137 1970-01-01 00:00:00.000000 lm_format_enforcer-0.9.6/PKG-INFO
```

### Comparing `lm_format_enforcer-0.9.5/LICENSE` & `lm_format_enforcer-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.5/README.md` & `lm_format_enforcer-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.5/lmformatenforcer/__init__.py` & `lm_format_enforcer-0.9.6/lmformatenforcer/__init__.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.5/lmformatenforcer/analyzer.py` & `lm_format_enforcer-0.9.6/lmformatenforcer/analyzer.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.5/lmformatenforcer/characterlevelparser.py` & `lm_format_enforcer-0.9.6/lmformatenforcer/characterlevelparser.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.5/lmformatenforcer/external/jsonschemaobject.py` & `lm_format_enforcer-0.9.6/lmformatenforcer/external/jsonschemaobject.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.5/lmformatenforcer/external/jsonschemaobjectutil.py` & `lm_format_enforcer-0.9.6/lmformatenforcer/external/jsonschemaobjectutil.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.5/lmformatenforcer/integrations/exllamav2.py` & `lm_format_enforcer-0.9.6/lmformatenforcer/integrations/exllamav2.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,30 +6,29 @@
     raise ImportError('exllamav2 is not installed. Please install it with "pip install exllamav2"')
 
 from ..characterlevelparser import CharacterLevelParser
 from ..tokenenforcer import TokenEnforcer, TokenEnforcerTokenizerData
 
 
 def _build_regular_tokens_list(tokenizer: ExLlamaV2Tokenizer) -> List[Tuple[int, str, bool]]:
-    token_0 = tokenizer.encode("0")[0]
-    regular_tokens = []
     vocab_size = tokenizer.tokenizer.vocab_size()
-    all_special_ids = [tokenizer.bos_token_id, tokenizer.eos_token_id, tokenizer.pad_token_id, tokenizer.unk_token_id]
+    all_special_ids = set(tokenizer.extended_id_to_piece.keys())
+    all_special_ids.update({ tokenizer.bos_token_id, tokenizer.eos_token_id, tokenizer.pad_token_id, tokenizer.unk_token_id })
+    id_to_piece = tokenizer.get_id_to_piece_list()
+    regular_tokens = []
     for token_idx in range(vocab_size):
         if token_idx in all_special_ids:
             continue
-        # We prepend token 0 and skip the first letter of the result to get a space if the token is a start word.
-        tensor_after_0 = torch.tensor(token_0.tolist() + [token_idx], dtype=torch.long)
-        decoded_after_0 = tokenizer.decode(tensor_after_0)[1:]
-        decoded_regular = tokenizer.decode(token_0)
-        is_word_start_token = len(decoded_after_0) > len(decoded_regular)
-        regular_tokens.append((token_idx, decoded_after_0, is_word_start_token))
+        decoded = id_to_piece[token_idx]
+        is_word_start_token = len(decoded) > 0 and decoded[0] == " "
+        regular_tokens.append((token_idx, decoded, is_word_start_token))
     return regular_tokens
 
 
+
 def build_token_enforcer_tokenizer_data(tokenizer: ExLlamaV2Tokenizer) -> TokenEnforcerTokenizerData:
     regular_tokens = _build_regular_tokens_list(tokenizer)
 
     def _decode(tokens: List[int]) -> str:
         tensor = torch.tensor(tokens, dtype=torch.long)
         return tokenizer.decode(tensor)
```

### Comparing `lm_format_enforcer-0.9.5/lmformatenforcer/integrations/haystackv1.py` & `lm_format_enforcer-0.9.6/lmformatenforcer/integrations/haystackv1.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.5/lmformatenforcer/integrations/haystackv2.py` & `lm_format_enforcer-0.9.6/lmformatenforcer/integrations/haystackv2.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.5/lmformatenforcer/integrations/llamacpp.py` & `lm_format_enforcer-0.9.6/lmformatenforcer/integrations/llamacpp.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.5/lmformatenforcer/integrations/transformers.py` & `lm_format_enforcer-0.9.6/lmformatenforcer/integrations/transformers.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.5/lmformatenforcer/integrations/trtllm.py` & `lm_format_enforcer-0.9.6/lmformatenforcer/integrations/trtllm.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.5/lmformatenforcer/integrations/vllm.py` & `lm_format_enforcer-0.9.6/lmformatenforcer/integrations/vllm.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.5/lmformatenforcer/jsonschemaparser.py` & `lm_format_enforcer-0.9.6/lmformatenforcer/jsonschemaparser.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.5/lmformatenforcer/regexparser.py` & `lm_format_enforcer-0.9.6/lmformatenforcer/regexparser.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.5/lmformatenforcer/tokenenforcer.py` & `lm_format_enforcer-0.9.6/lmformatenforcer/tokenenforcer.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.5/lmformatenforcer/tokenizerprefixtree.py` & `lm_format_enforcer-0.9.6/lmformatenforcer/tokenizerprefixtree.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.5/pyproject.toml` & `lm_format_enforcer-0.9.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lm-format-enforcer"
-version = "0.9.5"
+version = "0.9.6"
 description = "Enforce the output format (JSON Schema, Regex etc) of a language model"
 authors = ["Noam Gat <noamgat@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noamgat/lm-format-enforcer"
 repository = "https://github.com/noamgat/lm-format-enforcer"
 documentation = "https://github.com/noamgat/lm-format-enforcer"
```

### Comparing `lm_format_enforcer-0.9.5/PKG-INFO` & `lm_format_enforcer-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lm-format-enforcer
-Version: 0.9.5
+Version: 0.9.6
 Summary: Enforce the output format (JSON Schema, Regex etc) of a language model
 Home-page: https://github.com/noamgat/lm-format-enforcer
 License: MIT
 Author: Noam Gat
 Author-email: noamgat@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

