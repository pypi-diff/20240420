# Comparing `tmp/automotifs-1.3.tar.gz` & `tmp/automotifs-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automotifs-1.3.tar", last modified: Sat Apr 20 09:15:04 2024, max compression
+gzip compressed data, was "automotifs-1.4.1.tar", last modified: Sat Apr 20 21:14:22 2024, max compression
```

## Comparing `automotifs-1.3.tar` & `automotifs-1.4.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:15:04.869626 automotifs-1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-20 09:14:32.000000 automotifs-1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-20 09:15:04.869626 automotifs-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-20 09:14:32.000000 automotifs-1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:15:04.869626 automotifs-1.3/automotif/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-20 09:14:32.000000 automotifs-1.3/automotif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17183 2024-04-20 09:14:32.000000 automotifs-1.3/automotif/automotif.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:15:04.869626 automotifs-1.3/automotifs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-20 09:15:04.000000 automotifs-1.3/automotifs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-20 09:15:04.000000 automotifs-1.3/automotifs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 09:15:04.000000 automotifs-1.3/automotifs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-20 09:15:04.000000 automotifs-1.3/automotifs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 09:15:04.000000 automotifs-1.3/automotifs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 09:15:04.869626 automotifs-1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-20 09:14:32.000000 automotifs-1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:15:04.869626 automotifs-1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-20 09:14:32.000000 automotifs-1.3/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:14:22.434566 automotifs-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-20 21:14:02.000000 automotifs-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-20 21:14:22.434566 automotifs-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-20 21:14:02.000000 automotifs-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:14:22.430566 automotifs-1.4.1/automotif/
+-rw-r--r--   0 runner    (1001) docker     (127)    18615 2024-04-20 21:14:02.000000 automotifs-1.4.1/automotif/GPU_Executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-20 21:14:02.000000 automotifs-1.4.1/automotif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17661 2024-04-20 21:14:02.000000 automotifs-1.4.1/automotif/automotif.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:14:22.434566 automotifs-1.4.1/automotifs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-20 21:14:22.000000 automotifs-1.4.1/automotifs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-20 21:14:22.000000 automotifs-1.4.1/automotifs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 21:14:22.000000 automotifs-1.4.1/automotifs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-20 21:14:22.000000 automotifs-1.4.1/automotifs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 21:14:22.000000 automotifs-1.4.1/automotifs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 21:14:22.434566 automotifs-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-20 21:14:02.000000 automotifs-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:14:22.434566 automotifs-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-20 21:14:02.000000 automotifs-1.4.1/tests/test.py
```

### Comparing `automotifs-1.3/LICENSE` & `automotifs-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `automotifs-1.3/PKG-INFO` & `automotifs-1.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: automotifs
-Version: 1.3
+Version: 1.4.1
 Summary: A wrapper for automatic Motif Detection
 Home-page: https://github.com/GiorgioMB/auto_dotmotif/
 Author: Giorgio Micaletto
 Author-email: giorgio.micaletto@studbocconi.it
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=1.1.5
 Requires-Dist: pylint>=2.6.0
 Requires-Dist: numpy>=1.23
 Requires-Dist: dotmotif>=0.14.0
 Requires-Dist: networkx>=3.2.1
-Requires-Dist: tamarind>=0.2.1
-Requires-Dist: py2neo>=2021.2.4
 
 # AutoMotif: Automated Motif Detection in Network Graphs
 ## What is it?
 AutoMotif streamlines the identification and cataloging of motifs within network graphs. Utilizing NetworkX for graph manipulation, dotmotif for detecting motifs, and pandas for data management, it simplifies the process of uncovering patterns across both directed and undirected networks. Users can customize searches based on motif size, directionality, executors and the treatment of automorphisms, as well as even having the option to save the results for further analysis.
 
 ## Installation
```

