# Comparing `tmp/langfun-0.0.2.dev20240418.tar.gz` & `tmp/langfun-0.0.2.dev20240419.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfun-0.0.2.dev20240418.tar", last modified: Thu Apr 18 08:04:33 2024, max compression
+gzip compressed data, was "langfun-0.0.2.dev20240419.tar", last modified: Fri Apr 19 08:03:47 2024, max compression
```

## Comparing `langfun-0.0.2.dev20240418.tar` & `langfun-0.0.2.dev20240419.tar`

### file list

```diff
@@ -1,122 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:04:33.461948 langfun-0.0.2.dev20240418/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-18 08:04:33.461948 langfun-0.0.2.dev20240418/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:04:33.445948 langfun-0.0.2.dev20240418/langfun/
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:04:33.449948 langfun-0.0.2.dev20240418/langfun/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:04:33.449948 langfun-0.0.2.dev20240418/langfun/core/coding/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/coding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:04:33.453948 langfun-0.0.2.dev20240418/langfun/core/coding/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/coding/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/coding/python/correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/coding/python/correction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/coding/python/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/coding/python/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/coding/python/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/coding/python/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/coding/python/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/coding/python/generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/coding/python/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/coding/python/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/coding/python/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/coding/python/permissions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/component_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:04:33.453948 langfun-0.0.2.dev20240418/langfun/core/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55359 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/eval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21592 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/eval/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/eval/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/eval/matching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/eval/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/eval/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/langfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/langfunc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17510 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/language_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:04:33.457949 langfun-0.0.2.dev20240418/langfun/core/llms/
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/llms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:04:33.457949 langfun-0.0.2.dev20240418/langfun/core/llms/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/llms/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/llms/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/llms/cache/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/llms/cache/in_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/llms/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/llms/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/llms/google_genai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/llms/google_genai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/llms/llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/llms/llama_cpp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11463 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/llms/openai_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:04:33.457949 langfun-0.0.2.dev20240418/langfun/core/memories/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/memories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/memories/conversation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/memories/conversation_history_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/message_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:04:33.457949 langfun-0.0.2.dev20240418/langfun/core/modalities/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/modalities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/modalities/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/modalities/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/modalities/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/modalities/mime_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/modalities/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/modalities/video_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/modality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/modality_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/natural_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/natural_language_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/sampling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:04:33.461948 langfun-0.0.2.dev20240418/langfun/core/structured/
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/structured/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19301 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/structured/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/structured/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/structured/description_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/structured/function_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/structured/function_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/structured/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/structured/mapping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/structured/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20980 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/structured/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/structured/prompting.py
--rw-r--r--   0 runner    (1001) docker     (127)    19945 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/structured/prompting_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    25057 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/structured/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/structured/schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/structured/schema_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22360 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/structured/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/structured/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/structured/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/subscription_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17662 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    13572 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/template_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:04:33.461948 langfun-0.0.2.dev20240418/langfun/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/templates/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/templates/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/templates/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/templates/conversation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/templates/demonstration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/templates/demonstration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/templates/selfplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/templates/selfplay_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/text_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/langfun/core/text_formatting_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:04:33.461948 langfun-0.0.2.dev20240418/langfun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-18 08:04:33.000000 langfun-0.0.2.dev20240418/langfun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-04-18 08:04:33.000000 langfun-0.0.2.dev20240418/langfun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 08:04:33.000000 langfun-0.0.2.dev20240418/langfun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-18 08:04:33.000000 langfun-0.0.2.dev20240418/langfun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 08:04:33.000000 langfun-0.0.2.dev20240418/langfun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 08:04:33.461948 langfun-0.0.2.dev20240418/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-18 08:04:16.000000 langfun-0.0.2.dev20240418/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.283416 langfun-0.0.2.dev20240419/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-19 08:03:47.283416 langfun-0.0.2.dev20240419/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.263416 langfun-0.0.2.dev20240419/langfun/
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.271416 langfun-0.0.2.dev20240419/langfun/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.271416 langfun-0.0.2.dev20240419/langfun/core/coding/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.271416 langfun-0.0.2.dev20240419/langfun/core/coding/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/correction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/permissions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.275416 langfun-0.0.2.dev20240419/langfun/core/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55359 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/eval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21592 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/eval/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/eval/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/eval/matching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/eval/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/eval/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/langfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/langfunc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18331 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/language_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.275416 langfun-0.0.2.dev20240419/langfun/core/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/anthropic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.275416 langfun-0.0.2.dev20240419/langfun/core/llms/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/cache/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/cache/in_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/google_genai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/google_genai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/llama_cpp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11463 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/openai_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.275416 langfun-0.0.2.dev20240419/langfun/core/memories/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/memories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/memories/conversation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/memories/conversation_history_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/message_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.279416 langfun-0.0.2.dev20240419/langfun/core/modalities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/modalities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/modalities/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/modalities/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/modalities/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/modalities/mime_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/modalities/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/modalities/video_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/modality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/modality_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/natural_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/natural_language_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/sampling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.283416 langfun-0.0.2.dev20240419/langfun/core/structured/
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19301 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/description_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/function_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/function_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/mapping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20980 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/prompting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19945 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/prompting_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25057 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/schema_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22360 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/subscription_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17662 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13572 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/template_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.283416 langfun-0.0.2.dev20240419/langfun/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/templates/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/templates/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/templates/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/templates/conversation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/templates/demonstration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/templates/demonstration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/templates/selfplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/templates/selfplay_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/text_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/text_formatting_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.283416 langfun-0.0.2.dev20240419/langfun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-19 08:03:47.000000 langfun-0.0.2.dev20240419/langfun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-19 08:03:47.000000 langfun-0.0.2.dev20240419/langfun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:03:47.000000 langfun-0.0.2.dev20240419/langfun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-19 08:03:47.000000 langfun-0.0.2.dev20240419/langfun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 08:03:47.000000 langfun-0.0.2.dev20240419/langfun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 08:03:47.283416 langfun-0.0.2.dev20240419/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/setup.py
```

### Comparing `langfun-0.0.2.dev20240418/LICENSE` & `langfun-0.0.2.dev20240419/LICENSE`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/PKG-INFO` & `langfun-0.0.2.dev20240419/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240418
+Version: 0.0.2.dev20240419
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240418/README.md` & `langfun-0.0.2.dev20240419/README.md`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/__init__.py` & `langfun-0.0.2.dev20240419/langfun/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/__init__.py` & `langfun-0.0.2.dev20240419/langfun/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/coding/__init__.py` & `langfun-0.0.2.dev20240419/langfun/core/coding/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/coding/python/__init__.py` & `langfun-0.0.2.dev20240419/langfun/core/coding/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/coding/python/correction.py` & `langfun-0.0.2.dev20240419/langfun/core/coding/python/correction.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/coding/python/correction_test.py` & `langfun-0.0.2.dev20240419/langfun/core/coding/python/correction_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/coding/python/errors.py` & `langfun-0.0.2.dev20240419/langfun/core/coding/python/errors.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/coding/python/errors_test.py` & `langfun-0.0.2.dev20240419/langfun/core/coding/python/errors_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/coding/python/execution.py` & `langfun-0.0.2.dev20240419/langfun/core/coding/python/execution.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/coding/python/execution_test.py` & `langfun-0.0.2.dev20240419/langfun/core/coding/python/execution_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/coding/python/generation.py` & `langfun-0.0.2.dev20240419/langfun/core/coding/python/generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/coding/python/generation_test.py` & `langfun-0.0.2.dev20240419/langfun/core/coding/python/generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/coding/python/parsing.py` & `langfun-0.0.2.dev20240419/langfun/core/coding/python/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/coding/python/parsing_test.py` & `langfun-0.0.2.dev20240419/langfun/core/coding/python/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/coding/python/permissions.py` & `langfun-0.0.2.dev20240419/langfun/core/coding/python/permissions.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/coding/python/permissions_test.py` & `langfun-0.0.2.dev20240419/langfun/core/coding/python/permissions_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/component.py` & `langfun-0.0.2.dev20240419/langfun/core/component.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/component_test.py` & `langfun-0.0.2.dev20240419/langfun/core/component_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/concurrent.py` & `langfun-0.0.2.dev20240419/langfun/core/concurrent.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/concurrent_test.py` & `langfun-0.0.2.dev20240419/langfun/core/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/console.py` & `langfun-0.0.2.dev20240419/langfun/core/console.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/console_test.py` & `langfun-0.0.2.dev20240419/langfun/core/console_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/eval/__init__.py` & `langfun-0.0.2.dev20240419/langfun/core/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/eval/base.py` & `langfun-0.0.2.dev20240419/langfun/core/eval/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/eval/base_test.py` & `langfun-0.0.2.dev20240419/langfun/core/eval/base_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/eval/matching.py` & `langfun-0.0.2.dev20240419/langfun/core/eval/matching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/eval/matching_test.py` & `langfun-0.0.2.dev20240419/langfun/core/eval/matching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/eval/scoring.py` & `langfun-0.0.2.dev20240419/langfun/core/eval/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/eval/scoring_test.py` & `langfun-0.0.2.dev20240419/langfun/core/eval/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/langfunc.py` & `langfun-0.0.2.dev20240419/langfun/core/langfunc.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/langfunc_test.py` & `langfun-0.0.2.dev20240419/langfun/core/langfunc_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/language_model.py` & `langfun-0.0.2.dev20240419/langfun/core/language_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -436,70 +436,96 @@
       response = result.samples[0].response
       logprobs = result.samples[0].logprobs
       response.set('score', result.samples[0].score)
       response.metadata.logprobs = logprobs
       response.metadata.usage = result.usage
 
       elapse = time.time() - request_start
