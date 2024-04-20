# Comparing `tmp/imodelsx-1.0.0.tar.gz` & `tmp/imodelsx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imodelsx-1.0.0.tar", last modified: Mon Apr  1 02:42:26 2024, max compression
+gzip compressed data, was "imodelsx-1.0.1.tar", last modified: Sat Apr 20 00:17:00 2024, max compression
```

## Comparing `imodelsx-1.0.0.tar` & `imodelsx-1.0.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-01 02:42:26.284497 imodelsx-1.0.0/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12670 2024-04-01 02:42:26.284497 imodelsx-1.0.0/PKG-INFO
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-01 02:42:26.280497 imodelsx-1.0.0/imodelsx/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      561 2023-12-13 21:38:50.000000 imodelsx-1.0.0/imodelsx/__init__.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-01 02:42:26.280497 imodelsx-1.0.0/imodelsx/auglinear/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2022-10-04 23:40:44.000000 imodelsx-1.0.0/imodelsx/auglinear/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    17684 2024-02-13 16:34:50.000000 imodelsx-1.0.0/imodelsx/auglinear/auglinear.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7082 2024-02-13 16:36:25.000000 imodelsx-1.0.0/imodelsx/auglinear/embed.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-01 02:42:26.280497 imodelsx-1.0.0/imodelsx/augtree/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-24 23:36:41.000000 imodelsx-1.0.0/imodelsx/augtree/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11437 2023-04-07 17:36:23.000000 imodelsx-1.0.0/imodelsx/augtree/augtree.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1273 2023-11-02 14:39:42.000000 imodelsx-1.0.0/imodelsx/augtree/data.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6465 2023-11-02 14:40:10.000000 imodelsx-1.0.0/imodelsx/augtree/embed.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2234 2023-02-06 22:48:13.000000 imodelsx-1.0.0/imodelsx/augtree/ensemble.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2380 2023-04-07 16:31:41.000000 imodelsx-1.0.0/imodelsx/augtree/llm.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    16783 2023-04-07 05:20:42.000000 imodelsx-1.0.0/imodelsx/augtree/stump.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3260 2023-11-02 14:40:40.000000 imodelsx-1.0.0/imodelsx/augtree/utils.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2120 2024-03-24 12:39:14.000000 imodelsx-1.0.0/imodelsx/cache_save_utils.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-01 02:42:26.280497 imodelsx-1.0.0/imodelsx/d3/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2022-10-04 21:38:29.000000 imodelsx-1.0.0/imodelsx/d3/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4312 2023-04-07 05:02:55.000000 imodelsx-1.0.0/imodelsx/d3/d3.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7246 2022-10-04 22:03:12.000000 imodelsx-1.0.0/imodelsx/d3/step1_get_extreme.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7194 2022-10-04 22:27:59.000000 imodelsx-1.0.0/imodelsx/d3/step2_proposer.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8982 2022-10-04 22:12:36.000000 imodelsx-1.0.0/imodelsx/d3/step3_verifier.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6130 2023-07-28 21:36:15.000000 imodelsx-1.0.0/imodelsx/data.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      282 2023-02-16 23:25:53.000000 imodelsx-1.0.0/imodelsx/dummy_script.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2516 2023-09-13 00:14:38.000000 imodelsx-1.0.0/imodelsx/embeddings.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-01 02:42:26.280497 imodelsx-1.0.0/imodelsx/iprompt/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      195 2022-10-15 16:18:36.000000 imodelsx-1.0.0/imodelsx/iprompt/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    36551 2023-06-07 16:00:03.000000 imodelsx-1.0.0/imodelsx/iprompt/api.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11285 2023-06-07 16:00:03.000000 imodelsx-1.0.0/imodelsx/iprompt/autoprompt.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      624 2023-02-07 19:15:27.000000 imodelsx-1.0.0/imodelsx/iprompt/data.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2371 2022-10-15 16:18:36.000000 imodelsx-1.0.0/imodelsx/iprompt/gumbel.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    14226 2023-05-25 18:26:24.000000 imodelsx-1.0.0/imodelsx/iprompt/hotflip.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    19376 2023-06-07 16:00:03.000000 imodelsx-1.0.0/imodelsx/iprompt/ipromptx.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12909 2023-06-07 16:01:30.000000 imodelsx-1.0.0/imodelsx/iprompt/llm.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1751 2022-10-15 16:18:36.000000 imodelsx-1.0.0/imodelsx/iprompt/prompt_tune.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    24166 2023-02-14 20:42:53.000000 imodelsx-1.0.0/imodelsx/iprompt/utils.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6957 2023-11-02 14:36:50.000000 imodelsx-1.0.0/imodelsx/linear_finetune.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5618 2023-11-02 14:37:02.000000 imodelsx-1.0.0/imodelsx/linear_ngram.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    18931 2024-03-28 14:31:54.000000 imodelsx-1.0.0/imodelsx/llm.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1577 2023-04-24 18:43:24.000000 imodelsx-1.0.0/imodelsx/metrics.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5746 2024-03-13 01:22:46.000000 imodelsx-1.0.0/imodelsx/process_results.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-01 02:42:26.280497 imodelsx-1.0.0/imodelsx/sasc/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-05-15 21:34:39.000000 imodelsx-1.0.0/imodelsx/sasc/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5670 2023-06-27 00:56:11.000000 imodelsx-1.0.0/imodelsx/sasc/api.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4951 2023-05-15 20:33:55.000000 imodelsx-1.0.0/imodelsx/sasc/m1_ngrams.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4957 2023-06-27 00:10:16.000000 imodelsx-1.0.0/imodelsx/sasc/m2_summarize.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3543 2023-06-27 00:10:23.000000 imodelsx-1.0.0/imodelsx/sasc/m3_generate.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13757 2024-04-01 02:18:08.000000 imodelsx-1.0.0/imodelsx/submit_utils.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-01 02:42:26.280497 imodelsx-1.0.0/imodelsx/treeprompt/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-08-30 17:20:13.000000 imodelsx-1.0.0/imodelsx/treeprompt/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13430 2023-10-10 15:55:49.000000 imodelsx-1.0.0/imodelsx/treeprompt/stump.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6709 2023-10-10 16:25:57.000000 imodelsx-1.0.0/imodelsx/treeprompt/treeprompt.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6342 2023-12-14 18:21:43.000000 imodelsx-1.0.0/imodelsx/util.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8794 2024-01-19 23:29:14.000000 imodelsx-1.0.0/imodelsx/viz.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-01 02:42:26.280497 imodelsx-1.0.0/imodelsx.egg-info/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12670 2024-04-01 02:42:26.000000 imodelsx-1.0.0/imodelsx.egg-info/PKG-INFO
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1562 2024-04-01 02:42:26.000000 imodelsx-1.0.0/imodelsx.egg-info/SOURCES.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        1 2024-04-01 02:42:26.000000 imodelsx-1.0.0/imodelsx.egg-info/dependency_links.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      114 2024-04-01 02:42:26.000000 imodelsx-1.0.0/imodelsx.egg-info/requires.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        9 2024-04-01 02:42:26.000000 imodelsx-1.0.0/imodelsx.egg-info/top_level.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       38 2024-04-01 02:42:26.284497 imodelsx-1.0.0/setup.cfg
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1323 2024-04-01 02:42:15.000000 imodelsx-1.0.0/setup.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-01 02:42:26.284497 imodelsx-1.0.0/tests/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      146 2023-12-13 21:39:12.000000 imodelsx-1.0.0/tests/test_auglinear.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1685 2023-12-13 21:40:29.000000 imodelsx-1.0.0/tests/test_auglinear_pipeline.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5451 2023-04-07 16:34:10.000000 imodelsx-1.0.0/tests/test_augtree.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1099 2023-02-07 19:05:22.000000 imodelsx-1.0.0/tests/test_iprompt.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      917 2024-03-23 14:38:38.000000 imodelsx-1.0.0/tests/test_llm.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1451 2023-04-07 03:36:08.000000 imodelsx-1.0.0/tests/test_ngram_list.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      786 2023-05-15 21:35:21.000000 imodelsx-1.0.0/tests/test_sasc.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-20 00:17:00.121135 imodelsx-1.0.1/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12670 2024-04-20 00:17:00.121135 imodelsx-1.0.1/PKG-INFO
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-20 00:17:00.117134 imodelsx-1.0.1/imodelsx/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      561 2023-12-13 21:38:50.000000 imodelsx-1.0.1/imodelsx/__init__.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-20 00:17:00.117134 imodelsx-1.0.1/imodelsx/auglinear/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2022-10-04 23:40:44.000000 imodelsx-1.0.1/imodelsx/auglinear/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    17684 2024-02-13 16:34:50.000000 imodelsx-1.0.1/imodelsx/auglinear/auglinear.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7082 2024-02-13 16:36:25.000000 imodelsx-1.0.1/imodelsx/auglinear/embed.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-20 00:17:00.117134 imodelsx-1.0.1/imodelsx/augtree/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-24 23:36:41.000000 imodelsx-1.0.1/imodelsx/augtree/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11437 2023-04-07 17:36:23.000000 imodelsx-1.0.1/imodelsx/augtree/augtree.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1273 2023-11-02 14:39:42.000000 imodelsx-1.0.1/imodelsx/augtree/data.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6465 2023-11-02 14:40:10.000000 imodelsx-1.0.1/imodelsx/augtree/embed.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2234 2023-02-06 22:48:13.000000 imodelsx-1.0.1/imodelsx/augtree/ensemble.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2380 2023-04-07 16:31:41.000000 imodelsx-1.0.1/imodelsx/augtree/llm.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    16783 2023-04-07 05:20:42.000000 imodelsx-1.0.1/imodelsx/augtree/stump.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3260 2023-11-02 14:40:40.000000 imodelsx-1.0.1/imodelsx/augtree/utils.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2120 2024-03-24 12:39:14.000000 imodelsx-1.0.1/imodelsx/cache_save_utils.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-20 00:17:00.117134 imodelsx-1.0.1/imodelsx/d3/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2022-10-04 21:38:29.000000 imodelsx-1.0.1/imodelsx/d3/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4312 2023-04-07 05:02:55.000000 imodelsx-1.0.1/imodelsx/d3/d3.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7246 2022-10-04 22:03:12.000000 imodelsx-1.0.1/imodelsx/d3/step1_get_extreme.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7194 2022-10-04 22:27:59.000000 imodelsx-1.0.1/imodelsx/d3/step2_proposer.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8982 2022-10-04 22:12:36.000000 imodelsx-1.0.1/imodelsx/d3/step3_verifier.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6130 2023-07-28 21:36:15.000000 imodelsx-1.0.1/imodelsx/data.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      282 2023-02-16 23:25:53.000000 imodelsx-1.0.1/imodelsx/dummy_script.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2516 2023-09-13 00:14:38.000000 imodelsx-1.0.1/imodelsx/embeddings.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-20 00:17:00.121135 imodelsx-1.0.1/imodelsx/iprompt/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      195 2022-10-15 16:18:36.000000 imodelsx-1.0.1/imodelsx/iprompt/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    36551 2023-06-07 16:00:03.000000 imodelsx-1.0.1/imodelsx/iprompt/api.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11285 2023-06-07 16:00:03.000000 imodelsx-1.0.1/imodelsx/iprompt/autoprompt.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      624 2023-02-07 19:15:27.000000 imodelsx-1.0.1/imodelsx/iprompt/data.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2371 2022-10-15 16:18:36.000000 imodelsx-1.0.1/imodelsx/iprompt/gumbel.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    14226 2023-05-25 18:26:24.000000 imodelsx-1.0.1/imodelsx/iprompt/hotflip.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    19376 2023-06-07 16:00:03.000000 imodelsx-1.0.1/imodelsx/iprompt/ipromptx.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12909 2023-06-07 16:01:30.000000 imodelsx-1.0.1/imodelsx/iprompt/llm.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1751 2022-10-15 16:18:36.000000 imodelsx-1.0.1/imodelsx/iprompt/prompt_tune.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    24166 2023-02-14 20:42:53.000000 imodelsx-1.0.1/imodelsx/iprompt/utils.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8181 2024-04-12 13:28:41.000000 imodelsx-1.0.1/imodelsx/linear_finetune.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5618 2023-11-02 14:37:02.000000 imodelsx-1.0.1/imodelsx/linear_ngram.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    22658 2024-04-20 00:15:34.000000 imodelsx-1.0.1/imodelsx/llm.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1577 2023-04-24 18:43:24.000000 imodelsx-1.0.1/imodelsx/metrics.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6148 2024-04-19 21:47:37.000000 imodelsx-1.0.1/imodelsx/process_results.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-20 00:17:00.121135 imodelsx-1.0.1/imodelsx/sasc/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-05-15 21:34:39.000000 imodelsx-1.0.1/imodelsx/sasc/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5670 2023-06-27 00:56:11.000000 imodelsx-1.0.1/imodelsx/sasc/api.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4951 2023-05-15 20:33:55.000000 imodelsx-1.0.1/imodelsx/sasc/m1_ngrams.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4957 2023-06-27 00:10:16.000000 imodelsx-1.0.1/imodelsx/sasc/m2_summarize.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3543 2023-06-27 00:10:23.000000 imodelsx-1.0.1/imodelsx/sasc/m3_generate.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    14826 2024-04-03 15:01:50.000000 imodelsx-1.0.1/imodelsx/submit_utils.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-20 00:17:00.121135 imodelsx-1.0.1/imodelsx/treeprompt/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-08-30 17:20:13.000000 imodelsx-1.0.1/imodelsx/treeprompt/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13430 2023-10-10 15:55:49.000000 imodelsx-1.0.1/imodelsx/treeprompt/stump.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6709 2024-04-15 14:14:26.000000 imodelsx-1.0.1/imodelsx/treeprompt/treeprompt.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6342 2023-12-14 18:21:43.000000 imodelsx-1.0.1/imodelsx/util.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8794 2024-01-19 23:29:14.000000 imodelsx-1.0.1/imodelsx/viz.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-20 00:17:00.117134 imodelsx-1.0.1/imodelsx.egg-info/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12670 2024-04-20 00:17:00.000000 imodelsx-1.0.1/imodelsx.egg-info/PKG-INFO
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1562 2024-04-20 00:17:00.000000 imodelsx-1.0.1/imodelsx.egg-info/SOURCES.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        1 2024-04-20 00:17:00.000000 imodelsx-1.0.1/imodelsx.egg-info/dependency_links.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      114 2024-04-20 00:17:00.000000 imodelsx-1.0.1/imodelsx.egg-info/requires.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        9 2024-04-20 00:17:00.000000 imodelsx-1.0.1/imodelsx.egg-info/top_level.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       38 2024-04-20 00:17:00.121135 imodelsx-1.0.1/setup.cfg
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1323 2024-04-20 00:16:12.000000 imodelsx-1.0.1/setup.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-20 00:17:00.121135 imodelsx-1.0.1/tests/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      146 2023-12-13 21:39:12.000000 imodelsx-1.0.1/tests/test_auglinear.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1685 2023-12-13 21:40:29.000000 imodelsx-1.0.1/tests/test_auglinear_pipeline.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5451 2023-04-07 16:34:10.000000 imodelsx-1.0.1/tests/test_augtree.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1099 2023-02-07 19:05:22.000000 imodelsx-1.0.1/tests/test_iprompt.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      917 2024-03-23 14:38:38.000000 imodelsx-1.0.1/tests/test_llm.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1451 2023-04-07 03:36:08.000000 imodelsx-1.0.1/tests/test_ngram_list.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      786 2023-05-15 21:35:21.000000 imodelsx-1.0.1/tests/test_sasc.py
```

### Comparing `imodelsx-1.0.0/PKG-INFO` & `imodelsx-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imodelsx
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library to explain a dataset in natural language.
 Home-page: https://github.com/csinva/imodelsX
 Author: Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah Hsu, Yuntian Deng
 Author-email: chansingh@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: imodelsx Version: 1.0.0 Summary: Library to explain
