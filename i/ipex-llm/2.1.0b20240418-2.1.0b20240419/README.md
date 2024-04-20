# Comparing `tmp/ipex_llm-2.1.0b20240418-py3-none-win_amd64.whl.zip` & `tmp/ipex_llm-2.1.0b20240419-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5348168 bytes, number of entries: 218
+Zip file size: 5348051 bytes, number of entries: 218
 -rw-------  2.0 unx     1898 b- defN 24-Mar-25 11:36 ipex_llm/__init__.py
 -rw-------  2.0 unx     6816 b- defN 24-Mar-25 11:36 ipex_llm/convert_model.py
 -rw-------  2.0 unx     3091 b- defN 24-Apr-17 15:07 ipex_llm/llm_patching.py
 -rw-------  2.0 unx     1177 b- defN 24-Mar-25 11:36 ipex_llm/models.py
 -rw-------  2.0 unx    12404 b- defN 24-Apr-18 12:34 ipex_llm/optimize.py
 -rw-------  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-chat.ps1
 -rwx------  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-cli.ps1
@@ -38,47 +38,47 @@
 -rw-------  2.0 unx     1189 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/__init__.py
 -rw-------  2.0 unx    13589 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/bigdlllm.py
 -rw-------  2.0 unx     7225 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/transformersembeddings.py
 -rw-------  2.0 unx     1636 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/__init__.py
 -rw-------  2.0 unx    24438 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/bigdlllm.py
 -rw-------  2.0 unx    10576 b- defN 24-Apr-03 15:07 ipex_llm/langchain/llms/transformersllm.py
 -rw-------  2.0 unx     7379 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/transformerspipelinellm.py
--rw-------  2.0 unx        0 b- defN 24-Apr-18 12:34 ipex_llm/libs/__init__.py
--rw-------  2.0 unx    36352 b- defN 24-Apr-18 12:34 ipex_llm/libs/bloom-api.dll
--rw-------  2.0 unx   460288 b- defN 24-Apr-18 12:34 ipex_llm/libs/bloom.dll
--rw-------  2.0 unx   852992 b- defN 24-Apr-18 12:34 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
--rw-------  2.0 unx   856064 b- defN 24-Apr-18 12:34 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
--rw-------  2.0 unx   843776 b- defN 24-Apr-18 12:34 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
--rw-------  2.0 unx    24576 b- defN 24-Apr-18 12:34 ipex_llm/libs/gptneox-api.dll
--rw-------  2.0 unx   520192 b- defN 24-Apr-18 12:34 ipex_llm/libs/gptneox.dll
--rw-------  2.0 unx   485888 b- defN 24-Apr-18 12:34 ipex_llm/libs/libbloom_avx.dll
--rw-------  2.0 unx   460800 b- defN 24-Apr-18 12:34 ipex_llm/libs/libbloom_vnni.dll
--rw-------  2.0 unx   545792 b- defN 24-Apr-18 12:34 ipex_llm/libs/libgptneox_avx.dll
--rw-------  2.0 unx   520704 b- defN 24-Apr-18 12:34 ipex_llm/libs/libgptneox_vnni.dll
--rw-------  2.0 unx   540160 b- defN 24-Apr-18 12:34 ipex_llm/libs/libllama_avx.dll
--rw-------  2.0 unx   515072 b- defN 24-Apr-18 12:34 ipex_llm/libs/libllama_vnni.dll
--rw-------  2.0 unx   577024 b- defN 24-Apr-18 12:34 ipex_llm/libs/libstarcoder_avx.dll
--rw-------  2.0 unx   551936 b- defN 24-Apr-18 12:34 ipex_llm/libs/libstarcoder_vnni.dll
--rw-------  2.0 unx    25088 b- defN 24-Apr-18 12:34 ipex_llm/libs/llama-api.dll
--rw-------  2.0 unx   514560 b- defN 24-Apr-18 12:34 ipex_llm/libs/llama.dll
--rw-------  2.0 unx   103424 b- defN 24-Apr-18 12:34 ipex_llm/libs/main-bloom.exe
--rw-------  2.0 unx   726016 b- defN 24-Apr-18 12:34 ipex_llm/libs/main-chatglm_vnni.exe
--rw-------  2.0 unx    98816 b- defN 24-Apr-18 12:34 ipex_llm/libs/main-gptneox.exe
--rw-------  2.0 unx    99840 b- defN 24-Apr-18 12:34 ipex_llm/libs/main-llama.exe
--rw-------  2.0 unx   157696 b- defN 24-Apr-18 12:34 ipex_llm/libs/main-starcoder.exe
--rw-------  2.0 unx   125952 b- defN 24-Apr-18 12:34 ipex_llm/libs/quantize-bloom.exe
--rw-------  2.0 unx   127488 b- defN 24-Apr-18 12:34 ipex_llm/libs/quantize-bloom_vnni.exe
--rw-------  2.0 unx   103936 b- defN 24-Apr-18 12:34 ipex_llm/libs/quantize-gptneox.exe
--rw-------  2.0 unx   104448 b- defN 24-Apr-18 12:34 ipex_llm/libs/quantize-gptneox_vnni.exe
--rw-------  2.0 unx   109056 b- defN 24-Apr-18 12:34 ipex_llm/libs/quantize-llama.exe
--rw-------  2.0 unx   110080 b- defN 24-Apr-18 12:34 ipex_llm/libs/quantize-llama_vnni.exe
--rw-------  2.0 unx   126976 b- defN 24-Apr-18 12:34 ipex_llm/libs/quantize-starcoder.exe
--rw-------  2.0 unx   128000 b- defN 24-Apr-18 12:34 ipex_llm/libs/quantize-starcoder_vnni.exe
--rw-------  2.0 unx    21504 b- defN 24-Apr-18 12:34 ipex_llm/libs/starcoder-api.dll
--rw-------  2.0 unx   551424 b- defN 24-Apr-18 12:34 ipex_llm/libs/starcoder.dll
+-rw-------  2.0 unx        0 b- defN 24-Apr-19 15:10 ipex_llm/libs/__init__.py
+-rw-------  2.0 unx    36352 b- defN 24-Apr-19 15:10 ipex_llm/libs/bloom-api.dll
+-rw-------  2.0 unx   460288 b- defN 24-Apr-19 15:10 ipex_llm/libs/bloom.dll
+-rw-------  2.0 unx   852992 b- defN 24-Apr-19 15:10 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
+-rw-------  2.0 unx   856064 b- defN 24-Apr-19 15:10 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
+-rw-------  2.0 unx   843776 b- defN 24-Apr-19 15:10 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
+-rw-------  2.0 unx    24576 b- defN 24-Apr-19 15:10 ipex_llm/libs/gptneox-api.dll
+-rw-------  2.0 unx   520192 b- defN 24-Apr-19 15:10 ipex_llm/libs/gptneox.dll
+-rw-------  2.0 unx   485888 b- defN 24-Apr-19 15:10 ipex_llm/libs/libbloom_avx.dll
+-rw-------  2.0 unx   460800 b- defN 24-Apr-19 15:10 ipex_llm/libs/libbloom_vnni.dll
+-rw-------  2.0 unx   545792 b- defN 24-Apr-19 15:10 ipex_llm/libs/libgptneox_avx.dll
+-rw-------  2.0 unx   520704 b- defN 24-Apr-19 15:10 ipex_llm/libs/libgptneox_vnni.dll
+-rw-------  2.0 unx   540160 b- defN 24-Apr-19 15:10 ipex_llm/libs/libllama_avx.dll
+-rw-------  2.0 unx   515072 b- defN 24-Apr-19 15:10 ipex_llm/libs/libllama_vnni.dll
+-rw-------  2.0 unx   577024 b- defN 24-Apr-19 15:10 ipex_llm/libs/libstarcoder_avx.dll
+-rw-------  2.0 unx   551936 b- defN 24-Apr-19 15:10 ipex_llm/libs/libstarcoder_vnni.dll
+-rw-------  2.0 unx    25088 b- defN 24-Apr-19 15:10 ipex_llm/libs/llama-api.dll
+-rw-------  2.0 unx   514560 b- defN 24-Apr-19 15:10 ipex_llm/libs/llama.dll
+-rw-------  2.0 unx   103424 b- defN 24-Apr-19 15:10 ipex_llm/libs/main-bloom.exe
+-rw-------  2.0 unx   726016 b- defN 24-Apr-19 15:10 ipex_llm/libs/main-chatglm_vnni.exe
+-rw-------  2.0 unx    98816 b- defN 24-Apr-19 15:10 ipex_llm/libs/main-gptneox.exe
+-rw-------  2.0 unx    99840 b- defN 24-Apr-19 15:10 ipex_llm/libs/main-llama.exe
+-rw-------  2.0 unx   157696 b- defN 24-Apr-19 15:10 ipex_llm/libs/main-starcoder.exe
+-rw-------  2.0 unx   125952 b- defN 24-Apr-19 15:10 ipex_llm/libs/quantize-bloom.exe
+-rw-------  2.0 unx   127488 b- defN 24-Apr-19 15:10 ipex_llm/libs/quantize-bloom_vnni.exe
+-rw-------  2.0 unx   103936 b- defN 24-Apr-19 15:10 ipex_llm/libs/quantize-gptneox.exe
+-rw-------  2.0 unx   104448 b- defN 24-Apr-19 15:10 ipex_llm/libs/quantize-gptneox_vnni.exe
+-rw-------  2.0 unx   109056 b- defN 24-Apr-19 15:10 ipex_llm/libs/quantize-llama.exe
+-rw-------  2.0 unx   110080 b- defN 24-Apr-19 15:10 ipex_llm/libs/quantize-llama_vnni.exe
+-rw-------  2.0 unx   126976 b- defN 24-Apr-19 15:10 ipex_llm/libs/quantize-starcoder.exe
+-rw-------  2.0 unx   128000 b- defN 24-Apr-19 15:10 ipex_llm/libs/quantize-starcoder_vnni.exe
+-rw-------  2.0 unx    21504 b- defN 24-Apr-19 15:10 ipex_llm/libs/starcoder-api.dll
+-rw-------  2.0 unx   551424 b- defN 24-Apr-19 15:10 ipex_llm/libs/starcoder.dll
 -rw-------  2.0 unx      874 b- defN 24-Mar-25 11:36 ipex_llm/llamaindex/__init__.py
 -rw-------  2.0 unx     1139 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/__init__.py
 -rw-------  2.0 unx    26314 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/bigdlllm.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/__init__.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/__init__.py
 -rw-------  2.0 unx    10084 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/bigdl_llm_model.py
 -rw-------  2.0 unx    11371 b- defN 24-Mar-27 11:49 ipex_llm/serving/fastchat/ipex_llm_worker.py
@@ -94,15 +94,15 @@
 -rw-------  2.0 unx     5429 b- defN 24-Mar-25 11:36 ipex_llm/transformers/loader.py
 -rw-------  2.0 unx    14719 b- defN 24-Apr-17 15:07 ipex_llm/transformers/lookup.py
 -rw-------  2.0 unx    38388 b- defN 24-Apr-18 12:34 ipex_llm/transformers/low_bit_linear.py
 -rw-------  2.0 unx    36157 b- defN 24-Apr-18 12:34 ipex_llm/transformers/model.py
 -rw-------  2.0 unx     6921 b- defN 24-Mar-25 11:36 ipex_llm/transformers/modelling_bigdl.py
 -rw-------  2.0 unx    14770 b- defN 24-Mar-25 11:36 ipex_llm/transformers/qlora.py
 -rw-------  2.0 unx    16567 b- defN 24-Mar-25 11:36 ipex_llm/transformers/relora.py
