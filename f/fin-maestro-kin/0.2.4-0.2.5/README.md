# Comparing `tmp/fin_maestro_kin-0.2.4.tar.gz` & `tmp/fin_maestro_kin-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fin_maestro_kin-0.2.4.tar", max compression
+gzip compressed data, was "fin_maestro_kin-0.2.5.tar", max compression
```

## Comparing `fin_maestro_kin-0.2.4.tar` & `fin_maestro_kin-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,35 @@
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.4/fin_maestro_kin/__init__.py
--rw-r--r--   0        0        0     1606 2024-04-13 06:37:31.640875 fin_maestro_kin-0.2.4/fin_maestro_kin/constants.py
--rw-r--r--   0        0        0     1025 2024-04-15 18:30:00.477406 fin_maestro_kin-0.2.4/fin_maestro_kin/main.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/__init__.py
--rw-r--r--   0        0        0       18 2024-03-31 06:15:52.175723 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/nse/__init__.py
--rw-r--r--   0        0        0    12705 2024-04-15 18:39:19.947514 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/nse/helper.py
--rw-r--r--   0        0        0    19042 2024-04-15 18:33:45.624559 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/nse/nse_equities.py
--rw-r--r--   0        0        0     7634 2024-04-07 13:52:15.430589 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/nse/nse_indices.py
--rw-r--r--   0        0        0        0 2024-04-13 06:37:31.671927 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/screener/__init__.py
--rw-r--r--   0        0        0      514 2024-04-13 06:37:31.671927 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/screener/helper.py
--rw-r--r--   0        0        0     1865 2024-04-13 06:37:31.687590 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/screener/screener_equities.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/sentiment_analysis/__init__.py
--rw-r--r--   0        0        0     1563 2024-02-10 16:25:56.398293 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/sentiment_analysis/pcr_data.py
--rw-r--r--   0        0        0     2109 2024-02-25 06:17:29.811861 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/sentiment_analysis/sentiment_analysis.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.413185 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/trend_detector/__init__.py
--rw-r--r--   0        0        0     2074 2024-02-25 06:17:29.827487 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/trend_detector/trend_detector.py
--rw-r--r--   0        0        0     1090 2024-02-10 16:19:33.663653 fin_maestro_kin-0.2.4/LICENSE
--rw-r--r--   0        0        0      642 2024-04-15 18:48:30.804605 fin_maestro_kin-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     5347 2024-04-15 16:54:12.969094 fin_maestro_kin-0.2.4/README.md
--rw-r--r--   0        0        0     6235 1970-01-01 00:00:00.000000 fin_maestro_kin-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.5/fin_maestro_kin/__init__.py
+-rw-r--r--   0        0        0     1872 2024-04-20 19:23:53.441398 fin_maestro_kin-0.2.5/fin_maestro_kin/constants.py
+-rw-r--r--   0        0        0     1025 2024-04-15 18:30:00.477406 fin_maestro_kin-0.2.5/fin_maestro_kin/main.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/__init__.py
+-rw-r--r--   0        0        0      170 2024-03-23 08:46:49.868081 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0       18 2024-03-31 06:15:52.175723 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/__init__.py
+-rw-r--r--   0        0        0      203 2024-03-31 06:41:27.749444 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/nse/__init__.py
+-rw-r--r--   0        0        0      187 2024-03-23 08:47:13.994885 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/nse/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9115 2024-04-15 18:39:26.059998 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/nse/__pycache__/helper.cpython-39.pyc
+-rw-r--r--   0        0        0    13150 2024-04-15 18:33:51.983822 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/nse/__pycache__/nse_equities.cpython-39.pyc
+-rw-r--r--   0        0        0     5973 2024-04-07 13:52:21.935537 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/nse/__pycache__/nse_indices.cpython-39.pyc
+-rw-r--r--   0        0        0    12705 2024-04-15 18:39:19.947514 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/nse/helper.py
+-rw-r--r--   0        0        0    19042 2024-04-15 18:33:45.624559 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/nse/nse_equities.py
+-rw-r--r--   0        0        0     7634 2024-04-07 13:52:15.430589 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/nse/nse_indices.py
+-rw-r--r--   0        0        0        0 2024-04-13 06:37:31.671927 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/screener/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-15 16:55:29.743148 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/screener/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3011 2024-04-19 20:03:28.320060 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/screener/__pycache__/helper.cpython-39.pyc
+-rw-r--r--   0        0        0     8493 2024-04-19 20:04:53.435533 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/screener/__pycache__/screener_equities.cpython-39.pyc
+-rw-r--r--   0        0        0     3209 2024-04-20 19:23:53.441398 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/screener/helper.py
+-rw-r--r--   0        0        0    11704 2024-04-20 19:23:53.441398 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/screener/screener_equities.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/sentiment_analysis/__init__.py
+-rw-r--r--   0        0        0      189 2024-03-17 10:59:01.312818 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/sentiment_analysis/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1358 2024-03-17 10:59:01.500759 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/sentiment_analysis/__pycache__/pcr_data.cpython-39.pyc
+-rw-r--r--   0        0        0     2131 2024-03-17 10:59:01.344089 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/sentiment_analysis/__pycache__/sentiment_analysis.cpython-39.pyc
+-rw-r--r--   0        0        0     1563 2024-02-10 16:25:56.398293 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/sentiment_analysis/pcr_data.py
+-rw-r--r--   0        0        0     2109 2024-02-25 06:17:29.811861 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/sentiment_analysis/sentiment_analysis.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.413185 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/trend_detector/__init__.py
+-rw-r--r--   0        0        0      185 2024-03-17 10:59:10.299081 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/trend_detector/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2006 2024-03-17 10:59:10.346263 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/trend_detector/__pycache__/trend_detector.cpython-39.pyc
+-rw-r--r--   0        0        0     2074 2024-02-25 06:17:29.827487 fin_maestro_kin-0.2.5/fin_maestro_kin/modules/trend_detector/trend_detector.py
+-rw-r--r--   0        0        0     1090 2024-02-10 16:19:33.663653 fin_maestro_kin-0.2.5/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-20 19:24:48.839169 fin_maestro_kin-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     5347 2024-04-15 16:54:12.969094 fin_maestro_kin-0.2.5/README.md
+-rw-r--r--   0        0        0     6235 1970-01-01 00:00:00.000000 fin_maestro_kin-0.2.5/PKG-INFO
```

### Comparing `fin_maestro_kin-0.2.4/fin_maestro_kin/constants.py` & `fin_maestro_kin-0.2.5/fin_maestro_kin/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,9 +19,14 @@
     '/nseindices/returns?symbol=NIFTY 50&start_date=10-Jan-2024&end_date=12-Jan-2024',
     '/nseindices/indice-pcr?symbol=NIFTY',
     '/nseindices/india-vix?start_date=28-01-2024&end_date=01-02-2024',
     '/nseindices/index-symbols',
     '/sentiment/pcr-indice-analysis',
     '/sentiment/pcr-stocks-analysis?symbol=INFY',
     '/generate_plot?ticker=BSE.NS',
