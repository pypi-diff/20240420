# Comparing `tmp/llm_structured_output-0.0.7.tar.gz` & `tmp/llm_structured_output-0.0.8.tar.gz`

## Comparing `llm_structured_output-0.0.7.tar` & `llm_structured_output-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/_/_build.sh
--rwxr-xr-x   0        0        0      553 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/_/_eval.sh
--rwxr-xr-x   0        0        0     1991 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/_/_mistral_schema.sh
--rwxr-xr-x   0        0        0      853 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/_/_reluctance.sh
--rwxr-xr-x   0        0        0      219 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/_/_server.sh
--rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/_/_test_number_array.sh
--rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/_/_upload.sh
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/_/x.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/examples/json_schema_cli.py
--rw-r--r--   0        0        0    18108 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/examples/llm_schema.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/examples/reluctance.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/examples/requirements.txt
--rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/examples/server.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/llm_structured_output/__init__.py
--rw-r--r--   0        0        0    24610 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/llm_structured_output/acceptor.py
--rw-r--r--   0        0        0    15532 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/llm_structured_output/json_acceptor.py
--rw-r--r--   0        0        0    21243 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/llm_structured_output/json_schema_acceptor.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/llm_structured_output/util/__init__.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/llm_structured_output/util/bitmap.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/llm_structured_output/util/output.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/llm_structured_output/util/tokenization.py
--rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/llm_structured_output/util/tokentrie.py
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/tests/eval.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/src/tests/requirements.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/LICENSE
--rw-r--r--   0        0        0    13894 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/README.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    14495 2020-02-02 00:00:00.000000 llm_structured_output-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/.vscode/launch.json
+-rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/_/_build.sh
+-rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/_/_eval.sh
+-rwxr-xr-x   0        0        0     1995 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/_/_mistral_schema.sh
+-rwxr-xr-x   0        0        0      853 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/_/_reluctance.sh
+-rwxr-xr-x   0        0        0      219 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/_/_server.sh
+-rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/_/_test_number_array.sh
+-rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/_/_upload.sh
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/_/x.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/examples/json_schema_cli.py
+-rw-r--r--   0        0        0    20302 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/examples/llm_schema.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/examples/reluctance.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/examples/requirements.txt
+-rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/examples/server.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/llm_structured_output/__init__.py
+-rw-r--r--   0        0        0    23923 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/llm_structured_output/acceptor.py
+-rw-r--r--   0        0        0    15531 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/llm_structured_output/json_acceptor.py
+-rw-r--r--   0        0        0    21209 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/llm_structured_output/json_schema_acceptor.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/llm_structured_output/util/__init__.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/llm_structured_output/util/bitmap.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/llm_structured_output/util/output.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/llm_structured_output/util/tokenization.py
+-rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/llm_structured_output/util/tokentrie.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/tests/eval.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/src/tests/requirements.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/LICENSE
+-rw-r--r--   0        0        0    13894 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/README.md
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    14495 2020-02-02 00:00:00.000000 llm_structured_output-0.0.8/PKG-INFO
```

### Comparing `llm_structured_output-0.0.7/_/_eval.sh` & `llm_structured_output-0.0.8/_/_eval.sh`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 cd `dirname $0`/../src
 #MODEL=../local/models/mlx/Mistral-7B-v0.2-Instruct-f16
 #MODEL=mlx-community/Mistral-7B-Instruct-v0.2
-MODEL=mlx-community/Mistral-7B-v0.2-4bit
+#MODEL=mlx-community/Mistral-7B-v0.2-4bit
 #MODEL=mistralai/Mistral-7B-Instruct-v0.2
 #MODEL=mlx-community/Mixtral-8x22B-4bit
-#MODEL=mlx-community/CodeQwen1.5-7B-Chat-4bit
-EVAL_FILE=../../eval/fireworks-ai_function-calling-eval-dataset-v0/single_turn-00000-of-00001.json
-#EVAL_FILE=../../eval/fireworks-ai_function-calling-eval-dataset-v0/multi_turn-00000-of-00001.json
+MODEL=mlx-community/Meta-Llama-3-8B-Instruct-8bit
+#EVAL_FILE=../../eval/fireworks-ai_function-calling-eval-dataset-v0/single_turn-00000-of-00001.json
+EVAL_FILE=../../eval/fireworks-ai_function-calling-eval-dataset-v0/multi_turn-00000-of-00001.json
 python3 -m tests.eval --model $MODEL --dataset $EVAL_FILE $@
```

### Comparing `llm_structured_output-0.0.7/_/_mistral_schema.sh` & `llm_structured_output-0.0.8/_/_mistral_schema.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 cd `dirname $0`/../src
 
 LLM=examples.llm_schema
 #MODEL=../local/models/mlx/Mistral-7B-v0.2-Instruct-f16
 #MODEL=./mistral/mlx_model_q4
-#MODEL=mistralai/Mistral-7B-Instruct-v0.2
+MODEL=mistralai/Mistral-7B-Instruct-v0.2
 #MODEL=mlx-community/Mistral-7B-v0.2-4bit
-MODEL=mlx-community/Mixtral-8x22B-4bit
-#MODEL=mlx-community/CodeQwen1.5-7B-Chat-4bit
+#MODEL=mlx-community/Mixtral-8x22B-4bit
+MODEL=mlx-community/Meta-Llama-3-8B-Instruct-4bit
 OPTIONS="--max-tokens 1000 --repeat-prompt --temp 0.8"
 
 PROMPT='[INST] Parse the following address into a JSON object: "27 Barrow St, New York, NY 10014". Your answer should be only a JSON object according to this schema: {"type": "object", "properties": {"streetNumber": {"type": "number"}, "streetName": {"type": "string"}, "city": {"type": {"string"}}, "state": {"type": "string"}, "zipCode": {"type": "number"}}}. Do not explain the result, just output it. Do not add any additional information. [/INST]'
 
 if [ "$1" == "--mixtral" ]; then
   shift
   MODEL=./mixtral/mlx_model_q4