--rw-------  2.0 unx    54512 b- defN 24-Apr-17 15:07 ipex_llm/transformers/speculative.py
+-rw-------  2.0 unx    55517 b- defN 24-Apr-19 15:09 ipex_llm/transformers/speculative.py
 -rw-------  2.0 unx     8404 b- defN 24-Mar-25 11:36 ipex_llm/transformers/training_patch.py
 -rw-------  2.0 unx    13931 b- defN 24-Apr-18 12:34 ipex_llm/transformers/utils.py
 -rw-------  2.0 unx     7611 b- defN 24-Mar-25 11:36 ipex_llm/transformers/xpu_customize_fwd.py
 -rw-------  2.0 unx      875 b- defN 24-Mar-25 11:36 ipex_llm/transformers/awq/__init__.py
 -rw-------  2.0 unx     2172 b- defN 24-Mar-25 11:36 ipex_llm/transformers/awq/act.py
 -rw-------  2.0 unx     8861 b- defN 24-Mar-25 11:36 ipex_llm/transformers/awq/awq.py
 -rw-------  2.0 unx     4422 b- defN 24-Mar-25 11:36 ipex_llm/transformers/awq/awq_config.py
@@ -129,28 +129,28 @@
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/transformers/gguf/models/model_implement/yuan2/__init__.py
 -rw-------  2.0 unx     2192 b- defN 24-Mar-25 11:36 ipex_llm/transformers/gguf/models/model_implement/yuan2/configuration_yuan.py
 -rw-------  2.0 unx    51084 b- defN 24-Mar-25 11:36 ipex_llm/transformers/gguf/models/model_implement/yuan2/yuan_hf_model.py
 -rw-------  2.0 unx     2658 b- defN 24-Mar-25 11:36 ipex_llm/transformers/layers/rope_embedding.py
 -rw-------  2.0 unx      584 b- defN 24-Mar-25 11:36 ipex_llm/transformers/models/__init__.py
 -rw-------  2.0 unx     7415 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/aquila.py
 -rw-------  2.0 unx    24488 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/baichuan.py
--rw-------  2.0 unx    27214 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/baichuan2.py
+-rw-------  2.0 unx    27116 b- defN 24-Apr-19 15:09 ipex_llm/transformers/models/baichuan2.py
 -rw-------  2.0 unx     6085 b- defN 24-Mar-25 11:36 ipex_llm/transformers/models/bert.py
 -rw-------  2.0 unx     8971 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/bloom.py
 -rw-------  2.0 unx    13743 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/chatglm.py
--rw-------  2.0 unx    32040 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/chatglm2.py
+-rw-------  2.0 unx    31942 b- defN 24-Apr-19 15:09 ipex_llm/transformers/models/chatglm2.py
 -rw-------  2.0 unx     8697 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/chatglm2_32k.py
 -rw-------  2.0 unx     8654 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/decilm.py
 -rw-------  2.0 unx    33549 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/falcon.py
--rw-------  2.0 unx    12408 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/gemma.py
+-rw-------  2.0 unx    12310 b- defN 24-Apr-19 15:09 ipex_llm/transformers/models/gemma.py
 -rw-------  2.0 unx     4342 b- defN 24-Mar-25 11:36 ipex_llm/transformers/models/gptbigcode.py
 -rw-------  2.0 unx    17973 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/gptj.py
 -rw-------  2.0 unx     6219 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/gptneox.py
 -rw-------  2.0 unx    11647 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/internlm.py
--rw-------  2.0 unx    98235 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/llama.py
+-rw-------  2.0 unx    97385 b- defN 24-Apr-19 15:09 ipex_llm/transformers/models/llama.py
 -rw-------  2.0 unx    45181 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/mistral.py
 -rw-------  2.0 unx    27273 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/mixtral.py
 -rw-------  2.0 unx     9540 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/mpt.py
 -rw-------  2.0 unx     6268 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/phixtral.py
 -rw-------  2.0 unx    32349 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/qwen.py
 -rw-------  2.0 unx    32725 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/qwen2.py
 -rw-------  2.0 unx    30334 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/qwen2_moe.py
@@ -206,15 +206,15 @@
 -rw-------  2.0 unx     8707 b- defN 24-Mar-25 11:36 ipex_llm/vllm/transformers_utils/tokenizer.py
 -rw-------  2.0 unx    13950 b- defN 24-Mar-25 11:36 ipex_llm/vllm/worker/worker.py
 -rw-------  2.0 unx      585 b- defN 24-Apr-18 12:34 ipex_llm/vllm2/__init__.py
 -rw-------  2.0 unx     7208 b- defN 24-Apr-18 12:34 ipex_llm/vllm2/model_convert.py
 -rw-------  2.0 unx      747 b- defN 24-Apr-18 12:34 ipex_llm/vllm2/engine/__init__.py
 -rw-------  2.0 unx     5715 b- defN 24-Apr-18 12:34 ipex_llm/vllm2/engine/engine.py
 -rw-------  2.0 unx    10475 b- defN 24-Apr-18 12:34 ipex_llm/vllm2/entrypoints/openai/api_server.py
--rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240418.data/scripts/llm-chat.ps1
--rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240418.data/scripts/llm-cli.ps1
--rw-------  2.0 unx     4400 b- defN 24-Apr-18 12:34 ipex_llm-2.1.0b20240418.dist-info/METADATA
--rw-------  2.0 unx       98 b- defN 24-Apr-18 12:34 ipex_llm-2.1.0b20240418.dist-info/WHEEL
--rw-------  2.0 unx       61 b- defN 24-Apr-18 12:34 ipex_llm-2.1.0b20240418.dist-info/entry_points.txt
--rw-------  2.0 unx        9 b- defN 24-Apr-18 12:34 ipex_llm-2.1.0b20240418.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    20723 b- defN 24-Apr-18 12:34 ipex_llm-2.1.0b20240418.dist-info/RECORD
-218 files, 13087230 bytes uncompressed, 5315042 bytes compressed:  59.4%
+-rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240419.data/scripts/llm-chat.ps1
+-rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240419.data/scripts/llm-cli.ps1
+-rw-------  2.0 unx     4400 b- defN 24-Apr-19 15:10 ipex_llm-2.1.0b20240419.dist-info/METADATA
+-rw-------  2.0 unx       98 b- defN 24-Apr-19 15:10 ipex_llm-2.1.0b20240419.dist-info/WHEEL
+-rw-------  2.0 unx       61 b- defN 24-Apr-19 15:10 ipex_llm-2.1.0b20240419.dist-info/entry_points.txt
+-rw-------  2.0 unx        9 b- defN 24-Apr-19 15:10 ipex_llm-2.1.0b20240419.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    20723 b- defN 24-Apr-19 15:10 ipex_llm-2.1.0b20240419.dist-info/RECORD
+218 files, 13087091 bytes uncompressed, 5314925 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -627,29 +627,29 @@
 
 Filename: ipex_llm/vllm2/engine/engine.py
 Comment: 
 
 Filename: ipex_llm/vllm2/entrypoints/openai/api_server.py
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240418.data/scripts/llm-chat.ps1
+Filename: ipex_llm-2.1.0b20240419.data/scripts/llm-chat.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240418.data/scripts/llm-cli.ps1
+Filename: ipex_llm-2.1.0b20240419.data/scripts/llm-cli.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240418.dist-info/METADATA
+Filename: ipex_llm-2.1.0b20240419.dist-info/METADATA
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240418.dist-info/WHEEL
+Filename: ipex_llm-2.1.0b20240419.dist-info/WHEEL
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240418.dist-info/entry_points.txt
+Filename: ipex_llm-2.1.0b20240419.dist-info/entry_points.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240418.dist-info/top_level.txt
+Filename: ipex_llm-2.1.0b20240419.dist-info/top_level.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240418.dist-info/RECORD
+Filename: ipex_llm-2.1.0b20240419.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipex_llm/libs/bloom-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800036cc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 18 12:33:26 2024
+Time/Date		Fri Apr 19 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000003200
 SizeOfInitializedData	0000000000005e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000036cc
@@ -6375,16 +6375,16 @@
    180005621:	push   %rdx
    180005622:	add    %al,0x1(%rax)
    180005628:	pop    %rax
    180005629:	push   %rdx
    18000562a:	add    %al,0x1(%rax)
    180005630:	add    %al,(%rax)
    180005632:	add    %al,(%rax)
-   180005634:	(bad)
-   180005635:	adc    (%rcx),%esp
+   180005634:	xchg   %eax,%ecx
+   180005635:	xchg   %esp,(%rdx)
    180005637:	data16 add %al,(%rax)
    18000563a:	add    %al,(%rax)
    18000563c:	or     $0xe0000000,%eax
    180005641:	add    (%rax),%al
    180005643:	add    %cl,(%rcx,%rbx,2)
    180005646:	add    %al,(%rax)
    180005648:	or     $0x3f,%al
```

## ipex_llm/libs/bloom.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180052e48
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 18 12:33:26 2024
+Time/Date		Fri Apr 19 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000053400
 SizeOfInitializedData	00000000000bee00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000052e48
@@ -109410,19 +109410,17 @@
    18005c7ba:	add    $0x180,%eax
    18005c7bf:	add    %dh,0x56(%rax)
    18005c7c2:	add    $0x180,%eax
    18005c7c7:	add    %bh,0x56(%rax)
    18005c7ca:	add    $0x180,%eax
    18005c7cf:	add    %al,(%rax)
    18005c7d1:	add    %al,(%rax)
-   18005c7d3:	add    %dl,(%rsi)
-   18005c7d5:	adc    (%rcx),%esp
-   18005c7d7:	data16 add %al,(%rax)
-   18005c7da:	add    %al,(%rax)
-   18005c7dc:	or     $0x50000000,%eax
+   18005c7d3:	add    %dl,0x662287(%rcx)
+   18005c7d9:	add    %al,(%rax)
+   18005c7db:	add    %cl,0x50000000(%rip)        # 0x1d005c7e1
    18005c7e1:	add    (%rax),%eax
    18005c7e3:	add    %ah,-0x5ffffa2f(%rax)
    18005c7e9:	mov    $0x5,%ecx
 	...
    18005c7fe:	add    %al,(%rax)
    18005c800:	adc    %dl,%ch
    18005c802:	add    $0x180,%eax
```

## ipex_llm/libs/gptneox-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002cbc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 18 12:33:25 2024
+Time/Date		Fri Apr 19 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002600
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002cbc
@@ -5058,17 +5058,19 @@
    1800049c0:	cmp    %al,0x0(%rdx)
    1800049c3:	addb   $0x0,(%rcx)
    1800049c6:	add    %al,(%rax)
    1800049c8:	rex
    1800049c9:	rex.X add %al,0x1(%rax)
    1800049d0:	add    %al,(%rax)
    1800049d2:	add    %al,(%rax)
