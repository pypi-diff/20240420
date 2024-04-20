# Comparing `tmp/pyloadapi-1.0.3.tar.gz` & `tmp/pyloadapi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyloadapi-1.0.3.tar", last modified: Mon Apr 15 06:55:13 2024, max compression
+gzip compressed data, was "pyloadapi-1.1.0.tar", last modified: Sat Apr 20 05:38:45 2024, max compression
```

## Comparing `pyloadapi-1.0.3.tar` & `pyloadapi-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:55:13.332341 pyloadapi-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-15 06:55:07.000000 pyloadapi-1.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-15 06:55:07.000000 pyloadapi-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-15 06:55:13.332341 pyloadapi-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 06:55:07.000000 pyloadapi-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-15 06:55:07.000000 pyloadapi-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-15 06:55:13.332341 pyloadapi-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:55:13.328340 pyloadapi-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:55:13.332341 pyloadapi-1.0.3/src/PyLoadAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-15 06:55:13.000000 pyloadapi-1.0.3/src/PyLoadAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-15 06:55:13.000000 pyloadapi-1.0.3/src/PyLoadAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 06:55:13.000000 pyloadapi-1.0.3/src/PyLoadAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 06:55:13.000000 pyloadapi-1.0.3/src/PyLoadAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 06:55:13.000000 pyloadapi-1.0.3/src/PyLoadAPI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:55:13.332341 pyloadapi-1.0.3/src/pyloadapi/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 06:55:07.000000 pyloadapi-1.0.3/src/pyloadapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-15 06:55:07.000000 pyloadapi-1.0.3/src/pyloadapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-15 06:55:07.000000 pyloadapi-1.0.3/src/pyloadapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-15 06:55:07.000000 pyloadapi-1.0.3/src/pyloadapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:38:45.983420 pyloadapi-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-20 05:38:40.000000 pyloadapi-1.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-20 05:38:40.000000 pyloadapi-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-20 05:38:45.983420 pyloadapi-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-20 05:38:40.000000 pyloadapi-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-04-20 05:38:40.000000 pyloadapi-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-20 05:38:45.983420 pyloadapi-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:38:45.979420 pyloadapi-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:38:45.983420 pyloadapi-1.1.0/src/PyLoadAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-20 05:38:45.000000 pyloadapi-1.1.0/src/PyLoadAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-20 05:38:45.000000 pyloadapi-1.1.0/src/PyLoadAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 05:38:45.000000 pyloadapi-1.1.0/src/PyLoadAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-20 05:38:45.000000 pyloadapi-1.1.0/src/PyLoadAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 05:38:45.000000 pyloadapi-1.1.0/src/PyLoadAPI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:38:45.979420 pyloadapi-1.1.0/src/pyloadapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-20 05:38:40.000000 pyloadapi-1.1.0/src/pyloadapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8131 2024-04-20 05:38:40.000000 pyloadapi-1.1.0/src/pyloadapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-20 05:38:40.000000 pyloadapi-1.1.0/src/pyloadapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-20 05:38:40.000000 pyloadapi-1.1.0/src/pyloadapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:38:45.983420 pyloadapi-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-20 05:38:40.000000 pyloadapi-1.1.0/tests/test_api.py
```

### Comparing `pyloadapi-1.0.3/LICENSE` & `pyloadapi-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyloadapi-1.0.3/pyproject.toml` & `pyloadapi-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -136,10 +136,13 @@
 
 [tool.ruff.lint.mccabe]
 max-complexity = 25
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 testpaths = [
-    
+
     "tests",
 ]
+pythonpath = [
+  "src"
+]
```

### Comparing `pyloadapi-1.0.3/setup.cfg` & `pyloadapi-1.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = PyLoadAPI
-version = 1.0.3
+version = 1.1.0
 author = Manfred Dennerlein Rodelo
 author_email = manfred@dennerlein.name
 description = "Simple wrapper for pyLoad's API."
 long_description = file: README.md, CHANGELOG.md, LICENCE
 long_description_content_type = text/markdown
 license_files = LICENSE
 url = https://github.com/tr4nt0r/PyLoadAPI
```