-      self._debug(prompt, response, call_counter, elapse)
+      self._debug(prompt, response, call_counter, result.usage, elapse)
       return response
 
   def _debug(
       self,
       prompt: message_lib.Message,
       response: message_lib.Message,
       call_counter: int,
+      usage: LMSamplingUsage | None,
       elapse: float,
-  ):
+  ) -> None:
     """Outputs debugging information."""
     debug = self.debug
     if isinstance(debug, bool):
       debug = LMDebugMode.ALL if debug else LMDebugMode.NONE
 
     if debug & LMDebugMode.INFO:
-      self._debug_model_info(call_counter)
+      self._debug_model_info(call_counter, usage)
 
     if debug & LMDebugMode.PROMPT:
-      self._debug_prompt(prompt, call_counter)
+      self._debug_prompt(prompt, call_counter, usage)
 
     if debug & LMDebugMode.RESPONSE:
-      self._debug_response(response, call_counter, elapse)
+      self._debug_response(response, call_counter, usage, elapse)
 
-  def _debug_model_info(self, call_counter: int):
+  def _debug_model_info(
+      self, call_counter: int, usage: LMSamplingUsage | None) -> None:
     """Outputs debugging information about the model."""
+    title_suffix = ''
+    if usage and usage.total_tokens != 0:
+      title_suffix = console.colored(
+          f' (total {usage.total_tokens} tokens)', 'red')
+
     console.write(
         self.format(compact=True, use_inferred=True),
-        title=f'[{call_counter}] LM INFO:',
+        title=f'[{call_counter}] LM INFO{title_suffix}:',
         color='magenta',
     )
 