-   1800049d4:	adc    $0x662113,%eax
-   1800049d9:	add    %al,(%rax)
-   1800049db:	add    %cl,-0x20000000(%rip)        # 0x1600049e1
+   1800049d4:	xchg   %eax,%ecx
+   1800049d5:	xchg   %esp,(%rdx)
+   1800049d7:	data16 add %al,(%rax)
+   1800049da:	add    %al,(%rax)
+   1800049dc:	or     $0xe0000000,%eax
    1800049e1:	add    (%rax),%al
    1800049e3:	add    %ah,0x0(%rsp,%rcx,2)
    1800049e7:	add    %ah,0x0(%rsi,%rsi,1)
 	...
    1800049ff:	add    %al,(%rcx)
 	...
    180004a09:	add    %al,(%rax)
```

## ipex_llm/libs/gptneox.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005a5a8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 18 12:33:26 2024
+Time/Date		Fri Apr 19 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005ae00
 SizeOfInitializedData	00000000000c6000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005a5a8
@@ -120845,16 +120845,16 @@
    18006307d:	add    %al,(%rax)
    18006307f:	add    %bh,0x18005c6(%rax)
    180063085:	add    %al,(%rax)
    180063087:	add    %al,%al
    180063089:	movb   $0x0,0x180(%rip)        # 0x180063210
    180063090:	add    %al,(%rax)
    180063092:	add    %al,(%rax)
-   180063094:	(bad)
-   180063095:	adc    (%rcx),%esp
+   180063094:	xchg   %eax,%ecx
+   180063095:	xchg   %esp,(%rdx)
    180063097:	data16 add %al,(%rax)
    18006309a:	add    %al,(%rax)
    18006309c:	or     $0x50000000,%eax
    1800630a1:	add    (%rax),%eax
    1800630a3:	add    %al,0x2f040006(,%rdi,1)
    1800630aa:	(bad)
 	...
```

## ipex_llm/libs/libbloom_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180058c38
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 18 12:28:59 2024
+Time/Date		Fri Apr 19 15:03:46 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000059200
 SizeOfInitializedData	00000000000bf400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000058c38
@@ -114727,16 +114727,16 @@
    1800626ed:	add    %al,(%rax)
    1800626ef:	add    %dh,-0x4a(%rax)
    1800626f2:	add    $0x180,%eax
    1800626f7:	add    %bh,-0x4a(%rax)
    1800626fa:	add    $0x180,%eax
    1800626ff:	add    %al,(%rax)
    180062701:	add    %al,(%rax)
-   180062703:	add    %cl,(%rbx)
-   180062705:	adc    (%rcx),%ah
+   180062703:	add    %dl,%dl
+   180062705:	xchg   %esp,(%rdx)
    180062707:	data16 add %al,(%rax)
    18006270a:	add    %al,(%rax)
    18006270c:	or     $0x50000000,%eax
    180062711:	add    (%rax),%eax
    180062713:	add    %ah,(%rax)
    180062715:	xor    %eax,(%rsi)
    180062717:	add    %ah,(%rax)
```

## ipex_llm/libs/libbloom_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180053058
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 18 12:30:01 2024
+Time/Date		Fri Apr 19 15:05:17 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000053600
 SizeOfInitializedData	00000000000bee00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000053058
@@ -109461,16 +109461,15 @@
    18005c79a:	add    $0x180,%eax
    18005c79f:	add    %dh,0x56(%rax)
    18005c7a2:	add    $0x180,%eax
    18005c7a7:	add    %bh,0x56(%rax)
    18005c7aa:	add    $0x180,%eax
    18005c7af:	add    %al,(%rax)
    18005c7b1:	add    %al,(%rax)
-   18005c7b3:	add    %cl,0x12(%rcx)
-   18005c7b6:	and    %esp,0x0(%rsi)
+   18005c7b3:	add    %ch,0x662288(%rip)        # 0x1806bea41
    18005c7b9:	add    %al,(%rax)
    18005c7bb:	add    %cl,0x50000000(%rip)        # 0x1d005c7c1
    18005c7c1:	add    (%rax),%eax
    18005c7c3:	add    %ah,-0x5ffffa2f(%rax)
    18005c7c9:	mov    $0x5,%ebx
 	...
    18005c7fe:	add    %al,(%rax)
```

## ipex_llm/libs/libgptneox_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180060428
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 18 12:28:59 2024
+Time/Date		Fri Apr 19 15:03:46 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000060c00
 SizeOfInitializedData	00000000000c6600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000060428
@@ -126192,18 +126192,17 @@
    180068fb5:	add    %al,(%rax)
    180068fb7:	add    %al,%al
    180068fb9:	es (bad)
    180068fbb:	addb   $0x0,(%rcx)
    180068fbe:	add    %al,(%rax)
    180068fc0:	add    %al,(%rax)
    180068fc2:	add    %al,(%rax)
-   180068fc4:	or     (%rdx),%edx
-   180068fc6:	and    %esp,0x0(%rsi)
-   180068fc9:	add    %al,(%rax)
-   180068fcb:	add    %cl,0x50000000(%rip)        # 0x1d0068fd1
+   180068fc4:	rolb   %cl,0x6622(%rdi)
+   180068fca:	add    %al,(%rax)
+   180068fcc:	or     $0x50000000,%eax
    180068fd1:	add    (%rax),%eax
    180068fd3:	add    %al,(%rsp,%rbx,4)
    180068fd6:	(bad)
    180068fd7:	add    %al,(%rsp,%rcx,4)
    180068fda:	(bad)
 	...
    180068fff:	add    %bh,-0x61(%rax)
```

## ipex_llm/libs/libgptneox_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005a7b8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 18 12:30:01 2024
+Time/Date		Fri Apr 19 15:05:18 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005b000
 SizeOfInitializedData	00000000000c6000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005a7b8
@@ -121007,15 +121007,15 @@
    18006305d:	add    %al,(%rax)
    18006305f:	add    %bh,0x18005c6(%rax)
    180063065:	add    %al,(%rax)
    180063067:	add    %al,%al
    180063069:	movb   $0x0,0x180(%rip)        # 0x1800631f0
    180063070:	add    %al,(%rax)
    180063072:	add    %al,(%rax)
-   180063074:	rex.WB adc (%r9),%spl
+   180063074:	cs mov %ah,(%rdx)
    180063077:	data16 add %al,(%rax)
    18006307a:	add    %al,(%rax)
    18006307c:	or     $0x50000000,%eax
    180063081:	add    (%rax),%eax
    180063083:	add    %al,0x31040006(,%rdi,1)
    18006308a:	(bad)
 	...
```

## ipex_llm/libs/libllama_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005f138
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 18 12:28:59 2024
+Time/Date		Fri Apr 19 15:03:46 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005f800
 SizeOfInitializedData	00000000000c6400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005f138
@@ -124880,18 +124880,17 @@
    180068096:	add    %al,(%rax)
    180068098:	rclb   $1,(%rsi)
    18006809a:	(bad)
    18006809b:	addb   $0x0,(%rcx)
    18006809e:	add    %al,(%rax)
    1800680a0:	add    %al,(%rax)
    1800680a2:	add    %al,(%rax)
-   1800680a4:	or     (%rdx),%edx
-   1800680a6:	and    %esp,0x0(%rsi)
-   1800680a9:	add    %al,(%rax)
-   1800680ab:	add    %cl,0x50000000(%rip)        # 0x1d00680b1
+   1800680a4:	rolb   %cl,0x6622(%rdi)
+   1800680aa:	add    %al,(%rax)
+   1800680ac:	or     $0x50000000,%eax
    1800680b1:	add    (%rax),%eax
    1800680b3:	add    %al,(%rax)
    1800680b5:	lea    (%rsi),%eax
    1800680b7:	add    %al,(%rax)
    1800680b9:	jns    0x1800680c1
 	...
    1800680ff:	add    %dh,-0x70(%rax)
```

## ipex_llm/libs/libllama_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800594c8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 18 12:30:01 2024
+Time/Date		Fri Apr 19 15:05:18 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000059c00
 SizeOfInitializedData	00000000000c5e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000594c8
@@ -119683,15 +119683,15 @@
    180062140:	enter  $0x5b6,$0x80
    180062144:	add    %eax,(%rax)
    180062146:	add    %al,(%rax)
    180062148:	shlb   $1,0x18005(%rsi)
    18006214e:	add    %al,(%rax)
    180062150:	add    %al,(%rax)
    180062152:	add    %al,(%rax)
-   180062154:	rex.WB adc (%r9),%spl
+   180062154:	cs mov %ah,(%rdx)
    180062157:	data16 add %al,(%rax)
    18006215a:	add    %al,(%rax)
    18006215c:	or     $0x50000000,%eax
    180062161:	add    (%rax),%eax
    180062163:	add    %al,-0x7ffff9d3(%rax)
    180062169:	sbb    $0x6,%eax
 	...
```

## ipex_llm/libs/libstarcoder_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180066598
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 18 12:28:59 2024
+Time/Date		Fri Apr 19 15:03:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000066c00
 SizeOfInitializedData	00000000000c8000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000066598
@@ -135439,18 +135439,17 @@
    18006fbe5:	add    %al,(%rax)
    18006fbe7:	add    %al,%al
    18006fbe9:	xchg   %al,(%rsi)
    18006fbeb:	addb   $0x0,(%rcx)
    18006fbee:	add    %al,(%rax)
    18006fbf0:	add    %al,(%rax)
    18006fbf2:	add    %al,(%rax)
-   18006fbf4:	or     (%rdx),%edx
-   18006fbf6:	and    %esp,0x0(%rsi)
-   18006fbf9:	add    %al,(%rax)
-   18006fbfb:	add    %cl,0x50000000(%rip)        # 0x1d006fc01
+   18006fbf4:	roll   $1,0x6622(%rdi)
+   18006fbfa:	add    %al,(%rax)
+   18006fbfc:	or     $0x50000000,%eax
    18006fc01:	add    (%rax),%eax
    18006fc03:	add    %dl,%al
    18006fc05:	or     $0xfdd00007,%eax
    18006fc0a:	(bad)
 	...
    18006fc7f:	add    %al,0x11(%rax)
    18006fc82:	(bad)
```

## ipex_llm/libs/libstarcoder_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800609b8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 18 12:30:01 2024
+Time/Date		Fri Apr 19 15:05:17 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000061000
 SizeOfInitializedData	00000000000c7a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000609b8
@@ -130151,18 +130151,17 @@
    180069cb5:	add    %al,(%rax)
    180069cb7:	add    %al,%al
    180069cb9:	es (bad)
    180069cbb:	addb   $0x0,(%rcx)
    180069cbe:	add    %al,(%rax)
    180069cc0:	add    %al,(%rax)
    180069cc2:	add    %al,(%rax)
-   180069cc4:	rex.WB adc (%r9),%spl
-   180069cc7:	data16 add %al,(%rax)
-   180069cca:	add    %al,(%rax)
-   180069ccc:	or     $0x50000000,%eax
+   180069cc4:	sub    $0x662288,%eax
+   180069cc9:	add    %al,(%rax)
+   180069ccb:	add    %cl,0x50000000(%rip)        # 0x1d0069cd1
    180069cd1:	add    (%rax),%eax
    180069cd3:	add    %dl,-0x52(%rax)
    180069cd6:	(bad)
    180069cd7:	add    %dl,-0x5e(%rax)
    180069cda:	(bad)
 	...
    180069cff:	add    %al,%al
```

