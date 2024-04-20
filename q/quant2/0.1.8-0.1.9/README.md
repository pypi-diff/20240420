# Comparing `tmp/quant2-0.1.8.tar.gz` & `tmp/quant2-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant2-0.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "quant2-0.1.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `quant2-0.1.8.tar` & `quant2-0.1.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      574 2024-04-06 14:41:03.615629 quant2-0.1.8/.gitignore
--rw-r--r--   0        0        0    11357 2024-03-20 11:12:02.832412 quant2-0.1.8/LICENSE
--rw-r--r--   0        0        0        7 2024-03-20 11:12:02.832412 quant2-0.1.8/README.md
--rw-r--r--   0        0        0      971 2024-04-14 08:14:34.409434 quant2-0.1.8/configs/stnetv3/stnetv3_table20240326_2201to2312.cfg
--rw-r--r--   0        0        0     1049 2024-04-12 08:57:23.226862 quant2-0.1.8/configs/stnetv4/stnetv4_table20240410_2201to2312.cfg
--rw-r--r--   0        0        0      664 2024-04-10 00:12:18.347578 quant2-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1841 2024-03-23 05:01:23.359992 quant2-0.1.8/quant/README.md
--rw-r--r--   0        0        0      559 2024-04-19 14:23:17.224708 quant2-0.1.8/quant/__init__.py
--rw-r--r--   0        0        0       67 2024-03-23 04:17:48.269987 quant2-0.1.8/quant/__main__.py
--rw-r--r--   0        0        0        0 2024-04-08 01:35:10.284089 quant2-0.1.8/quant/evaluate/__init__.py
--rw-r--r--   0        0        0     2315 2024-04-18 14:45:48.737962 quant2-0.1.8/quant/evaluate/meters.py
--rw-r--r--   0        0        0     2584 2024-04-19 09:07:38.924732 quant2-0.1.8/quant/evaluate/table20240326.py
--rw-r--r--   0        0        0     3658 2024-04-19 09:14:49.360976 quant2-0.1.8/quant/evaluate/utils.py
--rw-r--r--   0        0        0      422 2024-03-23 04:21:50.819993 quant2-0.1.8/quant/football/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 14:09:03.305285 quant2-0.1.8/quant/football/data/__init__.py
--rw-r--r--   0        0        0     4348 2024-04-14 08:11:01.537268 quant2-0.1.8/quant/football/data/dataset.py
--rw-r--r--   0        0        0        0 2024-04-08 10:24:35.916611 quant2-0.1.8/quant/football/data/functional.py
--rw-r--r--   0        0        0     1336 2024-04-15 11:24:33.080117 quant2-0.1.8/quant/football/data/preprocessing.py
--rw-r--r--   0        0        0      993 2024-04-17 06:41:14.170874 quant2-0.1.8/quant/football/data/sampler.py
--rw-r--r--   0        0        0        0 2024-04-08 11:08:36.928001 quant2-0.1.8/quant/football/data/stats.py
--rw-r--r--   0        0        0     4560 2024-04-13 08:19:58.059662 quant2-0.1.8/quant/football/data/utils.py
--rw-r--r--   0        0        0        0 2024-04-11 16:55:37.649284 quant2-0.1.8/quant/football/infer/__init__.py
--rw-r--r--   0        0        0     2024 2024-04-16 01:19:44.599739 quant2-0.1.8/quant/football/infer/fastapi_app.py
--rw-r--r--   0        0        0      468 2024-04-11 16:55:50.160241 quant2-0.1.8/quant/football/infer/fastapi_app_test.py
--rw-r--r--   0        0        0     8035 2024-04-19 08:10:26.065510 quant2-0.1.8/quant/football/infer/football_infer_overunder_v1.py
--rw-r--r--   0        0        0      473 2024-04-11 16:56:07.430215 quant2-0.1.8/quant/football/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 04:22:28.629548 quant2-0.1.8/quant/football/models/mtnet.py
--rw-r--r--   0        0        0     6110 2024-04-11 17:12:37.365849 quant2-0.1.8/quant/football/models/stnet.py
--rw-r--r--   0        0        0      547 2024-04-19 12:53:57.861344 quant2-0.1.8/quant/football/transforms/__init__.py
--rw-r--r--   0        0        0     6622 2024-04-16 00:40:54.525920 quant2-0.1.8/quant/football/transforms/table20240326.py
--rw-r--r--   0        0        0     8541 2024-04-16 01:19:10.126956 quant2-0.1.8/quant/football/transforms/table20240410.py
--rw-r--r--   0        0        0     8825 2024-04-16 00:40:14.674251 quant2-0.1.8/quant/football/transforms/table20240414.py
--rw-r--r--   0        0        0     8396 2024-04-16 02:25:15.544645 quant2-0.1.8/quant/football/transforms/table20240415.py
--rw-r--r--   0        0        0     8669 2024-04-19 14:23:21.974668 quant2-0.1.8/quant/football/transforms/table20240419.py
--rw-r--r--   0        0        0        0 2024-03-31 10:26:04.538951 quant2-0.1.8/quant/layers/__init__.py
--rw-r--r--   0        0        0      483 2024-03-28 09:12:19.609652 quant2-0.1.8/quant/layers/layer_scale.py
--rw-r--r--   0        0        0     1070 2024-03-28 09:13:06.741829 quant2-0.1.8/quant/layers/mlp.py
--rw-r--r--   0        0        0     1314 2024-03-28 09:40:33.643889 quant2-0.1.8/quant/layers/normalization.py
--rw-r--r--   0        0        0      852 2024-03-28 09:16:09.540017 quant2-0.1.8/quant/layers/swiglu_ffn.py
--rw-r--r--   0        0        0        0 2024-04-03 13:03:10.745509 quant2-0.1.8/quant/utils/__init__.py
--rw-r--r--   0        0        0     1695 2024-04-11 16:56:25.721657 quant2-0.1.8/quant/utils/archive.py
--rw-r--r--   0        0        0     1884 2024-04-14 08:14:07.935771 quant2-0.1.8/quant/utils/config.py
--rw-r--r--   0        0        0     1047 2024-04-09 01:40:57.919653 quant2-0.1.8/quant/utils/io.py
--rw-r--r--   0        0        0     1006 2024-04-03 13:19:59.255567 quant2-0.1.8/quant/utils/logging.py
--rw-r--r--   0        0        0      182 2024-03-28 01:09:02.081511 quant2-0.1.8/tests/football/data/test_utils.py
--rw-r--r--   0        0        0     1632 2024-04-12 06:45:57.389803 quant2-0.1.8/tools/analysis_tools/analyze_cls_results.py
--rw-r--r--   0        0        0     2645 2024-04-16 01:48:23.763355 quant2-0.1.8/tools/experimental/make_dataset.py
--rw-r--r--   0        0        0     1580 2024-04-13 14:41:36.176420 quant2-0.1.8/tools/experimental/make_split.py
--rw-r--r--   0        0        0     8078 2024-04-17 06:34:03.034798 quant2-0.1.8/tools/experimental/nni_football.py
--rw-r--r--   0        0        0      600 2024-04-17 07:13:13.694051 quant2-0.1.8/tools/experimental/nni_football_config.yaml
--rw-r--r--   0        0        0     1832 2024-04-17 08:12:07.193491 quant2-0.1.8/tools/experimental/nni_football_config_search_space.json
--rw-r--r--   0        0        0      523 2024-04-14 02:37:47.884925 quant2-0.1.8/tools/experimental/nni_model.py
--rw-r--r--   0        0        0      441 2024-04-14 04:00:22.459245 quant2-0.1.8/tools/experimental/nni_model_config.yaml
--rw-r--r--   0        0        0     2867 2024-04-18 04:24:08.683016 quant2-0.1.8/tools/fb_cls_test.py
--rw-r--r--   0        0        0     7897 2024-04-17 06:33:07.892275 quant2-0.1.8/tools/fb_cls_train.py
--rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 quant2-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      574 2024-04-06 14:41:03.615629 quant2-0.1.9/.gitignore
+-rw-r--r--   0        0        0    11357 2024-03-20 11:12:02.832412 quant2-0.1.9/LICENSE
+-rw-r--r--   0        0        0        7 2024-03-20 11:12:02.832412 quant2-0.1.9/README.md
+-rw-r--r--   0        0        0      971 2024-04-14 08:14:34.409434 quant2-0.1.9/configs/stnetv3/stnetv3_table20240326_2201to2312.cfg
+-rw-r--r--   0        0        0     1049 2024-04-12 08:57:23.226862 quant2-0.1.9/configs/stnetv4/stnetv4_table20240410_2201to2312.cfg
+-rw-r--r--   0        0        0      664 2024-04-10 00:12:18.347578 quant2-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1841 2024-03-23 05:01:23.359992 quant2-0.1.9/quant/README.md
+-rw-r--r--   0        0        0      559 2024-04-19 14:38:39.421733 quant2-0.1.9/quant/__init__.py
+-rw-r--r--   0        0        0       67 2024-03-23 04:17:48.269987 quant2-0.1.9/quant/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-08 01:35:10.284089 quant2-0.1.9/quant/evaluate/__init__.py
+-rw-r--r--   0        0        0     2315 2024-04-18 14:45:48.737962 quant2-0.1.9/quant/evaluate/meters.py
+-rw-r--r--   0        0        0     2584 2024-04-19 09:07:38.924732 quant2-0.1.9/quant/evaluate/table20240326.py
+-rw-r--r--   0        0        0     3658 2024-04-19 09:14:49.360976 quant2-0.1.9/quant/evaluate/utils.py
+-rw-r--r--   0        0        0      422 2024-03-23 04:21:50.819993 quant2-0.1.9/quant/football/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 14:09:03.305285 quant2-0.1.9/quant/football/data/__init__.py
+-rw-r--r--   0        0        0     4348 2024-04-14 08:11:01.537268 quant2-0.1.9/quant/football/data/dataset.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:24:35.916611 quant2-0.1.9/quant/football/data/functional.py
+-rw-r--r--   0        0        0     1336 2024-04-15 11:24:33.080117 quant2-0.1.9/quant/football/data/preprocessing.py
+-rw-r--r--   0        0        0      993 2024-04-17 06:41:14.170874 quant2-0.1.9/quant/football/data/sampler.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:08:36.928001 quant2-0.1.9/quant/football/data/stats.py
+-rw-r--r--   0        0        0     4560 2024-04-13 08:19:58.059662 quant2-0.1.9/quant/football/data/utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 16:55:37.649284 quant2-0.1.9/quant/football/infer/__init__.py
+-rw-r--r--   0        0        0     2024 2024-04-16 01:19:44.599739 quant2-0.1.9/quant/football/infer/fastapi_app.py
+-rw-r--r--   0        0        0      468 2024-04-11 16:55:50.160241 quant2-0.1.9/quant/football/infer/fastapi_app_test.py
+-rw-r--r--   0        0        0     8035 2024-04-19 08:10:26.065510 quant2-0.1.9/quant/football/infer/football_infer_overunder_v1.py
+-rw-r--r--   0        0        0      473 2024-04-11 16:56:07.430215 quant2-0.1.9/quant/football/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 04:22:28.629548 quant2-0.1.9/quant/football/models/mtnet.py
+-rw-r--r--   0        0        0     6110 2024-04-11 17:12:37.365849 quant2-0.1.9/quant/football/models/stnet.py
+-rw-r--r--   0        0        0      547 2024-04-19 12:53:57.861344 quant2-0.1.9/quant/football/transforms/__init__.py
+-rw-r--r--   0        0        0     6622 2024-04-16 00:40:54.525920 quant2-0.1.9/quant/football/transforms/table20240326.py
+-rw-r--r--   0        0        0     8541 2024-04-16 01:19:10.126956 quant2-0.1.9/quant/football/transforms/table20240410.py
+-rw-r--r--   0        0        0     8825 2024-04-16 00:40:14.674251 quant2-0.1.9/quant/football/transforms/table20240414.py
+-rw-r--r--   0        0        0     8396 2024-04-16 02:25:15.544645 quant2-0.1.9/quant/football/transforms/table20240415.py
+-rw-r--r--   0        0        0     8662 2024-04-19 14:38:26.351623 quant2-0.1.9/quant/football/transforms/table20240419.py
+-rw-r--r--   0        0        0        0 2024-03-31 10:26:04.538951 quant2-0.1.9/quant/layers/__init__.py
+-rw-r--r--   0        0        0      483 2024-03-28 09:12:19.609652 quant2-0.1.9/quant/layers/layer_scale.py
+-rw-r--r--   0        0        0     1070 2024-03-28 09:13:06.741829 quant2-0.1.9/quant/layers/mlp.py
+-rw-r--r--   0        0        0     1314 2024-03-28 09:40:33.643889 quant2-0.1.9/quant/layers/normalization.py
+-rw-r--r--   0        0        0      852 2024-03-28 09:16:09.540017 quant2-0.1.9/quant/layers/swiglu_ffn.py
+-rw-r--r--   0        0        0        0 2024-04-03 13:03:10.745509 quant2-0.1.9/quant/utils/__init__.py
+-rw-r--r--   0        0        0     1695 2024-04-11 16:56:25.721657 quant2-0.1.9/quant/utils/archive.py
+-rw-r--r--   0        0        0     1884 2024-04-14 08:14:07.935771 quant2-0.1.9/quant/utils/config.py
+-rw-r--r--   0        0        0     1047 2024-04-09 01:40:57.919653 quant2-0.1.9/quant/utils/io.py
+-rw-r--r--   0        0        0     1006 2024-04-03 13:19:59.255567 quant2-0.1.9/quant/utils/logging.py
+-rw-r--r--   0        0        0      182 2024-03-28 01:09:02.081511 quant2-0.1.9/tests/football/data/test_utils.py
+-rw-r--r--   0        0        0     1632 2024-04-12 06:45:57.389803 quant2-0.1.9/tools/analysis_tools/analyze_cls_results.py
+-rw-r--r--   0        0        0     2645 2024-04-16 01:48:23.763355 quant2-0.1.9/tools/experimental/make_dataset.py
+-rw-r--r--   0        0        0     1580 2024-04-13 14:41:36.176420 quant2-0.1.9/tools/experimental/make_split.py
+-rw-r--r--   0        0        0     8078 2024-04-17 06:34:03.034798 quant2-0.1.9/tools/experimental/nni_football.py
+-rw-r--r--   0        0        0      600 2024-04-17 07:13:13.694051 quant2-0.1.9/tools/experimental/nni_football_config.yaml
+-rw-r--r--   0        0        0     1832 2024-04-17 08:12:07.193491 quant2-0.1.9/tools/experimental/nni_football_config_search_space.json
+-rw-r--r--   0        0        0      523 2024-04-14 02:37:47.884925 quant2-0.1.9/tools/experimental/nni_model.py
+-rw-r--r--   0        0        0      441 2024-04-14 04:00:22.459245 quant2-0.1.9/tools/experimental/nni_model_config.yaml
+-rw-r--r--   0        0        0     2867 2024-04-18 04:24:08.683016 quant2-0.1.9/tools/fb_cls_test.py
+-rw-r--r--   0        0        0     7897 2024-04-17 06:33:07.892275 quant2-0.1.9/tools/fb_cls_train.py
+-rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 quant2-0.1.9/PKG-INFO
```

### Comparing `quant2-0.1.8/.gitignore` & `quant2-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/LICENSE` & `quant2-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/configs/stnetv3/stnetv3_table20240326_2201to2312.cfg` & `quant2-0.1.9/configs/stnetv3/stnetv3_table20240326_2201to2312.cfg`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/configs/stnetv4/stnetv4_table20240410_2201to2312.cfg` & `quant2-0.1.9/configs/stnetv4/stnetv4_table20240410_2201to2312.cfg`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/pyproject.toml` & `quant2-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/README.md` & `quant2-0.1.9/quant/README.md`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/__init__.py` & `quant2-0.1.9/quant/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A collection of useful tools!"""
 import sys
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 help_doc_str = """\
 usage: quant [--version] [--help]
 
 shell command:
     quant -h
```

