# Comparing `tmp/envarify-1.1.1.tar.gz` & `tmp/envarify-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envarify-1.1.1.tar", last modified: Sat Mar 30 12:22:29 2024, max compression
+gzip compressed data, was "envarify-1.1.2.tar", last modified: Sat Apr 20 10:41:44 2024, max compression
```

## Comparing `envarify-1.1.1.tar` & `envarify-1.1.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:22:29.817846 envarify-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-30 12:22:17.000000 envarify-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-03-30 12:22:29.817846 envarify-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-03-30 12:22:17.000000 envarify-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-30 12:22:17.000000 envarify-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-03-30 12:22:29.817846 envarify-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-30 12:22:17.000000 envarify-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:22:29.809846 envarify-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:22:29.813846 envarify-1.1.1/src/envarify/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-30 12:22:17.000000 envarify-1.1.1/src/envarify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-03-30 12:22:17.000000 envarify-1.1.1/src/envarify/envarify.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-30 12:22:17.000000 envarify-1.1.1/src/envarify/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-03-30 12:22:17.000000 envarify-1.1.1/src/envarify/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-03-30 12:22:17.000000 envarify-1.1.1/src/envarify/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-30 12:22:29.000000 envarify-1.1.1/src/envarify/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:22:29.817846 envarify-1.1.1/src/envarify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-03-30 12:22:29.000000 envarify-1.1.1/src/envarify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-30 12:22:29.000000 envarify-1.1.1/src/envarify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 12:22:29.000000 envarify-1.1.1/src/envarify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-30 12:22:29.000000 envarify-1.1.1/src/envarify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-30 12:22:29.000000 envarify-1.1.1/src/envarify.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:22:29.813846 envarify-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-03-30 12:22:17.000000 envarify-1.1.1/tests/test_envarify.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-03-30 12:22:17.000000 envarify-1.1.1/tests/test_inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-03-30 12:22:17.000000 envarify-1.1.1/tests/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:41:44.389621 envarify-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 10:41:36.000000 envarify-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-20 10:41:44.389621 envarify-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-20 10:41:36.000000 envarify-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-20 10:41:36.000000 envarify-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-20 10:41:44.389621 envarify-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-20 10:41:36.000000 envarify-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:41:44.385621 envarify-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:41:44.385621 envarify-1.1.2/src/envarify/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-20 10:41:36.000000 envarify-1.1.2/src/envarify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-04-20 10:41:36.000000 envarify-1.1.2/src/envarify/envarify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-20 10:41:36.000000 envarify-1.1.2/src/envarify/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-20 10:41:36.000000 envarify-1.1.2/src/envarify/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-20 10:41:36.000000 envarify-1.1.2/src/envarify/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 10:41:36.000000 envarify-1.1.2/src/envarify/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-20 10:41:44.000000 envarify-1.1.2/src/envarify/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:41:44.389621 envarify-1.1.2/src/envarify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-20 10:41:44.000000 envarify-1.1.2/src/envarify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-20 10:41:44.000000 envarify-1.1.2/src/envarify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 10:41:44.000000 envarify-1.1.2/src/envarify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-20 10:41:44.000000 envarify-1.1.2/src/envarify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 10:41:44.000000 envarify-1.1.2/src/envarify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:41:44.389621 envarify-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-20 10:41:36.000000 envarify-1.1.2/tests/test_envarify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-20 10:41:36.000000 envarify-1.1.2/tests/test_inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-20 10:41:36.000000 envarify-1.1.2/tests/test_parse.py
```

### Comparing `envarify-1.1.1/LICENSE` & `envarify-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `envarify-1.1.1/PKG-INFO` & `envarify-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envarify
-Version: 1.1.1
+Version: 1.1.2
 Summary: Environment variables parsing and validation using python type hints
 Home-page: https://github.com/vadimtitov/envarify
 Author: Vadim Titov
 Author-email: titov.hse@gmail.com
 Project-URL: Bug Tracker, https://github.com/vadimtitov/envarify/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `envarify-1.1.1/README.md` & `envarify-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `envarify-1.1.1/pyproject.toml` & `envarify-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `envarify-1.1.1/setup.cfg` & `envarify-1.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `envarify-1.1.1/setup.py` & `envarify-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `envarify-1.1.1/src/envarify/envarify.py` & `envarify-1.1.2/src/envarify/envarify.py`

 * *Files identical despite different names*

### Comparing `envarify-1.1.1/src/envarify/errors.py` & `envarify-1.1.2/src/envarify/errors.py`

 * *Files identical despite different names*

### Comparing `envarify-1.1.1/src/envarify/inspect.py` & `envarify-1.1.2/src/envarify/inspect.py`

 * *Files identical despite different names*

### Comparing `envarify-1.1.1/src/envarify/parse.py` & `envarify-1.1.2/src/envarify/parse.py`

 * *Files identical despite different names*

### Comparing `envarify-1.1.1/src/envarify.egg-info/PKG-INFO` & `envarify-1.1.2/src/envarify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envarify
-Version: 1.1.1
+Version: 1.1.2
 Summary: Environment variables parsing and validation using python type hints
 Home-page: https://github.com/vadimtitov/envarify
 Author: Vadim Titov
 Author-email: titov.hse@gmail.com
 Project-URL: Bug Tracker, https://github.com/vadimtitov/envarify/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `envarify-1.1.1/tests/test_envarify.py` & `envarify-1.1.2/tests/test_envarify.py`

 * *Files identical despite different names*

### Comparing `envarify-1.1.1/tests/test_inspect.py` & `envarify-1.1.2/tests/test_inspect.py`

 * *Files identical despite different names*

### Comparing `envarify-1.1.1/tests/test_parse.py` & `envarify-1.1.2/tests/test_parse.py`

 * *Files identical despite different names*

