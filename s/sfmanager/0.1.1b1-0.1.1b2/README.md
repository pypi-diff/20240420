# Comparing `tmp/sfmanager-0.1.1b1.tar.gz` & `tmp/sfmanager-0.1.1b2.tar.gz`

## Comparing `sfmanager-0.1.1b1.tar` & `sfmanager-0.1.1b2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 sfmanager-0.1.1b1/sfmanager/__init__.py
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 sfmanager-0.1.1b1/sfmanager/app.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.1b1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.1b1/LICENSE
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sfmanager-0.1.1b1/README.md
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 sfmanager-0.1.1b1/pyproject.toml
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sfmanager-0.1.1b1/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 sfmanager-0.1.1b2/sfmanager/__init__.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 sfmanager-0.1.1b2/sfmanager/app.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.1b2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.1b2/LICENSE
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sfmanager-0.1.1b2/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 sfmanager-0.1.1b2/pyproject.toml
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sfmanager-0.1.1b2/PKG-INFO
```

### Comparing `sfmanager-0.1.1b1/sfmanager/app.py` & `sfmanager-0.1.1b2/sfmanager/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from PIL import Image
 import os
 import shutil
 
+def what():
+	print("Hello! This is a super filemanager for python! This library is not that useful. Perhaps someday it will become great.")
+
 class FileManager:
 	filename = None
 	level = None
 
 	# Initialization func
 
 	def __init__(self, filename, level):
```

### Comparing `sfmanager-0.1.1b1/.gitignore` & `sfmanager-0.1.1b2/.gitignore`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.1b1/LICENSE` & `sfmanager-0.1.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.1b1/PKG-INFO` & `sfmanager-0.1.1b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sfmanager
-Version: 0.1.1b1
+Version: 0.1.1b2
 Summary: This library is not that useful. Perhaps someday it will become great.
 Project-URL: Homepage, https://github.com/grandescobar/sfmanager
 Project-URL: Issues, https://github.com/grandescobar/sfmanager/issues
 Author-email: GrandTheBest <grandinfo-cm@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