```

### Comparing `llm_structured_output-0.0.7/_/_reluctance.sh` & `llm_structured_output-0.0.8/_/_reluctance.sh`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.7/_/x.py` & `llm_structured_output-0.0.8/_/x.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 import json
 import mlx.core as mx
-from mlx_lm.utils import load # Needs pip import mlx_lm
-from src.llm_structured_output import JsonSchemaAcceptorDriver, HuggingfaceTokenizerHelper, bias_logits
+from mlx_lm.utils import load  # Needs pip import mlx_lm
+from src.llm_structured_output import (
+    JsonSchemaAcceptorDriver,
+    HuggingfaceTokenizerHelper,
+    bias_logits,
+)
 
 
 MODEL_PATH = "mistralai/Mistral-7B-Instruct-v0.2"
 SCHEMA = {
     "type": "object",
     "properties": {
         "streetNumber": {"type": "number"},
         "streetName": {"type": "string"},
         "city": {"type": "string"},
         "state": {"type": "string"},
         "zipCode": {"type": "number"},
     },
 }
-PROMPT = f'''
+PROMPT = f"""
 [INST] Parse the following address into a JSON object: "27 Barrow St, New York, NY 10014".
 Your answer should be only a JSON object according to this schema: {json.dumps(SCHEMA)}
 Do not explain the result, just output it. Do not add any additional information. [/INST]
-'''
+"""
 
 
 # Load the model as usual.
 model, tokenizer = load(MODEL_PATH)
 
 # Instantiate a token acceptor
 tokenizer_helper = HuggingfaceTokenizerHelper(tokenizer)
 vocabulary, eos_id = tokenizer_helper.extract_vocabulary()
 token_acceptor = JsonSchemaAcceptorDriver(SCHEMA, vocabulary, eos_id)
 
 cache = None
 tokens = tokenizer_helper.encode_prompt(PROMPT)
 
 while tokens[-1] != eos_id:
-    # Evaluate the model as usual. 
+    # Evaluate the model as usual.
     logits, cache = model(mx.array(tokens)[None], cache)
 
     # Set probability to -inf for invalid tokens.
     accepted_token_bitmap = token_acceptor.select_valid_tokens()
     logits = bias_logits(mx, logits[0, -1, :], accepted_token_bitmap)
 
     # Sample as usual, e.g.:
```

### Comparing `llm_structured_output-0.0.7/src/examples/json_schema_cli.py` & `llm_structured_output-0.0.8/src/examples/json_schema_cli.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.7/src/examples/llm_schema.py` & `llm_structured_output-0.0.8/src/examples/llm_schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,90 +41,162 @@
 class Model:
     def __init__(self):
         mx.random.seed(0)
         self.model = None
         self.tokenizer = None
         self.vocabulary = None
         self.eos_id = None
+        self._cached_prompt = None
+        self._cached_cache = None
 
     def load(self, model_path: str):
         """
         Load locally or download from Huggingface hub.
         """
         self.model, tokenizer = load(model_path)
         self.tokenizer = HuggingfaceTokenizerHelper(tokenizer)
         self.vocabulary, self.eos_id = self.tokenizer.extract_vocabulary()
 
+    def _run_model(self, inputs: mx.array, cache=None):
+        """
+        This is like the model's __call__() method as implemented in
+        `mlx-examples/llms/mlx_lm/models/*.py`, except it is also able
+        to apply a causal mask once a cache is in place.
+        """
+        model = self.model.model
+        h = model.embed_tokens(inputs)
+
+        mask = None
+        T = h.shape[1]  # pylint: disable=invalid-name
+        if T > 1:
+            if cache is None:
+                S = 0  # pylint: disable=invalid-name
+            else:
+                S = cache[0][0].shape[2]  # pylint: disable=invalid-name
+            mask = nn.MultiHeadAttention.create_additive_causal_mask(S + T)
+            mask = mask.split([S])[1].astype(h.dtype)
+
+        if cache is None:
+            cache = [None] * len(model.layers)
+
+        for e, layer in enumerate(model.layers):
+            h, cache[e] = layer(h, mask, cache[e])
+
+        out = model.norm(h)
+        return self.model.lm_head(out), cache
+
     def _decode(self, tokens):
         return self.tokenizer.no_strip_decode(tokens)
 
-    def sample(self, logits, temp):
+    def _evaluate_prompt(
+        self, prompt: list[int], prior_prompt: list[int] = None, prior_cache=None
+    ):
+        if prior_prompt:
+            i = 0
+            for i, t in enumerate(prior_prompt):
+                if len(prompt) < i or prompt[i] != t:
+                    break
+            cache = [
+                (
+                    layer_key_cache[:, :, :i, :],
+                    layer_value_cache[:, :, :i, :],
+                )
+                for layer_key_cache, layer_value_cache in prior_cache
+            ]
+            tokens = prompt[i:]
+            debug(f"prompt reuse {i}")
+        else:
+            tokens = prompt
+            cache = None
+
+        logits, cache = self._run_model(mx.array(tokens)[None], cache)
+        return logits, cache
+
+    def _debug_top_tokens(self, logits, count=10):
+        token_logits = sorted(
+            enumerate(logits.tolist()), key=itemgetter(1), reverse=True
+        )
+        top_tokens = [
+            (self._decode([t]), p) for t, p in token_logits[:count] if p != -inf
+        ]
+        debug("TOP TOKENS:", top_tokens)
+
+    def _sample(self, logits, temp):
         if temp == 0:
             result = mx.argmax(logits, axis=-1)
         else:
             result = mx.random.categorical(logits * (1 / temp))
         return result.item()
 
-    def generate_without_schema(
-        self, prompt: Iterable[int], temp: Optional[float] = 0.0
-    ):
+    def generate_without_schema(self, logits, cache, temp: Optional[float] = 0.0):
         """
         For testing / comparison purposes.
         """
-        tokens = prompt
-        cache = None
-        while tokens[-1] != self.eos_id:
-            logits, cache = self.model(mx.array(tokens)[None], cache)
-            tokens = [self.sample(logits[0, -1, :], temp)]
+        while True:
+            tokens = [self._sample(logits[0, -1, :], temp)]
             yield tokens