## ipex_llm/libs/llama-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002dac
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 18 12:33:25 2024
+Time/Date		Fri Apr 19 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002800
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002dac
@@ -5355,17 +5355,19 @@
    180004a20:	cmp    %al,0x0(%rdx)
    180004a23:	addb   $0x0,(%rcx)
    180004a26:	add    %al,(%rax)
    180004a28:	rex
    180004a29:	rex.X add %al,0x1(%rax)
    180004a30:	add    %al,(%rax)
    180004a32:	add    %al,(%rax)
-   180004a34:	adc    $0x662113,%eax
-   180004a39:	add    %al,(%rax)
-   180004a3b:	add    %cl,-0x20000000(%rip)        # 0x160004a41
+   180004a34:	xchg   %eax,%ecx
+   180004a35:	xchg   %esp,(%rdx)
+   180004a37:	data16 add %al,(%rax)
+   180004a3a:	add    %al,(%rax)
+   180004a3c:	or     $0xe0000000,%eax
    180004a41:	add    (%rax),%al
    180004a43:	add    %ah,%ah
    180004a45:	rex.WR add %r8b,(%rax)
    180004a48:	in     $0x38,%al
 	...
    180004a7e:	add    %al,(%rax)
    180004a80:	add    %eax,(%rax)
```

## ipex_llm/libs/llama.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800592b8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 18 12:33:26 2024
+Time/Date		Fri Apr 19 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000059a00
 SizeOfInitializedData	00000000000c5e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000592b8
@@ -119535,16 +119535,16 @@
    180062160:	enter  $0x5b6,$0x80
    180062164:	add    %eax,(%rax)
    180062166:	add    %al,(%rax)
    180062168:	shlb   $1,0x18005(%rsi)
    18006216e:	add    %al,(%rax)
    180062170:	add    %al,(%rax)
    180062172:	add    %al,(%rax)
-   180062174:	(bad)
-   180062175:	adc    (%rcx),%esp
+   180062174:	xchg   %eax,%ecx
+   180062175:	xchg   %esp,(%rdx)
    180062177:	data16 add %al,(%rax)
    18006217a:	add    %al,(%rax)
    18006217c:	or     $0x50000000,%eax
    180062181:	add    (%rax),%eax
    180062183:	add    %al,(%rax)
    180062185:	cs (bad)
    180062187:	add    %al,(%rax)
```

## ipex_llm/libs/main-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001045c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu Apr 18 12:33:26 2024
+Time/Date		Fri Apr 19 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010800
 SizeOfInitializedData	0000000000008e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001045c
@@ -25509,16 +25509,16 @@
    140014ab0:	enter  $0x125,$0x40
    140014ab4:	add    %eax,(%rax)
    140014ab6:	add    %al,(%rax)
    140014ab8:	shlb   $1,0x14001(%rip)        # 0x140028abf
    140014abe:	add    %al,(%rax)
    140014ac0:	add    %al,(%rax)
    140014ac2:	add    %al,(%rax)
-   140014ac4:	(bad)
-   140014ac5:	adc    (%rcx),%esp
+   140014ac4:	xchg   %eax,%ecx
+   140014ac5:	xchg   %esp,(%rdx)
    140014ac7:	data16 add %al,(%rax)
    140014aca:	add    %al,(%rax)
    140014acc:	or     $0x20000000,%eax
    140014ad1:	add    (%rax),%eax
    140014ad3:	add    %cl,%ah
    140014ad5:	push   %rsp
    140014ad6:	add    %eax,(%rax)
```

## ipex_llm/libs/main-chatglm_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400836cc
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu Apr 18 12:30:28 2024
+Time/Date		Fri Apr 19 15:05:43 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000087c00
 SizeOfInitializedData	00000000000cbe00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000836cc
@@ -189024,18 +189024,18 @@
    140093ea5:	add    %al,(%rax)
    140093ea7:	add    %al,(%rax)
    140093ea9:	cltd
    140093eaa:	or     %al,0x1(%rax)
    140093ead:	add    %al,(%rax)
    140093eaf:	add    %al,(%rax)
    140093eb1:	add    %al,(%rax)
-   140093eb3:	add    %ah,0x21(%rdx,%rdx,1)
-   140093eb7:	data16 add %al,(%rax)
-   140093eba:	add    %al,(%rax)
-   140093ebc:	or     $0xcc000000,%eax
+   140093eb3:	add    %al,-0x78(%rdi)
+   140093eb6:	and    0x0(%rsi),%ah
+   140093eb9:	add    %al,(%rax)
+   140093ebb:	add    %cl,-0x34000000(%rip)        # 0x10c093ec1
    140093ec1:	add    (%rax),%eax
    140093ec3:	add    %dl,(%rax)
    140093ec5:	jae    0x140093ed0
    140093ec7:	add    %dl,(%rax)
    140093ec9:	movsxd (%rcx),%ecx
 	...
    140093eff:	add    %al,(%rax)
```

## ipex_llm/libs/main-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000ef6c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu Apr 18 12:33:26 2024
+Time/Date		Fri Apr 19 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f200
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000ef6c
@@ -24136,16 +24136,16 @@
    140013edf:	add    %ch,%al
    140013ee1:	adc    $0x14001,%eax
    140013ee6:	add    %al,(%rax)
    140013ee8:	lock adc $0x14001,%eax
    140013eee:	add    %al,(%rax)
    140013ef0:	add    %al,(%rax)
    140013ef2:	add    %al,(%rax)
-   140013ef4:	(bad)
-   140013ef5:	adc    (%rcx),%esp
+   140013ef4:	xchg   %eax,%ecx
+   140013ef5:	xchg   %esp,(%rdx)
    140013ef7:	data16 add %al,(%rax)
    140013efa:	add    %al,(%rax)
    140013efc:	or     $0x90000000,%eax
    140013f01:	add    (%rax),%eax
    140013f03:	add    %ch,0x1(%rcx,%rcx,2)
    140013f07:	add    %ch,0x1(%rdi,%rbp,1)
 	...
```

## ipex_llm/libs/main-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000f32c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu Apr 18 12:33:26 2024
+Time/Date		Fri Apr 19 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f600
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000f32c
@@ -24679,16 +24679,16 @@
    140013faf:	add    %ch,%al
    140013fb1:	adc    $0x14001,%eax
    140013fb6:	add    %al,(%rax)
    140013fb8:	lock adc $0x14001,%eax
    140013fbe:	add    %al,(%rax)
    140013fc0:	add    %al,(%rax)
    140013fc2:	add    %al,(%rax)
-   140013fc4:	(bad)
-   140013fc5:	adc    (%rcx),%esp
+   140013fc4:	xchg   %eax,%ecx
+   140013fc5:	xchg   %esp,(%rdx)
    140013fc7:	data16 add %al,(%rax)
    140013fca:	add    %al,(%rax)
    140013fcc:	or     $0x90000000,%eax
    140013fd1:	add    (%rax),%eax
    140013fd3:	add    %ch,%ah
    140013fd5:	add    %rax,(%r8)
    140013fd8:	in     (%dx),%al
```

## ipex_llm/libs/main-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001a85c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu Apr 18 12:33:26 2024
+Time/Date		Fri Apr 19 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000001b000
 SizeOfInitializedData	000000000000bc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001a85c
@@ -40341,19 +40341,17 @@
    14001f111:	movb   $0x40,(%rcx)
    14001f114:	add    %eax,(%rax)
    14001f116:	add    %al,(%rax)
    14001f118:	push   $0x14001c6
    14001f11d:	add    %al,(%rax)
    14001f11f:	add    %al,(%rax)
    14001f121:	add    %al,(%rax)
-   14001f123:	add    %dl,(%rsi)
-   14001f125:	adc    (%rcx),%esp
-   14001f127:	data16 add %al,(%rax)
-   14001f12a:	add    %al,(%rax)
-   14001f12c:	or     $0x20000000,%eax
+   14001f123:	add    %dl,0x662287(%rcx)
+   14001f129:	add    %al,(%rax)
+   14001f12b:	add    %cl,0x20000000(%rip)        # 0x16001f131
    14001f131:	add    (%rax),%eax
    14001f133:	add    %dl,(%rbx,%rax,1)
    14001f136:	add    (%rax),%al
    14001f138:	adc    $0xf7,%al
    14001f13a:	add    %eax,(%rax)
 	...
    14001f180:	add    %eax,(%rax)
```

## ipex_llm/libs/quantize-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013918
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu Apr 18 12:33:26 2024
+Time/Date		Fri Apr 19 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013a00
 SizeOfInitializedData	00000000000acc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013918
@@ -32227,19 +32227,17 @@
    1400191a5:	add    %al,(%rax)
    1400191a7:	add    %al,(%rax)
    1400191a9:	push   %rbp
    1400191aa:	add    %eax,0x1(%rax)
    1400191ad:	add    %al,(%rax)
    1400191af:	add    %al,(%rax)
    1400191b1:	add    %al,(%rax)
-   1400191b3:	add    %dl,(%rsi)
-   1400191b5:	adc    (%rcx),%esp
-   1400191b7:	data16 add %al,(%rax)
-   1400191ba:	add    %al,(%rax)
-   1400191bc:	or     $0x20000000,%eax
+   1400191b3:	add    %dl,0x662287(%rcx)
+   1400191b9:	add    %al,(%rax)
+   1400191bb:	add    %cl,0x20000000(%rip)        # 0x1600191c1
    1400191c1:	add    (%rax),%eax
    1400191c3:	add    %dh,-0x5f(%rax)
    1400191c6:	add    %eax,(%rax)
    1400191c8:	jo     0x140019159
    1400191ca:	add    %eax,(%rax)
 	...
    140019200:	add    %eax,(%rax)
```

## ipex_llm/libs/quantize-bloom_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013b28
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu Apr 18 12:30:01 2024
+Time/Date		Fri Apr 19 15:05:17 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ad000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013b28
@@ -32344,16 +32344,15 @@
    140019185:	add    %al,(%rax)
    140019187:	add    %al,(%rax)
    140019189:	push   %rbp
    14001918a:	add    %eax,0x1(%rax)
    14001918d:	add    %al,(%rax)
    14001918f:	add    %al,(%rax)
    140019191:	add    %al,(%rax)
-   140019193:	add    %cl,0x12(%rcx)
-   140019196:	and    %esp,0x0(%rsi)
+   140019193:	add    %ch,0x662288(%rip)        # 0x14067b421
    140019199:	add    %al,(%rax)
    14001919b:	add    %cl,0x20000000(%rip)        # 0x1600191a1
    1400191a1:	add    (%rax),%eax
    1400191a3:	add    %dh,-0x5f(%rax)
    1400191a6:	add    %eax,(%rax)
    1400191a8:	jo     0x14001913b
    1400191aa:	add    %eax,(%rax)
