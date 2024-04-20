# Comparing `tmp/xrpl_helpers-1.0.5.tar.gz` & `tmp/xrpl_helpers-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrpl_helpers-1.0.5.tar", max compression
+gzip compressed data, was "xrpl_helpers-1.0.6.tar", max compression
```

## Comparing `xrpl_helpers-1.0.5.tar` & `xrpl_helpers-1.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      628 2024-04-20 10:02:39.984801 xrpl_helpers-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1476 2023-10-27 08:21:46.912203 xrpl_helpers-1.0.5/xrpl_helpers/common/utils.py
--rw-r--r--   0        0        0     1373 2023-11-17 00:11:02.249989 xrpl_helpers-1.0.5/xrpl_helpers/genesis.ripple.json
--rw-r--r--   0        0        0    30234 2023-11-17 00:11:02.265722 xrpl_helpers-1.0.5/xrpl_helpers/genesis.xahau.json
--rw-r--r--   0        0        0     1839 2023-06-25 06:00:12.875396 xrpl_helpers-1.0.5/xrpl_helpers/libs/google/storage.py
--rw-r--r--   0        0        0     3228 2023-11-23 11:44:19.954389 xrpl_helpers-1.0.5/xrpl_helpers/rippled/utils.py
--rw-r--r--   0        0        0     1889 2023-06-25 06:00:12.875796 xrpl_helpers-1.0.5/xrpl_helpers/sdk/hooks.py
--rw-r--r--   0        0        0     2084 2023-06-25 06:00:12.875871 xrpl_helpers-1.0.5/xrpl_helpers/sdk/utils.py
--rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 xrpl_helpers-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      628 2024-04-20 10:03:03.410575 xrpl_helpers-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1476 2023-10-27 08:21:46.912203 xrpl_helpers-1.0.6/xrpl_helpers/common/utils.py
+-rw-r--r--   0        0        0    30234 2023-11-17 00:11:02.265722 xrpl_helpers-1.0.6/xrpl_helpers/genesis.xahau.json
+-rw-r--r--   0        0        0     1373 2023-11-17 00:11:02.249989 xrpl_helpers-1.0.6/xrpl_helpers/genesis.xrpl.json
+-rw-r--r--   0        0        0     1839 2023-06-25 06:00:12.875396 xrpl_helpers-1.0.6/xrpl_helpers/libs/google/storage.py
+-rw-r--r--   0        0        0     3228 2023-11-23 11:44:19.954389 xrpl_helpers-1.0.6/xrpl_helpers/rippled/utils.py
+-rw-r--r--   0        0        0     1889 2023-06-25 06:00:12.875796 xrpl_helpers-1.0.6/xrpl_helpers/sdk/hooks.py
+-rw-r--r--   0        0        0     2084 2023-06-25 06:00:12.875871 xrpl_helpers-1.0.6/xrpl_helpers/sdk/utils.py
+-rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 xrpl_helpers-1.0.6/PKG-INFO
```

### Comparing `xrpl_helpers-1.0.5/pyproject.toml` & `xrpl_helpers-1.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xrpl-helpers"
-version = "1.0.5"
+version = "1.0.6"
 description = ""
 authors = ["Denis Angell <dangell@transia.co>"]
 
 [tool.poetry.dependencies]
 python = "^3.9.6"
 pytest = "^7.2.1"
 PyYAML = "^6.0"
```

### Comparing `xrpl_helpers-1.0.5/xrpl_helpers/common/utils.py` & `xrpl_helpers-1.0.6/xrpl_helpers/common/utils.py`

 * *Files identical despite different names*

### Comparing `xrpl_helpers-1.0.5/xrpl_helpers/genesis.ripple.json` & `xrpl_helpers-1.0.6/xrpl_helpers/genesis.xrpl.json`

 * *Files identical despite different names*

### Comparing `xrpl_helpers-1.0.5/xrpl_helpers/genesis.xahau.json` & `xrpl_helpers-1.0.6/xrpl_helpers/genesis.xahau.json`

 * *Files identical despite different names*

### Comparing `xrpl_helpers-1.0.5/xrpl_helpers/libs/google/storage.py` & `xrpl_helpers-1.0.6/xrpl_helpers/libs/google/storage.py`

 * *Files identical despite different names*

### Comparing `xrpl_helpers-1.0.5/xrpl_helpers/rippled/utils.py` & `xrpl_helpers-1.0.6/xrpl_helpers/rippled/utils.py`

 * *Files identical despite different names*

### Comparing `xrpl_helpers-1.0.5/xrpl_helpers/sdk/hooks.py` & `xrpl_helpers-1.0.6/xrpl_helpers/sdk/hooks.py`

 * *Files identical despite different names*

### Comparing `xrpl_helpers-1.0.5/xrpl_helpers/sdk/utils.py` & `xrpl_helpers-1.0.6/xrpl_helpers/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `xrpl_helpers-1.0.5/PKG-INFO` & `xrpl_helpers-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrpl-helpers
-Version: 1.0.5
+Version: 1.0.6
 Summary: 
 Author: Denis Angell
 Author-email: dangell@transia.co
 Requires-Python: >=3.9.6,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