+            if tokens[-1] == self.eos_id:
+                break
+            logits, cache = self.model(mx.array(tokens)[None], cache)
 
     def generate_with_schema(
-        self, prompt: Iterable[int], token_acceptor, temp: Optional[float] = 0.0
+        self, logits, cache, token_acceptor, temp: Optional[float] = 0.0
     ):
-        tokens = prompt
-        cache = None
-        while tokens[-1] != self.eos_id:
-            logits, cache = self.model(mx.array(tokens)[None], cache)
+        while True:
+            t0 = time.time_ns()
             accepted_token_bitmap = token_acceptor.select_valid_tokens()
+            dt = (time.time_ns() - t0) / 1e6
+            if dt > 1:
+                debug(f"select_valid_tokens {dt:.3f}ms")
             if not accepted_token_bitmap:
-                debug("REJECT", token_acceptor.cursors)
-                self._debug_top_tokens(_debug_last_logits, 100)
                 raise RejectedCompletion()
+            t0 = time.time_ns()
             logits = bias_logits(mx, logits[0, -1, :], accepted_token_bitmap)
-            tokens = [self.sample(logits, temp)]
+            dt = (time.time_ns() - t0) / 1e6
+            if dt > 1:
+                debug(f"bias_logits {dt:.3f}ms")
+            tokens = [self._sample(logits, temp)]
             yield tokens
-            _debug_last_cursors = token_acceptor.cursors[:]
-            _debug_last_logits = logits
+            t0 = time.time_ns()
             token_acceptor.advance_token(self._decode(tokens))
+            dt = (time.time_ns() - t0) / 1e6
+            if dt > 1:
+                debug(f"advance_token {dt:.3f}ms")
+            if tokens[-1] == self.eos_id:
+                break
+            t0 = time.time_ns()
+            logits, cache = self.model(mx.array(tokens)[None], cache)
+            dt = (time.time_ns() - t0) / 1e6
+            if dt > 1:
+                debug(f"model {dt:.3f}ms")
 
     def generate_with_preemptive_decoding(
         self,
-        prompt: Iterable[int],
+        logits,
+        cache,
         token_acceptor,
         temp: Optional[float] = 0.0,
         max_batch_size=5,
     ):
         """
-        [Experimental]
         Try to generate faster by precomputing two tokens at a time when possible.
         If we know that the acceptor will only accept a small set of tokens after
         the current one, we can evaluate a batch with one entry per possible
         future token. Each entry in the batch contains the current token sampled,
         which we have to evaluate anyway, and a second token corresponding to one
         of the possible tokens that could be sampled from the output to the first
         token. We get back logits for both tokens for each item in the batch: the
         logits for the first token will be the same (as long as the model applies
         a causal mask), and we can sample those logits to select from which of the
         items in the batch we can select the second token.
         """
-        # Submit prompt for evaluation
-        logits, cache = self._run_model(mx.array(prompt)[None])
+        # Sample token from prompt evaluation
         accepted_token_bitmap = token_acceptor.select_valid_tokens()
         first_token_logits = bias_logits(mx, logits[0, -1, :], accepted_token_bitmap)
-        first_token = self.sample(first_token_logits, temp)
+        first_token = self._sample(first_token_logits, temp)
         tokens = [first_token]
         yield tokens
         token_acceptor.advance_token(self._decode(tokens))
         accepted_token_bitmap = token_acceptor.select_valid_tokens()
 
         while True:
             last_token = tokens[-1]
@@ -145,15 +217,15 @@
             else:  # Otherwise, submit the normal one-token continuation.
                 batch = [[last_token]]
 
             logits, cache = self._run_model(mx.array(batch), cache)
             mx.eval(logits)
 
             first_token_logits = bias_logits(mx, logits[0, 0, :], accepted_token_bitmap)
-            first_token = self.sample(first_token_logits, temp)
+            first_token = self._sample(first_token_logits, temp)
             tokens = [first_token]
 
             if first_token == self.eos_id:
                 yield tokens
                 break
 
             token_acceptor.advance_token(self._decode([first_token]))
@@ -167,15 +239,15 @@
                     i
                     for i, batch_item in enumerate(batch)
                     if batch_item[1] == first_token
                 )
                 second_token_logits = bias_logits(
                     mx, logits[index, 1, :], accepted_token_bitmap
                 )
-                second_token = self.sample(second_token_logits, temp)
+                second_token = self._sample(second_token_logits, temp)
                 tokens.append(second_token)
 
                 token_acceptor.advance_token(self._decode([second_token]))
                 accepted_token_bitmap = token_acceptor.select_valid_tokens()
 
                 # Select the accepted generation in the cache, restoring it to batch dimension 1.
                 cache = [
@@ -186,30 +258,30 @@
                     for layer_key_cache, layer_value_cache in cache
                 ]
 
             yield tokens
 
     def generate_with_preemptive_decoding_constant_batch(
         self,
-        prompt: Iterable[int],
+        logits,
+        cache,
         token_acceptor,
         temp: Optional[float] = 0.0,
         max_batch_size=5,
     ):
         """
         [Experimental]
         Same as generate_with_preemptive_decoding(), but keeping the batch size
-        constant through the generation to have consistent mathix sizes.
+        constant through the generation to have consistent matrix sizes.
         This is just for experimenting with performance.
         """
-        # Submit prompt for evaluation
-        logits, cache = self._run_model(mx.array([prompt] * max_batch_size))
+        # Sample token from prompt evaluation
         accepted_token_bitmap = token_acceptor.select_valid_tokens()
         first_token_logits = bias_logits(mx, logits[0, -1, :], accepted_token_bitmap)
-        first_token = self.sample(first_token_logits, temp)
+        first_token = self._sample(first_token_logits, temp)
         tokens = [first_token]
         yield tokens
         token_acceptor.advance_token(self._decode(tokens))
         accepted_token_bitmap = token_acceptor.select_valid_tokens()
 
         while True:
             last_token = tokens[-1]
@@ -225,15 +297,15 @@
             # Fill up to the batch capacity so that the matrices have the right shape.
             batch_array = mx.array(batch + [batch[-1]] * (max_batch_size - len(batch)))
 
             logits, cache = self._run_model(batch_array, cache)
             mx.eval(logits)
 
             first_token_logits = bias_logits(mx, logits[0, 0, :], accepted_token_bitmap)
