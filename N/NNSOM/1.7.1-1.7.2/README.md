# Comparing `tmp/nnsom-1.7.1.tar.gz` & `tmp/nnsom-1.7.2.tar.gz`

## Comparing `nnsom-1.7.1.tar` & `nnsom-1.7.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 nnsom-1.7.1/src/NNSOM/__init__.py
--rw-r--r--   0        0        0    77599 2020-02-02 00:00:00.000000 nnsom-1.7.1/src/NNSOM/plots.py
--rw-r--r--   0        0        0    19217 2020-02-02 00:00:00.000000 nnsom-1.7.1/src/NNSOM/som.py
--rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 nnsom-1.7.1/src/NNSOM/som_gpu.py
--rw-r--r--   0        0        0    20937 2020-02-02 00:00:00.000000 nnsom-1.7.1/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16111 2020-02-02 00:00:00.000000 nnsom-1.7.1/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.7.1/LICENSE
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 nnsom-1.7.1/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     9853 2020-02-02 00:00:00.000000 nnsom-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 nnsom-1.7.2/src/NNSOM/__init__.py
+-rw-r--r--   0        0        0    77599 2020-02-02 00:00:00.000000 nnsom-1.7.2/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    19217 2020-02-02 00:00:00.000000 nnsom-1.7.2/src/NNSOM/som.py
+-rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 nnsom-1.7.2/src/NNSOM/som_gpu.py
+-rw-r--r--   0        0        0    20937 2020-02-02 00:00:00.000000 nnsom-1.7.2/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16111 2020-02-02 00:00:00.000000 nnsom-1.7.2/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.7.2/LICENSE
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 nnsom-1.7.2/README.md
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 nnsom-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0     9914 2020-02-02 00:00:00.000000 nnsom-1.7.2/PKG-INFO
```

### Comparing `nnsom-1.7.1/src/NNSOM/plots.py` & `nnsom-1.7.2/src/NNSOM/plots.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.7.1/src/NNSOM/som.py` & `nnsom-1.7.2/src/NNSOM/som.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.7.1/src/NNSOM/som_gpu.py` & `nnsom-1.7.2/src/NNSOM/som_gpu.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.7.1/src/NNSOM/utils.py` & `nnsom-1.7.2/src/NNSOM/utils.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.7.1/.gitignore` & `nnsom-1.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.7.1/README.md` & `nnsom-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `nnsom-1.7.1/pyproject.toml` & `nnsom-1.7.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.7.1"
+version = "1.7.2"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
@@ -40,9 +40,10 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 keywords = ["SOM", "Neural Network", "Machine Learning", "Unsupervised Learning", "Clustering"]
 
 [project.urls]
+Documentation = "https://sravya-12.github.io/SOM/"
 Repository = "https://github.com/amir-jafari/SOM"
 Issues = "https://github.com/amir-jafari/SOM/issues"
```

### Comparing `nnsom-1.7.1/PKG-INFO` & `nnsom-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.7.1
+Version: 1.7.2
 Summary: A SOM package
+Project-URL: Documentation, https://sravya-12.github.io/SOM/
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
 Keywords: Clustering,Machine Learning,Neural Network,SOM,Unsupervised Learning
```

