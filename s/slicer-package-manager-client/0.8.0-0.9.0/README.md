# Comparing `tmp/slicer-package-manager-client-0.8.0.tar.gz` & `tmp/slicer_package_manager_client-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slicer-package-manager-client-0.8.0.tar", last modified: Thu May 11 02:54:45 2023, max compression
+gzip compressed data, was "slicer_package_manager_client-0.9.0.tar", last modified: Sat Apr 20 04:50:12 2024, max compression
```

## Comparing `slicer-package-manager-client-0.8.0.tar` & `slicer_package_manager_client-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:45.621388 slicer-package-manager-client-0.8.0/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1924 2023-05-11 02:54:45.621388 slicer-package-manager-client-0.8.0/PKG-INFO
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1070 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/README.rst
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1515 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/pyproject.toml
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       38 2023-05-11 02:54:45.621388 slicer-package-manager-client-0.8.0/setup.cfg
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      196 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/setup.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:45.617388 slicer-package-manager-client-0.8.0/slicer_package_manager_client/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    26004 2023-05-11 02:52:30.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       70 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client/__main__.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:45.621388 slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/__init__.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:45.621388 slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      631 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/__init__.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1159 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/errors.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     9397 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/objectid.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2815 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/py3compat.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1518 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/tz_util.py
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    26208 2023-05-11 02:51:26.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client/cli.py
-drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2023-05-11 02:54:45.621388 slicer-package-manager-client-0.8.0/slicer_package_manager_client.egg-info/
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1924 2023-05-11 02:54:45.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client.egg-info/PKG-INFO
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      850 2023-05-11 02:54:45.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client.egg-info/SOURCES.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        1 2023-05-11 02:54:45.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client.egg-info/dependency_links.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       89 2023-05-11 02:54:45.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client.egg-info/entry_points.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        1 2023-05-11 02:54:45.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client.egg-info/not-zip-safe
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       74 2023-05-11 02:54:45.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client.egg-info/requires.txt
--rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       30 2023-05-11 02:54:45.000000 slicer-package-manager-client-0.8.0/slicer_package_manager_client.egg-info/top_level.txt
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2024-04-20 04:50:12.099195 slicer_package_manager_client-0.9.0/
+-rw-r--r--   0 jcfr      (1000) jcfr      (1000)     2147 2024-04-20 04:50:12.099195 slicer_package_manager_client-0.9.0/PKG-INFO
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1070 2022-05-20 21:48:20.000000 slicer_package_manager_client-0.9.0/README.rst
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1531 2024-04-18 06:53:56.000000 slicer_package_manager_client-0.9.0/pyproject.toml
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       38 2024-04-20 04:50:12.099195 slicer_package_manager_client-0.9.0/setup.cfg
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      196 2024-04-18 04:51:03.000000 slicer_package_manager_client-0.9.0/setup.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2024-04-20 04:50:12.095195 slicer_package_manager_client-0.9.0/slicer_package_manager_client/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    26004 2024-04-20 04:47:42.000000 slicer_package_manager_client-0.9.0/slicer_package_manager_client/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       70 2022-05-20 20:46:19.000000 slicer_package_manager_client-0.9.0/slicer_package_manager_client/__main__.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2024-04-20 04:50:12.099195 slicer_package_manager_client-0.9.0/slicer_package_manager_client/_vendor/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        0 2022-05-20 20:46:19.000000 slicer_package_manager_client-0.9.0/slicer_package_manager_client/_vendor/__init__.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2024-04-20 04:50:12.099195 slicer_package_manager_client-0.9.0/slicer_package_manager_client/_vendor/bson/
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      631 2022-05-20 20:46:19.000000 slicer_package_manager_client-0.9.0/slicer_package_manager_client/_vendor/bson/__init__.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1159 2023-05-04 06:13:27.000000 slicer_package_manager_client-0.9.0/slicer_package_manager_client/_vendor/bson/errors.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     9397 2023-05-04 09:36:52.000000 slicer_package_manager_client-0.9.0/slicer_package_manager_client/_vendor/bson/objectid.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     2815 2023-05-04 08:20:27.000000 slicer_package_manager_client-0.9.0/slicer_package_manager_client/_vendor/bson/py3compat.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)     1518 2023-05-04 08:01:59.000000 slicer_package_manager_client-0.9.0/slicer_package_manager_client/_vendor/bson/tz_util.py
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)    26208 2024-04-18 04:51:03.000000 slicer_package_manager_client-0.9.0/slicer_package_manager_client/cli.py
+drwxrwxr-x   0 jcfr      (1000) jcfr      (1000)        0 2024-04-20 04:50:12.099195 slicer_package_manager_client-0.9.0/slicer_package_manager_client.egg-info/
+-rw-r--r--   0 jcfr      (1000) jcfr      (1000)     2147 2024-04-20 04:50:12.000000 slicer_package_manager_client-0.9.0/slicer_package_manager_client.egg-info/PKG-INFO
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)      850 2024-04-20 04:50:12.000000 slicer_package_manager_client-0.9.0/slicer_package_manager_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        1 2024-04-20 04:50:12.000000 slicer_package_manager_client-0.9.0/slicer_package_manager_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       89 2024-04-20 04:50:12.000000 slicer_package_manager_client-0.9.0/slicer_package_manager_client.egg-info/entry_points.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)        1 2023-05-05 04:04:04.000000 slicer_package_manager_client-0.9.0/slicer_package_manager_client.egg-info/not-zip-safe
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       90 2024-04-20 04:50:12.000000 slicer_package_manager_client-0.9.0/slicer_package_manager_client.egg-info/requires.txt
+-rw-rw-r--   0 jcfr      (1000) jcfr      (1000)       30 2024-04-20 04:50:12.000000 slicer_package_manager_client-0.9.0/slicer_package_manager_client.egg-info/top_level.txt
```

### Comparing `slicer-package-manager-client-0.8.0/PKG-INFO` & `slicer_package_manager_client-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 2.1
 Name: slicer-package-manager-client
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python client for interacting with the Slicer package manager endpoint.
 Author-email: Pierre Assemat <pierre.assemat@kitware.com>, Jean-Christophe Fillion-Robin <jchris.fillionr@kitware.com>
 Maintainer-email: Jean-Christophe Fillion-Robin <jchris.fillionr@kitware.com>
 Project-URL: Documentation, https://slicer-package-manager.readthedocs.io/en/latest/commands_shell.html#slicer-package-manager-client
 Project-URL: Source, https://github.com/girder/slicer_package_manager/tree/main/python_client
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Requires-Dist: click>=6.7
+Requires-Dist: girder_client~=3.1.20
+Requires-Dist: tabulate
 Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-vcr; extra == "test"