-            first_token = self.sample(first_token_logits, temp)
+            first_token = self._sample(first_token_logits, temp)
             tokens = [first_token]
 
             if first_token == self.eos_id:
                 yield tokens
                 break
 
             token_acceptor.advance_token(self._decode([first_token]))
@@ -247,15 +319,15 @@
                     i
                     for i, batch_item in enumerate(batch)
                     if batch_item[1] == first_token
                 )
                 second_token_logits = bias_logits(
                     mx, logits[index, 1, :], accepted_token_bitmap
                 )
-                second_token = self.sample(second_token_logits, temp)
+                second_token = self._sample(second_token_logits, temp)
                 tokens.append(second_token)
 
                 token_acceptor.advance_token(self._decode([second_token]))
                 accepted_token_bitmap = token_acceptor.select_valid_tokens()
 
                 # Select the accepted generation in the cache for the next round.
                 cache = [
@@ -264,130 +336,122 @@
                         mx.array([layer_value_cache[index]] * max_batch_size),
                     )
                     for layer_key_cache, layer_value_cache in cache
                 ]
 
             yield tokens
 
-    def _run_model(self, inputs: mx.array, cache=None):
-        """
-        [Experimental]
-        This is like the model's __call__() method as implemented in
-        `mlx-examples/llms/mlx_lm/models/*.py`, except it is able to apply a
-        causal mask once a cache is in place rather than just for the prompt.
-        """
-        model = self.model.model
-        h = model.embed_tokens(inputs)
+    def _generate_tokens(
+        self,
+        generator: Iterable,
+        max_tokens: int = 1000,
+    ) -> Iterable:
+        start_time = time.time_ns()
+        token_count = 0
 
-        mask = None
-        T = h.shape[1]  # pylint: disable=invalid-name
-        if T > 1:
-            if cache is None:
-                S = 0  # pylint: disable=invalid-name
-            else:
-                S = cache[0][0].shape[2]  # pylint: disable=invalid-name
-            mask = nn.MultiHeadAttention.create_additive_causal_mask(S + T)
-            mask = mask.split([S])[1].astype(h.dtype)
+        for tokens in generator:
+            token_count += len(tokens)
 
-        if cache is None:
-            cache = [None] * len(model.layers)
+            try:
+                eos_index = tokens.index(self.eos_id)
+                tokens = tokens[0:eos_index]
+            except ValueError:
+                eos_index = -1
 
-        for e, layer in enumerate(model.layers):
-            h, cache[e] = layer(h, mask, cache[e])
+            if tokens:
+                text = self._decode(tokens)
+                yield {
+                    "op": "generatedTokens",
+                    "text": text,
+                    "token_count": len(tokens),
+                    "time_ms": (time.time_ns() - start_time) / 1e6,
+                }
 
-        out = model.norm(h)
-        return self.model.lm_head(out), cache
+            if eos_index >= 0:
+                yield {"op": "stop", "reason": "end"}
+                return
+
+            if token_count >= max_tokens:
+                yield {"op": "stop", "reason": "max_tokens"}
+                return
+
+            start_time = time.time_ns()
+
+        assert False
 
     def completion(
         self,
         prompt: Union[str, Iterable[dict[str, str]]],
         schema: dict,
         encapsulated: bool = False,
         max_tokens: int = 1000,
         temp: float = 0.0,
         seed: int = None,
         preemptive_batch_size: int = 0,
+        cache_prompt: bool = False,
     ):
         if seed is not None:
             mx.random.seed(seed)
 
+        start_time = time.time_ns()
         prompt_tokens = self.tokenizer.encode_prompt(prompt)
+        logits, cache = self._evaluate_prompt(
+            prompt_tokens, self._cached_prompt, self._cached_cache
+        )
+        if cache_prompt:
+            self._cached_prompt = prompt_tokens
+            self._cached_cache = cache
+        # Eager eval to more accurately reflect the prompt evaluation time.
+        mx.eval(logits)
+        prompt_time = time.time_ns() - start_time
+        yield {
+            "op": "evaluatedPrompt",
+            "prompt": prompt,
+            "token_count": len(prompt_tokens),
+            "time_ms": prompt_time / 1e6,
+            "prompt_tps": len(prompt_tokens) / (prompt_time / 1e9),
+        }
 
         if schema:
             token_acceptor = JsonSchemaAcceptorDriver(
                 schema,
                 self.vocabulary,
                 self.eos_id,
                 is_encapsulated_json=encapsulated,
             )
             if preemptive_batch_size > 0:
                 generator = self.generate_with_preemptive_decoding(
-                    prompt_tokens,
+                    logits,
+                    cache,
                     token_acceptor,
                     temp,
                     max_batch_size=preemptive_batch_size,
                 )
             else:
                 generator = self.generate_with_schema(
-                    prompt_tokens, token_acceptor, temp
+                    logits, cache, token_acceptor, temp
                 )
         else:
-            generator = self.generate_without_schema(prompt_tokens, temp)
-
-        start_time = time.time_ns()
+            generator = self.generate_without_schema(logits, cache, temp)
 
         token_count = 0
