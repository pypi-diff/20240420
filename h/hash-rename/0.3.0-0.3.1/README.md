# Comparing `tmp/hash_rename-0.3.0.tar.gz` & `tmp/hash_rename-0.3.1.tar.gz`

## Comparing `hash_rename-0.3.0.tar` & `hash_rename-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hash_rename-0.3.0/src/hash_rename/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 hash_rename-0.3.0/src/hash_rename/__main__.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 hash_rename-0.3.0/src/hash_rename/cli.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 hash_rename-0.3.0/src/hash_rename/core.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hash_rename-0.3.0/.gitignore
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 hash_rename-0.3.0/LICENSE
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 hash_rename-0.3.0/README.md
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 hash_rename-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 hash_rename-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hash_rename-0.3.1/src/hash_rename/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 hash_rename-0.3.1/src/hash_rename/__main__.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 hash_rename-0.3.1/src/hash_rename/cli.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 hash_rename-0.3.1/src/hash_rename/core.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hash_rename-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 hash_rename-0.3.1/LICENSE
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 hash_rename-0.3.1/README.md
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 hash_rename-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 hash_rename-0.3.1/PKG-INFO
```

### Comparing `hash_rename-0.3.0/src/hash_rename/cli.py` & `hash_rename-0.3.1/src/hash_rename/cli.py`

 * *Files identical despite different names*

### Comparing `hash_rename-0.3.0/src/hash_rename/core.py` & `hash_rename-0.3.1/src/hash_rename/core.py`

 * *Files identical despite different names*

### Comparing `hash_rename-0.3.0/.gitignore` & `hash_rename-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hash_rename-0.3.0/LICENSE` & `hash_rename-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hash_rename-0.3.0/README.md` & `hash_rename-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `hash_rename-0.3.0/PKG-INFO` & `hash_rename-0.3.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 Metadata-Version: 2.3
 Name: hash_rename
-Version: 0.3.0
+Version: 0.3.1
 Summary: A tool to rename files in a folder to be prefixed with a hash of the file's contents
+Project-URL: homepage, https://github.com/DeflateAwning/hash_rename
+Project-URL: repository, https://github.com/DeflateAwning/hash_rename
+Project-URL: issues, https://github.com/DeflateAwning/hash_rename/issues
+Project-URL: license, https://github.com/DeflateAwning/hash_rename/blob/main/LICENSE
+Project-URL: pypi, https://pypi.org/project/hash-rename
 Author: DeflateAwning
 License-Expression: Unlicense
 License-File: LICENSE
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