### Comparing `quant2-0.1.8/quant/evaluate/meters.py` & `quant2-0.1.9/quant/evaluate/meters.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/evaluate/table20240326.py` & `quant2-0.1.9/quant/evaluate/table20240326.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/evaluate/utils.py` & `quant2-0.1.9/quant/evaluate/utils.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/football/data/dataset.py` & `quant2-0.1.9/quant/football/data/dataset.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/football/data/preprocessing.py` & `quant2-0.1.9/quant/football/data/preprocessing.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/football/data/sampler.py` & `quant2-0.1.9/quant/football/data/sampler.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/football/data/utils.py` & `quant2-0.1.9/quant/football/data/utils.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/football/infer/fastapi_app.py` & `quant2-0.1.9/quant/football/infer/fastapi_app.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/football/infer/football_infer_overunder_v1.py` & `quant2-0.1.9/quant/football/infer/football_infer_overunder_v1.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/football/models/stnet.py` & `quant2-0.1.9/quant/football/models/stnet.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/football/transforms/__init__.py` & `quant2-0.1.9/quant/football/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/football/transforms/table20240326.py` & `quant2-0.1.9/quant/football/transforms/table20240326.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/football/transforms/table20240410.py` & `quant2-0.1.9/quant/football/transforms/table20240410.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/football/transforms/table20240414.py` & `quant2-0.1.9/quant/football/transforms/table20240414.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/football/transforms/table20240415.py` & `quant2-0.1.9/quant/football/transforms/table20240415.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/football/transforms/table20240419.py` & `quant2-0.1.9/quant/football/transforms/table20240419.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         if _season not in encoder["season"] or _home not in encoder["team"] or _away not in encoder["team"]:
             continue
 
         _remaining_time = int((90 if whole else 45) - _time)
         a, b = divmod(_remaining_time - 1, 10)
 
         # 剩余时间必须小于40分钟
