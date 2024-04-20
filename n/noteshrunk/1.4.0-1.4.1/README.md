# Comparing `tmp/noteshrunk-1.4.0.tar.gz` & `tmp/noteshrunk-1.4.1.tar.gz`

## Comparing `noteshrunk-1.4.0.tar` & `noteshrunk-1.4.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 noteshrunk-1.4.0/CHANGELOG.md
--rwxr-xr-x   0        0        0    25034 2020-02-02 00:00:00.000000 noteshrunk-1.4.0/src/noteshrunk.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 noteshrunk-1.4.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 noteshrunk-1.4.0/LICENSE
--rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 noteshrunk-1.4.0/README.md
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 noteshrunk-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    47774 2020-02-02 00:00:00.000000 noteshrunk-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 noteshrunk-1.4.1/CHANGELOG.md
+-rwxr-xr-x   0        0        0    25034 2020-02-02 00:00:00.000000 noteshrunk-1.4.1/src/noteshrunk.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 noteshrunk-1.4.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 noteshrunk-1.4.1/LICENSE
+-rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 noteshrunk-1.4.1/README.md
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 noteshrunk-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0    47774 2020-02-02 00:00:00.000000 noteshrunk-1.4.1/PKG-INFO
```

### Comparing `noteshrunk-1.4.0/src/noteshrunk.py` & `noteshrunk-1.4.1/src/noteshrunk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
-VERSION = '1.4.0'
+VERSION = '1.4.1'
 
 import argparse
 from concurrent.futures import ThreadPoolExecutor
 import os
 from pathlib import Path
 import random
 import re
```

### Comparing `noteshrunk-1.4.0/.gitignore` & `noteshrunk-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `noteshrunk-1.4.0/LICENSE` & `noteshrunk-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `noteshrunk-1.4.0/README.md` & `noteshrunk-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `noteshrunk-1.4.0/pyproject.toml` & `noteshrunk-1.4.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "noteshrunk"
-version = "1.4.0"
+version = "1.4.1"
 description = "Document Color Palette Compression"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
 authors = [
     {name = "suuuehgi"}
 ]
```

### Comparing `noteshrunk-1.4.0/PKG-INFO` & `noteshrunk-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: noteshrunk
-Version: 1.4.0
+Version: 1.4.1
 Summary: Document Color Palette Compression
 Project-URL: Homepage, https://github.com/suuuehgi/noteshrunk
 Project-URL: Issues, https://github.com/suuuehgi/noteshrunk/issues
 Author: suuuehgi
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

