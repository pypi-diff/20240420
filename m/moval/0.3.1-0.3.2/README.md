# Comparing `tmp/moval-0.3.1.tar.gz` & `tmp/moval-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/zejuli/Local/Imperial/MOVAL/dist/.tmp-6icvosnx/moval-0.3.1.tar", last modified: Thu Apr 18 18:39:13 2024, max compression
+gzip compressed data, was "/Users/zejuli/Local/Imperial/MOVAL/dist/.tmp-pbbzones/moval-0.3.2.tar", last modified: Sat Apr 20 02:15:01 2024, max compression
```

## Comparing `moval-0.3.1.tar` & `moval-0.3.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-18 18:39:13.002766 moval-0.3.1/
--rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-04-18 18:39:13.002702 moval-0.3.1/PKG-INFO
--rw-r--r--   0 zejuli     (501) staff       (20)     2259 2024-01-19 15:02:41.000000 moval-0.3.1/README.md
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-18 18:39:12.999312 moval-0.3.1/moval/
--rw-r--r--   0 zejuli     (501) staff       (20)      706 2024-04-18 18:38:14.000000 moval-0.3.1/moval/__init__.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-18 18:39:13.000112 moval-0.3.1/moval/integrations/
--rw-r--r--   0 zejuli     (501) staff       (20)       68 2023-07-28 01:11:44.000000 moval-0.3.1/moval/integrations/__init__.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-18 18:39:13.000406 moval-0.3.1/moval/integrations/sklearn/
--rw-r--r--   0 zejuli     (501) staff       (20)      462 2023-10-26 14:28:12.000000 moval-0.3.1/moval/integrations/sklearn/__init__.py
--rw-r--r--   0 zejuli     (501) staff       (20)    41094 2024-04-15 02:33:08.000000 moval-0.3.1/moval/integrations/sklearn/moval.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-18 18:39:13.001464 moval-0.3.1/moval/models/
--rw-r--r--   0 zejuli     (501) staff       (20)      447 2023-11-09 00:55:21.000000 moval-0.3.1/moval/models/__init__.py
--rw-r--r--   0 zejuli     (501) staff       (20)     6840 2023-11-26 14:30:38.000000 moval-0.3.1/moval/models/confidences.py
--rw-r--r--   0 zejuli     (501) staff       (20)    44718 2024-04-17 02:22:33.000000 moval-0.3.1/moval/models/model.py
--rw-r--r--   0 zejuli     (501) staff       (20)     1631 2024-01-08 19:28:25.000000 moval-0.3.1/moval/models/solver_temperature.py
--rw-r--r--   0 zejuli     (501) staff       (20)    10841 2024-04-17 16:31:30.000000 moval-0.3.1/moval/models/utils.py
--rw-r--r--   0 zejuli     (501) staff       (20)    15406 2023-11-08 14:02:19.000000 moval-0.3.1/moval/registry.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-18 18:39:13.002199 moval-0.3.1/moval/solvers/
--rw-r--r--   0 zejuli     (501) staff       (20)      429 2023-11-09 00:58:57.000000 moval-0.3.1/moval/solvers/__init__.py
--rw-r--r--   0 zejuli     (501) staff       (20)    11235 2024-04-15 02:36:06.000000 moval-0.3.1/moval/solvers/criterions.py
--rw-r--r--   0 zejuli     (501) staff       (20)    28961 2024-04-18 18:36:48.000000 moval-0.3.1/moval/solvers/solver.py
--rw-r--r--   0 zejuli     (501) staff       (20)     3054 2024-04-08 23:54:48.000000 moval-0.3.1/moval/solvers/utils.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-18 18:39:13.002428 moval-0.3.1/moval.egg-info/
--rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-04-18 18:39:12.000000 moval-0.3.1/moval.egg-info/PKG-INFO
--rw-r--r--   0 zejuli     (501) staff       (20)      553 2024-04-18 18:39:12.000000 moval-0.3.1/moval.egg-info/SOURCES.txt
--rw-r--r--   0 zejuli     (501) staff       (20)        1 2024-04-18 18:39:12.000000 moval-0.3.1/moval.egg-info/dependency_links.txt
--rw-r--r--   0 zejuli     (501) staff       (20)       61 2024-04-18 18:39:12.000000 moval-0.3.1/moval.egg-info/requires.txt
--rw-r--r--   0 zejuli     (501) staff       (20)        6 2024-04-18 18:39:12.000000 moval-0.3.1/moval.egg-info/top_level.txt
--rw-r--r--   0 zejuli     (501) staff       (20)    15479 2023-12-08 04:03:18.000000 moval-0.3.1/pyproject.toml
--rw-r--r--   0 zejuli     (501) staff       (20)      896 2024-04-18 18:39:13.003157 moval-0.3.1/setup.cfg
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-20 02:15:01.693465 moval-0.3.2/
+-rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-04-20 02:15:01.693391 moval-0.3.2/PKG-INFO
+-rw-r--r--   0 zejuli     (501) staff       (20)     2259 2024-01-19 15:02:41.000000 moval-0.3.2/README.md
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-20 02:15:01.687841 moval-0.3.2/moval/
+-rw-r--r--   0 zejuli     (501) staff       (20)      706 2024-04-20 02:13:22.000000 moval-0.3.2/moval/__init__.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-20 02:15:01.689108 moval-0.3.2/moval/integrations/
+-rw-r--r--   0 zejuli     (501) staff       (20)       68 2023-07-28 01:11:44.000000 moval-0.3.2/moval/integrations/__init__.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-20 02:15:01.689688 moval-0.3.2/moval/integrations/sklearn/
+-rw-r--r--   0 zejuli     (501) staff       (20)      462 2023-10-26 14:28:12.000000 moval-0.3.2/moval/integrations/sklearn/__init__.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    41094 2024-04-15 02:33:08.000000 moval-0.3.2/moval/integrations/sklearn/moval.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-20 02:15:01.691848 moval-0.3.2/moval/models/
+-rw-r--r--   0 zejuli     (501) staff       (20)      447 2023-11-09 00:55:21.000000 moval-0.3.2/moval/models/__init__.py
+-rw-r--r--   0 zejuli     (501) staff       (20)     6840 2023-11-26 14:30:38.000000 moval-0.3.2/moval/models/confidences.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    44718 2024-04-17 02:22:33.000000 moval-0.3.2/moval/models/model.py
+-rw-r--r--   0 zejuli     (501) staff       (20)     1631 2024-01-08 19:28:25.000000 moval-0.3.2/moval/models/solver_temperature.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    10804 2024-04-20 02:13:02.000000 moval-0.3.2/moval/models/utils.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    15406 2023-11-08 14:02:19.000000 moval-0.3.2/moval/registry.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-20 02:15:01.692816 moval-0.3.2/moval/solvers/
+-rw-r--r--   0 zejuli     (501) staff       (20)      429 2023-11-09 00:58:57.000000 moval-0.3.2/moval/solvers/__init__.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    11235 2024-04-15 02:36:06.000000 moval-0.3.2/moval/solvers/criterions.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    28959 2024-04-20 02:13:00.000000 moval-0.3.2/moval/solvers/solver.py
+-rw-r--r--   0 zejuli     (501) staff       (20)     3054 2024-04-08 23:54:48.000000 moval-0.3.2/moval/solvers/utils.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-20 02:15:01.693132 moval-0.3.2/moval.egg-info/
+-rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-04-20 02:15:01.000000 moval-0.3.2/moval.egg-info/PKG-INFO
+-rw-r--r--   0 zejuli     (501) staff       (20)      553 2024-04-20 02:15:01.000000 moval-0.3.2/moval.egg-info/SOURCES.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)        1 2024-04-20 02:15:01.000000 moval-0.3.2/moval.egg-info/dependency_links.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)       61 2024-04-20 02:15:01.000000 moval-0.3.2/moval.egg-info/requires.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)        6 2024-04-20 02:15:01.000000 moval-0.3.2/moval.egg-info/top_level.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)    15479 2023-12-08 04:03:18.000000 moval-0.3.2/pyproject.toml
+-rw-r--r--   0 zejuli     (501) staff       (20)      896 2024-04-20 02:15:01.693816 moval-0.3.2/setup.cfg
```

### Comparing `moval-0.3.1/PKG-INFO` & `moval-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moval
-Version: 0.3.1
+Version: 0.3.2
 Summary: Model evaluation without manual labels
 Home-page: https://github.com/ZerojumpLine/MOVAL
 Author: Zeju Li
 Author-email: lizeju8@gmail.com
 Project-URL: Bug Tracker, https://github.com/ZerojumpLine/MOVAL/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moval Version: 0.3.1 Summary: Model evaluation
