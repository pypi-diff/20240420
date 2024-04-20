# Comparing `tmp/dolibarrpy-0.2.1.tar.gz` & `tmp/dolibarrpy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolibarrpy-0.2.1.tar", last modified: Sat Apr 20 14:22:18 2024, max compression
+gzip compressed data, was "dolibarrpy-0.2.2.tar", last modified: Sat Apr 20 14:31:39 2024, max compression
```

## Comparing `dolibarrpy-0.2.1.tar` & `dolibarrpy-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 14:22:18.581563 dolibarrpy-0.2.1/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.2.1/LICENSE.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 14:22:18.581718 dolibarrpy-0.2.1/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.2.1/README.md
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 14:22:18.579516 dolibarrpy-0.2.1/dolibarrpy/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)    11241 2024-04-20 14:18:32.000000 dolibarrpy-0.2.1/dolibarrpy/Dolibarrpy.py
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.2.1/dolibarrpy/__init__.py
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 14:22:18.581276 dolibarrpy-0.2.1/dolibarrpy.egg-info/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 14:22:18.000000 dolibarrpy-0.2.1/dolibarrpy.egg-info/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-20 14:22:18.000000 dolibarrpy-0.2.1/dolibarrpy.egg-info/SOURCES.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-20 14:22:18.000000 dolibarrpy-0.2.1/dolibarrpy.egg-info/dependency_links.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-20 14:22:18.000000 dolibarrpy-0.2.1/dolibarrpy.egg-info/top_level.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-20 14:22:18.582161 dolibarrpy-0.2.1/setup.cfg
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1040 2024-04-20 14:21:51.000000 dolibarrpy-0.2.1/setup.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 14:31:39.452175 dolibarrpy-0.2.2/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.2.2/LICENSE.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 14:31:39.452318 dolibarrpy-0.2.2/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.2.2/README.md
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 14:31:39.450059 dolibarrpy-0.2.2/dolibarrpy/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)    11332 2024-04-20 14:31:22.000000 dolibarrpy-0.2.2/dolibarrpy/Dolibarrpy.py
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.2.2/dolibarrpy/__init__.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 14:31:39.451899 dolibarrpy-0.2.2/dolibarrpy.egg-info/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 14:31:39.000000 dolibarrpy-0.2.2/dolibarrpy.egg-info/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-20 14:31:39.000000 dolibarrpy-0.2.2/dolibarrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-20 14:31:39.000000 dolibarrpy-0.2.2/dolibarrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-20 14:31:39.000000 dolibarrpy-0.2.2/dolibarrpy.egg-info/top_level.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-20 14:31:39.452750 dolibarrpy-0.2.2/setup.cfg
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1040 2024-04-20 14:28:38.000000 dolibarrpy-0.2.2/setup.py
```

### Comparing `dolibarrpy-0.2.1/LICENSE.txt` & `dolibarrpy-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dolibarrpy-0.2.1/PKG-INFO` & `dolibarrpy-0.2.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.2.1/dolibarrpy/Dolibarrpy.py` & `dolibarrpy-0.2.2/dolibarrpy/Dolibarrpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,15 +297,19 @@
                 page=page,
                 sqlfilters="(t.fk_statut:=:2)"
             )
         params = asdict(search_filter)
         result = self.call_list_api('projects', params=params)
         return result
 
-    def get_project_by_id(self, objid):
+    def get_project_by_pid(self, objid):
+        """
+        Get project based on project id
+        @return: project 
+        """
         result = self.call_get_api('projects', objid=objid)
         return result
 
     def get_project_tasks_by_pid(self, objid, includetimespent=0):
         """
         Get project tasks based on project id
         @param includetimespent: 0 => Return only list of tasks, 1 => Include a summary of time spent, 2=> Include details of time spent lines
```

### Comparing `dolibarrpy-0.2.1/dolibarrpy.egg-info/PKG-INFO` & `dolibarrpy-0.2.2/dolibarrpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.2.1/setup.py` & `dolibarrpy-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 import os
 
 setup(
     name='dolibarrpy',
     packages=['dolibarrpy'],
-    version="0.2.1",
+    version="0.2.2",
     license='MIT',
     description='Python wrapper for Dolibarr API',
     long_description='Python wrapper for Dolibarr',
     long_description_content_type='text/markdown',
     author='Jon Bendtsen',
     author_email='jon.bendtsen.github@jonb.dk',
     url='https://github.com/JonBendtsen/dolibarrpy.git',
```