-  def _debug_prompt(self, prompt: message_lib.Message, call_counter: int):
+  def _debug_prompt(
+      self,
+      prompt: message_lib.Message,
+      call_counter: int,
+      usage: LMSamplingUsage | None,
+  ) -> None:
     """Outputs debugging information about the prompt."""
+    title_suffix = ''
+    if usage and usage.prompt_tokens != 0:
+      title_suffix = console.colored(f' ({usage.prompt_tokens} tokens)', 'red')
+
     console.write(
         prompt,
-        title=f'\n[{call_counter}] PROMPT SENT TO LM:',
+        title=f'\n[{call_counter}] PROMPT SENT TO LM{title_suffix}:',
         color='green',
     )
     referred_modalities = prompt.referred_modalities()
     if referred_modalities:
       console.write(
           pg.object_utils.kvlist_str(
               [(k, repr(v), None) for k, v in referred_modalities.items()]
           ),
           title=f'\n[{call_counter}] MODALITY OBJECTS SENT TO LM:',
           color='green',
       )
 
   def _debug_response(
-      self, response: message_lib.Message, call_counter: int, elapse: float
-  ):
+      self,
+      response: message_lib.Message,
+      call_counter: int,
+      usage: LMSamplingUsage | None,
+      elapse: float
+  ) -> None:
     """Outputs debugging information about the response."""
