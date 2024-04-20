# Comparing `tmp/profiles_local-0.0.66.tar.gz` & `tmp/profiles_local-0.0.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profiles_local-0.0.66.tar", last modified: Fri Apr 19 11:37:13 2024, max compression
+gzip compressed data, was "profiles_local-0.0.67.tar", last modified: Fri Apr 19 14:09:29 2024, max compression
```

## Comparing `profiles_local-0.0.66.tar` & `profiles_local-0.0.67.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:37:13.261252 profiles_local-0.0.66/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-19 11:37:13.261252 profiles_local-0.0.66/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-19 11:36:35.000000 profiles_local-0.0.66/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:37:13.261252 profiles_local-0.0.66/profiles_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:37:13.261252 profiles_local-0.0.66/profiles_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 11:36:35.000000 profiles_local-0.0.66/profiles_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-19 11:36:35.000000 profiles_local-0.0.66/profiles_local/src/comprehensive_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-19 11:36:35.000000 profiles_local-0.0.66/profiles_local/src/constants_profiles_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-04-19 11:36:35.000000 profiles_local-0.0.66/profiles_local/src/profiles_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:37:13.261252 profiles_local-0.0.66/profiles_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-19 11:37:13.000000 profiles_local-0.0.66/profiles_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-19 11:37:13.000000 profiles_local-0.0.66/profiles_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 11:37:13.000000 profiles_local-0.0.66/profiles_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-19 11:37:13.000000 profiles_local-0.0.66/profiles_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 11:37:13.000000 profiles_local-0.0.66/profiles_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-19 11:36:35.000000 profiles_local-0.0.66/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 11:37:13.261252 profiles_local-0.0.66/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-19 11:36:35.000000 profiles_local-0.0.66/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:09:29.797635 profiles_local-0.0.67/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-19 14:09:29.797635 profiles_local-0.0.67/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-19 14:08:52.000000 profiles_local-0.0.67/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:09:29.793635 profiles_local-0.0.67/profiles_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:09:29.797635 profiles_local-0.0.67/profiles_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:08:52.000000 profiles_local-0.0.67/profiles_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-19 14:08:52.000000 profiles_local-0.0.67/profiles_local/src/comprehensive_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-19 14:08:52.000000 profiles_local-0.0.67/profiles_local/src/constants_profiles_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-04-19 14:08:52.000000 profiles_local-0.0.67/profiles_local/src/profiles_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:09:29.797635 profiles_local-0.0.67/profiles_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-19 14:09:29.000000 profiles_local-0.0.67/profiles_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-19 14:09:29.000000 profiles_local-0.0.67/profiles_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:09:29.000000 profiles_local-0.0.67/profiles_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-19 14:09:29.000000 profiles_local-0.0.67/profiles_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 14:09:29.000000 profiles_local-0.0.67/profiles_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-19 14:08:52.000000 profiles_local-0.0.67/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:09:29.797635 profiles_local-0.0.67/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-19 14:08:52.000000 profiles_local-0.0.67/setup.py
```

### Comparing `profiles_local-0.0.66/PKG-INFO` & `profiles_local-0.0.67/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profiles-local
-Version: 0.0.66
+Version: 0.0.67
 Summary: This is a package for sharing common crud operation to profile schema in the db
 Home-page: https://github.com/circles-zone/profiles-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `profiles_local-0.0.66/README.md` & `profiles_local-0.0.67/README.md`

 * *Files identical despite different names*

### Comparing `profiles_local-0.0.66/profiles_local/src/comprehensive_profile.py` & `profiles_local-0.0.67/profiles_local/src/comprehensive_profile.py`

 * *Files identical despite different names*

### Comparing `profiles_local-0.0.66/profiles_local/src/constants_profiles_local.py` & `profiles_local-0.0.67/profiles_local/src/constants_profiles_local.py`

 * *Files identical despite different names*

### Comparing `profiles_local-0.0.66/profiles_local/src/profiles_local.py` & `profiles_local-0.0.67/profiles_local/src/profiles_local.py`

 * *Files identical despite different names*

### Comparing `profiles_local-0.0.66/profiles_local.egg-info/PKG-INFO` & `profiles_local-0.0.67/profiles_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profiles-local
-Version: 0.0.66
+Version: 0.0.67
 Summary: This is a package for sharing common crud operation to profile schema in the db
 Home-page: https://github.com/circles-zone/profiles-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `profiles_local-0.0.66/setup.py` & `profiles_local-0.0.67/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "profiles-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.66',  # https://pypi.org/project/profiles-local/
+    version='0.0.67',  # https://pypi.org/project/profiles-local/
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     description="This is a package for sharing common crud operation to profile schema in the db",
```

