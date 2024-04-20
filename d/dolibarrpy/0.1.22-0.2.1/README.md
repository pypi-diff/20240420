# Comparing `tmp/dolibarrpy-0.1.22.tar.gz` & `tmp/dolibarrpy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolibarrpy-0.1.22.tar", last modified: Sat Apr 20 13:29:20 2024, max compression
+gzip compressed data, was "dolibarrpy-0.2.1.tar", last modified: Sat Apr 20 14:22:18 2024, max compression
```

## Comparing `dolibarrpy-0.1.22.tar` & `dolibarrpy-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 13:29:20.575873 dolibarrpy-0.1.22/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.1.22/LICENSE.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      648 2024-04-20 13:29:20.576006 dolibarrpy-0.1.22/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.1.22/README.md
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 13:29:20.573946 dolibarrpy-0.1.22/dolibarrpy/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)    10075 2024-04-20 13:16:07.000000 dolibarrpy-0.1.22/dolibarrpy/Dolibarrpy.py
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.1.22/dolibarrpy/__init__.py
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 13:29:20.575625 dolibarrpy-0.1.22/dolibarrpy.egg-info/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      648 2024-04-20 13:29:20.000000 dolibarrpy-0.1.22/dolibarrpy.egg-info/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-20 13:29:20.000000 dolibarrpy-0.1.22/dolibarrpy.egg-info/SOURCES.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-20 13:29:20.000000 dolibarrpy-0.1.22/dolibarrpy.egg-info/dependency_links.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-20 13:29:20.000000 dolibarrpy-0.1.22/dolibarrpy.egg-info/top_level.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-20 13:29:20.576410 dolibarrpy-0.1.22/setup.cfg
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1041 2024-04-20 13:26:21.000000 dolibarrpy-0.1.22/setup.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 14:22:18.581563 dolibarrpy-0.2.1/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.2.1/LICENSE.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 14:22:18.581718 dolibarrpy-0.2.1/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.2.1/README.md
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 14:22:18.579516 dolibarrpy-0.2.1/dolibarrpy/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)    11241 2024-04-20 14:18:32.000000 dolibarrpy-0.2.1/dolibarrpy/Dolibarrpy.py
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.2.1/dolibarrpy/__init__.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 14:22:18.581276 dolibarrpy-0.2.1/dolibarrpy.egg-info/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 14:22:18.000000 dolibarrpy-0.2.1/dolibarrpy.egg-info/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-20 14:22:18.000000 dolibarrpy-0.2.1/dolibarrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-20 14:22:18.000000 dolibarrpy-0.2.1/dolibarrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-20 14:22:18.000000 dolibarrpy-0.2.1/dolibarrpy.egg-info/top_level.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-20 14:22:18.582161 dolibarrpy-0.2.1/setup.cfg
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1040 2024-04-20 14:21:51.000000 dolibarrpy-0.2.1/setup.py
```

### Comparing `dolibarrpy-0.1.22/LICENSE.txt` & `dolibarrpy-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dolibarrpy-0.1.22/PKG-INFO` & `dolibarrpy-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.1.22
+Version: 0.2.1
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.1.22/dolibarrpy/Dolibarrpy.py` & `dolibarrpy-0.2.1/dolibarrpy/Dolibarrpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import requests
 import logging
 import json
 from dataclasses import dataclass, asdict
 from typing import Optional
+from icecream import install
+install()
 
 _logger = logging.getLogger(__name__)
 
 @dataclass
 class ProjectFilter():
     sortfield: Optional[str] = None
     sortorder: Optional[str] = None
@@ -18,19 +20,21 @@
     properties: Optional[str] = None        # Restrict the data returned to theses properties. Ignored if empty. Comma separated list of properties names
 
 
 class Dolibarrpy():
     url = 'https://dolibarr.example.com/api/index.php/'
     token = 'your token'
     timeout = 16
+    debug = False
 
-    def __init__(self, url, token, timeout):
+    def __init__(self, url, token, timeout, debug):
         self.url = url
         self.token = token
         self.timeout = timeout
+        self.debug = debug
 
     def get_headers(self):
         return {
             'DOLAPIKEY': self.token,
             'Accept': 'application/json'
         }
 
@@ -53,14 +57,17 @@
             result = response.text
         return result
 
     def call_get_api(self, object, objid):
         url = self.url + object + '/' + str(objid)
         headers = self.get_headers()
         response = requests.get(url, headers=headers, timeout=self.timeout)
+        if self.debug:
+            ic(url)
+            ic(response)
         json_result = json.loads(response.text)
 
         return json_result
 
     def call_create_api(self, object, params={}):
         url = self.url + object
         headers = self.get_headers()
@@ -71,16 +78,19 @@
             _logger.error(response)
             _logger.error(response.text)
             result = response
         return result
 
     def call_action_api(self, object, objid, action, params={}):
         url = self.url + object + '/' + str(objid) + "/" + action
-        headers = self.get_headers()
+        headers = self.post_headers()
         response = requests.post(url, json=params, headers=headers, timeout=self.timeout)
+        if self.debug:
+            ic(url)
+            ic(response)
         try:
             result = json.loads(response.text)
         except:
             raise Exception(response.text)
         return result
 
     def call_update_api(self, object, objid, params={}):
@@ -290,7 +300,28 @@
         params = asdict(search_filter)
         result = self.call_list_api('projects', params=params)
         return result
 
     def get_project_by_id(self, objid):
         result = self.call_get_api('projects', objid=objid)
         return result
+
+    def get_project_tasks_by_pid(self, objid, includetimespent=0):
+        """
+        Get project tasks based on project id
+        @param includetimespent: 0 => Return only list of tasks, 1 => Include a summary of time spent, 2=> Include details of time spent lines
+        @return: list of project tasks
+        """
+        objid = str(objid) + '/tasks?includetimespent=' + str(includetimespent)
+        result = self.call_get_api('projects', objid)
+        return result
+
+    def get_project_roles_by_pid(self, objid, userid=0):
+        """
+        Get project roles based on project id
+        @param userid: 0 => connected user, Any other number than 0 is interpretated as a user id and if that user has roles on that project, they are shown.
+        @return: list of project roles
+        """
+        objid = str(objid) + '/roles?userid=' + str(userid)
+        result = self.call_get_api('projects', objid)
+        return result
+
```

### Comparing `dolibarrpy-0.1.22/dolibarrpy.egg-info/PKG-INFO` & `dolibarrpy-0.2.1/dolibarrpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.1.22
+Version: 0.2.1
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.1.22/setup.py` & `dolibarrpy-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 import os
 
 setup(
     name='dolibarrpy',
     packages=['dolibarrpy'],
-    version="0.1.22",
+    version="0.2.1",
     license='MIT',
     description='Python wrapper for Dolibarr API',
     long_description='Python wrapper for Dolibarr',
     long_description_content_type='text/markdown',
     author='Jon Bendtsen',
     author_email='jon.bendtsen.github@jonb.dk',
     url='https://github.com/JonBendtsen/dolibarrpy.git',
```