+    title_suffix = ' ('
+    if usage and usage.completion_tokens != 0:
+      title_suffix += f'{usage.completion_tokens} tokens '
+    title_suffix += f'in {elapse:.2f} seconds)'
+    title_suffix = console.colored(title_suffix, 'red')
+
     console.write(
         str(response) + '\n',
-        title=f'\n[{call_counter}] LM RESPONSE (in {elapse:.2f} seconds):',
+        title=f'\n[{call_counter}] LM RESPONSE{title_suffix}:',
         color='blue',
     )
 
   def score(
       self,
       prompt: str | message_lib.Message,
       completions: list[str | message_lib.Message],
@@ -538,15 +564,15 @@
       elapse: float,
   ):
     debug = self.debug
     if isinstance(debug, bool):
       debug = LMDebugMode.ALL if debug else LMDebugMode.NONE
 
     if debug & LMDebugMode.INFO:
-      self._debug_model_info(call_counter)
+      self._debug_model_info(call_counter, None)
 
     if debug & LMDebugMode.PROMPT:
       console.write(
           prompt,
           title=f'\n[{call_counter}] SCORING LM WITH PROMPT:',
           color='green',
       )
```

### Comparing `langfun-0.0.2.dev20240418/langfun/core/language_model_test.py` & `langfun-0.0.2.dev20240419/langfun/core/language_model_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/llms/__init__.py` & `langfun-0.0.2.dev20240419/langfun/core/llms/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,20 @@
 from langfun.core.llms.openai import Gpt35
 
 from langfun.core.llms.openai import Gpt3
 from langfun.core.llms.openai import Gpt3Curie
 from langfun.core.llms.openai import Gpt3Babbage
 from langfun.core.llms.openai import Gpt3Ada
 
+from langfun.core.llms.anthropic import Anthropic
+from langfun.core.llms.anthropic import Claude3Opus
+from langfun.core.llms.anthropic import Claude3Sonnet
+from langfun.core.llms.anthropic import Claude3Haiku
+
+
 # LLaMA C++ models.
 from langfun.core.llms.llama_cpp import LlamaCppRemote
 
 # Placeholder for Google-internal imports.
 
 # Include cache as sub-module.
 from langfun.core.llms import cache
```

### Comparing `langfun-0.0.2.dev20240418/langfun/core/llms/cache/__init__.py` & `langfun-0.0.2.dev20240419/langfun/core/llms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/llms/cache/base.py` & `langfun-0.0.2.dev20240419/langfun/core/llms/cache/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/llms/cache/in_memory.py` & `langfun-0.0.2.dev20240419/langfun/core/llms/cache/in_memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/llms/cache/in_memory_test.py` & `langfun-0.0.2.dev20240419/langfun/core/llms/cache/in_memory_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/llms/fake.py` & `langfun-0.0.2.dev20240419/langfun/core/llms/fake.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/llms/fake_test.py` & `langfun-0.0.2.dev20240419/langfun/core/llms/fake_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 
   def test_call(self):
     string_io = io.StringIO()
     lm = fakelm.Echo(debug=True)
     with contextlib.redirect_stdout(string_io):
       self.assertEqual(lm('hi'), 'hi')
     debug_info = string_io.getvalue()
