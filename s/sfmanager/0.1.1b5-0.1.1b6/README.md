# Comparing `tmp/sfmanager-0.1.1b5.tar.gz` & `tmp/sfmanager-0.1.1b6.tar.gz`

## Comparing `sfmanager-0.1.1b5.tar` & `sfmanager-0.1.1b6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 sfmanager-0.1.1b5/sfmanager/__init__.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 sfmanager-0.1.1b5/sfmanager/about.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 sfmanager-0.1.1b5/sfmanager/app.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.1b5/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.1b5/LICENSE
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sfmanager-0.1.1b5/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 sfmanager-0.1.1b5/pyproject.toml
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sfmanager-0.1.1b5/PKG-INFO
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 sfmanager-0.1.1b6/sfmanager/__init__.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 sfmanager-0.1.1b6/sfmanager/about.py
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 sfmanager-0.1.1b6/sfmanager/app.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.1b6/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.1b6/LICENSE
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sfmanager-0.1.1b6/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 sfmanager-0.1.1b6/pyproject.toml
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sfmanager-0.1.1b6/PKG-INFO
```

### Comparing `sfmanager-0.1.1b5/sfmanager/about.py` & `sfmanager-0.1.1b6/sfmanager/about.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from time import sleep
+
 def whatIsIt():
 	print("Hello dear user!")
 	sleep(1)
 	print("Thanks for download my library!")
 	sleep(2)
 	print("Homepage on github: https://github.com/grandescobar/sfmanager")
 	sleep(2)
```

### Comparing `sfmanager-0.1.1b5/sfmanager/app.py` & `sfmanager-0.1.1b6/sfmanager/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from PIL import Image
 import os
 import shutil
-from time import sleep
 
 class FileManager:
 	filename = None
 	level = None
 
 	# Initialization func
```

### Comparing `sfmanager-0.1.1b5/.gitignore` & `sfmanager-0.1.1b6/.gitignore`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.1b5/LICENSE` & `sfmanager-0.1.1b6/LICENSE`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.1b5/pyproject.toml` & `sfmanager-0.1.1b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "sfmanager"
-version = "0.1.1b5"
+version = "0.1.1b6"
 authors = [
 	{name="GrandTheBest", email="grandinfo-cm@gmail.com"},
 ]
 description = "This library is not that useful. Perhaps someday it will become great."
 readme = "README.md"
 requires-python = ">=3.10.0"
 dependencies = [
```

### Comparing `sfmanager-0.1.1b5/PKG-INFO` & `sfmanager-0.1.1b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sfmanager
-Version: 0.1.1b5
+Version: 0.1.1b6
 Summary: This library is not that useful. Perhaps someday it will become great.
 Project-URL: Homepage, https://github.com/grandescobar/sfmanager
 Project-URL: Issues, https://github.com/grandescobar/sfmanager/issues
 Author-email: GrandTheBest <grandinfo-cm@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