-        for tokens in generator:
-            if not token_count:
-                yield {
-                    "op": "evaluatedPrompt",
-                    "prompt": prompt,
-                    "token_count": len(prompt_tokens),
-                    "time_ms": (time.time_ns() - start_time) / 1e6,
-                }
-                start_time = time.time_ns()
-
-            token_count += len(tokens)
-
-            try:
-                eos_index = tokens.index(self.eos_id)
-            except ValueError:
-                eos_index = -1
-            if eos_index >= 0:
-                tokens = tokens[0:eos_index]
-
-            if tokens:
-                text = self._decode(tokens)
-                yield {
-                    "op": "generatedTokens",
-                    "text": text,
-                    "token_count": len(tokens),
-                    "time_ms": (time.time_ns() - start_time) / 1e6,
-                }
-
-            if eos_index >= 0:
-                yield {"op": "stop", "reason": "end"}
-                return
-
-            if token_count == max_tokens:
-                yield {"op": "stop", "reason": "max_tokens"}
-                return
-
-            start_time = time.time_ns()
-
-        assert False
-
-    def _debug_top_tokens(self, logits, count=10):
-        token_logits = sorted(
-            enumerate(logits.tolist()), key=itemgetter(1), reverse=True
-        )
-        top_tokens = [
-            (self._decode([t]), p) for t, p in token_logits[:count] if p != -inf
-        ]
-        debug("TOP TOKENS:", top_tokens)
+        generation_time = 0
+        for generation_result in self._generate_tokens(generator, max_tokens):
+            if generation_result["op"] == "generatedTokens":
+                token_count += generation_result["token_count"]
+                generation_time += generation_result["time_ms"]
+            elif generation_result["op"] == "stop":
+                generation_result["token_count"] = token_count
+                generation_result["time_ms"] = generation_time
+                # This is slightly incorrect, because the first token is generated
+                # from the prompt evaluation.
+                generation_result["generation_tps"] = token_count / (
+                    generation_time / 1e3
+                )
+            yield generation_result
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="LLM inference script with schema-constrained sampling"
     )
     parser.add_argument(
@@ -447,43 +511,39 @@
     if args.schema is not None:
         schema = json.loads(args.schema)
         info("Using schema")
     else:
         schema = None
     info("Starting generation...")
 
-    generated_token_count = 0
-    generation_time = 0.0
-
     for result in model.completion(
         prompt=args.prompt,
         schema=schema,
         encapsulated=args.encapsulated,
         max_tokens=args.max_tokens,
         temp=args.temp,
         seed=args.seed,
         preemptive_batch_size=args.preemptive,
     ):
         if result["op"] == "evaluatedPrompt":
             prompt_token_count = result["token_count"]
             prompt_time = result["time_ms"]
+            prompt_tps = result["prompt_tps"]
             if args.repeat_prompt:
                 bolddim(result["prompt"], flush=True)
         elif result["op"] == "generatedTokens":
-            generated_token_count += result["token_count"]
-            generation_time += result["time_ms"]
             bold(result["text"], end="", flush=True)
         elif result["op"] == "stop":
             end_reason = result["reason"]
+            generated_token_count = result["token_count"]
+            generation_time = result["time_ms"]
+            generation_tps = result["generation_tps"]
         else:
             assert False
 
-    prompt_tps = prompt_token_count / (prompt_time / 1e3)
-    generation_tps = generated_token_count / (generation_time / 1e3)
-
     print()
     info(f"End reason: {end_reason}")
     info(f"Tokens: prompt {prompt_token_count}, generation {generated_token_count}")
     info(f"Tokens per second: prompt {prompt_tps:.2f}, generation {generation_tps:.2f}")
     info(f"Total time: prompt {prompt_time:.2f}ms, generation {generation_time:.2f}ms")
```

### Comparing `llm_structured_output-0.0.7/src/examples/reluctance.py` & `llm_structured_output-0.0.8/src/examples/reluctance.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.7/src/examples/server.py` & `llm_structured_output-0.0.8/src/examples/server.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.7/src/llm_structured_output/acceptor.py` & `llm_structured_output-0.0.8/src/llm_structured_output/acceptor.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,19 +176,17 @@
             multiple times with different inputs. See clone() method above.
             Override.
             """
             return []
 
         def in_accepted_state(self) -> bool:
             """
-            Returns True if the cursor has reached a final state.  Note that a cursor
-            in an accepted state can also continue to advance if other final states are
-            possible with additional input. A cursor that has reached a final state and
-            cannot advance further should return an empty iterable in advance().
-            Override.
+            Returns True if the cursor has reached a final state.
+            Typically, rather than override you should return an AcceptedState object
+            in the advance() method when the state is reached after consuming input.
             """
             return False
 
         def get_value(self):
             """
             Retuns the current value of the cursor as defined by itself. This can be
             either the ongoing representation of its temporary state, or its final value
@@ -269,21 +267,33 @@
                 )
                 debug_prune_start = time_ns()
             total_time = (time_ns() - debug_start) / 1e6
             debug_output_fn(f"{debug_prefix} {total_time=:.02f}ms")
             return bitmap
 
         def __repr__(self):
-            if self.in_accepted_state():
-                accepted = "✅"
-            else:
-                accepted = ""
-            return (
-                f"{accepted}{type(self).__qualname__}(value={repr(self.get_value())})"
-            )
+            return f"{type(self).__qualname__}(value={repr(self.get_value())})"
+
+
+class AcceptedState(TokenAcceptor.Cursor):
+    """
+    Holds a cursor that has reached the accepted state.
+    """
+
+    def __init__(self, cursor: TokenAcceptor.Cursor):
+        self.cursor = cursor
+
+    def in_accepted_state(self):
+        return True
+
+    def get_value(self):
+        return self.cursor.get_value()
+
+    def __repr__(self):
+        return f"✅{repr(self.cursor)}"
 
 
 class CharAcceptor(TokenAcceptor):
     """
     Accept one character iff is in the set of expected characters.
     """
 
@@ -296,27 +306,20 @@
         """
 
         def __init__(self, acceptor, value=None):
             self.acceptor = acceptor
             self.value = value
 
         def select(self, candidate_chars):
-            if self.value is not None:
-                return []
             return self.acceptor.charset
 
         def advance(self, char):
-            if self.in_accepted_state():
-                return []
             # Because we implemented the select method, we are guaranteed that the
             # char is in our accepted set.
-            return [CharAcceptor.Cursor(self.acceptor, char)]
-
-        def in_accepted_state(self):
-            return self.value is not None
+            return [AcceptedState(CharAcceptor.Cursor(self.acceptor, char))]
 
         def get_value(self):
             return self.value
 
 
 class TextAcceptor(TokenAcceptor):
     """
