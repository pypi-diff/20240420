# Comparing `tmp/drf_authentify-0.3.2.tar.gz` & `tmp/drf_authentify-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_authentify-0.3.2.tar", last modified: Sat Apr 20 17:31:14 2024, max compression
+gzip compressed data, was "drf_authentify-0.3.3.tar", last modified: Sat Apr 20 20:18:55 2024, max compression
```

## Comparing `drf_authentify-0.3.2.tar` & `drf_authentify-0.3.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 17:31:14.521394 drf_authentify-0.3.2/
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     1501 2024-04-20 17:25:25.000000 drf_authentify-0.3.2/LICENSE
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       33 2024-04-20 17:25:25.000000 drf_authentify-0.3.2/MANIFEST.in
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)     8215 2024-04-20 17:31:14.521394 drf_authentify-0.3.2/PKG-INFO
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     4727 2024-04-20 17:25:25.000000 drf_authentify-0.3.2/README.md
-drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 17:31:14.513393 drf_authentify-0.3.2/drf_authentify/
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 17:25:15.000000 drf_authentify-0.3.2/drf_authentify/__init__.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     1687 2024-04-20 17:25:15.000000 drf_authentify-0.3.2/drf_authentify/admin.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      159 2024-04-20 17:25:15.000000 drf_authentify-0.3.2/drf_authentify/apps.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     1806 2024-04-20 17:25:15.000000 drf_authentify-0.3.2/drf_authentify/auth.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      185 2024-04-20 17:25:15.000000 drf_authentify-0.3.2/drf_authentify/choices.py
-drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 17:31:14.517393 drf_authentify-0.3.2/drf_authentify/migrations/
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     1193 2024-04-20 17:25:15.000000 drf_authentify-0.3.2/drf_authentify/migrations/0001_initial.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 17:25:15.000000 drf_authentify-0.3.2/drf_authentify/migrations/__init__.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     2425 2024-04-20 17:25:15.000000 drf_authentify-0.3.2/drf_authentify/models.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      651 2024-04-20 17:25:15.000000 drf_authentify-0.3.2/drf_authentify/settings.py
-drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 17:31:14.517393 drf_authentify-0.3.2/drf_authentify/tests/
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 17:25:15.000000 drf_authentify-0.3.2/drf_authentify/tests/__init__.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 17:25:15.000000 drf_authentify-0.3.2/drf_authentify/tests/test_auth.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     9566 2024-04-20 17:25:15.000000 drf_authentify-0.3.2/drf_authentify/tests/test_models.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     2731 2024-04-20 17:25:15.000000 drf_authentify-0.3.2/drf_authentify/tests/test_utils.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      208 2024-04-20 17:25:15.000000 drf_authentify-0.3.2/drf_authentify/urls.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      888 2024-04-20 17:25:15.000000 drf_authentify-0.3.2/drf_authentify/utils.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       63 2024-04-20 17:25:15.000000 drf_authentify-0.3.2/drf_authentify/views.py
-drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 17:31:14.521394 drf_authentify-0.3.2/drf_authentify.egg-info/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)     8215 2024-04-20 17:31:14.000000 drf_authentify-0.3.2/drf_authentify.egg-info/PKG-INFO
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      697 2024-04-20 17:31:14.000000 drf_authentify-0.3.2/drf_authentify.egg-info/SOURCES.txt
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        1 2024-04-20 17:31:14.000000 drf_authentify-0.3.2/drf_authentify.egg-info/dependency_links.txt
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       37 2024-04-20 17:31:14.000000 drf_authentify-0.3.2/drf_authentify.egg-info/requires.txt
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       15 2024-04-20 17:31:14.000000 drf_authentify-0.3.2/drf_authentify.egg-info/top_level.txt
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     1818 2024-04-20 17:31:01.000000 drf_authentify-0.3.2/pyproject.toml
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       38 2024-04-20 17:31:14.521394 drf_authentify-0.3.2/setup.cfg
+drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 20:18:55.351765 drf_authentify-0.3.3/
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     1501 2024-04-20 17:25:25.000000 drf_authentify-0.3.3/LICENSE
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       33 2024-04-20 17:25:25.000000 drf_authentify-0.3.3/MANIFEST.in
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     8183 2024-04-20 20:18:55.351765 drf_authentify-0.3.3/PKG-INFO
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     4727 2024-04-20 17:25:25.000000 drf_authentify-0.3.3/README.md
+drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 20:18:55.343764 drf_authentify-0.3.3/drf_authentify/
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 17:25:15.000000 drf_authentify-0.3.3/drf_authentify/__init__.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     1687 2024-04-20 17:25:15.000000 drf_authentify-0.3.3/drf_authentify/admin.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      159 2024-04-20 17:25:15.000000 drf_authentify-0.3.3/drf_authentify/apps.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     1806 2024-04-20 17:25:15.000000 drf_authentify-0.3.3/drf_authentify/auth.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      185 2024-04-20 17:25:15.000000 drf_authentify-0.3.3/drf_authentify/choices.py
+drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 20:18:55.347765 drf_authentify-0.3.3/drf_authentify/migrations/
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     1193 2024-04-20 17:25:15.000000 drf_authentify-0.3.3/drf_authentify/migrations/0001_initial.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 17:25:15.000000 drf_authentify-0.3.3/drf_authentify/migrations/__init__.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     2425 2024-04-20 17:25:15.000000 drf_authentify-0.3.3/drf_authentify/models.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      651 2024-04-20 17:25:15.000000 drf_authentify-0.3.3/drf_authentify/settings.py
+drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 20:18:55.351765 drf_authentify-0.3.3/drf_authentify/tests/
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 17:25:15.000000 drf_authentify-0.3.3/drf_authentify/tests/__init__.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 17:25:15.000000 drf_authentify-0.3.3/drf_authentify/tests/test_auth.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     9566 2024-04-20 17:25:15.000000 drf_authentify-0.3.3/drf_authentify/tests/test_models.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     2731 2024-04-20 17:25:15.000000 drf_authentify-0.3.3/drf_authentify/tests/test_utils.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      208 2024-04-20 17:25:15.000000 drf_authentify-0.3.3/drf_authentify/urls.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      888 2024-04-20 17:25:15.000000 drf_authentify-0.3.3/drf_authentify/utils.py
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       63 2024-04-20 17:25:15.000000 drf_authentify-0.3.3/drf_authentify/views.py
+drwxrwxr-x   0 gabriel   (1000) gabriel   (1000)        0 2024-04-20 20:18:55.351765 drf_authentify-0.3.3/drf_authentify.egg-info/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     8183 2024-04-20 20:18:55.000000 drf_authentify-0.3.3/drf_authentify.egg-info/PKG-INFO
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)      697 2024-04-20 20:18:55.000000 drf_authentify-0.3.3/drf_authentify.egg-info/SOURCES.txt
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)        1 2024-04-20 20:18:55.000000 drf_authentify-0.3.3/drf_authentify.egg-info/dependency_links.txt
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       37 2024-04-20 20:18:55.000000 drf_authentify-0.3.3/drf_authentify.egg-info/requires.txt
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       15 2024-04-20 20:18:55.000000 drf_authentify-0.3.3/drf_authentify.egg-info/top_level.txt
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)     1783 2024-04-20 20:17:58.000000 drf_authentify-0.3.3/pyproject.toml
+-rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       38 2024-04-20 20:18:55.351765 drf_authentify-0.3.3/setup.cfg
```

### Comparing `drf_authentify-0.3.2/LICENSE` & `drf_authentify-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_authentify-0.3.2/PKG-INFO` & `drf_authentify-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: drf-authentify
-Version: 0.3.2
+Version: 0.3.3
 Summary: A simple authentication module for django rest framework
