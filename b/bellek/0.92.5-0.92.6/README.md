# Comparing `tmp/bellek-0.92.5.tar.gz` & `tmp/bellek-0.92.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bellek-0.92.5.tar", last modified: Sat Apr 20 13:46:03 2024, max compression
+gzip compressed data, was "bellek-0.92.6.tar", last modified: Sat Apr 20 15:39:19 2024, max compression
```

## Comparing `bellek-0.92.5.tar` & `bellek-0.92.6.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:46:03.190118 bellek-0.92.5/
--rw-rw-r--   0 bdsaglam   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 bellek-0.92.5/LICENSE
--rw-rw-r--   0 bdsaglam   (501) staff       (20)      111 2022-09-05 16:31:43.000000 bellek-0.92.5/MANIFEST.in
--rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-20 13:46:03.189611 bellek-0.92.5/PKG-INFO
--rw-r--r--   0 bdsaglam   (501) staff       (20)      184 2023-04-09 15:45:53.000000 bellek-0.92.5/README.md
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:46:03.142507 bellek-0.92.5/bellek/
--rw-r--r--   0 bdsaglam   (501) staff       (20)       23 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    56856 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/_modidx.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:46:03.151866 bellek-0.92.5/bellek/hf/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/hf/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:46:03.153116 bellek-0.92.5/bellek/hf/datasets/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/hf/datasets/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1193 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/hf/datasets/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:46:03.157859 bellek-0.92.5/bellek/hf/transformers/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/hf/transformers/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    12912 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/hf/transformers/experiment.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2369 2024-04-20 08:09:04.000000 bellek-0.92.5/bellek/hf/transformers/llama.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2039 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/hf/transformers/llama2.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      790 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/hf/transformers/llama3.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2934 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/hf/transformers/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:46:03.162058 bellek-0.92.5/bellek/jerx/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/jerx/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1314 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/jerx/dataset.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3386 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/jerx/eval.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:46:03.163398 bellek-0.92.5/bellek/jerx/fewshot/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/jerx/fewshot/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     5821 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/jerx/fewshot/llm.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     4110 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/jerx/prompt.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:46:03.164632 bellek-0.92.5/bellek/jerx/reward/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/jerx/reward/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2550 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/jerx/reward/gpt.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1186 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/jerx/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:46:03.167569 bellek-0.92.5/bellek/lang/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/lang/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1575 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/lang/dataset.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2160 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/lang/qdecomp.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:46:03.168985 bellek-0.92.5/bellek/langchain/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/langchain/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      915 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/langchain/cache.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1271 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/langchain/obs.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:46:03.171113 bellek-0.92.5/bellek/llama_index/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/llama_index/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:46:03.171881 bellek-0.92.5/bellek/llama_index/data_structs/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/llama_index/data_structs/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2483 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/llama_index/data_structs/data_structs.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:46:03.173015 bellek-0.92.5/bellek/llama_index/graph_stores/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/llama_index/graph_stores/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     9059 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/llama_index/graph_stores/kuzu.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:46:03.173776 bellek-0.92.5/bellek/llama_index/indices/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/llama_index/indices/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:46:03.175058 bellek-0.92.5/bellek/llama_index/indices/knowledge_graph/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    13058 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    14785 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/llama_index/indices/knowledge_graph/retrievers.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      855 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/llama_index/llms.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1420 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/llama_index/obs.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      779 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/logging.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:46:03.185781 bellek-0.92.5/bellek/ml/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/ml/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2225 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/ml/clip.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     8515 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/ml/coop.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    28983 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/ml/data.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3293 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/ml/evaluation.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3231 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/ml/experiment.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      711 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/ml/layer.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1718 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/ml/loss.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     9174 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/ml/mcd.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      939 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/ml/vision.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:46:03.187285 bellek-0.92.5/bellek/musique/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/musique/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3081 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/musique/eval.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      539 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/testing.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:46:03.188248 bellek-0.92.5/bellek/text/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/text/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/text/utils.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     4864 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/utils.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      823 2024-04-20 13:45:59.000000 bellek-0.92.5/bellek/wandb.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 13:46:03.151119 bellek-0.92.5/bellek.egg-info/
--rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-20 13:46:02.000000 bellek-0.92.5/bellek.egg-info/PKG-INFO
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1780 2024-04-20 13:46:03.000000 bellek-0.92.5/bellek.egg-info/SOURCES.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2024-04-20 13:46:02.000000 bellek-0.92.5/bellek.egg-info/dependency_links.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)       34 2024-04-20 13:46:02.000000 bellek-0.92.5/bellek.egg-info/entry_points.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2023-01-13 22:27:25.000000 bellek-0.92.5/bellek.egg-info/not-zip-safe
--rw-r--r--   0 bdsaglam   (501) staff       (20)      394 2024-04-20 13:46:02.000000 bellek-0.92.5/bellek.egg-info/requires.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        7 2024-04-20 13:46:02.000000 bellek-0.92.5/bellek.egg-info/top_level.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1307 2024-04-20 13:43:15.000000 bellek-0.92.5/settings.ini
--rw-r--r--   0 bdsaglam   (501) staff       (20)       38 2024-04-20 13:46:03.190290 bellek-0.92.5/setup.cfg
--rw-rw-r--   0 bdsaglam   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 bellek-0.92.5/setup.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:19.871195 bellek-0.92.6/
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 bellek-0.92.6/LICENSE
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)      111 2022-09-05 16:31:43.000000 bellek-0.92.6/MANIFEST.in
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-20 15:39:19.870640 bellek-0.92.6/PKG-INFO
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      184 2023-04-09 15:45:53.000000 bellek-0.92.6/README.md
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:19.825289 bellek-0.92.6/bellek/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       23 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    56856 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/_modidx.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:19.830601 bellek-0.92.6/bellek/hf/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/hf/__init__.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:19.831440 bellek-0.92.6/bellek/hf/datasets/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/hf/datasets/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1193 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/hf/datasets/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:19.835303 bellek-0.92.6/bellek/hf/transformers/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/hf/transformers/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    12901 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/hf/transformers/experiment.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2369 2024-04-20 08:09:04.000000 bellek-0.92.6/bellek/hf/transformers/llama.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2039 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/hf/transformers/llama2.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      790 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/hf/transformers/llama3.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2934 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/hf/transformers/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:19.838588 bellek-0.92.6/bellek/jerx/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/jerx/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1314 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/jerx/dataset.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3386 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/jerx/eval.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:19.839380 bellek-0.92.6/bellek/jerx/fewshot/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/jerx/fewshot/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     5821 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/jerx/fewshot/llm.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     4110 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/jerx/prompt.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:19.840366 bellek-0.92.6/bellek/jerx/reward/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/jerx/reward/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2550 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/jerx/reward/gpt.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1186 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/jerx/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:19.842153 bellek-0.92.6/bellek/lang/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/lang/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1575 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/lang/dataset.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2160 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/lang/qdecomp.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:19.844873 bellek-0.92.6/bellek/langchain/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/langchain/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      915 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/langchain/cache.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1271 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/langchain/obs.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:19.847772 bellek-0.92.6/bellek/llama_index/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/llama_index/__init__.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:19.848666 bellek-0.92.6/bellek/llama_index/data_structs/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/llama_index/data_structs/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2483 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/llama_index/data_structs/data_structs.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:19.849911 bellek-0.92.6/bellek/llama_index/graph_stores/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/llama_index/graph_stores/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     9059 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/llama_index/graph_stores/kuzu.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:19.850698 bellek-0.92.6/bellek/llama_index/indices/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/llama_index/indices/__init__.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:19.855176 bellek-0.92.6/bellek/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    13058 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    14785 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/llama_index/indices/knowledge_graph/retrievers.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      855 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/llama_index/llms.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1420 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/llama_index/obs.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      779 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/logging.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:19.865952 bellek-0.92.6/bellek/ml/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/ml/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2225 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/ml/clip.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     8515 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/ml/coop.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    28983 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/ml/data.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3293 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/ml/evaluation.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3231 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/ml/experiment.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      711 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/ml/layer.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1718 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/ml/loss.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     9174 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/ml/mcd.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      939 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/ml/vision.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:19.867719 bellek-0.92.6/bellek/musique/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/musique/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3081 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/musique/eval.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      539 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/testing.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:19.869513 bellek-0.92.6/bellek/text/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/text/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/text/utils.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     4864 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/utils.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      823 2024-04-20 15:39:15.000000 bellek-0.92.6/bellek/wandb.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-20 15:39:19.829995 bellek-0.92.6/bellek.egg-info/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-20 15:39:19.000000 bellek-0.92.6/bellek.egg-info/PKG-INFO
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1780 2024-04-20 15:39:19.000000 bellek-0.92.6/bellek.egg-info/SOURCES.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2024-04-20 15:39:19.000000 bellek-0.92.6/bellek.egg-info/dependency_links.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       34 2024-04-20 15:39:19.000000 bellek-0.92.6/bellek.egg-info/entry_points.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2023-01-13 22:27:25.000000 bellek-0.92.6/bellek.egg-info/not-zip-safe
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      394 2024-04-20 15:39:19.000000 bellek-0.92.6/bellek.egg-info/requires.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        7 2024-04-20 15:39:19.000000 bellek-0.92.6/bellek.egg-info/top_level.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1307 2024-04-20 15:38:50.000000 bellek-0.92.6/settings.ini
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       38 2024-04-20 15:39:19.871394 bellek-0.92.6/setup.cfg
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 bellek-0.92.6/setup.py
```

### Comparing `bellek-0.92.5/LICENSE` & `bellek-0.92.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/PKG-INFO` & `bellek-0.92.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bellek
-Version: 0.92.5
+Version: 0.92.6
 Summary: My digital memory
 Home-page: https://github.com/bdsaglam/bellek
 Author: Barış Deniz Sağlam
 Author-email: bdsaglam@gmail.com
 License: Apache Software License 2.0
 Keywords: notebook
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bellek-0.92.5/bellek/_modidx.py` & `bellek-0.92.6/bellek/_modidx.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/hf/datasets/utils.py` & `bellek-0.92.6/bellek/hf/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/hf/transformers/experiment.py` & `bellek-0.92.6/bellek/hf/transformers/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
         tokenizer=tokenizer,
         **config.at("evaluation.pipeline", {}),
     )
 
 
 def flat_pipeline(pipe):
     def func(inputs, **kwargs) -> list[str]:
