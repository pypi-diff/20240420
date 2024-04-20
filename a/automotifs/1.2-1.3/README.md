# Comparing `tmp/automotifs-1.2.tar.gz` & `tmp/automotifs-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automotifs-1.2.tar", last modified: Thu Apr 11 14:05:39 2024, max compression
+gzip compressed data, was "automotifs-1.3.tar", last modified: Sat Apr 20 09:15:04 2024, max compression
```

## Comparing `automotifs-1.2.tar` & `automotifs-1.3.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:05:39.288104 automotifs-1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-11 14:05:11.000000 automotifs-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-11 14:05:39.288104 automotifs-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-11 14:05:11.000000 automotifs-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:05:39.284104 automotifs-1.2/automotif/
--rw-r--r--   0 runner    (1001) docker     (127)    19087 2024-04-11 14:05:11.000000 automotifs-1.2/automotif/Neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-11 14:05:11.000000 automotifs-1.2/automotif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17518 2024-04-11 14:05:11.000000 automotifs-1.2/automotif/automotif.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:05:39.288104 automotifs-1.2/automotifs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-11 14:05:39.000000 automotifs-1.2/automotifs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-11 14:05:39.000000 automotifs-1.2/automotifs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:05:39.000000 automotifs-1.2/automotifs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-11 14:05:39.000000 automotifs-1.2/automotifs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 14:05:39.000000 automotifs-1.2/automotifs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 14:05:39.288104 automotifs-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-11 14:05:11.000000 automotifs-1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:05:39.288104 automotifs-1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-11 14:05:11.000000 automotifs-1.2/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:15:04.869626 automotifs-1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-20 09:14:32.000000 automotifs-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-20 09:15:04.869626 automotifs-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-20 09:14:32.000000 automotifs-1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:15:04.869626 automotifs-1.3/automotif/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-20 09:14:32.000000 automotifs-1.3/automotif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17183 2024-04-20 09:14:32.000000 automotifs-1.3/automotif/automotif.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:15:04.869626 automotifs-1.3/automotifs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-20 09:15:04.000000 automotifs-1.3/automotifs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-20 09:15:04.000000 automotifs-1.3/automotifs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 09:15:04.000000 automotifs-1.3/automotifs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-20 09:15:04.000000 automotifs-1.3/automotifs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 09:15:04.000000 automotifs-1.3/automotifs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 09:15:04.869626 automotifs-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-20 09:14:32.000000 automotifs-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:15:04.869626 automotifs-1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-20 09:14:32.000000 automotifs-1.3/tests/test.py
```

### Comparing `automotifs-1.2/LICENSE` & `automotifs-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `automotifs-1.2/PKG-INFO` & `automotifs-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automotifs
-Version: 1.2
+Version: 1.3
 Summary: A wrapper for automatic Motif Detection
 Home-page: https://github.com/GiorgioMB/auto_dotmotif/
 Author: Giorgio Micaletto
 Author-email: giorgio.micaletto@studbocconi.it
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `automotifs-1.2/README.md` & `automotifs-1.3/README.md`

 * *Files identical despite different names*

### Comparing `automotifs-1.2/automotif/automotif.py` & `automotifs-1.3/automotif/automotif.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 Developed by Giorgio Micaletto under the supervision of Professor Marta Zava at Bocconi University,
 this tool aims to facilitate the systematic study of network motifs.
 """
 import random
 import pandas as pd 
 import networkx as nx
-from .Neo4j import Neo4jExecutor
 import os
 from dotmotif import Motif
 from itertools import product
 import dotmotif.executors as executors
 from typing import Union
 import numpy as np
 import matplotlib.pyplot as plt
@@ -53,15 +52,14 @@
                  upto: bool = False,
                  lower: int = 3, 
                  save: bool = False, 
                  path: str = None,
                  find: bool = False, 
                  verbose: bool = False,
                  use_GrandISO: bool = False,
-                 use_Neo4j: bool = False,
                  personal_executor: executors.Executor = None):
         if not hasattr(Graph, "nodes") or not callable(getattr(Graph, "nodes")):
             raise ValueError("Graph should be a NetworkX graph")
         elif type(size) != int:
             raise ValueError("Size should be an integer")
         elif type(upto) != bool:
             raise ValueError("Upto should be a boolean")
@@ -86,18 +84,14 @@
         self.lower = lower
         if personal_executor is not None:
             self.Ex = personal_executor
         if use_GrandISO == True:
             self.Ex = executors.GrandIsoExecutor(graph = self.Graph)
             if personal_executor is not None:
                 print("Warning: The Executor provided will be ignored in favor of GrandIsoExecutor as use_GrandISO is set to True")
-        elif use_Neo4j == True:
-            self.Ex = Neo4jExecutor(graph = self.Graph)
-            if personal_executor is not None:
-                print("Warning: The Executor provided will be ignored in favor of Neo4jExecutor as use_Neo4j is set to True")
         else:
             self.Ex = executors.NetworkXExecutor(graph = self.Graph)
         self.motifs = None
         self.generate_required_motifs()
         self.motifs_found = None
         if find == True:
             self.find_all_motifs()
```

### Comparing `automotifs-1.2/automotifs.egg-info/PKG-INFO` & `automotifs-1.3/automotifs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automotifs
-Version: 1.2
+Version: 1.3
 Summary: A wrapper for automatic Motif Detection
 Home-page: https://github.com/GiorgioMB/auto_dotmotif/
 Author: Giorgio Micaletto
 Author-email: giorgio.micaletto@studbocconi.it
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `automotifs-1.2/setup.py` & `automotifs-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """This module sets up the package for distribution."""
 from setuptools import setup, find_packages
 setup(
     name='automotifs',
-    version='1.2',
+    version='1.3',
     packages=find_packages(),
     description='A wrapper for automatic Motif Detection',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Giorgio Micaletto',
     author_email='giorgio.micaletto@studbocconi.it',
     url='https://github.com/GiorgioMB/auto_dotmotif/',
```

### Comparing `automotifs-1.2/tests/test.py` & `automotifs-1.3/tests/test.py`

 * *Files identical despite different names*