-Author-email: Gabriel Idenyi <idenyigabriel@gmail.com>
+Author: Gabriel Idenyi
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Idenyi Gabriel
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `drf_authentify-0.3.2/README.md` & `drf_authentify-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `drf_authentify-0.3.2/drf_authentify/admin.py` & `drf_authentify-0.3.3/drf_authentify/admin.py`

 * *Files identical despite different names*

### Comparing `drf_authentify-0.3.2/drf_authentify/auth.py` & `drf_authentify-0.3.3/drf_authentify/auth.py`

 * *Files identical despite different names*

### Comparing `drf_authentify-0.3.2/drf_authentify/migrations/0001_initial.py` & `drf_authentify-0.3.3/drf_authentify/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf_authentify-0.3.2/drf_authentify/models.py` & `drf_authentify-0.3.3/drf_authentify/models.py`

 * *Files identical despite different names*

### Comparing `drf_authentify-0.3.2/drf_authentify/settings.py` & `drf_authentify-0.3.3/drf_authentify/settings.py`

 * *Files identical despite different names*

### Comparing `drf_authentify-0.3.2/drf_authentify/tests/test_models.py` & `drf_authentify-0.3.3/drf_authentify/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `drf_authentify-0.3.2/drf_authentify/tests/test_utils.py` & `drf_authentify-0.3.3/drf_authentify/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `drf_authentify-0.3.2/drf_authentify/utils.py` & `drf_authentify-0.3.3/drf_authentify/utils.py`

 * *Files identical despite different names*

### Comparing `drf_authentify-0.3.2/drf_authentify.egg-info/PKG-INFO` & `drf_authentify-0.3.3/drf_authentify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: drf-authentify
-Version: 0.3.2
+Version: 0.3.3
 Summary: A simple authentication module for django rest framework
-Author-email: Gabriel Idenyi <idenyigabriel@gmail.com>
+Author: Gabriel Idenyi
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Idenyi Gabriel
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `drf_authentify-0.3.2/drf_authentify.egg-info/SOURCES.txt` & `drf_authentify-0.3.3/drf_authentify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf_authentify-0.3.2/pyproject.toml` & `drf_authentify-0.3.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools >= 40.8.0"]
 build-backend = 'setuptools.build_meta'
 
 
 [project]
 name = "drf-authentify"
-version = "0.3.2"
+version = "0.3.3"
 description = "A simple authentication module for django rest framework"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ["django", "djangorestframework", "drf", "authentication"]
 authors = [
-    {name = "Gabriel Idenyi", email = "idenyigabriel@gmail.com"}
+    {name = "Gabriel Idenyi"}
 ]
 maintainers = []
 requires-python = ">=3.8"
 dependencies = [
     "Django >= 3.2",
     "djangorestframework >= 3.1",
 ]
```