-        return [result[0]["generated_text"] for result in tqdm.tqdm(pipe(inputs, **kwargs))]
+        return [result[0]["generated_text"] for result in pipe(inputs, **kwargs)]
 
     return func
 
 
 def predict(
     pipe,
     dataset,
```

### Comparing `bellek-0.92.5/bellek/hf/transformers/llama.py` & `bellek-0.92.6/bellek/hf/transformers/llama.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/hf/transformers/llama2.py` & `bellek-0.92.6/bellek/hf/transformers/llama2.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/hf/transformers/llama3.py` & `bellek-0.92.6/bellek/hf/transformers/llama3.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/hf/transformers/utils.py` & `bellek-0.92.6/bellek/hf/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/jerx/dataset.py` & `bellek-0.92.6/bellek/jerx/dataset.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/jerx/eval.py` & `bellek-0.92.6/bellek/jerx/eval.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/jerx/fewshot/llm.py` & `bellek-0.92.6/bellek/jerx/fewshot/llm.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/jerx/prompt.py` & `bellek-0.92.6/bellek/jerx/prompt.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/jerx/reward/gpt.py` & `bellek-0.92.6/bellek/jerx/reward/gpt.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/jerx/utils.py` & `bellek-0.92.6/bellek/jerx/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/lang/dataset.py` & `bellek-0.92.6/bellek/lang/dataset.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/lang/qdecomp.py` & `bellek-0.92.6/bellek/lang/qdecomp.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/langchain/cache.py` & `bellek-0.92.6/bellek/langchain/cache.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/langchain/obs.py` & `bellek-0.92.6/bellek/langchain/obs.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/llama_index/data_structs/data_structs.py` & `bellek-0.92.6/bellek/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/llama_index/graph_stores/kuzu.py` & `bellek-0.92.6/bellek/llama_index/graph_stores/kuzu.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/llama_index/indices/knowledge_graph/base.py` & `bellek-0.92.6/bellek/llama_index/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/llama_index/indices/knowledge_graph/retrievers.py` & `bellek-0.92.6/bellek/llama_index/indices/knowledge_graph/retrievers.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/llama_index/llms.py` & `bellek-0.92.6/bellek/llama_index/llms.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/llama_index/obs.py` & `bellek-0.92.6/bellek/llama_index/obs.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/logging.py` & `bellek-0.92.6/bellek/logging.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/ml/clip.py` & `bellek-0.92.6/bellek/ml/clip.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/ml/coop.py` & `bellek-0.92.6/bellek/ml/coop.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/ml/data.py` & `bellek-0.92.6/bellek/ml/data.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/ml/evaluation.py` & `bellek-0.92.6/bellek/ml/evaluation.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/ml/experiment.py` & `bellek-0.92.6/bellek/ml/experiment.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/ml/layer.py` & `bellek-0.92.6/bellek/ml/layer.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/ml/loss.py` & `bellek-0.92.6/bellek/ml/loss.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/ml/mcd.py` & `bellek-0.92.6/bellek/ml/mcd.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/ml/vision.py` & `bellek-0.92.6/bellek/ml/vision.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/musique/eval.py` & `bellek-0.92.6/bellek/musique/eval.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/testing.py` & `bellek-0.92.6/bellek/testing.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/utils.py` & `bellek-0.92.6/bellek/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek/wandb.py` & `bellek-0.92.6/bellek/wandb.py`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/bellek.egg-info/PKG-INFO` & `bellek-0.92.6/bellek.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bellek
-Version: 0.92.5
+Version: 0.92.6
 Summary: My digital memory
 Home-page: https://github.com/bdsaglam/bellek
 Author: Barış Deniz Sağlam
 Author-email: bdsaglam@gmail.com
 License: Apache Software License 2.0
 Keywords: notebook
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bellek-0.92.5/bellek.egg-info/SOURCES.txt` & `bellek-0.92.6/bellek.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bellek-0.92.5/settings.ini` & `bellek-0.92.6/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = bellek
 lib_name = bellek
-version = 0.92.5
+version = 0.92.6
 min_python = 3.10
 license = apache2
 doc_path = _docs
 lib_path = bellek
 nbs_path = nbs
 recursive = True
 tst_flags = notest
```

### Comparing `bellek-0.92.5/setup.py` & `bellek-0.92.6/setup.py`

 * *Files identical despite different names*