```

## ipex_llm/libs/quantize-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010988
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu Apr 18 12:33:25 2024
+Time/Date		Fri Apr 19 15:02:40 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010a00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010988
@@ -27188,15 +27188,15 @@
    140015f80:	push   $0x1400123
    140015f85:	add    %al,(%rax)
    140015f87:	add    %dh,0x23(%rax)
    140015f8a:	add    %eax,0x1(%rax)
    140015f8d:	add    %al,(%rax)
    140015f8f:	add    %al,(%rax)
    140015f91:	add    %al,(%rax)
-   140015f93:	add    %dl,0x662113(%rip)        # 0x1406780ac
+   140015f93:	add    %dl,0x662287(%rax)
    140015f99:	add    %al,(%rax)
    140015f9b:	add    %cl,-0x70000000(%rip)        # 0xd0015fa1
    140015fa1:	add    (%rax),%eax
    140015fa3:	add    %ch,0x65(%rax)
    140015fa6:	add    %eax,(%rax)
    140015fa8:	push   $0x153
 	...
```

## ipex_llm/libs/quantize-gptneox_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010b98
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu Apr 18 12:30:00 2024
+Time/Date		Fri Apr 19 15:05:16 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010c00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010b98
@@ -27296,16 +27296,16 @@
    140015f60:	push   $0x1400123
    140015f65:	add    %al,(%rax)
    140015f67:	add    %dh,0x23(%rax)
    140015f6a:	add    %eax,0x1(%rax)
    140015f6d:	add    %al,(%rax)
    140015f6f:	add    %al,(%rax)
    140015f71:	add    %al,(%rax)
-   140015f73:	add    %cl,0x12(%rax)
-   140015f76:	and    %esp,0x0(%rsi)
+   140015f73:	add    %ch,(%rax,%rcx,4)
+   140015f76:	and    0x0(%rsi),%ah
    140015f79:	add    %al,(%rax)
    140015f7b:	add    %cl,-0x70000000(%rip)        # 0xd0015f81
    140015f81:	add    (%rax),%eax
    140015f83:	add    %ch,0x65(%rax)
    140015f86:	add    %eax,(%rax)
    140015f88:	push   $0x155
 	...
```

## ipex_llm/libs/quantize-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400118e8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu Apr 18 12:33:25 2024
+Time/Date		Fri Apr 19 15:02:40 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011800
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000118e8
@@ -28454,15 +28454,15 @@
    14001706d:	add    %al,(%rax)
    14001706f:	add    %cl,0x1400133(%rax)
    140017075:	add    %al,(%rax)
    140017077:	add    %dl,0x1400133(%rax)
    14001707d:	add    %al,(%rax)
    14001707f:	add    %al,(%rax)
    140017081:	add    %al,(%rax)
-   140017083:	add    %dl,0x662113(%rip)        # 0x14067919c
+   140017083:	add    %dl,0x662287(%rax)
    140017089:	add    %al,(%rax)
    14001708b:	add    %cl,-0x70000000(%rip)        # 0xd0017091
    140017091:	add    (%rax),%eax
    140017093:	add    %ch,0x1(%rsi,%rsi,2)
    140017097:	add    %ch,0x1(%rdx,%riz,2)
 	...
    1400170ff:	add    %ah,(%rax)
```

## ipex_llm/libs/quantize-llama_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140011af8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu Apr 18 12:30:00 2024
+Time/Date		Fri Apr 19 15:05:16 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011c00
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000011af8
@@ -28600,16 +28600,16 @@
    14001704d:	add    %al,(%rax)
    14001704f:	add    %cl,0x1400133(%rax)
    140017055:	add    %al,(%rax)
    140017057:	add    %dl,0x1400133(%rax)
    14001705d:	add    %al,(%rax)
    14001705f:	add    %al,(%rax)
    140017061:	add    %al,(%rax)
-   140017063:	add    %cl,0x12(%rax)
-   140017066:	and    %esp,0x0(%rsi)
+   140017063:	add    %ch,(%rax,%rcx,4)
+   140017066:	and    0x0(%rsi),%ah
    140017069:	add    %al,(%rax)
    14001706b:	add    %cl,-0x70000000(%rip)        # 0xd0017071
    140017071:	add    (%rax),%eax
    140017073:	add    %ch,%ah
    140017075:	jne    0x140017078
    140017077:	add    %ch,%ah
    140017079:	add    %eax,%gs:(%rax)
```

## ipex_llm/libs/quantize-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013c70
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu Apr 18 12:33:26 2024
+Time/Date		Fri Apr 19 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013c70
@@ -32545,19 +32545,17 @@
    1400192a5:	add    %al,(%rax)
    1400192a7:	add    %al,(%rax)
    1400192a9:	push   %rbp
    1400192aa:	add    %eax,0x1(%rax)
    1400192ad:	add    %al,(%rax)
    1400192af:	add    %al,(%rax)
    1400192b1:	add    %al,(%rax)
-   1400192b3:	add    %dl,(%rsi)
-   1400192b5:	adc    (%rcx),%esp
-   1400192b7:	data16 add %al,(%rax)
-   1400192ba:	add    %al,(%rax)
-   1400192bc:	or     $0x20000000,%eax
+   1400192b3:	add    %dl,0x662287(%rcx)
+   1400192b9:	add    %al,(%rax)
+   1400192bb:	add    %cl,0x20000000(%rip)        # 0x1600192c1
    1400192c1:	add    (%rax),%eax
    1400192c3:	add    %bh,0x1(%rdx,%riz,4)
    1400192c7:	add    %bh,0x1(%rdx,%rdx,4)
 	...
    1400192ff:	add    %al,(%rcx)
 	...
    140019309:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-starcoder_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013e80
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu Apr 18 12:30:00 2024
+Time/Date		Fri Apr 19 15:05:17 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013e00
 SizeOfInitializedData	00000000000ad000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013e80
@@ -32652,16 +32652,15 @@
    140019285:	add    %al,(%rax)
    140019287:	add    %al,(%rax)
    140019289:	push   %rbp
    14001928a:	add    %eax,0x1(%rax)
    14001928d:	add    %al,(%rax)
    14001928f:	add    %al,(%rax)
    140019291:	add    %al,(%rax)
-   140019293:	add    %cl,0x12(%rax)
-   140019296:	and    %esp,0x0(%rsi)
+   140019293:	add    %ch,0x662288(%rip)        # 0x14067b521
    140019299:	add    %al,(%rax)
    14001929b:	add    %cl,0x20000000(%rip)        # 0x1600192a1
    1400192a1:	add    (%rax),%eax
    1400192a3:	add    %bh,0x1(%rdx,%riz,4)
    1400192a7:	add    %bh,0x1(%rsp,%rdx,4)
 	...
    1400192ff:	add    %al,(%rcx)
```

## ipex_llm/libs/starcoder-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018000277c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 18 12:33:25 2024
+Time/Date		Fri Apr 19 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002200
 SizeOfInitializedData	0000000000003400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000277c
@@ -4028,17 +4028,19 @@
    1800045f0:	cmp    %al,0x0(%rdx)
    1800045f3:	addb   $0x0,(%rcx)
    1800045f6:	add    %al,(%rax)
    1800045f8:	rex
    1800045f9:	rex.X add %al,0x1(%rax)
    180004600:	add    %al,(%rax)
    180004602:	add    %al,(%rax)
-   180004604:	adc    $0x662113,%eax
-   180004609:	add    %al,(%rax)
-   18000460b:	add    %cl,-0x20000000(%rip)        # 0x160004611
+   180004604:	xchg   %eax,%ecx
+   180004605:	xchg   %esp,(%rdx)
+   180004607:	data16 add %al,(%rax)
+   18000460a:	add    %al,(%rax)
+   18000460c:	or     $0xe0000000,%eax
    180004611:	add    (%rax),%al
    180004613:	add    %ah,%ah
    180004615:	rex.W add %al,(%rax)
    180004618:	in     $0x2e,%al
 	...
    18000467e:	add    %al,(%rax)
    180004680:	add    %eax,(%rax)
```

## ipex_llm/libs/starcoder.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800607a8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 18 12:33:26 2024
+Time/Date		Fri Apr 19 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000060e00
 SizeOfInitializedData	00000000000c7a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000607a8
@@ -129991,16 +129991,16 @@
    180069cd5:	add    %al,(%rax)
    180069cd7:	add    %al,%al
    180069cd9:	es (bad)
    180069cdb:	addb   $0x0,(%rcx)
    180069cde:	add    %al,(%rax)
    180069ce0:	add    %al,(%rax)
    180069ce2:	add    %al,(%rax)
-   180069ce4:	(bad)
-   180069ce5:	adc    (%rcx),%esp
+   180069ce4:	xchg   %eax,%ecx
+   180069ce5:	xchg   %esp,(%rdx)
    180069ce7:	data16 add %al,(%rax)
    180069cea:	add    %al,(%rax)
    180069cec:	or     $0x50000000,%eax
    180069cf1:	add    (%rax),%eax
    180069cf3:	add    %dl,-0x52(%rax)
    180069cf6:	(bad)
    180069cf7:	add    %dl,-0x60(%rax)
```

## ipex_llm/transformers/speculative.py

```diff
@@ -23,16 +23,27 @@
 import time
 import os
 import copy
 import logging
 import transformers
 from packaging import version
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
-from transformers import top_k_top_p_filtering, GenerationConfig, \
+from transformers import GenerationConfig, \
     LogitsProcessorList, StoppingCriteriaList
+from ipex_llm.utils.common import log4Error
+
+trans_version = transformers.__version__
+if version.parse(trans_version) >= version.parse("4.39.0"):
+    try:
+        from trl.core import top_k_top_p_filtering
+    except ModuleNotFoundError:
+        log4Error.invalidInputError(False, "For transformers version >= 4.39.0, pip install trl")
+else:
+    from transformers import top_k_top_p_filtering
+
 from ipex_llm.utils.common import invalidInputError
 from transformers.modeling_outputs import CausalLMOutputWithPast
 
 # patch GenerationMixin.generate
 from transformers import GenerationMixin
 original_generate = GenerationMixin.generate
 query_group_size = 16
@@ -436,14 +447,28 @@
                 past_key_values[i] = (new_cache_k.transpose(1, 2), new_cache_v.transpose(1, 2))
             else:
                 past_key_values[i] = (new_cache_k, new_cache_v)
     return past_key_values, not enough_kv_room
 
 
 def _crop_past_key_values(self, past_key_values, new_cache_size, _enable_ipex=False):
+    from ipex_llm.transformers.kv import DynamicFp8Cache, DynamicNormalCache
+    if isinstance(past_key_values, (DynamicFp8Cache, DynamicNormalCache)):
+        if hasattr(past_key_values, "_seen_tokens"):
+            past_key_values._seen_tokens -= new_cache_size
+        else:
+            past_key_values.seen_tokens -= new_cache_size
+
+        for i, k in enumerate(past_key_values.key_cache):
+            past_key_values.key_cache[i] = k[:, :, :-new_cache_size, :]
+        for i, v in enumerate(past_key_values.value_cache):
+            past_key_values.value_cache[i] = v[:, :, :-new_cache_size, :]
+
+        return past_key_values
+
     if _enable_ipex:
         cur_len = past_key_values[0][0].size(1)
         delta = new_cache_size
         tmp = torch.empty(1, (cur_len - delta), (cur_len - delta), 1,
                           dtype=torch.long).contiguous()
         past_key_values = [[tmp, key_cache, value_cache, beam_idx]
                            for _, key_cache, value_cache, beam_idx in past_key_values]
```