@@ -340,25 +343,21 @@
         """
 
         def __init__(self, acceptor, pos=0):
             self.acceptor = acceptor
             self.pos = pos
 
         def select(self, candidate_chars):
-            if self.pos == len(self.acceptor.text):
-                return []
             return self.acceptor.text[self.pos]
 
         def advance(self, char):
-            # Because we implemented the select method, the character is guaranteed
-            # to match.
-            return [TextAcceptor.Cursor(self.acceptor, self.pos + 1)]
-
-        def in_accepted_state(self):
-            return self.pos == len(self.acceptor.text)
+            next_cursor = TextAcceptor.Cursor(self.acceptor, self.pos + 1)
+            if next_cursor.pos == len(self.acceptor.text):
+                return [AcceptedState(next_cursor)]
+            return [next_cursor]
 
         def get_value(self) -> str:
             head = self.acceptor.text[0 : self.pos]
             tail = self.acceptor.text[self.pos :]
             if len(tail):
                 return f"{head}👉{tail}"
             else:
@@ -396,51 +395,55 @@
         try:
             edges = self.get_edges(cursor.current_state)
         except (KeyError, IndexError, TypeError):
             assert cursor.current_state in self.end_states
             return []
         cursors = []
         for transition_acceptor, target_state in edges:
-            if cursor.can_attempt_transition(transition_acceptor, target_state):
+            if cursor.start_transition(transition_acceptor, target_state):
                 for transition_cursor in transition_acceptor.get_cursors():
                     copy = cursor.clone()
                     copy.transition_cursor = transition_cursor
                     copy.target_state = target_state
-                    cursors.append(copy)
-                    # Handle optional acceptors like WhitespaceAcceptor
+                    # Handle cursors that start in an accepted state,
+                    # e.g. EmptyTransition, WhitespaceAcceptor
                     if transition_cursor.in_accepted_state():
                         new_visited_states = visited_states + [cursor.current_state]
                         assert target_state not in new_visited_states  # Infinite loop
                         cursors += self._cascade_transition(
                             copy, new_visited_states, traversed_edges
                         )
+                    else:
+                        cursors.append(copy)
         return cursors
 
     def _cascade_transition(self, cursor, visited_states, traversed_edges):
         assert cursor.transition_cursor.in_accepted_state()
-        # Copy before validation to allow for side effects, e.g. storing the value
+        # Copy before validation to allow for cursor mutation, e.g. storing the transition_value
         cursors = []
         copy: StateMachineAcceptor.Cursor = cursor.clone()
-        if copy.can_complete_transition(
+        if copy.complete_transition(
             copy.transition_cursor.get_value(),
             copy.target_state,
             copy.target_state in copy.acceptor.end_states,
         ):
             copy.current_state = copy.target_state
             copy.target_state = None
-            copy.accept_history = copy.accept_history + [copy.transition_cursor]
+            copy.accept_history = copy.accept_history + [copy.transition_cursor.cursor]
             copy.transition_cursor = None
             # De-duplicate cursors that have reached the same state with the same value.
             # This prevents combinatorial explosion because of e.g. empty transitions.
             state_value = (copy.current_state, repr(copy.get_value()))
             if state_value not in traversed_edges:
                 traversed_edges.add(state_value)
-                if copy.in_accepted_state():
-                    cursors.append(copy)
-                cursors += self._find_transitions(copy, visited_states, traversed_edges)
+                if copy.current_state in self.end_states:
+                    cursors.append(AcceptedState(copy))
+                cursors += self._find_transitions(
+                    copy, visited_states, traversed_edges
+                )
         return cursors
 
     class Cursor(TokenAcceptor.Cursor):
         """
         Cursor for StateMachineAcceptor
         """
 
@@ -469,54 +472,49 @@
         def advance(self, char):
             next_cursors = []
             traversed_edges = set()
             for followup_cursor in self.transition_cursor.advance(char):
                 copy = self.clone()
                 # pylint: disable-next=attribute-defined-outside-init
                 copy.transition_cursor = followup_cursor
-                next_cursors.append(copy)
                 if followup_cursor.in_accepted_state():
                     # pylint: disable-next=protected-access
                     next_cursors += self.acceptor._cascade_transition(
                         copy, [], traversed_edges
                     )
+                else:
+                    next_cursors.append(copy)
             return next_cursors
 
         # pylint: disable-next=unused-argument
-        def can_attempt_transition(self, transition_acceptor, target_state) -> bool:
+        def start_transition(self, transition_acceptor, target_state) -> bool:
             """
-            Override to prevent an edge to be traversed
+            Override to prevent an edge to be traversed.
             """
             return True
 
-        def can_complete_transition(  # pylint: disable-next=unused-argument
+        def complete_transition(  # pylint: disable-next=unused-argument
             self, transition_value, target_state, is_end_state
         ) -> bool:
             """
-            Override to perform additional checks on the acceptee
+            Override to perform additional checks on the acceptee and mutate the cursor
+            with the transition_value as appropriate.
             """
             return True
 
-        def in_accepted_state(self) -> bool:
-            return self.current_state in self.acceptor.end_states
-
         def get_value(self):
             value = [
                 accepted_transition_cursor.get_value()
                 for accepted_transition_cursor in self.accept_history
             ]
             if self.transition_cursor is not None:
                 value.append(self.transition_cursor.get_value())
             return value
 
         def __repr__(self) -> str:
-            if self.in_accepted_state():
-                accepted = "✅"
-            else:
-                accepted = ""
             if self.transition_cursor is not None:
                 transition_cursor = repr(self.transition_cursor)
                 target_state = self.target_state
             else:
                 transition_cursor = "None"
                 target_state = "None"
             if self.accept_history:
@@ -533,42 +531,38 @@
                         "".join(
                             [
                                 str(accepted_transition_cursor.get_value())
                                 for accepted_transition_cursor in accept_history
                             ]
                         )
                     )
-                    + "⬅️  "
                 )
             else:
                 history = ""
             state = (
-                f"{history}{self.current_state}=>{target_state} ➡️ {transition_cursor}"
+                f"{history} {self.current_state}⇒{target_state}  {transition_cursor}"
             )
-            return f"{accepted}{type(self).__qualname__}({state})"
+            return f"{type(self).__qualname__}({state})"
 
     class EmptyTransitionAcceptor(TokenAcceptor):
         """
         Faux acceptor that allows to create empty transition edges in a state
         machine graph for convenience in expressing complex graphs.
         An empty edge skips the current state altogether, without the need to
         consume input.
         """
 
+        def get_cursors(self):
+            return [AcceptedState(self.Cursor(self))]
+
         class Cursor(TokenAcceptor.Cursor):
             """
             Cursor for EmptyTransitionAcceptor
             """
 
-            def select(self, candidate_chars):
-                return set()
-
-            def in_accepted_state(self):
-                return True
-
             def get_value(self):
                 return ""
 
     # Singleton EmptyTransitionAcceptor
     EmptyTransition = EmptyTransitionAcceptor()
 
 
@@ -603,37 +597,27 @@
         Cursor for WaitForAcceptor
         """
 
         def __init__(self, acceptor, cursors=None):
             self.acceptor = acceptor
             if cursors:
                 self.cursors = cursors
