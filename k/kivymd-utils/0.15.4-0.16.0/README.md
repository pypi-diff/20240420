# Comparing `tmp/kivymd_utils-0.15.4.tar.gz` & `tmp/kivymd_utils-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kivymd_utils-0.15.4.tar", max compression
+gzip compressed data, was "kivymd_utils-0.16.0.tar", max compression
```

## Comparing `kivymd_utils-0.15.4.tar` & `kivymd_utils-0.16.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1068 2024-04-14 14:59:12.472183 kivymd_utils-0.15.4/LICENSE
--rw-r--r--   0        0        0    10957 2024-04-16 12:45:32.005000 kivymd_utils-0.15.4/README.md
--rw-r--r--   0        0        0       87 2024-04-08 13:05:21.394440 kivymd_utils-0.15.4/kivymd_utils/coroutine/__init__.py
--rw-r--r--   0        0        0     1614 2024-04-08 13:05:01.503980 kivymd_utils-0.15.4/kivymd_utils/coroutine/coroutineBuilder.py
--rw-r--r--   0        0        0      126 2024-04-08 13:04:51.743754 kivymd_utils-0.15.4/kivymd_utils/redrawAble/__init__.py
--rw-r--r--   0        0        0      272 2024-04-03 14:19:25.831870 kivymd_utils-0.15.4/kivymd_utils/redrawAble/notifyListeners.py
--rw-r--r--   0        0        0     1058 2024-04-08 13:04:48.060336 kivymd_utils-0.15.4/kivymd_utils/redrawAble/redrawAble.py
--rw-r--r--   0        0        0      164 2024-04-08 13:05:29.157953 kivymd_utils-0.15.4/kivymd_utils/router/__init__.py
--rw-r--r--   0        0        0      561 2024-04-04 09:48:59.355519 kivymd_utils-0.15.4/kivymd_utils/router/error_page.py
--rw-r--r--   0        0        0      569 2024-04-03 16:56:34.050126 kivymd_utils-0.15.4/kivymd_utils/router/path_utils.py
--rw-r--r--   0        0        0     4018 2024-04-16 11:38:02.610055 kivymd_utils-0.15.4/kivymd_utils/router/route.py
--rw-r--r--   0        0        0     4464 2024-04-16 12:20:36.238248 kivymd_utils-0.15.4/kivymd_utils/router/router.py
--rw-r--r--   0        0        0     1683 2024-04-08 13:05:46.818364 kivymd_utils-0.15.4/kivymd_utils/router/state.py
--rw-r--r--   0        0        0      327 2024-04-16 12:45:39.081699 kivymd_utils-0.15.4/pyproject.toml
--rw-r--r--   0        0        0    11417 1970-01-01 00:00:00.000000 kivymd_utils-0.15.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-14 14:59:12.472183 kivymd_utils-0.16.0/LICENSE
+-rw-r--r--   0        0        0    10957 2024-04-16 12:45:32.005000 kivymd_utils-0.16.0/README.md
+-rw-r--r--   0        0        0     8123 2024-04-20 11:54:05.625593 kivymd_utils-0.16.0/kivymd_utils/colors/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-08 13:05:21.394440 kivymd_utils-0.16.0/kivymd_utils/coroutine/__init__.py
+-rw-r--r--   0        0        0     1614 2024-04-08 13:05:01.503980 kivymd_utils-0.16.0/kivymd_utils/coroutine/coroutineBuilder.py
+-rw-r--r--   0        0        0      126 2024-04-08 13:04:51.743754 kivymd_utils-0.16.0/kivymd_utils/redrawAble/__init__.py
+-rw-r--r--   0        0        0      272 2024-04-03 14:19:25.831870 kivymd_utils-0.16.0/kivymd_utils/redrawAble/notifyListeners.py
+-rw-r--r--   0        0        0     1058 2024-04-08 13:04:48.060336 kivymd_utils-0.16.0/kivymd_utils/redrawAble/redrawAble.py
+-rw-r--r--   0        0        0      164 2024-04-08 13:05:29.157953 kivymd_utils-0.16.0/kivymd_utils/router/__init__.py
+-rw-r--r--   0        0        0      561 2024-04-04 09:48:59.355519 kivymd_utils-0.16.0/kivymd_utils/router/error_page.py
+-rw-r--r--   0        0        0      569 2024-04-03 16:56:34.050126 kivymd_utils-0.16.0/kivymd_utils/router/path_utils.py
+-rw-r--r--   0        0        0     4018 2024-04-16 11:38:02.610055 kivymd_utils-0.16.0/kivymd_utils/router/route.py
+-rw-r--r--   0        0        0     4464 2024-04-16 12:20:36.238248 kivymd_utils-0.16.0/kivymd_utils/router/router.py
+-rw-r--r--   0        0        0     1683 2024-04-08 13:05:46.818364 kivymd_utils-0.16.0/kivymd_utils/router/state.py
+-rw-r--r--   0        0        0      327 2024-04-20 11:54:12.598813 kivymd_utils-0.16.0/pyproject.toml
+-rw-r--r--   0        0        0    11417 1970-01-01 00:00:00.000000 kivymd_utils-0.16.0/PKG-INFO
```

### Comparing `kivymd_utils-0.15.4/LICENSE` & `kivymd_utils-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.15.4/README.md` & `kivymd_utils-0.16.0/README.md`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.15.4/kivymd_utils/coroutine/coroutineBuilder.py` & `kivymd_utils-0.16.0/kivymd_utils/coroutine/coroutineBuilder.py`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.15.4/kivymd_utils/redrawAble/redrawAble.py` & `kivymd_utils-0.16.0/kivymd_utils/redrawAble/redrawAble.py`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.15.4/kivymd_utils/router/error_page.py` & `kivymd_utils-0.16.0/kivymd_utils/router/error_page.py`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.15.4/kivymd_utils/router/path_utils.py` & `kivymd_utils-0.16.0/kivymd_utils/router/path_utils.py`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.15.4/kivymd_utils/router/route.py` & `kivymd_utils-0.16.0/kivymd_utils/router/route.py`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.15.4/kivymd_utils/router/router.py` & `kivymd_utils-0.16.0/kivymd_utils/router/router.py`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.15.4/kivymd_utils/router/state.py` & `kivymd_utils-0.16.0/kivymd_utils/router/state.py`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.15.4/PKG-INFO` & `kivymd_utils-0.16.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivymd-utils
-Version: 0.15.4
+Version: 0.16.0
 Summary: 
 Author: MilanR
 Author-email: milan.rombouts23@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