## ipex_llm/transformers/models/baichuan2.py

```diff
@@ -50,16 +50,14 @@
 
 
 def baichuan_13b_rms_norm_forward(self, hidden_states):
     if hidden_states.device.type == "xpu" and not (self.training and hidden_states.requires_grad):
         import linear_q4_0
         x_2d = hidden_states.reshape(-1, hidden_states.size(-1)).contiguous()
         output = linear_q4_0.rms_norm(self.weight, x_2d, self.epsilon)
-        if 1 < x_2d.size(0) <= 64:   # may use XMX, need copy
-            output = output.clone()
         return output.reshape(hidden_states.shape)
 
     input_dtype = hidden_states.dtype
     hidden_states = hidden_states.to(torch.float32)
     variance = hidden_states.pow(2).mean(-1, keepdim=True)
     hidden_states = hidden_states * torch.rsqrt(variance + self.epsilon)
     return self.weight * hidden_states.to(input_dtype)
```

## ipex_llm/transformers/models/chatglm2.py

```diff
@@ -97,16 +97,14 @@
 
 
 def chatglm_rms_norm_forward(self, hidden_states):
     if hidden_states.device.type == "xpu" and not (self.training and hidden_states.requires_grad):
         import linear_q4_0
         x_2d = hidden_states.reshape(-1, hidden_states.size(-1)).contiguous()
         output = linear_q4_0.rms_norm(self.weight, x_2d, self.eps)
-        if 1 < x_2d.size(0) <= 64:   # may use XMX, need copy
-            output = output.clone()
         return output.reshape(hidden_states.shape)
 
     input_dtype = hidden_states.dtype
     hidden_states = hidden_states.to(torch.float32)
     variance = hidden_states.pow(2).mean(-1, keepdim=True)
     hidden_states = hidden_states * torch.rsqrt(variance + self.eps)
     return self.weight * hidden_states.to(input_dtype)
```

## ipex_llm/transformers/models/gemma.py

```diff
@@ -78,16 +78,14 @@
 
 
 def gemma_rms_norm_forward(self, hidden_states):
     if hidden_states.device.type == "xpu" and not (self.training and hidden_states.requires_grad):
         import linear_q4_0
         x_2d = hidden_states.reshape(-1, hidden_states.size(-1)).contiguous()
         output = linear_q4_0.rms_norm(self.weight + 1, x_2d, self.eps)
-        if 1 < x_2d.size(0) <= 64:   # may use XMX, need copy
-            output = output.clone()
         return output.reshape(hidden_states.shape)
 
     input_dtype = hidden_states.dtype
     hidden_states = hidden_states.to(torch.float32)
     variance = hidden_states.pow(2).mean(-1, keepdim=True)
     hidden_states = hidden_states * torch.rsqrt(variance + self.eps)
     return (1 + self.weight) * hidden_states.to(input_dtype)
```

## ipex_llm/transformers/models/llama.py

```diff
@@ -134,16 +134,14 @@
 
 
 def llama_rms_norm_forward(self, hidden_states):
     if hidden_states.device.type == "xpu" and not (self.training and hidden_states.requires_grad):
         import linear_q4_0
         x_2d = hidden_states.reshape(-1, hidden_states.size(-1)).contiguous()
         output = linear_q4_0.rms_norm(self.weight, x_2d, self.variance_epsilon)
-        if 1 < x_2d.size(0) <= 64:   # may use XMX, need copy
-            output = output.clone()
         return output.reshape(hidden_states.shape)
 
     input_dtype = hidden_states.dtype
     hidden_states = hidden_states.to(torch.float32)
     variance = hidden_states.pow(2).mean(-1, keepdim=True)
     hidden_states = hidden_states * torch.rsqrt(variance + self.variance_epsilon)
     return self.weight * hidden_states.to(input_dtype)
@@ -1344,34 +1342,18 @@
         attn_output = attn_output.view(query_states.shape)
         attn_weights = None
     else:
         # repeat k/v heads if n_kv_heads < n_heads
         key_states = repeat_kv(key_states, self.num_key_value_groups)
         value_states = repeat_kv(value_states, self.num_key_value_groups)
         # otherwise, use native attention
-        if query_states.device.type == "xpu":
-            dev_name = torch.xpu.get_device_name(query_states.device.index)
-        else:
-            dev_name = "CPU"
-        if not output_attentions and not dev_name.startswith("Intel(R) Data Center GPU Max"):
-            attn_output = torch.nn.functional.scaled_dot_product_attention(
-                query_states,
-                key_states,
-                value_states,
-                attn_mask=attention_mask,
-                dropout_p=self.attention_dropout if self.training else 0.0,
-                # The q_len > 1 is necessary to match with AttentionMaskConverter.to_causal_4d that
-                # does not create a causal mask in case q_len == 1.
-                is_causal=self.is_causal and attention_mask is None and q_len > 1,
-            )
-        else:
-            attn_output, attn_weights = native_sdp(query_states, key_states, value_states,
-                                                   attention_mask,
-                                                   bsz, q_len, kv_seq_len,
-                                                   self.head_dim, self.num_heads, output_attentions)
+        attn_output, attn_weights = native_sdp(query_states, key_states, value_states,
+                                               attention_mask,
+                                               bsz, q_len, kv_seq_len,
+                                               self.head_dim, self.num_heads, output_attentions)
 
     attn_output_size = (bsz, self.num_heads, q_len, self.head_dim)
     if attn_output.size() != attn_output_size:
         invalidInputError(False,
                           f"`attn_output` should be of size {attn_output_size},"
                           f" but is {attn_output.size()}")
 
@@ -1787,14 +1769,17 @@
             dtype=torch.long, device=device
         )
         position_ids = position_ids.unsqueeze(0)
 
     if inputs_embeds is None:
         inputs_embeds = self.embed_tokens(input_ids)
 
+    # IPEX-LLM modifications:
+    # Disable sdpa for CPU
+    self._use_sdpa = False
     if self._use_flash_attention_2:
         # 2d mask is passed through the layers
         attention_mask = attention_mask if (attention_mask is not None and 0 in attention_mask) \
             else None
     elif self._use_sdpa and not output_attentions:
         # output_attentions=True can not be supported when using SDPA, and we fall back on
         # the manual implementation that requires a 4D causal mask in all cases.
```

## Comparing `ipex_llm-2.1.0b20240418.data/scripts/llm-chat.ps1` & `ipex_llm-2.1.0b20240419.data/scripts/llm-chat.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240418.data/scripts/llm-cli.ps1` & `ipex_llm-2.1.0b20240419.data/scripts/llm-cli.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240418.dist-info/METADATA` & `ipex_llm-2.1.0b20240419.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipex-llm
-Version: 2.1.0b20240418
+Version: 2.1.0b20240419
 Summary: Large Language Model Develop Toolkit
 Home-page: https://github.com/intel-analytics/BigDL
 Author: BigDL Authors
 Author-email: bigdl-user-group@googlegroups.com
 License: Apache License, Version 2.0
 Platform: windows
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,15 +21,15 @@
 Requires-Dist: transformers (==4.31.0) ; extra == 'all'
 Requires-Dist: sentencepiece ; extra == 'all'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'all'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'all'
 Requires-Dist: tabulate ; extra == 'all'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'all'
 Provides-Extra: cpp
-Requires-Dist: bigdl-core-cpp (==2.5.0b20240418) ; extra == 'cpp'
+Requires-Dist: bigdl-core-cpp (==2.5.0b20240419) ; extra == 'cpp'
 Provides-Extra: serving
 Requires-Dist: py-cpuinfo ; extra == 'serving'
 Requires-Dist: fschat[model_worker,webui] (==0.2.36) ; extra == 'serving'
 Requires-Dist: protobuf ; extra == 'serving'
 Provides-Extra: xpu
 Requires-Dist: py-cpuinfo ; extra == 'xpu'
 Requires-Dist: protobuf ; extra == 'xpu'
@@ -39,47 +39,47 @@
 Requires-Dist: sentencepiece ; extra == 'xpu'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu'
 Requires-Dist: tabulate ; extra == 'xpu'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240418) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240418) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240419) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240419) ; extra == 'xpu'
 Provides-Extra: xpu-2-0
 Requires-Dist: py-cpuinfo ; extra == 'xpu-2-0'
 Requires-Dist: protobuf ; extra == 'xpu-2-0'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'xpu-2-0'
 Requires-Dist: numpy (==1.26.4) ; extra == 'xpu-2-0'
 Requires-Dist: transformers (==4.31.0) ; extra == 'xpu-2-0'
 Requires-Dist: sentencepiece ; extra == 'xpu-2-0'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu-2-0'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu-2-0'
 Requires-Dist: tabulate ; extra == 'xpu-2-0'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-0'
 Requires-Dist: torch (==2.0.1a0) ; (platform_system == "Linux") and extra == 'xpu-2-0'
 Requires-Dist: torchvision (==0.15.2a0) ; (platform_system == "Linux") and extra == 'xpu-2-0'
 Requires-Dist: intel-extension-for-pytorch (==2.0.110+xpu) ; (platform_system == "Linux") and extra == 'xpu-2-0'
-Requires-Dist: bigdl-core-xe (==2.5.0b20240418) ; (platform_system == "Linux") and extra == 'xpu-2-0'
-Requires-Dist: bigdl-core-xe-esimd (==2.5.0b20240418) ; (platform_system == "Linux") and extra == 'xpu-2-0'
+Requires-Dist: bigdl-core-xe (==2.5.0b20240419) ; (platform_system == "Linux") and extra == 'xpu-2-0'
+Requires-Dist: bigdl-core-xe-esimd (==2.5.0b20240419) ; (platform_system == "Linux") and extra == 'xpu-2-0'
 Provides-Extra: xpu-2-1
 Requires-Dist: py-cpuinfo ; extra == 'xpu-2-1'
 Requires-Dist: protobuf ; extra == 'xpu-2-1'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'xpu-2-1'
 Requires-Dist: numpy (==1.26.4) ; extra == 'xpu-2-1'
 Requires-Dist: transformers (==4.31.0) ; extra == 'xpu-2-1'
 Requires-Dist: sentencepiece ; extra == 'xpu-2-1'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu-2-1'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu-2-1'
 Requires-Dist: tabulate ; extra == 'xpu-2-1'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240418) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240418) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240419) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240419) ; extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu'
 
 
 IPEX LLM
```

## Comparing `ipex_llm-2.1.0b20240418.dist-info/RECORD` & `ipex_llm-2.1.0b20240419.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -38,46 +38,46 @@
 ipex_llm/langchain/embeddings/bigdlllm.py,sha256=auNueZ-S5RQrngss_huXlYdWImX2vPYfuEVOZsx35rk,13589
 ipex_llm/langchain/embeddings/transformersembeddings.py,sha256=hBtqBfGmGg_xjb4Us7hLNfyvbLMo5mJk9a0iooOWtPM,7225
 ipex_llm/langchain/llms/__init__.py,sha256=vBCl9JF45vnk9CWBG1k8lp8J6F8OCR9UY2E-idkkm5Y,1636
 ipex_llm/langchain/llms/bigdlllm.py,sha256=FAZG6cAIJhRgbxm16gMq-cyBwLe-u165zE7yyxD7r9E,24438
 ipex_llm/langchain/llms/transformersllm.py,sha256=7eaIkJi1CbTCSgNxBCoZTe-o_5FYjD1GTYPWpn0Ccr4,10576
 ipex_llm/langchain/llms/transformerspipelinellm.py,sha256=vm522YPPwWxxAPVvQBtxRfBinC4hIbXdKW6VjHDaFXY,7379
 ipex_llm/libs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ipex_llm/libs/bloom-api.dll,sha256=r6sUxlJWFnRwoCsBSQ1EYe6VCv6bLg9IrsHB6pOkI18,36352
