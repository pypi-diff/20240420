# Comparing `tmp/contact-profiles-local-0.0.6.tar.gz` & `tmp/contact_profiles_local-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact-profiles-local-0.0.6.tar", last modified: Thu Apr 11 21:29:42 2024, max compression
+gzip compressed data, was "contact_profiles_local-0.0.7.tar", last modified: Sat Apr 20 11:18:11 2024, max compression
```

## Comparing `contact-profiles-local-0.0.6.tar` & `contact_profiles_local-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:29:42.429345 contact-profiles-local-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-11 21:29:42.429345 contact-profiles-local-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 21:29:16.000000 contact-profiles-local-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:29:42.429345 contact-profiles-local-0.0.6/contact_profiles_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:29:42.429345 contact-profiles-local-0.0.6/contact_profiles_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:29:16.000000 contact-profiles-local-0.0.6/contact_profiles_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-04-11 21:29:16.000000 contact-profiles-local-0.0.6/contact_profiles_local/src/contact_profiles_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-11 21:29:16.000000 contact-profiles-local-0.0.6/contact_profiles_local/src/contact_profiles_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:29:42.429345 contact-profiles-local-0.0.6/contact_profiles_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-11 21:29:42.000000 contact-profiles-local-0.0.6/contact_profiles_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-11 21:29:42.000000 contact-profiles-local-0.0.6/contact_profiles_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 21:29:42.000000 contact-profiles-local-0.0.6/contact_profiles_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-11 21:29:42.000000 contact-profiles-local-0.0.6/contact_profiles_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 21:29:42.000000 contact-profiles-local-0.0.6/contact_profiles_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-11 21:29:16.000000 contact-profiles-local-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 21:29:42.429345 contact-profiles-local-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-11 21:29:16.000000 contact-profiles-local-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:11.385280 contact_profiles_local-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-20 11:18:11.385280 contact_profiles_local-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-20 11:17:38.000000 contact_profiles_local-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:11.381280 contact_profiles_local-0.0.7/contact_profiles_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:11.381280 contact_profiles_local-0.0.7/contact_profiles_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 11:17:38.000000 contact_profiles_local-0.0.7/contact_profiles_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-04-20 11:17:38.000000 contact_profiles_local-0.0.7/contact_profiles_local/src/contact_profiles_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-20 11:17:38.000000 contact_profiles_local-0.0.7/contact_profiles_local/src/contact_profiles_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:18:11.385280 contact_profiles_local-0.0.7/contact_profiles_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-20 11:18:11.000000 contact_profiles_local-0.0.7/contact_profiles_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-20 11:18:11.000000 contact_profiles_local-0.0.7/contact_profiles_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 11:18:11.000000 contact_profiles_local-0.0.7/contact_profiles_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-20 11:18:11.000000 contact_profiles_local-0.0.7/contact_profiles_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-20 11:18:11.000000 contact_profiles_local-0.0.7/contact_profiles_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-20 11:17:38.000000 contact_profiles_local-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 11:18:11.385280 contact_profiles_local-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-20 11:17:38.000000 contact_profiles_local-0.0.7/setup.py
```

### Comparing `contact-profiles-local-0.0.6/PKG-INFO` & `contact_profiles_local-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-profiles-local
-Version: 0.0.6
+Version: 0.0.7
 Summary: PyPI Package for Circles contact-profiles-local Python
 Home-page: https://github.com/circles-zone/contact-profile-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact-profiles-local-0.0.6/contact_profiles_local/src/contact_profiles_local.py` & `contact_profiles_local-0.0.7/contact_profiles_local/src/contact_profiles_local.py`

 * *Files identical despite different names*

### Comparing `contact-profiles-local-0.0.6/contact_profiles_local/src/contact_profiles_local_constants.py` & `contact_profiles_local-0.0.7/contact_profiles_local/src/contact_profiles_local_constants.py`

 * *Files identical despite different names*

### Comparing `contact-profiles-local-0.0.6/contact_profiles_local.egg-info/PKG-INFO` & `contact_profiles_local-0.0.7/contact_profiles_local.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-profiles-local
-Version: 0.0.6
+Version: 0.0.7
 Summary: PyPI Package for Circles contact-profiles-local Python
 Home-page: https://github.com/circles-zone/contact-profile-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact-profiles-local-0.0.6/setup.py` & `contact_profiles_local-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "contact-profiles-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.6',  # update only the minor version each time # https://pypi.org/project/contact-profiles-local/
+    version='0.0.7',  # update only the minor version each time # https://pypi.org/project/contact-profiles-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles contact-profiles-local Python",
     long_description="PyPI Package for Circles contact-profiles-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/contact-profile-local-python-package",
     packages=[package_dir],
```

