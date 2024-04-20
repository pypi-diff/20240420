# Comparing `tmp/nog642_util-0.0.0.tar.gz` & `tmp/nog642_util-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/nog642/Documents/nog642-python-utils/nog642_util/dist/.tmp-0piw9c5b/nog642_util-0.0.0.tar", last modified: Thu Apr 18 20:34:04 2024, max compression
+gzip compressed data, was "/home/nog642/Documents/nog642-python-utils/nog642_util/dist/.tmp-521ukufe/nog642_util-0.1.0.tar", last modified: Sat Apr 20 21:16:52 2024, max compression
```

## Comparing `nog642_util-0.0.0.tar` & `nog642_util-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-18 20:34:04.654862 nog642_util-0.0.0/
--rw-r--r--   0 nog642    (1000) nog642    (1000)      535 2024-04-18 20:34:04.654862 nog642_util-0.0.0/PKG-INFO
--rw-rw-r--   0 nog642    (1000) nog642    (1000)       30 2024-04-17 22:14:45.000000 nog642_util-0.0.0/README.md
--rw-rw-r--   0 nog642    (1000) nog642    (1000)      597 2024-04-18 20:33:49.000000 nog642_util-0.0.0/pyproject.toml
--rw-rw-r--   0 nog642    (1000) nog642    (1000)       38 2024-04-18 20:34:04.654862 nog642_util-0.0.0/setup.cfg
-drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-18 20:34:04.650862 nog642_util-0.0.0/src/
-drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-18 20:34:04.650862 nog642_util-0.0.0/src/nog642_util/
--rw-rw-r--   0 nog642    (1000) nog642    (1000)       54 2024-04-18 15:00:25.000000 nog642_util-0.0.0/src/nog642_util/__init__.py
-drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-18 20:34:04.654862 nog642_util-0.0.0/src/nog642_util.egg-info/
--rw-r--r--   0 nog642    (1000) nog642    (1000)      535 2024-04-18 20:34:04.000000 nog642_util-0.0.0/src/nog642_util.egg-info/PKG-INFO
--rw-rw-r--   0 nog642    (1000) nog642    (1000)      208 2024-04-18 20:34:04.000000 nog642_util-0.0.0/src/nog642_util.egg-info/SOURCES.txt
--rw-rw-r--   0 nog642    (1000) nog642    (1000)        1 2024-04-18 20:34:04.000000 nog642_util-0.0.0/src/nog642_util.egg-info/dependency_links.txt
--rw-rw-r--   0 nog642    (1000) nog642    (1000)       12 2024-04-18 20:34:04.000000 nog642_util-0.0.0/src/nog642_util.egg-info/top_level.txt
+drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-20 21:16:52.083790 nog642_util-0.1.0/
+-rw-r--r--   0 nog642    (1000) nog642    (1000)      572 2024-04-20 21:16:52.083790 nog642_util-0.1.0/PKG-INFO
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)       67 2024-04-20 21:16:31.000000 nog642_util-0.1.0/README.md
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)      597 2024-04-20 21:16:31.000000 nog642_util-0.1.0/pyproject.toml
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)       38 2024-04-20 21:16:52.083790 nog642_util-0.1.0/setup.cfg
+drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-20 21:16:52.079790 nog642_util-0.1.0/src/
+drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-20 21:16:52.079790 nog642_util-0.1.0/src/nog642_util/
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)    12853 2024-04-20 21:16:31.000000 nog642_util-0.1.0/src/nog642_util/__init__.py
+drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-20 21:16:52.083790 nog642_util-0.1.0/src/nog642_util.egg-info/
+-rw-r--r--   0 nog642    (1000) nog642    (1000)      572 2024-04-20 21:16:52.000000 nog642_util-0.1.0/src/nog642_util.egg-info/PKG-INFO
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)      238 2024-04-20 21:16:52.000000 nog642_util-0.1.0/src/nog642_util.egg-info/SOURCES.txt
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)        1 2024-04-20 21:16:52.000000 nog642_util-0.1.0/src/nog642_util.egg-info/dependency_links.txt
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)       12 2024-04-20 21:16:52.000000 nog642_util-0.1.0/src/nog642_util.egg-info/top_level.txt
+drwxrwxr-x   0 nog642    (1000) nog642    (1000)        0 2024-04-20 21:16:52.083790 nog642_util-0.1.0/tests/
+-rw-rw-r--   0 nog642    (1000) nog642    (1000)     7012 2024-04-20 21:16:31.000000 nog642_util-0.1.0/tests/test_validate_schema.py
```

### Comparing `nog642_util-0.0.0/PKG-INFO` & `nog642_util-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: nog642_util
-Version: 0.0.0
+Version: 0.1.0
 Summary: Various utilities for python.
 Author-email: nog642 <nog642.contact@gmail.com>
 Project-URL: Homepage, https://gitlab.com/nog642-org/nog642-python-utils
 Project-URL: Issues, https://gitlab.com/nog642-org/nog642-python-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # nog642_util
 
-Example README
+This package contains various utilities for Python.
```

### Comparing `nog642_util-0.0.0/pyproject.toml` & `nog642_util-0.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nog642_util"
-version = "0.0.0"
+version = "0.1.0"
 authors = [
   { name="nog642", email="nog642.contact@gmail.com" },
 ]
 description = "Various utilities for python."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `nog642_util-0.0.0/src/nog642_util.egg-info/PKG-INFO` & `nog642_util-0.1.0/src/nog642_util.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: nog642_util
-Version: 0.0.0
+Version: 0.1.0
 Summary: Various utilities for python.
 Author-email: nog642 <nog642.contact@gmail.com>
 Project-URL: Homepage, https://gitlab.com/nog642-org/nog642-python-utils
 Project-URL: Issues, https://gitlab.com/nog642-org/nog642-python-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # nog642_util
 
-Example README
+This package contains various utilities for Python.
```

