# Comparing `tmp/sfmanager-0.1.1b0.tar.gz` & `tmp/sfmanager-0.1.1b1.tar.gz`

## Comparing `sfmanager-0.1.1b0.tar` & `sfmanager-0.1.1b1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 sfmanager-0.1.1b0/sfmanager/__init__.py
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 sfmanager-0.1.1b0/sfmanager/app.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.1b0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.1b0/LICENSE
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sfmanager-0.1.1b0/README.md
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 sfmanager-0.1.1b0/pyproject.toml
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sfmanager-0.1.1b0/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 sfmanager-0.1.1b1/sfmanager/__init__.py
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 sfmanager-0.1.1b1/sfmanager/app.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.1b1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.1b1/LICENSE
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sfmanager-0.1.1b1/README.md
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 sfmanager-0.1.1b1/pyproject.toml
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sfmanager-0.1.1b1/PKG-INFO
```

### Comparing `sfmanager-0.1.1b0/sfmanager/app.py` & `sfmanager-0.1.1b1/sfmanager/app.py`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.1b0/.gitignore` & `sfmanager-0.1.1b1/.gitignore`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.1b0/LICENSE` & `sfmanager-0.1.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.1b0/pyproject.toml` & `sfmanager-0.1.1b1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "sfmanager"
-version = "0.1.1-beta"
+version = "0.1.1b1"
 authors = [
 	{name="GrandTheBest", email="grandinfo-cm@gmail.com"},
 ]
 description = "This library is not that useful. Perhaps someday it will become great."
 readme = "README.md"
 requires-python = ">=3.10.0"
 dependencies = [
```

### Comparing `sfmanager-0.1.1b0/PKG-INFO` & `sfmanager-0.1.1b1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sfmanager
-Version: 0.1.1b0
+Version: 0.1.1b1
 Summary: This library is not that useful. Perhaps someday it will become great.
 Project-URL: Homepage, https://github.com/grandescobar/sfmanager
 Project-URL: Issues, https://github.com/grandescobar/sfmanager/issues
 Author-email: GrandTheBest <grandinfo-cm@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

