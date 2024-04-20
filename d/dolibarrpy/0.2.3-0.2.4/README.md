# Comparing `tmp/dolibarrpy-0.2.3.tar.gz` & `tmp/dolibarrpy-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolibarrpy-0.2.3.tar", last modified: Sat Apr 20 14:58:46 2024, max compression
+gzip compressed data, was "dolibarrpy-0.2.4.tar", last modified: Sat Apr 20 15:13:39 2024, max compression
```

## Comparing `dolibarrpy-0.2.3.tar` & `dolibarrpy-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 14:58:46.415634 dolibarrpy-0.2.3/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.2.3/LICENSE.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 14:58:46.415774 dolibarrpy-0.2.3/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.2.3/README.md
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 14:58:46.413709 dolibarrpy-0.2.3/dolibarrpy/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)    12379 2024-04-20 14:58:38.000000 dolibarrpy-0.2.3/dolibarrpy/Dolibarrpy.py
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.2.3/dolibarrpy/__init__.py
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 14:58:46.415362 dolibarrpy-0.2.3/dolibarrpy.egg-info/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 14:58:46.000000 dolibarrpy-0.2.3/dolibarrpy.egg-info/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-20 14:58:46.000000 dolibarrpy-0.2.3/dolibarrpy.egg-info/SOURCES.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-20 14:58:46.000000 dolibarrpy-0.2.3/dolibarrpy.egg-info/dependency_links.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-20 14:58:46.000000 dolibarrpy-0.2.3/dolibarrpy.egg-info/top_level.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-20 14:58:46.416203 dolibarrpy-0.2.3/setup.cfg
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1040 2024-04-20 14:38:12.000000 dolibarrpy-0.2.3/setup.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 15:13:39.047463 dolibarrpy-0.2.4/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.2.4/LICENSE.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 15:13:39.047625 dolibarrpy-0.2.4/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.2.4/README.md
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 15:13:39.045378 dolibarrpy-0.2.4/dolibarrpy/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)    12983 2024-04-20 15:13:29.000000 dolibarrpy-0.2.4/dolibarrpy/Dolibarrpy.py
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.2.4/dolibarrpy/__init__.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 15:13:39.047169 dolibarrpy-0.2.4/dolibarrpy.egg-info/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 15:13:39.000000 dolibarrpy-0.2.4/dolibarrpy.egg-info/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-20 15:13:39.000000 dolibarrpy-0.2.4/dolibarrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-20 15:13:39.000000 dolibarrpy-0.2.4/dolibarrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-20 15:13:39.000000 dolibarrpy-0.2.4/dolibarrpy.egg-info/top_level.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-20 15:13:39.048079 dolibarrpy-0.2.4/setup.cfg
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1040 2024-04-20 15:13:31.000000 dolibarrpy-0.2.4/setup.py
```

### Comparing `dolibarrpy-0.2.3/LICENSE.txt` & `dolibarrpy-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dolibarrpy-0.2.3/PKG-INFO` & `dolibarrpy-0.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.2.3/dolibarrpy/Dolibarrpy.py` & `dolibarrpy-0.2.4/dolibarrpy/Dolibarrpy.py`

 * *Files 5% similar despite different names*

```diff
@@ -343,20 +343,36 @@
         elif ref is None:
             raise Exception("ref can not be None")
         else:
             raise Exception("ref is wrong")
 
     def get_project_by_ref_ext(self, ref_ext):
         """
-        Get project tasks based on project ref
+        Get project tasks based on project ref_ext
         @return: project
         """
         if ref_ext:
             ref_ext = 'ref_ext/' + urllib.parse.quote(ref_ext)
             result = self.call_get_api('projects', ref_ext)
             return result
         elif ref_ext == '':
             raise Exception("ref_ext can not be empty")
         elif ref_ext is None:
             raise Exception("ref_ext can not be None")
         else:
             raise Exception("ref_ext is wrong")
+
+    def get_project_by_email_msgid(self, email_msgid):
+        """
+        Get project tasks based on project email_msgid
+        @return: project
+        """
+        if email_msgid:
+            email_msgid = 'email_msgid/' + urllib.parse.quote(email_msgid)
+            result = self.call_get_api('projects', email_msgid)
+            return result
+        elif email_msgid == '':
+            raise Exception("email_msgid can not be empty")
+        elif email_msgid is None:
+            raise Exception("email_msgid can not be None")
+        else:
+            raise Exception("email_msgid is wrong")
```

### Comparing `dolibarrpy-0.2.3/dolibarrpy.egg-info/PKG-INFO` & `dolibarrpy-0.2.4/dolibarrpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.2.3/setup.py` & `dolibarrpy-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 import os
 
 setup(
     name='dolibarrpy',
     packages=['dolibarrpy'],
-    version="0.2.3",
+    version="0.2.4",
     license='MIT',
     description='Python wrapper for Dolibarr API',
     long_description='Python wrapper for Dolibarr',
     long_description_content_type='text/markdown',
     author='Jon Bendtsen',
     author_email='jon.bendtsen.github@jonb.dk',
     url='https://github.com/JonBendtsen/dolibarrpy.git',
```

