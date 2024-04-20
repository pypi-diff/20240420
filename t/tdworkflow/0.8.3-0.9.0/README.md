# Comparing `tmp/tdworkflow-0.8.3.tar.gz` & `tmp/tdworkflow-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdworkflow-0.8.3.tar", last modified: Wed Apr 17 23:16:22 2024, max compression
+gzip compressed data, was "tdworkflow-0.9.0.tar", last modified: Sat Apr 20 19:20:14 2024, max compression
```

## Comparing `tdworkflow-0.8.3.tar` & `tdworkflow-0.9.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.682745 tdworkflow-0.8.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.674745 tdworkflow-0.8.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.674745 tdworkflow-0.8.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/.github/workflows/pythonapp.yml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18112 2024-04-17 23:16:22.682745 tdworkflow-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.674745 tdworkflow-0.8.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.678745 tdworkflow-0.8.3/docs/references/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/docs/references/client.rst
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/docs/references/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/docs/references/misc.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/docs/references/model.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 23:16:22.682745 tdworkflow-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.678745 tdworkflow-0.8.3/tdworkflow/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/attempt.py
--rw-r--r--   0 runner    (1001) docker     (127)    39160 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/project.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/revision.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tdworkflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.682745 tdworkflow-0.8.3/tdworkflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18112 2024-04-17 23:16:22.000000 tdworkflow-0.8.3/tdworkflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-17 23:16:22.000000 tdworkflow-0.8.3/tdworkflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 23:16:22.000000 tdworkflow-0.8.3/tdworkflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-17 23:16:22.000000 tdworkflow-0.8.3/tdworkflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 23:16:22.000000 tdworkflow-0.8.3/tdworkflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.678745 tdworkflow-0.8.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.674745 tdworkflow-0.8.3/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.678745 tdworkflow-0.8.3/tests/resources/sample_project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tests/resources/sample_project/.digdag
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.678745 tdworkflow-0.8.3/tests/resources/sample_project/ignore_dir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tests/resources/sample_project/ignore_dir/dummy
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tests/resources/sample_project/main.dig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.682745 tdworkflow-0.8.3/tests/resources/sample_project/py_scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:22.682745 tdworkflow-0.8.3/tests/resources/sample_project/py_scripts/__ignoredir__/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tests/resources/sample_project/py_scripts/__ignoredir__/dummy
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tests/resources/sample_project/py_scripts/exec.py
--rw-r--r--   0 runner    (1001) docker     (127)    24529 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-17 23:16:12.000000 tdworkflow-0.8.3/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:20:14.491861 tdworkflow-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:20:14.479861 tdworkflow-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:20:14.483861 tdworkflow-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/.github/workflows/pythonapp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18163 2024-04-20 19:20:14.491861 tdworkflow-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:20:14.483861 tdworkflow-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:20:14.483861 tdworkflow-0.9.0/docs/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/docs/references/client.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/docs/references/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/docs/references/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/docs/references/model.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 19:20:14.491861 tdworkflow-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:20:14.487861 tdworkflow-0.9.0/tdworkflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/tdworkflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/tdworkflow/attempt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40012 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/tdworkflow/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/tdworkflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/tdworkflow/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/tdworkflow/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/tdworkflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/tdworkflow/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/tdworkflow/revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/tdworkflow/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/tdworkflow/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/tdworkflow/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/tdworkflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/tdworkflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:20:14.487861 tdworkflow-0.9.0/tdworkflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18163 2024-04-20 19:20:14.000000 tdworkflow-0.9.0/tdworkflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-20 19:20:14.000000 tdworkflow-0.9.0/tdworkflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 19:20:14.000000 tdworkflow-0.9.0/tdworkflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-20 19:20:14.000000 tdworkflow-0.9.0/tdworkflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-20 19:20:14.000000 tdworkflow-0.9.0/tdworkflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:20:14.487861 tdworkflow-0.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:20:14.479861 tdworkflow-0.9.0/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:20:14.487861 tdworkflow-0.9.0/tests/resources/sample_project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/tests/resources/sample_project/.digdag
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:20:14.487861 tdworkflow-0.9.0/tests/resources/sample_project/ignore_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/tests/resources/sample_project/ignore_dir/dummy
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/tests/resources/sample_project/main.dig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:20:14.487861 tdworkflow-0.9.0/tests/resources/sample_project/py_scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:20:14.487861 tdworkflow-0.9.0/tests/resources/sample_project/py_scripts/__ignoredir__/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/tests/resources/sample_project/py_scripts/__ignoredir__/dummy
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/tests/resources/sample_project/py_scripts/exec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24529 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-20 19:20:01.000000 tdworkflow-0.9.0/tests/test_util.py
```

### Comparing `tdworkflow-0.8.3/.github/workflows/pythonapp.yml` & `tdworkflow-0.9.0/.github/workflows/pythonapp.yml`

 * *Files 27% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 on: [push]
 
 jobs:
   build:
     strategy:
       matrix:
-        python-version: ['3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
         os: [ubuntu-latest, windows-latest]
     runs-on: ${{ matrix.os }}
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
```