-    self.assertIn('[0] LM INFO:', debug_info)
-    self.assertIn('[0] PROMPT SENT TO LM:', debug_info)
+    self.assertIn('[0] LM INFO', debug_info)
+    self.assertIn('[0] PROMPT SENT TO LM', debug_info)
     self.assertIn('[0] LM RESPONSE', debug_info)
 
   def test_score(self):
     lm = fakelm.Echo()
     self.assertEqual(
         lm.score('hi', ['hello', 'how are you']),
         [lf.LMScoringResult(0.0), lf.LMScoringResult(-1.0)],
@@ -80,16 +80,16 @@
     canned_response = "I'm sorry, I can't help you with that."
     lm = fakelm.StaticResponse(canned_response, debug=True)
 
     with contextlib.redirect_stdout(string_io):
       self.assertEqual(lm('hi'), canned_response)
 
     debug_info = string_io.getvalue()
-    self.assertIn('[0] LM INFO:', debug_info)
-    self.assertIn('[0] PROMPT SENT TO LM:', debug_info)
+    self.assertIn('[0] LM INFO', debug_info)
+    self.assertIn('[0] PROMPT SENT TO LM', debug_info)
     self.assertIn('[0] LM RESPONSE', debug_info)
 
 
 class StaticMappingTest(unittest.TestCase):
 
   def test_sample(self):
     lm = fakelm.StaticMapping({
```

### Comparing `langfun-0.0.2.dev20240418/langfun/core/llms/google_genai.py` & `langfun-0.0.2.dev20240419/langfun/core/llms/google_genai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/llms/google_genai_test.py` & `langfun-0.0.2.dev20240419/langfun/core/llms/google_genai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/llms/llama_cpp.py` & `langfun-0.0.2.dev20240419/langfun/core/llms/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/llms/llama_cpp_test.py` & `langfun-0.0.2.dev20240419/langfun/core/llms/llama_cpp_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/llms/openai.py` & `langfun-0.0.2.dev20240419/langfun/core/llms/openai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/llms/openai_test.py` & `langfun-0.0.2.dev20240419/langfun/core/llms/openai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/memories/__init__.py` & `langfun-0.0.2.dev20240419/langfun/core/memories/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/memories/conversation_history.py` & `langfun-0.0.2.dev20240419/langfun/core/memories/conversation_history.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/memories/conversation_history_test.py` & `langfun-0.0.2.dev20240419/langfun/core/memories/conversation_history_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/memory.py` & `langfun-0.0.2.dev20240419/langfun/core/memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/message.py` & `langfun-0.0.2.dev20240419/langfun/core/message.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/message_test.py` & `langfun-0.0.2.dev20240419/langfun/core/message_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/modalities/__init__.py` & `langfun-0.0.2.dev20240419/langfun/core/modalities/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/modalities/image.py` & `langfun-0.0.2.dev20240419/langfun/core/modalities/image.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/modalities/image_test.py` & `langfun-0.0.2.dev20240419/langfun/core/modalities/image_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/modalities/mime.py` & `langfun-0.0.2.dev20240419/langfun/core/modalities/mime.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/modalities/mime_test.py` & `langfun-0.0.2.dev20240419/langfun/core/modalities/mime_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/modalities/video.py` & `langfun-0.0.2.dev20240419/langfun/core/modalities/video.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/modalities/video_test.py` & `langfun-0.0.2.dev20240419/langfun/core/modalities/video_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/modality.py` & `langfun-0.0.2.dev20240419/langfun/core/modality.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/modality_test.py` & `langfun-0.0.2.dev20240419/langfun/core/modality_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/natural_language.py` & `langfun-0.0.2.dev20240419/langfun/core/natural_language.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/natural_language_test.py` & `langfun-0.0.2.dev20240419/langfun/core/natural_language_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/sampling.py` & `langfun-0.0.2.dev20240419/langfun/core/sampling.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/sampling_test.py` & `langfun-0.0.2.dev20240419/langfun/core/sampling_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/structured/__init__.py` & `langfun-0.0.2.dev20240419/langfun/core/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/structured/completion.py` & `langfun-0.0.2.dev20240419/langfun/core/structured/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/structured/completion_test.py` & `langfun-0.0.2.dev20240419/langfun/core/structured/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/structured/description.py` & `langfun-0.0.2.dev20240419/langfun/core/structured/description.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/structured/description_test.py` & `langfun-0.0.2.dev20240419/langfun/core/structured/description_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/structured/function_generation.py` & `langfun-0.0.2.dev20240419/langfun/core/structured/function_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/structured/function_generation_test.py` & `langfun-0.0.2.dev20240419/langfun/core/structured/function_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/structured/mapping.py` & `langfun-0.0.2.dev20240419/langfun/core/structured/mapping.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/structured/mapping_test.py` & `langfun-0.0.2.dev20240419/langfun/core/structured/mapping_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/structured/parsing.py` & `langfun-0.0.2.dev20240419/langfun/core/structured/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/structured/parsing_test.py` & `langfun-0.0.2.dev20240419/langfun/core/structured/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/structured/prompting.py` & `langfun-0.0.2.dev20240419/langfun/core/structured/prompting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/structured/prompting_test.py` & `langfun-0.0.2.dev20240419/langfun/core/structured/prompting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/structured/schema.py` & `langfun-0.0.2.dev20240419/langfun/core/structured/schema.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/structured/schema_generation.py` & `langfun-0.0.2.dev20240419/langfun/core/structured/schema_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/structured/schema_generation_test.py` & `langfun-0.0.2.dev20240419/langfun/core/structured/schema_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/structured/schema_test.py` & `langfun-0.0.2.dev20240419/langfun/core/structured/schema_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/structured/scoring.py` & `langfun-0.0.2.dev20240419/langfun/core/structured/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/structured/scoring_test.py` & `langfun-0.0.2.dev20240419/langfun/core/structured/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/subscription.py` & `langfun-0.0.2.dev20240419/langfun/core/subscription.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/subscription_test.py` & `langfun-0.0.2.dev20240419/langfun/core/subscription_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/template.py` & `langfun-0.0.2.dev20240419/langfun/core/template.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/template_test.py` & `langfun-0.0.2.dev20240419/langfun/core/template_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/templates/__init__.py` & `langfun-0.0.2.dev20240419/langfun/core/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/templates/completion.py` & `langfun-0.0.2.dev20240419/langfun/core/templates/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/templates/completion_test.py` & `langfun-0.0.2.dev20240419/langfun/core/templates/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/templates/conversation.py` & `langfun-0.0.2.dev20240419/langfun/core/templates/conversation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/templates/conversation_test.py` & `langfun-0.0.2.dev20240419/langfun/core/templates/conversation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/templates/demonstration.py` & `langfun-0.0.2.dev20240419/langfun/core/templates/demonstration.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/templates/demonstration_test.py` & `langfun-0.0.2.dev20240419/langfun/core/templates/demonstration_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/templates/selfplay.py` & `langfun-0.0.2.dev20240419/langfun/core/templates/selfplay.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/templates/selfplay_test.py` & `langfun-0.0.2.dev20240419/langfun/core/templates/selfplay_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/text_formatting.py` & `langfun-0.0.2.dev20240419/langfun/core/text_formatting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun/core/text_formatting_test.py` & `langfun-0.0.2.dev20240419/langfun/core/text_formatting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240418/langfun.egg-info/PKG-INFO` & `langfun-0.0.2.dev20240419/langfun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240418
+Version: 0.0.2.dev20240419
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240418/langfun.egg-info/SOURCES.txt` & `langfun-0.0.2.dev20240419/langfun.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,16 @@
 langfun/core/eval/base.py
 langfun/core/eval/base_test.py
 langfun/core/eval/matching.py
 langfun/core/eval/matching_test.py
 langfun/core/eval/scoring.py
 langfun/core/eval/scoring_test.py
 langfun/core/llms/__init__.py
+langfun/core/llms/anthropic.py
+langfun/core/llms/anthropic_test.py
 langfun/core/llms/fake.py
 langfun/core/llms/fake_test.py
 langfun/core/llms/google_genai.py
 langfun/core/llms/google_genai_test.py
 langfun/core/llms/llama_cpp.py
 langfun/core/llms/llama_cpp_test.py
 langfun/core/llms/openai.py
```

### Comparing `langfun-0.0.2.dev20240418/setup.py` & `langfun-0.0.2.dev20240419/setup.py`

 * *Files identical despite different names*

