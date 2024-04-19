# Comparing `tmp/ciou-0.2.0.tar.gz` & `tmp/ciou-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciou-0.2.0.tar", last modified: Wed Mar  6 23:28:07 2024, max compression
+gzip compressed data, was "ciou-0.3.0.tar", last modified: Fri Apr 19 16:36:54 2024, max compression
```

## Comparing `ciou-0.2.0.tar` & `ciou-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 23:28:07.216765 ciou-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-06 23:28:03.000000 ciou-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-03-06 23:28:07.216765 ciou-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-06 23:28:03.000000 ciou-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 23:28:07.212765 ciou-0.2.0/ciou/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-06 23:28:03.000000 ciou-0.2.0/ciou/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 23:28:07.216765 ciou-0.2.0/ciou/color/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-06 23:28:03.000000 ciou-0.2.0/ciou/color/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-06 23:28:03.000000 ciou-0.2.0/ciou/color/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-03-06 23:28:03.000000 ciou-0.2.0/ciou/color/_color.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-06 23:28:03.000000 ciou-0.2.0/ciou/color/_dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 23:28:07.216765 ciou-0.2.0/ciou/progress/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-06 23:28:03.000000 ciou-0.2.0/ciou/progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-03-06 23:28:03.000000 ciou-0.2.0/ciou/progress/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-03-06 23:28:03.000000 ciou-0.2.0/ciou/progress/_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-03-06 23:28:03.000000 ciou-0.2.0/ciou/progress/_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-03-06 23:28:03.000000 ciou-0.2.0/ciou/progress/_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 23:28:07.216765 ciou-0.2.0/ciou/terminal/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-06 23:28:03.000000 ciou-0.2.0/ciou/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-06 23:28:03.000000 ciou-0.2.0/ciou/terminal/_windows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 23:28:07.216765 ciou-0.2.0/ciou/time/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-06 23:28:03.000000 ciou-0.2.0/ciou/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-06 23:28:03.000000 ciou-0.2.0/ciou/time/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-06 23:28:03.000000 ciou-0.2.0/ciou/time/_ticker.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-06 23:28:03.000000 ciou-0.2.0/ciou/time/_timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 23:28:07.216765 ciou-0.2.0/ciou.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-03-06 23:28:07.000000 ciou-0.2.0/ciou.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-06 23:28:07.000000 ciou-0.2.0/ciou.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 23:28:07.000000 ciou-0.2.0/ciou.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-06 23:28:07.000000 ciou-0.2.0/ciou.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-06 23:28:03.000000 ciou-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 23:28:07.216765 ciou-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:36:54.250671 ciou-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 16:36:50.000000 ciou-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-19 16:36:54.250671 ciou-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-19 16:36:50.000000 ciou-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:36:54.246671 ciou-0.3.0/ciou/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-19 16:36:50.000000 ciou-0.3.0/ciou/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:36:54.246671 ciou-0.3.0/ciou/color/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-19 16:36:50.000000 ciou-0.3.0/ciou/color/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-19 16:36:50.000000 ciou-0.3.0/ciou/color/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-19 16:36:50.000000 ciou-0.3.0/ciou/color/_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-19 16:36:50.000000 ciou-0.3.0/ciou/color/_dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:36:54.250671 ciou-0.3.0/ciou/progress/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-19 16:36:50.000000 ciou-0.3.0/ciou/progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-04-19 16:36:50.000000 ciou-0.3.0/ciou/progress/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-19 16:36:50.000000 ciou-0.3.0/ciou/progress/_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-19 16:36:50.000000 ciou-0.3.0/ciou/progress/_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-19 16:36:50.000000 ciou-0.3.0/ciou/progress/_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:36:54.250671 ciou-0.3.0/ciou/snapshot/
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-19 16:36:50.000000 ciou-0.3.0/ciou/snapshot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:36:54.250671 ciou-0.3.0/ciou/terminal/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-19 16:36:50.000000 ciou-0.3.0/ciou/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-19 16:36:50.000000 ciou-0.3.0/ciou/terminal/_windows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:36:54.250671 ciou-0.3.0/ciou/time/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-19 16:36:50.000000 ciou-0.3.0/ciou/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-19 16:36:50.000000 ciou-0.3.0/ciou/time/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-19 16:36:50.000000 ciou-0.3.0/ciou/time/_ticker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-19 16:36:50.000000 ciou-0.3.0/ciou/time/_timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:36:54.250671 ciou-0.3.0/ciou.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-19 16:36:54.000000 ciou-0.3.0/ciou.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-19 16:36:54.000000 ciou-0.3.0/ciou.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:36:54.000000 ciou-0.3.0/ciou.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 16:36:54.000000 ciou-0.3.0/ciou.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-19 16:36:50.000000 ciou-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 16:36:54.250671 ciou-0.3.0/setup.cfg
```

### Comparing `ciou-0.2.0/LICENSE` & `ciou-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ciou-0.2.0/PKG-INFO` & `ciou-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciou
-Version: 0.2.0
+Version: 0.3.0
 Summary: CLI input and output utils.
 Author: Toni Kangas
 License: MIT License
         
         Copyright (c) 2024 Toni Kangas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,15 +33,18 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CLI input and output utils (ciou)
 
 [![CI](https://github.com/kangasta/ciou/actions/workflows/ci.yml/badge.svg)](https://github.com/kangasta/ciou/actions/workflows/ci.yml)
+[![Docs](https://github.com/kangasta/ciou/actions/workflows/docs.yml/badge.svg)](https://github.com/kangasta/ciou/actions/workflows/docs.yml)
 [![Release](https://github.com/kangasta/ciou/actions/workflows/release.yml/badge.svg)](https://github.com/kangasta/ciou/actions/workflows/release.yml)
+[![Maintainability](https://api.codeclimate.com/v1/badges/b1f0abcbbb4d64f8b683/maintainability)](https://codeclimate.com/github/kangasta/ciou/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/b1f0abcbbb4d64f8b683/test_coverage)](https://codeclimate.com/github/kangasta/ciou/test_coverage)
 
 Utilities for working with inputs and outputs of command-line interfaces.
 
 ## Testing
 
 Check and automatically fix formatting with:
```

### Comparing `ciou-0.2.0/README.md` & `ciou-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # CLI input and output utils (ciou)
 
 [![CI](https://github.com/kangasta/ciou/actions/workflows/ci.yml/badge.svg)](https://github.com/kangasta/ciou/actions/workflows/ci.yml)
+[![Docs](https://github.com/kangasta/ciou/actions/workflows/docs.yml/badge.svg)](https://github.com/kangasta/ciou/actions/workflows/docs.yml)
 [![Release](https://github.com/kangasta/ciou/actions/workflows/release.yml/badge.svg)](https://github.com/kangasta/ciou/actions/workflows/release.yml)
+[![Maintainability](https://api.codeclimate.com/v1/badges/b1f0abcbbb4d64f8b683/maintainability)](https://codeclimate.com/github/kangasta/ciou/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/b1f0abcbbb4d64f8b683/test_coverage)](https://codeclimate.com/github/kangasta/ciou/test_coverage)
 
 Utilities for working with inputs and outputs of command-line interfaces.
 
 ## Testing
 
 Check and automatically fix formatting with:
 
@@ -33,8 +36,8 @@
 coverage report -m
 ```
 
 Generate the documentation with:
 
 ```sh
 pdoc -d google -o docs ./ciou
-```
+```
```

### Comparing `ciou-0.2.0/ciou/color/__init__.py` & `ciou-0.3.0/ciou/color/__init__.py`

 * *Files identical despite different names*

### Comparing `ciou-0.2.0/ciou/color/_color.py` & `ciou-0.3.0/ciou/color/_color.py`

 * *Files identical despite different names*

### Comparing `ciou-0.2.0/ciou/progress/_config.py` & `ciou-0.3.0/ciou/progress/_config.py`

 * *Files identical despite different names*

### Comparing `ciou-0.2.0/ciou/progress/_message.py` & `ciou-0.3.0/ciou/progress/_message.py`

 * *Files identical despite different names*

### Comparing `ciou-0.2.0/ciou/progress/_progress.py` & `ciou-0.3.0/ciou/progress/_progress.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 SCREEN_WRITE_INTERVAL = 0.095
 STOP = "_stop"
 
 
 class Progress:
     '''The main interface of the `ciou.progress` module.
     '''
+
     def __init__(self, config: OutputConfig = None):
         if not config:
             config = OutputConfig()
 
         self._renderer = MessageRenderer(config)
         self._store = MessageStore()
```

### Comparing `ciou-0.2.0/ciou/progress/_renderer.py` & `ciou-0.3.0/ciou/progress/_renderer.py`

 * *Files identical despite different names*

### Comparing `ciou-0.2.0/ciou/time/_ticker.py` & `ciou-0.3.0/ciou/time/_ticker.py`

 * *Files identical despite different names*

### Comparing `ciou-0.2.0/ciou.egg-info/PKG-INFO` & `ciou-0.3.0/ciou.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciou
-Version: 0.2.0
+Version: 0.3.0
 Summary: CLI input and output utils.
 Author: Toni Kangas
 License: MIT License
         
         Copyright (c) 2024 Toni Kangas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,15 +33,18 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CLI input and output utils (ciou)
 
 [![CI](https://github.com/kangasta/ciou/actions/workflows/ci.yml/badge.svg)](https://github.com/kangasta/ciou/actions/workflows/ci.yml)
+[![Docs](https://github.com/kangasta/ciou/actions/workflows/docs.yml/badge.svg)](https://github.com/kangasta/ciou/actions/workflows/docs.yml)
 [![Release](https://github.com/kangasta/ciou/actions/workflows/release.yml/badge.svg)](https://github.com/kangasta/ciou/actions/workflows/release.yml)
+[![Maintainability](https://api.codeclimate.com/v1/badges/b1f0abcbbb4d64f8b683/maintainability)](https://codeclimate.com/github/kangasta/ciou/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/b1f0abcbbb4d64f8b683/test_coverage)](https://codeclimate.com/github/kangasta/ciou/test_coverage)
 
 Utilities for working with inputs and outputs of command-line interfaces.
 
 ## Testing
 
 Check and automatically fix formatting with:
```

### Comparing `ciou-0.2.0/ciou.egg-info/SOURCES.txt` & `ciou-0.3.0/ciou.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,13 +11,14 @@
 ciou/color/_color.py
 ciou/color/_dynamic.py
 ciou/progress/__init__.py
 ciou/progress/_config.py
 ciou/progress/_message.py
 ciou/progress/_progress.py
 ciou/progress/_renderer.py
+ciou/snapshot/__init__.py
 ciou/terminal/__init__.py
 ciou/terminal/_windows.py
 ciou/time/__init__.py
 ciou/time/__main__.py
 ciou/time/_ticker.py
 ciou/time/_timestamp.py
```

### Comparing `ciou-0.2.0/pyproject.toml` & `ciou-0.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ciou"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
     {name = "Toni Kangas"},
 ]
 description = "CLI input and output utils."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
```

