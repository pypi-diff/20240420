# Comparing `tmp/wdl-lsp-0.0.84.tar.gz` & `tmp/wdl-lsp-0.0.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wdl-lsp-0.0.84.tar", last modified: Fri Apr 19 22:27:56 2024, max compression
+gzip compressed data, was "wdl-lsp-0.0.85.tar", last modified: Fri Apr 19 22:37:52 2024, max compression
```

## Comparing `wdl-lsp-0.0.84.tar` & `wdl-lsp-0.0.85.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:27:56.895051 wdl-lsp-0.0.84/
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-19 22:27:56.895051 wdl-lsp-0.0.84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 22:27:56.895051 wdl-lsp-0.0.84/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-19 22:27:52.000000 wdl-lsp-0.0.84/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:27:56.895051 wdl-lsp-0.0.84/wdl_lsp/
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-19 22:27:52.000000 wdl-lsp-0.0.84/wdl_lsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-19 22:27:52.000000 wdl-lsp-0.0.84/wdl_lsp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17170 2024-04-19 22:27:52.000000 wdl-lsp-0.0.84/wdl_lsp/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:27:56.895051 wdl-lsp-0.0.84/wdl_lsp/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-19 22:27:52.000000 wdl-lsp-0.0.84/wdl_lsp/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:27:56.895051 wdl-lsp-0.0.84/wdl_lsp/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-19 22:27:52.000000 wdl-lsp-0.0.84/wdl_lsp/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-19 22:27:52.000000 wdl-lsp-0.0.84/wdl_lsp/tests/unit/test_features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:27:56.895051 wdl-lsp-0.0.84/wdl_lsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-19 22:27:56.000000 wdl-lsp-0.0.84/wdl_lsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-19 22:27:56.000000 wdl-lsp-0.0.84/wdl_lsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 22:27:56.000000 wdl-lsp-0.0.84/wdl_lsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 22:27:56.000000 wdl-lsp-0.0.84/wdl_lsp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 22:27:56.000000 wdl-lsp-0.0.84/wdl_lsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 22:27:56.000000 wdl-lsp-0.0.84/wdl_lsp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:37:52.662180 wdl-lsp-0.0.85/
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-19 22:37:52.662180 wdl-lsp-0.0.85/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-19 22:37:47.000000 wdl-lsp-0.0.85/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 22:37:52.662180 wdl-lsp-0.0.85/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-19 22:37:47.000000 wdl-lsp-0.0.85/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:37:52.658180 wdl-lsp-0.0.85/wdl_lsp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-19 22:37:47.000000 wdl-lsp-0.0.85/wdl_lsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-19 22:37:47.000000 wdl-lsp-0.0.85/wdl_lsp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17170 2024-04-19 22:37:47.000000 wdl-lsp-0.0.85/wdl_lsp/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:37:52.658180 wdl-lsp-0.0.85/wdl_lsp/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-19 22:37:47.000000 wdl-lsp-0.0.85/wdl_lsp/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:37:52.658180 wdl-lsp-0.0.85/wdl_lsp/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-19 22:37:47.000000 wdl-lsp-0.0.85/wdl_lsp/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-19 22:37:47.000000 wdl-lsp-0.0.85/wdl_lsp/tests/unit/test_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:37:52.658180 wdl-lsp-0.0.85/wdl_lsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-19 22:37:52.000000 wdl-lsp-0.0.85/wdl_lsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-19 22:37:52.000000 wdl-lsp-0.0.85/wdl_lsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 22:37:52.000000 wdl-lsp-0.0.85/wdl_lsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 22:37:52.000000 wdl-lsp-0.0.85/wdl_lsp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 22:37:52.000000 wdl-lsp-0.0.85/wdl_lsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 22:37:52.000000 wdl-lsp-0.0.85/wdl_lsp.egg-info/top_level.txt
```

### Comparing `wdl-lsp-0.0.84/PKG-INFO` & `wdl-lsp-0.0.85/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wdl-lsp
-Version: 0.0.84
+Version: 0.0.85
 Summary: Language Server Protocol (LSP) implementation for Workflow Definition Language (WDL)
 Home-page: https://github.com/broadinstitute/wdl-ide
 Author: Broad Institute
 License: BSD 3-clause "New" or "Revised" License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Interpreters
```

### Comparing `wdl-lsp-0.0.84/setup.py` & `wdl-lsp-0.0.85/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from setuptools import find_packages, setup
 
 cwd = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(cwd, '..', 'README.md'), encoding='utf-8') as f:
+with open(os.path.join(cwd, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='wdl-lsp',
     author='Broad Institute',
     description='Language Server Protocol (LSP) implementation for Workflow Definition Language (WDL)',
     long_description=long_description,
@@ -35,14 +35,14 @@
     ],
     use_scm_version={
         'root': '..',
         'relative_to': __file__,
     },
     install_requires=[
         'cromwell-tools == 2.3.0',
-        "miniwdl >= 1.1.5",
+        'miniwdl >= 1.1.5',
         'pygls == 0.8.1',
     ],
     entry_points={
         'console_scripts': ['wdl-lsp = wdl_lsp.__main__:main'],
     },
 )
```

### Comparing `wdl-lsp-0.0.84/wdl_lsp/__init__.py` & `wdl-lsp-0.0.85/wdl_lsp/__init__.py`

 * *Files identical despite different names*

### Comparing `wdl-lsp-0.0.84/wdl_lsp/__main__.py` & `wdl-lsp-0.0.85/wdl_lsp/__main__.py`

 * *Files identical despite different names*

### Comparing `wdl-lsp-0.0.84/wdl_lsp/server.py` & `wdl-lsp-0.0.85/wdl_lsp/server.py`

 * *Files identical despite different names*

### Comparing `wdl-lsp-0.0.84/wdl_lsp/tests/__init__.py` & `wdl-lsp-0.0.85/wdl_lsp/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `wdl-lsp-0.0.84/wdl_lsp/tests/unit/__init__.py` & `wdl-lsp-0.0.85/wdl_lsp/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `wdl-lsp-0.0.84/wdl_lsp/tests/unit/test_features.py` & `wdl-lsp-0.0.85/wdl_lsp/tests/unit/test_features.py`

 * *Files identical despite different names*

### Comparing `wdl-lsp-0.0.84/wdl_lsp.egg-info/PKG-INFO` & `wdl-lsp-0.0.85/wdl_lsp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wdl-lsp
-Version: 0.0.84
+Version: 0.0.85
 Summary: Language Server Protocol (LSP) implementation for Workflow Definition Language (WDL)
 Home-page: https://github.com/broadinstitute/wdl-ide
 Author: Broad Institute
 License: BSD 3-clause "New" or "Revised" License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Interpreters
```

