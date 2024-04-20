# Comparing `tmp/stockdex-0.3.8.tar.gz` & `tmp/stockdex-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stockdex-0.3.8.tar", last modified: Sun Apr  7 10:34:36 2024, max compression
+gzip compressed data, was "stockdex-0.3.9.tar", last modified: Sun Apr  7 10:40:05 2024, max compression
```

## Comparing `stockdex-0.3.8.tar` & `stockdex-0.3.9.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:34:36.577845 stockdex-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-07 10:34:36.577845 stockdex-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-07 10:34:28.000000 stockdex-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 10:34:36.577845 stockdex-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-07 10:34:28.000000 stockdex-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:34:36.577845 stockdex-0.3.8/stockdex/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14539 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/justetf.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/nasdaq_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/selenium_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    15771 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/ticker.py
--rw-r--r--   0 runner    (1001) docker     (127)    11315 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/ticker_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/ticker_base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/ticker_etf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:34:36.577845 stockdex-0.3.8/stockdex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-07 10:34:36.000000 stockdex-0.3.8/stockdex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-07 10:34:36.000000 stockdex-0.3.8/stockdex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 10:34:36.000000 stockdex-0.3.8/stockdex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-07 10:34:36.000000 stockdex-0.3.8/stockdex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 10:34:36.000000 stockdex-0.3.8/stockdex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:34:36.577845 stockdex-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:34:28.000000 stockdex-0.3.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-07 10:34:28.000000 stockdex-0.3.8/tests/test_justetf.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-07 10:34:28.000000 stockdex-0.3.8/tests/test_nasdaq_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-07 10:34:28.000000 stockdex-0.3.8/tests/test_ticker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-07 10:34:28.000000 stockdex-0.3.8/tests/test_ticker_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:40:05.350794 stockdex-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-07 10:40:05.350794 stockdex-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-07 10:39:54.000000 stockdex-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 10:40:05.350794 stockdex-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-07 10:39:54.000000 stockdex-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:40:05.330794 stockdex-0.3.9/stockdex/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-07 10:39:54.000000 stockdex-0.3.9/stockdex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:40:05.330794 stockdex-0.3.9/stockdex/chromedriver_linux64/
+-rw-r--r--   0 runner    (1001) docker     (127)   326542 2024-04-07 10:39:54.000000 stockdex-0.3.9/stockdex/chromedriver_linux64/LICENSE.chromedriver
+-rwxr-xr-x   0 runner    (1001) docker     (127) 15039112 2024-04-07 10:39:54.000000 stockdex-0.3.9/stockdex/chromedriver_linux64/chromedriver
+-rw-r--r--   0 runner    (1001) docker     (127)    14539 2024-04-07 10:39:54.000000 stockdex-0.3.9/stockdex/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-07 10:39:54.000000 stockdex-0.3.9/stockdex/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-04-07 10:39:54.000000 stockdex-0.3.9/stockdex/justetf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-07 10:39:54.000000 stockdex-0.3.9/stockdex/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-07 10:39:54.000000 stockdex-0.3.9/stockdex/nasdaq_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-07 10:39:54.000000 stockdex-0.3.9/stockdex/selenium_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15771 2024-04-07 10:39:54.000000 stockdex-0.3.9/stockdex/ticker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11315 2024-04-07 10:39:54.000000 stockdex-0.3.9/stockdex/ticker_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-07 10:39:54.000000 stockdex-0.3.9/stockdex/ticker_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:39:54.000000 stockdex-0.3.9/stockdex/ticker_etf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:40:05.330794 stockdex-0.3.9/stockdex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-07 10:40:05.000000 stockdex-0.3.9/stockdex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-07 10:40:05.000000 stockdex-0.3.9/stockdex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 10:40:05.000000 stockdex-0.3.9/stockdex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-07 10:40:05.000000 stockdex-0.3.9/stockdex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 10:40:05.000000 stockdex-0.3.9/stockdex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:40:05.350794 stockdex-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:39:54.000000 stockdex-0.3.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-07 10:39:54.000000 stockdex-0.3.9/tests/test_justetf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-07 10:39:54.000000 stockdex-0.3.9/tests/test_nasdaq_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-07 10:39:54.000000 stockdex-0.3.9/tests/test_ticker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-07 10:39:54.000000 stockdex-0.3.9/tests/test_ticker_api.py
```

### Comparing `stockdex-0.3.8/PKG-INFO` & `stockdex-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockdex
-Version: 0.3.8
+Version: 0.3.9
 Summary: A package to get stock data from Yahoo Finance
 Home-page: https://github.com/ahnazary/stockdex
 Author: Amir Nazary
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `stockdex-0.3.8/README.md` & `stockdex-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.8/setup.py` & `stockdex-0.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,9 +13,9 @@
     long_description_content_type="text/markdown",
     url="https://github.com/ahnazary/stockdex",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    package_data={"stockdex": ["chromedriver_linux64"]},
+    package_data={"stockdex": ["chromedriver_linux64/*"]},
 )
```

### Comparing `stockdex-0.3.8/stockdex/config.py` & `stockdex-0.3.9/stockdex/config.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.8/stockdex/justetf.py` & `stockdex-0.3.9/stockdex/justetf.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.8/stockdex/lib.py` & `stockdex-0.3.9/stockdex/lib.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.8/stockdex/nasdaq_interface.py` & `stockdex-0.3.9/stockdex/nasdaq_interface.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.8/stockdex/selenium_interface.py` & `stockdex-0.3.9/stockdex/selenium_interface.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.8/stockdex/ticker.py` & `stockdex-0.3.9/stockdex/ticker.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.8/stockdex/ticker_api.py` & `stockdex-0.3.9/stockdex/ticker_api.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.8/stockdex/ticker_base.py` & `stockdex-0.3.9/stockdex/ticker_base.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.8/stockdex.egg-info/PKG-INFO` & `stockdex-0.3.9/stockdex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockdex
-Version: 0.3.8
+Version: 0.3.9
 Summary: A package to get stock data from Yahoo Finance
 Home-page: https://github.com/ahnazary/stockdex
 Author: Amir Nazary
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `stockdex-0.3.8/stockdex.egg-info/SOURCES.txt` & `stockdex-0.3.9/stockdex.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,12 +12,14 @@
 stockdex/ticker_base.py
 stockdex/ticker_etf.py
 stockdex.egg-info/PKG-INFO
 stockdex.egg-info/SOURCES.txt
 stockdex.egg-info/dependency_links.txt
 stockdex.egg-info/requires.txt
 stockdex.egg-info/top_level.txt
+stockdex/chromedriver_linux64/LICENSE.chromedriver
+stockdex/chromedriver_linux64/chromedriver
 tests/__init__.py
 tests/test_justetf.py
 tests/test_nasdaq_interface.py
 tests/test_ticker.py
 tests/test_ticker_api.py
```

### Comparing `stockdex-0.3.8/tests/test_justetf.py` & `stockdex-0.3.9/tests/test_justetf.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.8/tests/test_nasdaq_interface.py` & `stockdex-0.3.9/tests/test_nasdaq_interface.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.8/tests/test_ticker.py` & `stockdex-0.3.9/tests/test_ticker.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.8/tests/test_ticker_api.py` & `stockdex-0.3.9/tests/test_ticker_api.py`

 * *Files identical despite different names*

