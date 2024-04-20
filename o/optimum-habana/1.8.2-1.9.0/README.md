# Comparing `tmp/optimum-habana-1.8.2.tar.gz` & `tmp/optimum-habana-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-habana-1.8.2.tar", last modified: Fri Nov 24 21:13:37 2023, max compression
+gzip compressed data, was "optimum-habana-1.9.0.tar", last modified: Thu Nov 30 23:13:49 2023, max compression
```

## Comparing `optimum-habana-1.8.2.tar` & `optimum-habana-1.9.0.tar`

### file list

```diff
@@ -1,123 +1,127 @@
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.822194 optimum-habana-1.8.2/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    11357 2023-04-28 21:26:38.000000 optimum-habana-1.8.2/LICENSE
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      651 2023-04-28 21:26:38.000000 optimum-habana-1.8.2/MANIFEST.in
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    15313 2023-11-24 21:13:37.822194 optimum-habana-1.8.2/PKG-INFO
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    14162 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/README.md
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.813194 optimum-habana-1.8.2/optimum/
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.815194 optimum-habana-1.8.2/optimum/habana/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     1040 2023-05-15 07:33:53.000000 optimum-habana-1.8.2/optimum/habana/__init__.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.816194 optimum-habana-1.8.2/optimum/habana/accelerate/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      102 2023-08-13 13:33:13.000000 optimum-habana-1.8.2/optimum/habana/accelerate/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    32791 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/accelerate/accelerator.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     7538 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/accelerate/state.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.816194 optimum-habana-1.8.2/optimum/habana/accelerate/utils/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)       46 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/accelerate/utils/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     1270 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/accelerate/utils/dataclasses.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.816194 optimum-habana-1.8.2/optimum/habana/diffusers/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      415 2023-11-21 15:19:52.000000 optimum-habana-1.8.2/optimum/habana/diffusers/__init__.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.816194 optimum-habana-1.8.2/optimum/habana/diffusers/models/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)       69 2023-08-17 09:47:57.000000 optimum-habana-1.8.2/optimum/habana/diffusers/models/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    14349 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/diffusers/models/unet_2d_condition.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.816194 optimum-habana-1.8.2/optimum/habana/diffusers/pipelines/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    17559 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/diffusers/pipelines/pipeline_utils.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.816194 optimum-habana-1.8.2/optimum/habana/diffusers/pipelines/stable_diffusion/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    45026 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    39918 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_ldm3d.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    48326 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_upscale.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.817194 optimum-habana-1.8.2/optimum/habana/diffusers/schedulers/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)       48 2023-04-28 21:26:38.000000 optimum-habana-1.8.2/optimum/habana/diffusers/schedulers/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    15842 2023-11-21 15:19:52.000000 optimum-habana-1.8.2/optimum/habana/diffusers/schedulers/scheduling_ddim.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.817194 optimum-habana-1.8.2/optimum/habana/distributed/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)       93 2023-06-16 17:08:31.000000 optimum-habana-1.8.2/optimum/habana/distributed/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    10761 2023-08-13 13:33:13.000000 optimum-habana-1.8.2/optimum/habana/distributed/distributed_runner.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     6109 2023-06-30 18:00:40.000000 optimum-habana-1.8.2/optimum/habana/distributed/fast_ddp.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.818194 optimum-habana-1.8.2/optimum/habana/transformers/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     1031 2023-04-28 21:26:38.000000 optimum-habana-1.8.2/optimum/habana/transformers/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     4450 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/transformers/gaudi_configuration.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.818194 optimum-habana-1.8.2/optimum/habana/transformers/generation/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      132 2023-07-14 07:15:34.000000 optimum-habana-1.8.2/optimum/habana/transformers/generation/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     2218 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/transformers/generation/configuration_utils.py
--rwxrwxr-x   0 devcloud  (1000) devcloud  (1000)   153086 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/transformers/generation/utils.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     9369 2023-07-28 08:32:54.000000 optimum-habana-1.8.2/optimum/habana/transformers/gradient_checkpointing.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.818194 optimum-habana-1.8.2/optimum/habana/transformers/integrations/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     5870 2023-11-21 15:19:52.000000 optimum-habana-1.8.2/optimum/habana/transformers/integrations/deepspeed.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    13644 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/transformers/modeling_utils.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.818194 optimum-habana-1.8.2/optimum/habana/transformers/models/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     2721 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/__init__.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.818194 optimum-habana-1.8.2/optimum/habana/transformers/models/albert/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)       50 2023-04-28 21:26:38.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/albert/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     4563 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/albert/modeling_albert.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.818194 optimum-habana-1.8.2/optimum/habana/transformers/models/bart/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      387 2023-11-02 19:35:31.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/bart/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    33078 2023-11-02 19:35:31.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/bart/modeling_bart.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.819194 optimum-habana-1.8.2/optimum/habana/transformers/models/bloom/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      258 2023-08-27 09:47:58.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/bloom/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    25432 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/bloom/modeling_bloom.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.819194 optimum-habana-1.8.2/optimum/habana/transformers/models/codegen/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      156 2023-08-17 08:49:14.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/codegen/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    21972 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/codegen/modeling_codegen.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.819194 optimum-habana-1.8.2/optimum/habana/transformers/models/esm/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      237 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/esm/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      470 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/esm/modeling_esm.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    12419 2023-11-21 15:19:52.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/esm/modeling_esmfold.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.819194 optimum-habana-1.8.2/optimum/habana/transformers/models/falcon/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      242 2023-11-21 15:19:52.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/falcon/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    27859 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/falcon/modeling_falcon.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.819194 optimum-habana-1.8.2/optimum/habana/transformers/models/gpt2/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      114 2023-06-06 13:47:11.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/gpt2/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    29855 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/gpt2/modeling_gpt2.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.819194 optimum-habana-1.8.2/optimum/habana/transformers/models/gpt_bigcode/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      185 2023-08-17 08:49:14.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/gpt_bigcode/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    20165 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/gpt_bigcode/modeling_gpt_bigcode.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.820194 optimum-habana-1.8.2/optimum/habana/transformers/models/gpt_neox/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      170 2023-06-06 13:47:11.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/gpt_neox/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    16989 2023-11-21 15:19:52.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/gpt_neox/modeling_gpt_neox.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.820194 optimum-habana-1.8.2/optimum/habana/transformers/models/gptj/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      141 2023-08-12 14:24:11.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/gptj/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    24245 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/gptj/modeling_gptj.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.820194 optimum-habana-1.8.2/optimum/habana/transformers/models/llama/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      166 2023-11-02 19:35:31.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/llama/__init__.py
--rwxrwxr-x   0 devcloud  (1000) devcloud  (1000)    25957 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/llama/modeling_llama.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     5482 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/modeling_all_models.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.820194 optimum-habana-1.8.2/optimum/habana/transformers/models/mpt/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      136 2023-08-29 17:48:02.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/mpt/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    16726 2023-11-02 19:35:31.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/mpt/modeling_mpt.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.820194 optimum-habana-1.8.2/optimum/habana/transformers/models/opt/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      225 2023-06-06 13:47:11.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/opt/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    22098 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/opt/modeling_opt.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.820194 optimum-habana-1.8.2/optimum/habana/transformers/models/t5/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)       52 2023-11-21 15:19:52.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/t5/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     1148 2023-11-21 15:19:52.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/t5/modeling_t5.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.820194 optimum-habana-1.8.2/optimum/habana/transformers/models/vit/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)       59 2023-04-28 21:26:38.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/vit/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     2572 2023-04-28 21:26:38.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/vit/modeling_vit.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.821194 optimum-habana-1.8.2/optimum/habana/transformers/models/wav2vec2/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      190 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/wav2vec2/__init__.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    11639 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/transformers/models/wav2vec2/modeling_wav2vec2.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    96037 2023-11-24 21:08:54.000000 optimum-habana-1.8.2/optimum/habana/transformers/trainer.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    18198 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/transformers/trainer_seq2seq.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     2675 2023-04-28 21:26:38.000000 optimum-habana-1.8.2/optimum/habana/transformers/trainer_utils.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    29924 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/transformers/training_args.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     4736 2023-07-14 07:15:34.000000 optimum-habana-1.8.2/optimum/habana/transformers/training_args_seq2seq.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    11599 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/optimum/habana/utils.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      644 2023-11-24 21:06:57.000000 optimum-habana-1.8.2/optimum/habana/version.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.821194 optimum-habana-1.8.2/optimum_habana.egg-info/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    15313 2023-11-24 21:13:37.000000 optimum-habana-1.8.2/optimum_habana.egg-info/PKG-INFO
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     4138 2023-11-24 21:13:37.000000 optimum-habana-1.8.2/optimum_habana.egg-info/SOURCES.txt
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)        1 2023-11-24 21:13:37.000000 optimum-habana-1.8.2/optimum_habana.egg-info/dependency_links.txt
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)        1 2023-11-24 21:13:30.000000 optimum-habana-1.8.2/optimum_habana.egg-info/not-zip-safe
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      206 2023-11-24 21:13:37.000000 optimum-habana-1.8.2/optimum_habana.egg-info/requires.txt
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)        8 2023-11-24 21:13:37.000000 optimum-habana-1.8.2/optimum_habana.egg-info/top_level.txt
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     1079 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/pyproject.toml
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      112 2023-11-24 21:13:37.822194 optimum-habana-1.8.2/setup.cfg
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     2977 2023-11-24 20:45:46.000000 optimum-habana-1.8.2/setup.py
-drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-24 21:13:37.822194 optimum-habana-1.8.2/tests/
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    24960 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/tests/test_diffusers.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     3526 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/tests/test_encoder_decoder_text_summarization.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    22464 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/tests/test_examples.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     3251 2023-04-28 21:26:38.000000 optimum-habana-1.8.2/tests/test_examples_match_transformers.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     2959 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/tests/test_gaudi_configuration.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     2982 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/tests/test_text_generation_example.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    85470 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/tests/test_trainer.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     5868 2023-11-21 15:19:52.000000 optimum-habana-1.8.2/tests/test_trainer_distributed.py
--rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     4695 2023-11-24 20:45:39.000000 optimum-habana-1.8.2/tests/test_trainer_seq2seq.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.427827 optimum-habana-1.9.0/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    11357 2023-04-28 21:26:38.000000 optimum-habana-1.9.0/LICENSE
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      651 2023-04-28 21:26:38.000000 optimum-habana-1.9.0/MANIFEST.in
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    15439 2023-11-30 23:13:49.427827 optimum-habana-1.9.0/PKG-INFO
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    14288 2023-11-30 22:59:58.000000 optimum-habana-1.9.0/README.md
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.419826 optimum-habana-1.9.0/optimum/
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.421826 optimum-habana-1.9.0/optimum/habana/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     1040 2023-05-15 07:33:53.000000 optimum-habana-1.9.0/optimum/habana/__init__.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.421826 optimum-habana-1.9.0/optimum/habana/accelerate/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      102 2023-08-13 13:33:13.000000 optimum-habana-1.9.0/optimum/habana/accelerate/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    35347 2023-11-30 22:59:58.000000 optimum-habana-1.9.0/optimum/habana/accelerate/accelerator.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    10793 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/accelerate/data_loader.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     7451 2023-11-30 22:59:58.000000 optimum-habana-1.9.0/optimum/habana/accelerate/state.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.421826 optimum-habana-1.9.0/optimum/habana/accelerate/utils/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)       90 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/accelerate/utils/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     4945 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/accelerate/utils/dataclasses.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     4446 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/checkpoint_utils.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.421826 optimum-habana-1.9.0/optimum/habana/diffusers/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      415 2023-11-21 15:19:52.000000 optimum-habana-1.9.0/optimum/habana/diffusers/__init__.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.421826 optimum-habana-1.9.0/optimum/habana/diffusers/models/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)       69 2023-08-17 09:47:57.000000 optimum-habana-1.9.0/optimum/habana/diffusers/models/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    16047 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/diffusers/models/unet_2d_condition.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.422826 optimum-habana-1.9.0/optimum/habana/diffusers/pipelines/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    15207 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/diffusers/pipelines/pipeline_utils.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.422826 optimum-habana-1.9.0/optimum/habana/diffusers/pipelines/stable_diffusion/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    54388 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    43114 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_ldm3d.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    53530 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_upscale.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.422826 optimum-habana-1.9.0/optimum/habana/diffusers/schedulers/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)       48 2023-04-28 21:26:38.000000 optimum-habana-1.9.0/optimum/habana/diffusers/schedulers/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    15842 2023-11-21 15:19:52.000000 optimum-habana-1.9.0/optimum/habana/diffusers/schedulers/scheduling_ddim.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.422826 optimum-habana-1.9.0/optimum/habana/distributed/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)       93 2023-06-16 17:08:31.000000 optimum-habana-1.9.0/optimum/habana/distributed/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    10761 2023-08-13 13:33:13.000000 optimum-habana-1.9.0/optimum/habana/distributed/distributed_runner.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     6109 2023-06-30 18:00:40.000000 optimum-habana-1.9.0/optimum/habana/distributed/fast_ddp.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.423826 optimum-habana-1.9.0/optimum/habana/transformers/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     1031 2023-04-28 21:26:38.000000 optimum-habana-1.9.0/optimum/habana/transformers/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     3408 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/transformers/gaudi_configuration.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.423826 optimum-habana-1.9.0/optimum/habana/transformers/generation/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      132 2023-07-14 07:15:34.000000 optimum-habana-1.9.0/optimum/habana/transformers/generation/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     2373 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/transformers/generation/configuration_utils.py
+-rwxrwxr-x   0 devcloud  (1000) devcloud  (1000)   154761 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/transformers/generation/utils.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     9369 2023-07-28 08:32:54.000000 optimum-habana-1.9.0/optimum/habana/transformers/gradient_checkpointing.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.423826 optimum-habana-1.9.0/optimum/habana/transformers/integrations/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     5870 2023-11-21 15:19:52.000000 optimum-habana-1.9.0/optimum/habana/transformers/integrations/deepspeed.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    14629 2023-11-30 22:59:50.000000 optimum-habana-1.9.0/optimum/habana/transformers/modeling_utils.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.424826 optimum-habana-1.9.0/optimum/habana/transformers/models/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     2855 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/__init__.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.424826 optimum-habana-1.9.0/optimum/habana/transformers/models/albert/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)       50 2023-04-28 21:26:38.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/albert/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     4575 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/albert/modeling_albert.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.424826 optimum-habana-1.9.0/optimum/habana/transformers/models/bart/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      387 2023-11-02 19:35:31.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/bart/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    33078 2023-11-02 19:35:31.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/bart/modeling_bart.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.424826 optimum-habana-1.9.0/optimum/habana/transformers/models/bloom/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      258 2023-08-27 09:47:58.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/bloom/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    26195 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/bloom/modeling_bloom.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.424826 optimum-habana-1.9.0/optimum/habana/transformers/models/codegen/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      156 2023-08-17 08:49:14.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/codegen/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    21944 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/codegen/modeling_codegen.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.424826 optimum-habana-1.9.0/optimum/habana/transformers/models/esm/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      158 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/esm/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    12419 2023-11-21 15:19:52.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/esm/modeling_esmfold.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.424826 optimum-habana-1.9.0/optimum/habana/transformers/models/falcon/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      242 2023-11-21 15:19:52.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/falcon/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    28950 2023-11-30 22:59:58.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/falcon/modeling_falcon.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.425826 optimum-habana-1.9.0/optimum/habana/transformers/models/gpt2/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      114 2023-06-06 13:47:11.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/gpt2/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    28434 2023-11-30 22:59:58.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/gpt2/modeling_gpt2.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.425826 optimum-habana-1.9.0/optimum/habana/transformers/models/gpt_bigcode/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      185 2023-08-17 08:49:14.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/gpt_bigcode/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    20137 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/gpt_bigcode/modeling_gpt_bigcode.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.425826 optimum-habana-1.9.0/optimum/habana/transformers/models/gpt_neox/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      170 2023-06-06 13:47:11.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/gpt_neox/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    16799 2023-11-30 22:59:58.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/gpt_neox/modeling_gpt_neox.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.425826 optimum-habana-1.9.0/optimum/habana/transformers/models/gptj/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      141 2023-08-12 14:24:11.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/gptj/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    25162 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/gptj/modeling_gptj.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.425826 optimum-habana-1.9.0/optimum/habana/transformers/models/llama/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      166 2023-11-02 19:35:31.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/llama/__init__.py
+-rwxrwxr-x   0 devcloud  (1000) devcloud  (1000)    27169 2023-11-30 22:59:58.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/llama/modeling_llama.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.425826 optimum-habana-1.9.0/optimum/habana/transformers/models/mistral/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      169 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/mistral/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    17747 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/mistral/modeling_mistral.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     5506 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/modeling_all_models.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.426826 optimum-habana-1.9.0/optimum/habana/transformers/models/mpt/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      136 2023-08-29 17:48:02.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/mpt/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    16726 2023-11-02 19:35:31.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/mpt/modeling_mpt.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.426826 optimum-habana-1.9.0/optimum/habana/transformers/models/opt/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      225 2023-06-06 13:47:11.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/opt/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    21974 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/opt/modeling_opt.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.426826 optimum-habana-1.9.0/optimum/habana/transformers/models/t5/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)       52 2023-11-21 15:19:52.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/t5/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     1148 2023-11-21 15:19:52.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/t5/modeling_t5.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.426826 optimum-habana-1.9.0/optimum/habana/transformers/models/vit/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)       59 2023-04-28 21:26:38.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/vit/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     2572 2023-04-28 21:26:38.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/vit/modeling_vit.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.426826 optimum-habana-1.9.0/optimum/habana/transformers/models/wav2vec2/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      226 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/wav2vec2/__init__.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    15772 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/transformers/models/wav2vec2/modeling_wav2vec2.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    96122 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/transformers/trainer.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    18460 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/optimum/habana/transformers/trainer_seq2seq.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     2675 2023-04-28 21:26:38.000000 optimum-habana-1.9.0/optimum/habana/transformers/trainer_utils.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    32391 2023-11-30 22:59:58.000000 optimum-habana-1.9.0/optimum/habana/transformers/training_args.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     4736 2023-07-14 07:15:34.000000 optimum-habana-1.9.0/optimum/habana/transformers/training_args_seq2seq.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    12155 2023-11-30 22:59:58.000000 optimum-habana-1.9.0/optimum/habana/utils.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      644 2023-11-30 23:10:52.000000 optimum-habana-1.9.0/optimum/habana/version.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.427827 optimum-habana-1.9.0/optimum_habana.egg-info/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    15439 2023-11-30 23:13:49.000000 optimum-habana-1.9.0/optimum_habana.egg-info/PKG-INFO
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     4277 2023-11-30 23:13:49.000000 optimum-habana-1.9.0/optimum_habana.egg-info/SOURCES.txt
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)        1 2023-11-30 23:13:49.000000 optimum-habana-1.9.0/optimum_habana.egg-info/dependency_links.txt
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)        1 2023-11-30 23:13:41.000000 optimum-habana-1.9.0/optimum_habana.egg-info/not-zip-safe
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      208 2023-11-30 23:13:49.000000 optimum-habana-1.9.0/optimum_habana.egg-info/requires.txt
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)        8 2023-11-30 23:13:49.000000 optimum-habana-1.9.0/optimum_habana.egg-info/top_level.txt
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     1367 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/pyproject.toml
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)      112 2023-11-30 23:13:49.428826 optimum-habana-1.9.0/setup.cfg
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     2974 2023-11-30 23:10:41.000000 optimum-habana-1.9.0/setup.py
+drwxrwxr-x   0 devcloud  (1000) devcloud  (1000)        0 2023-11-30 23:13:49.427827 optimum-habana-1.9.0/tests/
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    25513 2023-11-30 22:59:58.000000 optimum-habana-1.9.0/tests/test_diffusers.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     3519 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/tests/test_encoder_decoder_text_summarization.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    23605 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/tests/test_examples.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     3251 2023-04-28 21:26:38.000000 optimum-habana-1.9.0/tests/test_examples_match_transformers.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     2788 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/tests/test_gaudi_configuration.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     4110 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/tests/test_text_generation_example.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)    90597 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/tests/test_trainer.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     5868 2023-11-21 15:19:52.000000 optimum-habana-1.9.0/tests/test_trainer_distributed.py
+-rw-rw-r--   0 devcloud  (1000) devcloud  (1000)     4662 2023-11-24 21:40:44.000000 optimum-habana-1.9.0/tests/test_trainer_seq2seq.py
```

### Comparing `optimum-habana-1.8.2/LICENSE` & `optimum-habana-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.8.2/MANIFEST.in` & `optimum-habana-1.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.8.2/PKG-INFO` & `optimum-habana-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-habana
-Version: 1.8.2
+Version: 1.9.0
 Summary: Optimum Habana is the interface between the Hugging Face Transformers and Diffusers libraries and Habana's Gaudi processor (HPU). It provides a set of tools enabling easy model loading, training and inference on single- and multi-HPU settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/habana
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,gaudi,hpu
 Classifier: Development Status :: 5 - Production/Stable
@@ -61,15 +61,15 @@
 pip install --upgrade-strategy eager optimum[habana]
 ```
 
 The `--upgrade-strategy eager` option is needed to ensure `optimum-habana` is upgraded to the latest stable release.
 
 > To use DeepSpeed on HPUs, you also need to run the following command:
 >```bash
->pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.12.0
+>pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.13.0
 >```
 
 Optimum Habana is a fast-moving project, and you may want to install it from source:
 
 ```bash
 pip install git+https://github.com/huggingface/optimum-habana.git
 ```
@@ -87,15 +87,15 @@
 ### Quick Start
 
 🤗 Optimum Habana was designed with one goal in mind: **to make training and inference straightforward for any 🤗 Transformers and 🤗 Diffusers user while leveraging the complete power of Gaudi processors**.
 
 #### Transformers Interface
 
 There are two main classes one needs to know:
-- [GaudiTrainer](https://huggingface.co/docs/optimum/habana/package_reference/trainer): the trainer class that takes care of compiling (lazy or eager mode) and distributing the model to run on HPUs, and performing training and evaluation.
+- [GaudiTrainer](https://huggingface.co/docs/optimum/habana/package_reference/trainer): the trainer class that takes care of compiling and distributing the model to run on HPUs, and performing training and evaluation.
 - [GaudiConfig](https://huggingface.co/docs/optimum/habana/package_reference/gaudi_config): the class that enables to configure Habana Mixed Precision and to decide whether optimized operators and optimizers should be used or not.
 
 The [GaudiTrainer](https://huggingface.co/docs/optimum/habana/package_reference/trainer) is very similar to the [🤗 Transformers Trainer](https://huggingface.co/docs/transformers/main_classes/trainer), and adapting a script using the Trainer to make it work with Gaudi will mostly consist in simply swapping the `Trainer` class for the `GaudiTrainer` one.
 That's how most of the [example scripts](https://github.com/huggingface/optimum-habana/tree/main/examples) were adapted from their [original counterparts](https://github.com/huggingface/transformers/tree/main/examples/pytorch).
 
 Here is an example:
 ```diff
@@ -181,19 +181,20 @@
 | DistilBERT |:heavy_check_mark: | :heavy_check_mark: | <li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering)</li><li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li> |
 | GPT2             | :heavy_check_mark: | :heavy_check_mark: | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li><li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | BLOOM(Z) | :x: | <div style="text-align:left"><li>DeepSpeed</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | StarCoder | :x: | <div style="text-align:left"><li>Single card</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | GPT-J | <div style="text-align:left"><li>DeepSpeed</li></div> | <div style="text-align:left"><li>Single card</li><li>DeepSpeed</li></div> | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li><li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | GPT-NeoX | <div style="text-align:left"><li>DeepSpeed</li></div> | <div style="text-align:left"><li>DeepSpeed</li></div> | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li><li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | OPT | :x: | <div style="text-align:left"><li>DeepSpeed</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
-| Llama 2 / CodeLlama | <div style="text-align:left"><li>DeepSpeed</li><li>LoRA</li></div> | <div style="text-align:left"><li>DeepSpeed</li><li>LoRA</li></div> | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li><li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
+| Llama 2 / CodeLlama | <div style="text-align:left"><li>DeepSpeed</li><li>LoRA</li></div> | :heavy_check_mark: | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li><li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | StableLM | :x: | <div style="text-align:left"><li>Single card</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
-| Falcon | :x: | <div style="text-align:left"><li>Single card</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
+| Falcon | <div style="text-align:left"><li>LoRA</li></div> | :heavy_check_mark: | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | CodeGen | :x: | <div style="text-align:left"><li>Single card</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | MPT | :x: | <div style="text-align:left"><li>Single card</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
+| Mistral | :x: | <div style="text-align:left"><li>Single card</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | T5 | :heavy_check_mark: | :heavy_check_mark: | <li>[summarization](https://github.com/huggingface/optimum-habana/tree/main/examples/summarization)</li><li>[translation](https://github.com/huggingface/optimum-habana/tree/main/examples/translation)</li><li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering#fine-tuning-t5-on-squad20)</li> |
 | BART | :x: | <div style="text-align:left"><li>Single card</li></div> | <li>[summarization](https://github.com/huggingface/optimum-habana/tree/main/examples/summarization)</li><li>[translation](https://github.com/huggingface/optimum-habana/tree/main/examples/translation)</li><li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering#fine-tuning-t5-on-squad20)</li> |
 | ViT | :heavy_check_mark: | :heavy_check_mark: | <li>[image classification](https://github.com/huggingface/optimum-habana/tree/main/examples/image-classification)</li> |
 | Swin | :heavy_check_mark: | :heavy_check_mark: | <li>[image classification](https://github.com/huggingface/optimum-habana/tree/main/examples/image-classification)</li> |
 | Wav2Vec2 | :heavy_check_mark: | :heavy_check_mark: | <li>[audio classification](https://github.com/huggingface/optimum-habana/tree/main/examples/audio-classification)</li><li>[speech recognition](https://github.com/huggingface/optimum-habana/tree/main/examples/speech-recognition)</li> |
 | CLIP | :heavy_check_mark: | :heavy_check_mark: | <li>[contrastive image-text training](https://github.com/huggingface/optimum-habana/tree/main/examples/contrastive-image-text)</li> |
 | BridgeTower | :heavy_check_mark: | :heavy_check_mark: | <li>[contrastive image-text training](https://github.com/huggingface/optimum-habana/tree/main/examples/contrastive-image-text)</li> |
```

### Comparing `optimum-habana-1.8.2/README.md` & `optimum-habana-1.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 pip install --upgrade-strategy eager optimum[habana]
 ```
 
 The `--upgrade-strategy eager` option is needed to ensure `optimum-habana` is upgraded to the latest stable release.
 
 > To use DeepSpeed on HPUs, you also need to run the following command:
 >```bash
->pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.12.0
+>pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.13.0
 >```
 
 Optimum Habana is a fast-moving project, and you may want to install it from source:
 
 ```bash
 pip install git+https://github.com/huggingface/optimum-habana.git
 ```
@@ -64,15 +64,15 @@
 ### Quick Start
 
 🤗 Optimum Habana was designed with one goal in mind: **to make training and inference straightforward for any 🤗 Transformers and 🤗 Diffusers user while leveraging the complete power of Gaudi processors**.
 
 #### Transformers Interface
 
 There are two main classes one needs to know:
-- [GaudiTrainer](https://huggingface.co/docs/optimum/habana/package_reference/trainer): the trainer class that takes care of compiling (lazy or eager mode) and distributing the model to run on HPUs, and performing training and evaluation.
+- [GaudiTrainer](https://huggingface.co/docs/optimum/habana/package_reference/trainer): the trainer class that takes care of compiling and distributing the model to run on HPUs, and performing training and evaluation.
 - [GaudiConfig](https://huggingface.co/docs/optimum/habana/package_reference/gaudi_config): the class that enables to configure Habana Mixed Precision and to decide whether optimized operators and optimizers should be used or not.
 
 The [GaudiTrainer](https://huggingface.co/docs/optimum/habana/package_reference/trainer) is very similar to the [🤗 Transformers Trainer](https://huggingface.co/docs/transformers/main_classes/trainer), and adapting a script using the Trainer to make it work with Gaudi will mostly consist in simply swapping the `Trainer` class for the `GaudiTrainer` one.
 That's how most of the [example scripts](https://github.com/huggingface/optimum-habana/tree/main/examples) were adapted from their [original counterparts](https://github.com/huggingface/transformers/tree/main/examples/pytorch).
 
 Here is an example:
 ```diff
@@ -158,19 +158,20 @@
 | DistilBERT |:heavy_check_mark: | :heavy_check_mark: | <li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering)</li><li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li> |
 | GPT2             | :heavy_check_mark: | :heavy_check_mark: | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li><li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | BLOOM(Z) | :x: | <div style="text-align:left"><li>DeepSpeed</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | StarCoder | :x: | <div style="text-align:left"><li>Single card</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | GPT-J | <div style="text-align:left"><li>DeepSpeed</li></div> | <div style="text-align:left"><li>Single card</li><li>DeepSpeed</li></div> | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li><li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | GPT-NeoX | <div style="text-align:left"><li>DeepSpeed</li></div> | <div style="text-align:left"><li>DeepSpeed</li></div> | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li><li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | OPT | :x: | <div style="text-align:left"><li>DeepSpeed</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
-| Llama 2 / CodeLlama | <div style="text-align:left"><li>DeepSpeed</li><li>LoRA</li></div> | <div style="text-align:left"><li>DeepSpeed</li><li>LoRA</li></div> | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li><li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
+| Llama 2 / CodeLlama | <div style="text-align:left"><li>DeepSpeed</li><li>LoRA</li></div> | :heavy_check_mark: | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li><li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | StableLM | :x: | <div style="text-align:left"><li>Single card</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
-| Falcon | :x: | <div style="text-align:left"><li>Single card</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
+| Falcon | <div style="text-align:left"><li>LoRA</li></div> | :heavy_check_mark: | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | CodeGen | :x: | <div style="text-align:left"><li>Single card</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | MPT | :x: | <div style="text-align:left"><li>Single card</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
+| Mistral | :x: | <div style="text-align:left"><li>Single card</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | T5 | :heavy_check_mark: | :heavy_check_mark: | <li>[summarization](https://github.com/huggingface/optimum-habana/tree/main/examples/summarization)</li><li>[translation](https://github.com/huggingface/optimum-habana/tree/main/examples/translation)</li><li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering#fine-tuning-t5-on-squad20)</li> |
 | BART | :x: | <div style="text-align:left"><li>Single card</li></div> | <li>[summarization](https://github.com/huggingface/optimum-habana/tree/main/examples/summarization)</li><li>[translation](https://github.com/huggingface/optimum-habana/tree/main/examples/translation)</li><li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering#fine-tuning-t5-on-squad20)</li> |
 | ViT | :heavy_check_mark: | :heavy_check_mark: | <li>[image classification](https://github.com/huggingface/optimum-habana/tree/main/examples/image-classification)</li> |
 | Swin | :heavy_check_mark: | :heavy_check_mark: | <li>[image classification](https://github.com/huggingface/optimum-habana/tree/main/examples/image-classification)</li> |
 | Wav2Vec2 | :heavy_check_mark: | :heavy_check_mark: | <li>[audio classification](https://github.com/huggingface/optimum-habana/tree/main/examples/audio-classification)</li><li>[speech recognition](https://github.com/huggingface/optimum-habana/tree/main/examples/speech-recognition)</li> |
 | CLIP | :heavy_check_mark: | :heavy_check_mark: | <li>[contrastive image-text training](https://github.com/huggingface/optimum-habana/tree/main/examples/contrastive-image-text)</li> |
 | BridgeTower | :heavy_check_mark: | :heavy_check_mark: | <li>[contrastive image-text training](https://github.com/huggingface/optimum-habana/tree/main/examples/contrastive-image-text)</li> |
```

### Comparing `optimum-habana-1.8.2/optimum/habana/__init__.py` & `optimum-habana-1.9.0/optimum/habana/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.8.2/optimum/habana/accelerate/accelerator.py` & `optimum-habana-1.9.0/optimum/habana/accelerate/accelerator.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,45 +31,46 @@
 from accelerate.state import GradientState
 from accelerate.tracking import GeneralTracker, filter_trackers
 from accelerate.utils import (
     AutocastKwargs,
     DeepSpeedPlugin,
     DistributedDataParallelKwargs,
     DistributedType,
-    DynamoBackend,
     FP8RecipeKwargs,
     FullyShardedDataParallelPlugin,
     GradientAccumulationPlugin,
     GradScalerKwargs,
     InitProcessGroupKwargs,
     KwargsHandler,
     LoggerType,
     MegatronLMPlugin,
     PrecisionType,
     ProjectConfiguration,
     RNGType,
-    TorchDynamoPlugin,
+    check_os_kernel,
     is_deepspeed_available,
     parse_choice_from_env,
 )
 from accelerate.utils.operations import _gpu_gather
+from accelerate.utils.other import is_compiled_module
 from torch.optim.lr_scheduler import LRScheduler
 
 
 if is_deepspeed_available():
     from accelerate.utils import (
         DeepSpeedEngineWrapper,
         DeepSpeedOptimizerWrapper,
         DeepSpeedSchedulerWrapper,
         DummyOptim,
         DummyScheduler,
     )
 
+from .data_loader import gaudi_prepare_data_loader
 from .state import GaudiAcceleratorState, GaudiPartialState
-from .utils import GaudiDistributedType
+from .utils import GaudiDistributedType, GaudiDynamoBackend, GaudiTorchDynamoPlugin
 
 
 logger = get_logger(__name__)
 
 
 class GaudiAccelerator(Accelerator):
     """
@@ -91,17 +92,18 @@
         project_dir: str | os.PathLike | None = None,
         project_config: ProjectConfiguration | None = None,
         gradient_accumulation_plugin: GradientAccumulationPlugin | None = None,
         dispatch_batches: bool | None = None,
         even_batches: bool = True,
         step_scheduler_with_optimizer: bool = True,
         kwargs_handlers: list[KwargsHandler] | None = None,
-        dynamo_backend: DynamoBackend | str | None = None,
+        dynamo_backend: GaudiDynamoBackend | str | None = None,
         distribution_strategy: str = None,
     ):
+        self.trackers = []
         if project_config is not None:
             self.project_configuration = project_config
         else:
             self.project_configuration = ProjectConfiguration(project_dir=project_dir)
         if project_dir is not None and self.project_dir is None:
             self.project_configuration.set_directories(project_dir)
         if mixed_precision is not None:
@@ -109,28 +111,30 @@
             if mixed_precision not in PrecisionType:
                 raise ValueError(
                     f"Unknown mixed_precision mode: {mixed_precision}. Choose between {PrecisionType.list()}"
                 )
             elif mixed_precision == "fp16":
                 raise ValueError("fp16 is not supported on Habana Gaudi.")
 
-        dynamo_plugin = TorchDynamoPlugin() if dynamo_backend is None else TorchDynamoPlugin(backend=dynamo_backend)
+        dynamo_plugin = (
+            GaudiTorchDynamoPlugin() if dynamo_backend is None else GaudiTorchDynamoPlugin(backend=dynamo_backend)
+        )
 
         if deepspeed_plugin is None:  # init from env variables
             deepspeed_plugin = (
                 DeepSpeedPlugin() if os.environ.get("ACCELERATE_USE_DEEPSPEED", "false") == "true" else None
             )
         else:
             if not isinstance(deepspeed_plugin, DeepSpeedPlugin):
                 raise TypeError("`deepspeed_plugin` must be an `accelerate.utils.DeepSpeedPlugin` object.")
             os.environ["ACCELERATE_USE_DEEPSPEED"] = "true"  # use DeepSpeed if plugin is provided
         if deepspeed_plugin:
             if not is_deepspeed_available():
                 raise ImportError(
-                    "DeepSpeed is not installed => run `pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.12.0`."
+                    "DeepSpeed is not installed => run `pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.13.0`."
                 )
 
             mixed_precision = (
                 os.environ.get("ACCELERATE_MIXED_PRECISION", "no") if mixed_precision is None else mixed_precision
             )
             deepspeed_plugin.set_mixed_precision(mixed_precision)
             deepspeed_plugin.set_deepspeed_weakref()
@@ -240,14 +244,16 @@
             self.rng_types = ["generator"]
 
         # Set a flag tensor for early stopping and other breakpoints
         self.flag_tensor = None
 
         self._distribution_strategy = distribution_strategy
 
+        check_os_kernel()
+
     @property
     def use_fp16(self):
         raise ValueError("fp16 is not supported on Habana Gaudi.")
 
     def prepare_model(self, model: torch.nn.Module, device_placement: bool = None, evaluation_mode: bool = False):
         """
         Prepares a PyTorch model for training in any distributed setup. It is recommended to use
@@ -357,16 +363,16 @@
         #         )
         #     model.forward = fp8_autocast(enabled=fp8_enabled, fp8_recipe=fp8_recipe)(model.forward)
         if not evaluation_mode:
             if self.distributed_type == GaudiDistributedType.MULTI_HPU and self._distribution_strategy != "fast_ddp":
                 if any(p.requires_grad for p in model.parameters()):
                     kwargs = self.ddp_handler.to_kwargs() if self.ddp_handler is not None else {}
                     model = torch.nn.parallel.DistributedDataParallel(model, **kwargs)
-        # torch.compile should be called last.
-        if self.state.dynamo_plugin.backend != DynamoBackend.NO:
+        # torch.compile should be called last and only if the model isn't already compiled.
+        if self.state.dynamo_plugin.backend != GaudiDynamoBackend.NO and not is_compiled_module(model):
             model = torch.compile(model, **self.state.dynamo_plugin.to_kwargs())
         return model
 
     def _prepare_deepspeed(self, *args):
         import deepspeed
 
         deepspeed_plugin = self.state.deepspeed_plugin
@@ -578,14 +584,65 @@
                 self._schedulers.append(scheduler)
             if len(self._models) > 1:
                 raise AssertionError(
                     "You can't use same `Accelerator()` instance with multiple models when using DeepSpeed"
                 )
         return tuple(result)
 
+    def prepare_data_loader(
+        self, data_loader: torch.utils.data.DataLoader, device_placement=None, slice_fn_for_dispatch=None
+    ):
+        """
+        Prepares a PyTorch DataLoader for training in any distributed setup. It is recommended to use
+        [`Accelerator.prepare`] instead.
+
+        Args:
+            data_loader (`torch.utils.data.DataLoader`):
+                A vanilla PyTorch DataLoader to prepare
+            device_placement (`bool`, *optional*):
+                Whether or not to place the batches on the proper device in the prepared dataloader. Will default to
+                `self.device_placement`.
+            slice_fn_for_dispatch (`Callable`, *optional*`):
+                If passed, this function will be used to slice tensors across `num_processes`. Will default to
+                [`~utils.slice_tensors`]. This argument is used only when `dispatch_batches` is set to `True` and will
+                be ignored otherwise.
+
+        Example:
+
+        ```python
+        >>> import torch
+        >>> from accelerate import Accelerator
+
+        >>> accelerator = Accelerator()
+        >>> data_loader = torch.utils.data.DataLoader(...)
+        >>> data_loader = accelerator.prepare_data_loader(data_loader, device_placement=True)
+        ```
+        """
+        # Ensure we can't double wrap a DataLoader due to `find_batch_size`
+        if getattr(data_loader, "_is_accelerate_prepared", False):
+            if data_loader not in self._dataloaders:
+                self._dataloaders.append(data_loader)
+            return data_loader
+        if device_placement is None:
+            device_placement = self.device_placement
+        prepared_data_loader = gaudi_prepare_data_loader(
+            data_loader,
+            self.device,
+            num_processes=self.num_processes,
+            process_index=self.process_index,
+            split_batches=self.split_batches,
+            put_on_device=device_placement,
+            rng_types=self.rng_types.copy(),
+            dispatch_batches=self.dispatch_batches,
+            even_batches=self.even_batches,
+            slice_fn_for_dispatch=slice_fn_for_dispatch,
+        )
+        self._dataloaders.append(prepared_data_loader)
+        return prepared_data_loader
+
     def gather(self, tensor):
         """
         Gather the values in *tensor* across all processes and concatenate them on the first dimension. Useful to
         regroup the predictions from all processes when doing evaluation.
 
         Note:
             This gather happens in all processes.
```

### Comparing `optimum-habana-1.8.2/optimum/habana/accelerate/state.py` & `optimum-habana-1.9.0/optimum/habana/accelerate/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,26 +47,25 @@
                 world_size, rank, local_rank = initialize_distributed_hpu()
                 self.backend = kwargs.pop("backend", "hccl")
 
                 if os.environ.get("ACCELERATE_USE_DEEPSPEED", "false") == "true":
                     if not is_deepspeed_available():
                         raise ImportError(
                             "DeepSpeed is not available, install it with: `pip install"
-                            " git+https://github.com/HabanaAI/DeepSpeed.git@1.12.0`."
+                            " git+https://github.com/HabanaAI/DeepSpeed.git@1.13.0`."
                         )
                     self.distributed_type = GaudiDistributedType.DEEPSPEED
-                    if not torch.distributed.is_initialized():
-                        import deepspeed
+                    import deepspeed
 
-                        if world_size > 1:
-                            os.environ["HLS_MODULE_ID"] = str(local_rank)
-                            os.environ["ID"] = str(rank)
+                    if world_size > 1:
+                        os.environ["HLS_MODULE_ID"] = str(local_rank)
+                        os.environ["ID"] = str(rank)
 
-                        deepspeed.init_distributed(dist_backend=self.backend, **kwargs)
-                        logger.info("DeepSpeed is enabled.")
+                    deepspeed.init_distributed(dist_backend=self.backend, **kwargs)
+                    logger.info("DeepSpeed is enabled.")
                     self._mixed_precision = "no"  # deepspeed handles mixed_precision using deepspeed_config
                 else:
                     self.distributed_type = GaudiDistributedType.MULTI_HPU
                     if not torch.distributed.is_initialized():
                         torch.distributed.init_process_group(backend=self.backend, rank=rank, world_size=world_size)
                         logger.info("Enabled distributed run.")
                 self.num_processes = world_size
```

### Comparing `optimum-habana-1.8.2/optimum/habana/diffusers/models/unet_2d_condition.py` & `optimum-habana-1.9.0/optimum/habana/diffusers/models/unet_2d_condition.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, Dict, Optional, Tuple, Union
 
 import torch
 from diffusers.models.unet_2d_condition import UNet2DConditionOutput
+from diffusers.utils import USE_PEFT_BACKEND, deprecate, scale_lora_layers, unscale_lora_layers
 
 from optimum.utils import logging
 
 
 logger = logging.get_logger(__name__)
 
 
@@ -17,14 +18,15 @@
     class_labels: Optional[torch.Tensor] = None,
     timestep_cond: Optional[torch.Tensor] = None,
     attention_mask: Optional[torch.Tensor] = None,
     cross_attention_kwargs: Optional[Dict[str, Any]] = None,
     added_cond_kwargs: Optional[Dict[str, torch.Tensor]] = None,
     down_block_additional_residuals: Optional[Tuple[torch.Tensor]] = None,
     mid_block_additional_residual: Optional[torch.Tensor] = None,
+    down_intrablock_additional_residuals: Optional[Tuple[torch.Tensor]] = None,
     encoder_attention_mask: Optional[torch.Tensor] = None,
     return_dict: bool = True,
 ) -> Union[UNet2DConditionOutput, Tuple]:
     r"""
     Copied from: https://github.com/huggingface/diffusers/blob/v0.19.3/src/diffusers/models/unet_2d_condition.py#L700
 
     Adds a workaround to be able to compute `conv_in` with Torch Autocast and full bf16 precision.
@@ -35,17 +37,19 @@
     # on the fly if necessary.
     default_overall_up_factor = 2**self.num_upsamplers
 
     # upsample size should be forwarded when sample is not a multiple of `default_overall_up_factor`
     forward_upsample_size = False
     upsample_size = None
 
-    if any(s % default_overall_up_factor != 0 for s in sample.shape[-2:]):
-        logger.info("Forward upsample size to force interpolation output size.")
-        forward_upsample_size = True
+    for dim in sample.shape[-2:]:
+        if dim % default_overall_up_factor != 0:
+            # Forward upsample size to force interpolation output size.
+            forward_upsample_size = True
+            break
 
     # ensure attention_mask is a bias, and give it a singleton query_tokens dimension
     # expects mask of shape:
     #   [batch, key_tokens]
     # adds singleton query_tokens dimension:
     #   [batch,                    1, key_tokens]
     # this helps to broadcast it as a bias over attention scores, which will be in one of the following shapes:
@@ -135,15 +139,14 @@
         if "time_ids" not in added_cond_kwargs:
             raise ValueError(
                 f"{self.__class__} has the config param `addition_embed_type` set to 'text_time' which requires the keyword argument `time_ids` to be passed in `added_cond_kwargs`"
             )
         time_ids = added_cond_kwargs.get("time_ids")
         time_embeds = self.add_time_proj(time_ids.flatten())
         time_embeds = time_embeds.reshape((text_embeds.shape[0], -1))
-
         add_embeds = torch.concat([text_embeds, time_embeds], dim=-1)
         add_embeds = add_embeds.to(emb.dtype)
         aug_emb = self.add_embedding(add_embeds)
     elif self.config.addition_embed_type == "image":
         # Kandinsky 2.2 - style
         if "image_embeds" not in added_cond_kwargs:
             raise ValueError(
@@ -185,15 +188,16 @@
                 f"{self.__class__} has the config param `encoder_hid_dim_type` set to 'image_proj' which requires the keyword argument `image_embeds` to be passed in  `added_conditions`"
             )
         image_embeds = added_cond_kwargs.get("image_embeds")
         encoder_hidden_states = self.encoder_hid_proj(image_embeds)
     # 2. pre-process
     import habana_frameworks.torch.hpu as hthpu
 
-    # Workaround for Synapse 1.11 for Torch Autocast
+    # Workaround for SynapseAI 1.11 for Torch Autocast
+    # TODO: to remove in SynapseAI 1.13?
     if hthpu.is_autocast_hpu_enabled():
         sample = self.conv_in(sample.to(torch.float))
     # Workaround for Synapse 1.11 for full bf16
     elif self.conv_in.bias.dtype == torch.float and sample.dtype == torch.bfloat16:
         sample = self.conv_in(sample.to(torch.float)).to(torch.bfloat16)
     else:
         sample = self.conv_in(sample)
@@ -202,40 +206,57 @@
     if cross_attention_kwargs is not None and cross_attention_kwargs.get("gligen", None) is not None:
         cross_attention_kwargs = cross_attention_kwargs.copy()
         gligen_args = cross_attention_kwargs.pop("gligen")
         cross_attention_kwargs["gligen"] = {"objs": self.position_net(**gligen_args)}
 
     # 3. down
     lora_scale = cross_attention_kwargs.get("scale", 1.0) if cross_attention_kwargs is not None else 1.0
+    if USE_PEFT_BACKEND:
+        # weight the lora layers by setting `lora_scale` for each PEFT layer
+        scale_lora_layers(self, lora_scale)
 
     is_controlnet = mid_block_additional_residual is not None and down_block_additional_residuals is not None
-    is_adapter = mid_block_additional_residual is None and down_block_additional_residuals is not None
+    # using new arg down_intrablock_additional_residuals for T2I-Adapters, to distinguish from controlnets
+    is_adapter = down_intrablock_additional_residuals is not None
+    # maintain backward compatibility for legacy usage, where
+    #       T2I-Adapter and ControlNet both use down_block_additional_residuals arg
+    #       but can only use one or the other
+    if not is_adapter and mid_block_additional_residual is None and down_block_additional_residuals is not None:
+        deprecate(
+            "T2I should not use down_block_additional_residuals",
+            "1.3.0",
+            "Passing intrablock residual connections with `down_block_additional_residuals` is deprecated \
+                    and will be removed in diffusers 1.3.0.  `down_block_additional_residuals` should only be used \
+                    for ControlNet. Please make sure use `down_intrablock_additional_residuals` instead. ",
+            standard_warn=False,
+        )
+        down_intrablock_additional_residuals = down_block_additional_residuals
+        is_adapter = True
 
     down_block_res_samples = (sample,)
     for downsample_block in self.down_blocks:
         if hasattr(downsample_block, "has_cross_attention") and downsample_block.has_cross_attention:
             # For t2i-adapter CrossAttnDownBlock2D
             additional_residuals = {}
-            if is_adapter and len(down_block_additional_residuals) > 0:
-                additional_residuals["additional_residuals"] = down_block_additional_residuals.pop(0)
+            if is_adapter and len(down_intrablock_additional_residuals) > 0:
+                additional_residuals["additional_residuals"] = down_intrablock_additional_residuals.pop(0)
 
             sample, res_samples = downsample_block(
                 hidden_states=sample,
                 temb=emb,
                 encoder_hidden_states=encoder_hidden_states,
                 attention_mask=attention_mask,
                 cross_attention_kwargs=cross_attention_kwargs,
                 encoder_attention_mask=encoder_attention_mask,
                 **additional_residuals,
             )
         else:
             sample, res_samples = downsample_block(hidden_states=sample, temb=emb, scale=lora_scale)
-
-            if is_adapter and len(down_block_additional_residuals) > 0:
-                sample += down_block_additional_residuals.pop(0)
+            if is_adapter and len(down_intrablock_additional_residuals) > 0:
+                sample += down_intrablock_additional_residuals.pop(0)
 
         down_block_res_samples += res_samples
 
     if is_controlnet:
         new_down_block_res_samples = ()
 
         for down_block_res_sample, down_block_additional_residual in zip(
@@ -244,29 +265,33 @@
             down_block_res_sample = down_block_res_sample + down_block_additional_residual
             new_down_block_res_samples = new_down_block_res_samples + (down_block_res_sample,)
 
         down_block_res_samples = new_down_block_res_samples
 
     # 4. mid
     if self.mid_block is not None:
-        sample = self.mid_block(
-            sample,
-            emb,
-            encoder_hidden_states=encoder_hidden_states,
-            attention_mask=attention_mask,
-            cross_attention_kwargs=cross_attention_kwargs,
-            encoder_attention_mask=encoder_attention_mask,
-        )
+        if hasattr(self.mid_block, "has_cross_attention") and self.mid_block.has_cross_attention:
+            sample = self.mid_block(
+                sample,
+                emb,
+                encoder_hidden_states=encoder_hidden_states,
+                attention_mask=attention_mask,
+                cross_attention_kwargs=cross_attention_kwargs,
+                encoder_attention_mask=encoder_attention_mask,
+            )
+        else:
+            sample = self.mid_block(sample, emb)
+
         # To support T2I-Adapter-XL
         if (
             is_adapter
-            and len(down_block_additional_residuals) > 0
-            and sample.shape == down_block_additional_residuals[0].shape
+            and len(down_intrablock_additional_residuals) > 0
+            and sample.shape == down_intrablock_additional_residuals[0].shape
         ):
-            sample += down_block_additional_residuals.pop(0)
+            sample += down_intrablock_additional_residuals.pop(0)
 
     if is_controlnet:
         sample = sample + mid_block_additional_residual
 
     # 5. up
     for i, upsample_block in enumerate(self.up_blocks):
         is_final_block = i == len(self.up_blocks) - 1
@@ -301,11 +326,15 @@
 
     # 6. post-process
     if self.conv_norm_out:
         sample = self.conv_norm_out(sample)
         sample = self.conv_act(sample)
     sample = self.conv_out(sample)
 
+    if USE_PEFT_BACKEND:
+        # remove `lora_scale` from each PEFT layer
+        unscale_lora_layers(self, lora_scale)
+
     if not return_dict:
         return (sample,)
 
     return UNet2DConditionOutput(sample=sample)
```

### Comparing `optimum-habana-1.8.2/optimum/habana/diffusers/pipelines/pipeline_utils.py` & `optimum-habana-1.9.0/optimum/habana/diffusers/pipelines/pipeline_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 # limitations under the License.
 
 import copy
 import importlib
 import inspect
 import os
 import sys
-import tempfile
-import warnings
 from typing import Optional, Union
 
 import torch
 from diffusers.pipelines import DiffusionPipeline
 from diffusers.utils.torch_utils import is_compiled_module
 from huggingface_hub import create_repo
 
@@ -106,61 +104,23 @@
                 # Config already initialized
                 self.gaudi_config = copy.deepcopy(gaudi_config)
             else:
                 raise ValueError(
                     f"`gaudi_config` must be a string or a GaudiConfig object but is {type(gaudi_config)}."
                 )
 
-            if self.gaudi_config.use_habana_mixed_precision or self.gaudi_config.use_torch_autocast:
+            if self.gaudi_config.use_torch_autocast:
                 if bf16_full_eval:
                     logger.warning(
-                        "`use_habana_mixed_precision` or `use_torch_autocast` is True in the given Gaudi configuration but "
+                        "`use_torch_autocast` is True in the given Gaudi configuration but "
                         "`torch_dtype=torch.blfloat16` was given. Disabling mixed precision and continuing in bf16 only."
                     )
                     self.gaudi_config.use_torch_autocast = False
-                    self.gaudi_config.use_habana_mixed_precision = False
-                elif self.gaudi_config.use_torch_autocast:
-                    # Open temporary files to write mixed-precision ops
-                    with tempfile.NamedTemporaryFile() as hmp_bf16_file:
-                        with tempfile.NamedTemporaryFile() as hmp_fp32_file:
-                            self.gaudi_config.write_bf16_fp32_ops_to_text_files(
-                                hmp_bf16_file.name,
-                                hmp_fp32_file.name,
-                            )
-                            os.environ["LOWER_LIST"] = str(hmp_bf16_file)
-                            os.environ["FP32_LIST"] = str(hmp_fp32_file)
-
-                            import habana_frameworks.torch.core  # noqa
-                elif self.gaudi_config.use_habana_mixed_precision:
-                    try:
-                        from habana_frameworks.torch.hpex import hmp
-                    except ImportError as error:
-                        error.msg = f"Could not import habana_frameworks.torch.hpex. {error.msg}."
-                        raise error
-
-                    warnings.warn(
-                        "Habana Mixed Precision is deprecated and will be removed in SynapseAI v1.12. Please"
-                        " use Torch Autocast instead setting `use_torch_autocast=true` in your Gaudi configuration.",
-                        FutureWarning,
-                    )
-
-                    # Open temporary files to write mixed-precision ops
-                    with tempfile.NamedTemporaryFile() as hmp_bf16_file:
-                        with tempfile.NamedTemporaryFile() as hmp_fp32_file:
-                            # hmp.convert needs ops to be written in text files
-                            self.gaudi_config.write_bf16_fp32_ops_to_text_files(
-                                hmp_bf16_file.name,
-                                hmp_fp32_file.name,
-                            )
-                            hmp.convert(
-                                opt_level=self.gaudi_config.hmp_opt_level,
-                                bf16_file_path=hmp_bf16_file.name,
-                                fp32_file_path=hmp_fp32_file.name,
-                                isVerbose=self.gaudi_config.hmp_is_verbose,
-                            )
+                else:
+                    self.gaudi_config.declare_autocast_bf16_fp32_ops()
 
             # Workaround for Synapse 1.11 for full bf16 and Torch Autocast
             if bf16_full_eval or self.gaudi_config.use_torch_autocast:
                 import diffusers
 
                 from ..models import gaudi_unet_2d_condition_model_forward
```

### Comparing `optimum-habana-1.8.2/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py` & `optimum-habana-1.9.0/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_ldm3d.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,78 +11,65 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import inspect
 import time
+import warnings
 from dataclasses import dataclass
 from math import ceil
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import numpy as np
 import PIL
 import torch
-from diffusers.configuration_utils import FrozenDict
-from diffusers.image_processor import VaeImageProcessor
+from diffusers.image_processor import VaeImageProcessorLDM3D
 from diffusers.loaders import FromSingleFileMixin, LoraLoaderMixin, TextualInversionLoaderMixin
 from diffusers.models import AutoencoderKL, UNet2DConditionModel
 from diffusers.models.lora import adjust_lora_scale_text_encoder
 from diffusers.pipelines.stable_diffusion import StableDiffusionSafetyChecker
 from diffusers.schedulers import KarrasDiffusionSchedulers
-from diffusers.utils import BaseOutput, deprecate
-from packaging import version
+from diffusers.utils import USE_PEFT_BACKEND, BaseOutput, deprecate, scale_lora_layers, unscale_lora_layers
 from transformers import CLIPImageProcessor, CLIPTextModel, CLIPTokenizer
 
 from optimum.utils import logging
 
 from ....transformers.gaudi_configuration import GaudiConfig
 from ....utils import speed_metrics
 from ..pipeline_utils import GaudiDiffusionPipeline
 
 
 logger = logging.get_logger(__name__)
 
 
 @dataclass
-class GaudiStableDiffusionPipelineOutput(BaseOutput):
-    images: Union[List[PIL.Image.Image], np.ndarray]
-    nsfw_content_detected: Optional[List[bool]]
+class GaudiStableDiffusionLDM3DPipelineOutput(BaseOutput):
+    rgb: Union[List[PIL.Image.Image], np.ndarray]
+    depth: Union[List[PIL.Image.Image], np.ndarray]
     throughput: float
+    nsfw_content_detected: Optional[List[bool]]
 
 
-def rescale_noise_cfg(noise_cfg, noise_pred_text, guidance_rescale=0.0):
-    """
-    Rescale `noise_cfg` according to `guidance_rescale`. Based on findings of [Common Diffusion Noise Schedules and
-    Sample Steps are Flawed](https://arxiv.org/pdf/2305.08891.pdf). See Section 3.4
-    """
-    std_text = noise_pred_text.std(dim=list(range(1, noise_pred_text.ndim)), keepdim=True)
-    std_cfg = noise_cfg.std(dim=list(range(1, noise_cfg.ndim)), keepdim=True)
-    # rescale the results from guidance (fixes overexposure)
-    noise_pred_rescaled = noise_cfg * (std_text / std_cfg)
-    # mix with the original results from guidance by factor guidance_rescale to avoid "plain looking" images
-    noise_cfg = guidance_rescale * noise_pred_rescaled + (1 - guidance_rescale) * noise_cfg
-    return noise_cfg
-
-
-class GaudiStableDiffusionPipeline(
+class GaudiStableDiffusionLDM3DPipeline(
     GaudiDiffusionPipeline, TextualInversionLoaderMixin, LoraLoaderMixin, FromSingleFileMixin
 ):
     """
     Extends the [`StableDiffusionPipeline`](https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion#diffusers.StableDiffusionPipeline) class:
     - Generation is performed by batches
     - Two `mark_step()` were added to add support for lazy mode
     - Added support for HPU graphs
+    - Adjusted original Stable Diffusion to match with the LDM3D implementation (input and output being different)
 
     Args:
         vae ([`AutoencoderKL`]):
             Variational Auto-Encoder (VAE) model to encode and decode images to and from latent representations.
         text_encoder ([`~transformers.CLIPTextModel`]):
             Frozen text-encoder ([clip-vit-large-patch14](https://huggingface.co/openai/clip-vit-large-patch14)).
-        tokenizer (`~transformers.CLIPTokenizer`):
+        tokenizer ([`~transformers.CLIPTokenizer`]):
             A `CLIPTokenizer` to tokenize text.
         unet ([`UNet2DConditionModel`]):
             A `UNet2DConditionModel` to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
             A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
             [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
         safety_checker ([`StableDiffusionSafetyChecker`]):
@@ -129,41 +116,14 @@
             bf16_full_eval,
         )
 
         # Workaround for Synapse 1.11 for full bf16
         if bf16_full_eval:
             unet.conv_in.float()
 
-        if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
-            deprecation_message = (
-                f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
-                f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
-                "to update the config accordingly as leaving `steps_offset` might led to incorrect results"
-                " in future versions. If you have downloaded this checkpoint from the Hugging Face Hub,"
-                " it would be very nice if you could open a Pull request for the `scheduler/scheduler_config.json`"
-                " file"
-            )
-            deprecate("steps_offset!=1", "1.0.0", deprecation_message, standard_warn=False)
-            new_config = dict(scheduler.config)
-            new_config["steps_offset"] = 1
-            scheduler._internal_dict = FrozenDict(new_config)
-
-        if hasattr(scheduler.config, "clip_sample") and scheduler.config.clip_sample is True:
-            deprecation_message = (
-                f"The configuration file of this scheduler: {scheduler} has not set the configuration `clip_sample`."
-                " `clip_sample` should be set to False in the configuration file. Please make sure to update the"
-                " config accordingly as not setting `clip_sample` in the config might lead to incorrect results in"
-                " future versions. If you have downloaded this checkpoint from the Hugging Face Hub, it would be very"
-                " nice if you could open a Pull request for the `scheduler/scheduler_config.json` file"
-            )
-            deprecate("clip_sample not set", "1.0.0", deprecation_message, standard_warn=False)
-            new_config = dict(scheduler.config)
-            new_config["clip_sample"] = False
-            scheduler._internal_dict = FrozenDict(new_config)
-
         if safety_checker is None and requires_safety_checker:
             logger.warning(
                 f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
                 " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
                 " results in services or applications open to the public. Both the diffusers team and Hugging Face"
                 " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
                 " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
@@ -172,46 +132,25 @@
 
         if safety_checker is not None and feature_extractor is None:
             raise ValueError(
                 "Make sure to define a feature extractor when loading {self.__class__} if you want to use the safety"
                 " checker. If you do not want to use the safety checker, you can pass `'safety_checker=None'` instead."
             )
 
-        is_unet_version_less_0_9_0 = hasattr(unet.config, "_diffusers_version") and version.parse(
-            version.parse(unet.config._diffusers_version).base_version
-        ) < version.parse("0.9.0.dev0")
-        is_unet_sample_size_less_64 = hasattr(unet.config, "sample_size") and unet.config.sample_size < 64
-        if is_unet_version_less_0_9_0 and is_unet_sample_size_less_64:
-            deprecation_message = (
-                "The configuration file of the unet has set the default `sample_size` to smaller than"
-                " 64 which seems highly unlikely. If your checkpoint is a fine-tuned version of any of the"
-                " following: \n- CompVis/stable-diffusion-v1-4 \n- CompVis/stable-diffusion-v1-3 \n-"
-                " CompVis/stable-diffusion-v1-2 \n- CompVis/stable-diffusion-v1-1 \n- runwayml/stable-diffusion-v1-5"
-                " \n- runwayml/stable-diffusion-inpainting \n you should change 'sample_size' to 64 in the"
-                " configuration file. Please make sure to update the config accordingly as leaving `sample_size=32`"
-                " in the config might lead to incorrect results in future versions. If you have downloaded this"
-                " checkpoint from the Hugging Face Hub, it would be very nice if you could open a Pull request for"
-                " the `unet/config.json` file"
-            )
-            deprecate("sample_size<64", "1.0.0", deprecation_message, standard_warn=False)
-            new_config = dict(unet.config)
-            new_config["sample_size"] = 64
-            unet._internal_dict = FrozenDict(new_config)
-
         self.register_modules(
             vae=vae,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
         self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
-        self.image_processor = VaeImageProcessor(vae_scale_factor=self.vae_scale_factor)
+        self.image_processor = VaeImageProcessorLDM3D(vae_scale_factor=self.vae_scale_factor)
         self.register_to_config(requires_safety_checker=requires_safety_checker)
 
         self.to(self._device)
 
     @property
     def _execution_device(self):
         r"""
@@ -236,27 +175,29 @@
         device,
         num_images_per_prompt,
         do_classifier_free_guidance,
         negative_prompt=None,
         prompt_embeds: Optional[torch.FloatTensor] = None,
         negative_prompt_embeds: Optional[torch.FloatTensor] = None,
         lora_scale: Optional[float] = None,
+        **kwargs,
     ):
         deprecation_message = "`_encode_prompt()` is deprecated and it will be removed in a future version. Use `encode_prompt()` instead. Also, be aware that the output format changed from a concatenated tensor to a tuple."
         deprecate("_encode_prompt()", "1.0.0", deprecation_message, standard_warn=False)
 
         prompt_embeds_tuple = self.encode_prompt(
             prompt=prompt,
             device=device,
             num_images_per_prompt=num_images_per_prompt,
             do_classifier_free_guidance=do_classifier_free_guidance,
             negative_prompt=negative_prompt,
             prompt_embeds=prompt_embeds,
             negative_prompt_embeds=negative_prompt_embeds,
             lora_scale=lora_scale,
+            **kwargs,
         )
 
         # concatenate for backwards comp
         prompt_embeds = torch.cat([prompt_embeds_tuple[1], prompt_embeds_tuple[0]])
 
         return prompt_embeds
 
@@ -266,14 +207,15 @@
         device,
         num_images_per_prompt,
         do_classifier_free_guidance,
         negative_prompt=None,
         prompt_embeds: Optional[torch.FloatTensor] = None,
         negative_prompt_embeds: Optional[torch.FloatTensor] = None,
         lora_scale: Optional[float] = None,
+        clip_skip: Optional[int] = None,
     ):
         r"""
         Encodes the prompt into text encoder hidden states.
 
         Args:
             prompt (`str` or `List[str]`, *optional*):
                 prompt to be encoded
@@ -291,23 +233,29 @@
                 Pre-generated text embeddings. Can be used to easily tweak text inputs, *e.g.* prompt weighting. If not
                 provided, text embeddings will be generated from `prompt` input argument.
             negative_prompt_embeds (`torch.FloatTensor`, *optional*):
                 Pre-generated negative text embeddings. Can be used to easily tweak text inputs, *e.g.* prompt
                 weighting. If not provided, negative_prompt_embeds will be generated from `negative_prompt` input
                 argument.
             lora_scale (`float`, *optional*):
-                A lora scale that will be applied to all LoRA layers of the text encoder if LoRA layers are loaded.
+                A LoRA scale that will be applied to all LoRA layers of the text encoder if LoRA layers are loaded.
+            clip_skip (`int`, *optional*):
+                Number of layers to be skipped from CLIP while computing the prompt embeddings. A value of 1 means that
+                the output of the pre-final layer will be used for computing the prompt embeddings.
         """
         # set lora scale so that monkey patched LoRA
         # function of text encoder can correctly access it
         if lora_scale is not None and isinstance(self, LoraLoaderMixin):
             self._lora_scale = lora_scale
 
             # dynamically adjust the LoRA scale
-            adjust_lora_scale_text_encoder(self.text_encoder, lora_scale)
+            if not USE_PEFT_BACKEND:
+                adjust_lora_scale_text_encoder(self.text_encoder, lora_scale)
+            else:
+                scale_lora_layers(self.text_encoder, lora_scale)
 
         if prompt is not None and isinstance(prompt, str):
             num_prompts = 1
         elif prompt is not None and isinstance(prompt, list):
             num_prompts = len(prompt)
         else:
             num_prompts = prompt_embeds.shape[0]
@@ -339,19 +287,30 @@
                 )
 
             if hasattr(self.text_encoder.config, "use_attention_mask") and self.text_encoder.config.use_attention_mask:
                 attention_mask = text_inputs.attention_mask.to(device)
             else:
                 attention_mask = None
 
-            prompt_embeds = self.text_encoder(
-                text_input_ids.to(device),
-                attention_mask=attention_mask,
-            )
-            prompt_embeds = prompt_embeds[0]
+            if clip_skip is None:
+                prompt_embeds = self.text_encoder(text_input_ids.to(device), attention_mask=attention_mask)
+                prompt_embeds = prompt_embeds[0]
+            else:
+                prompt_embeds = self.text_encoder(
+                    text_input_ids.to(device), attention_mask=attention_mask, output_hidden_states=True
+                )
+                # Access the `hidden_states` first, that contains a tuple of
+                # all the hidden states from the encoder layers. Then index into
+                # the tuple to access the hidden states from the desired layer.
+                prompt_embeds = prompt_embeds[-1][-(clip_skip + 1)]
+                # We also need to apply the final LayerNorm here to not mess with the
+                # representations. The `last_hidden_states` that we typically use for
+                # obtaining the final prompt representations passes through the LayerNorm
+                # layer.
+                prompt_embeds = self.text_encoder.text_model.final_layer_norm(prompt_embeds)
 
         if self.text_encoder is not None:
             prompt_embeds_dtype = self.text_encoder.dtype
         elif self.unet is not None:
             prompt_embeds_dtype = self.unet.dtype
         else:
             prompt_embeds_dtype = prompt_embeds.dtype
@@ -413,34 +372,41 @@
             seq_len = negative_prompt_embeds.shape[1]
 
             negative_prompt_embeds = negative_prompt_embeds.to(dtype=prompt_embeds_dtype, device=device)
 
             negative_prompt_embeds = negative_prompt_embeds.repeat(1, num_images_per_prompt, 1)
             negative_prompt_embeds = negative_prompt_embeds.view(num_prompts * num_images_per_prompt, seq_len, -1)
 
+        if isinstance(self, LoraLoaderMixin) and USE_PEFT_BACKEND:
+            # Retrieve the original scale by scaling back the LoRA layers
+            unscale_lora_layers(self.text_encoder, lora_scale)
+
         return prompt_embeds, negative_prompt_embeds
 
     def run_safety_checker(self, image, device, dtype):
         if self.safety_checker is None:
             has_nsfw_concept = None
         else:
             if torch.is_tensor(image):
                 feature_extractor_input = self.image_processor.postprocess(image, output_type="pil")
             else:
                 feature_extractor_input = self.image_processor.numpy_to_pil(image)
-            safety_checker_input = self.feature_extractor(feature_extractor_input, return_tensors="pt").to(device)
+            rgb_feature_extractor_input = feature_extractor_input[0]
+            safety_checker_input = self.feature_extractor(rgb_feature_extractor_input, return_tensors="pt").to(device)
             image, has_nsfw_concept = self.safety_checker(
                 images=image, clip_input=safety_checker_input.pixel_values.to(dtype)
             )
         return image, has_nsfw_concept
 
     def decode_latents(self, latents):
-        deprecation_message = "The decode_latents method is deprecated and will be removed in 1.0.0. Please use VaeImageProcessor.postprocess(...) instead"
-        deprecate("decode_latents", "1.0.0", deprecation_message, standard_warn=False)
-
+        warnings.warn(
+            "The decode_latents method is deprecated and will be removed in a future version. Please"
+            " use VaeImageProcessor instead",
+            FutureWarning,
+        )
         latents = 1 / self.vae.config.scaling_factor * latents
         image = self.vae.decode(latents, return_dict=False)[0]
         image = (image / 2 + 0.5).clamp(0, 1)
         # we always cast to float32 as this does not cause significant overhead and is compatible with bfloat16
         image = image.cpu().permute(0, 2, 3, 1).float().numpy()
         return image
 
@@ -466,25 +432,30 @@
         prompt,
         height,
         width,
         callback_steps,
         negative_prompt=None,
         prompt_embeds=None,
         negative_prompt_embeds=None,
+        callback_on_step_end_tensor_inputs=None,
     ):
         if height % 8 != 0 or width % 8 != 0:
             raise ValueError(f"`height` and `width` have to be divisible by 8 but are {height} and {width}.")
 
-        if (callback_steps is None) or (
-            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
-        ):
+        if callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0):
             raise ValueError(
                 f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
                 f" {type(callback_steps)}."
             )
+        if callback_on_step_end_tensor_inputs is not None and not all(
+            k in self._callback_tensor_inputs for k in callback_on_step_end_tensor_inputs
+        ):
+            raise ValueError(
+                f"`callback_on_step_end_tensor_inputs` has to be in {self._callback_tensor_inputs}, but found {[k for k in callback_on_step_end_tensor_inputs if k not in self._callback_tensor_inputs]}"
+            )
 
         if prompt is not None and prompt_embeds is not None:
             raise ValueError(
                 f"Cannot forward both `prompt`: {prompt} and `prompt_embeds`: {prompt_embeds}. Please make sure to"
                 " only forward one of the two."
             )
         elif prompt is None and prompt_embeds is None:
@@ -534,88 +505,100 @@
             latents = latents.to(device)
 
         # scale the initial noise by the standard deviation required by the scheduler
         latents = latents * self.scheduler.init_noise_sigma
         return latents
 
     @classmethod
-    def _split_inputs_into_batches(cls, batch_size, latents, text_embeddings):
+    def _split_inputs_into_batches(cls, batch_size, latents, prompt_embeds, negative_prompt_embeds):
         # Use torch.split to generate num_batches batches of size batch_size
         latents_batches = list(torch.split(latents, batch_size))
-        # If there are uncond embeddings, the batch size of text embeddings is 2x
-        multiple = text_embeddings.shape[0] // latents.shape[0]
-        text_embeddings_batches = list(torch.split(text_embeddings, multiple * batch_size))
+        prompt_embeds_batches = list(torch.split(prompt_embeds, batch_size))
+        if negative_prompt_embeds is not None:
+            negative_prompt_embeds_batches = list(torch.split(negative_prompt_embeds, batch_size))
 
         # If the last batch has less samples than batch_size, pad it with dummy samples
         num_dummy_samples = 0
         if latents_batches[-1].shape[0] < batch_size:
             num_dummy_samples = batch_size - latents_batches[-1].shape[0]
             # Pad latents_batches
             sequence_to_stack = (latents_batches[-1],) + tuple(
                 torch.zeros_like(latents_batches[-1][0][None, :]) for _ in range(num_dummy_samples)
             )
             latents_batches[-1] = torch.vstack(sequence_to_stack)
-            # Pad text_embeddings_batches
-            sequence_to_stack = (text_embeddings_batches[-1],) + tuple(
-                torch.zeros_like(text_embeddings_batches[-1][0][None, :]) for _ in range(multiple * num_dummy_samples)
-            )
-            text_embeddings_batches[-1] = torch.vstack(sequence_to_stack)
+            # Pad prompt_embeds_batches
+            sequence_to_stack = (prompt_embeds_batches[-1],) + tuple(
+                torch.zeros_like(prompt_embeds_batches[-1][0][None, :]) for _ in range(num_dummy_samples)
+            )
+            prompt_embeds_batches[-1] = torch.vstack(sequence_to_stack)
+            # Pad negative_prompt_embeds_batches if necessary
+            if negative_prompt_embeds is not None:
+                sequence_to_stack = (negative_prompt_embeds_batches[-1],) + tuple(
+                    torch.zeros_like(negative_prompt_embeds_batches[-1][0][None, :]) for _ in range(num_dummy_samples)
+                )
+                negative_prompt_embeds_batches[-1] = torch.vstack(sequence_to_stack)
 
         # Stack batches in the same tensor
         latents_batches = torch.stack(latents_batches)
-        text_embeddings_batches = torch.stack(text_embeddings_batches)
+        if negative_prompt_embeds is not None:
+            # For classifier free guidance, we need to do two forward passes.
+            # Here we concatenate the unconditional and text embeddings into a single batch
+            # to avoid doing two forward passes
+            for i, (negative_prompt_embeds_batch, prompt_embeds_batch) in enumerate(
+                zip(negative_prompt_embeds_batches, prompt_embeds_batches[:])
+            ):
+                prompt_embeds_batches[i] = torch.cat([negative_prompt_embeds_batch, prompt_embeds_batch])
+        prompt_embeds_batches = torch.stack(prompt_embeds_batches)
 
-        return latents_batches, text_embeddings_batches, num_dummy_samples
+        return latents_batches, prompt_embeds_batches, num_dummy_samples
 
     @torch.no_grad()
     def __call__(
         self,
         prompt: Union[str, List[str]] = None,
         height: Optional[int] = None,
         width: Optional[int] = None,
         num_inference_steps: int = 50,
-        guidance_scale: float = 7.5,
+        guidance_scale: float = 5.0,
         negative_prompt: Optional[Union[str, List[str]]] = None,
         num_images_per_prompt: Optional[int] = 1,
         batch_size: int = 1,
         eta: float = 0.0,
         generator: Optional[Union[torch.Generator, List[torch.Generator]]] = None,
         latents: Optional[torch.FloatTensor] = None,
         prompt_embeds: Optional[torch.FloatTensor] = None,
         negative_prompt_embeds: Optional[torch.FloatTensor] = None,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
         callback: Optional[Callable[[int, int, torch.FloatTensor], None]] = None,
         callback_steps: int = 1,
         cross_attention_kwargs: Optional[Dict[str, Any]] = None,
-        guidance_rescale: float = 0.0,
+        clip_skip: Optional[int] = None,
     ):
         r"""
         The call function to the pipeline for generation.
 
         Args:
             prompt (`str` or `List[str]`, *optional*):
                 The prompt or prompts to guide image generation. If not defined, you need to pass `prompt_embeds`.
             height (`int`, *optional*, defaults to `self.unet.config.sample_size * self.vae_scale_factor`):
-                The height in pixels of the generated images.
+                The height in pixels of the generated image.
             width (`int`, *optional*, defaults to `self.unet.config.sample_size * self.vae_scale_factor`):
-                The width in pixels of the generated images.
+                The width in pixels of the generated image.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
-            guidance_scale (`float`, *optional*, defaults to 7.5):
+            guidance_scale (`float`, *optional*, defaults to 5.0):
                 A higher guidance scale value encourages the model to generate images closely linked to the text
                 `prompt` at the expense of lower image quality. Guidance scale is enabled when `guidance_scale > 1`.
             negative_prompt (`str` or `List[str]`, *optional*):
                 The prompt or prompts to guide what to not include in image generation. If not defined, you need to
                 pass `negative_prompt_embeds` instead. Ignored when not using guidance (`guidance_scale < 1`).
             num_images_per_prompt (`int`, *optional*, defaults to 1):
                 The number of images to generate per prompt.
-            batch_size (`int`, *optional*, defaults to 1):
-                The number of images in a batch.
             eta (`float`, *optional*, defaults to 0.0):
                 Corresponds to parameter eta (η) from the [DDIM](https://arxiv.org/abs/2010.02502) paper. Only applies
                 to the [`~schedulers.DDIMScheduler`], and is ignored in other schedulers.
             generator (`torch.Generator` or `List[torch.Generator]`, *optional*):
                 A [`torch.Generator`](https://pytorch.org/docs/stable/generated/torch.Generator.html) to make
                 generation deterministic.
             latents (`torch.FloatTensor`, *optional*):
@@ -627,33 +610,32 @@
                 provided, text embeddings are generated from the `prompt` input argument.
             negative_prompt_embeds (`torch.FloatTensor`, *optional*):
                 Pre-generated negative text embeddings. Can be used to easily tweak text inputs (prompt weighting). If
                 not provided, `negative_prompt_embeds` are generated from the `negative_prompt` input argument.
             output_type (`str`, *optional*, defaults to `"pil"`):
                 The output format of the generated image. Choose between `PIL.Image` or `np.array`.
             return_dict (`bool`, *optional*, defaults to `True`):
-                Whether or not to return a [`~diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.GaudiStableDiffusionPipelineOutput`] instead of a
+                Whether or not to return a [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] instead of a
                 plain tuple.
             callback (`Callable`, *optional*):
                 A function that calls every `callback_steps` steps during inference. The function is called with the
                 following arguments: `callback(step: int, timestep: int, latents: torch.FloatTensor)`.
             callback_steps (`int`, *optional*, defaults to 1):
                 The frequency at which the `callback` function is called. If not specified, the callback is called at
                 every step.
             cross_attention_kwargs (`dict`, *optional*):
                 A kwargs dictionary that if specified is passed along to the [`AttentionProcessor`] as defined in
                 [`self.processor`](https://github.com/huggingface/diffusers/blob/main/src/diffusers/models/attention_processor.py).
-            guidance_rescale (`float`, *optional*, defaults to 0.7):
-                Guidance rescale factor from [Common Diffusion Noise Schedules and Sample Steps are
-                Flawed](https://arxiv.org/pdf/2305.08891.pdf). Guidance rescale factor should fix overexposure when
-                using zero terminal SNR.
+            clip_skip (`int`, *optional*):
+                Number of layers to be skipped from CLIP while computing the prompt embeddings. A value of 1 means that
+                the output of the pre-final layer will be used for computing the prompt embeddings.
 
         Returns:
             [`~diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.GaudiStableDiffusionPipelineOutput`] or `tuple`:
-                If `return_dict` is `True`, [`~diffusers.pipelines.stable_diffusion.StableDiffusionPipelineOutput`] is returned,
+                If `return_dict` is `True`, [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] is returned,
                 otherwise a `tuple` is returned where the first element is a list with the generated images and the
                 second element is a list of `bool`s indicating whether the corresponding generated image contains
                 "not-safe-for-work" (nsfw) content.
         """
         with torch.autocast(device_type="hpu", dtype=torch.bfloat16, enabled=self.gaudi_config.use_torch_autocast):
             # 0. Default height and width to unet
             height = height or self.unet.config.sample_size * self.vae_scale_factor
@@ -681,32 +663,24 @@
             device = self._execution_device
             # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
             # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
             # corresponds to doing no classifier free guidance.
             do_classifier_free_guidance = guidance_scale > 1.0
 
             # 3. Encode input prompt
-            text_encoder_lora_scale = (
-                cross_attention_kwargs.get("scale", None) if cross_attention_kwargs is not None else None
-            )
             prompt_embeds, negative_prompt_embeds = self.encode_prompt(
                 prompt,
                 device,
                 num_images_per_prompt,
                 do_classifier_free_guidance,
                 negative_prompt,
                 prompt_embeds=prompt_embeds,
                 negative_prompt_embeds=negative_prompt_embeds,
-                lora_scale=text_encoder_lora_scale,
+                clip_skip=clip_skip,
             )
-            # For classifier free guidance, we need to do two forward passes.
-            # Here we concatenate the unconditional and text embeddings into a single batch
-            # to avoid doing two forward passes
-            if do_classifier_free_guidance:
-                prompt_embeds = torch.cat([negative_prompt_embeds, prompt_embeds])
 
             # 4. Prepare timesteps
             self.scheduler.set_timesteps(num_inference_steps, device="cpu")
             timesteps = self.scheduler.timesteps.to(device)
 
             # 5. Prepare latent variables
             num_channels_latents = self.unet.config.in_channels
@@ -725,18 +699,20 @@
             extra_step_kwargs = self.prepare_extra_step_kwargs(generator, eta)
 
             # 7. Split into batches (HPU-specific step)
             latents_batches, text_embeddings_batches, num_dummy_samples = self._split_inputs_into_batches(
                 batch_size,
                 latents,
                 prompt_embeds,
+                negative_prompt_embeds,
             )
 
             outputs = {
                 "images": [],
+                "depths": [],
                 "has_nsfw_concept": [],
             }
             t0 = time.time()
             t1 = t0
 
             # 8. Denoising loop
             for j in self.progress_bar(range(num_batches)):
@@ -772,29 +748,26 @@
                     )
 
                     # perform guidance
                     if do_classifier_free_guidance:
                         noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
                         noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
 
-                    if do_classifier_free_guidance and guidance_rescale > 0.0:
-                        # Based on 3.4. in https://arxiv.org/pdf/2305.08891.pdf
-                        noise_pred = rescale_noise_cfg(noise_pred, noise_pred_text, guidance_rescale=guidance_rescale)
-
                     # compute the previous noisy sample x_t -> x_t-1
                     latents_batch = self.scheduler.step(
                         noise_pred, latents_batch, **extra_step_kwargs, return_dict=False
                     )[0]
 
                     if not self.use_hpu_graphs:
                         self.htcore.mark_step()
 
                     # call the callback, if provided
                     if callback is not None and i % callback_steps == 0:
-                        callback(i, timestep, latents_batch)
+                        step_idx = i // getattr(self.scheduler, "order", 1)
+                        callback(step_idx, timestep, latents_batch)
 
                 if not output_type == "latent":
                     # 8. Post-processing
                     image = self.vae.decode(latents_batch / self.vae.config.scaling_factor, return_dict=False)[0]
                 else:
                     image = latents_batch
                 outputs["images"].append(image)
@@ -829,35 +802,40 @@
                     image, has_nsfw_concept = self.run_safety_checker(image, device, prompt_embeds.dtype)
 
                 if has_nsfw_concept is None:
                     do_denormalize = [True] * image.shape[0]
                 else:
                     do_denormalize = [not has_nsfw for has_nsfw in has_nsfw_concept]
 
-                image = self.image_processor.postprocess(image, output_type=output_type, do_denormalize=do_denormalize)
+                rgb, depth = self.image_processor.postprocess(
+                    image, output_type=output_type, do_denormalize=do_denormalize
+                )
 
                 if output_type == "pil":
-                    outputs["images"] += image
+                    outputs["images"] += rgb
+                    outputs["depths"] += depth
                 else:
-                    outputs["images"] += [*image]
+                    outputs["images"] += [*rgb]
+                    outputs["depths"] += [*depth]
 
                 if has_nsfw_concept is not None:
                     outputs["has_nsfw_concept"] += has_nsfw_concept
                 else:
                     outputs["has_nsfw_concept"] = None
 
             # Offload all models
             self.maybe_free_model_hooks()
 
             if not return_dict:
-                return (outputs["images"], outputs["has_nsfw_concept"])
+                return ((rgb, depth), has_nsfw_concept)
 
-            return GaudiStableDiffusionPipelineOutput(
-                images=outputs["images"],
-                nsfw_content_detected=outputs["has_nsfw_concept"],
+            return GaudiStableDiffusionLDM3DPipelineOutput(
+                rgb=outputs["images"],
+                depth=outputs["depths"],
+                nsfw_content_detected=has_nsfw_concept,
                 throughput=speed_measures[f"{speed_metrics_prefix}_samples_per_second"],
             )
 
     @torch.no_grad()
     def unet_hpu(self, latent_model_input, timestep, encoder_hidden_states, cross_attention_kwargs, capture):
         if self.use_hpu_graphs:
             return self.capture_replay(latent_model_input, timestep, encoder_hidden_states, capture)
```

### Comparing `optimum-habana-1.8.2/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_ldm3d.py` & `optimum-habana-1.9.0/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,65 +11,78 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import inspect
 import time
-import warnings
 from dataclasses import dataclass
 from math import ceil
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import numpy as np
 import PIL
 import torch
-from diffusers.image_processor import VaeImageProcessorLDM3D
+from diffusers.configuration_utils import FrozenDict
+from diffusers.image_processor import VaeImageProcessor
 from diffusers.loaders import FromSingleFileMixin, LoraLoaderMixin, TextualInversionLoaderMixin
 from diffusers.models import AutoencoderKL, UNet2DConditionModel
 from diffusers.models.lora import adjust_lora_scale_text_encoder
 from diffusers.pipelines.stable_diffusion import StableDiffusionSafetyChecker
 from diffusers.schedulers import KarrasDiffusionSchedulers
-from diffusers.utils import BaseOutput, deprecate
+from diffusers.utils import USE_PEFT_BACKEND, BaseOutput, deprecate, scale_lora_layers, unscale_lora_layers
+from packaging import version
 from transformers import CLIPImageProcessor, CLIPTextModel, CLIPTokenizer
 
 from optimum.utils import logging
 
 from ....transformers.gaudi_configuration import GaudiConfig
 from ....utils import speed_metrics
 from ..pipeline_utils import GaudiDiffusionPipeline
 
 
 logger = logging.get_logger(__name__)
 
 
 @dataclass
-class GaudiStableDiffusionLDM3DPipelineOutput(BaseOutput):
-    rgb: Union[List[PIL.Image.Image], np.ndarray]
-    depth: Union[List[PIL.Image.Image], np.ndarray]
-    throughput: float
+class GaudiStableDiffusionPipelineOutput(BaseOutput):
+    images: Union[List[PIL.Image.Image], np.ndarray]
     nsfw_content_detected: Optional[List[bool]]
+    throughput: float
+
+
+def rescale_noise_cfg(noise_cfg, noise_pred_text, guidance_rescale=0.0):
+    """
+    Rescale `noise_cfg` according to `guidance_rescale`. Based on findings of [Common Diffusion Noise Schedules and
+    Sample Steps are Flawed](https://arxiv.org/pdf/2305.08891.pdf). See Section 3.4
+    """
+    std_text = noise_pred_text.std(dim=list(range(1, noise_pred_text.ndim)), keepdim=True)
+    std_cfg = noise_cfg.std(dim=list(range(1, noise_cfg.ndim)), keepdim=True)
+    # rescale the results from guidance (fixes overexposure)
+    noise_pred_rescaled = noise_cfg * (std_text / std_cfg)
+    # mix with the original results from guidance by factor guidance_rescale to avoid "plain looking" images
+    noise_cfg = guidance_rescale * noise_pred_rescaled + (1 - guidance_rescale) * noise_cfg
+    return noise_cfg
 
 
-class GaudiStableDiffusionLDM3DPipeline(
+class GaudiStableDiffusionPipeline(
     GaudiDiffusionPipeline, TextualInversionLoaderMixin, LoraLoaderMixin, FromSingleFileMixin
 ):
     """
     Extends the [`StableDiffusionPipeline`](https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion#diffusers.StableDiffusionPipeline) class:
     - Generation is performed by batches
     - Two `mark_step()` were added to add support for lazy mode
     - Added support for HPU graphs
-    - Adjusted original Stable Diffusion to match with the LDM3D implementation (input and output being different)
 
     Args:
         vae ([`AutoencoderKL`]):
             Variational Auto-Encoder (VAE) model to encode and decode images to and from latent representations.
         text_encoder ([`~transformers.CLIPTextModel`]):
             Frozen text-encoder ([clip-vit-large-patch14](https://huggingface.co/openai/clip-vit-large-patch14)).
-        tokenizer ([`~transformers.CLIPTokenizer`]):
+        tokenizer (`~transformers.CLIPTokenizer`):
             A `CLIPTokenizer` to tokenize text.
         unet ([`UNet2DConditionModel`]):
             A `UNet2DConditionModel` to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
             A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
             [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
         safety_checker ([`StableDiffusionSafetyChecker`]):
@@ -89,14 +102,15 @@
             Whether to use full bfloat16 evaluation instead of 32-bit.
             This will be faster and save memory compared to fp32/mixed precision but can harm generated images.
     """
 
     model_cpu_offload_seq = "text_encoder->unet->vae"
     _optional_components = ["safety_checker", "feature_extractor"]
     _exclude_from_cpu_offload = ["safety_checker"]
+    _callback_tensor_inputs = ["latents", "prompt_embeds", "negative_prompt_embeds"]
 
     def __init__(
         self,
         vae: AutoencoderKL,
         text_encoder: CLIPTextModel,
         tokenizer: CLIPTokenizer,
         unet: UNet2DConditionModel,
@@ -116,14 +130,41 @@
             bf16_full_eval,
         )
 
         # Workaround for Synapse 1.11 for full bf16
         if bf16_full_eval:
             unet.conv_in.float()
 
+        if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
+            deprecation_message = (
+                f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
+                f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
+                "to update the config accordingly as leaving `steps_offset` might led to incorrect results"
+                " in future versions. If you have downloaded this checkpoint from the Hugging Face Hub,"
+                " it would be very nice if you could open a Pull request for the `scheduler/scheduler_config.json`"
+                " file"
+            )
+            deprecate("steps_offset!=1", "1.0.0", deprecation_message, standard_warn=False)
+            new_config = dict(scheduler.config)
+            new_config["steps_offset"] = 1
+            scheduler._internal_dict = FrozenDict(new_config)
+
+        if hasattr(scheduler.config, "clip_sample") and scheduler.config.clip_sample is True:
+            deprecation_message = (
+                f"The configuration file of this scheduler: {scheduler} has not set the configuration `clip_sample`."
+                " `clip_sample` should be set to False in the configuration file. Please make sure to update the"
+                " config accordingly as not setting `clip_sample` in the config might lead to incorrect results in"
+                " future versions. If you have downloaded this checkpoint from the Hugging Face Hub, it would be very"
+                " nice if you could open a Pull request for the `scheduler/scheduler_config.json` file"
+            )
+            deprecate("clip_sample not set", "1.0.0", deprecation_message, standard_warn=False)
+            new_config = dict(scheduler.config)
+            new_config["clip_sample"] = False
+            scheduler._internal_dict = FrozenDict(new_config)
+
         if safety_checker is None and requires_safety_checker:
             logger.warning(
                 f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
                 " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
                 " results in services or applications open to the public. Both the diffusers team and Hugging Face"
                 " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
                 " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
@@ -132,25 +173,46 @@
 
         if safety_checker is not None and feature_extractor is None:
             raise ValueError(
                 "Make sure to define a feature extractor when loading {self.__class__} if you want to use the safety"
                 " checker. If you do not want to use the safety checker, you can pass `'safety_checker=None'` instead."
             )
 
+        is_unet_version_less_0_9_0 = hasattr(unet.config, "_diffusers_version") and version.parse(
+            version.parse(unet.config._diffusers_version).base_version
+        ) < version.parse("0.9.0.dev0")
+        is_unet_sample_size_less_64 = hasattr(unet.config, "sample_size") and unet.config.sample_size < 64
+        if is_unet_version_less_0_9_0 and is_unet_sample_size_less_64:
+            deprecation_message = (
+                "The configuration file of the unet has set the default `sample_size` to smaller than"
+                " 64 which seems highly unlikely. If your checkpoint is a fine-tuned version of any of the"
+                " following: \n- CompVis/stable-diffusion-v1-4 \n- CompVis/stable-diffusion-v1-3 \n-"
+                " CompVis/stable-diffusion-v1-2 \n- CompVis/stable-diffusion-v1-1 \n- runwayml/stable-diffusion-v1-5"
+                " \n- runwayml/stable-diffusion-inpainting \n you should change 'sample_size' to 64 in the"
+                " configuration file. Please make sure to update the config accordingly as leaving `sample_size=32`"
+                " in the config might lead to incorrect results in future versions. If you have downloaded this"
+                " checkpoint from the Hugging Face Hub, it would be very nice if you could open a Pull request for"
+                " the `unet/config.json` file"
+            )
+            deprecate("sample_size<64", "1.0.0", deprecation_message, standard_warn=False)
+            new_config = dict(unet.config)
+            new_config["sample_size"] = 64
+            unet._internal_dict = FrozenDict(new_config)
+
         self.register_modules(
             vae=vae,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
         self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
-        self.image_processor = VaeImageProcessorLDM3D(vae_scale_factor=self.vae_scale_factor)
+        self.image_processor = VaeImageProcessor(vae_scale_factor=self.vae_scale_factor)
         self.register_to_config(requires_safety_checker=requires_safety_checker)
 
         self.to(self._device)
 
     @property
     def _execution_device(self):
         r"""
@@ -175,27 +237,29 @@
         device,
         num_images_per_prompt,
         do_classifier_free_guidance,
         negative_prompt=None,
         prompt_embeds: Optional[torch.FloatTensor] = None,
         negative_prompt_embeds: Optional[torch.FloatTensor] = None,
         lora_scale: Optional[float] = None,
+        **kwargs,
     ):
         deprecation_message = "`_encode_prompt()` is deprecated and it will be removed in a future version. Use `encode_prompt()` instead. Also, be aware that the output format changed from a concatenated tensor to a tuple."
         deprecate("_encode_prompt()", "1.0.0", deprecation_message, standard_warn=False)
 
         prompt_embeds_tuple = self.encode_prompt(
             prompt=prompt,
             device=device,
             num_images_per_prompt=num_images_per_prompt,
             do_classifier_free_guidance=do_classifier_free_guidance,
             negative_prompt=negative_prompt,
             prompt_embeds=prompt_embeds,
             negative_prompt_embeds=negative_prompt_embeds,
             lora_scale=lora_scale,
+            **kwargs,
         )
 
         # concatenate for backwards comp
         prompt_embeds = torch.cat([prompt_embeds_tuple[1], prompt_embeds_tuple[0]])
 
         return prompt_embeds
 
@@ -205,14 +269,15 @@
         device,
         num_images_per_prompt,
         do_classifier_free_guidance,
         negative_prompt=None,
         prompt_embeds: Optional[torch.FloatTensor] = None,
         negative_prompt_embeds: Optional[torch.FloatTensor] = None,
         lora_scale: Optional[float] = None,
+        clip_skip: Optional[int] = None,
     ):
         r"""
         Encodes the prompt into text encoder hidden states.
 
         Args:
             prompt (`str` or `List[str]`, *optional*):
                 prompt to be encoded
@@ -230,23 +295,29 @@
                 Pre-generated text embeddings. Can be used to easily tweak text inputs, *e.g.* prompt weighting. If not
                 provided, text embeddings will be generated from `prompt` input argument.
             negative_prompt_embeds (`torch.FloatTensor`, *optional*):
                 Pre-generated negative text embeddings. Can be used to easily tweak text inputs, *e.g.* prompt
                 weighting. If not provided, negative_prompt_embeds will be generated from `negative_prompt` input
                 argument.
             lora_scale (`float`, *optional*):
-                A lora scale that will be applied to all LoRA layers of the text encoder if LoRA layers are loaded.
+                A LoRA scale that will be applied to all LoRA layers of the text encoder if LoRA layers are loaded.
+            clip_skip (`int`, *optional*):
+                Number of layers to be skipped from CLIP while computing the prompt embeddings. A value of 1 means that
+                the output of the pre-final layer will be used for computing the prompt embeddings.
         """
         # set lora scale so that monkey patched LoRA
         # function of text encoder can correctly access it
         if lora_scale is not None and isinstance(self, LoraLoaderMixin):
             self._lora_scale = lora_scale
 
             # dynamically adjust the LoRA scale
-            adjust_lora_scale_text_encoder(self.text_encoder, lora_scale)
+            if not USE_PEFT_BACKEND:
+                adjust_lora_scale_text_encoder(self.text_encoder, lora_scale)
+            else:
+                scale_lora_layers(self.text_encoder, lora_scale)
 
         if prompt is not None and isinstance(prompt, str):
             num_prompts = 1
         elif prompt is not None and isinstance(prompt, list):
             num_prompts = len(prompt)
         else:
             num_prompts = prompt_embeds.shape[0]
@@ -278,19 +349,30 @@
                 )
 
             if hasattr(self.text_encoder.config, "use_attention_mask") and self.text_encoder.config.use_attention_mask:
                 attention_mask = text_inputs.attention_mask.to(device)
             else:
                 attention_mask = None
 
-            prompt_embeds = self.text_encoder(
-                text_input_ids.to(device),
-                attention_mask=attention_mask,
-            )
-            prompt_embeds = prompt_embeds[0]
+            if clip_skip is None:
+                prompt_embeds = self.text_encoder(text_input_ids.to(device), attention_mask=attention_mask)
+                prompt_embeds = prompt_embeds[0]
+            else:
+                prompt_embeds = self.text_encoder(
+                    text_input_ids.to(device), attention_mask=attention_mask, output_hidden_states=True
+                )
+                # Access the `hidden_states` first, that contains a tuple of
+                # all the hidden states from the encoder layers. Then index into
+                # the tuple to access the hidden states from the desired layer.
+                prompt_embeds = prompt_embeds[-1][-(clip_skip + 1)]
+                # We also need to apply the final LayerNorm here to not mess with the
+                # representations. The `last_hidden_states` that we typically use for
+                # obtaining the final prompt representations passes through the LayerNorm
+                # layer.
+                prompt_embeds = self.text_encoder.text_model.final_layer_norm(prompt_embeds)
 
         if self.text_encoder is not None:
             prompt_embeds_dtype = self.text_encoder.dtype
         elif self.unet is not None:
             prompt_embeds_dtype = self.unet.dtype
         else:
             prompt_embeds_dtype = prompt_embeds.dtype
@@ -352,37 +434,38 @@
             seq_len = negative_prompt_embeds.shape[1]
 
             negative_prompt_embeds = negative_prompt_embeds.to(dtype=prompt_embeds_dtype, device=device)
 
             negative_prompt_embeds = negative_prompt_embeds.repeat(1, num_images_per_prompt, 1)
             negative_prompt_embeds = negative_prompt_embeds.view(num_prompts * num_images_per_prompt, seq_len, -1)
 
+        if isinstance(self, LoraLoaderMixin) and USE_PEFT_BACKEND:
+            # Retrieve the original scale by scaling back the LoRA layers
+            unscale_lora_layers(self.text_encoder, lora_scale)
+
         return prompt_embeds, negative_prompt_embeds
 
     def run_safety_checker(self, image, device, dtype):
         if self.safety_checker is None:
             has_nsfw_concept = None
         else:
             if torch.is_tensor(image):
                 feature_extractor_input = self.image_processor.postprocess(image, output_type="pil")
             else:
                 feature_extractor_input = self.image_processor.numpy_to_pil(image)
-            rgb_feature_extractor_input = feature_extractor_input[0]
-            safety_checker_input = self.feature_extractor(rgb_feature_extractor_input, return_tensors="pt").to(device)
+            safety_checker_input = self.feature_extractor(feature_extractor_input, return_tensors="pt").to(device)
             image, has_nsfw_concept = self.safety_checker(
                 images=image, clip_input=safety_checker_input.pixel_values.to(dtype)
             )
         return image, has_nsfw_concept
 
     def decode_latents(self, latents):
-        warnings.warn(
-            "The decode_latents method is deprecated and will be removed in a future version. Please"
-            " use VaeImageProcessor instead",
-            FutureWarning,
-        )
+        deprecation_message = "The decode_latents method is deprecated and will be removed in 1.0.0. Please use VaeImageProcessor.postprocess(...) instead"
+        deprecate("decode_latents", "1.0.0", deprecation_message, standard_warn=False)
+
         latents = 1 / self.vae.config.scaling_factor * latents
         image = self.vae.decode(latents, return_dict=False)[0]
         image = (image / 2 + 0.5).clamp(0, 1)
         # we always cast to float32 as this does not cause significant overhead and is compatible with bfloat16
         image = image.cpu().permute(0, 2, 3, 1).float().numpy()
         return image
 
@@ -408,25 +491,30 @@
         prompt,
         height,
         width,
         callback_steps,
         negative_prompt=None,
         prompt_embeds=None,
         negative_prompt_embeds=None,
+        callback_on_step_end_tensor_inputs=None,
     ):
         if height % 8 != 0 or width % 8 != 0:
             raise ValueError(f"`height` and `width` have to be divisible by 8 but are {height} and {width}.")
 
-        if (callback_steps is None) or (
-            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
-        ):
+        if callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0):
             raise ValueError(
                 f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
                 f" {type(callback_steps)}."
             )
+        if callback_on_step_end_tensor_inputs is not None and not all(
+            k in self._callback_tensor_inputs for k in callback_on_step_end_tensor_inputs
+        ):
+            raise ValueError(
+                f"`callback_on_step_end_tensor_inputs` has to be in {self._callback_tensor_inputs}, but found {[k for k in callback_on_step_end_tensor_inputs if k not in self._callback_tensor_inputs]}"
+            )
 
         if prompt is not None and prompt_embeds is not None:
             raise ValueError(
                 f"Cannot forward both `prompt`: {prompt} and `prompt_embeds`: {prompt_embeds}. Please make sure to"
                 " only forward one of the two."
             )
         elif prompt is None and prompt_embeds is None:
@@ -475,87 +563,188 @@
                 raise ValueError(f"Unexpected latents shape, got {latents.shape}, expected {shape}")
             latents = latents.to(device)
 
         # scale the initial noise by the standard deviation required by the scheduler
         latents = latents * self.scheduler.init_noise_sigma
         return latents
 
+    def enable_freeu(self, s1: float, s2: float, b1: float, b2: float):
+        r"""Enables the FreeU mechanism as in https://arxiv.org/abs/2309.11497.
+
+        The suffixes after the scaling factors represent the stages where they are being applied.
+
+        Please refer to the [official repository](https://github.com/ChenyangSi/FreeU) for combinations of the values
+        that are known to work well for different pipelines such as Stable Diffusion v1, v2, and Stable Diffusion XL.
+
+        Args:
+            s1 (`float`):
+                Scaling factor for stage 1 to attenuate the contributions of the skip features. This is done to
+                mitigate "oversmoothing effect" in the enhanced denoising process.
+            s2 (`float`):
+                Scaling factor for stage 2 to attenuate the contributions of the skip features. This is done to
+                mitigate "oversmoothing effect" in the enhanced denoising process.
+            b1 (`float`): Scaling factor for stage 1 to amplify the contributions of backbone features.
+            b2 (`float`): Scaling factor for stage 2 to amplify the contributions of backbone features.
+        """
+        if not hasattr(self, "unet"):
+            raise ValueError("The pipeline must have `unet` for using FreeU.")
+        self.unet.enable_freeu(s1=s1, s2=s2, b1=b1, b2=b2)
+
+    def disable_freeu(self):
+        """Disables the FreeU mechanism if enabled."""
+        self.unet.disable_freeu()
+
+    def get_guidance_scale_embedding(self, w, embedding_dim=512, dtype=torch.float32):
+        """
+        See https://github.com/google-research/vdm/blob/dc27b98a554f65cdc654b800da5aa1846545d41b/model_vdm.py#L298
+
+        Args:
+            timesteps (`torch.Tensor`):
+                generate embedding vectors at these timesteps
+            embedding_dim (`int`, *optional*, defaults to 512):
+                dimension of the embeddings to generate
+            dtype:
+                data type of the generated embeddings
+
+        Returns:
+            `torch.FloatTensor`: Embedding vectors with shape `(len(timesteps), embedding_dim)`
+        """
+        assert len(w.shape) == 1
+        w = w * 1000.0
+
+        half_dim = embedding_dim // 2
+        emb = torch.log(torch.tensor(10000.0)) / (half_dim - 1)
+        emb = torch.exp(torch.arange(half_dim, dtype=dtype) * -emb)
+        emb = w.to(dtype)[:, None] * emb[None, :]
+        emb = torch.cat([torch.sin(emb), torch.cos(emb)], dim=1)
+        if embedding_dim % 2 == 1:  # zero pad
+            emb = torch.nn.functional.pad(emb, (0, 1))
+        assert emb.shape == (w.shape[0], embedding_dim)
+        return emb
+
+    @property
+    def guidance_scale(self):
+        return self._guidance_scale
+
+    @property
+    def guidance_rescale(self):
+        return self._guidance_rescale
+
+    @property
+    def clip_skip(self):
+        return self._clip_skip
+
+    # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
+    # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
+    # corresponds to doing no classifier free guidance.
+    @property
+    def do_classifier_free_guidance(self):
+        return self._guidance_scale > 1 and self.unet.config.time_cond_proj_dim is None
+
+    @property
+    def cross_attention_kwargs(self):
+        return self._cross_attention_kwargs
+
+    @property
+    def num_timesteps(self):
+        return self._num_timesteps
+
     @classmethod
-    def _split_inputs_into_batches(cls, batch_size, latents, text_embeddings):
+    def _split_inputs_into_batches(cls, batch_size, latents, prompt_embeds, negative_prompt_embeds):
         # Use torch.split to generate num_batches batches of size batch_size
         latents_batches = list(torch.split(latents, batch_size))
-        # If there are uncond embeddings, the batch size of text embeddings is 2x
-        multiple = text_embeddings.shape[0] // latents.shape[0]
-        text_embeddings_batches = list(torch.split(text_embeddings, multiple * batch_size))
+        prompt_embeds_batches = list(torch.split(prompt_embeds, batch_size))
+        if negative_prompt_embeds is not None:
+            negative_prompt_embeds_batches = list(torch.split(negative_prompt_embeds, batch_size))
 
         # If the last batch has less samples than batch_size, pad it with dummy samples
         num_dummy_samples = 0
         if latents_batches[-1].shape[0] < batch_size:
             num_dummy_samples = batch_size - latents_batches[-1].shape[0]
             # Pad latents_batches
             sequence_to_stack = (latents_batches[-1],) + tuple(
                 torch.zeros_like(latents_batches[-1][0][None, :]) for _ in range(num_dummy_samples)
             )
             latents_batches[-1] = torch.vstack(sequence_to_stack)
-            # Pad text_embeddings_batches
-            sequence_to_stack = (text_embeddings_batches[-1],) + tuple(
-                torch.zeros_like(text_embeddings_batches[-1][0][None, :]) for _ in range(multiple * num_dummy_samples)
-            )
-            text_embeddings_batches[-1] = torch.vstack(sequence_to_stack)
+            # Pad prompt_embeds_batches
+            sequence_to_stack = (prompt_embeds_batches[-1],) + tuple(
+                torch.zeros_like(prompt_embeds_batches[-1][0][None, :]) for _ in range(num_dummy_samples)
+            )
+            prompt_embeds_batches[-1] = torch.vstack(sequence_to_stack)
+            # Pad negative_prompt_embeds_batches if necessary
+            if negative_prompt_embeds is not None:
+                sequence_to_stack = (negative_prompt_embeds_batches[-1],) + tuple(
+                    torch.zeros_like(negative_prompt_embeds_batches[-1][0][None, :]) for _ in range(num_dummy_samples)
+                )
+                negative_prompt_embeds_batches[-1] = torch.vstack(sequence_to_stack)
 
         # Stack batches in the same tensor
         latents_batches = torch.stack(latents_batches)
-        text_embeddings_batches = torch.stack(text_embeddings_batches)
+        if negative_prompt_embeds is not None:
+            # For classifier free guidance, we need to do two forward passes.
+            # Here we concatenate the unconditional and text embeddings into a single batch
+            # to avoid doing two forward passes
+            for i, (negative_prompt_embeds_batch, prompt_embeds_batch) in enumerate(
+                zip(negative_prompt_embeds_batches, prompt_embeds_batches[:])
+            ):
+                prompt_embeds_batches[i] = torch.cat([negative_prompt_embeds_batch, prompt_embeds_batch])
+        prompt_embeds_batches = torch.stack(prompt_embeds_batches)
 
-        return latents_batches, text_embeddings_batches, num_dummy_samples
+        return latents_batches, prompt_embeds_batches, num_dummy_samples
 
     @torch.no_grad()
     def __call__(
         self,
         prompt: Union[str, List[str]] = None,
         height: Optional[int] = None,
         width: Optional[int] = None,
         num_inference_steps: int = 50,
-        guidance_scale: float = 5.0,
+        guidance_scale: float = 7.5,
         negative_prompt: Optional[Union[str, List[str]]] = None,
         num_images_per_prompt: Optional[int] = 1,
         batch_size: int = 1,
         eta: float = 0.0,
         generator: Optional[Union[torch.Generator, List[torch.Generator]]] = None,
         latents: Optional[torch.FloatTensor] = None,
         prompt_embeds: Optional[torch.FloatTensor] = None,
         negative_prompt_embeds: Optional[torch.FloatTensor] = None,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
         callback: Optional[Callable[[int, int, torch.FloatTensor], None]] = None,
         callback_steps: int = 1,
         cross_attention_kwargs: Optional[Dict[str, Any]] = None,
         guidance_rescale: float = 0.0,
+        clip_skip: Optional[int] = None,
+        callback_on_step_end: Optional[Callable[[int, int, Dict], None]] = None,
+        callback_on_step_end_tensor_inputs: List[str] = ["latents"],
+        **kwargs,
     ):
         r"""
         The call function to the pipeline for generation.
 
         Args:
             prompt (`str` or `List[str]`, *optional*):
                 The prompt or prompts to guide image generation. If not defined, you need to pass `prompt_embeds`.
             height (`int`, *optional*, defaults to `self.unet.config.sample_size * self.vae_scale_factor`):
-                The height in pixels of the generated image.
+                The height in pixels of the generated images.
             width (`int`, *optional*, defaults to `self.unet.config.sample_size * self.vae_scale_factor`):
-                The width in pixels of the generated image.
+                The width in pixels of the generated images.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
-            guidance_scale (`float`, *optional*, defaults to 5.0):
+            guidance_scale (`float`, *optional*, defaults to 7.5):
                 A higher guidance scale value encourages the model to generate images closely linked to the text
                 `prompt` at the expense of lower image quality. Guidance scale is enabled when `guidance_scale > 1`.
             negative_prompt (`str` or `List[str]`, *optional*):
                 The prompt or prompts to guide what to not include in image generation. If not defined, you need to
                 pass `negative_prompt_embeds` instead. Ignored when not using guidance (`guidance_scale < 1`).
             num_images_per_prompt (`int`, *optional*, defaults to 1):
                 The number of images to generate per prompt.
+            batch_size (`int`, *optional*, defaults to 1):
+                The number of images in a batch.
             eta (`float`, *optional*, defaults to 0.0):
                 Corresponds to parameter eta (η) from the [DDIM](https://arxiv.org/abs/2010.02502) paper. Only applies
                 to the [`~schedulers.DDIMScheduler`], and is ignored in other schedulers.
             generator (`torch.Generator` or `List[torch.Generator]`, *optional*):
                 A [`torch.Generator`](https://pytorch.org/docs/stable/generated/torch.Generator.html) to make
                 generation deterministic.
             latents (`torch.FloatTensor`, *optional*):
@@ -567,43 +756,82 @@
                 provided, text embeddings are generated from the `prompt` input argument.
             negative_prompt_embeds (`torch.FloatTensor`, *optional*):
                 Pre-generated negative text embeddings. Can be used to easily tweak text inputs (prompt weighting). If
                 not provided, `negative_prompt_embeds` are generated from the `negative_prompt` input argument.
             output_type (`str`, *optional*, defaults to `"pil"`):
                 The output format of the generated image. Choose between `PIL.Image` or `np.array`.
             return_dict (`bool`, *optional*, defaults to `True`):
-                Whether or not to return a [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] instead of a
+                Whether or not to return a [`~diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.GaudiStableDiffusionPipelineOutput`] instead of a
                 plain tuple.
-            callback (`Callable`, *optional*):
-                A function that calls every `callback_steps` steps during inference. The function is called with the
-                following arguments: `callback(step: int, timestep: int, latents: torch.FloatTensor)`.
-            callback_steps (`int`, *optional*, defaults to 1):
-                The frequency at which the `callback` function is called. If not specified, the callback is called at
-                every step.
             cross_attention_kwargs (`dict`, *optional*):
                 A kwargs dictionary that if specified is passed along to the [`AttentionProcessor`] as defined in
                 [`self.processor`](https://github.com/huggingface/diffusers/blob/main/src/diffusers/models/attention_processor.py).
+            guidance_rescale (`float`, *optional*, defaults to 0.0):
+                Guidance rescale factor from [Common Diffusion Noise Schedules and Sample Steps are
+                Flawed](https://arxiv.org/pdf/2305.08891.pdf). Guidance rescale factor should fix overexposure when
+                using zero terminal SNR.
+            clip_skip (`int`, *optional*):
+                Number of layers to be skipped from CLIP while computing the prompt embeddings. A value of 1 means that
+                the output of the pre-final layer will be used for computing the prompt embeddings.
+            callback_on_step_end (`Callable`, *optional*):
+                A function that calls at the end of each denoising steps during the inference. The function is called
+                with the following arguments: `callback_on_step_end(self: DiffusionPipeline, step: int, timestep: int,
+                callback_kwargs: Dict)`. `callback_kwargs` will include a list of all tensors as specified by
+                `callback_on_step_end_tensor_inputs`.
+            callback_on_step_end_tensor_inputs (`List`, *optional*):
+                The list of tensor inputs for the `callback_on_step_end` function. The tensors specified in the list
+                will be passed as `callback_kwargs` argument. You will only be able to include variables listed in the
+                `._callback_tensor_inputs` attribute of your pipeine class.
 
         Returns:
             [`~diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.GaudiStableDiffusionPipelineOutput`] or `tuple`:
-                If `return_dict` is `True`, [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] is returned,
+                If `return_dict` is `True`, [`~diffusers.pipelines.stable_diffusion.StableDiffusionPipelineOutput`] is returned,
                 otherwise a `tuple` is returned where the first element is a list with the generated images and the
                 second element is a list of `bool`s indicating whether the corresponding generated image contains
                 "not-safe-for-work" (nsfw) content.
         """
+        callback = kwargs.pop("callback", None)
+        callback_steps = kwargs.pop("callback_steps", None)
+
+        if callback is not None:
+            deprecate(
+                "callback",
+                "1.0.0",
+                "Passing `callback` as an input argument to `__call__` is deprecated, consider using `callback_on_step_end`",
+            )
+        if callback_steps is not None:
+            deprecate(
+                "callback_steps",
+                "1.0.0",
+                "Passing `callback_steps` as an input argument to `__call__` is deprecated, consider using `callback_on_step_end`",
+            )
+
         with torch.autocast(device_type="hpu", dtype=torch.bfloat16, enabled=self.gaudi_config.use_torch_autocast):
             # 0. Default height and width to unet
             height = height or self.unet.config.sample_size * self.vae_scale_factor
             width = width or self.unet.config.sample_size * self.vae_scale_factor
+            # to deal with lora scaling and other possible forward hooks
 
             # 1. Check inputs. Raise error if not correct
             self.check_inputs(
-                prompt, height, width, callback_steps, negative_prompt, prompt_embeds, negative_prompt_embeds
+                prompt,
+                height,
+                width,
+                callback_steps,
+                negative_prompt,
+                prompt_embeds,
+                negative_prompt_embeds,
+                callback_on_step_end_tensor_inputs,
             )
 
+            self._guidance_scale = guidance_scale
+            self._guidance_rescale = guidance_rescale
+            self._clip_skip = clip_skip
+            self._cross_attention_kwargs = cross_attention_kwargs
+
             # 2. Define call parameters
             if prompt is not None and isinstance(prompt, str):
                 num_prompts = 1
             elif prompt is not None and isinstance(prompt, list):
                 num_prompts = len(prompt)
             else:
                 num_prompts = prompt_embeds.shape[0]
@@ -611,34 +839,31 @@
             logger.info(
                 f"{num_prompts} prompt(s) received, {num_images_per_prompt} generation(s) per prompt,"
                 f" {batch_size} sample(s) per batch, {num_batches} total batch(es)."
             )
             if num_batches < 3:
                 logger.warning("The first two iterations are slower so it is recommended to feed more batches.")
             device = self._execution_device
-            # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
-            # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
-            # corresponds to doing no classifier free guidance.
-            do_classifier_free_guidance = guidance_scale > 1.0
 
             # 3. Encode input prompt
+            lora_scale = (
+                self.cross_attention_kwargs.get("scale", None) if self.cross_attention_kwargs is not None else None
+            )
+
             prompt_embeds, negative_prompt_embeds = self.encode_prompt(
                 prompt,
                 device,
                 num_images_per_prompt,
-                do_classifier_free_guidance,
+                self.do_classifier_free_guidance,
                 negative_prompt,
                 prompt_embeds=prompt_embeds,
                 negative_prompt_embeds=negative_prompt_embeds,
+                lora_scale=lora_scale,
+                clip_skip=self.clip_skip,
             )
-            # For classifier free guidance, we need to do two forward passes.
-            # Here we concatenate the unconditional and text embeddings into a single batch
-            # to avoid doing two forward passes
-            if do_classifier_free_guidance:
-                prompt_embeds = torch.cat([negative_prompt_embeds, prompt_embeds])
 
             # 4. Prepare timesteps
             self.scheduler.set_timesteps(num_inference_steps, device="cpu")
             timesteps = self.scheduler.timesteps.to(device)
 
             # 5. Prepare latent variables
             num_channels_latents = self.unet.config.in_channels
@@ -652,28 +877,41 @@
                 generator,
                 latents,
             )
 
             # 6. Prepare extra step kwargs. TODO: Logic should ideally just be moved out of the pipeline
             extra_step_kwargs = self.prepare_extra_step_kwargs(generator, eta)
 
+            # 6.5 Optionally get Guidance Scale Embedding
+            timestep_cond = None
+            if self.unet.config.time_cond_proj_dim is not None:
+                guidance_scale_tensor = torch.tensor(self.guidance_scale - 1).repeat(
+                    batch_size * num_images_per_prompt
+                )
+                timestep_cond = self.get_guidance_scale_embedding(
+                    guidance_scale_tensor, embedding_dim=self.unet.config.time_cond_proj_dim
+                ).to(device=device, dtype=latents.dtype)
+
             # 7. Split into batches (HPU-specific step)
             latents_batches, text_embeddings_batches, num_dummy_samples = self._split_inputs_into_batches(
                 batch_size,
                 latents,
                 prompt_embeds,
+                negative_prompt_embeds,
             )
 
             outputs = {
                 "images": [],
                 "has_nsfw_concept": [],
             }
             t0 = time.time()
             t1 = t0
 
+            self._num_timesteps = len(timesteps)
+
             # 8. Denoising loop
             for j in self.progress_bar(range(num_batches)):
                 # The throughput is calculated from the 3rd iteration
                 # because compilation occurs in the first two iterations
                 if j == 2:
                     t1 = time.time()
 
@@ -686,47 +924,67 @@
                     timestep = timesteps[0]
                     timesteps = torch.roll(timesteps, shifts=-1, dims=0)
 
                     capture = True if self.use_hpu_graphs and i < 2 else False
 
                     # expand the latents if we are doing classifier free guidance
                     latent_model_input = (
-                        torch.cat([latents_batch] * 2) if do_classifier_free_guidance else latents_batch
+                        torch.cat([latents_batch] * 2) if self.do_classifier_free_guidance else latents_batch
                     )
-                    # latent_model_input = self.scheduler.scale_model_input(latent_model_input, timestep)
+                    latent_model_input = self.scheduler.scale_model_input(latent_model_input, timestep)
 
                     # predict the noise residual
                     noise_pred = self.unet_hpu(
                         latent_model_input,
                         timestep,
                         text_embeddings_batch,
-                        cross_attention_kwargs,
+                        timestep_cond,
+                        self.cross_attention_kwargs,
                         capture,
                     )
 
                     # perform guidance
-                    if do_classifier_free_guidance:
+                    if self.do_classifier_free_guidance:
                         noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
-                        noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
+                        noise_pred = noise_pred_uncond + self.guidance_scale * (noise_pred_text - noise_pred_uncond)
+
+                    if self.do_classifier_free_guidance and self.guidance_rescale > 0.0:
+                        # Based on 3.4. in https://arxiv.org/pdf/2305.08891.pdf
+                        noise_pred = rescale_noise_cfg(
+                            noise_pred, noise_pred_text, guidance_rescale=self.guidance_rescale
+                        )
 
                     # compute the previous noisy sample x_t -> x_t-1
                     latents_batch = self.scheduler.step(
                         noise_pred, latents_batch, **extra_step_kwargs, return_dict=False
                     )[0]
 
                     if not self.use_hpu_graphs:
                         self.htcore.mark_step()
 
+                    if callback_on_step_end is not None:
+                        callback_kwargs = {}
+                        for k in callback_on_step_end_tensor_inputs:
+                            callback_kwargs[k] = locals()[k]
+                        callback_outputs = callback_on_step_end(self, i, timestep, callback_kwargs)
+
+                        latents_batch = callback_outputs.pop("latents", latents_batch)
+                        text_embeddings_batch = callback_outputs.pop("prompt_embeds", text_embeddings_batch)
+                        # negative_prompt_embeds = callback_outputs.pop("negative_prompt_embeds", negative_prompt_embeds)
+
                     # call the callback, if provided
                     if callback is not None and i % callback_steps == 0:
-                        callback(i, timestep, latents_batch)
+                        step_idx = i // getattr(self.scheduler, "order", 1)
+                        callback(step_idx, timestep, latents_batch)
 
                 if not output_type == "latent":
                     # 8. Post-processing
-                    image = self.vae.decode(latents_batch / self.vae.config.scaling_factor, return_dict=False)[0]
+                    image = self.vae.decode(
+                        latents_batch / self.vae.config.scaling_factor, return_dict=False, generator=generator
+                    )[0]
                 else:
                     image = latents_batch
                 outputs["images"].append(image)
 
                 self.scheduler.reset_timestep_dependent_params()
 
                 if not self.use_hpu_graphs:
@@ -757,17 +1015,15 @@
                     image, has_nsfw_concept = self.run_safety_checker(image, device, prompt_embeds.dtype)
 
                 if has_nsfw_concept is None:
                     do_denormalize = [True] * image.shape[0]
                 else:
                     do_denormalize = [not has_nsfw for has_nsfw in has_nsfw_concept]
 
-                rgb, depth = self.image_processor.postprocess(
-                    image, output_type=output_type, do_denormalize=do_denormalize
-                )
+                image = self.image_processor.postprocess(image, output_type=output_type, do_denormalize=do_denormalize)
 
                 if output_type == "pil":
                     outputs["images"] += image
                 else:
                     outputs["images"] += [*image]
 
                 if has_nsfw_concept is not None:
@@ -775,32 +1031,34 @@
                 else:
                     outputs["has_nsfw_concept"] = None
 
             # Offload all models
             self.maybe_free_model_hooks()
 
             if not return_dict:
-                return ((rgb, depth), has_nsfw_concept)
+                return (outputs["images"], outputs["has_nsfw_concept"])
 
-            return GaudiStableDiffusionLDM3DPipelineOutput(
-                rgb=rgb,
-                depth=depth,
-                nsfw_content_detected=has_nsfw_concept,
+            return GaudiStableDiffusionPipelineOutput(
+                images=outputs["images"],
+                nsfw_content_detected=outputs["has_nsfw_concept"],
                 throughput=speed_measures[f"{speed_metrics_prefix}_samples_per_second"],
             )
 
     @torch.no_grad()
-    def unet_hpu(self, latent_model_input, timestep, encoder_hidden_states, cross_attention_kwargs, capture):
+    def unet_hpu(
+        self, latent_model_input, timestep, encoder_hidden_states, timestep_cond, cross_attention_kwargs, capture
+    ):
         if self.use_hpu_graphs:
             return self.capture_replay(latent_model_input, timestep, encoder_hidden_states, capture)
         else:
             return self.unet(
                 latent_model_input,
                 timestep,
                 encoder_hidden_states=encoder_hidden_states,
+                timestep_cond=timestep_cond,
                 cross_attention_kwargs=cross_attention_kwargs,
                 return_dict=False,
             )[0]
 
     @torch.no_grad()
     def capture_replay(self, latent_model_input, timestep, encoder_hidden_states, capture):
         inputs = [latent_model_input, timestep, encoder_hidden_states, False]
```

### Comparing `optimum-habana-1.8.2/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_upscale.py` & `optimum-habana-1.9.0/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_upscale.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,26 +20,25 @@
 from math import ceil
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import numpy as np
 import PIL
 import torch
 from diffusers.image_processor import VaeImageProcessor
-from diffusers.loaders import LoraLoaderMixin, TextualInversionLoaderMixin
+from diffusers.loaders import FromSingleFileMixin, LoraLoaderMixin, TextualInversionLoaderMixin
 from diffusers.models import AutoencoderKL, UNet2DConditionModel
 from diffusers.models.attention_processor import (
     AttnProcessor2_0,
     LoRAAttnProcessor2_0,
     LoRAXFormersAttnProcessor,
     XFormersAttnProcessor,
 )
-
-# Added for upscaling
+from diffusers.models.lora import adjust_lora_scale_text_encoder
 from diffusers.schedulers import DDPMScheduler, KarrasDiffusionSchedulers
-from diffusers.utils import BaseOutput, deprecate
+from diffusers.utils import USE_PEFT_BACKEND, BaseOutput, deprecate, scale_lora_layers, unscale_lora_layers
 from diffusers.utils.torch_utils import randn_tensor
 from transformers import CLIPImageProcessor, CLIPTextModel, CLIPTokenizer
 
 from optimum.utils import logging
 
 from ....transformers.gaudi_configuration import GaudiConfig
 from ....utils import speed_metrics
@@ -85,15 +84,17 @@
         image = 2.0 * image - 1.0
         image = torch.from_numpy(image)
     elif isinstance(image[0], torch.Tensor):
         image = torch.cat(image, dim=0)
     return image
 
 
-class GaudiStableDiffusionUpscalePipeline(GaudiDiffusionPipeline, TextualInversionLoaderMixin, LoraLoaderMixin):
+class GaudiStableDiffusionUpscalePipeline(
+    GaudiDiffusionPipeline, TextualInversionLoaderMixin, LoraLoaderMixin, FromSingleFileMixin
+):
     """
     Pipeline for text-guided image super-resolution using Stable Diffusion 2.
 
     Extends the [`StableDiffusionUpscalePipeline`](https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion#diffusers.StableDiffusionUpscalePipeline) class:
     - Generation is performed by batches
     - Two `mark_step()` were added to add support for lazy mode
     - Added support for HPU graphs
@@ -216,14 +217,47 @@
         device,
         num_images_per_prompt,
         do_classifier_free_guidance,
         negative_prompt=None,
         prompt_embeds: Optional[torch.FloatTensor] = None,
         negative_prompt_embeds: Optional[torch.FloatTensor] = None,
         lora_scale: Optional[float] = None,
+        **kwargs,
+    ):
+        deprecation_message = "`_encode_prompt()` is deprecated and it will be removed in a future version. Use `encode_prompt()` instead. Also, be aware that the output format changed from a concatenated tensor to a tuple."
+        deprecate("_encode_prompt()", "1.0.0", deprecation_message, standard_warn=False)
+
+        prompt_embeds_tuple = self.encode_prompt(
+            prompt=prompt,
+            device=device,
+            num_images_per_prompt=num_images_per_prompt,
+            do_classifier_free_guidance=do_classifier_free_guidance,
+            negative_prompt=negative_prompt,
+            prompt_embeds=prompt_embeds,
+            negative_prompt_embeds=negative_prompt_embeds,
+            lora_scale=lora_scale,
+            **kwargs,
+        )
+
+        # concatenate for backwards comp
+        prompt_embeds = torch.cat([prompt_embeds_tuple[1], prompt_embeds_tuple[0]])
+
+        return prompt_embeds
+
+    def encode_prompt(
+        self,
+        prompt,
+        device,
+        num_images_per_prompt,
+        do_classifier_free_guidance,
+        negative_prompt=None,
+        prompt_embeds: Optional[torch.FloatTensor] = None,
+        negative_prompt_embeds: Optional[torch.FloatTensor] = None,
+        lora_scale: Optional[float] = None,
+        clip_skip: Optional[int] = None,
     ):
         r"""
         Encodes the prompt into text encoder hidden states.
 
         Args:
             prompt (`str` or `List[str]`, *optional*):
                 prompt to be encoded
@@ -241,21 +275,29 @@
                 Pre-generated text embeddings. Can be used to easily tweak text inputs, *e.g.* prompt weighting. If not
                 provided, text embeddings will be generated from `prompt` input argument.
             negative_prompt_embeds (`torch.FloatTensor`, *optional*):
                 Pre-generated negative text embeddings. Can be used to easily tweak text inputs, *e.g.* prompt
                 weighting. If not provided, negative_prompt_embeds will be generated from `negative_prompt` input
                 argument.
             lora_scale (`float`, *optional*):
-                A lora scale that will be applied to all LoRA layers of the text encoder if LoRA layers are loaded.
+                A LoRA scale that will be applied to all LoRA layers of the text encoder if LoRA layers are loaded.
+            clip_skip (`int`, *optional*):
+                Number of layers to be skipped from CLIP while computing the prompt embeddings. A value of 1 means that
+                the output of the pre-final layer will be used for computing the prompt embeddings.
         """
         # set lora scale so that monkey patched LoRA
         # function of text encoder can correctly access it
         if lora_scale is not None and isinstance(self, LoraLoaderMixin):
             self._lora_scale = lora_scale
-            # adjust_lora_scale_text_encoder(self.text_encoder, lora_scale) #TODO why this has been removed?
+
+            # dynamically adjust the LoRA scale
+            if not USE_PEFT_BACKEND:
+                adjust_lora_scale_text_encoder(self.text_encoder, lora_scale)
+            else:
+                scale_lora_layers(self.text_encoder, lora_scale)
 
         if prompt is not None and isinstance(prompt, str):
             num_prompts = 1
         elif prompt is not None and isinstance(prompt, list):
             num_prompts = len(prompt)
         else:
             num_prompts = prompt_embeds.shape[0]
@@ -287,18 +329,39 @@
                 )
 
             if hasattr(self.text_encoder.config, "use_attention_mask") and self.text_encoder.config.use_attention_mask:
                 attention_mask = text_inputs.attention_mask.to(device)
             else:
                 attention_mask = None
 
-            prompt_embeds = self.text_encoder(text_input_ids.to(device), attention_mask=attention_mask)
-            prompt_embeds = prompt_embeds[0]
+            if clip_skip is None:
+                prompt_embeds = self.text_encoder(text_input_ids.to(device), attention_mask=attention_mask)
+                prompt_embeds = prompt_embeds[0]
+            else:
+                prompt_embeds = self.text_encoder(
+                    text_input_ids.to(device), attention_mask=attention_mask, output_hidden_states=True
+                )
+                # Access the `hidden_states` first, that contains a tuple of
+                # all the hidden states from the encoder layers. Then index into
+                # the tuple to access the hidden states from the desired layer.
+                prompt_embeds = prompt_embeds[-1][-(clip_skip + 1)]
+                # We also need to apply the final LayerNorm here to not mess with the
+                # representations. The `last_hidden_states` that we typically use for
+                # obtaining the final prompt representations passes through the LayerNorm
+                # layer.
+                prompt_embeds = self.text_encoder.text_model.final_layer_norm(prompt_embeds)
+
+        if self.text_encoder is not None:
+            prompt_embeds_dtype = self.text_encoder.dtype
+        elif self.unet is not None:
+            prompt_embeds_dtype = self.unet.dtype
+        else:
+            prompt_embeds_dtype = prompt_embeds.dtype
 
-        prompt_embeds = prompt_embeds.to(dtype=self.text_encoder.dtype, device=device)
+        prompt_embeds = prompt_embeds.to(dtype=prompt_embeds_dtype, device=device)
 
         bs_embed, seq_len, _ = prompt_embeds.shape
         # duplicate text embeddings for each generation per prompt, using mps friendly method
         prompt_embeds = prompt_embeds.repeat(1, num_images_per_prompt, 1)
         prompt_embeds = prompt_embeds.view(bs_embed * num_images_per_prompt, seq_len, -1)
 
         # get unconditional embeddings for classifier free guidance
@@ -324,36 +387,45 @@
 
             # textual inversion: procecss multi-vector tokens if necessary
             if isinstance(self, TextualInversionLoaderMixin):
                 uncond_tokens = self.maybe_convert_prompt(uncond_tokens, self.tokenizer)
 
             max_length = prompt_embeds.shape[1]
             uncond_input = self.tokenizer(
-                uncond_tokens, padding="max_length", max_length=max_length, truncation=True, return_tensors="pt"
+                uncond_tokens,
+                padding="max_length",
+                max_length=max_length,
+                truncation=True,
+                return_tensors="pt",
             )
 
             if hasattr(self.text_encoder.config, "use_attention_mask") and self.text_encoder.config.use_attention_mask:
                 attention_mask = uncond_input.attention_mask.to(device)
             else:
                 attention_mask = None
 
             negative_prompt_embeds = self.text_encoder(
-                uncond_input.input_ids.to(device), attention_mask=attention_mask
+                uncond_input.input_ids.to(device),
+                attention_mask=attention_mask,
             )
             negative_prompt_embeds = negative_prompt_embeds[0]
 
         if do_classifier_free_guidance:
             # duplicate unconditional embeddings for each generation per prompt, using mps friendly method
             seq_len = negative_prompt_embeds.shape[1]
 
-            negative_prompt_embeds = negative_prompt_embeds.to(dtype=self.text_encoder.dtype, device=device)
+            negative_prompt_embeds = negative_prompt_embeds.to(dtype=prompt_embeds_dtype, device=device)
 
             negative_prompt_embeds = negative_prompt_embeds.repeat(1, num_images_per_prompt, 1)
             negative_prompt_embeds = negative_prompt_embeds.view(num_prompts * num_images_per_prompt, seq_len, -1)
 
+        if isinstance(self, LoraLoaderMixin) and USE_PEFT_BACKEND:
+            # Retrieve the original scale by scaling back the LoRA layers
+            unscale_lora_layers(self.text_encoder, lora_scale)
+
         return prompt_embeds, negative_prompt_embeds
 
     def run_safety_checker(self, image, device, dtype):
         if self.safety_checker is not None:
             feature_extractor_input = self.image_processor.postprocess(image, output_type="pil")
             safety_checker_input = self.feature_extractor(feature_extractor_input, return_tensors="pt").to(device)
             image, nsfw_detected, watermark_detected = self.safety_checker(
@@ -437,23 +509,24 @@
         if prompt_embeds is not None and negative_prompt_embeds is not None:
             if prompt_embeds.shape != negative_prompt_embeds.shape:
                 raise ValueError(
                     "`prompt_embeds` and `negative_prompt_embeds` must have the same shape when passed directly, but"
                     f" got: `prompt_embeds` {prompt_embeds.shape} != `negative_prompt_embeds`"
                     f" {negative_prompt_embeds.shape}."
                 )
-                if (
-                    not isinstance(image, torch.Tensor)
-                    and not isinstance(image, PIL.Image.Image)
-                    and not isinstance(image, np.ndarray)
-                    and not isinstance(image, list)
-                ):
-                    raise ValueError(
-                        f"`image` has to be of type `torch.Tensor`, `np.ndarray`, `PIL.Image.Image` or `list` but is {type(image)}"
-                    )
+
+        if (
+            not isinstance(image, torch.Tensor)
+            and not isinstance(image, PIL.Image.Image)
+            and not isinstance(image, np.ndarray)
+            and not isinstance(image, list)
+        ):
+            raise ValueError(
+                f"`image` has to be of type `torch.Tensor`, `np.ndarray`, `PIL.Image.Image` or `list` but is {type(image)}"
+            )
 
         # verify batch size of prompt and image are same if image is a list or tensor or numpy array
         if isinstance(image, list) or isinstance(image, torch.Tensor) or isinstance(image, np.ndarray):
             if prompt is not None and isinstance(prompt, str):
                 batch_size = 1
             elif prompt is not None and isinstance(prompt, list):
                 batch_size = len(prompt)
@@ -515,14 +588,40 @@
         # if xformers or torch_2_0 is used attention block does not need
         # to be in float32 which can save lots of memory
         if use_torch_2_0_or_xformers:
             self.vae.post_quant_conv.to(dtype)
             self.vae.decoder.conv_in.to(dtype)
             self.vae.decoder.mid_block.to(dtype)
 
+    def enable_freeu(self, s1: float, s2: float, b1: float, b2: float):
+        r"""Enables the FreeU mechanism as in https://arxiv.org/abs/2309.11497.
+
+        The suffixes after the scaling factors represent the stages where they are being applied.
+
+        Please refer to the [official repository](https://github.com/ChenyangSi/FreeU) for combinations of the values
+        that are known to work well for different pipelines such as Stable Diffusion v1, v2, and Stable Diffusion XL.
+
+        Args:
+            s1 (`float`):
+                Scaling factor for stage 1 to attenuate the contributions of the skip features. This is done to
+                mitigate "oversmoothing effect" in the enhanced denoising process.
+            s2 (`float`):
+                Scaling factor for stage 2 to attenuate the contributions of the skip features. This is done to
+                mitigate "oversmoothing effect" in the enhanced denoising process.
+            b1 (`float`): Scaling factor for stage 1 to amplify the contributions of backbone features.
+            b2 (`float`): Scaling factor for stage 2 to amplify the contributions of backbone features.
+        """
+        if not hasattr(self, "unet"):
+            raise ValueError("The pipeline must have `unet` for using FreeU.")
+        self.unet.enable_freeu(s1=s1, s2=s2, b1=b1, b2=b2)
+
+    def disable_freeu(self):
+        """Disables the FreeU mechanism if enabled."""
+        self.unet.disable_freeu()
+
     @classmethod
     def _split_inputs_into_batches(cls, batch_size, latents, text_embeddings, uncond_embeddings, image, noise_level):
         # Use torch.split to generate num_batches batches of size batch_size
         latents_batches = list(torch.split(latents, batch_size))
         text_embeddings_batches = list(torch.split(text_embeddings, batch_size))
         image_batches = list(torch.split(image, batch_size))
         noise_level_batches = list(torch.split(noise_level.view(-1, 1), batch_size))
@@ -593,14 +692,15 @@
         prompt_embeds: Optional[torch.FloatTensor] = None,
         negative_prompt_embeds: Optional[torch.FloatTensor] = None,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
         callback: Optional[Callable[[int, int, torch.FloatTensor], None]] = None,
         callback_steps: int = 1,
         cross_attention_kwargs: Optional[Dict[str, Any]] = None,
+        clip_skip: int = None,
     ):
         r"""
         Function invoked when calling the pipeline for generation.
 
         Args:
             prompt (`str` or `List[str]`, *optional*):
                 The prompt or prompts to guide the image generation. If not defined, one has to pass `prompt_embeds`.
@@ -653,14 +753,17 @@
             callback_steps (`int`, *optional*, defaults to 1):
                 The frequency at which the `callback` function will be called. If not specified, the callback will be
                 called at every step.
             cross_attention_kwargs (`dict`, *optional*):
                 A kwargs dictionary that if specified is passed along to the `AttentionProcessor` as defined under
                 `self.processor` in
                 [diffusers.cross_attention](https://github.com/huggingface/diffusers/blob/main/src/diffusers/models/cross_attention.py).
+            clip_skip (`int`, *optional*):
+                Number of layers to be skipped from CLIP while computing the prompt embeddings. A value of 1 means that
+                the output of the pre-final layer will be used for computing the prompt embeddings.
 
         Returns:
             [`~diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.GaudiStableDiffusionPipelineOutput`] or `tuple`:
             [`~diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.GaudiStableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple`.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
@@ -719,23 +822,24 @@
             # corresponds to doing no classifier free guidance.
             do_classifier_free_guidance = guidance_scale > 1.0
 
             # 2. Encode input prompt
             text_encoder_lora_scale = (
                 cross_attention_kwargs.get("scale", None) if cross_attention_kwargs is not None else None
             )
-            prompt_embeds, negative_prompt_embeds = self._encode_prompt(
+            prompt_embeds, negative_prompt_embeds = self.encode_prompt(
                 prompt,
                 device,
                 num_images_per_prompt,
                 do_classifier_free_guidance,
                 negative_prompt,
                 prompt_embeds=prompt_embeds,
                 negative_prompt_embeds=negative_prompt_embeds,
                 lora_scale=text_encoder_lora_scale,
+                clip_skip=clip_skip,
             )
 
             # 3. Preprocess image
             image = self.image_processor.preprocess(image)
             image = image.to(dtype=prompt_embeds.dtype, device=device)
 
             # 4. Prepare timesteps
@@ -847,25 +951,27 @@
                     )[0]
 
                     if not self.use_hpu_graphs:
                         self.htcore.mark_step()
 
                     # call the callback, if provided
                     if callback is not None and i % callback_steps == 0:
-                        callback(i, timestep, latents_batch)
+                        step_idx = i // getattr(self.scheduler, "order", 1)
+                        callback(step_idx, timestep, latents_batch)
 
                 if not output_type == "latent":
                     # 8. Post-processing
                     # make sure the VAE is in float32 mode, as it overflows in bfloat16
                     needs_upcasting = self.vae.dtype == torch.bfloat16 and self.vae.config.force_upcast
 
                     if needs_upcasting:
                         self.upcast_vae()
-                        latents = latents.to(next(iter(self.vae.post_quant_conv.parameters())).dtype)
 
+                    # Ensure latents are always the same type as the VAE
+                    latents_batch = latents_batch.to(next(iter(self.vae.post_quant_conv.parameters())).dtype)
                     image = self.vae.decode(latents_batch / self.vae.config.scaling_factor, return_dict=False)[0]
 
                     # cast back to fp16 if needed
                     if needs_upcasting:
                         self.vae.to(dtype=torch.bfloat16)
 
                     image, has_nsfw_concept, _ = self.run_safety_checker(image, device, prompt_embeds.dtype)
```

### Comparing `optimum-habana-1.8.2/optimum/habana/diffusers/schedulers/scheduling_ddim.py` & `optimum-habana-1.9.0/optimum/habana/diffusers/schedulers/scheduling_ddim.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.8.2/optimum/habana/distributed/distributed_runner.py` & `optimum-habana-1.9.0/optimum/habana/distributed/distributed_runner.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.8.2/optimum/habana/distributed/fast_ddp.py` & `optimum-habana-1.9.0/optimum/habana/distributed/fast_ddp.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/__init__.py` & `optimum-habana-1.9.0/optimum/habana/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/gaudi_configuration.py` & `optimum-habana-1.9.0/optimum/habana/transformers/gaudi_configuration.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import sys
-import warnings
 from pathlib import Path
 
 from optimum.configuration_utils import BaseConfig
 from optimum.utils import logging
 
 
 logger = logging.get_logger(__name__)
@@ -50,52 +49,35 @@
 
 
 class GaudiConfig(BaseConfig):
     CONFIG_NAME = "gaudi_config.json"
     FULL_CONFIGURATION_FILE = "gaudi_config.json"
 
     def __init__(self, **kwargs):
-        # Habana Mixed Precision (MHP) configuration
-        self.use_habana_mixed_precision = kwargs.pop("use_habana_mixed_precision", False)
-        self.hmp_bf16_ops = kwargs.pop("hmp_bf16_ops", DEFAULT_BF16_OPS)
-        self.hmp_fp32_ops = kwargs.pop("hmp_fp32_ops", DEFAULT_FP32_OPS)
-        self.hmp_is_verbose = kwargs.pop("hmp_is_verbose", False)
         # Torch Autocast
         self.use_torch_autocast = kwargs.pop("use_torch_autocast", False)
         self.autocast_bf16_ops = kwargs.pop("autocast_bf16_ops", None)
         self.autocast_fp32_ops = kwargs.pop("autocast_fp32_ops", None)
-
-        if self.use_habana_mixed_precision and self.use_torch_autocast:
-            raise ValueError(
-                "`use_habana_mixed_precision` and `use_torch_autocast` cannot be both `True` in your Gaudi configuration, you must choose one or the other to perform mixed-precision training."
-            )
+        self.use_dynamic_shapes = kwargs.pop("use_dynamic_shapes", False)
 
         # Use Habana's custom AdamW implementation
         self.use_fused_adam = kwargs.pop("use_fused_adam", False)
         # Use Habana's custom fused clip norm implementation
         self.use_fused_clip_norm = kwargs.pop("use_fused_clip_norm", False)
 
         # TODO: to remove in a future version
-        if "hmp_opt_level" in kwargs:
-            warnings.warn(
-                "`hmp_opt_level` is deprecated and will be removed in a future version.",
-                FutureWarning,
-            )
-        self.hmp_opt_level = kwargs.pop("hmp_opt_level", "O1")
 
     def write_bf16_fp32_ops_to_text_files(
         self,
         path_to_bf16_file: Path,
         path_to_fp32_file: Path,
-        autocast: bool = False,
     ):
-        bf16_ops = self.autocast_bf16_ops if autocast else self.hmp_bf16_ops
-        fp32_ops = self.autocast_fp32_ops if autocast else self.hmp_fp32_ops
-
-        for path, ops in zip([Path(path_to_bf16_file), Path(path_to_fp32_file)], [bf16_ops, fp32_ops]):
+        for path, ops in zip(
+            [Path(path_to_bf16_file), Path(path_to_fp32_file)], [self.autocast_bf16_ops, self.autocast_fp32_ops]
+        ):
             with path.open("w") as text_file:
                 # writelines does not add new lines after each element so "\n" is inserted
                 text_file.writelines(op + "\n" for op in ops)
 
     def declare_autocast_bf16_fp32_ops(self):
         if self.autocast_bf16_ops is not None and self.autocast_fp32_ops is not None:
             if "habana_frameworks.torch.core" in sys.modules:
@@ -106,11 +88,10 @@
             else:
                 autocast_bf16_filename = "/tmp/lower_list.txt"
                 autocast_fp32_filename = "/tmp/fp32_list.txt"
 
                 self.write_bf16_fp32_ops_to_text_files(
                     autocast_bf16_filename,
                     autocast_fp32_filename,
-                    autocast=True,
                 )
                 os.environ["LOWER_LIST"] = autocast_bf16_filename
                 os.environ["FP32_LIST"] = autocast_fp32_filename
```

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/generation/configuration_utils.py` & `optimum-habana-1.9.0/optimum/habana/transformers/generation/configuration_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,21 @@
         Skip HPU Graph usage for first token to save memory
     reuse_cache (`bool`, *optional*):
         Whether to reuse key/value cache for decoding. It should save memory.
     bucket_size (`int`, *optional*):
         If negative (default=-1) pad to max if `static_shapes` is set. Else start with
         `shape = bucket_size * ceil(prompt_len/bucket_size)` and then grow space by `bucket_size` when needed.
         Only active if `static_shapes` is used. Can't be used with `reuse_cache`.
+    kv_cache_fp8 (`bool`, *optional*):
+        Store kv-cache in float8 when kv-cache is used
     """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.trim_logits = kwargs.get("trim_logits", None)
         self.static_shapes = kwargs.get("static_shapes", None)
         self.ignore_eos = kwargs.get("ignore_eos", None)
         self.attn_softmax_bf16 = kwargs.get("attn_softmax_bf16", None)
         self.limit_hpu_graphs = kwargs.get("limit_hpu_graphs", None)
         self.reuse_cache = kwargs.get("reuse_cache", None)
         self.bucket_size = kwargs.get("bucket_size", -1)
+        self.kv_cache_fp8 = kwargs.get("kv_cache_fp8", None)
```

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/generation/utils.py` & `optimum-habana-1.9.0/optimum/habana/transformers/generation/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,20 +72,44 @@
     "gpt_neox",
     "llama",
     "falcon",
     "codegen",
     "gpt_bigcode",
     "bart",
     "mpt",
+    "mistral",
 ]
 
 
 logger = logging.get_logger(__name__)
 
 
+def incrementor(bucket_size, prompt_len):
+    assert bucket_size > 0
+    passnum = -1
+    while True:
+        passnum += 1
+        if passnum == 0:
+            token_idx = prompt_len
+            allocated_space = int(math.ceil(prompt_len / bucket_size) * bucket_size)
+            need_expansion = not (prompt_len == allocated_space)
+        else:
+            token_idx += 1
+            need_expansion = token_idx >= allocated_space
+            if need_expansion:
+                assert (allocated_space - token_idx) <= bucket_size
+                allocated_space += bucket_size
+        yield {
+            "allocated_space": allocated_space,
+            "passnum": passnum,
+            "token_idx": token_idx,
+            "need_expansion": need_expansion,
+        }
+
+
 class StaticMaxLengthCriteria(StoppingCriteria):
     def __init__(self, max_steps: int):
         self.max_steps = max_steps
         self.cur_step = 0
 
     def __call__(self, input_ids: torch.LongTensor, scores: torch.FloatTensor, **kwargs) -> bool:
         self.cur_step += 1
@@ -276,15 +300,18 @@
         self, generation_config: GaudiGenerationConfig, stopping_criteria: Optional[StoppingCriteriaList]
     ) -> StoppingCriteriaList:
         criteria = StoppingCriteriaList()
         if generation_config.max_length is not None:
             if (
                 generation_config.static_shapes
                 and self.config.is_encoder_decoder
-                and self.generation_config.generation_mode == GenerationMode.GREEDY_SEARCH
+                and (
+                    self.generation_config.generation_mode == GenerationMode.GREEDY_SEARCH
+                    or self.generation_config.generation_mode == GenerationMode.BEAM_SEARCH
+                )
             ):
                 criteria.append(StaticMaxLengthCriteria(generation_config.max_length))
             else:
                 max_position_embeddings = getattr(self.config, "max_position_embeddings", None)
                 criteria.append(
                     MaxLengthCriteria(
                         max_length=generation_config.max_length,
@@ -293,14 +320,63 @@
                 )
         if generation_config.max_time is not None:
             criteria.append(MaxTimeCriteria(max_time=generation_config.max_time))
         criteria = self._merge_criteria_processor_list(criteria, stopping_criteria)
         return criteria
 
     @torch.no_grad()
+    def update_model_kwargs_for_bucketing(self, params, input_ids, model_kwargs, pad_token_id, bucket_size):
+        if params["need_expansion"]:
+            # Pad inputs to have static shapes during generation, this gives better performance than dynamic shapes on HPUs
+            pad_amount = params["allocated_space"] - input_ids.shape[-1]
+            input_ids = torch.nn.functional.pad(input_ids, (0, pad_amount), value=pad_token_id)
+            if model_kwargs["attention_mask"] is not None:
+                model_kwargs["attention_mask"] = torch.nn.functional.pad(
+                    model_kwargs["attention_mask"], (0, pad_amount), value=0
+                )
+            else:
+                assert False, "Not tested for cases where attn_mask isnt passed"
+
+            if "past_key_values" in model_kwargs:
+
+                def create_pad_arg(pad_amount, i, j):
+                    if model_kwargs["past_key_values"][0][0].dim() == 3:
+                        assert self.config.model_type == "bloom"
+                        if j == 0:
+                            return (0, pad_amount)
+                        elif j == 1:
+                            return (0, 0, 0, pad_amount)
+                        else:
+                            assert False
+                    elif model_kwargs["past_key_values"][0][0].dim() == 4:
+                        return (0, 0, 0, pad_amount)  # llama, falcon
+                    else:
+                        assert False, "Unknown case, please handle, or dont use bucketing"
+
+                new_kv = [None for i in range(len(model_kwargs["past_key_values"]))]
+                for i in range(len(model_kwargs["past_key_values"])):
+                    tmp_lst = [None for j in range(len(model_kwargs["past_key_values"][i]))]
+                    for j in range(len(model_kwargs["past_key_values"][i])):
+                        pad_tuple = create_pad_arg(pad_amount, i, j)
+                        # Different models might have different shapes of kv-cache
+                        # create_pad_arg handles them on a per-model basis
+                        # This is a necessary (but not sufficient) condition: what ever dimension we are padding, should be a multiple of bucket_size
+                        # This check is added in case we get a new model with a new kv-cache structure, and we attempt to pad some wrong dimension
+                        assert model_kwargs["past_key_values"][i][j].shape[-(len(pad_tuple) // 2)] % bucket_size == 0
+                        tmp_lst[j] = torch.nn.functional.pad(
+                            model_kwargs["past_key_values"][i][j], pad_tuple, value=pad_token_id
+                        )
+                    new_kv[i] = tuple(tmp_lst)
+                model_kwargs["past_key_values"] = tuple(new_kv)
+
+        if "token_idx" not in model_kwargs:
+            model_kwargs["token_idx"] = torch.tensor(params["token_idx"], device=self.device)
+        return input_ids, model_kwargs
+
+    @torch.no_grad()
     def generate(
         self,
         inputs: Optional[torch.Tensor] = None,
         generation_config: Optional[GaudiGenerationConfig] = None,
         logits_processor: Optional[LogitsProcessorList] = None,
         stopping_criteria: Optional[StoppingCriteriaList] = None,
         prefix_allowed_tokens_fn: Optional[Callable[[int, torch.Tensor], List[int]]] = None,
@@ -416,33 +492,37 @@
         if hpu_graphs and not lazy_mode:
             raise ValueError(
                 "`hpu_graphs` is True but `lazy_mode` is False. HPU graphs require `lazy_mode` to be set to True."
             )
 
         # priority: `generation_config` argument > `model.generation_config` (the default generation config)
         if generation_config is None:
-            # legacy: users may modify the model configuration to control generation -- update the generation config
-            # model attribute accordingly, if it was created from the model config
-            if self.generation_config._from_model_config:
+            # legacy: users may modify the model configuration to control generation. To trigger this legacy behavior,
+            # two conditions must be met
+            # 1) the generation config must have been created from the model config (`_from_model_config` field);
+            # 2) the generation config must have seen no modification since its creation (the hash is the same).
+            if self.generation_config._from_model_config and self.generation_config._original_object_hash == hash(
+                self.generation_config
+            ):
                 new_generation_config = GaudiGenerationConfig.from_model_config(self.config)
                 if new_generation_config != self.generation_config:
                     warnings.warn(
                         "You have modified the pretrained model configuration to control generation. This is a"
                         " deprecated strategy to control generation and will be removed soon, in a future version."
-                        " Please use a generation configuration file (see"
-                        " https://huggingface.co/docs/transformers/main_classes/text_generation )"
+                        " Please use and modify the model generation configuration (see"
+                        " https://huggingface.co/docs/transformers/generation_strategies#default-text-generation-configuration )"
                     )
                     self.generation_config = new_generation_config
             generation_config = self.generation_config
 
         generation_config = copy.deepcopy(generation_config)
         if generation_config.static_shapes is None:
             generation_config.static_shapes = self.config.model_type in MODELS_OPTIMIZED_WITH_STATIC_SHAPES
         if generation_config.ignore_eos is None:
-            generation_config.ignore_eos = lazy_mode
+            generation_config.ignore_eos = kwargs.get("ignore_eos", lazy_mode)
         generation_config.validate()
         model_kwargs = generation_config.update(**kwargs)  # All unused kwargs must be model kwargs
         self._validate_model_kwargs(model_kwargs.copy())
         # 2. Set generation parameters if not already defined
         logits_processor = logits_processor if logits_processor is not None else LogitsProcessorList()
         stopping_criteria = stopping_criteria if stopping_criteria is not None else StoppingCriteriaList()
 
@@ -484,41 +564,44 @@
         requires_attention_mask = "encoder_outputs" not in model_kwargs
 
         if model_kwargs.get("attention_mask", None) is None and requires_attention_mask and accepts_attention_mask:
             model_kwargs["attention_mask"] = self._prepare_attention_mask_for_generation(
                 inputs_tensor, generation_config.pad_token_id, generation_config.eos_token_id
             )
 
-        is_greedy_and_bucket = (
-            generation_config.bucket_size > 0
-            and self._get_generation_mode(generation_config, assistant_model) == GenerationMode.GREEDY_SEARCH
+        is_greedy_or_beam_and_bucket = generation_config.bucket_size > 0 and (
+            self._get_generation_mode(generation_config, assistant_model) == GenerationMode.GREEDY_SEARCH
+            or self._get_generation_mode(generation_config, assistant_model) == GenerationMode.BEAM_SEARCH
         )
         model_kwargs["bucket_size"] = generation_config.bucket_size if generation_config.static_shapes else -1
         if generation_config.reuse_cache:
             assert generation_config.bucket_size <= 0, "reuse_cache and bucketing flags set together"
 
         if generation_config.static_shapes:
             # Pad inputs to have static shapes during generation, this gives better performance than dynamic shapes on HPUs
             # In encoder_decoder models, Inputs are already padded
 
             if not self.config.is_encoder_decoder:
                 # only pad if bucket_size < -1. If we are bucketing (bucket_size > 0), then that is taken care in greedy_search()
-                if not is_greedy_and_bucket:
+                if not is_greedy_or_beam_and_bucket:
                     # token_idx is the current index in the generation process, it is incremented each time a new token is generated
-                    model_kwargs["token_idx"] = torch.tensor(inputs_tensor.shape[-1], device=inputs_tensor.device)
+                    token_idx = inputs_tensor.shape[-1]
+                    model_kwargs["token_idx"] = torch.tensor(token_idx, device=inputs_tensor.device)
                     inputs_tensor = torch.nn.functional.pad(
                         inputs_tensor, (0, generation_config.max_new_tokens), value=generation_config.pad_token_id
                     )
-                    if model_kwargs["attention_mask"] is not None:
-                        model_kwargs["attention_mask"] = torch.nn.functional.pad(
-                            model_kwargs["attention_mask"], (0, generation_config.max_new_tokens), value=0
-                        )
+                    for other_inputs in ["attention_mask", "token_type_ids"]:
+                        if model_kwargs.get(other_inputs) is not None:
+                            model_kwargs[other_inputs] = torch.nn.functional.pad(
+                                model_kwargs[other_inputs], (0, generation_config.max_new_tokens), value=0
+                            )
             else:
                 assert generation_config.bucket_size <= 0, "Untested path for bucket>0"
-                model_kwargs["token_idx"] = torch.tensor(1, device=inputs_tensor.device)
+                token_idx = 1
+                model_kwargs["token_idx"] = torch.tensor(token_idx, device=inputs_tensor.device)
                 if model_kwargs.get("decoder_attention_mask", None) is None and generation_config.use_cache:
                     model_kwargs["decoder_attention_mask"] = self._prepare_decoder_attention_mask(
                         generation_config.max_length,
                         inputs_tensor.shape[0],
                         generation_config.pad_token_id,
                         inputs_tensor.device,
                     )
@@ -561,15 +644,15 @@
         if streamer is not None:
             streamer.put(input_ids.cpu())
 
         # 6. Prepare `max_length` depending on other stopping criteria.
         input_ids_length = input_ids.shape[-1]
         has_default_max_length = kwargs.get("max_length") is None and generation_config.max_length is not None
         if generation_config.max_new_tokens is not None:
-            if not has_default_max_length:
+            if not has_default_max_length and generation_config.max_length is not None:
                 logger.warning(
                     f"Both `max_new_tokens` (={generation_config.max_new_tokens}) and `max_length`(="
                     f"{generation_config.max_length}) seem to have been set. `max_new_tokens` will take precedence. "
                     "Please refer to the documentation for more information. "
                     "(https://huggingface.co/docs/transformers/main/en/main_classes/text_generation)"
                 )
             generation_config.max_length = generation_config.max_new_tokens + input_ids_length
@@ -589,27 +672,33 @@
 
         if not self.config.is_encoder_decoder:
             calculated_max_length = input_ids.shape[-1]
             if not generation_config.static_shapes and generation_config.max_new_tokens is not None:
                 calculated_max_length = input_ids.shape[-1] + generation_config.max_new_tokens
             if generation_config.use_cache and generation_config.reuse_cache:
                 bs, _ = input_ids.shape
-                if not is_greedy_and_bucket:
+                if not is_greedy_or_beam_and_bucket:
                     unwrap_deepspeed_model(self).allocate_kv_cache(
-                        bs * generation_config.num_beams, calculated_max_length
+                        bs * generation_config.num_beams,
+                        calculated_max_length,
+                        token_idx,
+                        generation_config.kv_cache_fp8,
                     )
+            if self.config.model_type in ["llama"]:
+                if self.config.max_position_embeddings < calculated_max_length:
+                    unwrap_deepspeed_model(self).update_sincos_cache(seq_len=calculated_max_length)
 
         # 7. determine generation mode
         generation_mode = self._get_generation_mode(generation_config, assistant_model)
         if generation_config.bucket_size > 0:
             assert generation_config.static_shapes, "bucket_size > 0 can be set only when static_shapes is set"
         # if generation_config.bucket_size <= 0, padding is handled by the generating fn (like greedy_search)
         if generation_config.static_shapes and generation_config.bucket_size > 0:
             assert (
-                generation_mode == GenerationMode.GREEDY_SEARCH
+                generation_mode == GenerationMode.GREEDY_SEARCH or generation_mode == GenerationMode.BEAM_SEARCH
             ), "generation_config.bucket_size > 0 supported only for greedy mode"
 
         if streamer is not None and (generation_config.num_beams > 1):
             raise ValueError(
                 "`streamer` cannot be used with beam search (yet!). Make sure that `num_beams` is set to 1."
             )
 
@@ -1247,36 +1336,14 @@
             unfinished_sequences = torch.ones(input_ids.shape[0], dtype=torch.long, device=input_ids.device)
 
         hb_profer = HabanaProfile(warmup=profiling_warmup_steps, active=profiling_steps)
         hb_profer.start()
         this_peer_finished = False  # used by synced_gpus only
         bucket_size = model_kwargs["bucket_size"]
 
-        def incrementor(bucket_size, prompt_len):
-            assert bucket_size > 0
-            passnum = -1
-            while True:
-                passnum += 1
-                if passnum == 0:
-                    token_idx = prompt_len
-                    allocated_space = int(math.ceil(prompt_len / bucket_size) * bucket_size)
-                    need_expansion = not (prompt_len == allocated_space)
-                else:
-                    token_idx += 1
-                    need_expansion = token_idx >= allocated_space
-                    if need_expansion:
-                        assert (allocated_space - token_idx) <= bucket_size
-                        allocated_space += bucket_size
-                yield {
-                    "allocated_space": allocated_space,
-                    "passnum": passnum,
-                    "token_idx": token_idx,
-                    "need_expansion": need_expansion,
-                }
-
         prompt_len = input_ids.shape[-1]
         if bucket_size >= 0:
             inc = iter(incrementor(bucket_size, prompt_len))
         if bucket_size > 0:
             assert "position_ids" not in model_kwargs, "Untested path"
 
         while True:
@@ -1292,63 +1359,17 @@
                 # did all peers finish? the reduced sum will be 0.0 then
                 if this_peer_finished_flag.item() == 0.0:
                     break
 
             if bucket_size > 0:
                 # it will not have been padded if bucket_size > 0
                 params = next(inc)
-
-                if params["need_expansion"]:
-                    # Pad inputs to have static shapes during generation, this gives better performance than dynamic shapes on HPUs
-                    pad_amount = params["allocated_space"] - input_ids.shape[-1]
-                    input_ids = torch.nn.functional.pad(input_ids, (0, pad_amount), value=pad_token_id)
-                    if model_kwargs["attention_mask"] is not None:
-                        model_kwargs["attention_mask"] = torch.nn.functional.pad(
-                            model_kwargs["attention_mask"], (0, pad_amount), value=0
-                        )
-                    else:
-                        assert False, "Not tested for cases where attn_mask isnt passed"
-
-                    if "past_key_values" in model_kwargs:
-
-                        def create_pad_arg(pad_amount, i, j):
-                            if model_kwargs["past_key_values"][0][0].dim() == 3:
-                                assert self.config.model_type == "bloom"
-                                if j == 0:
-                                    return (0, pad_amount)
-                                elif j == 1:
-                                    return (0, 0, 0, pad_amount)
-                                else:
-                                    assert False
-                            elif model_kwargs["past_key_values"][0][0].dim() == 4:
-                                return (0, 0, 0, pad_amount)  # llama, falcon
-                            else:
-                                assert False, "Unknown case, please handle, or dont use bucketing"
-
-                        new_kv = [None for i in range(len(model_kwargs["past_key_values"]))]
-                        for i in range(len(model_kwargs["past_key_values"])):
-                            tmp_lst = [None for j in range(len(model_kwargs["past_key_values"][i]))]
-                            for j in range(len(model_kwargs["past_key_values"][i])):
-                                pad_tuple = create_pad_arg(pad_amount, i, j)
-                                # Different models might have different shapes of kv-cache
-                                # create_pad_arg handles them on a per-model basis
-                                # This is a necessary (but not sufficient) condition: what ever dimension we are padding, should be a multiple of bucket_size
-                                # This check is added in case we get a new model with a new kv-cache structure, and we attempt to pad some wrong dimension
-                                assert (
-                                    model_kwargs["past_key_values"][i][j].shape[-(len(pad_tuple) // 2)] % bucket_size
-                                    == 0
-                                )
-                                tmp_lst[j] = torch.nn.functional.pad(
-                                    model_kwargs["past_key_values"][i][j], pad_tuple, value=pad_token_id
-                                )
-                            new_kv[i] = tuple(tmp_lst)
-                        model_kwargs["past_key_values"] = tuple(new_kv)
-
-                if "token_idx" not in model_kwargs:
-                    model_kwargs["token_idx"] = torch.tensor(params["token_idx"], device=self.device)
+                input_ids, model_kwargs = self.update_model_kwargs_for_bucketing(
+                    params, input_ids, model_kwargs, pad_token_id, bucket_size
+                )
 
             # prepare model inputs
             model_inputs = self.prepare_inputs_for_generation(input_ids, **model_kwargs)
 
             hpu_graphs_kwargs = self._get_hpu_graphs_kwargs(model_kwargs)
 
             # forward pass to get next token
@@ -1975,25 +1996,39 @@
         # of the first beam are considered to avoid sampling the exact same tokens across all beams.
         beam_scores = torch.zeros((batch_size, num_beams), dtype=torch.float, device=input_ids.device)
         beam_scores[:, 1:] = -1e9
         beam_scores = beam_scores.view((batch_size * num_beams,))
         hb_profer = HabanaProfile(warmup=profiling_warmup_steps, active=profiling_steps)
         hb_profer.start()
         this_peer_finished = False  # used by synced_gpus only
+
+        bucket_size = model_kwargs["bucket_size"]
+        prompt_len = input_ids.shape[-1]
+        if bucket_size >= 0:
+            inc = iter(incrementor(bucket_size, prompt_len))
+        if bucket_size > 0:
+            assert "position_ids" not in model_kwargs, "Untested path"
         while True:
             if synced_gpus:
                 # Under synced_gpus the `forward` call must continue until all gpus complete their sequence.
                 # The following logic allows an early break if all peers finished generating their sequence
                 this_peer_finished_flag = torch.tensor(0.0 if this_peer_finished else 1.0).to(input_ids.device)
                 # send 0.0 if we finished, 1.0 otherwise
                 dist.all_reduce(this_peer_finished_flag, op=dist.ReduceOp.SUM)
                 # did all peers finish? the reduced sum will be 0.0 then
                 if this_peer_finished_flag.item() == 0.0:
                     break
 
+            if bucket_size > 0:
+                # it will not have been padded if bucket_size > 0
+                params = next(inc)
+                input_ids, model_kwargs = self.update_model_kwargs_for_bucketing(
+                    params, input_ids, model_kwargs, pad_token_id, bucket_size
+                )
+
             model_inputs = self.prepare_inputs_for_generation(input_ids, **model_kwargs)
 
             hpu_graphs_kwargs = self._get_hpu_graphs_kwargs(model_kwargs)
 
             outputs = self(
                 **model_inputs,
                 return_dict=True,
@@ -2013,15 +2048,17 @@
                 next_token_logits = outputs.logits[:, -1, :]
 
             next_token_scores = torch.nn.functional.log_softmax(
                 next_token_logits, dim=-1
             )  # (batch_size * num_beams, vocab_size)
 
             next_token_scores_processed = logits_processor(input_ids, next_token_scores)
-            next_token_scores = next_token_scores_processed + beam_scores[:, None].expand_as(next_token_scores)
+            next_token_scores = next_token_scores_processed + beam_scores[:, None].expand_as(
+                next_token_scores_processed
+            )
 
             # Store scores, attentions and hidden_states when required
             if return_dict_in_generate:
                 if output_scores:
                     scores += (next_token_scores_processed,)
                 if output_attentions:
                     decoder_attentions += (
@@ -2093,15 +2130,15 @@
                 if not synced_gpus:
                     break
                 else:
                     this_peer_finished = True
         hb_profer.stop()
 
         sequence_outputs = beam_scorer.finalize(
-            input_ids,
+            input_ids[:, :cur_len],
             beam_scores,
             next_tokens,
             next_indices,
             pad_token_id=pad_token_id,
             eos_token_id=eos_token_id,
             max_length=stopping_criteria.max_length,
             beam_indices=beam_indices,
@@ -2663,15 +2700,17 @@
 
             next_token_scores = torch.nn.functional.log_softmax(
                 next_token_logits, dim=-1
             )  # (batch_size * num_beams, vocab_size)
 
             next_token_scores_processed = logits_processor(input_ids, next_token_scores)
 
-            next_token_scores = next_token_scores_processed + beam_scores[:, None].expand_as(next_token_scores)
+            next_token_scores = next_token_scores_processed + beam_scores[:, None].expand_as(
+                next_token_scores_processed
+            )
 
             scores_for_all_vocab = next_token_scores.clone()
 
             # Store scores, attentions and hidden_states when required
             if return_dict_in_generate:
                 if output_scores:
                     scores += (next_token_scores,)
```

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/gradient_checkpointing.py` & `optimum-habana-1.9.0/optimum/habana/transformers/gradient_checkpointing.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/integrations/deepspeed.py` & `optimum-habana-1.9.0/optimum/habana/transformers/integrations/deepspeed.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/modeling_utils.py` & `optimum-habana-1.9.0/optimum/habana/transformers/modeling_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,18 +29,21 @@
     GaudiGPTJAttention,
     GaudiGPTJForCausalLM,
     GaudiGPTNeoXForCausalLM,
     GaudiLlamaAttention,
     GaudiLlamaDecoderLayer,
     GaudiLlamaForCausalLM,
     GaudiLlamaModel,
+    GaudiMistralForCausalLM,
     GaudiMptForCausalLM,
     GaudiMptModel,
     GaudiOPTForCausalLM,
     GaudiOPTLearnedPositionalEmbedding,
+    # _gaudi_wav2vec2_compute_mask_indices,
+    # _gaudi_wav2vec2_mask_hidden_states,
     gaudi_albert_forward,
     gaudi_BartAttention_forward,
     gaudi_BartDecoder_forward,
     gaudi_BartDecoderLayer_forward,
     gaudi_BartEncoder_forward,
     gaudi_BartEncoderLayer_forward,
     gaudi_BartForConditionalGeneration_forward,
@@ -53,16 +56,14 @@
     gaudi_bloom_convert_to_standard_cache,
     gaudi_bloom_model_forward,
     gaudi_codegen_block_forward,
     gaudi_codegen_model_forward,
     gaudi_conv1d_forward,
     gaudi_esm_for_protein_folding_forward,
     gaudi_esmfolding_trunk_forward,
-    gaudi_esmoutput_forward,
-    gaudi_esmselfoutput_forward,
     gaudi_falcon_attention_forward,
     gaudi_falcon_attention_split_heads,
     gaudi_falcon_decoder_layer_forward,
     gaudi_falcon_rotary_embedding_forward,
     gaudi_get_extended_attention_mask,
     gaudi_gpt2_block_forward,
     gaudi_gpt2_forward,
@@ -72,24 +73,28 @@
     gaudi_gpt_neox_attention_forward,
     gaudi_gpt_neox_layer_forward,
     gaudi_gpt_neox_model_forward,
     gaudi_gptj_block_forward,
     gaudi_gptj_model_forward,
     gaudi_invert_attention_mask,
     gaudi_llama_rmsnorm_forward,
+    gaudi_mistral_attn_forward,
+    gaudi_mistral_decoder_layer_forward,
+    gaudi_mistral_model_forward,
     gaudi_mpt_attention_forward,
     gaudi_mpt_block_forward,
     gaudi_opt_attention_forward,
     gaudi_opt_decoder_forward,
     gaudi_opt_decoder_layer_forward,
     gaudi_opt_model_forward,
     gaudi_rot_matmul,
     gaudi_rot_vec_mul,
     gaudi_t5_layernorm_forward,
     gaudi_vit_self_attention_forward,
+    # gaudi_wav2vec2_encoder_forward,
     gaudi_wav2vec2_forward,
 )
 
 
 def adapt_transformers_to_gaudi():
     """
     Replaces some Transformers' methods for equivalent methods optimized
@@ -99,24 +104,33 @@
     # optimize Conv1D
     transformers.pytorch_utils.Conv1D.forward = gaudi_conv1d_forward
 
     # Optimization tweak for ViT
     transformers.models.vit.modeling_vit.ViTSelfAttention.forward = gaudi_vit_self_attention_forward
 
     # Optimization tweak for Wav2Vec2
+    # TODO: enable _gaudi_wav2vec2_compute_mask_indices, _gaudi_wav2vec2_mask_hidden_states and
+    # gaudi_wav2vec2_encoder_forward when SynapseAI v1.13 is released
+    # They are disabled for now due to accuracy issues
     # transformers.models.wav2vec2.modeling_wav2vec2._compute_mask_indices = _gaudi_wav2vec2_compute_mask_indices
     # transformers.models.wav2vec2.modeling_wav2vec2._sample_negative_indices = _gaudi_wav2vec2_sample_negative_indices
-    # transformers.models.wav2vec2.modeling_wav2vec2.Wav2Vec2Model._mask_hidden_states = _gaudi_wav2vec2_mask_hidden_states
+    # transformers.models.wav2vec2.modeling_wav2vec2.Wav2Vec2Model._mask_hidden_states = (
+    #     _gaudi_wav2vec2_mask_hidden_states
+    # )
     transformers.models.wav2vec2.modeling_wav2vec2.Wav2Vec2Model.forward = gaudi_wav2vec2_forward
+    # transformers.models.wav2vec2.modeling_wav2vec2.Wav2Vec2Encoder.forward = gaudi_wav2vec2_encoder_forward
 
     # Generation is modified to run faster in lazy mode
     transformers.generation.GenerationMixin.generate = GaudiGenerationMixin.generate
     transformers.generation.GenerationMixin._update_model_kwargs_for_generation = (
         GaudiGenerationMixin._update_model_kwargs_for_generation
     )
+    transformers.generation.GenerationMixin.update_model_kwargs_for_bucketing = (
+        GaudiGenerationMixin.update_model_kwargs_for_bucketing
+    )
     transformers.generation.GenerationMixin._get_hpu_graphs_kwargs = GaudiGenerationMixin._get_hpu_graphs_kwargs
     transformers.generation.GenerationMixin._expand_inputs_for_generation = staticmethod(
         GaudiGenerationMixin._expand_inputs_for_generation
     )
     transformers.generation.GenerationMixin._prepare_attention_mask_for_generation = (
         GaudiGenerationMixin._prepare_attention_mask_for_generation
     )
@@ -169,15 +183,15 @@
     # Since HCCL cannot handle this dtype, we revert it back to uint8
     transformers.models.codegen.modeling_codegen.CodeGenAttention = GaudiCodeGenAttention
     transformers.models.codegen.modeling_codegen.CodeGenForCausalLM = GaudiCodeGenForCausalLM
     transformers.models.codegen.modeling_codegen.CodeGenModel.forward = gaudi_codegen_model_forward
     transformers.models.codegen.modeling_codegen.CodeGenBlock.forward = gaudi_codegen_block_forward
 
     # Replace invert_attention_mask and get_extended_attention_mask
-    # so that HMP is disabled for specific parts of the code
+    # so that Torch Autocast is disabled for specific parts of the code
     transformers.modeling_utils.ModuleUtilsMixin.invert_attention_mask = gaudi_invert_attention_mask
     transformers.modeling_utils.ModuleUtilsMixin.get_extended_attention_mask = gaudi_get_extended_attention_mask
     # AlbertModel.forward does not rely on get_extended_attention_mask so it also needs to be replaced
     transformers.models.albert.modeling_albert.AlbertModel.forward = gaudi_albert_forward
 
     # From Transformers 4.27, the bias in the GPT2Attention layer is a Boolean
     # Since HCCL cannot handle this dtype, we revert it back to uint8 (same behaviour as Transformers <= 4.26)
@@ -187,16 +201,14 @@
     transformers.models.gpt2.modeling_gpt2.GPT2Block.forward = gaudi_gpt2_block_forward
 
     # Optimization for EsmFold on Gaudi
     transformers.models.esm.modeling_esmfold.EsmFoldingTrunk.forward = gaudi_esmfolding_trunk_forward
     transformers.models.esm.modeling_esmfold.EsmForProteinFolding.forward = gaudi_esm_for_protein_folding_forward
     transformers.models.esm.openfold_utils.rigid_utils.rot_matmul = gaudi_rot_matmul
     transformers.models.esm.openfold_utils.rigid_utils.rot_vec_mul = gaudi_rot_vec_mul
-    transformers.models.esm.modeling_esm.EsmSelfOutput.forward = gaudi_esmselfoutput_forward
-    transformers.models.esm.modeling_esm.EsmOutput.forward = gaudi_esmoutput_forward
 
     # Optimization for OPT generation on Gaudi
     transformers.models.opt.modeling_opt.OPTAttention.forward = gaudi_opt_attention_forward
     transformers.models.opt.modeling_opt.OPTDecoder.forward = gaudi_opt_decoder_forward
     transformers.models.opt.modeling_opt.OPTForCausalLM = GaudiOPTForCausalLM
     transformers.models.opt.modeling_opt.OPTModel.forward = gaudi_opt_model_forward
     transformers.models.opt.modeling_opt.OPTDecoderLayer.forward = gaudi_opt_decoder_layer_forward
@@ -244,7 +256,13 @@
     transformers.models.t5.modeling_t5.T5LayerNorm.forward = gaudi_t5_layernorm_forward
 
     # Optimization for mpt on Gaudi
     transformers.models.mpt.modeling_mpt.MptForCausalLM = GaudiMptForCausalLM
     transformers.models.mpt.modeling_mpt.MptModel = GaudiMptModel
     transformers.models.mpt.modeling_mpt.MptAttention.forward = gaudi_mpt_attention_forward
     transformers.models.mpt.modeling_mpt.MptBlock.forward = gaudi_mpt_block_forward
+
+    # Optimization for mistral on Gaudi
+    transformers.models.mistral.modeling_mistral.MistralForCausalLM = GaudiMistralForCausalLM
+    transformers.models.mistral.modeling_mistral.MistralModel.forward = gaudi_mistral_model_forward
+    transformers.models.mistral.modeling_mistral.MistralAttention.forward = gaudi_mistral_attn_forward
+    transformers.models.mistral.modeling_mistral.MistralDecoderLayer.forward = gaudi_mistral_decoder_layer_forward
```

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/models/__init__.py` & `optimum-habana-1.9.0/optimum/habana/transformers/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,14 @@
     GaudiCodeGenForCausalLM,
     gaudi_codegen_block_forward,
     gaudi_codegen_model_forward,
 )
 from .esm import (
     gaudi_esm_for_protein_folding_forward,
     gaudi_esmfolding_trunk_forward,
-    gaudi_esmoutput_forward,
-    gaudi_esmselfoutput_forward,
     gaudi_rot_matmul,
     gaudi_rot_vec_mul,
 )
 from .falcon import (
     GaudiFalconForCausalLM,
     GaudiFalconModel,
     gaudi_falcon_attention_forward,
@@ -63,14 +61,20 @@
 from .llama import (
     GaudiLlamaAttention,
     GaudiLlamaDecoderLayer,
     GaudiLlamaForCausalLM,
     GaudiLlamaModel,
     gaudi_llama_rmsnorm_forward,
 )
+from .mistral import (
+    GaudiMistralForCausalLM,
+    gaudi_mistral_attn_forward,
+    gaudi_mistral_decoder_layer_forward,
+    gaudi_mistral_model_forward,
+)
 from .modeling_all_models import gaudi_conv1d_forward, gaudi_get_extended_attention_mask, gaudi_invert_attention_mask
 from .mpt import (
     GaudiMptForCausalLM,
     GaudiMptModel,
     gaudi_mpt_attention_forward,
     gaudi_mpt_block_forward,
 )
@@ -84,9 +88,10 @@
 )
 from .t5 import gaudi_t5_layernorm_forward
 from .vit import gaudi_vit_self_attention_forward
 from .wav2vec2 import (
     _gaudi_wav2vec2_compute_mask_indices,
     _gaudi_wav2vec2_mask_hidden_states,
     _gaudi_wav2vec2_sample_negative_indices,
+    gaudi_wav2vec2_encoder_forward,
     gaudi_wav2vec2_forward,
 )
```

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/models/albert/modeling_albert.py` & `optimum-habana-1.9.0/optimum/habana/transformers/models/albert/modeling_albert.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     inputs_embeds: Optional[torch.FloatTensor] = None,
     output_attentions: Optional[bool] = None,
     output_hidden_states: Optional[bool] = None,
     return_dict: Optional[bool] = None,
 ) -> Union[BaseModelOutputWithPooling, Tuple]:
     """
     Same as https://github.com/huggingface/transformers/blob/a9eee2ffecc874df7dd635b2c6abb246fdb318cc/src/transformers/models/albert/modeling_albert.py#L689
-    except that HMP is disabled for computing:
+    except that mixed precision is disabled for computing:
         extended_attention_mask = (1.0 - extended_attention_mask) * torch.finfo(self.dtype).min
     """
     output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
     output_hidden_states = (
         output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
     )
     return_dict = return_dict if return_dict is not None else self.config.use_return_dict
```

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/models/bart/modeling_bart.py` & `optimum-habana-1.9.0/optimum/habana/transformers/models/bart/modeling_bart.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/models/bloom/modeling_bloom.py` & `optimum-habana-1.9.0/optimum/habana/transformers/models/bloom/modeling_bloom.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,21 @@
     else:
         # code taken from Megatron transformer.py
         alibi = slopes.unsqueeze(1).unsqueeze(1) * torch.arange(seq_length, device=attention_mask.device).unsqueeze(
             0
         ).unsqueeze(0).expand(num_heads, -1, -1)
 
         # Select the part of the tensor that corresponds to our tensor parallel index.
-        tp_world_size = int(os.environ.get("WORLD_SIZE", 1))
-        tp_index = int(os.environ.get("RANK", 0))
+        # if inference_tp_size is set use it instead of world size
+        world = int(os.environ.get("WORLD_SIZE", 1))
+        tp_world_size = GaudiBloomForCausalLM.inference_tp_size if GaudiBloomForCausalLM.inference_tp_size else world
+        tp_index = 0  # if world size == 1 ignore rank and use 0 (for cases where WORLD_SIZE is not equal to tp size)
+        if tp_world_size > 1:
+            tp_index = int(os.environ.get("RANK", 0))
+
         alibi = alibi.reshape((tp_world_size, -1, *alibi.shape[1:]))[tp_index]
 
         alibi = alibi.repeat(batch_size, 1, 1)
         return alibi.to(dtype)
 
 
 def update(prev, cur, dim, idx):
@@ -278,15 +283,16 @@
     Standardizes the format of the cache so as to match most implementations, i.e. to tuple(tuple([batch_size,
     num_heads, ...]))
     """
     batch_size_times_num_heads, head_dim, seq_length = past_key_value[0][0].shape
     if training:
         num_heads = batch_size_times_num_heads // batch_size
     else:
-        tp_world_size = int(os.environ.get("WORLD_SIZE", 1))
+        world = int(os.environ.get("WORLD_SIZE", 1))
+        tp_world_size = GaudiBloomForCausalLM.inference_tp_size if GaudiBloomForCausalLM.inference_tp_size else world
         num_heads = self.config.n_head // tp_world_size
         batch_size = batch_size_times_num_heads // num_heads
     # key: [batch_size * num_heads, head_dim, seq_length] -> [batch_size, num_heads, head_dim, seq_length]
     # value: [batch_size * num_heads, seq_length, head_dim] -> [batch_size, num_heads, seq_length, head_dim]
     return tuple(
         (
             layer_past[0].view(batch_size, num_heads, head_dim, seq_length),
@@ -458,14 +464,21 @@
         past_key_values=presents,
         hidden_states=all_hidden_states,
         attentions=all_self_attentions,
     )
 
 
 class GaudiBloomForCausalLM(BloomForCausalLM):
+    inference_tp_size = None
+
+    def set_tp_for_inference(tp_for_inference: int):
+        world = int(os.environ.get("WORLD_SIZE", 1))
+        assert tp_for_inference == 1 or tp_for_inference == world, "only setting 1 (no tp) or world size is supported"
+        GaudiBloomForCausalLM.inference_tp_size = tp_for_inference
+
     def prepare_inputs_for_generation(
         self,
         input_ids: torch.LongTensor,
         past_key_values: Optional[torch.Tensor] = None,
         attention_mask: Optional[torch.Tensor] = None,
         inputs_embeds: Optional[torch.Tensor] = None,
         token_idx: Optional[torch.Tensor] = None,
```

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/models/codegen/modeling_codegen.py` & `optimum-habana-1.9.0/optimum/habana/transformers/models/codegen/modeling_codegen.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,17 +413,17 @@
     """
 
     def prepare_inputs_for_generation(self, input_ids, past_key_values=None, token_idx=None, **kwargs):
         token_type_ids = kwargs.get("token_type_ids", None)
         # only last token for inputs_ids if past is defined in kwargs
         if past_key_values:
             if token_idx is not None:
-                input_ids = torch.index_select(input_ids, 1, token_idx - 1).unsqueeze(-1)
+                input_ids = torch.index_select(input_ids, 1, token_idx - 1)
                 if token_type_ids is not None:
-                    token_type_ids = torch.index_select(token_type_ids, 1, token_idx - 1).unsqueeze(-1)
+                    token_type_ids = torch.index_select(token_type_ids, 1, token_idx - 1)
             else:
                 input_ids = input_ids[:, -1].unsqueeze(-1)
                 if token_type_ids is not None:
                     token_type_ids = token_type_ids[:, -1].unsqueeze(-1)
 
         attention_mask = kwargs.get("attention_mask", None)
         position_ids = kwargs.get("position_ids", None)
```

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/models/esm/modeling_esmfold.py` & `optimum-habana-1.9.0/optimum/habana/transformers/models/esm/modeling_esmfold.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/models/falcon/modeling_falcon.py` & `optimum-habana-1.9.0/optimum/habana/transformers/models/falcon/modeling_falcon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,34 @@
+import contextlib
 import math
 from typing import Optional, Tuple, Union
 
 import torch
 
-from ....utils import get_device_name
-
 
 try:
     from habana_frameworks.torch.hpex.kernels import FusedSDPA
 except ImportError:
     print("Not using HPU fused kernel for scaled_dot_product_attention")
     FusedSDPA = None
 
-# TODO: remove this workaround when FusedRoPE properly works on Gaudi
-if get_device_name() == "gaudi2":
-    try:
-        from habana_frameworks.torch.hpex.kernels import RotaryPosEmbeddingHelperV1 as FusedRoPE
-    except ImportError:
-        print("Not using HPU fused kernel for apply_rotary_pos_emb")
-        FusedRoPE = None
-else:
+try:
+    from habana_frameworks.torch.hpu import sdp_kernel
+
+    SDPContext = True
+except ImportError:
+    SDPContext = False
+
+try:
+    from habana_frameworks.torch.hpex.kernels import RotaryPosEmbeddingHelperV1 as FusedRoPE
+except ImportError:
+    print("Not using HPU fused kernel for apply_rotary_pos_emb")
     FusedRoPE = None
 
+
 import habana_frameworks.torch.core as htcore
 from torch.nn import CrossEntropyLoss
 from torch.nn import functional as F
 from transformers.modeling_outputs import (
     BaseModelOutputWithPastAndCrossAttentions,
     CausalLMOutputWithCrossAttentions,
 )
@@ -53,25 +56,104 @@
 
     if FusedRoPE:
         return FusedRoPE.apply(query, cos, sin, 0), FusedRoPE.apply(key, cos, sin, 0)
     else:
         return (query * cos) + (rotate_half(query) * sin), (key * cos) + (rotate_half(key) * sin)
 
 
+def _make_causal_mask(
+    input_ids_shape: torch.Size, device: torch.device, past_key_values_length: int
+) -> torch.BoolTensor:
+    batch_size, target_length = input_ids_shape
+
+    mask = torch.empty((target_length, target_length + past_key_values_length), dtype=torch.bool, device=device)
+
+    # ONNX doesn't support `torch.Tensor.triu` properly, thus we use this workaround
+    seq_ids = torch.arange(target_length, device=device)
+    mask[:, past_key_values_length:] = seq_ids[:, None] < seq_ids[None, :]
+
+    if past_key_values_length > 0:
+        mask[:, :past_key_values_length] = False
+
+    expanded_mask = mask[None, None, :, :].expand(batch_size, 1, target_length, target_length + past_key_values_length)
+    return expanded_mask
+
+
+def _expand_mask(mask: torch.Tensor, past_key_values_length: int, tgt_len: int) -> torch.BoolTensor:
+    """
+    Copied from transformers.models.falcon.modeling_falcon._expand_mask
+    Expands attention_mask from `[batch_size, seq_length]` to `[batch_size, 1, seq_length, seq_length + past_length]`
+    when past_key_values_length is not 0 or to `[batch_size, 1, seq_length, tgt_len] when past_key_values_length is 0.`
+    """
+    batch_size, total_length = mask.shape
+    if tgt_len > 0:
+        seq_length = tgt_len
+    else:
+        seq_length = total_length - past_key_values_length if past_key_values_length is not None else total_length
+
+    expanded_mask = ~(mask[:, None, None, :].to(torch.bool))
+    return expanded_mask.expand(batch_size, 1, seq_length, total_length)
+
+
+def gaudi_falcon_attention_split_heads(
+    self, fused_qkv: torch.Tensor
+) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+    """
+    Copied from FalconAttention._split_heads https://github.com/huggingface/transformers/blob/v4.33.2/src/transformers/models/falcon/modeling_falcon.py
+    Changing index operation of qkv[:::] to use torch.index_select to work around gradient accuracy issue and improve performance.
+    """
+    if self.new_decoder_architecture:
+        batch, seq_len, _ = fused_qkv.shape
+
+        if self.config.num_attention_heads != self.num_heads:  # When DS divides heads for TP
+            num_heads = self.config.num_attention_heads
+        else:  # When DS not in use
+            num_heads = self.num_heads
+
+        qkv = fused_qkv.view(batch, seq_len, -1, num_heads // self.num_kv_heads + 2, self.head_dim)
+        # query = qkv[:, :, :, :-2]
+        # key = qkv[:, :, :, [-2]]
+        # value = qkv[:, :, :, [-1]]
+        d3 = qkv.shape[3] - 2
+        query = torch.index_select(qkv, 3, index=torch.arange(d3, device=qkv.device))
+        key = torch.index_select(qkv, 3, index=torch.tensor([d3], device=qkv.device))
+        value = torch.index_select(qkv, 3, index=torch.tensor([d3 + 1], device=qkv.device))
+
+        key = torch.broadcast_to(key, query.shape)
+        value = torch.broadcast_to(value, query.shape)
+
+        query, key, value = [x.flatten(2, 3) for x in (query, key, value)]
+        return query, key, value
+    elif not self.multi_query:
+        batch_size, seq_length, three_times_hidden_size = fused_qkv.shape
+        fused_qkv = fused_qkv.view(batch_size, seq_length, self.num_heads, 3, self.head_dim)
+        # TODO : Need to be fixed to use index_select()
+        return fused_qkv[..., 0, :], fused_qkv[..., 1, :], fused_qkv[..., 2, :]
+    else:
+        batch_size, seq_length, three_times_hidden_size = fused_qkv.shape
+        fused_qkv = fused_qkv.view(batch_size, seq_length, self.num_heads + 2, self.head_dim)
+        # return fused_qkv[..., :-2, :], fused_qkv[..., [-2], :], fused_qkv[..., [-1], :]
+        d2 = fused_qkv.shape[2] - 2
+        query = torch.index_select(fused_qkv, 2, index=torch.arange(d2, device=fused_qkv.device))
+        key = torch.index_select(fused_qkv, 2, index=torch.tensor([d2], device=fused_qkv.device))
+        value = torch.index_select(fused_qkv, 2, index=torch.tensor([d2 + 1], device=fused_qkv.device))
+        return query, key, value
+
+
 def gaudi_falcon_attention_forward(
     self,
     hidden_states: torch.Tensor,
     alibi: Optional[torch.Tensor],
     attention_mask: torch.Tensor,
+    position_ids: Optional[torch.LongTensor] = None,
     layer_past: Optional[Tuple[torch.Tensor, torch.Tensor]] = None,
     head_mask: Optional[torch.Tensor] = None,
     use_cache: bool = False,
     output_attentions: bool = False,
     token_idx: Optional[torch.Tensor] = None,
-    position_ids: Optional[torch.LongTensor] = None,
 ):
     """
     Copied from FalconAttention.forward: https://github.com/huggingface/transformers/blob/main/src/transformers/models/falcon/modeling_falcon.py
     The only differences are:
     - add new args token_idx and position_ids
     - replace F.scaled_dot_product_attention with Habana torch's version
     """
@@ -114,30 +196,34 @@
 
     _, kv_length, _ = key_layer.shape
     if use_cache:
         present = (key_layer, value_layer)
     else:
         present = None
 
-    attention_mask_float = (attention_mask * 1.0).masked_fill(attention_mask, float("-1e9")).to(query_layer.dtype)
+    float_min = torch.finfo(query_layer.dtype).min
+    attention_mask_float = (attention_mask * 1.0).masked_fill(attention_mask, float_min).to(query_layer.dtype)
 
     query_layer_ = query_layer.reshape(batch_size, -1, query_length, self.head_dim)
     key_layer_ = key_layer.reshape(batch_size, -1, seq_len, self.head_dim)
     value_layer_ = value_layer.reshape(batch_size, -1, seq_len, self.head_dim)
 
     if alibi is None:
         if output_attentions:
             attention_scores = query_layer_ @ key_layer_.transpose(-1, -2)
             attention_scores /= math.sqrt(self.head_dim)
 
             attention_scores = F.softmax(attention_scores + attention_mask_float, dim=-1, dtype=hidden_states.dtype)
             attn_output = attention_scores @ value_layer_
         else:
             if FusedSDPA:
-                attn_output = FusedSDPA.apply(query_layer_, key_layer_, value_layer_, attention_mask_float, 0.0, False)
+                with sdp_kernel(enable_recompute=False) if SDPContext else contextlib.nullcontext():
+                    attn_output = FusedSDPA.apply(
+                        query_layer_, key_layer_, value_layer_, attention_mask_float, 0.0, False
+                    )
             else:
                 # Workaround util scaled_dot_product_attention support broadcast.
                 if self.training is True and query_layer_.shape != key_layer_.shape:
                     key_layer_ = torch.broadcast_to(key_layer_, query_layer_.shape)
                     value_layer_ = torch.broadcast_to(value_layer_, query_layer_.shape)
                 attn_output = F.scaled_dot_product_attention(
                     query_layer_, key_layer_, value_layer_, attention_mask_float, 0.0, is_causal=False
@@ -200,20 +286,20 @@
 
 
 def gaudi_falcon_decoder_layer_forward(
     self,
     hidden_states: torch.Tensor,
     alibi: Optional[torch.Tensor],
     attention_mask: torch.Tensor,
+    position_ids: Optional[torch.LongTensor] = None,
     layer_past: Optional[Tuple[torch.Tensor, torch.Tensor]] = None,
     head_mask: Optional[torch.Tensor] = None,
     use_cache: bool = False,
     output_attentions: bool = False,
     token_idx: Optional[torch.Tensor] = None,
-    position_ids: Optional[torch.LongTensor] = None,
 ):
     """
     Copied from FalconDecoderLayer.forward: https://github.com/huggingface/transformers/blob/main/src/transformers/models/falcon/modeling_falcon.py
     The only differences are:
     - add new args token_idx and position_ids
     - add token_idx and position_ids into attention inputs
     """
@@ -226,20 +312,20 @@
         attention_layernorm_out = self.input_layernorm(hidden_states)
 
     # Self attention.
     attn_outputs = self.self_attention(
         attention_layernorm_out,
         layer_past=layer_past,
         attention_mask=attention_mask,
+        position_ids=position_ids,
         alibi=alibi,
         head_mask=head_mask,
         use_cache=use_cache,
         output_attentions=output_attentions,
         token_idx=token_idx,
-        position_ids=position_ids,
     )
 
     attention_output = attn_outputs[0]
 
     if not self.config.new_decoder_architecture:
         if self.config.parallel_attn:
             mlp_layernorm_out = attention_layernorm_out
@@ -261,87 +347,14 @@
         outputs = (output,) + outputs
     else:
         outputs = (output,) + outputs[1:]
 
     return outputs  # hidden_states, present, attentions
 
 
-def gaudi_falcon_attention_split_heads(
-    self, fused_qkv: torch.Tensor
-) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
-    """
-    Copied from FalconAttention._split_heads https://github.com/huggingface/transformers/blob/v4.33.2/src/transformers/models/falcon/modeling_falcon.py
-    Changing index operation of qkv[:::] to use torch.index_select to work around gradient accuracy issue and improve performance.
-    """
-    if self.new_decoder_architecture:
-        batch, seq_len, _ = fused_qkv.shape
-        qkv = fused_qkv.view(batch, seq_len, self.num_kv_heads, -1, self.head_dim)
-        # query = qkv[:, :, :, :-2]
-        # key = qkv[:, :, :, [-2]]
-        # value = qkv[:, :, :, [-1]]
-        d3 = qkv.shape[3] - 2
-        query = torch.index_select(qkv, 3, index=torch.arange(d3, device=qkv.device))
-        key = torch.index_select(qkv, 3, index=torch.tensor([d3], device=qkv.device))
-        value = torch.index_select(qkv, 3, index=torch.tensor([d3 + 1], device=qkv.device))
-
-        key = torch.broadcast_to(key, query.shape)
-        value = torch.broadcast_to(value, query.shape)
-
-        query, key, value = [x.flatten(2, 3) for x in (query, key, value)]
-        return query, key, value
-    elif not self.multi_query:
-        batch_size, seq_length, three_times_hidden_size = fused_qkv.shape
-        fused_qkv = fused_qkv.view(batch_size, seq_length, self.num_heads, 3, self.head_dim)
-        # TODO : Need to be fixed to use index_select()
-        return fused_qkv[..., 0, :], fused_qkv[..., 1, :], fused_qkv[..., 2, :]
-    else:
-        batch_size, seq_length, three_times_hidden_size = fused_qkv.shape
-        fused_qkv = fused_qkv.view(batch_size, seq_length, self.num_heads + 2, self.head_dim)
-        # return fused_qkv[..., :-2, :], fused_qkv[..., [-2], :], fused_qkv[..., [-1], :]
-        d2 = fused_qkv.shape[2] - 2
-        query = torch.index_select(fused_qkv, 2, index=torch.arange(d2, device=fused_qkv.device))
-        key = torch.index_select(fused_qkv, 2, index=torch.tensor([d2], device=fused_qkv.device))
-        value = torch.index_select(fused_qkv, 2, index=torch.tensor([d2 + 1], device=fused_qkv.device))
-        return query, key, value
-
-
-def _expand_mask(mask: torch.Tensor, past_key_values_length: int, tgt_len: int) -> torch.BoolTensor:
-    """
-    Copied from transformers.models.falcon.modeling_falcon._expand_mask
-    Expands attention_mask from `[batch_size, seq_length]` to `[batch_size, 1, seq_length, seq_length + past_length]`
-    when past_key_values_length is not 0 or to `[batch_size, 1, seq_length, tgt_len] when past_key_values_length is 0.`
-    """
-    batch_size, total_length = mask.shape
-    if tgt_len > 0:
-        seq_length = tgt_len
-    else:
-        seq_length = total_length - past_key_values_length if past_key_values_length is not None else total_length
-
-    expanded_mask = ~(mask[:, None, None, :].to(torch.bool))
-    return expanded_mask.expand(batch_size, 1, seq_length, total_length)
-
-
-def _make_causal_mask(
-    input_ids_shape: torch.Size, device: torch.device, past_key_values_length: int
-) -> torch.BoolTensor:
-    batch_size, target_length = input_ids_shape
-
-    mask = torch.empty((target_length, target_length + past_key_values_length), dtype=torch.bool, device=device)
-
-    # ONNX doesn't support `torch.Tensor.triu` properly, thus we use this workaround
-    seq_ids = torch.arange(target_length, device=device)
-    mask[:, past_key_values_length:] = seq_ids[:, None] < seq_ids[None, :]
-
-    if past_key_values_length > 0:
-        mask[:, :past_key_values_length] = False
-
-    expanded_mask = mask[None, None, :, :].expand(batch_size, 1, target_length, target_length + past_key_values_length)
-    return expanded_mask
-
-
 class GaudiFalconModel(FalconModel):
     """
     Inherits from FalconModel: https://github.com/huggingface/transformers/blob/main/src/transformers/models/falcon/modeling_falcon.py
     The only differences are:
     - add new args token_idx and position_ids
     - add token_idx and position_ids into decoder inputs
     - set past_key_values_length=0 when token_idx is used (with static input shape)
@@ -385,22 +398,22 @@
         return combined_attention_mask
 
     def forward(
         self,
         input_ids: Optional[torch.LongTensor] = None,
         past_key_values: Optional[Tuple[Tuple[torch.Tensor, torch.Tensor], ...]] = None,
         attention_mask: Optional[torch.Tensor] = None,
+        position_ids: Optional[torch.LongTensor] = None,
         head_mask: Optional[torch.LongTensor] = None,
         inputs_embeds: Optional[torch.LongTensor] = None,
         use_cache: Optional[bool] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
         token_idx: Optional[torch.Tensor] = None,
-        position_ids: Optional[torch.LongTensor] = None,
     ) -> Union[Tuple[torch.Tensor, ...], BaseModelOutputWithPastAndCrossAttentions]:
         output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
         output_hidden_states = (
             output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
         )
         use_cache = use_cache if use_cache is not None else self.config.use_cache
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
@@ -454,14 +467,22 @@
         else:
             attention_mask = attention_mask.to(hidden_states.device)
 
         if self.use_alibi:
             alibi = build_alibi_tensor(attention_mask, self.num_heads, dtype=hidden_states.dtype)
         else:
             alibi = None
+            if position_ids is None:
+                device = input_ids.device if input_ids is not None else inputs_embeds.device
+                position_ids = torch.arange(
+                    past_key_values_length, seq_length + past_key_values_length, dtype=torch.long, device=device
+                )
+                position_ids = position_ids.unsqueeze(0).view(-1, seq_length)
+            else:
+                position_ids = position_ids.view(-1, seq_length).long()
 
         causal_mask = self._prepare_attn_mask(
             attention_mask,
             input_shape=(batch_size, seq_length),
             past_key_values_length=past_key_values_length,
         )
 
@@ -484,27 +505,28 @@
                     return custom_forward
 
                 outputs = torch.utils.checkpoint.checkpoint(
                     create_custom_forward(block),
                     hidden_states,
                     alibi,
                     causal_mask,
+                    position_ids,
                     head_mask[i],
                 )
             else:
                 outputs = block(
                     hidden_states,
                     layer_past=layer_past,
                     attention_mask=causal_mask,
+                    position_ids=position_ids,
                     head_mask=head_mask[i],
                     use_cache=use_cache,
                     output_attentions=output_attentions,
                     alibi=alibi,
                     token_idx=token_idx,
-                    position_ids=position_ids,
                 )
 
             hidden_states = outputs[0]
             if use_cache is True:
                 presents = presents + (outputs[1],)
 
             if output_attentions:
@@ -536,49 +558,89 @@
     The only differences are:
     - add new args token_idx and position_ids
     - add token_idx and position_ids into model inputs
     - from step2 when enable KV cache, slice next_input_ids from input_ids base on the token_idx
     - from step2 when enable KV cache, slice next_position_ids from position_ids base on the token_idx
     """
 
+    def prepare_inputs_for_generation(
+        self,
+        input_ids: torch.LongTensor,
+        past_key_values: Optional[torch.Tensor] = None,
+        attention_mask: Optional[torch.Tensor] = None,
+        position_ids: Optional[torch.Tensor] = None,
+        token_idx: Optional[torch.Tensor] = None,
+        **kwargs,
+    ) -> dict:
+        if past_key_values is not None:
+            if token_idx is not None:
+                input_ids = torch.index_select(input_ids, 1, token_idx - 1)
+            else:
+                input_ids = input_ids[:, -1:]
+
+        # Note: versions of Falcon with alibi do not use position_ids. It is used with RoPE.
+        if (
+            not self.transformer.use_alibi
+            and attention_mask is not None
+            and position_ids is None
+            and token_idx is not None
+        ):
+            # create position_ids on the fly for batch generation
+            position_ids = attention_mask.long().cumsum(-1) - 1
+            position_ids.masked_fill_(attention_mask == 0, 1)
+            if past_key_values:
+                if token_idx is not None:
+                    position_ids = torch.index_select(position_ids, 1, token_idx - 1)
+                else:
+                    position_ids = position_ids[:, -1].unsqueeze(-1)
+
+        return {
+            "input_ids": input_ids,
+            "position_ids": position_ids,
+            "past_key_values": past_key_values,
+            "use_cache": kwargs.get("use_cache"),
+            "attention_mask": attention_mask,
+            "token_idx": token_idx,
+        }
+
     def forward(
         self,
         input_ids: Optional[torch.LongTensor] = None,
         past_key_values: Optional[Tuple[Tuple[torch.Tensor, torch.Tensor], ...]] = None,
         attention_mask: Optional[torch.Tensor] = None,
+        position_ids: Optional[torch.LongTensor] = None,
         head_mask: Optional[torch.Tensor] = None,
         inputs_embeds: Optional[torch.Tensor] = None,
         labels: Optional[torch.Tensor] = None,
         use_cache: Optional[bool] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
         token_idx: Optional[torch.Tensor] = None,
-        position_ids: Optional[torch.LongTensor] = None,
     ) -> Union[Tuple[torch.Tensor], CausalLMOutputWithCrossAttentions]:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size, sequence_length)`, *optional*):
             Labels for language modeling. Note that the labels **are shifted** inside the model, i.e. you can set
             `labels = input_ids` Indices are selected in `[-100, 0, ..., config.vocab_size]` All labels set to `-100`
             are ignored (masked), the loss is only computed for labels in `[0, ..., config.vocab_size]`
         """
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
         transformer_outputs = self.transformer(
             input_ids,
             past_key_values=past_key_values,
             attention_mask=attention_mask,
+            position_ids=position_ids,
             head_mask=head_mask,
             inputs_embeds=inputs_embeds,
             use_cache=use_cache,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
             token_idx=token_idx,
-            position_ids=position_ids,
         )
         hidden_states = transformer_outputs[0]
 
         lm_logits = self.lm_head(hidden_states)
 
         loss = None
         if labels is not None:
@@ -599,41 +661,7 @@
         return CausalLMOutputWithCrossAttentions(
             loss=loss,
             logits=lm_logits,
             past_key_values=transformer_outputs.past_key_values,
             hidden_states=transformer_outputs.hidden_states,
             attentions=transformer_outputs.attentions,
         )
-
-    def prepare_inputs_for_generation(
-        self,
-        input_ids: torch.LongTensor,
-        past_key_values: Optional[torch.Tensor] = None,
-        attention_mask: Optional[torch.Tensor] = None,
-        token_idx: Optional[torch.Tensor] = None,
-        **kwargs,
-    ) -> dict:
-        if past_key_values is not None:
-            if token_idx is not None:
-                input_ids = torch.index_select(input_ids, 1, token_idx - 1)
-            else:
-                input_ids = input_ids[:, -1:]
-
-        position_ids = kwargs.get("position_ids", None)
-        if attention_mask is not None and position_ids is None and token_idx is not None:
-            # create position_ids on the fly for batch generation
-            position_ids = attention_mask.long().cumsum(-1) - 1
-            position_ids.masked_fill_(attention_mask == 0, 1)
-            if past_key_values:
-                if token_idx is not None:
-                    position_ids = torch.index_select(position_ids, 1, token_idx - 1)
-                else:
-                    position_ids = position_ids[:, -1].unsqueeze(-1)
-
-        return {
-            "input_ids": input_ids,
-            "past_key_values": past_key_values,
-            "use_cache": kwargs.get("use_cache"),
-            "attention_mask": attention_mask,
-            "token_idx": token_idx,
-            "position_ids": position_ids,
-        }
```

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/models/gpt2/modeling_gpt2.py` & `optimum-habana-1.9.0/optimum/habana/transformers/models/gpt2/modeling_gpt2.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 import torch
 from torch.nn import CrossEntropyLoss
 from transformers.modeling_outputs import BaseModelOutputWithPastAndCrossAttentions, CausalLMOutputWithCrossAttentions
 from transformers.models.gpt2.modeling_gpt2 import GPT2LMHeadModel, logger
 from transformers.pytorch_utils import Conv1D, find_pruneable_heads_and_indices, prune_conv1d_layer
 
-from ....utils import get_device_name
-
 
 class GaudiGPT2Attention(torch.nn.Module):
     """
     Copied from GPT2Attention: https://github.com/huggingface/transformers/blob/main/src/transformers/models/gpt2/modeling_gpt2.py
     The only differences are:
     - `self.bias` is a torch.uint8 and not a torch.bool
     - it is casted to bool before being used in torch.where
@@ -262,23 +260,15 @@
     """
     Copied from GPT2Block.forward: https://github.com/huggingface/transformers/blob/main/src/transformers/models/gpt2/modeling_gpt2.py
     The only differences are:
     - add new args token_idx
     """
 
     residual = hidden_states
-
-    # TODO: remove this workaround when SynapseAI 1.13 is released
-    if not self.ln_1.training and get_device_name() == "gaudi2" and hidden_states.shape[:-1] == torch.Size([1, 1]):
-        # Change to 1,2,1600 and back to 1,1,1600
-        hidden_states = hidden_states.repeat([1, 2, 1])  # this changes the shape 1x2x1600
-        hidden_states = self.ln_1(hidden_states)
-        hidden_states = hidden_states[:, :1, :]
-    else:
-        hidden_states = self.ln_1(hidden_states)
+    hidden_states = self.ln_1(hidden_states)
 
     attn_outputs = self.attn(
         hidden_states,
         layer_past=layer_past,
         attention_mask=attention_mask,
         head_mask=head_mask,
         use_cache=use_cache,
@@ -309,23 +299,15 @@
         )
         attn_output = cross_attn_outputs[0]
         # residual connection
         hidden_states = residual + attn_output
         outputs = outputs + cross_attn_outputs[2:]  # add cross attentions if we output attention weights
 
     residual = hidden_states
-
-    # TODO: remove this workaround when SynapseAI 1.13 is released
-    if not self.ln_2.training and get_device_name() == "gaudi2" and hidden_states.shape[:-1] == torch.Size([1, 1]):
-        # Change to 1,2,1600 and back to 1,1,1600
-        hidden_states = hidden_states.repeat([1, 2, 1])  # this changes the shape 1x2x1600
-        hidden_states = self.ln_2(hidden_states)
-        hidden_states = hidden_states[:, :1, :]
-    else:
-        hidden_states = self.ln_2(hidden_states)
+    hidden_states = self.ln_2(hidden_states)
 
     feed_forward_hidden_states = self.mlp(hidden_states)
     # residual connection
     hidden_states = residual + feed_forward_hidden_states
 
     if use_cache:
         outputs = (hidden_states,) + outputs
@@ -351,15 +333,15 @@
     output_hidden_states: Optional[bool] = None,
     return_dict: Optional[bool] = None,
     token_idx: Optional[torch.Tensor] = None,
 ) -> Union[Tuple, BaseModelOutputWithPastAndCrossAttentions]:
     """
     Copied from GPT2Model.forward: https://github.com/huggingface/transformers/blob/main/src/transformers/models/gpt2/modeling_gpt2.py
     The only differences are:
-    - disable HMP cast for attention_mask
+    - disable autocast for attention_mask
     - add new args token_idx
     """
 
     output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
     output_hidden_states = (
         output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
     )
@@ -410,17 +392,15 @@
         # Since attention_mask is 1.0 for positions we want to attend and 0.0 for
         # masked positions, this operation will create a tensor which is 0.0 for
         # positions we want to attend and the dtype's smallest value for masked positions.
         # Since we are adding it to the raw scores before the softmax, this is
         # effectively the same as removing these entirely.
         attention_mask = attention_mask.to(dtype=self.dtype)  # fp16 compatibility
 
-        from habana_frameworks.torch.hpex import hmp
-
-        with hmp.disable_casts(), torch.autocast(enabled=False, device_type="hpu"):
+        with torch.autocast(enabled=False, device_type="hpu"):
             attention_mask = (1.0 - attention_mask) * torch.finfo(self.dtype).min
 
     # If a 2D or 3D attention mask is provided for the cross-attention
     # we need to make broadcastable to [batch_size, num_heads, seq_length, seq_length]
     if self.config.add_cross_attention and encoder_hidden_states is not None:
         encoder_batch_size, encoder_sequence_length, _ = encoder_hidden_states.size()
         encoder_hidden_shape = (encoder_batch_size, encoder_sequence_length)
@@ -517,22 +497,15 @@
 
         # Model Parallel: If it's the last layer for that device, put things on the next device
         if self.model_parallel:
             for k, v in self.device_map.items():
                 if i == v[-1] and "cuda:" + str(k) != self.last_device:
                     hidden_states = hidden_states.to("cuda:" + str(k + 1))
 
-    # TODO: remove this workaround when SynapseAI 1.13 is released
-    if not self.ln_f.training and get_device_name() == "gaudi2" and hidden_states.shape[:-1] == torch.Size([1, 1]):
-        # Change to 1,2,1600 and back to 1,1,1600
-        hidden_states = hidden_states.repeat([1, 2, 1])  # this changes the shape 1x2x1600
-        hidden_states = self.ln_f(hidden_states)
-        hidden_states = hidden_states[:, :1, :]
-    else:
-        hidden_states = self.ln_f(hidden_states)
+    hidden_states = self.ln_f(hidden_states)
 
     hidden_states = hidden_states.view(output_shape)
     # Add last hidden state
     if output_hidden_states:
         all_hidden_states = all_hidden_states + (hidden_states,)
 
     if not return_dict:
```

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/models/gpt_bigcode/modeling_gpt_bigcode.py` & `optimum-habana-1.9.0/optimum/habana/transformers/models/gpt_bigcode/modeling_gpt_bigcode.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,17 +348,17 @@
     def prepare_inputs_for_generation(
         self, input_ids, past_key_values=None, inputs_embeds=None, token_idx=None, **kwargs
     ):
         token_type_ids = kwargs.get("token_type_ids", None)
         # only last token for inputs_ids if past is defined in kwargs
         if past_key_values:
             if token_idx is not None:
-                input_ids = torch.index_select(input_ids, 1, token_idx - 1).unsqueeze(-1)
+                input_ids = torch.index_select(input_ids, 1, token_idx - 1)
                 if token_type_ids is not None:
-                    token_type_ids = torch.index_select(token_type_ids, 1, token_idx - 1).unsqueeze(-1)
+                    token_type_ids = torch.index_select(token_type_ids, 1, token_idx - 1)
             else:
                 input_ids = input_ids[:, -1].unsqueeze(-1)
                 if token_type_ids is not None:
                     token_type_ids = token_type_ids[:, -1].unsqueeze(-1)
 
         attention_mask = kwargs.get("attention_mask", None)
         position_ids = kwargs.get("position_ids", None)
```

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/models/gpt_neox/modeling_gpt_neox.py` & `optimum-habana-1.9.0/optimum/habana/transformers/models/gpt_neox/modeling_gpt_neox.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 from typing import Optional, Tuple, Union
 
 import torch
 from torch.nn import CrossEntropyLoss
 from transformers.modeling_outputs import BaseModelOutputWithPast, CausalLMOutputWithPast
 from transformers.models.gpt_neox.modeling_gpt_neox import GPTNeoXForCausalLM, apply_rotary_pos_emb, logger
 
-from ....utils import get_device_name
 
-
-# TODO: remove this workaround when FusedRoPE properly works on Gaudi
-if get_device_name() == "gaudi2":
-    try:
-        from habana_frameworks.torch.hpex.kernels import RotaryPosEmbeddingHelperV2 as FusedRoPE
-    except ImportError:
-        print("Not using HPU fused kernel for apply_rotary_pos_emb")
-        FusedRoPE = None
-else:
+try:
+    from habana_frameworks.torch.hpex.kernels import RotaryPosEmbeddingHelperV2 as FusedRoPE
+except ImportError:
+    print("Not using HPU fused kernel for apply_rotary_pos_emb")
     FusedRoPE = None
 
 
 def gaudi_gpt_neox_attention_forward(
     self,
     hidden_states: torch.FloatTensor,
     attention_mask: torch.FloatTensor,
```

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/models/gptj/modeling_gptj.py` & `optimum-habana-1.9.0/optimum/habana/transformers/models/gptj/modeling_gptj.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,16 +39,14 @@
         self.scale_attn = torch.sqrt(torch.tensor(self.head_dim, dtype=torch.float32)).to(torch.get_default_dtype())
 
         self.k_proj = nn.Linear(self.embed_dim, self.embed_dim, bias=False)
         self.v_proj = nn.Linear(self.embed_dim, self.embed_dim, bias=False)
         self.q_proj = nn.Linear(self.embed_dim, self.embed_dim, bias=False)
         self.out_proj = nn.Linear(self.embed_dim, self.embed_dim, bias=False)
         self.rotary_dim = config.rotary_dim
-        pos_embd_dim = self.rotary_dim or self.embed_dim
-        self.embed_positions = create_sinusoidal_positions(max_positions, pos_embd_dim)
 
     def _split_heads(self, tensor, num_attention_heads, attn_head_size, rotary):
         """
         Splits hidden dim into attn_head_size and num_attention_heads
         """
         new_shape = tensor.size()[:-1] + (num_attention_heads, attn_head_size)
         tensor = tensor.view(new_shape)
@@ -82,25 +80,24 @@
         attention_mask=None,
         head_mask=None,
     ):
         # compute causal mask from causal mask buffer
         query_length, key_length = query.size(-2), key.size(-2)
         causal_mask = self.bias[:, :, key_length - query_length : key_length, :key_length].bool()
 
-        # Keep the attention weights computation in fp32 to avoid overflow issues
-        query = query.to(torch.float32).contiguous()
-        key = key.to(torch.float32).contiguous()
+        query = query.contiguous()
+        key = key.contiguous()
         value = value.contiguous()
 
         attn_weights = torch.matmul(query, key.transpose(-1, -2))
 
         mask_value = torch.finfo(attn_weights.dtype).min
         # Need to be a tensor, otherwise we get error: `RuntimeError: expected scalar type float but found double`.
         # Need to be on the same device, otherwise `RuntimeError: ..., x and y to be on the same device`
-        mask_value = torch.tensor(mask_value, dtype=attn_weights.dtype).to(attn_weights.device)
+        mask_value = torch.tensor(mask_value, dtype=attn_weights.dtype, device=attn_weights.device)
         attn_weights = torch.where(causal_mask, attn_weights, mask_value)
 
         attn_weights = attn_weights / self.scale_attn
 
         if attention_mask is not None:
             # Apply the attention mask
             attn_weights = attn_weights + attention_mask
@@ -113,74 +110,64 @@
         if head_mask is not None:
             attn_weights = attn_weights * head_mask
 
         attn_output = torch.matmul(attn_weights, value)
 
         return attn_output, attn_weights
 
-    def _get_embed_positions(self, position_ids):
-        embed_positions = self.embed_positions
-        if embed_positions.device != position_ids.device:
-            embed_positions = embed_positions.to(position_ids.device)
-            self.embed_positions = embed_positions
-        return embed_positions.repeat(position_ids.shape[0], 1, 1)
-
     def forward(
         self,
         hidden_states: torch.FloatTensor,
         layer_past: Optional[Tuple[torch.Tensor]] = None,
         attention_mask: Optional[torch.FloatTensor] = None,
         position_ids: Optional[torch.LongTensor] = None,
         head_mask: Optional[torch.FloatTensor] = None,
         use_cache: Optional[bool] = False,
         output_attentions: Optional[bool] = False,
         token_idx: Optional[torch.Tensor] = None,
+        sin: Optional[torch.Tensor] = None,
+        cos: Optional[torch.Tensor] = None,
     ) -> Union[
         Tuple[torch.Tensor, Tuple[torch.Tensor]],
         Optional[Tuple[torch.Tensor, Tuple[torch.Tensor], Tuple[torch.Tensor, ...]]],
     ]:
         """
         Copied from GPTJAttention.forward: https://github.com/huggingface/transformers/blob/main/src/transformers/models/gptj/modeling_gptj.py
         The only differences are:
         - add new args token_idx
         - remove is_torch_fx_proxy
         - optimize KV cache
+        - pass sin and cos from upper level as they are identical for each attn block
         """
         query = self.q_proj(hidden_states)
         key = self.k_proj(hidden_states)
         value = self.v_proj(hidden_states)
 
         query = self._split_heads(query, self.num_attention_heads, self.head_dim, True).contiguous()
         key = self._split_heads(key, self.num_attention_heads, self.head_dim, True).contiguous()
         value = self._split_heads(value, self.num_attention_heads, self.head_dim, False).contiguous()
 
-        embed_positions = self._get_embed_positions(position_ids)
-
-        repeated_position_ids = position_ids.unsqueeze(-1).repeat(1, 1, embed_positions.shape[-1])
-        sincos = torch.gather(embed_positions, 1, repeated_position_ids)
-        sin, cos = torch.split(sincos, sincos.shape[-1] // 2, dim=-1)
-
         if self.rotary_dim is not None:
             k_rot = key[:, :, :, : self.rotary_dim]
             k_pass = key[:, :, :, self.rotary_dim :]
 
             q_rot = query[:, :, :, : self.rotary_dim]
             q_pass = query[:, :, :, self.rotary_dim :]
-
-            k_rot = apply_rotary_pos_emb(k_rot, sin, cos)
-            q_rot = apply_rotary_pos_emb(q_rot, sin, cos)
+            # Note: it appears that if we use bf16 RoPE(whether use fused kernel or not), there could be acc issue, hence use fp32 RoPE here Fused kernel feasibility needs to be confirmed in the future
+            k_rot = apply_rotary_pos_emb(k_rot.to(torch.float32), sin, cos).to(torch.bfloat16)
+            q_rot = apply_rotary_pos_emb(q_rot.to(torch.float32), sin, cos).to(torch.bfloat16)
 
             key = torch.cat([k_rot, k_pass], dim=-1)
             query = torch.cat([q_rot, q_pass], dim=-1)
         else:
-            key = apply_rotary_pos_emb(key, sin, cos)
-            query = apply_rotary_pos_emb(query, sin, cos)
+            key = apply_rotary_pos_emb(key.to(torch.float32), sin, cos).to(torch.bfloat16)
+            query = apply_rotary_pos_emb(query.to(torch.float32), sin, cos).to(torch.bfloat16)
 
-        key = key.permute(0, 2, 1, 3)
-        query = query.permute(0, 2, 1, 3)
+        key = key.permute(0, 2, 1, 3).contiguous()
+        query = query.permute(0, 2, 1, 3).contiguous()
 
         if layer_past is not None:
             past_key = layer_past[0]
             past_value = layer_past[1]
 
             if token_idx is not None:
                 past_key.index_copy_(2, token_idx - 1, key)
@@ -216,31 +203,36 @@
     layer_past: Optional[Tuple[torch.Tensor]] = None,
     attention_mask: Optional[torch.FloatTensor] = None,
     position_ids: Optional[torch.LongTensor] = None,
     head_mask: Optional[torch.FloatTensor] = None,
     use_cache: Optional[bool] = False,
     output_attentions: Optional[bool] = False,
     token_idx: Optional[torch.Tensor] = None,
+    sin: Optional[torch.Tensor] = None,
+    cos: Optional[torch.Tensor] = None,
 ) -> Union[Tuple[torch.Tensor], Optional[Tuple[torch.Tensor, Tuple[torch.FloatTensor, ...]]]]:
     """
     Copied from GPTJBlock.forward: https://github.com/huggingface/transformers/blob/main/src/transformers/models/gptj/modeling_gptj.py
     The only differences are:
     - add new args token_idx
+    - pass sin and cos from upper level as they are identical for each attn block
     """
     residual = hidden_states
     hidden_states = self.ln_1(hidden_states)
     attn_outputs = self.attn(
         hidden_states=hidden_states,
         layer_past=layer_past,
         attention_mask=attention_mask,
         position_ids=position_ids,
         head_mask=head_mask,
         use_cache=use_cache,
         output_attentions=output_attentions,
         token_idx=token_idx,
+        sin=sin,
+        cos=cos,
     )
     attn_output = attn_outputs[0]  # output_attn: a, present, (attentions)
     outputs = attn_outputs[1:]
 
     feed_forward_hidden_states = self.mlp(hidden_states)
     hidden_states = attn_output + feed_forward_hidden_states + residual
 
@@ -262,19 +254,22 @@
     head_mask: Optional[torch.FloatTensor] = None,
     inputs_embeds: Optional[torch.FloatTensor] = None,
     use_cache: Optional[bool] = None,
     output_attentions: Optional[bool] = None,
     output_hidden_states: Optional[bool] = None,
     return_dict: Optional[bool] = None,
     token_idx: Optional[torch.Tensor] = None,
+    sin: Optional[torch.Tensor] = None,
+    cos: Optional[torch.Tensor] = None,
 ) -> Union[Tuple, BaseModelOutputWithPast]:
     """
     Copied from GPTJModel.forward: https://github.com/huggingface/transformers/blob/main/src/transformers/models/gptj/modeling_gptj.py
     The only differences are:
     - add new args token_idx
+    - pass sin and cos from upper level as they are identical for each attn block
     """
     output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
     output_hidden_states = (
         output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
     )
     use_cache = use_cache if use_cache is not None else self.config.use_cache
     return_dict = return_dict if return_dict is not None else self.config.use_return_dict
@@ -355,14 +350,30 @@
                 "`use_cache=True` is incompatible with gradient checkpointing. Setting `use_cache=False`..."
             )
             use_cache = False
 
     presents = () if use_cache else None
     all_self_attentions = () if output_attentions else None
     all_hidden_states = () if output_hidden_states else None
+
+    # replace original `_get_embed_positions` method and sin cos calculation in the attn block here to improve perf
+    rotary_dim = self.config.rotary_dim
+    embed_dim = self.config.hidden_size
+    pos_embd_dim = rotary_dim or embed_dim
+    max_positions = self.config.max_position_embeddings
+    embed_positions = create_sinusoidal_positions(max_positions, pos_embd_dim).to(torch.bfloat16)
+    embed_positions = embed_positions.repeat(position_ids.shape[0], 1, 1)
+    if embed_positions.device != position_ids.device:
+        embed_positions = embed_positions.to(position_ids.device)
+    repeated_position_ids = position_ids.unsqueeze(-1).repeat(1, 1, embed_positions.shape[-1])
+    sincos = torch.gather(embed_positions, 1, repeated_position_ids)
+    sin, cos = torch.split(sincos, sincos.shape[-1] // 2, dim=-1)
+    sin = sin.contiguous()
+    cos = cos.contiguous()
+
     for i, (block, layer_past) in enumerate(zip(self.h, past_key_values)):
         # Model parallel
         if self.model_parallel:
             torch.cuda.set_device(hidden_states.device)
             # Ensure layer_past is on same device as hidden_states (might not be correct)
             if layer_past is not None:
                 layer_past = tuple(past_state.to(hidden_states.device) for past_state in layer_past)
@@ -397,14 +408,16 @@
                 layer_past=layer_past,
                 attention_mask=attention_mask,
                 position_ids=position_ids,
                 head_mask=head_mask[i],
                 use_cache=use_cache,
                 output_attentions=output_attentions,
                 token_idx=token_idx,
+                sin=sin,
+                cos=cos,
             )
 
         hidden_states = outputs[0]
         if use_cache is True:
             presents = presents + (outputs[1],)
 
         if output_attentions:
```

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/models/llama/modeling_llama.py` & `optimum-habana-1.9.0/optimum/habana/transformers/models/llama/modeling_llama.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,43 +10,40 @@
     LlamaDecoderLayer,
     LlamaForCausalLM,
     LlamaModel,
     apply_rotary_pos_emb,
     logger,
 )
 
-from ....utils import get_device_name
 
-
-# TODO: remove this workaround when FusedRoPE properly works on Gaudi
-if get_device_name() == "gaudi2":
-    try:
-        from habana_frameworks.torch.hpex.kernels import RotaryPosEmbeddingHelperV2 as FusedRoPE
-    except ImportError:
-        print("Not using HPU fused kernel for apply_rotary_pos_emb")
-        FusedRoPE = None
-else:
+try:
+    from habana_frameworks.torch.hpex.kernels import RotaryPosEmbeddingHelperV2 as FusedRoPE
+except ImportError:
+    print("Not using HPU fused kernel for apply_rotary_pos_emb")
     FusedRoPE = None
 
 try:
     from habana_frameworks.torch.hpex.normalization import FusedRMSNorm as FusedRMSNorm
 except ImportError:
     print("Not using HPU fused kernel for RMSNorm")
     FusedRMSNorm = None
 
 
-def update(prev, cur, dim, idx):
+def update(prev, cur, dim, idx, inp_seq_len):
     orig_cur = cur
+    cur = cur.to(dtype=prev.dtype)
     if cur.shape[2] > 1 and cur.shape[2] <= prev.shape[2]:
         # Initialize
-        prev[:, :, :idx, :].copy_(cur)
+        prev[:, :, :inp_seq_len, :].copy_(cur)
         return orig_cur
     assert cur.shape[2] == 1, f"Cannot update kv-cache. Unsupported shapes. prev:{prev.shape} cur:{cur.shape}"
     if idx is not None:
-        return prev.index_copy_(dim, idx - 1, cur)
+        prev.index_copy_(dim, idx - 1, cur)
+        prev_cast = prev.to(orig_cur.dtype)
+        return prev_cast
     else:
         return torch.cat((prev, cur), dim=dim)
 
 
 def gaudi_llama_rmsnorm_forward(self, hidden_states):
     """
     Copied from LlamaRMSNorm.forward: https://github.com/huggingface/transformers/blob/main/src/transformers/models/llama/modeling_llama.py
@@ -82,27 +79,42 @@
 
 class GaudiLlamaAttention(LlamaAttention):
     def __init__(self, config: LlamaConfig):
         super().__init__(config)
 
         self.past_key = None
         self.past_value = None
+        self.inp_seq_len = -1
 
-    def allocate_kv_cache(self, batch_size, seq_len):
-        key_shape = (batch_size, self.num_key_value_heads, seq_len, self.head_dim)
-        value_shape = (batch_size, self.num_key_value_heads, seq_len, self.head_dim)
+    def allocate_kv_cache(self, batch_size, max_seq_len, inp_seq_len, kv_cache_fp8):
+        key_shape = (batch_size, self.num_key_value_heads, max_seq_len, self.head_dim)
+        value_shape = (batch_size, self.num_key_value_heads, max_seq_len, self.head_dim)
         if self.past_key is None or self.past_key.shape != key_shape:
+            self.inp_seq_len = inp_seq_len
             device = self.k_proj.weight.device
             dtype = self.k_proj.weight.dtype
+            if kv_cache_fp8:
+                dtype = torch.float8_e4m3fn
             self.past_key = torch.zeros(key_shape, dtype=dtype, device=device)
             self.past_value = torch.zeros(value_shape, dtype=dtype, device=device)
         else:
+            assert (
+                self.inp_seq_len == inp_seq_len
+            ), f"inp_seq_len must be the same. self.inp_seq_len:{self.inp_seq_len} inp_seq_len:{inp_seq_len}"
             self.past_key.fill_(0)
             self.past_value.fill_(0)
 
+    def update_sincos_cache(self, seq_len):
+        # Call rotary emb forward() to update cos/sin cache when infering more than self.max_position_embeddings
+        # This helps in avoiding creation of these caches during actual model forward pass and
+        # reduce memory consumption and improve performance.
+        if seq_len > self.max_position_embeddings:
+            self.max_position_embeddings = seq_len
+            _, _ = self.rotary_emb(self.k_proj.weight, seq_len=seq_len)
+
     def reorder(self, tensor, beam_idx, dim_a, dim_b):
         updated = tensor.index_select(0, beam_idx)
         tensor.copy_(updated)
 
     def reorder_kv_cache(self, beam_idx: torch.LongTensor):
         if self.past_key is None:
             return (None, None)
@@ -178,26 +190,25 @@
             # reuse k, v, self_attention
             if reuse_cache:
                 past_key = self.past_key
                 past_value = self.past_value
             else:
                 past_key = past_key_value[0]
                 past_value = past_key_value[1]
-            key_states = update(past_key, key_states, 2, token_idx)
-            value_states = update(past_value, value_states, 2, token_idx)
+            key_states = update(past_key, key_states, 2, token_idx, self.inp_seq_len)
+            value_states = update(past_value, value_states, 2, token_idx, self.inp_seq_len)
 
         if use_cache:
             if reuse_cache:
                 past_key_value = (self.past_key.shape, self.past_value.shape)
             else:
                 past_key_value = (key_states.contiguous(), value_states.contiguous())
         else:
             past_key_value = None
 
-        # repeat k/v heads if n_kv_heads < n_heads
         key_states = gaudi_llama_repeat_kv(key_states, self.num_key_value_groups)
         value_states = gaudi_llama_repeat_kv(value_states, self.num_key_value_groups)
 
         attn_weights = torch.matmul(query_states, key_states.transpose(2, 3)) / math.sqrt(self.head_dim)
 
         if attn_weights.size() != (bsz, self.num_heads, q_len, kv_seq_len):
             raise ValueError(
@@ -225,14 +236,15 @@
         if attn_output.size() != (bsz, self.num_heads, q_len, self.head_dim):
             raise ValueError(
                 f"`attn_output` should be of size {(bsz, self.num_heads, q_len, self.head_dim)}, but is"
                 f" {attn_output.size()}"
             )
 
         attn_output = attn_output.transpose(1, 2).contiguous()
+
         attn_output = attn_output.reshape(bsz, q_len, self.hidden_size)
 
         if self.config.pretraining_tp > 1:
             attn_output = attn_output.split(self.hidden_size // self.config.pretraining_tp, dim=2)
             o_proj_slices = self.o_proj.weight.split(self.hidden_size // self.config.pretraining_tp, dim=1)
             attn_output = sum([F.linear(attn_output[i], o_proj_slices[i]) for i in range(self.config.pretraining_tp)])
         else:
@@ -241,20 +253,23 @@
         if not output_attentions:
             attn_weights = None
 
         return attn_output, attn_weights, past_key_value
 
 
 class GaudiLlamaDecoderLayer(LlamaDecoderLayer):
-    def allocate_kv_cache(self, batch_size, seq_len):
-        self.self_attn.allocate_kv_cache(batch_size, seq_len)
+    def allocate_kv_cache(self, batch_size, max_seq_len, inp_seq_len, kv_cache_fp8):
+        self.self_attn.allocate_kv_cache(batch_size, max_seq_len, inp_seq_len, kv_cache_fp8)
 
     def reorder_kv_cache(self, beam_idx: torch.LongTensor):
         return self.self_attn.reorder_kv_cache(beam_idx)
 
+    def update_sincos_cache(self, seq_len):
+        self.self_attn.update_sincos_cache(seq_len)
+
     def forward(
         self,
         hidden_states: torch.Tensor,
         attention_mask: Optional[torch.Tensor] = None,
         position_ids: Optional[torch.LongTensor] = None,
         past_key_value: Optional[Tuple[torch.Tensor]] = None,
         output_attentions: Optional[bool] = False,
@@ -301,21 +316,25 @@
         if use_cache:
             outputs += (present_key_value,)
 
         return outputs
 
 
 class GaudiLlamaModel(LlamaModel):
-    def allocate_kv_cache(self, batch_size, seq_len):
+    def allocate_kv_cache(self, batch_size, max_seq_len, inp_seq_len, kv_cache_fp8):
         for layer in self.layers:
-            layer.allocate_kv_cache(batch_size, seq_len)
+            layer.allocate_kv_cache(batch_size, max_seq_len, inp_seq_len, kv_cache_fp8)
 
     def reorder_kv_cache(self, beam_idx: torch.LongTensor):
         return tuple(layer.reorder_kv_cache(beam_idx) for layer in self.layers)
 
+    def update_sincos_cache(self, seq_len):
+        for layer in self.layers:
+            layer.update_sincos_cache(seq_len)
+
     def forward(
         self,
         input_ids: torch.LongTensor = None,
         attention_mask: Optional[torch.Tensor] = None,
         position_ids: Optional[torch.LongTensor] = None,
         past_key_values: Optional[List[torch.FloatTensor]] = None,
         inputs_embeds: Optional[torch.FloatTensor] = None,
@@ -340,21 +359,21 @@
         )
         use_cache = use_cache if use_cache is not None else self.config.use_cache
 
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
         # retrieve input_ids and inputs_embeds
         if input_ids is not None and inputs_embeds is not None:
-            raise ValueError("You cannot specify both decoder_input_ids and decoder_inputs_embeds at the same time")
+            raise ValueError("You cannot specify both input_ids and inputs_embeds at the same time")
         elif input_ids is not None:
             batch_size, seq_length = input_ids.shape
         elif inputs_embeds is not None:
             batch_size, seq_length, _ = inputs_embeds.shape
         else:
-            raise ValueError("You have to specify either decoder_input_ids or decoder_inputs_embeds")
+            raise ValueError("You have to specify either input_ids or inputs_embeds")
 
         seq_length_with_past = seq_length
         past_key_values_length = 0
 
         if past_key_values is not None:
             if reuse_cache:
                 past_key_values_length = past_key_values[0][0][2]
@@ -403,23 +422,20 @@
             past_key_value = past_key_values[idx] if past_key_values is not None else None
 
             if self.gradient_checkpointing and self.training:
 
                 def create_custom_forward(module):
                     def custom_forward(*inputs):
                         # None for past_key_value
-                        return module(*inputs, past_key_value, output_attentions)
+                        return module(*inputs, past_key_value, output_attentions, attn_softmax_bf16=attn_softmax_bf16)
 
                     return custom_forward
 
                 layer_outputs = torch.utils.checkpoint.checkpoint(
-                    create_custom_forward(decoder_layer),
-                    hidden_states,
-                    attention_mask,
-                    position_ids,
+                    create_custom_forward(decoder_layer), hidden_states, attention_mask, position_ids
                 )
             else:
                 layer_outputs = decoder_layer(
                     hidden_states,
                     attention_mask=attention_mask,
                     position_ids=position_ids,
                     past_key_value=past_key_value,
@@ -463,20 +479,23 @@
     - add token_idx into model_inputs
     - from step2 when enable KV cache, slice next_input_ids from input_ids base on the token_idx
     - from step2 when enable KV cache, slice next_position_ids from position_ids base on the token_idx
     - add new args attn_softmax_bf16
     - add new args reuse_cache
     """
 
-    def allocate_kv_cache(self, batch_size, seq_len):
-        self.model.allocate_kv_cache(batch_size, seq_len)
+    def allocate_kv_cache(self, batch_size, max_seq_len, inp_seq_len, kv_cache_fp8):
+        self.model.allocate_kv_cache(batch_size, max_seq_len, inp_seq_len, kv_cache_fp8)
 
     def reorder_kv_cache(self, beam_idx: torch.LongTensor):
         return self.model.reorder_kv_cache(beam_idx)
 
+    def update_sincos_cache(self, seq_len):
+        self.model.update_sincos_cache(seq_len)
+
     def forward(
         self,
         input_ids: torch.LongTensor = None,
         attention_mask: Optional[torch.Tensor] = None,
         position_ids: Optional[torch.LongTensor] = None,
         past_key_values: Optional[List[torch.FloatTensor]] = None,
         inputs_embeds: Optional[torch.FloatTensor] = None,
```

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/models/modeling_all_models.py` & `optimum-habana-1.9.0/optimum/habana/transformers/models/modeling_all_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import torch
 from transformers.modeling_utils import ModuleUtilsMixin
 
 
 def gaudi_invert_attention_mask(self, encoder_attention_mask: torch.Tensor) -> torch.Tensor:
     """
     Same as https://github.com/huggingface/transformers/blob/a9eee2ffecc874df7dd635b2c6abb246fdb318cc/src/transformers/modeling_utils.py#L640
-    except that HMP is disabled for computing:
+    except that mixed precision is disabled for computing:
         encoder_extended_attention_mask = (1.0 - encoder_extended_attention_mask) * torch.finfo(self.dtype).min
     """
     if encoder_attention_mask.dim() == 3:
         encoder_extended_attention_mask = encoder_attention_mask[:, None, :, :]
     if encoder_attention_mask.dim() == 2:
         encoder_extended_attention_mask = encoder_attention_mask[:, None, None, :]
     # T5 has a mask that can compare sequence ids, we can simulate this here with this transposition
@@ -47,15 +47,15 @@
 
 
 def gaudi_get_extended_attention_mask(
     self, attention_mask: torch.Tensor, input_shape: Tuple[int], device: torch.device = None, dtype: torch.float = None
 ) -> torch.Tensor:
     """
     Same as https://github.com/huggingface/transformers/blob/a9eee2ffecc874df7dd635b2c6abb246fdb318cc/src/transformers/modeling_utils.py#L692
-    except that HMP is disabled for computing:
+    except that mixed precision is disabled for computing:
         extended_attention_mask = (1.0 - extended_attention_mask) * torch.finfo(dtype).min
     """
     if dtype is None:
         dtype = self.dtype
 
     if not (attention_mask.dim() == 2 and self.config.is_decoder):
         # show warning only if it won't be shown in `create_extended_attention_mask_for_decoder`
```

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/models/mpt/modeling_mpt.py` & `optimum-habana-1.9.0/optimum/habana/transformers/models/mpt/modeling_mpt.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/models/opt/modeling_opt.py` & `optimum-habana-1.9.0/optimum/habana/transformers/models/opt/modeling_opt.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     output_attentions: bool = False,
     token_idx: Optional[torch.Tensor] = None,
 ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
     """
     Copied from OPTAttention.forward: https://github.com/huggingface/transformers/blob/main/src/transformers/models/opt/modeling_opt.py
     The only differences are:
     - add new args token_idx
-    - disable HMP for attention softmax
     - optimize KV cache
     """
     # if key_value_states are provided this layer is used as a cross-attention layer
     # for the decoder
     is_cross_attention = key_value_states is not None
 
     bsz, tgt_len, _ = hidden_states.size()
@@ -114,18 +113,15 @@
             )
         attn_weights = attn_weights.view(bsz, self.num_heads, tgt_len, src_len) + attention_mask
         attn_weights = torch.max(
             attn_weights, torch.tensor(torch.finfo(attn_weights.dtype).min, device=attn_weights.device)
         )
         attn_weights = attn_weights.view(bsz * self.num_heads, tgt_len, src_len)
 
-    from habana_frameworks.torch.hpex import hmp
-
-    with hmp.disable_casts():
-        attn_weights = torch.nn.functional.softmax(attn_weights, dim=-1)
+    attn_weights = torch.nn.functional.softmax(attn_weights, dim=-1)
 
     if layer_head_mask is not None:
         if layer_head_mask.size() != (self.num_heads,):
             raise ValueError(
                 f"Head mask for a single layer should be of size {(self.num_heads,)}, but is"
                 f" {layer_head_mask.size()}"
             )
```

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/models/t5/modeling_t5.py` & `optimum-habana-1.9.0/optimum/habana/transformers/models/t5/modeling_t5.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/models/vit/modeling_vit.py` & `optimum-habana-1.9.0/optimum/habana/transformers/models/vit/modeling_vit.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/trainer.py` & `optimum-habana-1.9.0/optimum/habana/transformers/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import contextlib
 import copy
 import math
 import os
 import random
 import shutil
 import sys
-import tempfile
 import time
 import warnings
 from collections.abc import Mapping
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
 import huggingface_hub.utils as hf_hub_utils
@@ -34,27 +33,26 @@
 from accelerate.utils import DistributedDataParallelKwargs, GradientAccumulationPlugin
 from huggingface_hub import upload_folder
 from torch.utils.data import DataLoader, Dataset, RandomSampler
 from transformers import Trainer
 from transformers.data.data_collator import DataCollator
 from transformers.debug_utils import DebugOption, DebugUnderflowOverflow
 from transformers.integrations import hp_params
-from transformers.integrations.deepspeed import deepspeed_load_checkpoint
+from transformers.integrations.deepspeed import deepspeed_load_checkpoint, is_deepspeed_available
 from transformers.modeling_utils import PreTrainedModel, load_sharded_checkpoint, unwrap_model
-from transformers.pytorch_utils import ALL_LAYERNORM_LAYERS
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.trainer_callback import TrainerCallback, TrainerState
 from transformers.trainer_pt_utils import (
     DistributedTensorGatherer,
     IterableDatasetShard,
     LengthGroupedSampler,
     SequentialDistributedSampler,
     find_batch_size,
+    get_dataloader_sampler,
     get_model_param_count,
-    get_parameter_names,
     nested_concat,
     nested_detach,
     nested_numpify,
     reissue_pt_warnings,
     remove_dummy_checkpoint,
 )
 from transformers.trainer_utils import (
@@ -109,14 +107,18 @@
     import safetensors.torch
 
 
 if is_peft_available():
     from peft import PeftModel
 
 
+if is_deepspeed_available():
+    from accelerate.utils import DeepSpeedSchedulerWrapper
+
+
 if TYPE_CHECKING:
     import optuna
 
 
 logger = logging.get_logger(__name__)
 
 
@@ -182,95 +184,55 @@
         )
 
         if gaudi_config is None:
             self.gaudi_config = GaudiConfig.from_pretrained(args.gaudi_config_name)
         else:
             self.gaudi_config = copy.deepcopy(gaudi_config)
 
-        # Workaround for GPT2 and Wav2Vec2 that don't support Torch Autocast
-        if model.config.model_type == "gpt2" and self.gaudi_config == GaudiConfig.from_pretrained("Habana/gpt2"):
-            self.gaudi_config = GaudiConfig.from_pretrained(
-                "Habana/gpt2",
-                revision="84e72f935cb53d9c8c99e2911d725dae635a0d01",
-            )
-        elif model.config.model_type == "wav2vec2" and self.gaudi_config == GaudiConfig.from_pretrained(
-            "Habana/wav2vec2"
-        ):
-            self.gaudi_config = GaudiConfig.from_pretrained(
-                "Habana/wav2vec2",
-                revision="bb9159d3dca36202d752edca3fca2722d33c00e9",
-            )
-
         if self.args.use_habana:
             if self.args.use_hpu_graphs_for_inference:
                 self.already_wrapped_for_hpu_graphs = False
 
             if self.args.deepspeed:
                 # Mixed-precision backends are turned off when using DeepSpeed since it manages this itself
-                self.gaudi_config.use_habana_mixed_precision = False
                 self.gaudi_config.use_torch_autocast = False
                 self.use_hpu_amp = False
 
             if self.args.deepspeed or self.args.dataloader_num_workers >= 1:
                 # To avoid warnings about parallelism in tokenizers
                 os.environ["TOKENIZERS_PARALLELISM"] = "false"
 
             if self.gaudi_config.use_torch_autocast:
                 if not self.use_hpu_amp and not self.use_cpu_amp:
                     self.use_hpu_amp = True
                     logger.warning(
                         "The argument `--bf16` was not given but `use_torch_autocast` is True in the Gaudi configuration so mixed-precision training with Torch Autocast is enabled."
                     )
-            elif self.gaudi_config.use_habana_mixed_precision and self.use_hpu_amp:
-                self.gaudi_config.use_habana_mixed_precision = False
-                logger.warning(
-                    "`--bf16` was given and `use_habana_mixed_precision` is True in the Gaudi configuration. Using Torch Autocast as mixed-precision backend."
-                )
 
             if self.use_hpu_amp and "LOWER_LIST" not in os.environ:
                 gaudi_config.declare_autocast_bf16_fp32_ops()
 
-            if self.gaudi_config.use_habana_mixed_precision and not (self.use_hpu_amp or self.use_cpu_amp):
-                try:
-                    from habana_frameworks.torch.hpex import hmp
-                except ImportError as error:
-                    error.msg = f"Could not import habana_frameworks.torch.hpex. {error.msg}."
-                    raise error
-                self.hmp = hmp
-
-                warnings.warn(
-                    "Habana Mixed Precision is deprecated and will be removed in SynapseAI v1.12. Please"
-                    " use Torch Autocast instead using `--bf16` or setting `use_torch_autocast=true` in your"
-                    " Gaudi configuration.",
-                    FutureWarning,
-                )
-
-                # Open temporary files to mixed-precision write ops
-                with tempfile.NamedTemporaryFile() as hmp_bf16_file:
-                    with tempfile.NamedTemporaryFile() as hmp_fp32_file:
-                        # hmp.convert needs ops to be written in text files
-                        self.gaudi_config.write_bf16_fp32_ops_to_text_files(
-                            hmp_bf16_file.name,
-                            hmp_fp32_file.name,
-                        )
-                        self.hmp.convert(
-                            opt_level=self.gaudi_config.hmp_opt_level,
-                            bf16_file_path=hmp_bf16_file.name,
-                            fp32_file_path=hmp_fp32_file.name,
-                            isVerbose=self.gaudi_config.hmp_is_verbose,
-                        )
-
             if self.args.use_lazy_mode:
                 try:
                     import habana_frameworks.torch.core as htcore
                 except ImportError as error:
                     error.msg = f"Could not import habana_frameworks.torch.core. {error.msg}."
                     raise error
                 self.htcore = htcore
 
+                try:
+                    import habana_frameworks.torch.hpu as hthpu
+                except ImportError as error:
+                    error.msg = f"Could not import habana_frameworks.torch.hpu. {error.msg}."
+                    raise error
+                if self.gaudi_config.use_dynamic_shapes:
+                    hthpu.enable_dynamic_shape()
+                else:
+                    hthpu.disable_dynamic_shape()
+
             try:
                 from habana_frameworks.torch.hpu import random as hpu_random
             except ImportError as error:
                 error.msg = f"Could not import habana_frameworks.torch.hpu.random. {error.msg}."
                 raise error
             self.hpu_random = hpu_random
 
@@ -335,16 +297,15 @@
     def create_optimizer(self):
         """
         Setup the optimizer.
         We provide a reasonable default that works well. If you want to use something else, you can pass a tuple in the
         Trainer's init through `optimizers`, or subclass and override this method in a subclass.
         """
         if self.optimizer is None:
-            decay_parameters = get_parameter_names(self.model, ALL_LAYERNORM_LAYERS)
-            decay_parameters = [name for name in decay_parameters if "bias" not in name]
+            decay_parameters = self.get_decay_parameter_names(self.model)
 
             optimizer_grouped_parameters = []
             for t_params, t_weight_decay in zip(
                 [
                     [p for n, p in self.model.named_parameters() if n in decay_parameters and p.requires_grad],
                     [p for n, p in self.model.named_parameters() if n not in decay_parameters and p.requires_grad],
                 ],
@@ -546,38 +507,47 @@
         # Setting up training control variables:
         # number of training epochs: num_train_epochs
         # number of training steps per epoch: num_update_steps_per_epoch
         # total number of training steps to execute: max_steps
         total_train_batch_size = self._train_batch_size * args.gradient_accumulation_steps * args.world_size
 
         len_dataloader = None
+        num_train_tokens = None
         if has_length(train_dataloader):
             len_dataloader = len(train_dataloader)
             num_update_steps_per_epoch = len(train_dataloader) // args.gradient_accumulation_steps
             num_update_steps_per_epoch = max(num_update_steps_per_epoch, 1)
             num_examples = self.num_examples(train_dataloader)
             if args.max_steps > 0:
                 max_steps = args.max_steps
                 num_train_epochs = args.max_steps // num_update_steps_per_epoch + int(
                     args.max_steps % num_update_steps_per_epoch > 0
                 )
                 # May be slightly incorrect if the last batch in the training dataloader has a smaller size but it's
                 # the best we can do.
                 num_train_samples = args.max_steps * total_train_batch_size
+                if args.include_tokens_per_second:
+                    num_train_tokens = (
+                        self.num_tokens(train_dataloader, args.max_steps) * args.gradient_accumulation_steps
+                    )
             else:
                 max_steps = math.ceil(args.num_train_epochs * num_update_steps_per_epoch)
                 num_train_epochs = math.ceil(args.num_train_epochs)
                 num_train_samples = self.num_examples(train_dataloader) * args.num_train_epochs
+                if args.include_tokens_per_second:
+                    num_train_tokens = self.num_tokens(train_dataloader) * args.num_train_epochs
         elif args.max_steps > 0:  # Rely on max_steps when dataloader does not have a working size
             max_steps = args.max_steps
             # Setting a very large number of epochs so we go as many times as necessary over the iterator.
             num_train_epochs = sys.maxsize
             num_update_steps_per_epoch = max_steps
             num_examples = total_train_batch_size * args.max_steps
             num_train_samples = args.max_steps * total_train_batch_size
+            if args.include_tokens_per_second:
+                num_train_tokens = self.num_tokens(train_dataloader, args.max_steps) * args.gradient_accumulation_steps
         else:
             raise ValueError(
                 "args.max_steps must be set to a positive value if dataloader does not have a length, was"
                 f" {args.max_steps}"
             )
 
         if DebugOption.UNDERFLOW_OVERFLOW in self.args.debug:
@@ -639,14 +609,18 @@
             # For T5, checkpointing is imported with `from torch.utils.checkpoint import checkpoint`: https://github.com/huggingface/transformers/blob/04ab5605fbb4ef207b10bf2772d88c53fc242e83/src/transformers/models/t5/modeling_t5.py#L27
             # Whereas for other models we do `import torch.utils.checkpoint`
             # So monkey patching at Torch's level does not work
             if self.model.config.model_type == "t5":
                 import transformers.models.t5.modeling_t5 as modeling_t5
 
                 modeling_t5.checkpoint = torch.utils.checkpoint.checkpoint
+        else:
+            # Hack because `RegressionModel` in test_trainer.py doesn't have `gradient_checkpointing_disable`
+            if hasattr(self.model, "gradient_checkpointing_disable"):
+                self.model.gradient_checkpointing_disable()
 
         model = self._wrap_model(self.model_wrapped)
 
         # as the model is wrapped, don't use `accelerator.prepare`
         # this is for unhandled cases such as
         # FSDP-XLA, SageMaker MP/DP, DataParallel, IPEX
         use_accelerator_prepare = True if model is self.model else False
@@ -775,16 +749,25 @@
         self._zero_model_grad(model)
 
         self.control = self.callback_handler.on_train_begin(args, self.state, self.control)
 
         # Skip the first epochs_trained epochs to get the random state of the dataloader at the right point.
         if not args.ignore_data_skip:
             for epoch in range(epochs_trained):
-                for _ in train_dataloader:
-                    break
+                sampler = get_dataloader_sampler(train_dataloader)
+                is_random_sampler = isinstance(sampler, RandomSampler)
+                if not is_random_sampler:
+                    # We just need to begin an iteration to create the randomization of the sampler.
+                    for _ in train_dataloader:
+                        break
+                else:
+                    # Otherwise we need to call the whooooole sampler cause there is some random operation added
+                    # AT THE VERY END!
+                    sampler = sampler if sampler is not None else []
+                    _ = list(sampler)
 
         if self.args.adjust_throughput:
             self.log_evaluate_save_time = 0
         else:
             self.log_evaluate_save_time = None
 
         hb_profiler = HabanaProfile(
@@ -845,14 +828,19 @@
                 elif steps_trained_progress_bar is not None:
                     steps_trained_progress_bar.close()
                     steps_trained_progress_bar = None
 
                 if step % args.gradient_accumulation_steps == 0:
                     self.control = self.callback_handler.on_step_begin(args, self.state, self.control)
 
+                # attn_softmax_bf16 is enabled only for llama
+                if hasattr(self.model, "generation_config") and self.model.generation_config is not None:
+                    if self.model.config.model_type == "llama" and self.model.generation_config.attn_softmax_bf16:
+                        inputs["attn_softmax_bf16"] = True
+
                 # TODO: keep syncs for fast DDP?
                 with self.accelerator.accumulate(model):
                     tr_loss_step = self.training_step(model, inputs)
 
                 is_last_step_and_steps_less_than_grad_acc = (
                     steps_in_epoch <= args.gradient_accumulation_steps and (step + 1) == steps_in_epoch
                 )
@@ -900,39 +888,22 @@
                             # Some models (like FullyShardedDDP) have a specific way to do gradient clipping
                             model.clip_grad_norm_(args.max_grad_norm)
                         elif self.gaudi_config.use_fused_clip_norm and args.use_habana:
                             # TODO: to merge self.accelerator.clip_grad_norm_ when HMP is removed
                             self.FusedNorm.clip_norm(model.parameters())
                         else:
                             # Revert to normal clipping otherwise
-                            if (
-                                args.use_habana
-                                and (not (self.use_hpu_amp or self.use_cpu_amp))
-                                and self.gaudi_config.use_habana_mixed_precision
-                            ):
-                                with self.hmp.disable_casts():
-                                    torch.nn.utils.clip_grad_norm_(model.parameters(), args.max_grad_norm)
-                            else:
-                                self.accelerator.clip_grad_norm_(
-                                    model.parameters(),
-                                    args.max_grad_norm,
-                                )
+                            self.accelerator.clip_grad_norm_(
+                                model.parameters(),
+                                args.max_grad_norm,
+                            )
 
                     # Optimizer step
                     optimizer_was_run = True
-                    if (
-                        args.use_habana
-                        and self.gaudi_config.use_habana_mixed_precision
-                        and (not self.gaudi_config.use_fused_adam)
-                        and (not (self.use_hpu_amp or self.use_cpu_amp))
-                    ):
-                        with self.hmp.disable_casts():
-                            self.optimizer.step()
-                    else:
-                        self.optimizer.step()
+                    self.optimizer.step()
                     optimizer_was_run = not self.accelerator.optimizer_step_was_skipped
 
                     if optimizer_was_run:
                         # Delay optimizer scheduling until metrics are generated
                         if not isinstance(self.lr_scheduler, torch.optim.lr_scheduler.ReduceLROnPlateau):
                             self.lr_scheduler.step()
 
@@ -987,14 +958,15 @@
         num_samples_for_speed_metrics = num_train_samples - args.throughput_warmup_steps * total_train_batch_size
         num_steps_for_speed_metrics = self.state.max_steps - args.throughput_warmup_steps
         metrics = speed_metrics(
             "train",
             start_time,
             num_samples=num_samples_for_speed_metrics,
             num_steps=num_steps_for_speed_metrics,
+            num_tokens=num_train_tokens,
             start_time_after_warmup=start_time_after_warmup,
             log_evaluate_save_time=self.log_evaluate_save_time,
         )
         self.store_flos()
         metrics["total_flos"] = self.state.total_flos
         metrics["train_loss"] = train_loss
 
@@ -1195,17 +1167,21 @@
             scheduler_dict = self.lr_scheduler.state_dict()
             if self.args.use_habana:
                 # Move the state dict from HPU to CPU before saving
                 optim_dict = to_device_dtype(optim_dict, target_device=torch.device("cpu"))
                 scheduler_dict = to_device_dtype(scheduler_dict, target_device=torch.device("cpu"))
             torch.save(optim_dict, os.path.join(output_dir, OPTIMIZER_NAME))
 
-            # Save SCHEDULER & SCALER
+        # Save SCHEDULER & SCALER
+        is_deepspeed_custom_scheduler = self.is_deepspeed_enabled and not isinstance(
+            self.lr_scheduler, DeepSpeedSchedulerWrapper
+        )
+        if self.args.should_save and (not self.is_deepspeed_enabled or is_deepspeed_custom_scheduler):
             with warnings.catch_warnings(record=True) as caught_warnings:
-                torch.save(scheduler_dict, os.path.join(output_dir, SCHEDULER_NAME))
+                torch.save(self.lr_scheduler.state_dict(), os.path.join(output_dir, SCHEDULER_NAME))
             reissue_pt_warnings(caught_warnings)
 
         # Determine the new best metric / best model checkpoint
         if metrics is not None and self.args.metric_for_best_model is not None:
             metric_to_check = self.args.metric_for_best_model
             if not metric_to_check.startswith("eval_"):
                 metric_to_check = f"eval_{metric_to_check}"
@@ -1261,18 +1237,31 @@
     def _load_optimizer_and_scheduler(self, checkpoint):
         """If optimizer and scheduler states exist, load them."""
         if checkpoint is None:
             return
 
         if self.is_deepspeed_enabled:
             # deepspeed loads optimizer/lr_scheduler together with the model in deepspeed_init
+            if not isinstance(self.lr_scheduler, DeepSpeedSchedulerWrapper):
+                with warnings.catch_warnings(record=True) as caught_warnings:
+                    self.lr_scheduler.load_state_dict(torch.load(os.path.join(checkpoint, SCHEDULER_NAME)))
+                reissue_pt_warnings(caught_warnings)
             return
 
-        checkpoint_file_exists = os.path.isfile(os.path.join(checkpoint, OPTIMIZER_NAME)) or os.path.isfile(
-            os.path.join(checkpoint, OPTIMIZER_NAME_BIN)
+        checkpoint_file_exists = (
+            os.path.isfile(os.path.join(checkpoint, OPTIMIZER_NAME))
+            or os.path.isfile(os.path.join(checkpoint, OPTIMIZER_NAME_BIN))
+            or (
+                os.path.isdir(checkpoint)
+                and any(
+                    OPTIMIZER_NAME_BIN.split(".")[0] in folder_name
+                    for folder_name in os.listdir(checkpoint)
+                    if os.path.isdir(os.path.join(checkpoint, folder_name))
+                )
+            )
         )
 
         if checkpoint_file_exists and os.path.isfile(os.path.join(checkpoint, SCHEDULER_NAME)):
             # We use the CPU when training on one GPU to avoid OOM for GPU RAM when training big models.
             # In distributed training however, we load directly on each GPU and risk the GPU OOM as it's more
             # likely to get OOM on CPU (since we load num_gpu times the optimizer state
             map_location = "cpu" if self.args.use_habana else self.args.device
@@ -1394,15 +1383,16 @@
                 if self.args.should_save:
                     self._save(output_dir, state_dict=state_dict)
             except ValueError:
                 logger.warning(
                     " stage3_gather_16bit_weights_on_model_save=false. Saving the full checkpoint instead, use"
                     " zero_to_fp32.py to recover weights"
                 )
-                self._save(output_dir, state_dict={})
+                if self.args.should_save:
+                    self._save(output_dir, state_dict={})
                 # remove the dummy state_dict
                 remove_dummy_checkpoint(self.args.should_save, output_dir, [WEIGHTS_NAME, SAFE_WEIGHTS_NAME])
                 self.model_wrapped.save_checkpoint(output_dir)
         elif self.args.should_save:
             self._save(output_dir)
 
         # Push to the Hub when `save_model` is called by the user.
@@ -1490,15 +1480,17 @@
         # Do not use HPU graphs if the training is ongoing because it detaches gradients
         if args.use_hpu_graphs_for_inference and not self.is_in_train:
             logger.info("Using HPU graphs for inference.")
             # Do not wrap the model in HPU graphs if it has already been done
             if not self.already_wrapped_for_hpu_graphs:
                 from habana_frameworks.torch.hpu import wrap_in_hpu_graph
 
-                model = wrap_in_hpu_graph(model)
+                model = wrap_in_hpu_graph(
+                    model, disable_tensor_cache=args.disable_tensor_cache_hpu_graphs, max_graphs=args.max_hpu_graphs
+                )
                 self.already_wrapped_for_hpu_graphs = True
 
         batch_size = self.args.eval_batch_size
 
         logger.info(f"***** Running {description} *****")
         if has_length(dataloader):
             logger.info(f"  Num examples = {self.num_examples(dataloader)}")
@@ -1534,14 +1526,19 @@
             observed_batch_size = find_batch_size(inputs)
             if observed_batch_size is not None:
                 observed_num_examples += observed_batch_size
                 # For batch samplers, batch_size is not known by the dataloader in advance.
                 if batch_size is None:
                     batch_size = observed_batch_size
 
+            # attn_softmax_bf16 is enabled only for llama
+            if hasattr(self.model, "generation_config") and self.model.generation_config is not None:
+                if self.model.config.model_type == "llama" and self.model.generation_config.attn_softmax_bf16:
+                    inputs["attn_softmax_bf16"] = True
+
             # Prediction step
             loss, logits, labels = self.prediction_step(model, inputs, prediction_loss_only, ignore_keys=ignore_keys)
             main_input_name = getattr(self.model, "main_input_name", "input_ids")
             inputs_decode = self._prepare_input(inputs[main_input_name]) if args.include_inputs_for_metrics else None
 
             # Save the logits dtype since we need to convert them into floats during the process
             # They will be converted back into their original dtype right before computing metrics
@@ -1871,15 +1868,17 @@
         # Do not use HPU graphs if the training is ongoing because it detaches gradients
         if args.use_hpu_graphs_for_inference and not self.is_in_train:
             logger.info("Using HPU graphs for inference.")
             # Do not wrap the model in HPU graphs if it has already been done
             if not self.already_wrapped_for_hpu_graphs:
                 from habana_frameworks.torch.hpu import wrap_in_hpu_graph
 
-                model = wrap_in_hpu_graph(model)
+                model = wrap_in_hpu_graph(
+                    model, disable_tensor_cache=args.disable_tensor_cache_hpu_graphs, max_graphs=args.max_hpu_graphs
+                )
                 self.already_wrapped_for_hpu_graphs = True
 
         batch_size = dataloader.batch_size
         num_examples = self.num_examples(dataloader)
         logger.info(f"***** Running {description} *****")
         logger.info(f"  Num examples = {num_examples}")
         logger.info(f"  Batch size = {batch_size}")
```

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/trainer_seq2seq.py` & `optimum-habana-1.9.0/optimum/habana/transformers/trainer_seq2seq.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,32 +269,36 @@
         gen_kwargs["synced_gpus"] = (
             gen_kwargs["synced_gpus"] if gen_kwargs.get("synced_gpus") is not None else default_synced_gpus
         )
         # pad batches to max_length on-the-fly in lazy mode
         gen_kwargs["lazy_mode"] = (
             gen_kwargs["lazy_mode"] if gen_kwargs.get("lazy_mode") is not None else self.args.use_lazy_mode
         )
+        gen_kwargs["ignore_eos"] = (
+            gen_kwargs["ignore_eos"] if gen_kwargs.get("ignore_eos") is not None else self.args.ignore_eos
+        )
         gen_kwargs["hpu_graphs"] = (
             gen_kwargs["hpu_graphs"]
             if gen_kwargs.get("hpu_graphs") is not None
             else self.args.use_hpu_graphs_for_inference
         )
 
+        generation_inputs = inputs.copy()
         # If the `decoder_input_ids` was created from `labels`, evict the former, so that the model can freely generate
         # (otherwise, it would continue generating from the padded `decoder_input_ids`)
         if (
-            "labels" in inputs
-            and "decoder_input_ids" in inputs
-            and inputs["labels"].shape == inputs["decoder_input_ids"].shape
+            "labels" in generation_inputs
+            and "decoder_input_ids" in generation_inputs
+            and generation_inputs["labels"].shape == generation_inputs["decoder_input_ids"].shape
         ):
-            inputs = {k: v for k, v in inputs.items() if k != "decoder_input_ids"}
+            generation_inputs = {k: v for k, v in inputs.items() if k != "decoder_input_ids"}
         try:
             with torch.autocast(device_type="hpu", dtype=torch.bfloat16, enabled=self.use_hpu_amp):
                 generated_tokens = self.model.generate(
-                    **inputs,
+                    **generation_inputs,
                     generation_config=self.model.generation_config,
                     **gen_kwargs,
                 )
         except RuntimeError as error:
             if "cpu fallback is not supported during hpu graph capturing" in str(error):
                 error.args = (
                     f"{error}. You should run inference in lazy mode only with `use_lazy_mode=True` and `use_hpu_graphs_for_inference=False`.",
```

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/trainer_utils.py` & `optimum-habana-1.9.0/optimum/habana/transformers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/training_args.py` & `optimum-habana-1.9.0/optimum/habana/transformers/training_args.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     strtobool,
 )
 
 from optimum.utils import logging
 
 from ..accelerate.state import GaudiAcceleratorState, GaudiPartialState
 from ..accelerate.utils import GaudiDistributedType
+from ..utils import get_habana_frameworks_version
 from .gaudi_configuration import GaudiConfig
 
 
 if is_torch_available():
     import torch
 
 
@@ -80,22 +81,26 @@
     to enable deployment on Habana's Gaudi.
 
     Args:
         use_habana (`bool`, *optional*, defaults to `False`):
             Whether to use Habana's HPU for running the model.
         gaudi_config_name (`str`, *optional*):
             Pretrained Gaudi config name or path.
-        use_lazy_mode (`bool`, *optional*, defaults to `False`):
+        use_lazy_mode (`bool`, *optional*, defaults to `True`):
             Whether to use lazy mode for running the model.
         use_hpu_graphs (`bool`, *optional*, defaults to `False`):
             Deprecated, use `use_hpu_graphs_for_inference` instead. Whether to use HPU graphs for performing inference.
         use_hpu_graphs_for_inference (`bool`, *optional*, defaults to `False`):
             Whether to use HPU graphs for performing inference. It will speed up latency but may not be compatible with some operations.
         use_hpu_graphs_for_training (`bool`, *optional*, defaults to `False`):
             Whether to use HPU graphs for performing inference. It will speed up training but may not be compatible with some operations.
+        disable_tensor_cache_hpu_graphs (`bool`, *optional*, defaults to `False`):
+            Whether to disable tensor cache when using hpu graphs. If True, tensors won't be cached in hpu graph and memory can be saved.
+        max_hpu_graphs (`int`, *optional*):
+            Maximum number of hpu graphs to be cached. Reduce to save device memory.
         distribution_strategy (`str`, *optional*, defaults to `ddp`):
             Determines how data parallel distributed training is achieved. May be: `ddp` or `fast_ddp`.
         throughput_warmup_steps (`int`, *optional*, defaults to 0):
             Number of steps to ignore for throughput calculation. For example, with `throughput_warmup_steps=N`,
             the first N steps will not be considered in the calculation of the throughput. This is especially
             useful in lazy mode where the first two or three iterations typically take longer.
         adjust_throughput ('bool', *optional*, defaults to `False`):
@@ -118,15 +123,15 @@
 
     gaudi_config_name: Optional[str] = field(
         default=None,
         metadata={"help": "Pretrained Gaudi config name or path."},
     )
 
     use_lazy_mode: Optional[bool] = field(
-        default=False,
+        default=True,
         metadata={"help": "Whether to use lazy mode for running the model."},
     )
 
     use_hpu_graphs: Optional[bool] = field(
         default=False,
         metadata={
             "help": "Deprecated, use `use_hpu_graphs_for_inference` instead. Whether to use HPU graphs for performing inference."
@@ -143,14 +148,24 @@
     use_hpu_graphs_for_training: Optional[bool] = field(
         default=False,
         metadata={
             "help": "Whether to use HPU graphs for performing training. It will speed up training but may not be compatible with some operations."
         },
     )
 
+    disable_tensor_cache_hpu_graphs: Optional[bool] = field(
+        default=False,
+        metadata={"help": "Whether to use a tensor cache for hpu graphs."},
+    )
+
+    max_hpu_graphs: Optional[int] = field(
+        default=None,
+        metadata={"help": "Maximum number of HPU graphs to use."},
+    )
+
     distribution_strategy: Optional[str] = field(
         default="ddp",
         metadata={
             "help": "Determines how distributed data parallel training is achieved. "
             "Can be either `ddp` (i.e. using `DistributedDataParallel`) or "
             "`fast_ddp` (i.e. using `optimum.habana.distributed.all_reduce_gradients`).",
             "choices": ["ddp", "fast_ddp"],
@@ -181,14 +196,19 @@
             "help": (
                 "Whether to add an additional `mark_step` between forward and backward for pipelining "
                 "host backward building and HPU forward computing."
             )
         },
     )
 
+    ignore_eos: Optional[bool] = field(
+        default=True,
+        metadata={"help": ("Whether to disable stopping with eos token when calling `generate`.")},
+    )
+
     non_blocking_data_copy: Optional[bool] = field(
         default=False,
         metadata={"help": ("Whether to enable async data copy when preparing inputs.")},
     )
 
     profiling_warmup_steps: Optional[int] = field(
         default=0,
@@ -262,37 +282,41 @@
         },
     )
 
     def __post_init__(self):
         if self.use_hpu_graphs:
             warnings.warn(
                 (
-                    "`--use_hpu_graphs` is deprecated and will be removed in a future version of 🤗 Optimum Habana. Use "
-                    "`--use_hpu_graphs_for_inference` instead."
+                    "`--use_hpu_graphs` is deprecated and will be removed in a future version of 🤗 Optimum Habana. Use `--use_hpu_graphs_for_training` or `--use_hpu_graphs_for_inference` instead."
                 ),
                 FutureWarning,
             )
 
         use_hpu_graphs = self.use_hpu_graphs or self.use_hpu_graphs_for_inference or self.use_hpu_graphs_for_training
 
         if (self.use_lazy_mode or use_hpu_graphs or self.gaudi_config_name) and not self.use_habana:
             raise ValueError(
                 "`--use_lazy_mode`, `--use_hpu_graphs_for_inference`, `--use_hpu_graphs_for_training` and `--gaudi_config_name` cannot be used without `--use_habana`."
             )
-
-        if use_hpu_graphs and not self.use_lazy_mode:
+        if use_hpu_graphs and (not self.use_lazy_mode and not self.torch_compile_backend):
             raise ValueError(
                 "`--use_hpu_graphs_for_inference` and `--use_hpu_graphs_for_training` cannot be used in eager mode. Please set `--use_lazy_mode` to True."
             )
 
         if self.distribution_strategy not in SUPPORTED_DISTRIBUTION_STRATEGIES:
             raise ValueError(
                 f"`--distribution_strategy` is {self.distribution_strategy} which is an invalid or unsupported value. Possible choices are: {', '.join(SUPPORTED_DISTRIBUTION_STRATEGIES)}."
             )
 
+        if self.disable_tensor_cache_hpu_graphs and not use_hpu_graphs:
+            raise ValueError("must be using hpu graphs to set disable_tensor_cache_hpu_graphs.")
+
+        if self.max_hpu_graphs is not None and not use_hpu_graphs:
+            raise ValueError("must be using hpu graphs to set max_hpu_graphs.")
+
         # Raise errors for arguments that are not supported by optimum-habana
         if self.bf16_full_eval:
             raise ValueError("--bf16_full_eval is not supported by optimum-habana.")
         if self.fp16 or self.fp16_full_eval:
             raise ValueError(
                 "--fp16, --fp16_backend, --fp16_full_eval and --fp16_opt_level are not"
                 " supported by optimum-habana. Mixed-precision can be enabled in your Gaudi configuration."
@@ -433,14 +457,31 @@
                 FutureWarning,
             )
             self.optim = OptimizerNames.ADAFACTOR
         if self.optim == OptimizerNames.ADAMW_TORCH_FUSED and is_torch_available():
             if version.parse(version.parse(torch.__version__).base_version) < version.parse("2.0.0"):
                 raise ValueError("--optim adamw_torch_fused requires PyTorch 2.0 or higher")
 
+        if (self.torch_compile_mode is not None or self.torch_compile_backend is not None) and not self.torch_compile:
+            assert get_habana_frameworks_version().minor > 12, "Torch compile is not available"
+            self.torch_compile = True
+            assert not os.getenv("PT_HPU_LAZY_MODE", "1") != "0", "Dynamo and lazy are mutually exclusive."
+            # Note: PT_HPU_LAZY_MODE=0 needs to be set before library is loaded,
+            #       setting it here would be too late - hence assertion.
+        if self.torch_compile and self.torch_compile_backend is None:
+            self.torch_compile_backend = "inductor"
+
+        # accelerate integration for torch compile
+        if self.torch_compile:
+            # set env vars for accelerate
+            prefix = "ACCELERATE_DYNAMO_"
+            os.environ[prefix + "BACKEND"] = self.torch_compile_backend
+            if self.torch_compile_mode is not None:
+                os.environ[prefix + "MODE"] = self.torch_compile_mode
+
         # if training args is specified, it will override the one specified in the accelerate config
         mixed_precision_dtype = os.environ.get("ACCELERATE_MIXED_PRECISION", "no")
         if self.bf16:
             mixed_precision_dtype = "bf16"
         os.environ["ACCELERATE_MIXED_PRECISION"] = mixed_precision_dtype
 
         if self.report_to is None:
@@ -606,16 +647,19 @@
             # Otherwise this will fail when some __init__ methods are overridden (cf. GPT2Attention)
             from .modeling_utils import adapt_transformers_to_gaudi
 
             adapt_transformers_to_gaudi()
 
             if self.use_lazy_mode:
                 logger.info("Enabled lazy mode.")
-            else:
-                os.environ["PT_HPU_LAZY_MODE"] = "2"
+            # TODO: remove the block below when upgrade to SynapseAI 1.13 is done
+            # as eager mode will not be available anymore
+            elif not self.torch_compile:
+                if os.getenv("PT_HPU_LAZY_MODE", "1") != "0":
+                    os.environ["PT_HPU_LAZY_MODE"] = "2"
                 logger.info("Enabled eager mode because use_lazy_mode=False.")
 
             if self.deepspeed:
                 # Need to do similar for Accelerator init
                 os.environ["ACCELERATE_USE_DEEPSPEED"] = "true"
                 self.distributed_state = GaudiPartialState(timeout=timedelta(seconds=self.ddp_timeout))
                 del os.environ["ACCELERATE_USE_DEEPSPEED"]
```

### Comparing `optimum-habana-1.8.2/optimum/habana/transformers/training_args_seq2seq.py` & `optimum-habana-1.9.0/optimum/habana/transformers/training_args_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.8.2/optimum/habana/utils.py` & `optimum-habana-1.9.0/optimum/habana/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 from .version import __version__
 
 
 logger = logging.get_logger(__name__)
 
 
-CURRENTLY_VALIDATED_SYNAPSE_VERSION = version.parse("1.12.0")
+CURRENTLY_VALIDATED_SYNAPSE_VERSION = version.parse("1.13.0")
 
 
 def to_device_dtype(my_input: Any, target_device: torch.device = None, target_dtype: torch.dtype = None):
     """
     Move a state_dict to the target device and convert it into target_dtype.
 
     Args:
@@ -63,27 +63,30 @@
 
 
 def speed_metrics(
     split: str,
     start_time: float,
     num_samples: int = None,
     num_steps: int = None,
+    num_tokens: int = None,
     start_time_after_warmup: float = None,
     log_evaluate_save_time: float = None,
 ) -> Dict[str, float]:
     """
     Measure and return speed performance metrics.
+
     This function requires a time snapshot `start_time` before the operation to be measured starts and this function
     should be run immediately after the operation to be measured has completed.
 
     Args:
         split (str): name to prefix metric (like train, eval, test...)
         start_time (float): operation start time
         num_samples (int, optional): number of samples processed. Defaults to None.
         num_steps (int, optional): number of steps performed. Defaults to None.
+        num_tokens (int, optional): number of tokens processed. Defaults to None.
         start_time_after_warmup (float, optional): time after warmup steps have been performed. Defaults to None.
         log_evaluate_save_time (float, optional): time spent to log, evaluate and save. Defaults to None.
 
     Returns:
         Dict[str, float]: dictionary with performance metrics.
     """
 
@@ -103,14 +106,17 @@
     # Compute throughputs
     if num_samples is not None:
         samples_per_second = num_samples / runtime
         result[f"{split}_samples_per_second"] = round(samples_per_second, 3)
     if num_steps is not None:
         steps_per_second = num_steps / runtime
         result[f"{split}_steps_per_second"] = round(steps_per_second, 3)
+    if num_tokens is not None:
+        tokens_per_second = num_tokens / runtime
+        result[f"{split}_tokens_per_second"] = round(tokens_per_second, 3)
 
     return result
 
 
 def to_gb_rounded(mem: float) -> float:
     """
     Rounds and converts to GB.
@@ -205,15 +211,15 @@
     output = subprocess.run(
         "pip list | grep habana-torch-plugin",
         shell=True,
         text=True,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     )
-    return version.parse(output.stdout.split("\n")[0].split(" ")[-1])
+    return version.parse(output.stdout.split("\n")[0].split()[-1])
 
 
 def get_driver_version():
     """
     Returns the driver version.
     """
     output = subprocess.run(
@@ -316,14 +322,24 @@
             error_message += (
                 "You can install it from source with: "
                 "`pip install git+https://github.com/huggingface/optimum-habana.git`."
             )
         raise ImportError(error_message)
 
 
+def check_habana_frameworks_min_version(min_version):
+    """
+    Checks if the installed version of `habana_frameworks` is larger than or equal to `min_version`.
+    """
+    if get_habana_frameworks_version() < version.parse(min_version):
+        return False
+    else:
+        return True
+
+
 def get_device_name():
     """
     Returns the name of the current device: Gaudi or Gaudi2.
 
     Inspired from: https://github.com/HabanaAI/Model-References/blob/a87c21f14f13b70ffc77617b9e80d1ec989a3442/PyTorch/computer_vision/classification/torchvision/utils.py#L274
     """
     import habana_frameworks.torch.utils.experimental as htexp
```

### Comparing `optimum-habana-1.8.2/optimum/habana/version.py` & `optimum-habana-1.9.0/optimum/habana/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.8.2"
+__version__ = "1.9.0"
```

### Comparing `optimum-habana-1.8.2/optimum_habana.egg-info/PKG-INFO` & `optimum-habana-1.9.0/optimum_habana.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-habana
-Version: 1.8.2
+Version: 1.9.0
 Summary: Optimum Habana is the interface between the Hugging Face Transformers and Diffusers libraries and Habana's Gaudi processor (HPU). It provides a set of tools enabling easy model loading, training and inference on single- and multi-HPU settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/habana
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,gaudi,hpu
 Classifier: Development Status :: 5 - Production/Stable
@@ -61,15 +61,15 @@
 pip install --upgrade-strategy eager optimum[habana]
 ```
 
 The `--upgrade-strategy eager` option is needed to ensure `optimum-habana` is upgraded to the latest stable release.
 
 > To use DeepSpeed on HPUs, you also need to run the following command:
 >```bash
->pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.12.0
+>pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.13.0
 >```
 
 Optimum Habana is a fast-moving project, and you may want to install it from source:
 
 ```bash
 pip install git+https://github.com/huggingface/optimum-habana.git
 ```
@@ -87,15 +87,15 @@
 ### Quick Start
 
 🤗 Optimum Habana was designed with one goal in mind: **to make training and inference straightforward for any 🤗 Transformers and 🤗 Diffusers user while leveraging the complete power of Gaudi processors**.
 
 #### Transformers Interface
 
 There are two main classes one needs to know:
-- [GaudiTrainer](https://huggingface.co/docs/optimum/habana/package_reference/trainer): the trainer class that takes care of compiling (lazy or eager mode) and distributing the model to run on HPUs, and performing training and evaluation.
+- [GaudiTrainer](https://huggingface.co/docs/optimum/habana/package_reference/trainer): the trainer class that takes care of compiling and distributing the model to run on HPUs, and performing training and evaluation.
 - [GaudiConfig](https://huggingface.co/docs/optimum/habana/package_reference/gaudi_config): the class that enables to configure Habana Mixed Precision and to decide whether optimized operators and optimizers should be used or not.
 
 The [GaudiTrainer](https://huggingface.co/docs/optimum/habana/package_reference/trainer) is very similar to the [🤗 Transformers Trainer](https://huggingface.co/docs/transformers/main_classes/trainer), and adapting a script using the Trainer to make it work with Gaudi will mostly consist in simply swapping the `Trainer` class for the `GaudiTrainer` one.
 That's how most of the [example scripts](https://github.com/huggingface/optimum-habana/tree/main/examples) were adapted from their [original counterparts](https://github.com/huggingface/transformers/tree/main/examples/pytorch).
 
 Here is an example:
 ```diff
@@ -181,19 +181,20 @@
 | DistilBERT |:heavy_check_mark: | :heavy_check_mark: | <li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering)</li><li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li> |
 | GPT2             | :heavy_check_mark: | :heavy_check_mark: | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li><li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | BLOOM(Z) | :x: | <div style="text-align:left"><li>DeepSpeed</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | StarCoder | :x: | <div style="text-align:left"><li>Single card</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | GPT-J | <div style="text-align:left"><li>DeepSpeed</li></div> | <div style="text-align:left"><li>Single card</li><li>DeepSpeed</li></div> | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li><li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | GPT-NeoX | <div style="text-align:left"><li>DeepSpeed</li></div> | <div style="text-align:left"><li>DeepSpeed</li></div> | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li><li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | OPT | :x: | <div style="text-align:left"><li>DeepSpeed</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
-| Llama 2 / CodeLlama | <div style="text-align:left"><li>DeepSpeed</li><li>LoRA</li></div> | <div style="text-align:left"><li>DeepSpeed</li><li>LoRA</li></div> | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li><li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
+| Llama 2 / CodeLlama | <div style="text-align:left"><li>DeepSpeed</li><li>LoRA</li></div> | :heavy_check_mark: | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li><li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | StableLM | :x: | <div style="text-align:left"><li>Single card</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
-| Falcon | :x: | <div style="text-align:left"><li>Single card</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
+| Falcon | <div style="text-align:left"><li>LoRA</li></div> | :heavy_check_mark: | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | CodeGen | :x: | <div style="text-align:left"><li>Single card</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | MPT | :x: | <div style="text-align:left"><li>Single card</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
+| Mistral | :x: | <div style="text-align:left"><li>Single card</li></div> | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 | T5 | :heavy_check_mark: | :heavy_check_mark: | <li>[summarization](https://github.com/huggingface/optimum-habana/tree/main/examples/summarization)</li><li>[translation](https://github.com/huggingface/optimum-habana/tree/main/examples/translation)</li><li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering#fine-tuning-t5-on-squad20)</li> |
 | BART | :x: | <div style="text-align:left"><li>Single card</li></div> | <li>[summarization](https://github.com/huggingface/optimum-habana/tree/main/examples/summarization)</li><li>[translation](https://github.com/huggingface/optimum-habana/tree/main/examples/translation)</li><li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering#fine-tuning-t5-on-squad20)</li> |
 | ViT | :heavy_check_mark: | :heavy_check_mark: | <li>[image classification](https://github.com/huggingface/optimum-habana/tree/main/examples/image-classification)</li> |
 | Swin | :heavy_check_mark: | :heavy_check_mark: | <li>[image classification](https://github.com/huggingface/optimum-habana/tree/main/examples/image-classification)</li> |
 | Wav2Vec2 | :heavy_check_mark: | :heavy_check_mark: | <li>[audio classification](https://github.com/huggingface/optimum-habana/tree/main/examples/audio-classification)</li><li>[speech recognition](https://github.com/huggingface/optimum-habana/tree/main/examples/speech-recognition)</li> |
 | CLIP | :heavy_check_mark: | :heavy_check_mark: | <li>[contrastive image-text training](https://github.com/huggingface/optimum-habana/tree/main/examples/contrastive-image-text)</li> |
 | BridgeTower | :heavy_check_mark: | :heavy_check_mark: | <li>[contrastive image-text training](https://github.com/huggingface/optimum-habana/tree/main/examples/contrastive-image-text)</li> |
```

### Comparing `optimum-habana-1.8.2/optimum_habana.egg-info/SOURCES.txt` & `optimum-habana-1.9.0/optimum_habana.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 optimum/habana/__init__.py
+optimum/habana/checkpoint_utils.py
 optimum/habana/utils.py
 optimum/habana/version.py
 optimum/habana/accelerate/__init__.py
 optimum/habana/accelerate/accelerator.py
+optimum/habana/accelerate/data_loader.py
 optimum/habana/accelerate/state.py
 optimum/habana/accelerate/utils/__init__.py
 optimum/habana/accelerate/utils/dataclasses.py
 optimum/habana/diffusers/__init__.py
 optimum/habana/diffusers/models/__init__.py
 optimum/habana/diffusers/models/unet_2d_condition.py
 optimum/habana/diffusers/pipelines/pipeline_utils.py
@@ -44,28 +46,29 @@
 optimum/habana/transformers/models/bart/__init__.py
 optimum/habana/transformers/models/bart/modeling_bart.py
 optimum/habana/transformers/models/bloom/__init__.py
 optimum/habana/transformers/models/bloom/modeling_bloom.py
 optimum/habana/transformers/models/codegen/__init__.py
 optimum/habana/transformers/models/codegen/modeling_codegen.py
 optimum/habana/transformers/models/esm/__init__.py
-optimum/habana/transformers/models/esm/modeling_esm.py
 optimum/habana/transformers/models/esm/modeling_esmfold.py
 optimum/habana/transformers/models/falcon/__init__.py
 optimum/habana/transformers/models/falcon/modeling_falcon.py
 optimum/habana/transformers/models/gpt2/__init__.py
 optimum/habana/transformers/models/gpt2/modeling_gpt2.py
 optimum/habana/transformers/models/gpt_bigcode/__init__.py
 optimum/habana/transformers/models/gpt_bigcode/modeling_gpt_bigcode.py
 optimum/habana/transformers/models/gpt_neox/__init__.py
 optimum/habana/transformers/models/gpt_neox/modeling_gpt_neox.py
 optimum/habana/transformers/models/gptj/__init__.py
 optimum/habana/transformers/models/gptj/modeling_gptj.py
 optimum/habana/transformers/models/llama/__init__.py
 optimum/habana/transformers/models/llama/modeling_llama.py
+optimum/habana/transformers/models/mistral/__init__.py
+optimum/habana/transformers/models/mistral/modeling_mistral.py
 optimum/habana/transformers/models/mpt/__init__.py
 optimum/habana/transformers/models/mpt/modeling_mpt.py
 optimum/habana/transformers/models/opt/__init__.py
 optimum/habana/transformers/models/opt/modeling_opt.py
 optimum/habana/transformers/models/t5/__init__.py
 optimum/habana/transformers/models/t5/modeling_t5.py
 optimum/habana/transformers/models/vit/__init__.py
```

### Comparing `optimum-habana-1.8.2/setup.py` & `optimum-habana-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,34 +25,33 @@
     with open(filepath) as version_file:
         (__version__,) = re.findall('__version__ = "(.*)"', version_file.read())
 except Exception as error:
     assert False, "Error: Could not open '%s' due %s\n" % (filepath, error)
 
 
 INSTALL_REQUIRES = [
-    "transformers >= 4.33.0, < 4.35.0",
+    "transformers >= 4.34.0, < 4.35.0",
     "optimum",
     "torch",
     "accelerate >= 0.23.0",
-    "diffusers >= 0.18.0",
+    "diffusers >= 0.18.0, < 0.24.0",
 ]
 
 TESTS_REQUIRE = [
     "pytest",
     "psutil",
     "parameterized",
     "GitPython",
     "optuna",
     "sentencepiece",
     "datasets",
     "safetensors",
 ]
 
 QUALITY_REQUIRES = [
-    "black",
     "ruff",
     "hf_doc_builder",
 ]
 
 EXTRAS_REQUIRE = {
     "tests": TESTS_REQUIRE,
     "quality": QUALITY_REQUIRES,
```

### Comparing `optimum-habana-1.8.2/tests/test_diffusers.py` & `optimum-habana-1.9.0/tests/test_diffusers.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import os
 import tempfile
 from io import BytesIO
 from pathlib import Path
 from unittest import TestCase
 
 import numpy as np
 import requests
 import torch
 from diffusers import AutoencoderKL, UNet2DConditionModel
-from habana_frameworks.torch.hpex import hmp
 from parameterized import parameterized
 from PIL import Image
 from transformers import CLIPTextConfig, CLIPTextModel, CLIPTokenizer
 from transformers.testing_utils import slow
 
 from optimum.habana import GaudiConfig
 from optimum.habana.diffusers import (
@@ -36,17 +36,20 @@
     GaudiStableDiffusionLDM3DPipeline,
     GaudiStableDiffusionPipeline,
     GaudiStableDiffusionUpscalePipeline,
 )
 from optimum.habana.utils import set_seed
 
 
-THROUGHPUT_BASELINE_HMP = 0.298
-THROUGHPUT_BASELINE_BF16 = 0.309
-THROUGHPUT_BASELINE_AUTOCAST = 0.111
+if os.environ.get("GAUDI2_CI", "0") == "1":
+    THROUGHPUT_BASELINE_BF16 = 1.019
+    THROUGHPUT_BASELINE_AUTOCAST = 0.389
+else:
+    THROUGHPUT_BASELINE_BF16 = 0.301
+    THROUGHPUT_BASELINE_AUTOCAST = 0.108
 
 
 class GaudiPipelineUtilsTester(TestCase):
     """
     Tests the features added on top of diffusers/pipeline_utils.py.
     """
 
@@ -125,51 +128,54 @@
 
 
 class GaudiStableDiffusionPipelineTester(TestCase):
     """
     Tests the StableDiffusionPipeline for Gaudi.
     """
 
-    def get_dummy_components(self):
+    def get_dummy_components(self, time_cond_proj_dim=None):
         torch.manual_seed(0)
         unet = UNet2DConditionModel(
-            block_out_channels=(32, 64),
-            layers_per_block=2,
+            block_out_channels=(4, 8),
+            layers_per_block=1,
             sample_size=32,
+            time_cond_proj_dim=time_cond_proj_dim,
             in_channels=4,
             out_channels=4,
             down_block_types=("DownBlock2D", "CrossAttnDownBlock2D"),
             up_block_types=("CrossAttnUpBlock2D", "UpBlock2D"),
             cross_attention_dim=32,
+            norm_num_groups=2,
         )
         scheduler = GaudiDDIMScheduler(
             beta_start=0.00085,
             beta_end=0.012,
             beta_schedule="scaled_linear",
             clip_sample=False,
             set_alpha_to_one=False,
         )
         torch.manual_seed(0)
         vae = AutoencoderKL(
-            block_out_channels=[32, 64],
+            block_out_channels=[4, 8],
             in_channels=3,
             out_channels=3,
             down_block_types=["DownEncoderBlock2D", "DownEncoderBlock2D"],
             up_block_types=["UpDecoderBlock2D", "UpDecoderBlock2D"],
             latent_channels=4,
+            norm_num_groups=2,
         )
         torch.manual_seed(0)
         text_encoder_config = CLIPTextConfig(
             bos_token_id=0,
             eos_token_id=2,
             hidden_size=32,
-            intermediate_size=37,
+            intermediate_size=64,
             layer_norm_eps=1e-05,
-            num_attention_heads=4,
-            num_hidden_layers=5,
+            num_attention_heads=8,
+            num_hidden_layers=3,
             pad_token_id=1,
             vocab_size=1000,
         )
         text_encoder = CLIPTextModel(text_encoder_config)
         tokenizer = CLIPTokenizer.from_pretrained("hf-internal-testing/tiny-random-clip")
 
         components = {
@@ -191,40 +197,39 @@
             "num_inference_steps": 2,
             "guidance_scale": 6.0,
             "output_type": "numpy",
         }
         return inputs
 
     def test_stable_diffusion_ddim(self):
-        with hmp.disable_casts():
-            device = "cpu"
+        device = "cpu"
 
-            components = self.get_dummy_components()
-            gaudi_config = GaudiConfig(use_habana_mixed_precision=False)
+        components = self.get_dummy_components()
+        gaudi_config = GaudiConfig(use_torch_autocast=False)
 
-            sd_pipe = GaudiStableDiffusionPipeline(
-                use_habana=True,
-                gaudi_config=gaudi_config,
-                **components,
-            )
-            sd_pipe.set_progress_bar_config(disable=None)
+        sd_pipe = GaudiStableDiffusionPipeline(
+            use_habana=True,
+            gaudi_config=gaudi_config,
+            **components,
+        )
+        sd_pipe.set_progress_bar_config(disable=None)
 
-            inputs = self.get_dummy_inputs(device)
-            output = sd_pipe(**inputs)
-            image = output.images[0]
+        inputs = self.get_dummy_inputs(device)
+        output = sd_pipe(**inputs)
+        image = output.images[0]
 
-            image_slice = image[-3:, -3:, -1]
+        image_slice = image[-3:, -3:, -1]
 
-            self.assertEqual(image.shape, (64, 64, 3))
-            expected_slice = np.array([0.5756, 0.6118, 0.5005, 0.5041, 0.5471, 0.4726, 0.4976, 0.4865, 0.4864])
+        self.assertEqual(image.shape, (64, 64, 3))
+        expected_slice = np.array([0.3203, 0.4555, 0.4711, 0.3505, 0.3973, 0.4650, 0.5137, 0.3392, 0.4045])
 
-            self.assertLess(np.abs(image_slice.flatten() - expected_slice).max(), 1e-2)
+        self.assertLess(np.abs(image_slice.flatten() - expected_slice).max(), 1e-2)
 
     def test_stable_diffusion_no_safety_checker(self):
-        gaudi_config = GaudiConfig(use_habana_mixed_precision=False)
+        gaudi_config = GaudiConfig()
         scheduler = GaudiDDIMScheduler(
             beta_start=0.00085,
             beta_end=0.012,
             beta_schedule="scaled_linear",
             clip_sample=False,
             set_alpha_to_one=False,
         )
@@ -504,41 +509,14 @@
             num_images_per_prompt=5,
         ).images
 
         self.assertEqual(len(images), 10)
         self.assertEqual(images[-1].shape, (64, 64, 3))
 
     @slow
-    def test_no_throughput_regression_hmp(self):
-        prompts = [
-            "An image of a squirrel in Picasso style",
-            "High quality photo of an astronaut riding a horse in space",
-        ]
-        num_images_per_prompt = 11
-        batch_size = 4
-        model_name = "runwayml/stable-diffusion-v1-5"
-        scheduler = GaudiDDIMScheduler.from_pretrained(model_name, subfolder="scheduler")
-
-        pipeline = GaudiStableDiffusionPipeline.from_pretrained(
-            model_name,
-            scheduler=scheduler,
-            use_habana=True,
-            use_hpu_graphs=True,
-            gaudi_config=GaudiConfig.from_pretrained("Habana/stable-diffusion"),
-        )
-        set_seed(27)
-        outputs = pipeline(
-            prompt=prompts,
-            num_images_per_prompt=num_images_per_prompt,
-            batch_size=batch_size,
-        )
-        self.assertEqual(len(outputs.images), num_images_per_prompt * len(prompts))
-        self.assertGreaterEqual(outputs.throughput, 0.95 * THROUGHPUT_BASELINE_HMP)
-
-    @slow
     def test_no_throughput_regression_bf16(self):
         prompts = [
             "An image of a squirrel in Picasso style",
             "High quality photo of an astronaut riding a horse in space",
         ]
         num_images_per_prompt = 11
         batch_size = 4
@@ -591,99 +569,164 @@
         self.assertEqual(len(outputs.images), num_images_per_prompt * len(prompts))
         self.assertGreaterEqual(outputs.throughput, 0.95 * THROUGHPUT_BASELINE_AUTOCAST)
 
     @slow
     def test_no_generation_regression(self):
         model_name = "CompVis/stable-diffusion-v1-4"
         # fp32
-        with hmp.disable_casts():
-            scheduler = GaudiDDIMScheduler.from_pretrained(model_name, subfolder="scheduler")
-            pipeline = GaudiStableDiffusionPipeline.from_pretrained(
-                model_name,
-                scheduler=scheduler,
-                safety_checker=None,
-                use_habana=True,
-                use_hpu_graphs=True,
-                gaudi_config=GaudiConfig(use_habana_mixed_precision=False),
-            )
-            set_seed(27)
-            outputs = pipeline(
-                prompt="An image of a squirrel in Picasso style",
-                output_type="np",
-            )
+        scheduler = GaudiDDIMScheduler.from_pretrained(model_name, subfolder="scheduler")
+        pipeline = GaudiStableDiffusionPipeline.from_pretrained(
+            model_name,
+            scheduler=scheduler,
+            safety_checker=None,
+            use_habana=True,
+            use_hpu_graphs=True,
+            gaudi_config=GaudiConfig(use_torch_autocast=False),
+        )
+        set_seed(27)
+        outputs = pipeline(
+            prompt="An image of a squirrel in Picasso style",
+            output_type="np",
+        )
 
+        if os.environ.get("GAUDI2_CI", "0") == "1":
+            expected_slice = np.array(
+                [
+                    0.350823,
+                    0.34849027,
+                    0.33486015,
+                    0.35479546,
+                    0.3231264,
+                    0.33130097,
+                    0.34374988,
+                    0.30728853,
+                    0.30011398,
+                ]
+            )
+        else:
             expected_slice = np.array(
                 [0.70760196, 0.7136303, 0.7000798, 0.714934, 0.6776865, 0.6800843, 0.6923707, 0.6653969, 0.6408076]
             )
-            image = outputs.images[0]
+        image = outputs.images[0]
 
-            self.assertEqual(image.shape, (512, 512, 3))
-            self.assertLess(np.abs(expected_slice - image[-3:, -3:, -1].flatten()).max(), 5e-3)
+        self.assertEqual(image.shape, (512, 512, 3))
+        self.assertLess(np.abs(expected_slice - image[-3:, -3:, -1].flatten()).max(), 5e-3)
 
     @slow
     def test_no_generation_regression_ldm3d(self):
         model_name = "Intel/ldm3d-4c"
         # fp32
-        with hmp.disable_casts():
-            scheduler = GaudiDDIMScheduler.from_pretrained(model_name, subfolder="scheduler")
-            pipeline = GaudiStableDiffusionLDM3DPipeline.from_pretrained(
-                model_name,
-                scheduler=scheduler,
-                safety_checker=None,
-                use_habana=True,
-                use_hpu_graphs=True,
-                gaudi_config=GaudiConfig(use_habana_mixed_precision=False),
+        scheduler = GaudiDDIMScheduler.from_pretrained(model_name, subfolder="scheduler")
+        pipeline = GaudiStableDiffusionLDM3DPipeline.from_pretrained(
+            model_name,
+            scheduler=scheduler,
+            safety_checker=None,
+            use_habana=True,
+            use_hpu_graphs=True,
+            gaudi_config=GaudiConfig(),
+        )
+        set_seed(27)
+        outputs = pipeline(
+            prompt="An image of a squirrel in Picasso style",
+            output_type="np",
+        )
+
+        if os.environ.get("GAUDI2_CI", "0") == "1":
+            expected_slice_rgb = np.array(
+                [
+                    0.2099357,
+                    0.16664368,
+                    0.08352646,
+                    0.20643419,
+                    0.16748399,
+                    0.08781305,
+                    0.21379063,
+                    0.19943115,
+                    0.04389626,
+                ]
             )
-            set_seed(27)
-            outputs = pipeline(
-                prompt="An image of a squirrel in Picasso style",
-                output_type="np",
+            expected_slice_depth = np.array(
+                [
+                    0.68369114,
+                    0.6827824,
+                    0.6852779,
+                    0.6836072,
+                    0.6888298,
+                    0.6895473,
+                    0.6853674,
+                    0.67561126,
+                    0.660434,
+                ]
             )
-
+        else:
             expected_slice_rgb = np.array([0.7083766, 1.0, 1.0, 0.70610344, 0.9867363, 1.0, 0.7214538, 1.0, 1.0])
             expected_slice_depth = np.array(
-                [0.919621, 0.92072034, 0.9184986, 0.91994286, 0.9242079, 0.93387043, 0.92345214, 0.93558526, 0.9223714]
+                [
+                    0.919621,
+                    0.92072034,
+                    0.9184986,
+                    0.91994286,
+                    0.9242079,
+                    0.93387043,
+                    0.92345214,
+                    0.93558526,
+                    0.9223714,
+                ]
             )
-            rgb = outputs.rgb[0]
-            depth = outputs.depth[0]
+        rgb = outputs.rgb[0]
+        depth = outputs.depth[0]
 
-            self.assertEqual(rgb.shape, (512, 512, 3))
-            self.assertEqual(depth.shape, (512, 512, 1))
-            self.assertLess(np.abs(expected_slice_rgb - rgb[-3:, -3:, -1].flatten()).max(), 5e-3)
-            self.assertLess(np.abs(expected_slice_depth - depth[-3:, -3:, -1].flatten()).max(), 5e-3)
+        self.assertEqual(rgb.shape, (512, 512, 3))
+        self.assertEqual(depth.shape, (512, 512, 1))
+        self.assertLess(np.abs(expected_slice_rgb - rgb[-3:, -3:, -1].flatten()).max(), 5e-3)
+        self.assertLess(np.abs(expected_slice_depth - depth[-3:, -3:, -1].flatten()).max(), 5e-3)
 
     @slow
     def test_no_generation_regression_upscale(self):
         model_name = "stabilityai/stable-diffusion-x4-upscaler"
         # fp32
-        with hmp.disable_casts():
-            scheduler = GaudiDDIMScheduler.from_pretrained(model_name, subfolder="scheduler")
-            pipeline = GaudiStableDiffusionUpscalePipeline.from_pretrained(
-                model_name,
-                scheduler=scheduler,
-                use_habana=True,
-                use_hpu_graphs=True,
-                gaudi_config=GaudiConfig(use_habana_mixed_precision=False),
-            )
-            set_seed(27)
+        scheduler = GaudiDDIMScheduler.from_pretrained(model_name, subfolder="scheduler")
+        pipeline = GaudiStableDiffusionUpscalePipeline.from_pretrained(
+            model_name,
+            scheduler=scheduler,
+            use_habana=True,
+            use_hpu_graphs=True,
+            gaudi_config=GaudiConfig(use_torch_autocast=False),
+        )
+        set_seed(27)
 
-            url = "https://huggingface.co/datasets/hf-internal-testing/diffusers-images/resolve/main/sd2-upscale/low_res_cat.png"
-            response = requests.get(url)
-            low_res_img = Image.open(BytesIO(response.content)).convert("RGB")
-            low_res_img = low_res_img.resize((128, 128))
-            prompt = "a white cat"
-            upscaled_image = pipeline(prompt=prompt, image=low_res_img, output_type="np").images[0]
+        url = "https://huggingface.co/datasets/hf-internal-testing/diffusers-images/resolve/main/sd2-upscale/low_res_cat.png"
+        response = requests.get(url)
+        low_res_img = Image.open(BytesIO(response.content)).convert("RGB")
+        low_res_img = low_res_img.resize((128, 128))
+        prompt = "a white cat"
+        upscaled_image = pipeline(prompt=prompt, image=low_res_img, output_type="np").images[0]
+        if os.environ.get("GAUDI2_CI", "0") == "1":
+            expected_slice = np.array(
+                [
+                    0.16527882,
+                    0.161616,
+                    0.15665859,
+                    0.1660901,
+                    0.1594379,
+                    0.14936888,
+                    0.1578255,
+                    0.15342498,
+                    0.14590919,
+                ]
+            )
+        else:
             expected_slice = np.array(
                 [
                     0.1652787,
                     0.16161594,
                     0.15665877,
                     0.16608998,
                     0.1594378,
                     0.14936894,
                     0.15782538,
                     0.15342498,
                     0.14590913,
                 ]
             )
-            self.assertEqual(upscaled_image.shape, (512, 512, 3))
-            self.assertLess(np.abs(expected_slice - upscaled_image[-3:, -3:, -1].flatten()).max(), 5e-3)
+        self.assertEqual(upscaled_image.shape, (512, 512, 3))
+        self.assertLess(np.abs(expected_slice - upscaled_image[-3:, -3:, -1].flatten()).max(), 5e-3)
```

### Comparing `optimum-habana-1.8.2/tests/test_encoder_decoder_text_summarization.py` & `optimum-habana-1.9.0/tests/test_encoder_decoder_text_summarization.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 from tempfile import TemporaryDirectory
 
 import pytest
 
 from .test_examples import ACCURACY_PERF_FACTOR, TIME_PERF_FACTOR
 
 
-if os.environ.get("GAUDI2_CI", "false") == "true":
+if os.environ.get("GAUDI2_CI", "0") == "1":
     # Gaudi2 CI baselines
     MODELS_TO_TEST = {
         "bf16": [
-            ("facebook/bart-large-cnn", "Habana/bart", 5.568, 26.0688, 2, 1),
+            ("facebook/bart-large-cnn", "Habana/bart", 4.691, 26.0688, 2, 1),
         ],
     }
 else:
     # Gaudi1 CI baselines
     MODELS_TO_TEST = {
         "bf16": [
             ("facebook/bart-large-cnn", "Habana/bart", 2.612, 26.3777, 2, 1),
```

### Comparing `optimum-habana-1.8.2/tests/test_examples.py` & `optimum-habana-1.9.0/tests/test_examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,14 +133,24 @@
         MODELS_TO_TEST_FOR_SEQ2SEQ,
     ),
     "run_clip": _get_supported_models_for_script(
         MODELS_TO_TEST_MAPPING,
         MODEL_MAPPING,
         MODELS_TO_TEST_FOR_IMAGE_TEXT,
     ),
+    "run_bridgetower": _get_supported_models_for_script(
+        MODELS_TO_TEST_MAPPING,
+        MODEL_MAPPING,
+        ["bridgetower"],
+    ),
+    "run_lora_clm": _get_supported_models_for_script(
+        MODELS_TO_TEST_MAPPING,
+        MODEL_FOR_CAUSAL_LM_MAPPING,
+        ["llama", "falcon"],
+    ),
 }
 
 
 class ExampleTestMeta(type):
     """
     Metaclass that takes care of creating the proper example tests for a given task.
     It uses example_name to figure out which models support this task, and create a run example test for each of these
@@ -150,29 +160,46 @@
     @staticmethod
     def to_test(model_name: str, multi_card: bool, deepspeed: bool, example_name: str):
         models_with_specific_rules = [
             "albert-xxlarge-v1",
             "gpt2-xl",
             "facebook/wav2vec2-base",
             "facebook/wav2vec2-large-lv60",
+            "BridgeTower/bridgetower-large-itm-mlm-itc",
+            "EleutherAI/gpt-neox-20b",
+            "google/flan-t5-xxl",
+            "tiiuae/falcon-40b",
+            "bigscience/bloom-7b1",
         ]
 
         if model_name not in models_with_specific_rules and not deepspeed:
             return True
         elif model_name == "gpt2-xl" and deepspeed:
             # GPT2-XL is tested only with DeepSpeed
             return True
+        elif "gpt-neox" in model_name and os.environ.get("GAUDI2_CI", "0") == "1" and deepspeed:
+            # GPT-NeoX is tested only on Gaudi2 and with DeepSpeed
+            return True
+        elif "flan-t5" in model_name and os.environ.get("GAUDI2_CI", "0") == "1" and deepspeed:
+            # Flan-T5 is tested only on Gaudi2 and with DeepSpeed
+            return True
         elif model_name == "albert-xxlarge-v1":
             if (("RUN_ALBERT_XXL_1X" in os.environ) and strtobool(os.environ["RUN_ALBERT_XXL_1X"])) or multi_card:
                 # ALBERT XXL 1X is tested only if the required flag is present because it takes long
                 return True
         elif "wav2vec2-base" in model_name and example_name == "run_audio_classification":
             return True
         elif "wav2vec2-large" in model_name and example_name == "run_speech_recognition_ctc":
             return True
+        elif "bridgetower" in model_name and os.environ.get("GAUDI2_CI", "0") == "1":
+            return True
+        elif "falcon" in model_name and os.environ.get("GAUDI2_CI", "0") == "1":
+            return True
+        elif "bloom" in model_name and deepspeed and os.environ.get("GAUDI2_CI", "0") == "0":
+            return True
 
         return False
 
     def __new__(cls, name, bases, attrs, example_name=None, multi_card=False, deepspeed=False):
         distribution = "single_card"
         if multi_card:
             distribution = "multi_card"
@@ -231,71 +258,57 @@
             if self.EXAMPLE_NAME == "run_esmfold":
                 p = subprocess.Popen(["python3", example_script])
                 return_code = p.wait()
 
                 # Ensure the run finished without any issue
                 self.assertEqual(return_code, 0)
                 return
-            # At the moment, just run the LORA example to check if there is no error
-            elif self.EXAMPLE_NAME == "run_lora_clm":
-                self._install_requirements(example_script.parent / "requirements.txt")
-
-                command = [
-                    "python3",
-                    # TODO: uncomment the following lines when LoRA 8x is fixed
-                    # f"{example_script.parent.parent / 'gaudi_spawn.py'}",
-                    # "--use_mpi",
-                    # "--world_size 8",
-                    f"{example_script}",
-                    "--model_name_or_path huggyllama/llama-7b",
-                    "--dataset_name tatsu-lab/alpaca",
-                    "--bf16",
-                    "--output_dir /tmp/model_lora_llama",
-                    "--num_train_epochs 1",
-                    "--per_device_train_batch_size 2",
-                    "--per_device_eval_batch_size 2",
-                    "--gradient_accumulation_steps 4",
-                    "--save_strategy no",
-                    "--learning_rate 1e-4",
-                    "--dataset_concatenation",
-                    "--do_train",
-                    "--use_habana",
-                    "--use_lazy_mode",
-                    "--throughput_warmup_steps 3",
-                    "--max_steps 100",
-                ]
-                pattern = re.compile(r"([\"\'].+?[\"\'])|\s")
-                command = [x for y in command for x in re.split(pattern, y) if x]
-                p = subprocess.Popen(command)
-                return_code = p.wait()
-
-                # Ensure the run finished without any issue
-                self.assertEqual(return_code, 0)
-                return
-            # The CLIP example requires COCO and a clip-roberta model
             elif self.EXAMPLE_NAME == "run_clip":
                 from .clip_coco_utils import create_clip_roberta_model, download_coco
 
                 download_coco()
                 create_clip_roberta_model()
 
             self._install_requirements(example_script.parent / "requirements.txt")
 
             path_to_baseline = BASELINE_DIRECTORY / Path(model_name.split("/")[-1].replace("-", "_")).with_suffix(
                 ".json"
             )
             with path_to_baseline.open("r") as json_file:
-                baseline = json.load(json_file)[self.TASK_NAME]
+                device = "gaudi2" if os.environ.get("GAUDI2_CI", "0") == "1" else "gaudi"
+                baseline = json.load(json_file)[device]
+                if isinstance(self.TASK_NAME, list):
+                    for key in self.TASK_NAME:
+                        if key in baseline:
+                            baseline = baseline[key]
+                            break
+                    if "num_train_epochs" not in baseline:
+                        raise ValueError(
+                            f"Couldn't find a baseline associated to any of these tasks: {self.TASK_NAME}."
+                        )
+                    self.TASK_NAME = key
+                else:
+                    baseline = baseline[self.TASK_NAME]
 
             distribution = "single_card"
             if multi_card:
                 distribution = "multi_card"
             elif deepspeed:
                 distribution = "deepspeed"
 
+            env_variables = os.environ.copy()
+            if "falcon" in model_name:
+                env_variables["LOWER_LIST"] = str(example_script.parent / "ops_bf16.txt")
+            elif "flan" in model_name:
+                env_variables["PT_HPU_MAX_COMPOUND_OP_SIZE"] = "512"
+            elif "bloom" in model_name:
+                env_variables["DEEPSPEED_HPU_ZERO3_SYNC_MARK_STEP_REQUIRED"] = "1"
+                env_variables["PT_HPU_MAX_COMPOUND_OP_SYNC"] = "1"
+                env_variables["PT_HPU_MAX_COMPOUND_OP_SIZE"] = "1"
+
             with TemporaryDirectory() as tmp_dir:
                 cmd_line = self._create_command_line(
                     multi_card,
                     deepspeed,
                     example_script,
                     model_name,
                     gaudi_config_name,
@@ -306,25 +319,25 @@
                     eval_batch_size=baseline.get("eval_batch_size"),
                     num_epochs=baseline.get("num_train_epochs"),
                     extra_command_line_arguments=baseline.get("distribution")
                     .get(distribution)
                     .get("extra_arguments", []),
                 )
 
-                p = subprocess.Popen(cmd_line)
+                p = subprocess.Popen(cmd_line, env=env_variables)
                 return_code = p.wait()
 
                 # Ensure the run finished without any issue
                 self.assertEqual(return_code, 0)
 
                 with open(Path(tmp_dir) / "all_results.json") as fp:
                     results = json.load(fp)
 
                 # Ensure performance requirements (accuracy, training time) are met
-                self.assert_no_regression(results, baseline.get("distribution").get(distribution))
+                self.assert_no_regression(results, baseline.get("distribution").get(distribution), model_name)
 
             # TODO: is a cleanup of the dataset cache needed?
             # self._cleanup_dataset_cache()
 
         return test
 
 
@@ -388,27 +401,29 @@
 
         cmd_line += [
             f"{script}",
             f"--model_name_or_path {model_name}",
             f"--gaudi_config_name {gaudi_config_name}",
             f"{task_option}",
             "--do_train",
-            "--do_eval",
             f"--output_dir {output_dir}",
             "--overwrite_output_dir",
             f"--learning_rate {lr}",
             f"--per_device_train_batch_size {train_batch_size}",
             f"--per_device_eval_batch_size {eval_batch_size}",
             f" --num_train_epochs {num_epochs}",
             "--use_habana",
             "--use_lazy_mode",
             "--throughput_warmup_steps 3",
             "--save_strategy no",
         ]
 
+        if "bloom" not in model_name:
+            cmd_line.append("--do_eval")
+
         if extra_command_line_arguments is not None:
             cmd_line += extra_command_line_arguments
 
         pattern = re.compile(r"([\"\'].+?[\"\'])|\s")
         return [x for y in cmd_line for x in re.split(pattern, y) if x]
 
     def _install_requirements(self, requirements_filename: Union[str, os.PathLike]):
@@ -420,29 +435,31 @@
             return
 
         cmd_line = f"pip install -r {requirements_filename}".split()
         p = subprocess.Popen(cmd_line)
         return_code = p.wait()
         self.assertEqual(return_code, 0)
 
-    def assert_no_regression(self, results: Dict, baseline: Dict):
+    def assert_no_regression(self, results: Dict, baseline: Dict, model_name: str):
         """
         Assert whether all possible performance requirements are met.
         Attributes:
             results (Dict): results of the run to assess
             baseline (Dict): baseline to assert whether or not there is regression
         """
         # Gather all the metrics to assess
         metrics_to_assess = []
         for metric_name in self.REGRESSION_METRICS.keys():
             if metric_name in baseline and metric_name in results:
                 metrics_to_assess.append(metric_name)
 
-        # There is no accuracy metric for `run_clip.py`
-        min_number_metrics = 2 if self.EXAMPLE_NAME == "run_clip" else 3
+        # There is no accuracy metric for `run_clip.py`, `run_bridgetower.py` and BLOOM
+        min_number_metrics = 3
+        if self.EXAMPLE_NAME in ["run_clip", "run_bridgetower"] or "bloom" in model_name:
+            min_number_metrics = 2
 
         # Check that at least 3 metrics are assessed:
         # training time + throughput + accuracy metric (F1, accuracy, perplexity,...)
         self.assertGreaterEqual(
             len(metrics_to_assess),
             min_number_metrics,
             (
@@ -527,30 +544,32 @@
 
 class MultiCardAudioClassificationExampleTester(
     ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_audio_classification", multi_card=True
 ):
     TASK_NAME = "common_language"
 
 
-# class SpeechRecognitionExampleTester(ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_speech_recognition_ctc"):
-#     TASK_NAME = "regisss/librispeech_asr_for_optimum_habana_ci"
-
-
 class MultiCardSpeechRecognitionExampleTester(
     ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_speech_recognition_ctc", multi_card=True
 ):
     TASK_NAME = "regisss/librispeech_asr_for_optimum_habana_ci"
 
 
 class MultiCardSummarizationExampleTester(
     ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_summarization", multi_card=True
 ):
     TASK_NAME = "cnn_dailymail"
 
 
+class DeepspeedSummarizationExampleTester(
+    ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_summarization", deepspeed=True
+):
+    TASK_NAME = "cnn_dailymail"
+
+
 class MultiCardSeq2SeqQuestionAnsweringExampleTester(
     ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_seq2seq_qa", multi_card=True
 ):
     TASK_NAME = "squad_v2"
 
 
 class MultiCardVisionLanguageExampleTester(
@@ -560,10 +579,16 @@
 
 
 class ProteinFoldingExampleTester(ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_esmfold"):
     pass
 
 
 class MultiCardCausalLanguageModelingLORAExampleTester(
-    ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_lora_clm"
+    ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_lora_clm", multi_card=True
 ):
-    pass
+    TASK_NAME = ["tatsu-lab/alpaca", "timdettmers/openassistant-guanaco"]
+
+
+class MultiCardBridgetowerExampleTester(
+    ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_bridgetower", multi_card=True
+):
+    TASK_NAME = "jmhessel/newyorker_caption_contest"
```

### Comparing `optimum-habana-1.8.2/tests/test_examples_match_transformers.py` & `optimum-habana-1.9.0/tests/test_examples_match_transformers.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.8.2/tests/test_gaudi_configuration.py` & `optimum-habana-1.9.0/tests/test_gaudi_configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,60 +13,61 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import filecmp
 import tempfile
 import unittest
 from pathlib import Path
-from typing import List
 
 from optimum.habana import GaudiConfig
 
 
 BF16_OPS_REFERENCE_FILE = Path(__file__).parent.resolve() / Path("configs/bf16_ops.txt")
 FP32_OPS_REFERENCE_FILE = Path(__file__).parent.resolve() / Path("configs/fp32_ops.txt")
 
 
-def is_list_of_strings(my_list: List) -> bool:
-    """
-    This method assesses whether an object is a list of strings or not.
-
-    Args:
-        my_list (List): list to assess
-
-    Returns:
-        bool: whether the input argument is a list of strings or not
-    """
-    if my_list and isinstance(my_list, list):
-        return all(isinstance(op, str) for op in my_list)
-    else:
-        return False
-
-
 class GaudiConfigTester(unittest.TestCase):
     """
     Unit tests for Gaudi configuration class GaudiConfig.
     """
 
     def test_default_parameter_types(self):
         gaudi_config = GaudiConfig()
 
-        self.assertIsInstance(gaudi_config.use_habana_mixed_precision, bool)
-        self.assertIsInstance(gaudi_config.hmp_is_verbose, bool)
         self.assertIsInstance(gaudi_config.use_fused_adam, bool)
         self.assertIsInstance(gaudi_config.use_fused_clip_norm, bool)
         self.assertIsInstance(gaudi_config.use_torch_autocast, bool)
 
-        self.assertTrue(is_list_of_strings(gaudi_config.hmp_bf16_ops))
-        self.assertTrue(is_list_of_strings(gaudi_config.hmp_fp32_ops))
         self.assertIsNone(gaudi_config.autocast_bf16_ops)
         self.assertIsNone(gaudi_config.autocast_fp32_ops)
 
     def test_write_bf16_fp32_ops_to_text_files(self):
-        gaudi_config = GaudiConfig()
+        gaudi_config = GaudiConfig(
+            autocast_bf16_ops=[
+                "add",
+                "addmm",
+                "bmm",
+                "div",
+                "dropout",
+                "gelu",
+                "iadd",
+                "linear",
+                "layer_norm",
+                "matmul",
+                "mm",
+                "rsub",
+                "softmax",
+                "truediv",
+            ],
+            autocast_fp32_ops=[
+                "embedding",
+                "nll_loss",
+                "log_softmax",
+            ],
+        )
 
         with tempfile.NamedTemporaryFile() as bf16_file:
             with tempfile.NamedTemporaryFile() as fp32_file:
                 gaudi_config.write_bf16_fp32_ops_to_text_files(
                     bf16_file.name,
                     fp32_file.name,
                 )
```

### Comparing `optimum-habana-1.8.2/tests/test_text_generation_example.py` & `optimum-habana-1.9.0/tests/test_text_generation_example.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,60 @@
 import json
+import os
 import re
 import subprocess
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 import pytest
 
 from .test_examples import TIME_PERF_FACTOR
 
 
-MODELS_TO_TEST = {
-    "bf16": [
-        ("bigscience/bloomz-7b1", 41.93942748147396),
-        ("gpt2-xl", 126.6292071377241),
-        # TODO: fix OPT 6.7B
-        # ("facebook/opt-6.7b", 0.0),
-        ("EleutherAI/gpt-j-6b", 37.14562499113717),
-        # TODO: GPT-NeoX doesn't fit on 1 Gaudi1 card
-        # ("EleutherAI/gpt-neox-20b", 0.0),
-        ("meta-llama/Llama-2-7b-hf", 43.951804139391925),
-        ("tiiuae/falcon-7b", 44.288602257903726),
-        ("bigcode/starcoder", 15.955986010526113),
-        ("Salesforce/codegen2-1B", 109.03016111561857),
-        ("mosaicml/mpt-7b", 44.888696119070424),
-    ],
-    "deepspeed": [
-        ("bigscience/bloomz-7b1", 27.34439410425298),
-    ],
-}
+if os.environ.get("GAUDI2_CI", "0") == "1":
+    # Gaudi2 CI baselines
+    MODELS_TO_TEST = {
+        "bf16": [
+            ("bigscience/bloomz-7b1", 129.80481357662882),
+            ("gpt2-xl", 272.3868331435149),
+            ("EleutherAI/gpt-j-6b", 137.46821395745388),
+            ("EleutherAI/gpt-neox-20b", 50.236713606109355),
+            ("meta-llama/Llama-2-7b-hf", 139.82510055437686),
+            ("tiiuae/falcon-40b", 25.260978255750498),
+            ("bigcode/starcoder", 65.38483087362695),
+            ("Salesforce/codegen2-1B", 231.1951513223901),
+            ("mosaicml/mpt-30b", 35.825021595560855),
+            ("mistralai/Mistral-7B-v0.1", 113.64661982817469),
+        ],
+        "deepspeed": [
+            ("bigscience/bloomz", 33.05719168230658),
+            ("meta-llama/Llama-2-70b-hf", 58.2750262232098),
+            ("facebook/opt-66b", 28.16154122335556),
+        ],
+    }
+else:
+    # Gaudi1 CI baselines
+    MODELS_TO_TEST = {
+        "bf16": [
+            ("bigscience/bloomz-7b1", 41.93942748147396),
+            ("gpt2-xl", 126.6292071377241),
+            # TODO: fix OPT 6.7B
+            # ("facebook/opt-6.7b", 0.0),
+            ("EleutherAI/gpt-j-6b", 37.14562499113717),
+            ("meta-llama/Llama-2-7b-hf", 43.951804139391925),
+            ("tiiuae/falcon-7b", 44.288602257903726),
+            ("bigcode/starcoder", 15.955986010526113),
+            ("Salesforce/codegen2-1B", 109.03016111561857),
+            ("mosaicml/mpt-7b", 44.888696119070424),
+            ("mistralai/Mistral-7B-v0.1", 40.0690067247771),
+        ],
+        "deepspeed": [
+            ("bigscience/bloomz-7b1", 27.34439410425298),
+        ],
+    }
 
 
 def _test_text_generation(model_name: str, baseline: float, token: str, deepspeed: bool = False, world_size: int = 8):
     command = ["python3"]
     path_to_example_dir = Path(__file__).resolve().parent.parent / "examples"
 
     if deepspeed:
@@ -49,14 +72,17 @@
         "--use_kv_cache",
         "--max_new_tokens 100",
     ]
 
     if not deepspeed:
         command.append("--bf16")
 
+    if "falcon" in model_name:
+        command.append("--skip_hash_with_views")
+
     with TemporaryDirectory() as tmp_dir:
         command.append(f"--output_dir {tmp_dir}")
         print(f"\n\nCommand to test: {' '.join(command)}\n")
 
         command.append(f"--token {token.value}")
 
         pattern = re.compile(r"([\"\'].+?[\"\'])|\s")
@@ -83,8 +109,9 @@
 @pytest.mark.parametrize("model_name, baseline", MODELS_TO_TEST["bf16"])
 def test_text_generation_bf16(model_name: str, baseline: float, token: str):
     _test_text_generation(model_name, baseline, token)
 
 
 @pytest.mark.parametrize("model_name, baseline", MODELS_TO_TEST["deepspeed"])
 def test_text_generation_deepspeed(model_name: str, baseline: float, token: str):
-    _test_text_generation(model_name, baseline, token, deepspeed=True)
+    world_size = 2 if "opt-66b" in model_name else 8
+    _test_text_generation(model_name, baseline, token, deepspeed=True, world_size=world_size)
```

### Comparing `optimum-habana-1.8.2/tests/test_trainer.py` & `optimum-habana-1.9.0/tests/test_trainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import random
 import re
 import subprocess
 import tempfile
 import unittest
 from itertools import product
 from pathlib import Path
-from typing import Optional, Union
+from typing import Dict, List, Optional, Union
 
 import numpy as np
 from huggingface_hub import HfFolder, delete_repo, list_repo_commits
 from parameterized import parameterized
 from requests.exceptions import HTTPError
 from transformers import IntervalStrategy, PretrainedConfig, is_torch_available
 from transformers.hyperparameter_search import ALL_HYPERPARAMETER_SEARCH_BACKENDS
@@ -93,14 +93,34 @@
 
     def __getitem__(self, i):
         result = {name: y[i] for name, y in zip(self.label_names, self.ys)}
         result["input_x"] = self.x[i]
         return result
 
 
+class RegressionDatasetDynamic:
+    def __init__(self, a=2, b=3, length=128, seed=42, label_names=None):
+        np.random.seed(seed)
+        self.label_names = ["labels"] if label_names is None else label_names
+        self.length = length
+        self.a = a
+        self.b = b
+
+    def __len__(self):
+        return self.length
+
+    def __getitem__(self, i):
+        self.x = np.random.normal(size=(self.length + i,)).astype(np.float32)
+        self.ys = self.a * self.x + self.b + np.random.normal(scale=0.1, size=(self.length + i,)).astype(np.float32)
+        result = {}
+        result["labels"] = self.ys
+        result["input_x"] = self.x
+        return result
+
+
 @dataclasses.dataclass
 class RegressionGaudiTrainingArguments(GaudiTrainingArguments):
     a: float = 0.0
     b: float = 0.0
 
     def __post_init__(self):
         # save resources not dealing with reporting (also avoids the warning when it's not set)
@@ -116,14 +136,30 @@
     def __len__(self):
         return self.length
 
     def __getitem__(self, i):
         return {"input_ids": self.x, "labels": self.x}
 
 
+class DynamicShapesDataset:
+    def __init__(self, length=64, seed=42, batch_size=8):
+        self.length = length
+        np.random.seed(seed)
+        sizes = np.random.randint(1, 20, (length // batch_size,))
+        # For easy batching, we make every batch_size consecutive samples the same size.
+        self.xs = [np.random.normal(size=(s,)) for s in sizes.repeat(batch_size)]
+        self.ys = [np.random.normal(size=(s,)) for s in sizes.repeat(batch_size)]
+
+    def __len__(self):
+        return self.length
+
+    def __getitem__(self, i):
+        return {"input_x": self.xs[i], "labels": self.ys[i]}
+
+
 class AlmostAccuracy:
     def __init__(self, thresh=0.25):
         self.thresh = thresh
 
     def __call__(self, eval_pred):
         predictions, labels = eval_pred
         true = np.abs(predictions - labels) <= self.thresh
@@ -688,14 +724,16 @@
         gaudi_config = get_gaudi_config()
         args = GaudiTrainingArguments(
             "./regression",
             use_habana=True,
             use_lazy_mode=True,
             use_hpu_graphs_for_training=True,
             use_hpu_graphs_for_inference=True,
+            disable_tensor_cache_hpu_graphs=True,
+            max_hpu_graphs=1,
         )
         trainer = GaudiTrainer(model, gaudi_config, args, train_dataset=train_dataset, eval_dataset=eval_dataset)
         trainer.train()
         _ = trainer.evaluate()
         _ = trainer.predict(eval_dataset)
 
     def test_trainer_works_with_dict(self):
@@ -925,49 +963,91 @@
         x = trainer.eval_dataset.x
         self.assertEqual(len(preds), 2)
         self.assertTrue(np.allclose(preds[0], 1.5 * x + 2.5))
         self.assertTrue(np.allclose(preds[1], 1.5 * x + 2.5))
         self.assertTrue(np.array_equal(labels[0], trainer.eval_dataset.ys[0]))
         self.assertTrue(np.array_equal(labels[1], trainer.eval_dataset.ys[1]))
 
-    # def test_dynamic_shapes(self):
-    #     eval_dataset = DynamicShapesDataset(batch_size=self.batch_size)
-    #     model = RegressionModel(a=2, b=1)
-    #     args = TrainingArguments("./regression")
-    #     trainer = Trainer(model, args, eval_dataset=eval_dataset)
-
-    #     # Check evaluation can run to completion
-    #     _ = trainer.evaluate()
-
-    #     # Check predictions
-    #     preds = trainer.predict(eval_dataset)
-    #     for expected, seen in zip(eval_dataset.ys, preds.label_ids):
-    #         self.assertTrue(np.array_equal(expected, seen[: expected.shape[0]]))
-    #         self.assertTrue(np.all(seen[expected.shape[0] :] == -100))
-
-    #     for expected, seen in zip(eval_dataset.xs, preds.predictions):
-    #         self.assertTrue(np.array_equal(2 * expected + 1, seen[: expected.shape[0]]))
-    #         self.assertTrue(np.all(seen[expected.shape[0] :] == -100))
-
-    #     # Same tests with eval accumulation
-    #     args = TrainingArguments("./regression", eval_accumulation_steps=2)
-    #     trainer = Trainer(model, args, eval_dataset=eval_dataset)
-
-    #     # Check evaluation can run to completion
-    #     _ = trainer.evaluate()
-
-    #     # Check predictions
-    #     preds = trainer.predict(eval_dataset)
-    #     for expected, seen in zip(eval_dataset.ys, preds.label_ids):
-    #         self.assertTrue(np.array_equal(expected, seen[: expected.shape[0]]))
-    #         self.assertTrue(np.all(seen[expected.shape[0] :] == -100))
-
-    #     for expected, seen in zip(eval_dataset.xs, preds.predictions):
-    #         self.assertTrue(np.array_equal(2 * expected + 1, seen[: expected.shape[0]]))
-    #         self.assertTrue(np.all(seen[expected.shape[0] :] == -100))
+    def test_dynamic_shapes(self):
+        eval_dataset = DynamicShapesDataset(batch_size=self.batch_size)
+        model = RegressionModel(a=2, b=1)
+        args = GaudiTrainingArguments("./regression", use_habana=True, use_lazy_mode=True)
+        gaudi_config = get_gaudi_config()
+        gaudi_config.use_dynamic_shapes = True
+        trainer = GaudiTrainer(model, gaudi_config, args, eval_dataset=eval_dataset)
+
+        # Check evaluation can run to completion
+        _ = trainer.evaluate()
+
+        # Check predictions
+        preds = trainer.predict(eval_dataset)
+        for expected, seen in zip(eval_dataset.ys, preds.label_ids):
+            self.assertTrue(np.allclose(expected, seen[: expected.shape[0]]))
+            self.assertTrue(np.all(seen[expected.shape[0] :] == -100))
+
+        for expected, seen in zip(eval_dataset.xs, preds.predictions):
+            self.assertTrue(np.allclose(2 * expected + 1, seen[: expected.shape[0]]))
+            self.assertTrue(np.all(seen[expected.shape[0] :] == -100))
+
+        # Same tests with eval accumulation
+        args = GaudiTrainingArguments("./regression", use_habana=True, use_lazy_mode=True, eval_accumulation_steps=2)
+        trainer = GaudiTrainer(model, gaudi_config, args, eval_dataset=eval_dataset)
+
+        # Check evaluation can run to completion
+        _ = trainer.evaluate()
+
+        # Check predictions
+        preds = trainer.predict(eval_dataset)
+        for expected, seen in zip(eval_dataset.ys, preds.label_ids):
+            self.assertTrue(np.allclose(expected, seen[: expected.shape[0]]))
+            self.assertTrue(np.all(seen[expected.shape[0] :] == -100))
+
+        for expected, seen in zip(eval_dataset.xs, preds.predictions):
+            self.assertTrue(np.allclose(2 * expected + 1, seen[: expected.shape[0]]))
+            self.assertTrue(np.all(seen[expected.shape[0] :] == -100))
+
+    def test_dynamic_shape_feature(self):
+        # Run training with variable length inputs and enable dynamic shapes support
+        train_dataset = RegressionDatasetDynamic(length=256)
+        gaudi_config = get_gaudi_config()
+        gaudi_config.use_dynamic_shapes = True
+        args = GaudiTrainingArguments(
+            "./regression", use_habana=True, use_lazy_mode=True, per_device_train_batch_size=1, num_train_epochs=1
+        )
+        model = RegressionModel()
+        trainer = GaudiTrainer(
+            model,
+            gaudi_config,
+            args,
+            train_dataset=train_dataset,
+        )
+        train_output_ds = trainer.train()
+
+        # Run training again with variable length inputs and disable dynamic shapes support
+        train_dataset = RegressionDatasetDynamic(length=256)
+        gaudi_config = get_gaudi_config()
+        gaudi_config.use_dynamic_shapes = False
+        args = GaudiTrainingArguments(
+            "./regression", use_habana=True, use_lazy_mode=True, per_device_train_batch_size=1, num_train_epochs=1
+        )
+        model = RegressionModel()
+        trainer = GaudiTrainer(
+            model,
+            gaudi_config,
+            args,
+            train_dataset=train_dataset,
+        )
+        train_output_static = trainer.train()
+
+        # Check if performance with dynamic shapes support is at least 5 times that without dynamic shapes
+        # Note "5x" number is not applicable across models, it is tuned for this particular dummy model
+        self.assertGreaterEqual(
+            train_output_ds.metrics["train_samples_per_second"],
+            5 * train_output_static.metrics["train_samples_per_second"],
+        )
 
     def test_log_level(self):
         # testing only --log_level (--log_level_replica requires multiple gpus and DDP and is tested elsewhere)
         logger = logging.get_logger()
         log_info_string = "Running training"
 
         # test with the default log_level - should be the same as before and thus we test depending on is_info
@@ -1599,17 +1679,15 @@
 
     def test_no_wd_param_group(self):
         model = nn.Sequential(TstLayer(128), nn.ModuleList([TstLayer(128), TstLayer(128)]))
         gaudi_config = get_gaudi_config()
         args = GaudiTrainingArguments(output_dir="./test", use_habana=True, use_lazy_mode=True)
         trainer = GaudiTrainer(model=model, gaudi_config=gaudi_config, args=args)
         trainer.create_optimizer_and_scheduler(10)
-        # fmt: off
-        wd_names = ['0.linear1.weight', '0.linear2.weight', '1.0.linear1.weight', '1.0.linear2.weight', '1.1.linear1.weight', '1.1.linear2.weight']
-        # fmt: on
+        wd_names = ['0.linear1.weight', '0.linear2.weight', '1.0.linear1.weight', '1.0.linear2.weight', '1.1.linear1.weight', '1.1.linear2.weight']  # fmt: skip
         wd_params = [p for n, p in model.named_parameters() if n in wd_names]
         no_wd_params = [p for n, p in model.named_parameters() if n not in wd_names]
         self.assertListEqual(trainer.optimizer.param_groups[0]["params"], wd_params)
         self.assertListEqual(trainer.optimizer.param_groups[1]["params"], no_wd_params)
 
     def test_profiling(self):
         # 24 total steps and compilation takes place during the 1st three steps
@@ -1779,14 +1857,70 @@
                 logging_dir="runs",
                 run_name="test",
                 model_init=model_init,
             )
             trainer.hyperparameter_search(direction="minimize", hp_space=hp_space, hp_name=hp_name, n_trials=4)
 
 
+@require_torch
+@require_optuna
+class TrainerHyperParameterMultiObjectOptunaIntegrationTest(unittest.TestCase):
+    def setUp(self):
+        args = GaudiTrainingArguments("..", use_habana=True, use_lazy_mode=True)
+        self.n_epochs = args.num_train_epochs
+        self.batch_size = args.train_batch_size
+
+    def test_hyperparameter_search(self):
+        class MyTrialShortNamer(TrialShortNamer):
+            DEFAULTS = {"a": 0, "b": 0}
+
+        def hp_space(trial):
+            return {}
+
+        def model_init(trial):
+            if trial is not None:
+                a = trial.suggest_int("a", -4, 4)
+                b = trial.suggest_int("b", -4, 4)
+            else:
+                a = 0
+                b = 0
+            config = RegressionModelConfig(a=a, b=b, double_output=False)
+
+            return RegressionPreTrainedModel(config)
+
+        def hp_name(trial):
+            return MyTrialShortNamer.shortname(trial.params)
+
+        def compute_objective(metrics: Dict[str, float]) -> List[float]:
+            return metrics["eval_loss"], metrics["eval_accuracy"]
+
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            trainer = get_regression_trainer(
+                output_dir=tmp_dir,
+                learning_rate=0.1,
+                logging_steps=1,
+                evaluation_strategy=IntervalStrategy.EPOCH,
+                save_strategy=IntervalStrategy.EPOCH,
+                num_train_epochs=10,
+                disable_tqdm=True,
+                load_best_model_at_end=True,
+                logging_dir="runs",
+                run_name="test",
+                model_init=model_init,
+                compute_metrics=AlmostAccuracy(),
+            )
+            trainer.hyperparameter_search(
+                direction=["minimize", "maximize"],
+                hp_space=hp_space,
+                hp_name=hp_name,
+                n_trials=4,
+                compute_objective=compute_objective,
+            )
+
+
 # TODO: crashes because `TypeError: cannot pickle 'PyCapsule' object`
 # @require_torch
 # @require_ray
 # class GaudiTrainerHyperParameterRayIntegrationTest(unittest.TestCase):
 #     def setUp(self):
 #         args = GaudiTrainingArguments("..", use_habana=True, use_lazy_mode=True)
 #         self.n_epochs = args.num_train_epochs
```

### Comparing `optimum-habana-1.8.2/tests/test_trainer_distributed.py` & `optimum-habana-1.9.0/tests/test_trainer_distributed.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.8.2/tests/test_trainer_seq2seq.py` & `optimum-habana-1.9.0/tests/test_trainer_seq2seq.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,27 +23,40 @@
 if is_datasets_available():
     import datasets
 
 
 class GaudiSeq2seqTrainerTester(TestCasePlus):
     @require_torch
     def test_finetune_t5(self):
-        model = T5ForConditionalGeneration.from_pretrained("hf-internal-testing/tiny-random-t5-v1.1")
-        tokenizer = AutoTokenizer.from_pretrained("t5-small")
-
-        model.config.max_length = 128
-
         train_dataset = datasets.load_dataset("cnn_dailymail", "3.0.0", split="train[:1%]")
         val_dataset = datasets.load_dataset("cnn_dailymail", "3.0.0", split="validation[:1%]")
 
         train_dataset = train_dataset.select(range(32))
         val_dataset = val_dataset.select(range(16))
 
         batch_size = 4
 
+        training_args = GaudiSeq2SeqTrainingArguments(
+            output_dir=self.get_auto_remove_tmp_dir(),
+            gaudi_config_name="Habana/t5",
+            per_device_train_batch_size=batch_size,
+            per_device_eval_batch_size=batch_size,
+            predict_with_generate=True,
+            do_train=True,
+            do_eval=True,
+            use_habana=True,
+            use_lazy_mode=True,
+            use_hpu_graphs_for_inference=True,
+        )
+
+        model = T5ForConditionalGeneration.from_pretrained("hf-internal-testing/tiny-random-t5-v1.1")
+        tokenizer = AutoTokenizer.from_pretrained("t5-small")
+
+        model.config.max_length = 128
+
         def _map_to_encoder_decoder_inputs(batch):
             # Tokenizer will automatically set [BOS] <text> [EOS]
             inputs = tokenizer(batch["article"], padding="max_length", truncation=True, max_length=512)
             outputs = tokenizer(batch["highlights"], padding="max_length", truncation=True, max_length=128)
             batch["input_ids"] = inputs.input_ids
             batch["attention_mask"] = inputs.attention_mask
 
@@ -88,29 +101,14 @@
             remove_columns=["article", "highlights"],
         )
         val_dataset.set_format(
             type="torch",
             columns=["input_ids", "attention_mask", "decoder_input_ids", "labels"],
         )
 
-        output_dir = self.get_auto_remove_tmp_dir()
-
-        training_args = GaudiSeq2SeqTrainingArguments(
-            output_dir=output_dir,
-            gaudi_config_name="Habana/t5",
-            per_device_train_batch_size=batch_size,
-            per_device_eval_batch_size=batch_size,
-            predict_with_generate=True,
-            do_train=True,
-            do_eval=True,
-            use_habana=True,
-            use_lazy_mode=True,
-            use_hpu_graphs_for_inference=True,
-        )
-
         # instantiate trainer
         trainer = GaudiSeq2SeqTrainer(
             model=model,
             args=training_args,
             compute_metrics=_compute_metrics,
             train_dataset=train_dataset,
             eval_dataset=val_dataset,
```