+Metadata-Version: 2.1 Name: imodelsx Version: 1.0.1 Summary: Library to explain
 a dataset in natural language. Home-page: https://github.com/csinva/imodelsX
 Author: Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah
 Hsu, Yuntian Deng Author-email: chansingh@microsoft.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown
   [https://microsoft.github.io/aug-models/embgam_gif.gif][https://csinva.io/
```

### Comparing `imodelsx-1.0.0/imodelsx/__init__.py` & `imodelsx-1.0.1/imodelsx/__init__.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/auglinear/auglinear.py` & `imodelsx-1.0.1/imodelsx/auglinear/auglinear.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/auglinear/embed.py` & `imodelsx-1.0.1/imodelsx/auglinear/embed.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/augtree/augtree.py` & `imodelsx-1.0.1/imodelsx/augtree/augtree.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/augtree/data.py` & `imodelsx-1.0.1/imodelsx/augtree/data.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/augtree/embed.py` & `imodelsx-1.0.1/imodelsx/augtree/embed.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/augtree/ensemble.py` & `imodelsx-1.0.1/imodelsx/augtree/ensemble.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/augtree/llm.py` & `imodelsx-1.0.1/imodelsx/augtree/llm.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/augtree/stump.py` & `imodelsx-1.0.1/imodelsx/augtree/stump.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/augtree/utils.py` & `imodelsx-1.0.1/imodelsx/augtree/utils.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/cache_save_utils.py` & `imodelsx-1.0.1/imodelsx/cache_save_utils.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/d3/d3.py` & `imodelsx-1.0.1/imodelsx/d3/d3.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/d3/step1_get_extreme.py` & `imodelsx-1.0.1/imodelsx/d3/step1_get_extreme.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/d3/step2_proposer.py` & `imodelsx-1.0.1/imodelsx/d3/step2_proposer.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/d3/step3_verifier.py` & `imodelsx-1.0.1/imodelsx/d3/step3_verifier.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/data.py` & `imodelsx-1.0.1/imodelsx/data.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/embeddings.py` & `imodelsx-1.0.1/imodelsx/embeddings.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/iprompt/api.py` & `imodelsx-1.0.1/imodelsx/iprompt/api.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/iprompt/autoprompt.py` & `imodelsx-1.0.1/imodelsx/iprompt/autoprompt.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/iprompt/data.py` & `imodelsx-1.0.1/imodelsx/iprompt/data.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/iprompt/gumbel.py` & `imodelsx-1.0.1/imodelsx/iprompt/gumbel.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/iprompt/hotflip.py` & `imodelsx-1.0.1/imodelsx/iprompt/hotflip.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/iprompt/ipromptx.py` & `imodelsx-1.0.1/imodelsx/iprompt/ipromptx.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/iprompt/llm.py` & `imodelsx-1.0.1/imodelsx/iprompt/llm.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/iprompt/prompt_tune.py` & `imodelsx-1.0.1/imodelsx/iprompt/prompt_tune.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/iprompt/utils.py` & `imodelsx-1.0.1/imodelsx/iprompt/utils.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/linear_finetune.py` & `imodelsx-1.0.1/imodelsx/linear_finetune.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import transformers
 from tqdm import tqdm
 import os
 import os.path
 import warnings
 import pickle as pkl
 import torch
+import torch.nn
 from sklearn.exceptions import ConvergenceWarning
 
 device = "cuda" if torch.cuda.is_available() else "cpu"
 
 
 class LinearFinetune(BaseEstimator):
     def __init__(
@@ -172,43 +173,78 @@
     def predict_proba(self, X_text):
         check_is_fitted(self)
         embs = self._get_embs(X_text)
         if self.normalize_embs:
             embs = self.normalizer.transform(embs)
         return self.linear.predict_proba(embs)
 
+    def _export_to_pytorch(self):
+        assert self.normalize_embs == False, "not implemented"
+        weights = self.linear.coef_
+        intercept = self.linear.intercept_
+        torch_model = LinearModelPytorch(
+            in_features=weights.shape[1],
+            out_classes=weights.shape[0],
+        )
+        torch_model.linear.weight = torch.nn.Parameter(
+            torch.tensor(weights, dtype=torch.float32))
+        torch_model.linear.bias = torch.nn.Parameter(
+            torch.tensor(intercept, dtype=torch.float32))
+        return torch_model
+
 
 class LinearFinetuneRegressor(LinearFinetune, RegressorMixin):
     ...
 
 
 class LinearFinetuneClassifier(LinearFinetune, ClassifierMixin):
     ...
 
 
+class LinearModelPytorch(torch.nn.Module):
+    def __init__(self, in_features, out_classes):
+        super(LinearModelPytorch, self).__init__()
+        self.linear = torch.nn.Linear(in_features, out_classes)
+
+    def forward(self, x):
+        return self.linear(x)
+
+
+def sigmoid(z):
+    """Apply the sigmoid function."""
+    return 1 / (1 + np.exp(-z))
+
+
 if __name__ == "__main__":
     import imodelsx.data
 
     dset, k = imodelsx.data.load_huggingface_dataset(
-        "rotten_tomatoes", binary_classification=False, subsample_frac=0.1
+        "rotten_tomatoes", subsample_frac=0.01
     )
+    text_test = dset["test"]["text"][:100]
     print(dset)
     print(dset["train"])
     print(np.unique(dset["train"]["label"]))
 
     clf = LinearFinetuneClassifier()
     clf.fit(dset["train"]["text"], dset["train"]["label"])
 
-    print("predicting")
-    preds = clf.predict(dset["test"]["text"])
-    print(preds.shape)
-
     print("predicting proba")
-    preds_proba = clf.predict_proba(dset["test"]["text"])
+    preds_proba = clf.predict_proba(text_test)
     print(preds_proba.shape)
 
+    print('predicting proba pytorch')
+    clf_pytorch = clf._export_to_pytorch()
+    preds_pytorch = clf_pytorch(torch.tensor(clf._get_embs(text_test)))
+    preds_proba_pytorch = sigmoid(preds_pytorch.detach().numpy())
+    assert np.allclose(preds_proba[:, 1].flatten(
+    ), preds_proba_pytorch.flatten(), atol=1e-3)
+
+    print("predicting")
+    preds = clf.predict(text_test)
+
     assert preds_proba.shape[0] == preds.shape[0]
     print(
         "acc_train",
         np.mean(clf.predict(dset["train"]["text"]) == dset["train"]["label"]),
     )
     print("acc_test", np.mean(preds == dset["test"]["label"]))
```

### Comparing `imodelsx-1.0.0/imodelsx/linear_ngram.py` & `imodelsx-1.0.1/imodelsx/linear_ngram.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/llm.py` & `imodelsx-1.0.1/imodelsx/llm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from copy import deepcopy
 import json
 from transformers import (
     T5ForConditionalGeneration,
 )
 import transformers
 from transformers import AutoConfig, AutoModel, AutoTokenizer, AutoModelForCausalLM
 import re
@@ -12,21 +13,27 @@
 from os.path import join, dirname
 import os
 import pickle as pkl
 from scipy.special import softmax
 import hashlib
 import torch
 import time
+from tqdm import tqdm
 
-
+HF_TOKEN = None
+if 'HF_TOKEN' in os.environ:
+    HF_TOKEN = os.environ.get("HF_TOKEN")
+elif os.path.exists('~/.HF_TOKEN'):
+    HF_TOKEN = open(os.path.expanduser('~/.HF_TOKEN'), 'r').read().strip()
 '''
 Example usage:
-checkpoint = 'meta-llama/Llama-2-7b-hf' # gpt-4, gpt-35-turbo, meta-llama/Llama-2-70b-hf, mistralai/Mistral-7B-v0.1
+# gpt-4, gpt-35-turbo, meta-llama/Llama-2-70b-hf, mistralai/Mistral-7B-v0.1
+checkpoint = 'meta-llama/Llama-2-7b-hf'
 llm = imodelsx.llm.get_llm(checkpoint)
-llm('may the force be') # returns ' with you'    
+llm('may the force be') # returns ' with you'
 '''
 
 # change these settings before using these classes!
 LLM_CONFIG = {
     # how long to wait before recalling a failed llm call (can set to None)
     "LLM_REPEAT_DELAY": None,
     "CACHE_DIR": join(
@@ -50,14 +57,16 @@
         LLM_CONFIG["LLM_REPEAT_DELAY"] = repeat_delay
 
     """Get an LLM with a call function and caching capabilities"""
     if checkpoint.startswith("text-da"):
         return LLM_OpenAI(checkpoint, seed=seed, CACHE_DIR=CACHE_DIR)
     elif checkpoint.startswith("gpt-3") or checkpoint.startswith("gpt-4"):
         return LLM_Chat(checkpoint, seed, role, CACHE_DIR)
+    elif 'Meta-Llama-3-8B' in checkpoint and 'Instruct' in checkpoint:
+        return LLM_HF_Pipeline(checkpoint, CACHE_DIR)
     else:
         # warning: this sets torch.manual_seed(seed)
         return LLM_HF(checkpoint, seed=seed, CACHE_DIR=CACHE_DIR, LLAMA_DIR=LLAMA_DIR)
 
 
 def repeatedly_call_with_delay(llm_call):
     def wrapper(*args, **kwargs):
@@ -97,14 +106,16 @@
         self.checkpoint = checkpoint
 
     @repeatedly_call_with_delay
     def __call__(
         self,
         prompt: str,
         max_new_tokens=250,
+        frequency_penalty=0.25,  # maximum is 2
+        temperature=0.1,
         do_sample=True,
         stop=None,
         return_str=True,
     ):
         import openai
 
         # cache
@@ -115,17 +126,17 @@
         if os.path.exists(cache_file):
             return pkl.load(open(cache_file, "rb"))
 
         response = openai.Completion.create(
             engine=self.checkpoint,
             prompt=prompt,
             max_tokens=max_new_tokens,
-            temperature=0.1,
+            temperature=temperature,
             top_p=1,
-            frequency_penalty=0.25,  # maximum is 2
+            frequency_penalty=frequency_penalty,
             presence_penalty=0,
             stop=stop,
             # stop=["101"]
         )
         if return_str:
             response = response["choices"][0]["text"]
 
@@ -164,15 +175,16 @@
         frequency_penalty=0.25,
     ):
         """
         prompts_list: list of dicts, each dict has keys 'role' and 'content'
             Example: [
                 {"role": "system", "content": "You are a helpful assistant."},
                 {"role": "user", "content": "Who won the world series in 2020?"},
-                {"role": "assistant", "content": "The Los Angeles Dodgers won the World Series in 2020."},
+                {"role": "assistant",
+                    "content": "The Los Angeles Dodgers won the World Series in 2020."},
                 {"role": "user", "content": "Where was it played?"}
             ]
         prompts_list: str
             Alternatively, string which gets formatted into basic prompts_list:
             messages = [
                 {"role": "system", "content": "You are a helpful assistant."},
                 {"role": "user", "content": <<<<<prompts_list>>>>},
@@ -240,70 +252,130 @@
 
         return response
 
 
 def load_tokenizer(checkpoint: str) -> transformers.PreTrainedTokenizer:
     if "facebook/opt" in checkpoint:
         # opt can't use fast tokenizer
-        return AutoTokenizer.from_pretrained(checkpoint, use_fast=False, padding_side='left')
+        tokenizer = AutoTokenizer.from_pretrained(
+            checkpoint, use_fast=False, padding_side='left', token=HF_TOKEN)
     elif "PMC_LLAMA" in checkpoint:
-        return transformers.LlamaTokenizer.from_pretrained("chaoyi-wu/PMC_LLAMA_7B", padding_side='left')
+        tokenizer = transformers.LlamaTokenizer.from_pretrained(
+            "chaoyi-wu/PMC_LLAMA_7B", padding_side='left', token=HF_TOKEN)
     else:
         # , use_fast=True)
-        return AutoTokenizer.from_pretrained(checkpoint, padding_side='left')
-    # return AutoTokenizer.from_pretrained(checkpoint,
-    # token=os.environ.get("LLAMA_TOKEN"),)
+        tokenizer = AutoTokenizer.from_pretrained(
+            checkpoint, padding_side='left', use_fast=True, token=HF_TOKEN)
+
+    if tokenizer.pad_token_id is None:
+        tokenizer.pad_token_id = tokenizer.eos_token_id
+    return tokenizer
+
+
+def load_hf_model(checkpoint: str) -> transformers.PreTrainedModel:
+    # set checkpoint
+    kwargs = {
+        "pretrained_model_name_or_path": checkpoint,
+        "output_hidden_states": False,
+        # "pad_token_id": tokenizer.eos_token_id,
+        "low_cpu_mem_usage": True,
+    }
+    if "google/flan" in checkpoint:
+        return T5ForConditionalGeneration.from_pretrained(
+            checkpoint, device_map="auto", torch_dtype=torch.float16
+        )
+    elif checkpoint == "EleutherAI/gpt-j-6B":
+        return AutoModelForCausalLM.from_pretrained(
+            checkpoint,
+            revision="float16",
+            torch_dtype=torch.float16,
+            **kwargs,
+        )
+    elif "llama-2" in checkpoint.lower():
+        return AutoModelForCausalLM.from_pretrained(
+            checkpoint,
+            torch_dtype=torch.float16,
+            device_map="auto",
+            token=HF_TOKEN,
+            offload_folder="offload",
+        )
+    elif "llama_" in checkpoint:
+        return transformers.LlamaForCausalLM.from_pretrained(
+            join(LLAMA_DIR, checkpoint),
+            device_map="auto",
+            torch_dtype=torch.float16,
+        )
+    elif 'microsoft/phi' in checkpoint:
+        return AutoModelForCausalLM.from_pretrained(
+            checkpoint
+        )
+    elif checkpoint == "gpt-xl":
+        return AutoModelForCausalLM.from_pretrained(checkpoint)
+    else:
+        return AutoModelForCausalLM.from_pretrained(
+            checkpoint, device_map="auto", torch_dtype=torch.float16,
+            token=HF_TOKEN,
+        )
 
 
-class LLM_HF:
-    def __init__(self, checkpoint, seed, CACHE_DIR, LLAMA_DIR=None):
-        self._tokenizer = load_tokenizer(checkpoint)
+class LLM_HF_Pipeline:
+    def __init__(self, checkpoint, CACHE_DIR):
 
-        # set checkpoint
-        kwargs = {
-            "pretrained_model_name_or_path": checkpoint,
-            "output_hidden_states": False,
-            # "pad_token_id": tokenizer.eos_token_id,
-            "low_cpu_mem_usage": True,
-        }
-        if "google/flan" in checkpoint:
-            self._model = T5ForConditionalGeneration.from_pretrained(
-                checkpoint, device_map="auto", torch_dtype=torch.float16
-            )
-        elif checkpoint == "EleutherAI/gpt-j-6B":
-            self._model = AutoModelForCausalLM.from_pretrained(
-                checkpoint,
-                revision="float16",
-                torch_dtype=torch.float16,
-                **kwargs,
-            )
-        elif "llama-2" in checkpoint.lower():
-            self._model = transformers.AutoModelForCausalLM.from_pretrained(
-                checkpoint,
-                torch_dtype=torch.float16,
-                device_map="auto",
-                token=os.environ.get("LLAMA_TOKEN"),
-                offload_folder="offload",
-            )
-        elif "llama_" in checkpoint:
-            self._model = transformers.LlamaForCausalLM.from_pretrained(
-                join(LLAMA_DIR, checkpoint),
-                device_map="auto",
-                torch_dtype=torch.float16,
-            )
-        elif 'microsoft/phi' in checkpoint:
-            self._model = AutoModelForCausalLM.from_pretrained(
-                checkpoint
+        self.pipeline_ = transformers.pipeline(
+            "text-generation",
+            model=checkpoint,
+            model_kwargs={"torch_dtype": torch.bfloat16},
+            device_map="auto"
+        )
+        self.cache_dir = join(CACHE_DIR)
+
+    def __call__(
+        self,
+        prompt: Union[str, List[str]],
+        max_new_tokens=20,
+        use_cache=True,
+        verbose=False,
+    ):
+
+        if use_cache:
+            os.makedirs(self.cache_dir, exist_ok=True)
+            hash_str = hashlib.sha256(str(prompt).encode()).hexdigest()
+            cache_file = join(
+                self.cache_dir, f"{hash_str}__num_tok={max_new_tokens}.pkl"
             )
-        elif checkpoint == "gpt-xl":
-            self._model = AutoModelForCausalLM.from_pretrained(checkpoint)
+
+            if os.path.exists(cache_file):
+                if verbose:
+                    print("cached!")
+                try:
+                    return pkl.load(open(cache_file, "rb"))
+                except:
+                    print('failed to load cache so rerunning...')
+            if verbose:
+                print("not cached...")
+        outputs = self.pipeline_(
+            prompt,
+            max_new_tokens=max_new_tokens,
+        )
+        print('outs', outputs)
+        if isinstance(prompt, str):
+            texts = outputs[0]["generated_text"][len(prompt):]
         else:
-            self._model = AutoModelForCausalLM.from_pretrained(
-                checkpoint, device_map="auto", torch_dtype=torch.float16
-            )
+            texts = [outputs[i][0]['generated_text']
+                     [len(prompt[i]):] for i in range(len(outputs))]
+
+        if use_cache:
+            pkl.dump(texts, open(cache_file, "wb"))
+        return texts
+
+
+class LLM_HF:
+    def __init__(self, checkpoint, seed, CACHE_DIR, LLAMA_DIR=None):
+        self.tokenizer_ = load_tokenizer(checkpoint)
+        self.model_ = load_hf_model(checkpoint)
         self.checkpoint = checkpoint
         self.cache_dir = join(
             CACHE_DIR, "cache_hf", f'{checkpoint.replace("/", "_")}___{seed}'
         )
         self.seed = seed
 
     def __call__(
@@ -318,14 +390,16 @@
         target_token_strs: List[str] = None,
         return_top_target_token_str: bool = False,
         # batch_size=1,
     ) -> Union[str, List[str]]:
         """Warning: stop is used posthoc but not during generation.
         Be careful, caching can take up a lot of memory....
 
+        Example mistral-instruct prompt: "<s>[INST]'Input text: {example}\nQuestion: {question} Answer yes or no.[/INST]"
+
 
         Params
         ------
         return_next_token_prob_scores: bool
             If this is true, then the function will return the probability of the next token being each of the target_token_strs
             target_token_strs: List[str]
                 If this is not None and return_next_token_prob_scores is True, then the function will return the probability of the next token being each of the target_token_strs
@@ -354,28 +428,26 @@
                     except:
                         print('failed to load cache so rerunning...')
                 if verbose:
                     print("not cached...")
 
             # if stop is not None:
             # raise ValueError("stop kwargs are not permitted.")
-            if self._tokenizer.pad_token_id is None:
-                self._tokenizer.pad_token_id = self._tokenizer.eos_token_id
-            inputs = self._tokenizer(
+            inputs = self.tokenizer_(
                 prompt, return_tensors="pt",
                 return_attention_mask=True,
                 padding=True,
                 truncation=False,
-            ).to(self._model.device)
+            ).to(self.model_.device)
 
             if return_next_token_prob_scores or target_token_strs or return_top_target_token_str:
-                outputs = self._model.generate(
+                outputs = self.model_.generate(
                     **inputs,
                     max_new_tokens=1,
-                    pad_token_id=self._tokenizer.pad_token_id,
+                    pad_token_id=self.tokenizer_.pad_token_id,
                     output_logits=True,
                     return_dict_in_generate=True,
                 )
                 next_token_logits = outputs['logits'][0]
                 next_token_probs = next_token_logits.softmax(
                     axis=-1).detach().cpu().numpy()
 
@@ -401,64 +473,104 @@
                         {target_token_strs[i]: next_token_probs[prompt_num, target_token_ids[i]]
                             for i in range(len(target_token_strs))
                          }
                         for prompt_num in range(len(prompt))
                     ]
                     return out_dict_list
             else:
-                outputs = self._model.generate(
+                outputs = self.model_.generate(
                     **inputs,
                     max_new_tokens=max_new_tokens,
                     do_sample=do_sample,
-                    pad_token_id=self._tokenizer.pad_token_id,
+                    pad_token_id=self.tokenizer_.pad_token_id,
                 )
                 # top_p=0.92,
                 # temperature=0,
                 # top_k=0
             if input_is_str:
-                out_str = self._tokenizer.decode(
+                out_str = self.tokenizer_.decode(
                     outputs[0], skip_special_tokens=True)
-                out_str = out_str[len(prompt):]
+                # print('out_str', out_str)
+                if 'mistral' in self.checkpoint and 'Instruct' in self.checkpoint:
+                    out_str = out_str[len(prompt) - 2:]
+                elif 'Meta-Llama-3' in self.checkpoint and 'Instruct' in self.checkpoint:
+                    out_str = out_str[len(prompt) - 145:]
+                else:
+                    out_str = out_str[len(prompt):]
+
                 if use_cache:
                     pkl.dump(out_str, open(cache_file, "wb"))
                 return out_str
             else:
                 out_strs = []
                 for i in range(outputs.shape[0]):
                     out_tokens = outputs[i]
-                    out_str = self._tokenizer.decode(
+                    out_str = self.tokenizer_.decode(
                         out_tokens, skip_special_tokens=True)
-                    out_str = out_str[len(prompt[i]):]
+                    if 'mistral' in self.checkpoint and 'Instruct' in self.checkpoint:
+                        out_str = out_str[len(prompt[i]) - 2:]
+                    elif 'Meta-Llama-3' in self.checkpoint and 'Instruct' in self.checkpoint:
+                        # print('here')
+                        out_str = out_str[len(prompt) + 187:]
+                    else:
+                        out_str = out_str[len(prompt[i]):]
                     out_strs.append(out_str)
                 if use_cache:
                     pkl.dump(out_strs, open(cache_file, "wb"))
                 return out_strs
 
     def _check_target_token_strs(self, target_token_strs, override_token_with_first_token_id=False):
         if isinstance(target_token_strs, str):
             target_token_strs = [target_token_strs]
 
-        target_token_ids = [self._tokenizer(target_token_str, add_special_tokens=False)["input_ids"]
+        target_token_ids = [self.tokenizer_(target_token_str, add_special_tokens=False)["input_ids"]
                             for target_token_str in target_token_strs]
 
         # Check that the target token is in the vocab
         if override_token_with_first_token_id:
             # Get first token id in target_token_str
             target_token_ids = [target_token_id[0]
                                 for target_token_id in target_token_ids]
         else:
             for i in range(len(target_token_strs)):
                 if len(target_token_ids[i]) > 1:
                     raise ValueError(
                         f"target_token_str {target_token_strs[i]} has multiple tokens: " +
-                        str([self._tokenizer.decode(target_token_id)
+                        str([self.tokenizer_.decode(target_token_id)
                             for target_token_id in target_token_ids[i]]))
         return target_token_ids
 
 
+class LLMEmbs:
+    def __init__(self, checkpoint):
+        self.tokenizer_ = load_tokenizer(checkpoint)
+        self.model_ = AutoModel.from_pretrained(
+            checkpoint, output_hidden_states=True,
+            device_map="auto",
+            torch_dtype=torch.float16,)
+
+    def __call__(self, texts: List[str], layer_idx: int = 18, batch_size=16):
+        '''Returns embeddings
+        '''
+        embs = []
+        for i in tqdm(range(0, len(texts), batch_size)):
+            inputs = self.tokenizer_(
+                texts[i:i + batch_size], return_tensors='pt', padding=True).to(self.model_.device)
+            hidden_states = self.model_(**inputs).hidden_states
+
+            # layers x batch x tokens x features
+            emb = hidden_states[layer_idx].detach().cpu().numpy()
+
+            # get emb from last token
+            emb = emb[:, -1, :]
+            embs.append(deepcopy(emb))
+        embs = np.concatenate(embs)
+        return embs
+
+
 if __name__ == "__main__":
     # llm = get_llm("text-davinci-003")
     # text = llm("What do these have in common? Horse, ")
     # print("text", text)
 
     # llm = get_llm("gpt2")
     # text = llm(
@@ -490,15 +602,15 @@
     # llm = get_llm("gpt2")
     # prompts = ['roses are red, violets are', 'may the force be with']
     # # prompts = ['may the force be with', 'so may the light be with']
     # target_token_strs = [' blue', ' you']
     # ans = llm(prompts, return_next_token_prob_scores=True,
     #           use_cache=False, target_token_strs=target_token_strs)
 
-    # FORCE WORDSSSSSSSSS ##########
+    # FORCE WORDS ##########
     llm = get_llm("gpt2")
     prompts = ['roses are red, violets are',
                'may the force be with', 'trees are usually']
     # prompts = ['may the force be with', 'so may the light be with']
     target_token_strs = [' green', ' you', 'orange']
     llm._check_target_token_strs(target_token_strs)
     ans = llm(prompts, use_cache=False,
```

### Comparing `imodelsx-1.0.0/imodelsx/metrics.py` & `imodelsx-1.0.1/imodelsx/metrics.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/process_results.py` & `imodelsx-1.0.1/imodelsx/process_results.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import numpy as np
 import joblib
 import json
 
 repo_dir = dirname(dirname(os.path.abspath(__file__)))
 
 
-def get_results_df(results_dir, use_cached=False, results_fname='results.pkl') -> pd.DataFrame:
+def get_results_df(results_dir, use_cached=False, results_fname='results.pkl', save_pickle=False) -> pd.DataFrame:
     """Load results from a directory of experiments,
     each experiments is a row in the dataframe
     """
     fname = join(results_dir, "results_aggregated.pkl")
     if use_cached and os.path.exists(fname):
         return pd.read_pickle(fname)
     dir_names = sorted(
@@ -42,15 +42,16 @@
                     open(join(results_dir, dir_name, results_fname), "r"))
             ser = pd.Series(result)
             results_list.append(ser)
         except:
             print(
                 f'Error loading {join(results_dir, dir_name, results_fname)}')
     r = pd.concat(results_list, axis=1).T.infer_objects()
-    r.to_pickle(fname)
+    if save_pickle:
+        r.to_pickle(fname)
     return r
 
 
 def get_main_args_list(experiment_filename="01_train_model.py"):
     """Returns main arguments from the argparser used by an experiments script
 
     Params
@@ -89,27 +90,35 @@
         if v is None:
             v = "None"
         df[k] = df[k].fillna(v)
     return df
 
 
 def delete_runs_in_dataframe(
-    df: pd.DataFrame, actually_delete=False, directory_key="save_dir_unique"
+    df: pd.DataFrame, actually_delete=False,
+    directory_key="save_dir_unique",
+    # save_dir_prefix_replace=('/mntv1', '/home/chansingh/mntv1')
 ):
     """Deletes stored results for all runs in the dataframe r."""
     if not actually_delete:
         print(
             f"Not actually deleting {df.shape[0]} directories. Set actually_delete=True to actually delete the directories."
         )
         return
 
     num_deleted = 0
     for i in tqdm(range(df.shape[0])):
+        save_dir = df.iloc[i][directory_key]
+        # if save_dir_prefix_replace is not None:
+        #     if save_dir.startswith(save_dir_prefix_replace[0]):
+        #         save_dir = save_dir.replace(
+        #             save_dir_prefix_replace[0], save_dir_prefix_replace[1]
+        #         )
         try:
-            os.system(f"rm -rf {df.iloc[i][directory_key]}")
+            os.system(f"rm -rf {save_dir}")
             num_deleted += 1
         except:
             pass
     print(f"Deleted {num_deleted}/{df.shape[0]} directories.")
 
 
 def average_over_seeds(
```

### Comparing `imodelsx-1.0.0/imodelsx/sasc/api.py` & `imodelsx-1.0.1/imodelsx/sasc/api.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/sasc/m1_ngrams.py` & `imodelsx-1.0.1/imodelsx/sasc/m1_ngrams.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/sasc/m2_summarize.py` & `imodelsx-1.0.1/imodelsx/sasc/m2_summarize.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/sasc/m3_generate.py` & `imodelsx-1.0.1/imodelsx/sasc/m3_generate.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/submit_utils.py` & `imodelsx-1.0.1/imodelsx/submit_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     args_list: List[Dict[str, Any]],
     cmd_python: str = 'python',
     script_name: str = '02_train_suffix.py',
     actually_run: bool = True,
     debug_mode: bool = False,
     shuffle: bool = False,
     reverse: bool = False,
+    unique_seeds: bool = False,
     n_cpus: int = 1,
     gpu_ids: Union[List[int], List[List[int]]] = [],
     repeat_failed_jobs: bool = False,
     slurm: bool = False,
     slurm_kwargs: Optional[Dict] = None,
     amlt_kwargs: Optional[Dict] = None,
 ):
@@ -45,14 +46,16 @@
         Whether to actually run the script (otherwise just print the command)
     debug_mode: bool
         Whether to open debugger after failure (stops all parallelilization) 
     shuffle: bool
         Whether to shuffle the order of the script calls
     reverse: bool
         Whether to reverse the order of the script calls
+    unique_seeds: bool
+        Whether to assign random, unique seeds to each run
     n_cpus: int
         Number of cpus to use (if >1, parallelizes over local machine)
     gpu_ids: List[int], List[List[int]]
         Ids of GPUs to run on (e.g. [0, 1] for 2 gpus)
         If List[List[int]], then each inner list is a group of GPUs to run on, e.g. [[0, 1], [2, 3]] for 2 groups of 2 GPUs
     repeat_failed_jobs: bool
         Whether to repeatedly run failed jobs
@@ -79,14 +82,19 @@
     if debug_mode:
         cmd_python = 'python -m pdb -c continue'
         if n_cpus > 1 or n_gpus > 1:
             print('\n###\n### Debug mode, setting n_cpus=1 and n_gpus=0 ###\n###\n')
             n_cpus = 1
             n_gpus = 0
 
+    # assign unique seeds
+    if unique_seeds:
+        for i, args in enumerate(args_list):
+            args_list[i]['seed'] = random.randint(1, int(1e6))
+
     # construct commands
     param_str_list = [_param_str_from_args(
         args, cmd_python, script_name) for args in args_list]
 
     # just print and exit
     if not actually_run:
         print('Not actually running the commands, just printing them.')
@@ -102,35 +110,53 @@
             print(
                 f'\n\n-------------------{i + 1}/{len(param_str_list)}--------------------\n' + param_str)
             run_slurm(param_str, slurm_kwargs=slurm_kwargs)
         return
     elif amlt_kwargs is not None:
         assert 'amlt_file' in amlt_kwargs
         sku = amlt_kwargs.get('sku', 'G1')
+        process_count_per_node = amlt_kwargs.get('process_count_per_node', 1)
         amlt_dir = dirname(amlt_kwargs['amlt_file'])
-
         amlt_text = open(amlt_kwargs['amlt_file'], 'r').read()
+        assert amlt_text.endswith('jobs:'), 'amlt file must end with jobs:'
         script_name = script_name.replace(amlt_dir, '').strip('/')
         param_str_list = [_param_str_from_args(
-            args, 'python', script_name) for args in args_list]
+            args, cmd_python, script_name) for args in args_list]
+        if 'mnt_rename' in amlt_kwargs:
+            param_str_list = [
+                param_str.replace(
+                    amlt_kwargs['mnt_rename'][0], amlt_kwargs['mnt_rename'][1])
+                for param_str in param_str_list
+            ]
 
+        # save yaml file with multiple jobs in logs dir and run with amlt
         logs_dir = join(amlt_dir, 'logs')
         os.makedirs(logs_dir, exist_ok=True)
+        job_template = '''
+- name: {name}
+  process_count_per_node: {process_count_per_node}
+  sku: {sku}
+  command:
+  - {param_str}'''
+        out_file = join(logs_dir, sha256({'s': str(param_str_list)}) + '.yaml')
+        s = amlt_text
         for i, param_str in enumerate(param_str_list):
-            out_file = join(logs_dir, sha256(
-                {'s': param_str_list[i]}) + '.yaml')
-            s = amlt_text.format(
-                param_str=param_str_list[i],
-                sku=sku
-            ).replace('$CONFIG_DIR', '$CONFIG_DIR/..')
-            with open(out_file, 'w') as f:
-                f.write(s)
-            subprocess.run(
-                f'amlt run {out_file}', shell=True, check=True,
+            job_text = job_template.format(
+                name=f'job_{i}',
+                process_count_per_node=process_count_per_node,
+                sku=sku,
+                param_str=param_str
             )
+            s = s + job_text
+        s = s.replace('$CONFIG_DIR', '$CONFIG_DIR/..')
+        with open(out_file, 'w') as f:
+            f.write(s)
+        subprocess.run(
+            f'amlt run {out_file}', shell=True, check=True,
+        )
         return
 
     # run serial
     elif n_cpus == 1 and n_gpus == 0:
         for i, param_str in enumerate(param_str_list):
             print(
                 f'\n\n-------------------{i + 1}/{len(param_str_list)}--------------------\n' + param_str)
@@ -269,15 +295,15 @@
     finally:
         job_queue_multiprocessing.put(gpu_id)
         return failed_job
 
 
 def get_args_list(
     params_shared_dict: Dict[str, List],
-    params_coupled_dict: Dict[Tuple[str], List[Tuple]],
+    params_coupled_dict: Dict[Tuple[str], List[Tuple]] = {},
 ) -> List[Dict[str, Any]]:
     _validate_arguments(params_shared_dict, params_coupled_dict)
 
     def combos_collapse(l: List[List[Dict]]) -> List[Dict]:
         # get param combos as List[Tuple[Dict]] then convert to List[Dict]
         return [
             # convert List[Dict[Tuple]] -> List[Dict]
@@ -312,14 +338,16 @@
 
 
 def _validate_arguments(
     params_shared_dict: Dict[str, List],
     params_coupled_dict: Dict[Tuple[str], List[Tuple]],
 ):
     for k, v in params_shared_dict.items():
+        if isinstance(v, range):
+            v = list(v)
         assert isinstance(
             k, str), f"params_shared_dict key {k} must be type list, got type {type(k)}"
         assert isinstance(
             v, list), f"params_shared_dict val {v} must be type list, got type {type(v)}"
     for k_tup, v_tup_list in params_coupled_dict.items():
         assert isinstance(
             k_tup, tuple), f"params_coupled_dict key {k_tup} must be type tuple, got type {type(k_tup)}"
```

### Comparing `imodelsx-1.0.0/imodelsx/treeprompt/stump.py` & `imodelsx-1.0.1/imodelsx/treeprompt/stump.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/treeprompt/treeprompt.py` & `imodelsx-1.0.1/imodelsx/treeprompt/treeprompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             1:
         ]  # remove first element which is -2
 
         return self
 
     def _calc_prompt_features(self, X, prompts):
         prompt_features = np.zeros((len(X), len(prompts)))
-        llm = imodelsx.llm.get_llm(self.checkpoint)._model
+        llm = imodelsx.llm.get_llm(self.checkpoint).model_
         if self.device is not None:
             llm = llm.to(self.device)
         stump = None
 
         for i, prompt in enumerate(prompts):
             print(f"Prompt {i}: {prompt}")
```

### Comparing `imodelsx-1.0.0/imodelsx/util.py` & `imodelsx-1.0.1/imodelsx/util.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx/viz.py` & `imodelsx-1.0.1/imodelsx/viz.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/imodelsx.egg-info/PKG-INFO` & `imodelsx-1.0.1/imodelsx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imodelsx
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library to explain a dataset in natural language.
 Home-page: https://github.com/csinva/imodelsX
 Author: Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah Hsu, Yuntian Deng
 Author-email: chansingh@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: imodelsx Version: 1.0.0 Summary: Library to explain
+Metadata-Version: 2.1 Name: imodelsx Version: 1.0.1 Summary: Library to explain
 a dataset in natural language. Home-page: https://github.com/csinva/imodelsX
 Author: Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah
 Hsu, Yuntian Deng Author-email: chansingh@microsoft.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown
   [https://microsoft.github.io/aug-models/embgam_gif.gif][https://csinva.io/
```

### Comparing `imodelsx-1.0.0/imodelsx.egg-info/SOURCES.txt` & `imodelsx-1.0.1/imodelsx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/setup.py` & `imodelsx-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     # 'InstructorEmbedding', # embeddings for emb_diff_module
     # 'sentence-transformers', # embeddings for emb_diff_module
     # pdoc3 # for generating docs
 ]
 
 setuptools.setup(
     name="imodelsx",
-    version="1.0.0",
+    version="1.0.1",
     author="Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah Hsu, Yuntian Deng",
     author_email="chansingh@microsoft.com",
     description="Library to explain a dataset in natural language.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/csinva/imodelsX",
     packages=setuptools.find_packages(
```

### Comparing `imodelsx-1.0.0/tests/test_auglinear_pipeline.py` & `imodelsx-1.0.1/tests/test_auglinear_pipeline.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/tests/test_augtree.py` & `imodelsx-1.0.1/tests/test_augtree.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/tests/test_iprompt.py` & `imodelsx-1.0.1/tests/test_iprompt.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/tests/test_llm.py` & `imodelsx-1.0.1/tests/test_llm.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/tests/test_ngram_list.py` & `imodelsx-1.0.1/tests/test_ngram_list.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.0/tests/test_sasc.py` & `imodelsx-1.0.1/tests/test_sasc.py`

 * *Files identical despite different names*

