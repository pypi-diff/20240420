# Comparing `tmp/hash_rename-0.1.0.tar.gz` & `tmp/hash_rename-0.2.0.tar.gz`

## Comparing `hash_rename-0.1.0.tar` & `hash_rename-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 hash_rename-0.1.0/src/hash_rename/__init__.py
--rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 hash_rename-0.1.0/src/hash_rename/__main__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hash_rename-0.1.0/.gitignore
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 hash_rename-0.1.0/LICENSE
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 hash_rename-0.1.0/README.md
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 hash_rename-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 hash_rename-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 hash_rename-0.2.0/src/hash_rename/__init__.py
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 hash_rename-0.2.0/src/hash_rename/__main__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hash_rename-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 hash_rename-0.2.0/LICENSE
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 hash_rename-0.2.0/README.md
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 hash_rename-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 hash_rename-0.2.0/PKG-INFO
```

### Comparing `hash_rename-0.1.0/src/hash_rename/__main__.py` & `hash_rename-0.2.0/src/hash_rename/__main__.py`

 * *Files identical despite different names*

### Comparing `hash_rename-0.1.0/.gitignore` & `hash_rename-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hash_rename-0.1.0/LICENSE` & `hash_rename-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hash_rename-0.1.0/README.md` & `hash_rename-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hash_rename-0.1.0/pyproject.toml` & `hash_rename-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hash_rename"
-version = "0.1.0"
+version = "0.2.0"
 description = "A tool to rename files in a folder to be prefixed with a hash of the file's contents"
 authors = [{ name = "DeflateAwning" }]
 license = "Unlicense"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: The Unlicense (Unlicense)",
     "Operating System :: OS Independent",
 ]
 
 [project.scripts]
-hash_rename = "src/hash_rename/__main__.py"
+hash_rename = "hash_rename.__main__:main"
```

### Comparing `hash_rename-0.1.0/PKG-INFO` & `hash_rename-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hash_rename
-Version: 0.1.0
+Version: 0.2.0
 Summary: A tool to rename files in a folder to be prefixed with a hash of the file's contents
 Author: DeflateAwning
 License-Expression: Unlicense
 License-File: LICENSE
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