-                self.accepted_cursor = next(
-                    (cursor for cursor in cursors if cursor.in_accepted_state()), None
-                )
             else:
                 self.cursors = acceptor.wait_for_acceptor.get_cursors()
-                self.accepted_cursor = None
 
         def matches_all(self):
-            return not self.in_accepted_state()
+            return True
 
         def select(self, candidate_chars):
-            if self.in_accepted_state():
-                return set()
-            else:
-                return candidate_chars
+            return candidate_chars
 
         def advance(self, char):
-            if self.in_accepted_state():
-                return []
             cursors = TokenAcceptor.advance_all(self.cursors, char)
+            accepted_cursor = next(
+                (cursor for cursor in cursors if cursor.in_accepted_state()), None
+            )
+            if accepted_cursor:
+                return [AcceptedState(accepted_cursor)]
             return [WaitForAcceptor.Cursor(self.acceptor, cursors)]
 
-        def in_accepted_state(self):
-            return self.accepted_cursor is not None
-
         def get_value(self):
-            if self.accepted_cursor is not None:
-                return self.accepted_cursor.get_value()
-            else:
-                return f"Waiting for {repr(self.cursors)}"
+            return f"Waiting for {repr(self.cursors)}"
```

### Comparing `llm_structured_output-0.0.7/src/llm_structured_output/json_acceptor.py` & `llm_structured_output-0.0.8/src/llm_structured_output/json_acceptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Acceptors for JSON parsing or constraning LLM generation to JSON outputs.
 """
 
 import json
 
 from .acceptor import (
     TokenAcceptor,
+    AcceptedState,
     CharAcceptor,
     StateMachineAcceptor,
     SequenceAcceptor,
     TextAcceptor,
 )
 from .util.tokentrie import TokenTrie
 
@@ -75,14 +76,19 @@
             return cls._cached_tries[trie_id]
         collapsed_trie = WhitespaceTokenTrie.from_trie(
             trie, WhitespaceAcceptor.WHITESPACE
         )
         cls._cached_tries[trie_id] = collapsed_trie
         return collapsed_trie
 
+    def get_cursors(self):
+        # Whitespace is optional
+        cursor = WhitespaceAcceptor.Cursor(self)
+        return [cursor, AcceptedState(cursor)]
+
     class Cursor(TokenAcceptor.Cursor):
         """
         Cursor for WhitespaceAcceptor
         """
 
         def __init__(self, acceptor, text=""):
             self.text = text
@@ -103,18 +109,17 @@
                 # generations. If the LLM triggers this often, consider whether the LLM is
                 # suitable for emitting JSON and/or whether the task is achievable and makes sense
                 # with the information provided in the prompt.
                 return super().prune(TokenTrie())
             return super().prune(WhitespaceAcceptor.prepare_trie(trie))
 
         def advance(self, char):
-            return [WhitespaceAcceptor.Cursor(None, self.text + char)]
-
-        def in_accepted_state(self):
-            return True
+            # More whitespace is optional
+            next_cursor = WhitespaceAcceptor.Cursor(None, self.text + char)
+            return [next_cursor, AcceptedState(next_cursor)]
 
         def get_value(self):
             return self.text
 
 
 class BooleanAcceptor(StateMachineAcceptor):
     """
@@ -129,15 +134,15 @@
         Cursor for BooleanAcceptor
         """
 
         def __init__(self, acceptor):
             super().__init__(acceptor)
             self.value = None
 
-        def can_complete_transition(self, transition_value, target_state, is_end_state):
+        def complete_transition(self, transition_value, target_state, is_end_state):
             if is_end_state:
                 if transition_value == "true":
                     self.value = True
                 else:
                     assert transition_value == "false"
                     self.value = False
             return True
@@ -220,32 +225,25 @@
         """
 
         def __init__(self, acceptor, value=None):
             self.acceptor = acceptor
             self.value = value
 
         def select(self, candidate_chars):
-            if self.in_accepted_state():
-                return []
             return candidate_chars - StringCharAcceptor.INVALID_CHARS
 
         def prune(self, trie):
             """
             Use a custom matching trie to avoid an explosion of valid options that
             are equivalent from the point of view of token matching.
             """
             return super().prune(StringCharAcceptor.prepare_trie(trie))
 
         def advance(self, char):
-            if self.in_accepted_state():
-                return []
-            return [StringCharAcceptor.Cursor(self.acceptor, char)]
-
-        def in_accepted_state(self):
-            return self.value is not None
+            return [AcceptedState(StringCharAcceptor.Cursor(self.acceptor, char))]
 
         def get_value(self):
             return self.value
 
 
 class StringAcceptor(StateMachineAcceptor):
     """
@@ -275,15 +273,15 @@
 
         def __init__(self, acceptor):
             super().__init__(acceptor)
             self.text = ""
             self.length = 0
             self.value = None
 
-        def can_complete_transition(self, transition_value, target_state, is_end_state):
+        def complete_transition(self, transition_value, target_state, is_end_state):
             self.text += transition_value
             if target_state == 1 and self.current_state != 0:
                 self.length += 1
             if is_end_state:
                 self.value = json.loads(self.text)
             return True
 
@@ -328,15 +326,15 @@
         """
 
         def __init__(self, acceptor):
             super().__init__(acceptor)
             self.text = ""
             self.value = None
 
-        def can_complete_transition(self, transition_value, target_state, is_end_state):
+        def complete_transition(self, transition_value, target_state, is_end_state):
             self.text += transition_value
             if is_end_state:
                 self.value = json.loads(self.text)
             return True
 
         def get_value(self):
             if self.value is None:
