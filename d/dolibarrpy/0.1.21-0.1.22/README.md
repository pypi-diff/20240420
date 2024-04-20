# Comparing `tmp/dolibarrpy-0.1.21.tar.gz` & `tmp/dolibarrpy-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolibarrpy-0.1.21.tar", last modified: Sat Apr 20 12:21:47 2024, max compression
+gzip compressed data, was "dolibarrpy-0.1.22.tar", last modified: Sat Apr 20 13:29:20 2024, max compression
```

## Comparing `dolibarrpy-0.1.21.tar` & `dolibarrpy-0.1.22.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 12:21:47.980284 dolibarrpy-0.1.21/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.1.21/LICENSE.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      648 2024-04-20 12:21:47.980442 dolibarrpy-0.1.21/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.1.21/README.md
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 12:21:47.978302 dolibarrpy-0.1.21/dolibarrpy/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     9953 2024-04-20 11:54:32.000000 dolibarrpy-0.1.21/dolibarrpy/Dolibarrpy.py
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.1.21/dolibarrpy/__init__.py
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 12:21:47.980017 dolibarrpy-0.1.21/dolibarrpy.egg-info/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      648 2024-04-20 12:21:47.000000 dolibarrpy-0.1.21/dolibarrpy.egg-info/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-20 12:21:47.000000 dolibarrpy-0.1.21/dolibarrpy.egg-info/SOURCES.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-20 12:21:47.000000 dolibarrpy-0.1.21/dolibarrpy.egg-info/dependency_links.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-20 12:21:47.000000 dolibarrpy-0.1.21/dolibarrpy.egg-info/top_level.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-20 12:21:47.980969 dolibarrpy-0.1.21/setup.cfg
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1041 2024-04-20 11:06:10.000000 dolibarrpy-0.1.21/setup.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 13:29:20.575873 dolibarrpy-0.1.22/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.1.22/LICENSE.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      648 2024-04-20 13:29:20.576006 dolibarrpy-0.1.22/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.1.22/README.md
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 13:29:20.573946 dolibarrpy-0.1.22/dolibarrpy/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)    10075 2024-04-20 13:16:07.000000 dolibarrpy-0.1.22/dolibarrpy/Dolibarrpy.py
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.1.22/dolibarrpy/__init__.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 13:29:20.575625 dolibarrpy-0.1.22/dolibarrpy.egg-info/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      648 2024-04-20 13:29:20.000000 dolibarrpy-0.1.22/dolibarrpy.egg-info/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-20 13:29:20.000000 dolibarrpy-0.1.22/dolibarrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-20 13:29:20.000000 dolibarrpy-0.1.22/dolibarrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-20 13:29:20.000000 dolibarrpy-0.1.22/dolibarrpy.egg-info/top_level.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-20 13:29:20.576410 dolibarrpy-0.1.22/setup.cfg
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1041 2024-04-20 13:26:21.000000 dolibarrpy-0.1.22/setup.py
```

### Comparing `dolibarrpy-0.1.21/LICENSE.txt` & `dolibarrpy-0.1.22/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dolibarrpy-0.1.21/PKG-INFO` & `dolibarrpy-0.1.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.1.21
+Version: 0.1.22
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.1.21/dolibarrpy/Dolibarrpy.py` & `dolibarrpy-0.1.22/dolibarrpy/Dolibarrpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,10 +284,13 @@
             )
         if "closed" == with_status.lower():
             search_filter = ProjectFilter(
                 page=page,
                 sqlfilters="(t.fk_statut:=:2)"
             )
         params = asdict(search_filter)
-
         result = self.call_list_api('projects', params=params)
         return result
+
+    def get_project_by_id(self, objid):
+        result = self.call_get_api('projects', objid=objid)
+        return result
```

### Comparing `dolibarrpy-0.1.21/dolibarrpy.egg-info/PKG-INFO` & `dolibarrpy-0.1.22/dolibarrpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.1.21
+Version: 0.1.22
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.1.21/setup.py` & `dolibarrpy-0.1.22/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 import os
 
 setup(
     name='dolibarrpy',
     packages=['dolibarrpy'],
-    version="0.1.21",
+    version="0.1.22",
     license='MIT',
     description='Python wrapper for Dolibarr API',
     long_description='Python wrapper for Dolibarr',
     long_description_content_type='text/markdown',
     author='Jon Bendtsen',
     author_email='jon.bendtsen.github@jonb.dk',
     url='https://github.com/JonBendtsen/dolibarrpy.git',
```