+Metadata-Version: 2.1 Name: moval Version: 0.3.2 Summary: Model evaluation
 without manual labels Home-page: https://github.com/ZerojumpLine/MOVAL Author:
 Zeju Li Author-email: lizeju8@gmail.com Project-URL: Bug Tracker, https://
 github.com/ZerojumpLine/MOVAL/issues Classifier: Development Status :: 3 -
 Alpha Classifier: Environment :: GPU :: NVIDIA CUDA Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: License :: Free
```

### Comparing `moval-0.3.1/README.md` & `moval-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `moval-0.3.1/moval/__init__.py` & `moval-0.3.2/moval/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 try:
     from moval.integrations.sklearn.moval import MOVAL
 except ImportError as e:
     # silently fail for now
     pass
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 __all__ = ["MOVAL"]
 
 def __getattr__(key):
     """Lazy import of moval submodules and -packages.
 
     Once :py:mod:`moval` is imported, it is possible to lazy import
```

### Comparing `moval-0.3.1/moval/integrations/sklearn/moval.py` & `moval-0.3.2/moval/integrations/sklearn/moval.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.1/moval/models/confidences.py` & `moval-0.3.2/moval/models/confidences.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.1/moval/models/model.py` & `moval-0.3.2/moval/models/model.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.1/moval/models/solver_temperature.py` & `moval-0.3.2/moval/models/solver_temperature.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.1/moval/models/utils.py` & `moval-0.3.2/moval/models/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     
     Returns:
         energy: The calculated energy of shape ``(n, )``
 
     """
 
     denominator = np.sum(np.exp(x.transpose() / T), axis=0)
-    # energy = - T * np.log(denominator)
-    energy = - np.log(denominator)
+    energy = - T * np.log(denominator)
 
     return energy
 
 def cal_mcp(x: np.ndarray, T = 1) -> np.ndarray:
     """Compute maximum class probability (MCP) for each sets of scores in x.
     
     Args:
