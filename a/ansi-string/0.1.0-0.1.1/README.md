# Comparing `tmp/ansi-string-0.1.0.tar.gz` & `tmp/ansi-string-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansi-string-0.1.0.tar", last modified: Sat Apr 20 01:01:45 2024, max compression
+gzip compressed data, was "ansi-string-0.1.1.tar", last modified: Sat Apr 20 01:05:34 2024, max compression
```

## Comparing `ansi-string-0.1.0.tar` & `ansi-string-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:01:45.167129 ansi-string-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 01:01:35.000000 ansi-string-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-20 01:01:35.000000 ansi-string-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-20 01:01:45.167129 ansi-string-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-20 01:01:35.000000 ansi-string-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:01:45.167129 ansi-string-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)   320348 2024-04-20 01:01:35.000000 ansi-string-0.1.0/docs/examples.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-20 01:01:35.000000 ansi-string-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-20 01:01:45.167129 ansi-string-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-20 01:01:35.000000 ansi-string-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:01:45.163128 ansi-string-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:01:45.167129 ansi-string-0.1.0/src/ansi_string/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-20 01:01:35.000000 ansi-string-0.1.0/src/ansi_string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52215 2024-04-20 01:01:35.000000 ansi-string-0.1.0/src/ansi_string/ansi_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:01:45.167129 ansi-string-0.1.0/src/ansi_string.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-20 01:01:45.000000 ansi-string-0.1.0/src/ansi_string.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-20 01:01:45.000000 ansi-string-0.1.0/src/ansi_string.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:01:45.000000 ansi-string-0.1.0/src/ansi_string.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 01:01:45.000000 ansi-string-0.1.0/src/ansi_string.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-20 01:01:45.000000 ansi-string-0.1.0/src/ansi_string.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:05:34.326753 ansi-string-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 01:05:23.000000 ansi-string-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-20 01:05:23.000000 ansi-string-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-20 01:05:34.326753 ansi-string-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-20 01:05:23.000000 ansi-string-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-20 01:05:23.000000 ansi-string-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-20 01:05:34.326753 ansi-string-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-20 01:05:23.000000 ansi-string-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:05:34.326753 ansi-string-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:05:34.326753 ansi-string-0.1.1/src/ansi_string/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-20 01:05:23.000000 ansi-string-0.1.1/src/ansi_string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52215 2024-04-20 01:05:23.000000 ansi-string-0.1.1/src/ansi_string/ansi_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:05:34.326753 ansi-string-0.1.1/src/ansi_string.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-20 01:05:34.000000 ansi-string-0.1.1/src/ansi_string.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-20 01:05:34.000000 ansi-string-0.1.1/src/ansi_string.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:05:34.000000 ansi-string-0.1.1/src/ansi_string.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 01:05:34.000000 ansi-string-0.1.1/src/ansi_string.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-20 01:05:34.000000 ansi-string-0.1.1/src/ansi_string.egg-info/top_level.txt
```

### Comparing `ansi-string-0.1.0/LICENSE` & `ansi-string-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansi-string-0.1.0/PKG-INFO` & `ansi-string-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansi-string
-Version: 0.1.0
+Version: 0.1.1
 Summary: ANSI String Formatter in Python for CLI Color and Style Formatting
 Home-page: https://github.com/Tails86/ansi-string
 Author: James Smith
 Author-email: jmsmith86@gmail.com
 Project-URL: Documentation, https://github.com/Tails86/ansi-string
 Project-URL: Bug Reports, https://github.com/Tails86/ansi-string/issues
 Project-URL: Source Code, https://github.com/Tails86/ansi-string
@@ -30,8 +30,8 @@
 
 This is a work in progress.
 
 This code was originally written for [greplica](https://pypi.org/project/greplica/), but I felt it deserved its own, separate library.
 
 ## Examples:
 
-![Examples](docs/examples.jpg)
+![Examples](https://raw.githubusercontent.com/Tails86/ansi-string/edfa8234f9b408c594c3659585c4e2c6de602cb8/docs/examples.jpg)
```

### Comparing `ansi-string-0.1.0/setup.py` & `ansi-string-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `ansi-string-0.1.0/src/ansi_string/ansi_string.py` & `ansi-string-0.1.1/src/ansi_string/ansi_string.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import re
 import copy
 import math
 from enum import Enum, EnumMeta, auto as enum_auto
 import io
 from typing import Any, Union, List
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 PACKAGE_NAME = 'ansi-string'
 
 IS_WINDOWS = sys.platform.lower().startswith('win')
 
 if IS_WINDOWS:
     try:
         import ctypes
```

### Comparing `ansi-string-0.1.0/src/ansi_string.egg-info/PKG-INFO` & `ansi-string-0.1.1/src/ansi_string.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansi-string
-Version: 0.1.0
+Version: 0.1.1
 Summary: ANSI String Formatter in Python for CLI Color and Style Formatting
 Home-page: https://github.com/Tails86/ansi-string
 Author: James Smith
 Author-email: jmsmith86@gmail.com
 Project-URL: Documentation, https://github.com/Tails86/ansi-string
 Project-URL: Bug Reports, https://github.com/Tails86/ansi-string/issues
 Project-URL: Source Code, https://github.com/Tails86/ansi-string
@@ -30,8 +30,8 @@
 
 This is a work in progress.
 
 This code was originally written for [greplica](https://pypi.org/project/greplica/), but I felt it deserved its own, separate library.
 
 ## Examples:
 
-![Examples](docs/examples.jpg)
+![Examples](https://raw.githubusercontent.com/Tails86/ansi-string/edfa8234f9b408c594c3659585c4e2c6de602cb8/docs/examples.jpg)
```