-    '/screener-equities/quarterly-result?symbol=vedl'
+    '/screener-equities/quarterly-result?symbol=vedl',
+    '/screener-equities/shareholding-pattern?symbol=vedl',
+    '/screener-equities/cash-flow?symbol=vedl',
+    '/screener-equities/balance-sheet?symbol=vedl',
+    '/screener-equities/annual-profit-loss?symbol=vedl',
+    '/screener-equities/ratios?symbol=vedl'
 ]
```

### Comparing `fin_maestro_kin-0.2.4/fin_maestro_kin/main.py` & `fin_maestro_kin-0.2.5/fin_maestro_kin/main.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/nse/helper.py` & `fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/nse/helper.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/nse/nse_equities.py` & `fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/nse/nse_equities.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/nse/nse_indices.py` & `fin_maestro_kin-0.2.5/fin_maestro_kin/modules/data_toolkit/nse/nse_indices.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.4/fin_maestro_kin/modules/sentiment_analysis/pcr_data.py` & `fin_maestro_kin-0.2.5/fin_maestro_kin/modules/sentiment_analysis/pcr_data.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.4/fin_maestro_kin/modules/sentiment_analysis/sentiment_analysis.py` & `fin_maestro_kin-0.2.5/fin_maestro_kin/modules/sentiment_analysis/sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.4/fin_maestro_kin/modules/trend_detector/trend_detector.py` & `fin_maestro_kin-0.2.5/fin_maestro_kin/modules/trend_detector/trend_detector.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.4/LICENSE` & `fin_maestro_kin-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.4/pyproject.toml` & `fin_maestro_kin-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fin-maestro-kin"
-version = "0.2.4"
+version = "0.2.5"
 description = "Where Data Meets FastAPI Brilliance with Fin-Maestro-Kin – Your All-in-One Finance API."
 authors = ["DEV_FINWIZ <devjuneja43@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `fin_maestro_kin-0.2.4/README.md` & `fin_maestro_kin-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.4/PKG-INFO` & `fin_maestro_kin-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fin-maestro-kin
-Version: 0.2.4
+Version: 0.2.5
 Summary: Where Data Meets FastAPI Brilliance with Fin-Maestro-Kin – Your All-in-One Finance API.
 License: MIT
 Author: DEV_FINWIZ
 Author-email: devjuneja43@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fin-maestro-kin Version: 0.2.4 Summary: Where Data
+Metadata-Version: 2.1 Name: fin-maestro-kin Version: 0.2.5 Summary: Where Data
 Meets FastAPI Brilliance with Fin-Maestro-Kin â Your All-in-One Finance API.
 License: MIT Author: DEV_FINWIZ Author-email: devjuneja43@gmail.com Requires-
 Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
```