```

### Comparing `moval-0.3.1/moval/registry.py` & `moval-0.3.2/moval/registry.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.1/moval/solvers/criterions.py` & `moval-0.3.2/moval/solvers/criterions.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.1/moval/solvers/solver.py` & `moval-0.3.2/moval/solvers/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,24 +238,24 @@
 
         if self.model.mode == "classification":
             if self.model.estim_algorithm == "doc-model":
                 # the range of doc estimation is [0, 2].
                 initial_conditions = [np.array([0.01]), np.array([0.1]), np.array([0.5]), np.array([1.5]), np.array([1.8])]
             else:
                 # the range of ts estimation is [0, inf].
-                initial_conditions = [np.array([0.01]), np.array([0.5]), np.array([3.]), np.array([5.]), np.array([10.])]
+                initial_conditions = [np.array([0.1]), np.array([0.5]), np.array([3.]), np.array([5.]), np.array([10.])]
             print(f"Opitimizing with {inp.shape[0]} samples...")
             
         else:
             if self.model.estim_algorithm == "doc-model":
                 # the range of doc estimation is [0, 2].
                 initial_conditions = [np.array([0.01]), np.array([1.5])]
             else:
                 # the range of ts estimation is [0, inf].
-                initial_conditions = [np.array([0.01]), np.array([5])]
+                initial_conditions = [np.array([0.1]), np.array([5])]
 
             print(f"Opitimizing with {len(inp)} samples...")
             print("Be patient, it should take a while...")
             if self.metric != "accuracy":
                 exclusive_background = True # leave the background class uncalibrated.
 
         # generate a list of length kcls, from high to low
```

### Comparing `moval-0.3.1/moval/solvers/utils.py` & `moval-0.3.2/moval/solvers/utils.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.1/moval.egg-info/PKG-INFO` & `moval-0.3.2/moval.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moval
-Version: 0.3.1
+Version: 0.3.2
 Summary: Model evaluation without manual labels
 Home-page: https://github.com/ZerojumpLine/MOVAL
 Author: Zeju Li
 Author-email: lizeju8@gmail.com
 Project-URL: Bug Tracker, https://github.com/ZerojumpLine/MOVAL/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moval Version: 0.3.1 Summary: Model evaluation
+Metadata-Version: 2.1 Name: moval Version: 0.3.2 Summary: Model evaluation
 without manual labels Home-page: https://github.com/ZerojumpLine/MOVAL Author:
 Zeju Li Author-email: lizeju8@gmail.com Project-URL: Bug Tracker, https://
 github.com/ZerojumpLine/MOVAL/issues Classifier: Development Status :: 3 -
 Alpha Classifier: Environment :: GPU :: NVIDIA CUDA Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: License :: Free
```

### Comparing `moval-0.3.1/moval.egg-info/SOURCES.txt` & `moval-0.3.2/moval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moval-0.3.1/pyproject.toml` & `moval-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moval-0.3.1/setup.cfg` & `moval-0.3.2/setup.cfg`

 * *Files identical despite different names*

