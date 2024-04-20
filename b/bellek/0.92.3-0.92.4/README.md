# Comparing `tmp/bellek-0.92.3.tar.gz` & `tmp/bellek-0.92.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bellek-0.92.3.tar", last modified: Sat Apr 20 12:37:28 2024, max compression
+gzip compressed data, was "bellek-0.92.4.tar", last modified: Sat Apr 20 13:03:47 2024, max compression
```

## Comparing `bellek-0.92.3.tar` & `bellek-0.92.4.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:28.517691 bellek-0.92.3/
--rw-rw-r--   0 bdsaglam   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 bellek-0.92.3/LICENSE
--rw-rw-r--   0 bdsaglam   (501) staff       (20)      111 2022-09-05 16:31:43.000000 bellek-0.92.3/MANIFEST.in
--rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-20 12:37:28.514461 bellek-0.92.3/PKG-INFO
--rw-r--r--   0 bdsaglam   (501) staff       (20)      184 2023-04-09 15:45:53.000000 bellek-0.92.3/README.md
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:28.466131 bellek-0.92.3/bellek/
--rw-r--r--   0 bdsaglam   (501) staff       (20)       23 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    56856 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/_modidx.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:28.472677 bellek-0.92.3/bellek/hf/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/hf/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:28.474337 bellek-0.92.3/bellek/hf/datasets/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/hf/datasets/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1193 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/hf/datasets/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:28.480641 bellek-0.92.3/bellek/hf/transformers/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/hf/transformers/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    12887 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/hf/transformers/experiment.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2369 2024-04-20 08:09:04.000000 bellek-0.92.3/bellek/hf/transformers/llama.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2039 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/hf/transformers/llama2.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      790 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/hf/transformers/llama3.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2934 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/hf/transformers/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:28.483913 bellek-0.92.3/bellek/jerx/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/jerx/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1314 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/jerx/dataset.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3386 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/jerx/eval.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:28.485168 bellek-0.92.3/bellek/jerx/fewshot/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/jerx/fewshot/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     5821 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/jerx/fewshot/llm.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     4110 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/jerx/prompt.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:28.486941 bellek-0.92.3/bellek/jerx/reward/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/jerx/reward/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2550 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/jerx/reward/gpt.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1186 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/jerx/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:28.488859 bellek-0.92.3/bellek/lang/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/lang/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1575 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/lang/dataset.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2160 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/lang/qdecomp.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:28.490191 bellek-0.92.3/bellek/langchain/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/langchain/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      915 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/langchain/cache.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1271 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/langchain/obs.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:28.492858 bellek-0.92.3/bellek/llama_index/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/llama_index/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:28.493751 bellek-0.92.3/bellek/llama_index/data_structs/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/llama_index/data_structs/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2483 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/llama_index/data_structs/data_structs.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:28.494670 bellek-0.92.3/bellek/llama_index/graph_stores/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/llama_index/graph_stores/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     9059 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/llama_index/graph_stores/kuzu.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:28.495117 bellek-0.92.3/bellek/llama_index/indices/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/llama_index/indices/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:28.499618 bellek-0.92.3/bellek/llama_index/indices/knowledge_graph/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    13058 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    14785 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/llama_index/indices/knowledge_graph/retrievers.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      855 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/llama_index/llms.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1420 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/llama_index/obs.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      779 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/logging.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:28.508506 bellek-0.92.3/bellek/ml/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/ml/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2225 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/ml/clip.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     8515 2024-04-20 12:37:23.000000 bellek-0.92.3/bellek/ml/coop.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    28983 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/ml/data.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3293 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/ml/evaluation.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3231 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/ml/experiment.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      711 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/ml/layer.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1718 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/ml/loss.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     9174 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/ml/mcd.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      939 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/ml/vision.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:28.510599 bellek-0.92.3/bellek/musique/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/musique/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3081 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/musique/eval.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      539 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/testing.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:28.512684 bellek-0.92.3/bellek/text/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/text/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/text/utils.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     4864 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/utils.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      823 2024-04-20 12:37:24.000000 bellek-0.92.3/bellek/wandb.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 12:37:28.471900 bellek-0.92.3/bellek.egg-info/
--rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-20 12:37:28.000000 bellek-0.92.3/bellek.egg-info/PKG-INFO
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1780 2024-04-20 12:37:28.000000 bellek-0.92.3/bellek.egg-info/SOURCES.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2024-04-20 12:37:28.000000 bellek-0.92.3/bellek.egg-info/dependency_links.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)       34 2024-04-20 12:37:28.000000 bellek-0.92.3/bellek.egg-info/entry_points.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2023-01-13 22:27:25.000000 bellek-0.92.3/bellek.egg-info/not-zip-safe
--rw-r--r--   0 bdsaglam   (501) staff       (20)      394 2024-04-20 12:37:28.000000 bellek-0.92.3/bellek.egg-info/requires.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        7 2024-04-20 12:37:28.000000 bellek-0.92.3/bellek.egg-info/top_level.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1356 2024-04-20 12:37:07.000000 bellek-0.92.3/settings.ini
--rw-r--r--   0 bdsaglam   (501) staff       (20)       38 2024-04-20 12:37:28.518841 bellek-0.92.3/setup.cfg
--rw-rw-r--   0 bdsaglam   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 bellek-0.92.3/setup.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:47.376426 bellek-0.92.4/
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 bellek-0.92.4/LICENSE
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)      111 2022-09-05 16:31:43.000000 bellek-0.92.4/MANIFEST.in
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-20 13:03:47.375861 bellek-0.92.4/PKG-INFO
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      184 2023-04-09 15:45:53.000000 bellek-0.92.4/README.md
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:47.335577 bellek-0.92.4/bellek/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       23 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    56856 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/_modidx.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:47.341132 bellek-0.92.4/bellek/hf/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/hf/__init__.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:47.342177 bellek-0.92.4/bellek/hf/datasets/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/hf/datasets/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1193 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/hf/datasets/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:47.345962 bellek-0.92.4/bellek/hf/transformers/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/hf/transformers/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    12876 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/hf/transformers/experiment.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2369 2024-04-20 08:09:04.000000 bellek-0.92.4/bellek/hf/transformers/llama.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2039 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/hf/transformers/llama2.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      790 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/hf/transformers/llama3.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2934 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/hf/transformers/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:47.349894 bellek-0.92.4/bellek/jerx/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/jerx/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1314 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/jerx/dataset.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3386 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/jerx/eval.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:47.352662 bellek-0.92.4/bellek/jerx/fewshot/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/jerx/fewshot/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     5821 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/jerx/fewshot/llm.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     4110 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/jerx/prompt.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:47.353647 bellek-0.92.4/bellek/jerx/reward/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/jerx/reward/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2550 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/jerx/reward/gpt.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1186 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/jerx/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:47.355336 bellek-0.92.4/bellek/lang/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/lang/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1575 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/lang/dataset.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2160 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/lang/qdecomp.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:47.357108 bellek-0.92.4/bellek/langchain/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/langchain/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      915 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/langchain/cache.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1271 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/langchain/obs.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:47.358826 bellek-0.92.4/bellek/llama_index/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/llama_index/__init__.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:47.360015 bellek-0.92.4/bellek/llama_index/data_structs/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/llama_index/data_structs/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2483 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/llama_index/data_structs/data_structs.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:47.361028 bellek-0.92.4/bellek/llama_index/graph_stores/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/llama_index/graph_stores/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     9059 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/llama_index/graph_stores/kuzu.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:47.361577 bellek-0.92.4/bellek/llama_index/indices/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/llama_index/indices/__init__.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:47.363872 bellek-0.92.4/bellek/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    13058 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    14785 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/llama_index/indices/knowledge_graph/retrievers.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      855 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/llama_index/llms.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1420 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/llama_index/obs.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      779 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/logging.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:47.372378 bellek-0.92.4/bellek/ml/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/ml/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2225 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/ml/clip.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     8515 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/ml/coop.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    28983 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/ml/data.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3293 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/ml/evaluation.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3231 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/ml/experiment.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      711 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/ml/layer.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1718 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/ml/loss.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     9174 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/ml/mcd.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      939 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/ml/vision.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:47.373606 bellek-0.92.4/bellek/musique/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/musique/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3081 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/musique/eval.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      539 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/testing.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:47.374834 bellek-0.92.4/bellek/text/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/text/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/text/utils.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     4864 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/utils.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      823 2024-04-20 13:03:42.000000 bellek-0.92.4/bellek/wandb.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:03:47.340391 bellek-0.92.4/bellek.egg-info/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-20 13:03:47.000000 bellek-0.92.4/bellek.egg-info/PKG-INFO
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1780 2024-04-20 13:03:47.000000 bellek-0.92.4/bellek.egg-info/SOURCES.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2024-04-20 13:03:47.000000 bellek-0.92.4/bellek.egg-info/dependency_links.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       34 2024-04-20 13:03:47.000000 bellek-0.92.4/bellek.egg-info/entry_points.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2023-01-13 22:27:25.000000 bellek-0.92.4/bellek.egg-info/not-zip-safe
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      394 2024-04-20 13:03:47.000000 bellek-0.92.4/bellek.egg-info/requires.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        7 2024-04-20 13:03:47.000000 bellek-0.92.4/bellek.egg-info/top_level.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1307 2024-04-20 13:03:26.000000 bellek-0.92.4/settings.ini
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       38 2024-04-20 13:03:47.376587 bellek-0.92.4/setup.cfg
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 bellek-0.92.4/setup.py
```

### Comparing `bellek-0.92.3/LICENSE` & `bellek-0.92.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/PKG-INFO` & `bellek-0.92.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bellek
-Version: 0.92.3
+Version: 0.92.4
 Summary: My digital memory
 Home-page: https://github.com/bdsaglam/bellek
 Author: Barış Deniz Sağlam
 Author-email: bdsaglam@gmail.com
 License: Apache Software License 2.0
 Keywords: notebook
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bellek-0.92.3/bellek/_modidx.py` & `bellek-0.92.4/bellek/_modidx.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/hf/datasets/utils.py` & `bellek-0.92.4/bellek/hf/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/hf/transformers/experiment.py` & `bellek-0.92.4/bellek/hf/transformers/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,23 +258,23 @@
     if "max_new_tokens" not in generation_kwargs:
         tokenized_outputs = dataset.map(lambda examples: pipe.tokenizer(examples["output"]), batched=True)
         token_counts = [len(input_ids) for input_ids in tokenized_outputs["input_ids"]]
         log.info(f"Output token counts: min={min(token_counts)}, max={max(token_counts)}")
         generation_kwargs["max_new_tokens"] = ceil(max(token_counts) / 8) * 8
 
     terminators = generation_kwargs.pop("terminators", [])
