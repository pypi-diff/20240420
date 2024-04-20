# Comparing `tmp/ansi-string-0.0.3.tar.gz` & `tmp/ansi-string-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansi-string-0.0.3.tar", last modified: Fri Apr 19 02:54:23 2024, max compression
+gzip compressed data, was "ansi-string-0.0.4.tar", last modified: Fri Apr 19 03:22:56 2024, max compression
```

## Comparing `ansi-string-0.0.3.tar` & `ansi-string-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:54:23.529635 ansi-string-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-19 02:54:15.000000 ansi-string-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-19 02:54:23.529635 ansi-string-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 02:54:15.000000 ansi-string-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-19 02:54:15.000000 ansi-string-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 02:54:23.529635 ansi-string-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-19 02:54:15.000000 ansi-string-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:54:23.525635 ansi-string-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:54:23.525635 ansi-string-0.0.3/src/ansi_string/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-19 02:54:15.000000 ansi-string-0.0.3/src/ansi_string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17015 2024-04-19 02:54:15.000000 ansi-string-0.0.3/src/ansi_string/ansi_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:54:23.529635 ansi-string-0.0.3/src/ansi_string.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-19 02:54:23.000000 ansi-string-0.0.3/src/ansi_string.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-19 02:54:23.000000 ansi-string-0.0.3/src/ansi_string.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 02:54:23.000000 ansi-string-0.0.3/src/ansi_string.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 02:54:23.000000 ansi-string-0.0.3/src/ansi_string.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 02:54:23.000000 ansi-string-0.0.3/src/ansi_string.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:22:56.257717 ansi-string-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 03:22:48.000000 ansi-string-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-19 03:22:56.257717 ansi-string-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 03:22:48.000000 ansi-string-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-19 03:22:48.000000 ansi-string-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 03:22:56.257717 ansi-string-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-19 03:22:48.000000 ansi-string-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:22:56.257717 ansi-string-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:22:56.257717 ansi-string-0.0.4/src/ansi_string/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-19 03:22:48.000000 ansi-string-0.0.4/src/ansi_string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17015 2024-04-19 03:22:48.000000 ansi-string-0.0.4/src/ansi_string/ansi_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:22:56.257717 ansi-string-0.0.4/src/ansi_string.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-19 03:22:56.000000 ansi-string-0.0.4/src/ansi_string.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-19 03:22:56.000000 ansi-string-0.0.4/src/ansi_string.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 03:22:56.000000 ansi-string-0.0.4/src/ansi_string.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 03:22:56.000000 ansi-string-0.0.4/src/ansi_string.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 03:22:56.000000 ansi-string-0.0.4/src/ansi_string.egg-info/top_level.txt
```

### Comparing `ansi-string-0.0.3/PKG-INFO` & `ansi-string-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansi-string
-Version: 0.0.3
+Version: 0.0.4
 Summary: ANSI String Formatter in Python for CLI Color and Style Formatting
 Home-page: https://github.com/Tails86/ansi-string
 Author: James Smith
 Author-email: jmsmith86@gmail.com
 Project-URL: Documentation, https://github.com/Tails86/ansi-string
 Project-URL: Bug Reports, https://github.com/Tails86/ansi-string/issues
 Project-URL: Source Code, https://github.com/Tails86/ansi-string
@@ -27,7 +27,11 @@
 Provides-Extra: dev
 
 # ansi-string
 
 This is a work in progress.
 
 This code was originally written for [greplica](https://pypi.org/project/greplica/), but I felt it deserved its own, separate library.
+
+## Examples:
+
+![Examples](https://github.com/Tails86/ansi-string/blob/main/docs/examples.jpg?raw=true)
```

### Comparing `ansi-string-0.0.3/setup.py` & `ansi-string-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `ansi-string-0.0.3/src/ansi_string/ansi_string.py` & `ansi-string-0.0.4/src/ansi_string/ansi_string.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # SOFTWARE.
 
 import sys
 from enum import Enum
 import io
 from typing import Any, Union, List
 
-__version__ = '0.0.3'
+__version__ = '0.0.4'
 PACKAGE_NAME = 'ansi-string'
 
 IS_WINDOWS = sys.platform.lower().startswith('win')
 
 if IS_WINDOWS:
     try:
         import ctypes
```

### Comparing `ansi-string-0.0.3/src/ansi_string.egg-info/PKG-INFO` & `ansi-string-0.0.4/src/ansi_string.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansi-string
-Version: 0.0.3
+Version: 0.0.4
 Summary: ANSI String Formatter in Python for CLI Color and Style Formatting
 Home-page: https://github.com/Tails86/ansi-string
 Author: James Smith
 Author-email: jmsmith86@gmail.com
 Project-URL: Documentation, https://github.com/Tails86/ansi-string
 Project-URL: Bug Reports, https://github.com/Tails86/ansi-string/issues
 Project-URL: Source Code, https://github.com/Tails86/ansi-string
@@ -27,7 +27,11 @@
 Provides-Extra: dev
 
 # ansi-string
 
 This is a work in progress.
 
 This code was originally written for [greplica](https://pypi.org/project/greplica/), but I felt it deserved its own, separate library.
+
+## Examples:
+
+![Examples](https://github.com/Tails86/ansi-string/blob/main/docs/examples.jpg?raw=true)
```

