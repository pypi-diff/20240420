# Comparing `tmp/deshima_rawdata-2024.4.0.tar.gz` & `tmp/deshima_rawdata-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deshima_rawdata-2024.4.0.tar", max compression
+gzip compressed data, was "deshima_rawdata-2024.4.1.tar", max compression
```

## Comparing `deshima_rawdata-2024.4.0.tar` & `deshima_rawdata-2024.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2024-04-20 15:51:38.456840 deshima_rawdata-2024.4.0/LICENSE
--rw-r--r--   0        0        0     1759 2024-04-20 15:51:38.456840 deshima_rawdata-2024.4.0/README.md
--rw-r--r--   0        0        0      138 2024-04-20 15:51:39.152848 deshima_rawdata-2024.4.0/deshima_rawdata/__init__.py
--rw-r--r--   0        0        0     2822 2024-04-20 15:51:39.152848 deshima_rawdata-2024.4.0/deshima_rawdata/cli.py
--rw-r--r--   0        0        0      289 2024-04-20 15:51:39.152848 deshima_rawdata-2024.4.0/deshima_rawdata/data.csv
--rw-r--r--   0        0        0        0 2024-04-20 15:51:39.152848 deshima_rawdata-2024.4.0/deshima_rawdata/py.typed
--rw-r--r--   0        0        0      728 2024-04-20 15:51:39.152848 deshima_rawdata-2024.4.0/pyproject.toml
--rw-r--r--   0        0        0     2524 1970-01-01 00:00:00.000000 deshima_rawdata-2024.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-20 16:18:34.800494 deshima_rawdata-2024.4.1/LICENSE
+-rw-r--r--   0        0        0     1759 2024-04-20 16:18:34.800494 deshima_rawdata-2024.4.1/README.md
+-rw-r--r--   0        0        0      138 2024-04-20 16:18:35.644500 deshima_rawdata-2024.4.1/deshima_rawdata/__init__.py
+-rw-r--r--   0        0        0     2822 2024-04-20 16:18:35.644500 deshima_rawdata-2024.4.1/deshima_rawdata/cli.py
+-rw-r--r--   0        0        0      347 2024-04-20 16:18:35.644500 deshima_rawdata-2024.4.1/deshima_rawdata/data.csv
+-rw-r--r--   0        0        0        0 2024-04-20 16:18:35.644500 deshima_rawdata-2024.4.1/deshima_rawdata/py.typed
+-rw-r--r--   0        0        0      728 2024-04-20 16:18:35.644500 deshima_rawdata-2024.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2524 1970-01-01 00:00:00.000000 deshima_rawdata-2024.4.1/PKG-INFO
```

### Comparing `deshima_rawdata-2024.4.0/LICENSE` & `deshima_rawdata-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deshima_rawdata-2024.4.0/README.md` & `deshima_rawdata-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `deshima_rawdata-2024.4.0/deshima_rawdata/cli.py` & `deshima_rawdata-2024.4.1/deshima_rawdata/cli.py`

 * *Files identical despite different names*

### Comparing `deshima_rawdata-2024.4.0/pyproject.toml` & `deshima_rawdata-2024.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deshima-rawdata"
-version = "2024.4.0"
+version = "2024.4.1"
 description = "DESHIMA raw data and downloader package"
 authors = ["Akio Taniguchi <taniguchi@a.phys.nagoya-u.ac.jp>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.13"
```

### Comparing `deshima_rawdata-2024.4.0/PKG-INFO` & `deshima_rawdata-2024.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deshima-rawdata
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: DESHIMA raw data and downloader package
 License: MIT
 Author: Akio Taniguchi
 Author-email: taniguchi@a.phys.nagoya-u.ac.jp
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

