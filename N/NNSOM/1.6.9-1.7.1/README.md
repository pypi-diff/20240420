# Comparing `tmp/nnsom-1.6.9.tar.gz` & `tmp/nnsom-1.7.1.tar.gz`

## Comparing `nnsom-1.6.9.tar` & `nnsom-1.7.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 nnsom-1.6.9/src/NNSOM/__init__.py
--rw-r--r--   0        0        0    77599 2020-02-02 00:00:00.000000 nnsom-1.6.9/src/NNSOM/plots.py
--rw-r--r--   0        0        0    19217 2020-02-02 00:00:00.000000 nnsom-1.6.9/src/NNSOM/som.py
--rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 nnsom-1.6.9/src/NNSOM/som_gpu.py
--rw-r--r--   0        0        0    20937 2020-02-02 00:00:00.000000 nnsom-1.6.9/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16111 2020-02-02 00:00:00.000000 nnsom-1.6.9/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.6.9/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.6.9/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.6.9/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.6.9/PKG-INFO
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 nnsom-1.7.1/src/NNSOM/__init__.py
+-rw-r--r--   0        0        0    77599 2020-02-02 00:00:00.000000 nnsom-1.7.1/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    19217 2020-02-02 00:00:00.000000 nnsom-1.7.1/src/NNSOM/som.py
+-rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 nnsom-1.7.1/src/NNSOM/som_gpu.py
+-rw-r--r--   0        0        0    20937 2020-02-02 00:00:00.000000 nnsom-1.7.1/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16111 2020-02-02 00:00:00.000000 nnsom-1.7.1/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.7.1/LICENSE
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 nnsom-1.7.1/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     9853 2020-02-02 00:00:00.000000 nnsom-1.7.1/PKG-INFO
```

### Comparing `nnsom-1.6.9/src/NNSOM/plots.py` & `nnsom-1.7.1/src/NNSOM/plots.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.6.9/src/NNSOM/som.py` & `nnsom-1.7.1/src/NNSOM/som.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.6.9/src/NNSOM/som_gpu.py` & `nnsom-1.7.1/src/NNSOM/som_gpu.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.6.9/src/NNSOM/utils.py` & `nnsom-1.7.1/src/NNSOM/utils.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.6.9/.gitignore` & `nnsom-1.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.6.9/pyproject.toml` & `nnsom-1.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.6.9"
+version = "1.7.1"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