+Requires-Dist: pytest-girder~=3.1.20; extra == "test"
 
 Slicer package manager Python Client
 ====================================
 
 Python client for managing Slicer application and extension packages
 organized on a server with the corresponding Girder plugin installed.
```

### Comparing `slicer-package-manager-client-0.8.0/README.rst` & `slicer_package_manager_client-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `slicer-package-manager-client-0.8.0/pyproject.toml` & `slicer_package_manager_client-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -15,27 +15,27 @@
 readme = "README.rst"
 classifiers = [
     "Environment :: Console",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dynamic = ["version"]
 dependencies = [
     "click>=6.7",
-    "girder_client",
+    "girder_client~=3.1.20",
     "tabulate",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-vcr",
-    "pytest-girder",
+    "pytest-girder~=3.1.20",
 ]
 
 [project.urls]
 Documentation = "https://slicer-package-manager.readthedocs.io/en/latest/commands_shell.html#slicer-package-manager-client"
 Source = "https://github.com/girder/slicer_package_manager/tree/main/python_client"
 
 [project.scripts]
```

### Comparing `slicer-package-manager-client-0.8.0/slicer_package_manager_client/__init__.py` & `slicer_package_manager_client-0.9.0/slicer_package_manager_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 from girder_client import GirderClient
 
 from ._vendor.bson.objectid import ObjectId
 
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 __license__ = 'Apache 2.0'
 
 appName = 'Slicer'
 
 
 class Constant:
     """
```

### Comparing `slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/__init__.py` & `slicer_package_manager_client-0.9.0/slicer_package_manager_client/_vendor/bson/__init__.py`

 * *Files identical despite different names*

### Comparing `slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/errors.py` & `slicer_package_manager_client-0.9.0/slicer_package_manager_client/_vendor/bson/errors.py`

 * *Files identical despite different names*

### Comparing `slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/objectid.py` & `slicer_package_manager_client-0.9.0/slicer_package_manager_client/_vendor/bson/objectid.py`

 * *Files identical despite different names*

### Comparing `slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/py3compat.py` & `slicer_package_manager_client-0.9.0/slicer_package_manager_client/_vendor/bson/py3compat.py`

 * *Files identical despite different names*

### Comparing `slicer-package-manager-client-0.8.0/slicer_package_manager_client/_vendor/bson/tz_util.py` & `slicer_package_manager_client-0.9.0/slicer_package_manager_client/_vendor/bson/tz_util.py`

 * *Files identical despite different names*

### Comparing `slicer-package-manager-client-0.8.0/slicer_package_manager_client/cli.py` & `slicer_package_manager_client-0.9.0/slicer_package_manager_client/cli.py`

 * *Files identical despite different names*

### Comparing `slicer-package-manager-client-0.8.0/slicer_package_manager_client.egg-info/PKG-INFO` & `slicer_package_manager_client-0.9.0/slicer_package_manager_client.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 2.1
 Name: slicer-package-manager-client
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python client for interacting with the Slicer package manager endpoint.
 Author-email: Pierre Assemat <pierre.assemat@kitware.com>, Jean-Christophe Fillion-Robin <jchris.fillionr@kitware.com>
 Maintainer-email: Jean-Christophe Fillion-Robin <jchris.fillionr@kitware.com>
 Project-URL: Documentation, https://slicer-package-manager.readthedocs.io/en/latest/commands_shell.html#slicer-package-manager-client
 Project-URL: Source, https://github.com/girder/slicer_package_manager/tree/main/python_client
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Requires-Dist: click>=6.7
+Requires-Dist: girder_client~=3.1.20
+Requires-Dist: tabulate
 Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-vcr; extra == "test"
+Requires-Dist: pytest-girder~=3.1.20; extra == "test"
 
 Slicer package manager Python Client
 ====================================
 
 Python client for managing Slicer application and extension packages
 organized on a server with the corresponding Girder plugin installed.
```

### Comparing `slicer-package-manager-client-0.8.0/slicer_package_manager_client.egg-info/SOURCES.txt` & `slicer_package_manager_client-0.9.0/slicer_package_manager_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