-        _time_codes = np.zeros(5, dtype=int)
+        _time_codes = [0, 0, 0, 0, 0]
         _time_codes[a], _time_codes[-1] = 1, b + 1
 
         # 进球,换人,黄牌,红牌,乌龙,点球,射失点球,两黄变红,视频裁判
         _home_score = sum([_vals[i] for i in [0, 4, 5]])
         _away_score = sum([_vals[cycle_size + i] for i in [0, 4, 5]])
         _curr_score = [_home_score + _away_score, _home_score, _away_score]
```

### Comparing `quant2-0.1.8/quant/layers/mlp.py` & `quant2-0.1.9/quant/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/layers/normalization.py` & `quant2-0.1.9/quant/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/layers/swiglu_ffn.py` & `quant2-0.1.9/quant/layers/swiglu_ffn.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/utils/archive.py` & `quant2-0.1.9/quant/utils/archive.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/utils/config.py` & `quant2-0.1.9/quant/utils/config.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/utils/io.py` & `quant2-0.1.9/quant/utils/io.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/quant/utils/logging.py` & `quant2-0.1.9/quant/utils/logging.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/tools/analysis_tools/analyze_cls_results.py` & `quant2-0.1.9/tools/analysis_tools/analyze_cls_results.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/tools/experimental/make_dataset.py` & `quant2-0.1.9/tools/experimental/make_dataset.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/tools/experimental/make_split.py` & `quant2-0.1.9/tools/experimental/make_split.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/tools/experimental/nni_football.py` & `quant2-0.1.9/tools/experimental/nni_football.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/tools/experimental/nni_football_config.yaml` & `quant2-0.1.9/tools/experimental/nni_football_config.yaml`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/tools/experimental/nni_football_config_search_space.json` & `quant2-0.1.9/tools/experimental/nni_football_config_search_space.json`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/tools/experimental/nni_model.py` & `quant2-0.1.9/tools/experimental/nni_model.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/tools/fb_cls_test.py` & `quant2-0.1.9/tools/fb_cls_test.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/tools/fb_cls_train.py` & `quant2-0.1.9/tools/fb_cls_train.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.8/PKG-INFO` & `quant2-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant2
-Version: 0.1.8
+Version: 0.1.9
 Summary: A collection of useful tools!
 Author-email: Hejian <flystarhe@qq.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: prettytable
 Requires-Dist: scikit-learn
```