### Comparing `tdworkflow-0.8.3/.github/workflows/pythonpublish.yml` & `tdworkflow-0.9.0/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.3/.gitignore` & `tdworkflow-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.3/.readthedocs.yml` & `tdworkflow-0.9.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.3/CHANGES.rst` & `tdworkflow-0.9.0/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.3/LICENSE` & `tdworkflow-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.3/PKG-INFO` & `tdworkflow-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdworkflow
-Version: 0.8.3
+Version: 0.9.0
 Summary: Unofficial Treasure Workflow API client
 Author-email: Aki Ariga <chezou@gmail.com>
 Maintainer-email: Aki Ariga <chezou@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -216,14 +216,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Database
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: mypy-extensions
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `tdworkflow-0.8.3/README.rst` & `tdworkflow-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.3/docs/Makefile` & `tdworkflow-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.3/docs/conf.py` & `tdworkflow-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.3/docs/make.bat` & `tdworkflow-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.3/docs/references/model.rst` & `tdworkflow-0.9.0/docs/references/model.rst`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.3/pyproject.toml` & `tdworkflow-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
+requires = ["setuptools>=64", "setuptools_scm>=8"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tdworkflow"
 description = "Unofficial Treasure Workflow API client"
 authors = [
   {name = "Aki Ariga", email = "chezou@gmail.com"}
@@ -20,14 +20,15 @@
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Database",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 requires-python = ">=3.8"
 dependencies = [
   "requests",
   "mypy-extensions",
 ]
 dynamic = ["version"]
```

### Comparing `tdworkflow-0.8.3/tdworkflow/attempt.py` & `tdworkflow-0.9.0/tdworkflow/attempt.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.3/tdworkflow/client.py` & `tdworkflow-0.9.0/tdworkflow/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from .attempt import Attempt
 from .log import LogFile
 from .project import Project
 from .revision import Revision
 from .schedule import Schedule, ScheduleAttempt
 from .session import Session
 from .task import Task
-from .util import archive_files, to_iso8601
+from .util import archive_files, to_iso8601, to_iso_instant
 from .workflow import Workflow
 
 logger = logging.getLogger(__name__)
 
 GetResponse = Union[Dict[str, Any], bytes]
 PostResponse = Optional[Union[Dict[str, Any], bytes]]
 PutResponse = Optional[Dict[str, Any]]
@@ -98,15 +98,15 @@
         [str, DefaultArg(Params, "params"), DefaultArg(bool, "content")], GetResponse
     ]
     put: Callable[
         [
             str,
             DefaultArg(DataType, "data"),
             DefaultArg(Dict[str, Any], "_json"),
-            DefaultArg(Dict[str, str], "params"),
+            DefaultArg(Dict[str, Union[str, List[str]]], "params"),
         ],
         PutResponse,
     ]
     delete: Callable[[Any], DeleteResponse]
 
     def project(self, project: Union[int, Project]) -> Project:
         """Get a project
@@ -189,30 +189,45 @@
         else:
             return []
 
     def create_project(
         self,
         project_name: str,
         target_dir: str,
+        schedule_from: Optional[datetime] = None,
+        clear_schedules: Optional[List[str]] = None,
+        clear_schedule_all: Optional[bool] = None,
         exclude_patterns: Optional[List[str]] = None,
         revision: Optional[str] = None,
     ) -> Project:
         """Create a new project
 
         :param project_name: Project name
         :param target_dir: Target directory name
+        :param schedule_from: Start scheduling of new workflows from the given time instead of current time
+        :param clear_schedules: Clear last_session_time info for schedules of the for the given workflow names
+        :param clear_schedule_all: Clear last_session_time info for all schedules
         :param exclude_patterns: Exclude file patterns. They are treated as regexp
                                  patterns.
                                  default: ["venv", ".venv", "__pycache__", ".egg-info",\
                                   ".digdag", ".pyc"] + dot files
         :param revision: Revision name
         :return:
         """
         revision = revision or str(uuid.uuid4())
-        params = {"project": project_name, "revision": revision}
+        params: Dict[str, Union[str, List[str]]] = {
+            "project": project_name,
+            "revision": revision,
+        }
+        if schedule_from:
+            params["schedule_from"] = to_iso_instant(schedule_from)
+        if clear_schedules:
+            params["clear_schedule"] = clear_schedules
+        if clear_schedule_all:
+            params["clear_schedule_all"] = "true"
 
         default_excludes = [
             "venv",
             ".venv",
             "__pycache__",
             ".egg-info",
             ".digdag",
@@ -448,15 +463,15 @@
 class AttemptAPI:
     get: Callable[[str, DefaultArg(Params, "params")], GetResponse]
     put: Callable[
         [
             str,
             DefaultArg(DataType, "data"),
             DefaultArg(Dict[str, Any], "_json"),
-            DefaultArg(Dict[str, str], "params"),
+            DefaultArg(Dict[str, Union[str, List[str]]], "params"),
         ],
         PutResponse,
     ]
     post: Callable[
         [str, DefaultArg(Any, "body"), DefaultArg(bool, "content")], PostResponse
     ]
 
@@ -1034,15 +1049,15 @@
         return None
 
     def put(
         self,
         path: str,
         data: Optional[DataType] = None,
         _json: Optional[Dict[str, Any]] = None,
-        params: Optional[Dict[str, str]] = None,
+        params: Optional[Dict[str, Union[str, List[str]]]] = None,
     ) -> PutResponse:
         """PUT operator for REST API
 
         :param path: Treasure Workflow API path
         :type path: str
         :param data: Content body
         :type data: Optional[str, Union[Dict, List[Tuple], BinaryIO]], optional
```

### Comparing `tdworkflow-0.8.3/tdworkflow/log.py` & `tdworkflow-0.9.0/tdworkflow/log.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.3/tdworkflow/project.py` & `tdworkflow-0.9.0/tdworkflow/project.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.3/tdworkflow/resource.py` & `tdworkflow-0.9.0/tdworkflow/resource.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.3/tdworkflow/revision.py` & `tdworkflow-0.9.0/tdworkflow/revision.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.3/tdworkflow/schedule.py` & `tdworkflow-0.9.0/tdworkflow/schedule.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.3/tdworkflow/session.py` & `tdworkflow-0.9.0/tdworkflow/session.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.3/tdworkflow/task.py` & `tdworkflow-0.9.0/tdworkflow/task.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.3/tdworkflow/util.py` & `tdworkflow-0.9.0/tdworkflow/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,17 +44,29 @@
 def to_iso8601(dt: Optional[Union[str, datetime]]) -> str:
     if not dt:
         return ""
 
     if isinstance(dt, datetime):
         # Naive object
         if not dt.tzinfo:
-            return dt.astimezone(timezone(timedelta(0), "UTC")).isoformat()
+            return dt.astimezone(timezone.utc).isoformat()
         # Aware object
         else:
             return dt.isoformat()
 
     elif isinstance(dt, str):
         return dt
 
     else:
         raise ValueError("Unexpected type")
+
+
+def to_iso_instant(dt: datetime) -> str:
+    if isinstance(dt, datetime):
+        return (
+            dt.astimezone(timezone.utc)
+            .isoformat(timespec="seconds")
+            .replace("+00:00", "Z")
+        )
+
+    else:
+        raise ValueError("Unexpected type")
```

### Comparing `tdworkflow-0.8.3/tdworkflow/workflow.py` & `tdworkflow-0.9.0/tdworkflow/workflow.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.3/tdworkflow.egg-info/PKG-INFO` & `tdworkflow-0.9.0/tdworkflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdworkflow
-Version: 0.8.3
+Version: 0.9.0
 Summary: Unofficial Treasure Workflow API client
 Author-email: Aki Ariga <chezou@gmail.com>
 Maintainer-email: Aki Ariga <chezou@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -216,14 +216,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Database
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: mypy-extensions
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `tdworkflow-0.8.3/tdworkflow.egg-info/SOURCES.txt` & `tdworkflow-0.9.0/tdworkflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.3/tests/test_client.py` & `tdworkflow-0.9.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.3/tests/test_util.py` & `tdworkflow-0.9.0/tests/test_util.py`

 * *Files identical despite different names*