-ipex_llm/libs/bloom.dll,sha256=oHJPtTBPeXD5xfmELGifHIdA_Zf5DbUq00aMSwEsGtU,460288
-ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=802UG3TqYPXdhOxwJ1rEuoDnjLXtoazrcAFBP4lFtAc,852992
-ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=ZpTsTtdqXcXrcWRBY-wqP-dHQ5WT6DGqgQT9GgmUZgU,856064
-ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=ZFzWNNs3TAIca9ScFToMN9rsnerjmFzAm0-IZOrGaks,843776
-ipex_llm/libs/gptneox-api.dll,sha256=KFDesaulI3J4WK4PgyB-FSx7aY2Njk9aYH4KY9GiYwk,24576
-ipex_llm/libs/gptneox.dll,sha256=_4Jj7n5kiPqd4KOz4bNNCmKK8G7nRwAef15Ikwo_nzo,520192
-ipex_llm/libs/libbloom_avx.dll,sha256=SzfK2IFqcouXbRGK215ksZHI0cO3qRKr59Poq8v1HIU,485888
-ipex_llm/libs/libbloom_vnni.dll,sha256=TEgbbY0Uuv1AOlmXhEy4x0KzJubvZaZj7iZO9LxXDxU,460800
-ipex_llm/libs/libgptneox_avx.dll,sha256=p9APTf_QZZnnWHiiR1l6GvZUl8oMEDYep2pH2pHmhjA,545792
-ipex_llm/libs/libgptneox_vnni.dll,sha256=GA11nD2Jzcs2HpQE10S2k5zq7P29RyxQKt28kikA_Ss,520704
-ipex_llm/libs/libllama_avx.dll,sha256=0P4P_1rvs0ls8sISuMn1TeEZsggFr2IlgjuRRSrgogs,540160
-ipex_llm/libs/libllama_vnni.dll,sha256=KV74MQhjyb7J2-028DJBIYpQQmt2rbr5Hw1Uw-5OA8Q,515072
-ipex_llm/libs/libstarcoder_avx.dll,sha256=y0ohs4Fd5lXjeTQoqUnRWImvMS-trqtz0ggKcfRyu_c,577024
-ipex_llm/libs/libstarcoder_vnni.dll,sha256=jp0BLDNtTrk9OIJD4gdxmfoeMSUwi3oW8u7hQgYNec4,551936
-ipex_llm/libs/llama-api.dll,sha256=9dBux7YFPIx5T7M7IkO8z5U4jEv70ggiwPb1d33ecKI,25088
-ipex_llm/libs/llama.dll,sha256=VGR3j6fed8xtJ_CI1qBg6lalDAXYdt4mco2l14nDnRE,514560
-ipex_llm/libs/main-bloom.exe,sha256=nOvWesKJNUYVW57NTO1D8yk0luqXX2db1etTzAxG_AE,103424
-ipex_llm/libs/main-chatglm_vnni.exe,sha256=kFDf8srzb4sP-8EHB_6LUXfN-yr60MyNoUjNMoTZlGU,726016
-ipex_llm/libs/main-gptneox.exe,sha256=xrEv8e9pWYwpVYfoc1p6WwyZsVdXw-uxIrpnA-Rh0w0,98816
-ipex_llm/libs/main-llama.exe,sha256=sLVJP_SptVhlHgv3XAkJIbrMTqOt6oKWhOUPQ79MjEs,99840
-ipex_llm/libs/main-starcoder.exe,sha256=kd6PcveHxi8tTDfn2itoyx-urPEH4IL1Zl6PJH5orcE,157696
-ipex_llm/libs/quantize-bloom.exe,sha256=dEDDzrgMtd90eobESWPsmt_h_8nxi6R2deNeyWgVKIo,125952
-ipex_llm/libs/quantize-bloom_vnni.exe,sha256=JmFOK3jR2dUdWXegMDrLIcR0np0tbaxLYhup_MVftfk,127488
-ipex_llm/libs/quantize-gptneox.exe,sha256=ZoYRNnQPWRA7JA-qOdHyyK-9pHa8cBHOLds5com3F0Q,103936
-ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=Ly-3CKLMDJFs4cl4OJaJIdr02Bbd8fJO7Pr3F91tYMg,104448
-ipex_llm/libs/quantize-llama.exe,sha256=kGBmin6OOaJ1JB_hErSE0cM2P7eiK4TCpaTrhp7fSkM,109056
-ipex_llm/libs/quantize-llama_vnni.exe,sha256=R_0T5P36odPqV1c4B3hhscUS9oRnfqMZOGwWwch6h6g,110080
-ipex_llm/libs/quantize-starcoder.exe,sha256=rc6aRrfJmZGbGEGku8nd-dLIle1UE88OjfGnPjQ0vUQ,126976
-ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=ISmkhy8V2BH2_1IoTlSYxfQbztXTUXCmAIAE28Xl2QA,128000
-ipex_llm/libs/starcoder-api.dll,sha256=bBjCAYaGJX40XVofAahNpwpvv5nD4MIBPZDfPNudMeE,21504
-ipex_llm/libs/starcoder.dll,sha256=TG1tZIix3SWLfDjCMsAavLfrU4pSbDJMQKwxx4QAoDg,551424
+ipex_llm/libs/bloom-api.dll,sha256=wi4VoYCxRBVk3AqNbr_q_M_TlLVCwx7F3rXhoO1SPAY,36352
+ipex_llm/libs/bloom.dll,sha256=-Klp_l9D5MoIBc6ZIPUR3w8CSdLANUdDrmlptHx5dcU,460288
+ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=yHCGFtFSiJuF6bQ0JSosLQNTyE45ksl_dHldGFYc2q0,852992
+ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=YiRoQn8h8eBpu70XmB16DMjZzcjV48BfAp_AIB4NhTM,856064
+ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=sf3sfRJeKBZwupsYHbUjqgnnJgEUPnC0phkCOybpxY4,843776
+ipex_llm/libs/gptneox-api.dll,sha256=9hLV-KHCGtIBIO7lA1uYaV531SyuU3qQWTPaC6_nWZg,24576
+ipex_llm/libs/gptneox.dll,sha256=E4Rdn7qJzUuo2XXf6AsN8FcG1Mdt1AEWfiZoWylJj1U,520192
+ipex_llm/libs/libbloom_avx.dll,sha256=BXj53qiPHQEvDghjz4LAMe-K8bA7EX6M1FQOTwi9tdQ,485888
+ipex_llm/libs/libbloom_vnni.dll,sha256=i0K_bA7AMwm9tQVyawCPyLB626QmJ28U1gqzaMQaeHg,460800
+ipex_llm/libs/libgptneox_avx.dll,sha256=7QcKO0oKbqHhMui8j4vqsGn4BM3-4TnoCpf7m-d6EcM,545792
+ipex_llm/libs/libgptneox_vnni.dll,sha256=ROHhclmlcpx6yiXn534qFkpfo3bG012_DEzCwwB6Mr4,520704
+ipex_llm/libs/libllama_avx.dll,sha256=fugYQZS1-2_CJ8QiYArsjsFJ57NdMDEvVMq25m7ZxIU,540160
+ipex_llm/libs/libllama_vnni.dll,sha256=RVzc6h4MdvO4OG8nA_Oe4TZEYI3k1enbkH6UoFoMuNA,515072
+ipex_llm/libs/libstarcoder_avx.dll,sha256=FqoK_KSRXi5_NRUCrji7ei8PwwvFyiPaVWPh29ZWq_E,577024
+ipex_llm/libs/libstarcoder_vnni.dll,sha256=n_C6wov-ROnOVqlifLwA_mxyDi2dX3NlW1620wYdAsY,551936
+ipex_llm/libs/llama-api.dll,sha256=G2tJW9VW1cgyQ98xc68N6pJqxhKg9U5gnIK74HMdW2g,25088
+ipex_llm/libs/llama.dll,sha256=mOmC5OqZiTAMufrmXLRQL-pE3-rpPKZPrKBU2n_W6WE,514560
+ipex_llm/libs/main-bloom.exe,sha256=K8TWindDurekNP8tYXOsB_5ReURz1i3JjvvleSmvzAw,103424
+ipex_llm/libs/main-chatglm_vnni.exe,sha256=HMPIszl25VqZ2i7AH4EmhdsdrsnzEW5Nf-mGnvwUUl0,726016
+ipex_llm/libs/main-gptneox.exe,sha256=Rg4QjTiSkus9PmhqcFNndv6tEN84NuVbtxpgD6vAziI,98816
+ipex_llm/libs/main-llama.exe,sha256=JEo00mqtJq-x2MYYELGFR_zVgyL7-e6s_lw6EYQ3mYY,99840
+ipex_llm/libs/main-starcoder.exe,sha256=HUa8V3-MLxb6r1gcdhKavEUGLYQd0m7Au0Vl3W0t6bM,157696
+ipex_llm/libs/quantize-bloom.exe,sha256=XsiKFWsyB795HTLl2Py7WmGO16jcscGd3rnujiJD6qc,125952
+ipex_llm/libs/quantize-bloom_vnni.exe,sha256=0jVMEj2zgibSBFeXj3MF42o6XsjhQLIEx2m9T_pQ4oM,127488
+ipex_llm/libs/quantize-gptneox.exe,sha256=5AB7ejKhjl4smKsxsLDkJ5X7uoEh8r0kfjFMKFt28nU,103936
+ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=morYxSJ2lTYbfRBsj55LT7fsP0i1-cbGKQrFHy3OYJY,104448
+ipex_llm/libs/quantize-llama.exe,sha256=kIZyL-LsY2-udEnZATWGpy3eiCWMlJA0lIABo2_Jcak,109056
+ipex_llm/libs/quantize-llama_vnni.exe,sha256=DjwjJz3EoJxapo4XvI5t47eRq0oCGB_3_Th7EPg3u9E,110080
+ipex_llm/libs/quantize-starcoder.exe,sha256=FapQasiqXcdfRFAg9qC_OlbiB2D2NBPWYm80Ou-tgww,126976
+ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=VLVVwSZtzHkGHW1yK92Ytc-qZ234vDQzOlbvmesbFfE,128000
+ipex_llm/libs/starcoder-api.dll,sha256=cVmEg9K9udFqLYXNE5lGaiOjxYrJ-LmR-RZrBzFUfzA,21504
+ipex_llm/libs/starcoder.dll,sha256=375_M4NLjCCafLkTj_4v4dExsT1kt1gm53hm8TbfLB8,551424
 ipex_llm/llamaindex/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
 ipex_llm/llamaindex/llms/__init__.py,sha256=KP1lEdGqDuxPoxL1ZSH25Pm2kKMPJBWUTLR0ckSLMIU,1139
 ipex_llm/llamaindex/llms/bigdlllm.py,sha256=FQBzq1KOjfc6uofTXAha3O7TqpJkNfOFepXQmOVlbnI,26314
 ipex_llm/serving/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/bigdl_llm_model.py,sha256=NXEN_3EPmcP3dDnvug4MokEXXE2zVUnENgBYxfubqic,10084
 ipex_llm/serving/fastchat/ipex_llm_worker.py,sha256=LNMHFYgJqna-4TfIYH7zfKElUXIYMqE0J0ICHpvMGPk,11371