@@ -369,15 +367,15 @@
         Cursor for ArrayAcceptor
         """
 
         def __init__(self, acceptor):
             super().__init__(acceptor)
             self.value = []
 
-        def can_complete_transition(
+        def complete_transition(
             self, transition_value, target_state, is_end_state
         ) -> bool:
             if self.current_state == 3:
                 self.value.append(transition_value)
             return True
 
 
@@ -406,15 +404,15 @@
         Cursor for ObjectAcceptor
         """
 
         def __init__(self, acceptor):
             super().__init__(acceptor)
             self.value = {}
 
-        def can_complete_transition(
+        def complete_transition(
             self, transition_value, target_state, is_end_state
         ) -> bool:
             if self.current_state == 3:
                 prop_name, prop_value = transition_value
                 self.value[prop_name] = prop_value
             return True
 
@@ -443,15 +441,15 @@
             """
 
             def __init__(self, acceptor):
                 super().__init__(acceptor)
                 self.prop_name = None
                 self.prop_value = None
 
-            def can_complete_transition(
+            def complete_transition(
                 self, transition_value, target_state, is_end_state
             ) -> bool:
                 if target_state == 1:
                     self.prop_name = transition_value
                 elif is_end_state:
                     self.prop_value = transition_value
                 return True
```

### Comparing `llm_structured_output-0.0.7/src/llm_structured_output/json_schema_acceptor.py` & `llm_structured_output-0.0.8/src/llm_structured_output/json_schema_acceptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,24 +96,24 @@
         Cursor for StringSchemaAcceptor
         """
 
         def __init__(self, acceptor):
             super().__init__(acceptor)
             self.acceptor = acceptor
 
-        def can_attempt_transition(self, transition_acceptor, target_state):
+        def start_transition(self, transition_acceptor, target_state):
             if self.current_state == 1:
                 if target_state == "$":
                     return self.length >= self.acceptor.min_length()
                 else:
                     return self.length < self.acceptor.max_length()
             return True
 
-        def can_complete_transition(self, transition_value, target_state, is_end_state):
-            if not super().can_complete_transition(
+        def complete_transition(self, transition_value, target_state, is_end_state):
+            if not super().complete_transition(
                 transition_value, target_state, is_end_state
             ):
                 return False
             if is_end_state:
                 return self.acceptor.validate_value(self.get_value())
             return True
 
@@ -157,16 +157,16 @@
         Cursor for NumberAcceptor
         """
 
         def __init__(self, acceptor):
             super().__init__(acceptor)
             self.acceptor = acceptor
 
-        def can_complete_transition(self, transition_value, target_state, is_end_state):
-            if not super().can_complete_transition(
+        def complete_transition(self, transition_value, target_state, is_end_state):
+            if not super().complete_transition(
                 transition_value, target_state, is_end_state
             ):
                 return False
             if is_end_state:
                 return self.acceptor.validate_value(self.get_value())
             return True
 
@@ -236,15 +236,15 @@
         Cursor for ArrayAcceptor
         """
 
         def __init__(self, acceptor):
             super().__init__(acceptor)
             self.acceptor = acceptor
 
-        def can_attempt_transition(self, transition_acceptor, target_state) -> bool:
+        def start_transition(self, transition_acceptor, target_state) -> bool:
             if self.current_state == 4 and target_state == 2:
                 return len(self.value) < self.acceptor.max_items()
             if target_state == "$":
                 return len(self.value) >= self.acceptor.min_items()
             return True
 
 
@@ -340,15 +340,15 @@
         Cursor for ObjectAcceptor
         """
 
         def __init__(self, acceptor):
             super().__init__(acceptor)
             self.acceptor = acceptor
 
-        def can_attempt_transition(self, transition_acceptor, target_state) -> bool:
+        def start_transition(self, transition_acceptor, target_state) -> bool:
             if target_state == "$":
                 return all(
                     prop_name in self.value
                     for prop_name in self.acceptor.required_property_names()
                 )
             if self.current_state == 3 and target_state == 4:
                 # Is a property already set?
```

### Comparing `llm_structured_output-0.0.7/src/llm_structured_output/util/bitmap.py` & `llm_structured_output-0.0.8/src/llm_structured_output/util/bitmap.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.7/src/llm_structured_output/util/output.py` & `llm_structured_output-0.0.8/src/llm_structured_output/util/output.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.7/src/llm_structured_output/util/tokenization.py` & `llm_structured_output-0.0.8/src/llm_structured_output/util/tokenization.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.7/src/llm_structured_output/util/tokentrie.py` & `llm_structured_output-0.0.8/src/llm_structured_output/util/tokentrie.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.7/src/tests/eval.py` & `llm_structured_output-0.0.8/src/tests/eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     for result in model.completion(
         messages,
         schema=schema,
         max_tokens=4000,
         temp=temp,
         seed=seed,
         preemptive_batch_size=preemptive_batch_size,
+        cache_prompt=True,
     ):
         if result["op"] == "evaluatedPrompt":
             prompt_tokens += result["token_count"]
             prompt_time = result["time_ms"]
         elif result["op"] == "generatedTokens":
             completion_tokens += result["token_count"]
             completion_time += result["time_ms"]
```

### Comparing `llm_structured_output-0.0.7/LICENSE` & `llm_structured_output-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.7/README.md` & `llm_structured_output-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.7/pyproject.toml` & `llm_structured_output-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "llm_structured_output"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Oscar D.P. Triscon", email="github@triscon.com" },
 ]
 description = "Constrain LLM generation to structured output, such as function calling a.k.a. tool use"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `llm_structured_output-0.0.7/PKG-INFO` & `llm_structured_output-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: llm_structured_output
-Version: 0.0.7
+Version: 0.0.8
 Summary: Constrain LLM generation to structured output, such as function calling a.k.a. tool use
 Project-URL: Homepage, https://github.com/otriscon/llm-structured-output
 Project-URL: Issues, https://github.com/otriscon/llm-structured-output/issues
 Author-email: "Oscar D.P. Triscon" <github@triscon.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

