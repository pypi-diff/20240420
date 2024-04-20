# Comparing `tmp/astabc-0.1.4.tar.gz` & `tmp/astabc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astabc-0.1.4.tar", last modified: Fri Apr 12 08:09:03 2024, max compression
+gzip compressed data, was "astabc-0.1.5.tar", last modified: Sat Apr 20 11:11:37 2024, max compression
```

## Comparing `astabc-0.1.4.tar` & `astabc-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-12 08:09:03.472099 astabc-0.1.4/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-04-12 07:46:41.000000 astabc-0.1.4/LICENSE
--rw-r--r--   0 jgi       (1000) jgi       (1000)     1149 2024-04-12 08:09:03.472099 astabc-0.1.4/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      701 2024-04-12 07:32:42.000000 astabc-0.1.4/README.md
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-12 08:09:03.472099 astabc-0.1.4/astabc/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       58 2024-04-12 07:32:31.000000 astabc-0.1.4/astabc/__init__.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2283 2024-04-12 08:08:39.000000 astabc-0.1.4/astabc/astabc.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-12 08:09:03.472099 astabc-0.1.4/astabc.egg-info/
--rw-r--r--   0 jgi       (1000) jgi       (1000)     1149 2024-04-12 08:09:03.000000 astabc-0.1.4/astabc.egg-info/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      265 2024-04-12 08:09:03.000000 astabc-0.1.4/astabc.egg-info/SOURCES.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-04-12 08:09:03.000000 astabc-0.1.4/astabc.egg-info/dependency_links.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       46 2024-04-12 08:09:03.000000 astabc-0.1.4/astabc.egg-info/entry_points.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       14 2024-04-12 08:09:03.000000 astabc-0.1.4/astabc.egg-info/requires.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        7 2024-04-12 08:09:03.000000 astabc-0.1.4/astabc.egg-info/top_level.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       38 2024-04-12 08:09:03.472099 astabc-0.1.4/setup.cfg
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      729 2024-04-12 08:09:01.000000 astabc-0.1.4/setup.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-12 08:09:03.472099 astabc-0.1.4/tests/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1313 2024-04-12 07:32:38.000000 astabc-0.1.4/tests/test_astabc.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-20 11:11:37.152974 astabc-0.1.5/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-04-12 07:46:41.000000 astabc-0.1.5/LICENSE
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1120 2024-04-20 11:11:37.152974 astabc-0.1.5/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      701 2024-04-12 07:32:42.000000 astabc-0.1.5/README.md
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-20 11:11:37.152974 astabc-0.1.5/astabc/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       58 2024-04-12 07:32:31.000000 astabc-0.1.5/astabc/__init__.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2283 2024-04-12 08:08:39.000000 astabc-0.1.5/astabc/astabc.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-20 11:11:37.152974 astabc-0.1.5/astabc.egg-info/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1120 2024-04-20 11:11:36.000000 astabc-0.1.5/astabc.egg-info/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      265 2024-04-20 11:11:37.000000 astabc-0.1.5/astabc.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-04-20 11:11:36.000000 astabc-0.1.5/astabc.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       71 2024-04-20 11:11:36.000000 astabc-0.1.5/astabc.egg-info/entry_points.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       14 2024-04-20 11:11:36.000000 astabc-0.1.5/astabc.egg-info/requires.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        7 2024-04-20 11:11:36.000000 astabc-0.1.5/astabc.egg-info/top_level.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       38 2024-04-20 11:11:37.152974 astabc-0.1.5/setup.cfg
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      755 2024-04-20 11:10:58.000000 astabc-0.1.5/setup.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-20 11:11:37.152974 astabc-0.1.5/tests/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1313 2024-04-12 07:32:38.000000 astabc-0.1.5/tests/test_astabc.py
```

### Comparing `astabc-0.1.4/LICENSE` & `astabc-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `astabc-0.1.4/PKG-INFO` & `astabc-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: astabc
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python module for automatic brightness and contrast optimization
 Home-page: https://github.com/jgwill/gia-abc
 Author: Guillaume Descoteaux-Isabelle
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: opencv-python
 
 # astabc
 
 The `astabc` module is a Python module that provides functions for automatic brightness and contrast optimization of images.
 
 ## Installation
```

### Comparing `astabc-0.1.4/README.md` & `astabc-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `astabc-0.1.4/astabc/astabc.py` & `astabc-0.1.5/astabc/astabc.py`

 * *Files identical despite different names*

### Comparing `astabc-0.1.4/astabc.egg-info/PKG-INFO` & `astabc-0.1.5/astabc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: astabc
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python module for automatic brightness and contrast optimization
 Home-page: https://github.com/jgwill/gia-abc
 Author: Guillaume Descoteaux-Isabelle
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: opencv-python
 
 # astabc
 
 The `astabc` module is a Python module that provides functions for automatic brightness and contrast optimization of images.
 
 ## Installation
```

### Comparing `astabc-0.1.4/tests/test_astabc.py` & `astabc-0.1.5/tests/test_astabc.py`

 * *Files identical despite different names*

