# Comparing `tmp/pyanglianwater-0.1.1.tar.gz` & `tmp/pyanglianwater-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyanglianwater-0.1.1.tar", last modified: Mon Apr  8 23:13:38 2024, max compression
+gzip compressed data, was "pyanglianwater-0.2.0.tar", last modified: Fri Apr 19 21:45:38 2024, max compression
```

## Comparing `pyanglianwater-0.1.1.tar` & `pyanglianwater-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:13:38.666261 pyanglianwater-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 23:13:16.000000 pyanglianwater-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-08 23:13:38.666261 pyanglianwater-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-08 23:13:16.000000 pyanglianwater-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:13:38.662261 pyanglianwater-0.1.1/pyanglianwater/
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-08 23:13:16.000000 pyanglianwater-0.1.1/pyanglianwater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 23:13:16.000000 pyanglianwater-0.1.1/pyanglianwater/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-08 23:13:16.000000 pyanglianwater-0.1.1/pyanglianwater/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-08 23:13:16.000000 pyanglianwater-0.1.1/pyanglianwater/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-08 23:13:16.000000 pyanglianwater-0.1.1/pyanglianwater/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-08 23:13:16.000000 pyanglianwater-0.1.1/pyanglianwater/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 23:13:16.000000 pyanglianwater-0.1.1/pyanglianwater/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:13:38.662261 pyanglianwater-0.1.1/pyanglianwater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-08 23:13:38.000000 pyanglianwater-0.1.1/pyanglianwater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-08 23:13:38.000000 pyanglianwater-0.1.1/pyanglianwater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 23:13:38.000000 pyanglianwater-0.1.1/pyanglianwater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-08 23:13:38.000000 pyanglianwater-0.1.1/pyanglianwater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 23:13:38.000000 pyanglianwater-0.1.1/pyanglianwater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-08 23:13:16.000000 pyanglianwater-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 23:13:38.666261 pyanglianwater-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-08 23:13:16.000000 pyanglianwater-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:45:38.966113 pyanglianwater-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-19 21:45:18.000000 pyanglianwater-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-19 21:45:38.966113 pyanglianwater-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-19 21:45:18.000000 pyanglianwater-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:45:38.962113 pyanglianwater-0.2.0/pyanglianwater/
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-19 21:45:18.000000 pyanglianwater-0.2.0/pyanglianwater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 21:45:18.000000 pyanglianwater-0.2.0/pyanglianwater/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-19 21:45:18.000000 pyanglianwater-0.2.0/pyanglianwater/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-19 21:45:18.000000 pyanglianwater-0.2.0/pyanglianwater/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-19 21:45:18.000000 pyanglianwater-0.2.0/pyanglianwater/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-19 21:45:18.000000 pyanglianwater-0.2.0/pyanglianwater/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:45:18.000000 pyanglianwater-0.2.0/pyanglianwater/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:45:38.966113 pyanglianwater-0.2.0/pyanglianwater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-19 21:45:38.000000 pyanglianwater-0.2.0/pyanglianwater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-19 21:45:38.000000 pyanglianwater-0.2.0/pyanglianwater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:45:38.000000 pyanglianwater-0.2.0/pyanglianwater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-19 21:45:38.000000 pyanglianwater-0.2.0/pyanglianwater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 21:45:38.000000 pyanglianwater-0.2.0/pyanglianwater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-19 21:45:18.000000 pyanglianwater-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:45:38.966113 pyanglianwater-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-19 21:45:18.000000 pyanglianwater-0.2.0/setup.py
```

### Comparing `pyanglianwater-0.1.1/LICENSE` & `pyanglianwater-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyanglianwater-0.1.1/PKG-INFO` & `pyanglianwater-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyanglianwater
-Version: 0.1.1
+Version: 0.2.0
 Summary: A package to interact with Anglian Water
 Home-page: http://github.com/pantherale0/pyanglianwater
 Author: pantherale0
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyanglianwater-0.1.1/README.md` & `pyanglianwater-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyanglianwater-0.1.1/pyanglianwater/api.py` & `pyanglianwater-0.2.0/pyanglianwater/api.py`

 * *Files identical despite different names*

### Comparing `pyanglianwater-0.1.1/pyanglianwater/exceptions.py` & `pyanglianwater-0.2.0/pyanglianwater/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,13 +11,15 @@
 
 class UnknownEndpointError(Exception):
     """Defines an unknown error."""
 
 class ExpiredAccessTokenError(Exception):
     """401 Unauthorized"""
 
+class TariffNotAvailableError(Exception):
+    """Tariff information not available or set."""
 
 API_RESPONSE_STATUS_CODE_MAPPING = {
     "E_LGN_006": InvalidPasswordError,
     "E_LGN_008": InvalidUsernameError,
     "S_SMR_1058": EndpointUnavailableError
 }
```

### Comparing `pyanglianwater-0.1.1/pyanglianwater.egg-info/PKG-INFO` & `pyanglianwater-0.2.0/pyanglianwater.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyanglianwater
-Version: 0.1.1
+Version: 0.2.0
 Summary: A package to interact with Anglian Water
 Home-page: http://github.com/pantherale0/pyanglianwater
 Author: pantherale0
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyanglianwater-0.1.1/setup.py` & `pyanglianwater-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,20 +35,14 @@
     version=version,
     description='A package to interact with Anglian Water',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://github.com/pantherale0/pyanglianwater',
     author='pantherale0',
     license='MIT',
-    packages=setuptools.find_packages(
-        exclude=[
-            'examples',
-            'test',
-        ]
-    ),
     package_data={
         'pyanglianwater': [
             'py.typed',
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
```