@@ -93,15 +93,15 @@
 ipex_llm/transformers/loader.py,sha256=mC9-RuJGIvpSdP0eyDQ3OY2q1SFTwM-TDlcv2ZSVNIo,5429
 ipex_llm/transformers/lookup.py,sha256=--9zJiNFvsEwtg7gdZAtsBVhewGDQvCdYZ-lkPmBxXo,14719
 ipex_llm/transformers/low_bit_linear.py,sha256=ifclEZ2AAh5ZN3G6fHy-8K9NgRRHJcg6rg0z7lZwaZw,38388
 ipex_llm/transformers/model.py,sha256=hHExQLCrSntBXY8c9FXGgIMQNiL8BQ99ll4GoglGFM0,36157
 ipex_llm/transformers/modelling_bigdl.py,sha256=AqbRwpSAiHmKUo2FGOiwKtytlh-35NWb6eDy7YyNzoo,6921
 ipex_llm/transformers/qlora.py,sha256=WwHn2NXwx8SM6k7_xK1veppWiwL3g5PKihrbC3SPm-g,14770
 ipex_llm/transformers/relora.py,sha256=-dYzUV0P-IhO2jFdnzN9-v_sFzJpRj3ZwN9eCJzOoCw,16567
-ipex_llm/transformers/speculative.py,sha256=LSYX7-HG_UcwEEn_T8N5nLMIkElcb8pHVe7_mA6KaPw,54512
+ipex_llm/transformers/speculative.py,sha256=_-zqypaWWvNppbtAbnzJg3J_0QhC2Slmnad7_zhAJZs,55517
 ipex_llm/transformers/training_patch.py,sha256=4_eQ2uCtGOnRVC2iPkzquuYnvERdneBb7Ovu_pc-VCA,8404
 ipex_llm/transformers/utils.py,sha256=DZJ4Tz-WVeGORkE_Ld8YYCz4WrePiQvtfwPOK5KJlnE,13931
 ipex_llm/transformers/xpu_customize_fwd.py,sha256=wFpIhs5F6tkNs8gBOrLxWdhLzO3EDHovVkERPIAoAvg,7611
 ipex_llm/transformers/awq/__init__.py,sha256=Du5gu3-eeAkeDO_dEMBTzrDBA66DSN3uL3-rn8WGXQw,875
 ipex_llm/transformers/awq/act.py,sha256=YwomJzOOKwkKtzGrm4L4kwBstBLO1Z8SK4CKi8PSYVQ,2172
 ipex_llm/transformers/awq/awq.py,sha256=cGyRQJWwAEJtOtdSbsBoQ33KX_Ie0pv5OJHC0ACEELE,8861
 ipex_llm/transformers/awq/awq_config.py,sha256=SDZJUCAxuphwwnGqjLrbCJIo4KmFmiNgZOeKJI4DmvY,4422
@@ -128,28 +128,28 @@
 ipex_llm/transformers/gguf/models/model_implement/yuan2/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/transformers/gguf/models/model_implement/yuan2/configuration_yuan.py,sha256=PDCUoD7z5cR-61oBjMc5uBCzgtiLx7sbTZ6nTnDU49A,2192
 ipex_llm/transformers/gguf/models/model_implement/yuan2/yuan_hf_model.py,sha256=_AOGMV65XHxgTxIib7lgs49InopcecTzRwgtYR8NTUg,51084
 ipex_llm/transformers/layers/rope_embedding.py,sha256=aL36BVCsjrWSi9DyMWsPOgj5VUNDooYsaO2HDaWAEzs,2658
 ipex_llm/transformers/models/__init__.py,sha256=tp2DcVkKg1-QvdYk7DY7rZvQWCDQ4ZjU8NAQ7Fclrpg,584
 ipex_llm/transformers/models/aquila.py,sha256=xLMxa8EOtpXDdyT9fAc0If_DkuH8Knzmi0Logrv0Jdk,7415
 ipex_llm/transformers/models/baichuan.py,sha256=Q8mEr3BubdhtW6sV_qMWYcvp_Uavvy8A7_2RcMSrOvg,24488
-ipex_llm/transformers/models/baichuan2.py,sha256=sskdX_cSuSY6IYIjBlp6L1feFK2B__41mEJB-0r5anc,27214
+ipex_llm/transformers/models/baichuan2.py,sha256=_oBedlO1kR6dzagl1ADOZCcpKMBqgQW9p6RU73WDzKU,27116
 ipex_llm/transformers/models/bert.py,sha256=bJNic2pt1kph0kBwdK5MRGyWupFfx2Ts0V3D1L-5kWo,6085
 ipex_llm/transformers/models/bloom.py,sha256=IfR1rEwQb157lY2yIBQmrsS185jsBpKhgPYXEeLDQVQ,8971
 ipex_llm/transformers/models/chatglm.py,sha256=crFSh7Df1xSpND27PPBtuDUOzT1aniNjW7xMHUiIcis,13743
-ipex_llm/transformers/models/chatglm2.py,sha256=7POlTOCeelx-chyud7e7ZRf6j6rtovThubkciSYYhwY,32040
+ipex_llm/transformers/models/chatglm2.py,sha256=9RhnrlqQFIgoMkc55NkjtlagU-fioCX7I50hO0ay-xE,31942
 ipex_llm/transformers/models/chatglm2_32k.py,sha256=ch9Mw7T4haXcXMgqqubIi-mIQvlsdZ8gw6RhSbaUrao,8697
 ipex_llm/transformers/models/decilm.py,sha256=oAKyfB2_9GWheuqi3SyQXCBcRd6ixr6jeuYhN1z_d6A,8654
 ipex_llm/transformers/models/falcon.py,sha256=f5BzMbv4E-R5Pete8zBscbgiueXGIaWGs-5RbcMlUo4,33549
-ipex_llm/transformers/models/gemma.py,sha256=o6x0lHZ6lLmxmytBIFri_3d-jWO4RFj_xC1tvfn0CBE,12408
+ipex_llm/transformers/models/gemma.py,sha256=ZMn_BizM1ekqZ3erJep8L_QNLSEDgJNrUm1hEJWsQLQ,12310
 ipex_llm/transformers/models/gptbigcode.py,sha256=93l2PRLk1aLEhCGpio_7Y93amALS4SPrD5VXWiRl6hs,4342
 ipex_llm/transformers/models/gptj.py,sha256=TTIx461X2nOcIkrAcZhEf7d7mjJ3yvEC9KLVc1-hrpc,17973
 ipex_llm/transformers/models/gptneox.py,sha256=MVVdTbxV2oGzpCCzBMUy6oysVlnMtohJkl7SiC0xMAA,6219
 ipex_llm/transformers/models/internlm.py,sha256=mHyKQswtAHpT8R44gVvH7N57jjbk_GNtxjZWJy7ioog,11647
-ipex_llm/transformers/models/llama.py,sha256=t39TfBGYN_W-_qA4Xi-X2LyHnO_qC9FhmwlWyVO-QS8,98235
+ipex_llm/transformers/models/llama.py,sha256=6vQqOVYlquXh404SLTqucu8QOQDpH9fGDST4TwlIAoM,97385
 ipex_llm/transformers/models/mistral.py,sha256=GC0qaiQ1P-eOOmbvHoiaDziB2LFjhf8srll0fkr7c6M,45181
 ipex_llm/transformers/models/mixtral.py,sha256=qHeOIz8t7dTIPS9yu3QaOiN5jrUzDZ6NU9_wR6bb47U,27273
 ipex_llm/transformers/models/mpt.py,sha256=z02NwHogJZVh-Mk4sYoIzR90SFIKhoNN_-ifsD907TQ,9540
 ipex_llm/transformers/models/phixtral.py,sha256=4B_2iE26GlzTVdaemd6mwYQ8mp4Yo4Yq9DgSFkF0yvc,6268
 ipex_llm/transformers/models/qwen.py,sha256=JLUFrgJ3cD_2iG_pqov5zZmkZDhZUZ9Lg9bgQYJCcWk,32349
 ipex_llm/transformers/models/qwen2.py,sha256=NFLzgdvBcj5cdmCeJi0lqXz4c0JfBioZK_im2Ysynac,32725
 ipex_llm/transformers/models/qwen2_moe.py,sha256=Wv9oU1vOx087DeC4BSVLtrAAdKKnyk2y1czzhfG7ncc,30334
@@ -205,14 +205,14 @@
 ipex_llm/vllm/transformers_utils/tokenizer.py,sha256=PKmEi1ROhf9dKRa-7AuKYwvAY-htP-ZIAz4HhNqhokU,8707
 ipex_llm/vllm/worker/worker.py,sha256=eifKuzefL9HC1R62P0mCYBsZlclo_5hQf01vFgc6mFA,13950
 ipex_llm/vllm2/__init__.py,sha256=zBSG6nzrVF5QnpR6_f7kPhBFeowTE9gaZ7D5m98E7_w,585
 ipex_llm/vllm2/model_convert.py,sha256=jbsUSUAeVHm24CokIiLdyv6ubd_HuCrN_pnF3cLhhWE,7208
 ipex_llm/vllm2/engine/__init__.py,sha256=mzPVAyZdbvfzBQi-wxZh1sbme_NElPMmtrJ9C2zh8Us,747
 ipex_llm/vllm2/engine/engine.py,sha256=4jQucwE46X_Bn2dA7uzjWKSJWeSiDZ76-9XW7WHJHAA,5715
 ipex_llm/vllm2/entrypoints/openai/api_server.py,sha256=M7pwasNK1J6kTTrcFgbxgXmKnPWUA4D6cw89EeA7Vw0,10475
-ipex_llm-2.1.0b20240418.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
-ipex_llm-2.1.0b20240418.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
-ipex_llm-2.1.0b20240418.dist-info/METADATA,sha256=KGb6aFiHEVsSCYpGme47elXqRxY2JACv0EyXnHhBXqw,4400
-ipex_llm-2.1.0b20240418.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-ipex_llm-2.1.0b20240418.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
-ipex_llm-2.1.0b20240418.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
-ipex_llm-2.1.0b20240418.dist-info/RECORD,,
+ipex_llm-2.1.0b20240419.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
+ipex_llm-2.1.0b20240419.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
+ipex_llm-2.1.0b20240419.dist-info/METADATA,sha256=Hw72NCBQYc3HR3FB57Ebu6kgPDCO1qDZrqSB2DXGRSg,4400
+ipex_llm-2.1.0b20240419.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+ipex_llm-2.1.0b20240419.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
+ipex_llm-2.1.0b20240419.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
+ipex_llm-2.1.0b20240419.dist-info/RECORD,,
```