-    eos_token_ids = [pipe.tokenizer.eos_token_id]
+    eos_token_ids = {pipe.tokenizer.eos_token_id}
     for terminator in terminators:
         if isinstance(terminator, int):
-            eos_token_ids.append(terminator)
+            eos_token_ids.add(terminator)
         elif isinstance(terminator, str):
-            eos_token_ids.append(pipe.tokenizer.convert_tokens_to_ids(terminator))
+            eos_token_ids.add(pipe.tokenizer.convert_tokens_to_ids(terminator))
         else:
             raise ValueError(f"Invalid terminator token {terminator}.")
-    generation_kwargs["eos_token_id"] = sorted(set(eos_token_ids))
+    generation_kwargs["eos_token_id"] = sorted(eos_token_ids)
 
     # Generate text
     generations = flat_pipeline(pipe)(dataset["input"], **generation_kwargs)
 
     # Parse outputs
     predictions = [output_parse_fn(text) for text in generations]
     references = [output_parse_fn(text) for text in dataset["output"]]
```

### Comparing `bellek-0.92.3/bellek/hf/transformers/llama.py` & `bellek-0.92.4/bellek/hf/transformers/llama.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/hf/transformers/llama2.py` & `bellek-0.92.4/bellek/hf/transformers/llama2.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/hf/transformers/llama3.py` & `bellek-0.92.4/bellek/hf/transformers/llama3.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/hf/transformers/utils.py` & `bellek-0.92.4/bellek/hf/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/jerx/dataset.py` & `bellek-0.92.4/bellek/jerx/dataset.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/jerx/eval.py` & `bellek-0.92.4/bellek/jerx/eval.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/jerx/fewshot/llm.py` & `bellek-0.92.4/bellek/jerx/fewshot/llm.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/jerx/prompt.py` & `bellek-0.92.4/bellek/jerx/prompt.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/jerx/reward/gpt.py` & `bellek-0.92.4/bellek/jerx/reward/gpt.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/jerx/utils.py` & `bellek-0.92.4/bellek/jerx/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/lang/dataset.py` & `bellek-0.92.4/bellek/lang/dataset.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/lang/qdecomp.py` & `bellek-0.92.4/bellek/lang/qdecomp.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/langchain/cache.py` & `bellek-0.92.4/bellek/langchain/cache.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/langchain/obs.py` & `bellek-0.92.4/bellek/langchain/obs.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/llama_index/data_structs/data_structs.py` & `bellek-0.92.4/bellek/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/llama_index/graph_stores/kuzu.py` & `bellek-0.92.4/bellek/llama_index/graph_stores/kuzu.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/llama_index/indices/knowledge_graph/base.py` & `bellek-0.92.4/bellek/llama_index/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/llama_index/indices/knowledge_graph/retrievers.py` & `bellek-0.92.4/bellek/llama_index/indices/knowledge_graph/retrievers.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/llama_index/llms.py` & `bellek-0.92.4/bellek/llama_index/llms.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/llama_index/obs.py` & `bellek-0.92.4/bellek/llama_index/obs.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/logging.py` & `bellek-0.92.4/bellek/logging.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/ml/clip.py` & `bellek-0.92.4/bellek/ml/clip.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/ml/coop.py` & `bellek-0.92.4/bellek/ml/coop.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/ml/data.py` & `bellek-0.92.4/bellek/ml/data.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/ml/evaluation.py` & `bellek-0.92.4/bellek/ml/evaluation.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/ml/experiment.py` & `bellek-0.92.4/bellek/ml/experiment.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/ml/layer.py` & `bellek-0.92.4/bellek/ml/layer.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/ml/loss.py` & `bellek-0.92.4/bellek/ml/loss.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/ml/mcd.py` & `bellek-0.92.4/bellek/ml/mcd.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/ml/vision.py` & `bellek-0.92.4/bellek/ml/vision.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/musique/eval.py` & `bellek-0.92.4/bellek/musique/eval.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/testing.py` & `bellek-0.92.4/bellek/testing.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/utils.py` & `bellek-0.92.4/bellek/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek/wandb.py` & `bellek-0.92.4/bellek/wandb.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/bellek.egg-info/PKG-INFO` & `bellek-0.92.4/bellek.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bellek
-Version: 0.92.3
+Version: 0.92.4
 Summary: My digital memory
 Home-page: https://github.com/bdsaglam/bellek
 Author: Barış Deniz Sağlam
 Author-email: bdsaglam@gmail.com
 License: Apache Software License 2.0
 Keywords: notebook
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bellek-0.92.3/bellek.egg-info/SOURCES.txt` & `bellek-0.92.4/bellek.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bellek-0.92.3/settings.ini` & `bellek-0.92.4/settings.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = bellek
 lib_name = bellek
-version = 0.92.3
+version = 0.92.4
 min_python = 3.10
 license = apache2
 doc_path = _docs
 lib_path = bellek
 nbs_path = nbs
 recursive = True
 tst_flags = notest
@@ -39,15 +39,15 @@
     litellm~=1.16.12
     sentence_transformers>=2.2.2
     transformers>=4.39.3
     text-generation~=0.6.1
     arize-phoenix>=2.1.0
     python-dotenv 
     wandb 
-    # clip@git+https://github.com/openai/CLIP.git
+
 dev_requirements = 
     nbdev 
     jupyter 
     twine 
     pre-commit 
     isort 
     black
```

### Comparing `bellek-0.92.3/setup.py` & `bellek-0.92.4/setup.py`

 * *Files identical despite different names*

