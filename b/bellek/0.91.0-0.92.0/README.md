# Comparing `tmp/bellek-0.91.0.tar.gz` & `tmp/bellek-0.92.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bellek-0.91.0.tar", last modified: Sat Apr 20 09:40:46 2024, max compression
+gzip compressed data, was "bellek-0.92.0.tar", last modified: Sat Apr 20 11:00:51 2024, max compression
```

## Comparing `bellek-0.91.0.tar` & `bellek-0.92.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:46.325341 bellek-0.91.0/
--rw-rw-r--   0 bdsaglam   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 bellek-0.91.0/LICENSE
--rw-rw-r--   0 bdsaglam   (501) staff       (20)      111 2022-09-05 16:31:43.000000 bellek-0.91.0/MANIFEST.in
--rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-20 09:40:46.324773 bellek-0.91.0/PKG-INFO
--rw-r--r--   0 bdsaglam   (501) staff       (20)      184 2023-04-09 15:45:53.000000 bellek-0.91.0/README.md
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:46.291352 bellek-0.91.0/bellek/
--rw-r--r--   0 bdsaglam   (501) staff       (20)       23 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    57190 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/_modidx.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:46.295239 bellek-0.91.0/bellek/hf/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/hf/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:46.295885 bellek-0.91.0/bellek/hf/datasets/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/hf/datasets/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1193 2024-04-20 09:40:41.000000 bellek-0.91.0/bellek/hf/datasets/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:46.298677 bellek-0.91.0/bellek/hf/transformers/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/hf/transformers/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    12919 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/hf/transformers/experiment.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2369 2024-04-20 08:09:04.000000 bellek-0.91.0/bellek/hf/transformers/llama.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2039 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/hf/transformers/llama2.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      790 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/hf/transformers/llama3.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2934 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/hf/transformers/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:46.301016 bellek-0.91.0/bellek/jerx/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/jerx/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1314 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/jerx/dataset.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3386 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/jerx/eval.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:46.301874 bellek-0.91.0/bellek/jerx/fewshot/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/jerx/fewshot/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     5821 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/jerx/fewshot/llm.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     4110 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/jerx/prompt.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:46.303092 bellek-0.91.0/bellek/jerx/reward/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/jerx/reward/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2550 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/jerx/reward/gpt.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1186 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/jerx/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:46.304719 bellek-0.91.0/bellek/lang/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/lang/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1575 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/lang/dataset.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2160 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/lang/qdecomp.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:46.307054 bellek-0.91.0/bellek/langchain/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/langchain/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      915 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/langchain/cache.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1271 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/langchain/obs.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:46.308564 bellek-0.91.0/bellek/llama_index/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/llama_index/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:46.309432 bellek-0.91.0/bellek/llama_index/data_structs/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/llama_index/data_structs/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2483 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/llama_index/data_structs/data_structs.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:46.310666 bellek-0.91.0/bellek/llama_index/graph_stores/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/llama_index/graph_stores/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     9059 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/llama_index/graph_stores/kuzu.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:46.311343 bellek-0.91.0/bellek/llama_index/indices/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/llama_index/indices/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:46.312490 bellek-0.91.0/bellek/llama_index/indices/knowledge_graph/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    13058 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    14785 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/llama_index/indices/knowledge_graph/retrievers.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      855 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/llama_index/llms.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1420 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/llama_index/obs.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      779 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/logging.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:46.318833 bellek-0.91.0/bellek/ml/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/ml/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2225 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/ml/clip.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     8515 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/ml/coop.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    28983 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/ml/data.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3293 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/ml/evaluation.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3231 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/ml/experiment.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      711 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/ml/layer.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1718 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/ml/loss.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     9174 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/ml/mcd.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      939 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/ml/vision.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:46.321061 bellek-0.91.0/bellek/musique/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/musique/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3081 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/musique/eval.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      539 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/testing.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:46.323363 bellek-0.91.0/bellek/text/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/text/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/text/utils.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     4864 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/utils.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      823 2024-04-20 09:40:42.000000 bellek-0.91.0/bellek/wandb.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 09:40:46.294745 bellek-0.91.0/bellek.egg-info/
--rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-20 09:40:46.000000 bellek-0.91.0/bellek.egg-info/PKG-INFO
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1780 2024-04-20 09:40:46.000000 bellek-0.91.0/bellek.egg-info/SOURCES.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2024-04-20 09:40:46.000000 bellek-0.91.0/bellek.egg-info/dependency_links.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)       34 2024-04-20 09:40:46.000000 bellek-0.91.0/bellek.egg-info/entry_points.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2023-01-13 22:27:25.000000 bellek-0.91.0/bellek.egg-info/not-zip-safe
--rw-r--r--   0 bdsaglam   (501) staff       (20)      394 2024-04-20 09:40:46.000000 bellek-0.91.0/bellek.egg-info/requires.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        7 2024-04-20 09:40:46.000000 bellek-0.91.0/bellek.egg-info/top_level.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1356 2024-04-20 09:32:12.000000 bellek-0.91.0/settings.ini
--rw-r--r--   0 bdsaglam   (501) staff       (20)       38 2024-04-20 09:40:46.325467 bellek-0.91.0/setup.cfg
--rw-rw-r--   0 bdsaglam   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 bellek-0.91.0/setup.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:51.850071 bellek-0.92.0/
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 bellek-0.92.0/LICENSE
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)      111 2022-09-05 16:31:43.000000 bellek-0.92.0/MANIFEST.in
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-20 11:00:51.849683 bellek-0.92.0/PKG-INFO
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      184 2023-04-09 15:45:53.000000 bellek-0.92.0/README.md
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:51.817461 bellek-0.92.0/bellek/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       23 2024-04-20 11:00:37.000000 bellek-0.92.0/bellek/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    56856 2024-04-20 11:00:37.000000 bellek-0.92.0/bellek/_modidx.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:51.823046 bellek-0.92.0/bellek/hf/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:37.000000 bellek-0.92.0/bellek/hf/__init__.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:51.824450 bellek-0.92.0/bellek/hf/datasets/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:37.000000 bellek-0.92.0/bellek/hf/datasets/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1193 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/hf/datasets/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:51.828134 bellek-0.92.0/bellek/hf/transformers/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:37.000000 bellek-0.92.0/bellek/hf/transformers/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    12922 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/hf/transformers/experiment.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2369 2024-04-20 08:09:04.000000 bellek-0.92.0/bellek/hf/transformers/llama.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2039 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/hf/transformers/llama2.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      790 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/hf/transformers/llama3.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2934 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/hf/transformers/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:51.830917 bellek-0.92.0/bellek/jerx/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:37.000000 bellek-0.92.0/bellek/jerx/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1314 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/jerx/dataset.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3386 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/jerx/eval.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:51.831868 bellek-0.92.0/bellek/jerx/fewshot/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:37.000000 bellek-0.92.0/bellek/jerx/fewshot/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     5821 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/jerx/fewshot/llm.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     4110 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/jerx/prompt.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:51.832654 bellek-0.92.0/bellek/jerx/reward/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:37.000000 bellek-0.92.0/bellek/jerx/reward/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2550 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/jerx/reward/gpt.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1186 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/jerx/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:51.834366 bellek-0.92.0/bellek/lang/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:37.000000 bellek-0.92.0/bellek/lang/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1575 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/lang/dataset.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2160 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/lang/qdecomp.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:51.835761 bellek-0.92.0/bellek/langchain/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/langchain/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      915 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/langchain/cache.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1271 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/langchain/obs.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:51.837228 bellek-0.92.0/bellek/llama_index/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:37.000000 bellek-0.92.0/bellek/llama_index/__init__.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:51.838209 bellek-0.92.0/bellek/llama_index/data_structs/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:37.000000 bellek-0.92.0/bellek/llama_index/data_structs/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2483 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/llama_index/data_structs/data_structs.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:51.839335 bellek-0.92.0/bellek/llama_index/graph_stores/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/llama_index/graph_stores/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     9059 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/llama_index/graph_stores/kuzu.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:51.839970 bellek-0.92.0/bellek/llama_index/indices/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/llama_index/indices/__init__.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:51.841127 bellek-0.92.0/bellek/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    13058 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    14785 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/llama_index/indices/knowledge_graph/retrievers.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      855 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/llama_index/llms.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1420 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/llama_index/obs.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      779 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/logging.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:51.846724 bellek-0.92.0/bellek/ml/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:37.000000 bellek-0.92.0/bellek/ml/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2225 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/ml/clip.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     8515 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/ml/coop.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    28983 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/ml/data.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3293 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/ml/evaluation.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3231 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/ml/experiment.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      711 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/ml/layer.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1718 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/ml/loss.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     9174 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/ml/mcd.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      939 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/ml/vision.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:51.847600 bellek-0.92.0/bellek/musique/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:37.000000 bellek-0.92.0/bellek/musique/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3081 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/musique/eval.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      539 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/testing.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:51.848698 bellek-0.92.0/bellek/text/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:37.000000 bellek-0.92.0/bellek/text/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/text/utils.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     4864 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/utils.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      823 2024-04-20 11:00:36.000000 bellek-0.92.0/bellek/wandb.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 11:00:51.822432 bellek-0.92.0/bellek.egg-info/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-20 11:00:51.000000 bellek-0.92.0/bellek.egg-info/PKG-INFO
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1780 2024-04-20 11:00:51.000000 bellek-0.92.0/bellek.egg-info/SOURCES.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2024-04-20 11:00:51.000000 bellek-0.92.0/bellek.egg-info/dependency_links.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       34 2024-04-20 11:00:51.000000 bellek-0.92.0/bellek.egg-info/entry_points.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2023-01-13 22:27:25.000000 bellek-0.92.0/bellek.egg-info/not-zip-safe
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      394 2024-04-20 11:00:51.000000 bellek-0.92.0/bellek.egg-info/requires.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        7 2024-04-20 11:00:51.000000 bellek-0.92.0/bellek.egg-info/top_level.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1356 2024-04-20 10:58:54.000000 bellek-0.92.0/settings.ini
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       38 2024-04-20 11:00:51.850183 bellek-0.92.0/setup.cfg
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 bellek-0.92.0/setup.py
```

### Comparing `bellek-0.91.0/LICENSE` & `bellek-0.92.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/PKG-INFO` & `bellek-0.92.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bellek
-Version: 0.91.0
+Version: 0.92.0
 Summary: My digital memory
 Home-page: https://github.com/bdsaglam/bellek
 Author: Barış Deniz Sağlam
 Author-email: bdsaglam@gmail.com
 License: Apache Software License 2.0
 Keywords: notebook
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bellek-0.91.0/bellek/_modidx.py` & `bellek-0.92.0/bellek/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,26 +11,24 @@
                                                                                       'bellek/hf/datasets/utils.py')},
             'bellek.hf.transformers.experiment': { 'bellek.hf.transformers.experiment._load_tokenizer_model': ( 'hf.transformers.experiment.html#_load_tokenizer_model',
                                                                                                                 'bellek/hf/transformers/experiment.py'),
                                                    'bellek.hf.transformers.experiment.calculate_token_counts': ( 'hf.transformers.experiment.html#calculate_token_counts',
                                                                                                                  'bellek/hf/transformers/experiment.py'),
                                                    'bellek.hf.transformers.experiment.evaluate_': ( 'hf.transformers.experiment.html#evaluate_',
                                                                                                     'bellek/hf/transformers/experiment.py'),
-                                                   'bellek.hf.transformers.experiment.evaluate_pipeline': ( 'hf.transformers.experiment.html#evaluate_pipeline',
-                                                                                                            'bellek/hf/transformers/experiment.py'),
                                                    'bellek.hf.transformers.experiment.fine_tune': ( 'hf.transformers.experiment.html#fine_tune',
                                                                                                     'bellek/hf/transformers/experiment.py'),
                                                    'bellek.hf.transformers.experiment.flat_pipeline': ( 'hf.transformers.experiment.html#flat_pipeline',
                                                                                                         'bellek/hf/transformers/experiment.py'),
                                                    'bellek.hf.transformers.experiment.make_datacollator': ( 'hf.transformers.experiment.html#make_datacollator',
                                                                                                             'bellek/hf/transformers/experiment.py'),
-                                                   'bellek.hf.transformers.experiment.make_io_dataset': ( 'hf.transformers.experiment.html#make_io_dataset',
-                                                                                                          'bellek/hf/transformers/experiment.py'),
                                                    'bellek.hf.transformers.experiment.make_pipeline': ( 'hf.transformers.experiment.html#make_pipeline',
                                                                                                         'bellek/hf/transformers/experiment.py'),
+                                                   'bellek.hf.transformers.experiment.predict': ( 'hf.transformers.experiment.html#predict',
+                                                                                                  'bellek/hf/transformers/experiment.py'),
                                                    'bellek.hf.transformers.experiment.prepare_config_for_fp': ( 'hf.transformers.experiment.html#prepare_config_for_fp',
                                                                                                                 'bellek/hf/transformers/experiment.py'),
                                                    'bellek.hf.transformers.experiment.prepare_model_for_inference': ( 'hf.transformers.experiment.html#prepare_model_for_inference',
                                                                                                                       'bellek/hf/transformers/experiment.py'),
                                                    'bellek.hf.transformers.experiment.prepare_model_for_training': ( 'hf.transformers.experiment.html#prepare_model_for_training',
                                                                                                                      'bellek/hf/transformers/experiment.py'),
                                                    'bellek.hf.transformers.experiment.preprocess_config': ( 'hf.transformers.experiment.html#preprocess_config',
```

### Comparing `bellek-0.91.0/bellek/hf/datasets/utils.py` & `bellek-0.92.0/bellek/hf/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/hf/transformers/experiment.py` & `bellek-0.92.0/bellek/hf/transformers/experiment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../../nbs/hf.transformers.experiment.ipynb.
 
 # %% auto 0
 __all__ = ['log', 'prepare_config_for_fp', 'preprocess_config', 'make_datacollator', 'prepare_model_for_training',
-           'calculate_token_counts', 'fine_tune', 'prepare_model_for_inference', 'make_io_dataset', 'make_pipeline',
-           'flat_pipeline', 'evaluate_pipeline', 'evaluate_']
+           'calculate_token_counts', 'fine_tune', 'prepare_model_for_inference', 'make_pipeline', 'flat_pipeline',
+           'predict', 'evaluate_']
 
 # %% ../../../nbs/hf.transformers.experiment.ipynb 3
 from copy import deepcopy
 from math import ceil
 from typing import Any, Callable
 
 import torch
@@ -98,25 +98,25 @@
 # %% ../../../nbs/hf.transformers.experiment.ipynb 7
 def prepare_model_for_training(tokenizer, model):
     model_id = model.name_or_path.lower()
 
     if "llama-2" in model_id:
         from bellek.hf.transformers.llama2 import prepare_llama2_for_training
 
-        log.info("Base model is a LLAMA-2 model, preparing it for training.")
+        log.info("Base model is a llama-2 model, preparing it for training.")
         prepare_llama2_for_training(tokenizer, model)
     
     elif "llama-3" in model_id:
         from bellek.hf.transformers.llama3 import prepare_llama3_for_training
 
-        log.info("Base model is a LLAMA-3 model, preparing it for training.")
+        log.info("Base model is a llama-3 model, preparing it for training.")
         prepare_llama3_for_training(tokenizer, model)
     
     else:
-        log.warning(f"Base model '{model_id}' is not a LLAMA-2 or LLAMA-3 model, no special preparation is done.")
+        log.warning(f"Base model '{model_id}' is not a llama-2 or llama-3 model, no special preparation is done.")
 
 # %% ../../../nbs/hf.transformers.experiment.ipynb 8
 def calculate_token_counts(tokenizer, dataset: Dataset, dataset_text_field: str | None):
     if dataset_text_field is None:
         if "messages" not in dataset.column_names:
             raise ValueError("Dataset must have 'messages' columns if `dataset_text_field` is not specified.")
         
@@ -201,141 +201,134 @@
 # %% ../../../nbs/hf.transformers.experiment.ipynb 10
 def prepare_model_for_inference(tokenizer, model):
     model_id = model.name_or_path.lower()
 
     if "llama-2" in model_id:
         from bellek.hf.transformers.llama2 import prepare_llama2_for_inference
 
-        log.info("Base model is a LLAMA-2 model, preparing it for inference.")
+        log.info("Base model is a llama-2 model, preparing it for inference.")
         prepare_llama2_for_inference(tokenizer, model)
     
     elif "llama-3" in model_id:
         from bellek.hf.transformers.llama3 import prepare_llama3_for_inference
 
-        log.info("Base model is a LLAMA-3 model, preparing it for inference.")
+        log.info("Base model is a llama-3 model, preparing it for inference.")
         prepare_llama3_for_inference(tokenizer, model)
     
     else:
-        log.warning(f"Base model '{model_id}' is not a LLAMA-2 or LLAMA-3 model, no special preparation is done.")
+        log.warning(f"Base model '{model_id}' is not a llama-2 or llama-3 model, no special preparation is done.")
 
 # %% ../../../nbs/hf.transformers.experiment.ipynb 11
-def make_io_dataset(dataset: Dataset, response_template: str) -> Dataset:
-    def extract_input_output(example):
-        input, output = example["text"].rsplit(response_template, 1)
-        input += response_template
-        return {"input": input, "output": output}
-
-    return dataset.map(extract_input_output)
-
-
 def _load_tokenizer_model(config: NestedDict):
     model_id = config.at("hfhub.model_id")
     kwargs = deepcopy(config.get("pretrained_model", {}))
     kwargs.pop("model_name_or_path", None)
     return load_tokenizer_model(model_id, **kwargs)
 
+
 def make_pipeline(config, tokenizer, model):
     prepare_model_for_inference(tokenizer, model)
-
-    # Create pipeline
     return pipeline(
         task="text-generation",
         model=model,
         tokenizer=tokenizer,
         **config.at("evaluation.pipeline", {}),
     )
 
 
 def flat_pipeline(pipe):
-    def func(inputs) -> list[str]:
-        results = pipe(inputs)
+    def func(inputs, **kwargs) -> list[str]:
+        results = pipe(inputs, **kwargs)
         return [result[0]["generated_text"] for result in results]
 
     return func
 
 
-def evaluate_pipeline(
-    dataset,
+def predict(
     pipe,
+    dataset,
     *,
-    metric,
-    metric_kwargs: dict | None = None,
     output_parse_fn: Callable[[str], Any] | None = None,
+    **generation_kwargs,
 ):
-    eos_token = pipe.tokenizer.special_tokens_map["eos_token"]
-    def parse_output(text):
-        text = text.replace(eos_token, "").strip()
-        if output_parse_fn:
-            text = output_parse_fn(text)
-        return text
-
     log.info(f"Running pipeline on dataset with {len(dataset)} samples...")
-    generations = flat_pipeline(pipe)(dataset["input"])
 
-    predictions = [parse_output(text) for text in generations]
-    references = [parse_output(text) for text in dataset["output"]]
+    # Setup generation parameters
+    generation_kwargs["return_full_text"] = False
+
+    if "max_new_tokens" not in generation_kwargs:
+        tokenized_outputs = dataset.map(lambda examples: pipe.tokenizer(examples["output"]), batched=True)
+        token_counts = [len(input_ids) for input_ids in tokenized_outputs["input_ids"]]
+        log.info(f"Output token counts: min={min(token_counts)}, max={max(token_counts)}")
+        generation_kwargs["max_new_tokens"] = ceil(max(token_counts) / 8) * 8
+    
+    terminators = generation_kwargs.pop("terminators", [])
+    eos_token_ids = [pipe.tokenizer.eos_token_id]
+    for terminator in terminators:
+        if isinstance(terminator, int):
+            eos_token_ids.append(terminator)
+        elif isinstance(terminator, str):
+            eos_token_ids.append(pipe.tokenizer.convert_tokens_to_ids(terminator))
+        else:
+            raise ValueError(f"Invalid terminator token {terminator}.")
+    generation_kwargs["eos_token_id"] = sorted(set(eos_token_ids))
+
+    # Generate text
+    generations = flat_pipeline(pipe)(dataset["input"], **generation_kwargs)
 
+    # Parse outputs
+    predictions = [output_parse_fn(text) for text in generations]
+    references = [output_parse_fn(text) for text in dataset["output"]]
+
+    # Create dataframe
     dataf = dataset.to_pandas()
     dataf["generation"] = generations
     dataf["prediction"] = predictions
     dataf["reference"] = references
-    
-    metric_kwargs = metric_kwargs or {}
-    scores = metric.compute(predictions=predictions, references=references, **metric_kwargs)
 
-    return scores, dataf
+    return dataf
 
 
 def evaluate_(
     config,
     *,
     tokenizer=None,
     model=None,
     metric_kwargs: dict | None = None,
     output_parse_fn: Callable[[str], Any] | None = None,
 ):
     import evaluate
 
     # Load validation dataset
-    ds_config = config.at("dataset.validation")
-    assert ds_config
-    ds = load_datasets(ds_config)
-    assert len(ds) > 0, "Dataset is empty!"
-    
+    dataset_config = config.at("dataset.validation")
+    assert dataset_config, "Validation dataset is not provided!"
+    dataset = load_datasets(dataset_config)
+    assert len(dataset) > 0, "Validation dataset is empty!"
+
     # Prepare text generation pipeline
     if tokenizer is None or model is None:
         tokenizer, model = _load_tokenizer_model(config)
 
-    # Convert chat to text
-    if "text" not in ds.column_names:
-        if "messages" not in ds.column_names:
-            raise ValueError("Dataset does not have 'text' or 'messages' columns.")
-        ds = ds.map(
-            lambda example: {"text": tokenizer.apply_chat_template(example["messages"], tokenize=False, add_generation_prompt=False)}
-        )
-
     # Ensure the dataset has input/output columns
-    cols = ds[0].keys()
+    cols = dataset[0].keys()
     if "input" not in cols or "output" not in cols:
-        response_template = config.at("trainer.response_template")
-        assert response_template
-        ds = make_io_dataset(ds, response_template)
+        if "messages" not in dataset.column_names:
+            raise ValueError("Dataset must have 'messages' column if 'input' and 'output' columns are not provided.")
+        dataset["input"] = dataset.map(lambda x: x["messages"][:-1])
+        dataset["output"] = dataset.map(lambda x: x["messages"][-1]["content"])
+        dataset = dataset.remove_columns("messages")
 
-    if config.at("evaluation.pipeline.max_new_tokens") is None:
-        tokenized_outputs = ds.map(lambda examples: tokenizer(examples["output"]), batched=True)
-        token_counts = [len(input_ids) for input_ids in tokenized_outputs["input_ids"]]
-        config.set("evaluation.pipeline.max_new_tokens", ceil(max(token_counts) / 8) * 8)
-        
-    log.info(f"Input token counts: min={min(token_counts)}, max={max(token_counts)}")
     pipe = make_pipeline(config, tokenizer, model)
 
-    # Load evaluation metric
-    metric = evaluate.load(config.at("evaluation.metric"))
-
-    return evaluate_pipeline(
-        ds,
+    dataf = predict(
         pipe,
-        metric=metric,
-        metric_kwargs=metric_kwargs,
+        dataset,
         output_parse_fn=output_parse_fn,
+        **config.at("evaluation.generation_params", {}),
     )
 
+    # Compute metrics
+    metric = evaluate.load(config.at("evaluation.metric"))
+    metric_kwargs = metric_kwargs or {}
+    scores = metric.compute(predictions=dataf["prediction"], references=dataf["reference"], **metric_kwargs)
+
+    return scores, dataf
```

### Comparing `bellek-0.91.0/bellek/hf/transformers/llama.py` & `bellek-0.92.0/bellek/hf/transformers/llama.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/hf/transformers/llama2.py` & `bellek-0.92.0/bellek/hf/transformers/llama2.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/hf/transformers/llama3.py` & `bellek-0.92.0/bellek/hf/transformers/llama3.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/hf/transformers/utils.py` & `bellek-0.92.0/bellek/hf/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/jerx/dataset.py` & `bellek-0.92.0/bellek/jerx/dataset.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/jerx/eval.py` & `bellek-0.92.0/bellek/jerx/eval.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/jerx/fewshot/llm.py` & `bellek-0.92.0/bellek/jerx/fewshot/llm.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/jerx/prompt.py` & `bellek-0.92.0/bellek/jerx/prompt.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/jerx/reward/gpt.py` & `bellek-0.92.0/bellek/jerx/reward/gpt.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/jerx/utils.py` & `bellek-0.92.0/bellek/jerx/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/lang/dataset.py` & `bellek-0.92.0/bellek/lang/dataset.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/lang/qdecomp.py` & `bellek-0.92.0/bellek/lang/qdecomp.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/langchain/cache.py` & `bellek-0.92.0/bellek/langchain/cache.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/langchain/obs.py` & `bellek-0.92.0/bellek/langchain/obs.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/llama_index/data_structs/data_structs.py` & `bellek-0.92.0/bellek/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/llama_index/graph_stores/kuzu.py` & `bellek-0.92.0/bellek/llama_index/graph_stores/kuzu.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/llama_index/indices/knowledge_graph/base.py` & `bellek-0.92.0/bellek/llama_index/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/llama_index/indices/knowledge_graph/retrievers.py` & `bellek-0.92.0/bellek/llama_index/indices/knowledge_graph/retrievers.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/llama_index/llms.py` & `bellek-0.92.0/bellek/llama_index/llms.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/llama_index/obs.py` & `bellek-0.92.0/bellek/llama_index/obs.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/logging.py` & `bellek-0.92.0/bellek/logging.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/ml/clip.py` & `bellek-0.92.0/bellek/ml/clip.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/ml/coop.py` & `bellek-0.92.0/bellek/ml/coop.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/ml/data.py` & `bellek-0.92.0/bellek/ml/data.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/ml/evaluation.py` & `bellek-0.92.0/bellek/ml/evaluation.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/ml/experiment.py` & `bellek-0.92.0/bellek/ml/experiment.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/ml/layer.py` & `bellek-0.92.0/bellek/ml/layer.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/ml/loss.py` & `bellek-0.92.0/bellek/ml/loss.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/ml/mcd.py` & `bellek-0.92.0/bellek/ml/mcd.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/ml/vision.py` & `bellek-0.92.0/bellek/ml/vision.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/musique/eval.py` & `bellek-0.92.0/bellek/musique/eval.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/testing.py` & `bellek-0.92.0/bellek/testing.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/utils.py` & `bellek-0.92.0/bellek/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek/wandb.py` & `bellek-0.92.0/bellek/wandb.py`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/bellek.egg-info/PKG-INFO` & `bellek-0.92.0/bellek.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bellek
-Version: 0.91.0
+Version: 0.92.0
 Summary: My digital memory
 Home-page: https://github.com/bdsaglam/bellek
 Author: Barış Deniz Sağlam
 Author-email: bdsaglam@gmail.com
 License: Apache Software License 2.0
 Keywords: notebook
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bellek-0.91.0/bellek.egg-info/SOURCES.txt` & `bellek-0.92.0/bellek.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bellek-0.91.0/settings.ini` & `bellek-0.92.0/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = bellek
 lib_name = bellek
-version = 0.91.0
+version = 0.92.0
 min_python = 3.10
 license = apache2
 doc_path = _docs
 lib_path = bellek
 nbs_path = nbs
 recursive = True
 tst_flags = notest
```

### Comparing `bellek-0.91.0/setup.py` & `bellek-0.92.0/setup.py`

 * *Files identical despite different names*