### Comparing `automotifs-1.3/README.md` & `automotifs-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `automotifs-1.3/automotif/automotif.py` & `automotifs-1.4.1/automotif/automotif.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from dotmotif import Motif
 from itertools import product
 import dotmotif.executors as executors
 from typing import Union
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
+from .GPU_Executor import AcceleratedExecutor
 
 class AutoMotif:
     """
     Wrapper class for dotmotif to find all possible motifs in a graph automatically.
     Inputs:
     - Graph (networkx.Graph): The graph to analyze.
     - size (int): Size of the motif to find.
@@ -38,28 +39,30 @@
     - upto (bool, optional): Whether to generate motifs from a lower bound to the specified size. Defaults to False.
     - lower (int, optional): Lower bound for motif size. Defaults to 3.
     - save (bool, optional): Whether to save the motifs to a CSV file. Defaults to False.
     - path (str, optional): Directory to save the motifs. Defaults to None.
     - find (bool, optional): Whether to find all motifs directly. Defaults to False.
     - verbose (bool, optional): Whether to print progress. Defaults to False.
     - use_GrandISO (bool, optional): Whether to use GrandISO for motif detection. Defaults to False.
+    - use_GPU (bool, optional): Whether to use the GPU accelerated executor for motif detection. Defaults to False
     - personal_executor (dotmotif.executors.Executor, optional): Executor to use for motif detection. Defaults to None.
     """
     def __init__(self, 
                  Graph: Union[nx.Graph, nx.DiGraph, nx.MultiGraph, nx.MultiDiGraph], 
                  size: int, 
                  directed: bool = False, 
                  allow_automorphism: bool = False, 
                  upto: bool = False,
                  lower: int = 3, 
                  save: bool = False, 
                  path: str = None,
                  find: bool = False, 
                  verbose: bool = False,
                  use_GrandISO: bool = False,
+                 use_GPU: bool = False
                  personal_executor: executors.Executor = None):
         if not hasattr(Graph, "nodes") or not callable(getattr(Graph, "nodes")):
             raise ValueError("Graph should be a NetworkX graph")
         elif type(size) != int:
             raise ValueError("Size should be an integer")
         elif type(upto) != bool:
             raise ValueError("Upto should be a boolean")
@@ -80,25 +83,29 @@
         self.path = path
         self.verbose = verbose
         self.directed = directed
         self.allow_automorphism = allow_automorphism
         self.lower = lower
         if personal_executor is not None:
             self.Ex = personal_executor
-        if use_GrandISO == True:
+        if use_GrandISO:
             self.Ex = executors.GrandIsoExecutor(graph = self.Graph)
             if personal_executor is not None:
                 print("Warning: The Executor provided will be ignored in favor of GrandIsoExecutor as use_GrandISO is set to True")
+        if use_GPU:
+            self.Ex = AcceleratedExecutor (graph = self.Graph)
+            if personal_executor is not None or use_GrandISO == True:
+                print("Warning: GPU Accelerator Executor will be used, ignoring other executors provided, as use_GPU is set to True")
         else:
             self.Ex = executors.NetworkXExecutor(graph = self.Graph)
         self.motifs = None
         self.generate_required_motifs()
         self.motifs_found = None
-        if find == True:
-            self.find_all_motifs()    
+        if find:
+            return self.find_all_motifs()    
     
     def generate_graphs(self, n: int) -> list:
         """
         Generate all possible directed graphs for n nodes, ignoring self-loops,
         and ensure no isolated nodes are present. Each graph is represented by its adjacency matrix.
         Inputs:
         - n (int): Number of nodes.
```

### Comparing `automotifs-1.3/automotifs.egg-info/PKG-INFO` & `automotifs-1.4.1/automotifs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: automotifs
-Version: 1.3
+Version: 1.4.1
 Summary: A wrapper for automatic Motif Detection
 Home-page: https://github.com/GiorgioMB/auto_dotmotif/
 Author: Giorgio Micaletto
 Author-email: giorgio.micaletto@studbocconi.it
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=1.1.5
 Requires-Dist: pylint>=2.6.0
 Requires-Dist: numpy>=1.23
 Requires-Dist: dotmotif>=0.14.0
 Requires-Dist: networkx>=3.2.1
-Requires-Dist: tamarind>=0.2.1
-Requires-Dist: py2neo>=2021.2.4
 
 # AutoMotif: Automated Motif Detection in Network Graphs
 ## What is it?
 AutoMotif streamlines the identification and cataloging of motifs within network graphs. Utilizing NetworkX for graph manipulation, dotmotif for detecting motifs, and pandas for data management, it simplifies the process of uncovering patterns across both directed and undirected networks. Users can customize searches based on motif size, directionality, executors and the treatment of automorphisms, as well as even having the option to save the results for further analysis.
 
 ## Installation
```

### Comparing `automotifs-1.3/tests/test.py` & `automotifs-1.4.1/tests/test.py`

 * *Files identical despite different names*

