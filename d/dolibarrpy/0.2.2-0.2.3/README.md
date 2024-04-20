# Comparing `tmp/dolibarrpy-0.2.2.tar.gz` & `tmp/dolibarrpy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolibarrpy-0.2.2.tar", last modified: Sat Apr 20 14:31:39 2024, max compression
+gzip compressed data, was "dolibarrpy-0.2.3.tar", last modified: Sat Apr 20 14:58:46 2024, max compression
```

## Comparing `dolibarrpy-0.2.2.tar` & `dolibarrpy-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 14:31:39.452175 dolibarrpy-0.2.2/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.2.2/LICENSE.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 14:31:39.452318 dolibarrpy-0.2.2/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.2.2/README.md
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 14:31:39.450059 dolibarrpy-0.2.2/dolibarrpy/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)    11332 2024-04-20 14:31:22.000000 dolibarrpy-0.2.2/dolibarrpy/Dolibarrpy.py
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.2.2/dolibarrpy/__init__.py
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 14:31:39.451899 dolibarrpy-0.2.2/dolibarrpy.egg-info/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 14:31:39.000000 dolibarrpy-0.2.2/dolibarrpy.egg-info/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-20 14:31:39.000000 dolibarrpy-0.2.2/dolibarrpy.egg-info/SOURCES.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-20 14:31:39.000000 dolibarrpy-0.2.2/dolibarrpy.egg-info/dependency_links.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-20 14:31:39.000000 dolibarrpy-0.2.2/dolibarrpy.egg-info/top_level.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-20 14:31:39.452750 dolibarrpy-0.2.2/setup.cfg
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1040 2024-04-20 14:28:38.000000 dolibarrpy-0.2.2/setup.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 14:58:46.415634 dolibarrpy-0.2.3/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.2.3/LICENSE.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 14:58:46.415774 dolibarrpy-0.2.3/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.2.3/README.md
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 14:58:46.413709 dolibarrpy-0.2.3/dolibarrpy/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)    12379 2024-04-20 14:58:38.000000 dolibarrpy-0.2.3/dolibarrpy/Dolibarrpy.py
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.2.3/dolibarrpy/__init__.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 14:58:46.415362 dolibarrpy-0.2.3/dolibarrpy.egg-info/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 14:58:46.000000 dolibarrpy-0.2.3/dolibarrpy.egg-info/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-20 14:58:46.000000 dolibarrpy-0.2.3/dolibarrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-20 14:58:46.000000 dolibarrpy-0.2.3/dolibarrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-20 14:58:46.000000 dolibarrpy-0.2.3/dolibarrpy.egg-info/top_level.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-20 14:58:46.416203 dolibarrpy-0.2.3/setup.cfg
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1040 2024-04-20 14:38:12.000000 dolibarrpy-0.2.3/setup.py
```

### Comparing `dolibarrpy-0.2.2/LICENSE.txt` & `dolibarrpy-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dolibarrpy-0.2.2/PKG-INFO` & `dolibarrpy-0.2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.2.2/dolibarrpy/Dolibarrpy.py` & `dolibarrpy-0.2.3/dolibarrpy/Dolibarrpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 import logging
-import json
+import json, urllib
 from dataclasses import dataclass, asdict
 from typing import Optional
 from icecream import install
 install()
 
 _logger = logging.getLogger(__name__)
 
@@ -325,7 +325,38 @@
         @param userid: 0 => connected user, Any other number than 0 is interpretated as a user id and if that user has roles on that project, they are shown.
         @return: list of project roles
         """
         objid = str(objid) + '/roles?userid=' + str(userid)
         result = self.call_get_api('projects', objid)
         return result
 
+    def get_project_by_ref(self, ref):
+        """
+        Get project tasks based on project ref
+        @return: project
+        """
+        if ref:
+            ref = 'ref/' + urllib.parse.quote(ref)
+            result = self.call_get_api('projects', ref)
+            return result
+        elif ref == '':
+            raise Exception("ref can not be empty")
+        elif ref is None:
+            raise Exception("ref can not be None")
+        else:
+            raise Exception("ref is wrong")
+
+    def get_project_by_ref_ext(self, ref_ext):
+        """
+        Get project tasks based on project ref
+        @return: project
+        """
+        if ref_ext:
+            ref_ext = 'ref_ext/' + urllib.parse.quote(ref_ext)
+            result = self.call_get_api('projects', ref_ext)
+            return result
+        elif ref_ext == '':
+            raise Exception("ref_ext can not be empty")
+        elif ref_ext is None:
+            raise Exception("ref_ext can not be None")
+        else:
+            raise Exception("ref_ext is wrong")
```

### Comparing `dolibarrpy-0.2.2/dolibarrpy.egg-info/PKG-INFO` & `dolibarrpy-0.2.3/dolibarrpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.2.2/setup.py` & `dolibarrpy-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 import os
 
 setup(
     name='dolibarrpy',
     packages=['dolibarrpy'],
-    version="0.2.2",
+    version="0.2.3",
     license='MIT',
     description='Python wrapper for Dolibarr API',
     long_description='Python wrapper for Dolibarr',
     long_description_content_type='text/markdown',
     author='Jon Bendtsen',
     author_email='jon.bendtsen.github@jonb.dk',
     url='https://github.com/JonBendtsen/dolibarrpy.git',
```

