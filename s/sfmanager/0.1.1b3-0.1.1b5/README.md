# Comparing `tmp/sfmanager-0.1.1b3.tar.gz` & `tmp/sfmanager-0.1.1b5.tar.gz`

## Comparing `sfmanager-0.1.1b3.tar` & `sfmanager-0.1.1b5.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 sfmanager-0.1.1b3/sfmanager/__init__.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 sfmanager-0.1.1b3/sfmanager/app.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.1b3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.1b3/LICENSE
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sfmanager-0.1.1b3/README.md
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 sfmanager-0.1.1b3/pyproject.toml
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sfmanager-0.1.1b3/PKG-INFO
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 sfmanager-0.1.1b5/sfmanager/__init__.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 sfmanager-0.1.1b5/sfmanager/about.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 sfmanager-0.1.1b5/sfmanager/app.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.1b5/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.1b5/LICENSE
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sfmanager-0.1.1b5/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 sfmanager-0.1.1b5/pyproject.toml
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sfmanager-0.1.1b5/PKG-INFO
```

### Comparing `sfmanager-0.1.1b3/sfmanager/app.py` & `sfmanager-0.1.1b5/sfmanager/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from PIL import Image
 import os
 import shutil
-
-def what():
-	print("Hello! This is a super filemanager for python! This library is not that useful. Perhaps someday it will become great.")
+from time import sleep
 
 class FileManager:
 	filename = None
 	level = None
 
 	# Initialization func
```

### Comparing `sfmanager-0.1.1b3/.gitignore` & `sfmanager-0.1.1b5/.gitignore`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.1b3/LICENSE` & `sfmanager-0.1.1b5/LICENSE`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.1b3/PKG-INFO` & `sfmanager-0.1.1b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sfmanager
-Version: 0.1.1b3
+Version: 0.1.1b5
 Summary: This library is not that useful. Perhaps someday it will become great.
 Project-URL: Homepage, https://github.com/grandescobar/sfmanager
 Project-URL: Issues, https://github.com/grandescobar/sfmanager/issues
 Author-email: GrandTheBest <grandinfo-cm@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

