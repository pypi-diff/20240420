# Comparing `tmp/sfmanager-0.1.1b2.tar.gz` & `tmp/sfmanager-0.1.1b3.tar.gz`

## Comparing `sfmanager-0.1.1b2.tar` & `sfmanager-0.1.1b3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 sfmanager-0.1.1b2/sfmanager/__init__.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 sfmanager-0.1.1b2/sfmanager/app.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.1b2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.1b2/LICENSE
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sfmanager-0.1.1b2/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 sfmanager-0.1.1b2/pyproject.toml
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sfmanager-0.1.1b2/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 sfmanager-0.1.1b3/sfmanager/__init__.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 sfmanager-0.1.1b3/sfmanager/app.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.1b3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.1b3/LICENSE
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sfmanager-0.1.1b3/README.md
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 sfmanager-0.1.1b3/pyproject.toml
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sfmanager-0.1.1b3/PKG-INFO
```

### Comparing `sfmanager-0.1.1b2/sfmanager/app.py` & `sfmanager-0.1.1b3/sfmanager/app.py`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.1b2/.gitignore` & `sfmanager-0.1.1b3/.gitignore`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.1b2/LICENSE` & `sfmanager-0.1.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.1b2/pyproject.toml` & `sfmanager-0.1.1b3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "sfmanager"
-version = "0.1.1b2"
+version = "0.1.1b3"
 authors = [
 	{name="GrandTheBest", email="grandinfo-cm@gmail.com"},
 ]
 description = "This library is not that useful. Perhaps someday it will become great."
 readme = "README.md"
 requires-python = ">=3.10.0"
 dependencies = [
 	"Pillow>=9.0.1"
 ]
 classifiers = [
    "Programming Language :: Python :: 3",
    "License :: OSI Approved :: MIT License",
    "Operating System :: OS Independent",
 ]
-[tool.poetry.scripts]
+[project.scripts]
 sfmanager = "sfmanager:what"
 [project.urls]
 Homepage = "https://github.com/grandescobar/sfmanager"
 Issues = "https://github.com/grandescobar/sfmanager/issues"
```

### Comparing `sfmanager-0.1.1b2/PKG-INFO` & `sfmanager-0.1.1b3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sfmanager
-Version: 0.1.1b2
+Version: 0.1.1b3
 Summary: This library is not that useful. Perhaps someday it will become great.
 Project-URL: Homepage, https://github.com/grandescobar/sfmanager
 Project-URL: Issues, https://github.com/grandescobar/sfmanager/issues
 Author-email: GrandTheBest <grandinfo-cm@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

