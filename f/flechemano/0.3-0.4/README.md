# Comparing `tmp/flechemano-0.3.tar.gz` & `tmp/flechemano-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flechemano-0.3.tar", last modified: Sat Apr 20 07:46:23 2024, max compression
+gzip compressed data, was "flechemano-0.4.tar", last modified: Sat Apr 20 07:51:30 2024, max compression
```

## Comparing `flechemano-0.3.tar` & `flechemano-0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 07:46:23.594133 flechemano-0.3/
--rw-r--r--   0 root         (0) root         (0)      709 2024-04-20 07:46:23.594133 flechemano-0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      413 2024-04-20 07:12:43.000000 flechemano-0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 07:46:23.594133 flechemano-0.3/flechemano.egg-info/
--rw-r--r--   0 root         (0) root         (0)      709 2024-04-20 07:46:23.000000 flechemano-0.3/flechemano.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      187 2024-04-20 07:46:23.000000 flechemano-0.3/flechemano.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 07:46:23.000000 flechemano-0.3/flechemano.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-20 07:46:23.000000 flechemano-0.3/flechemano.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 07:46:23.000000 flechemano-0.3/flechemano.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 07:46:23.594133 flechemano-0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      466 2024-04-20 07:46:16.000000 flechemano-0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 07:51:30.215316 flechemano-0.4/
+-rw-r--r--   0 root         (0) root         (0)      683 2024-04-20 07:51:30.215316 flechemano-0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      387 2024-04-20 07:51:01.000000 flechemano-0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 07:51:30.215316 flechemano-0.4/flechemano.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      683 2024-04-20 07:51:30.000000 flechemano-0.4/flechemano.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      187 2024-04-20 07:51:30.000000 flechemano-0.4/flechemano.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 07:51:30.000000 flechemano-0.4/flechemano.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-20 07:51:30.000000 flechemano-0.4/flechemano.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 07:51:30.000000 flechemano-0.4/flechemano.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 07:51:30.215316 flechemano-0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      466 2024-04-20 07:51:16.000000 flechemano-0.4/setup.py
```

### Comparing `flechemano-0.3/PKG-INFO` & `flechemano-0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: flechemano
-Version: 0.3
+Version: 0.4
 Summary: A package developed for blacktea024 to integrate it with PyPI.
 Home-page: https://github.com/flechemano/flechemano
 Author: flechemano
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-
-```
 # flechemano
 
 flechemano is a Python package developed for blacktea024 to integrate it with PyPI.
 
 ## Installation
 
 You can install flechemano using pip:
@@ -24,26 +22,24 @@
 ```
 
 ## Usage
 
 ```python
 import oktay1024
 
-# Example usage here
 ```
 
 ## Dependencies
 
 flechemano depends on the following:
-- blacktea024
-
+- oktay1024
 ## Author
 
 flechemano
 
 ## License
 
+```
 This project is licensed under the MIT License.
 ```
 
 
-
```

### Comparing `flechemano-0.3/flechemano.egg-info/PKG-INFO` & `flechemano-0.4/flechemano.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: flechemano
-Version: 0.3
+Version: 0.4
 Summary: A package developed for blacktea024 to integrate it with PyPI.
 Home-page: https://github.com/flechemano/flechemano
 Author: flechemano
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-
-```
 # flechemano
 
 flechemano is a Python package developed for blacktea024 to integrate it with PyPI.
 
 ## Installation
 
 You can install flechemano using pip:
@@ -24,26 +22,24 @@
 ```
 
 ## Usage
 
 ```python
 import oktay1024
 
-# Example usage here
 ```
 
 ## Dependencies
 
 flechemano depends on the following:
-- blacktea024
-
+- oktay1024
 ## Author
 
 flechemano
 
 ## License
 
+```
 This project is licensed under the MIT License.
 ```
 
 
-
```

