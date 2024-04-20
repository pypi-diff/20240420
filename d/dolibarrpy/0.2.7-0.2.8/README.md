# Comparing `tmp/dolibarrpy-0.2.7.tar.gz` & `tmp/dolibarrpy-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolibarrpy-0.2.7.tar", last modified: Sat Apr 20 17:53:49 2024, max compression
+gzip compressed data, was "dolibarrpy-0.2.8.tar", last modified: Sat Apr 20 18:39:46 2024, max compression
```

## Comparing `dolibarrpy-0.2.7.tar` & `dolibarrpy-0.2.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 17:53:49.989516 dolibarrpy-0.2.7/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.2.7/LICENSE.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 17:53:49.989675 dolibarrpy-0.2.7/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.2.7/README.md
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 17:53:49.987078 dolibarrpy-0.2.7/dolibarrpy/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)    18077 2024-04-20 17:50:48.000000 dolibarrpy-0.2.7/dolibarrpy/Dolibarrpy.py
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.2.7/dolibarrpy/__init__.py
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 17:53:49.989223 dolibarrpy-0.2.7/dolibarrpy.egg-info/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 17:53:49.000000 dolibarrpy-0.2.7/dolibarrpy.egg-info/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-20 17:53:49.000000 dolibarrpy-0.2.7/dolibarrpy.egg-info/SOURCES.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-20 17:53:49.000000 dolibarrpy-0.2.7/dolibarrpy.egg-info/dependency_links.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-20 17:53:49.000000 dolibarrpy-0.2.7/dolibarrpy.egg-info/top_level.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-20 17:53:49.990142 dolibarrpy-0.2.7/setup.cfg
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1040 2024-04-20 17:32:13.000000 dolibarrpy-0.2.7/setup.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 18:39:46.413258 dolibarrpy-0.2.8/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.2.8/LICENSE.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 18:39:46.413422 dolibarrpy-0.2.8/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.2.8/README.md
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 18:39:46.411055 dolibarrpy-0.2.8/dolibarrpy/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)    18363 2024-04-20 18:38:11.000000 dolibarrpy-0.2.8/dolibarrpy/Dolibarrpy.py
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.2.8/dolibarrpy/__init__.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 18:39:46.412894 dolibarrpy-0.2.8/dolibarrpy.egg-info/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 18:39:46.000000 dolibarrpy-0.2.8/dolibarrpy.egg-info/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-20 18:39:46.000000 dolibarrpy-0.2.8/dolibarrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-20 18:39:46.000000 dolibarrpy-0.2.8/dolibarrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-20 18:39:46.000000 dolibarrpy-0.2.8/dolibarrpy.egg-info/top_level.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-20 18:39:46.413873 dolibarrpy-0.2.8/setup.cfg
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1040 2024-04-20 17:58:43.000000 dolibarrpy-0.2.8/setup.py
```

### Comparing `dolibarrpy-0.2.7/LICENSE.txt` & `dolibarrpy-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dolibarrpy-0.2.7/PKG-INFO` & `dolibarrpy-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.2.7/dolibarrpy/Dolibarrpy.py` & `dolibarrpy-0.2.8/dolibarrpy/Dolibarrpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -404,35 +404,41 @@
             ic(from_MemberFilter)
         if from_MemberFilter is None:
             search_filter = MemberFilter()
         else:
             search_filter = from_MemberFilter
         all_members=[]
         page = 0
-        some_members = self.find_some_members(search_filter, page)
-        while some_members:
-            all_members = all_members + list(some_members)
-            page += 1
+        while True:
             some_members = self.find_some_members(search_filter, page)
-            if len(some_members) < 100:
-                all_members = all_members + list(some_members)
+            if "error" in some_members:
+                break
+            elif [] == some_members:
                 break
+            elif {} == some_members:
+                break
+            else:
+                page += 1
+                all_members = all_members + list(some_members)
         return all_members
 
     def find_some_members(self, from_MemberFilter = None, page = 0):
         if self.debug:
             ic()
             ic(page)
             ic(from_MemberFilter)
         if from_MemberFilter is None:
             search_filter = MemberFilter()
         else:
             search_filter = from_MemberFilter
         search_filter.page = page
         params = asdict(search_filter)
+        limit = params.get("limit")
+        if 0 == limit:
+            raise Exception("sorry, but a limit if 0 does not make sense, be sensible")
         result = self.call_list_api('members', params=params)
         return result
 
     def get_member_by_mid(self, objid):
         """
         Get member based on member id
         @return: member
@@ -487,22 +493,25 @@
             ic(from_MemberFilter)
         if from_MemberFilter is None:
             search_filter = MemberFilter()
         else:
             search_filter = from_MemberFilter
         all_member_types=[]
         page = 0
-        some_member_types = self.find_some_member_types(search_filter, page)
-        while some_member_types:
-            all_member_types = all_member_types + list(some_member_types)
-            page += 1
+        while True:
             some_member_types = self.find_some_member_types(search_filter, page)
-            if len(some_member_types) < 100:
-                all_member_types = all_member_types + list(some_member_types)
+            if "error" in some_member_types:
+                break
+            elif [] == some_member_types:
                 break
+            elif {} == some_member_types:
+                break
+            else:
+                page += 1
+                all_member_types = all_member_types + list(some_member_types)
         return all_member_types
 
     def find_some_member_types(self, from_MemberFilter = None, page = 0):
         if self.debug:
             ic()
             ic(page)
             ic(from_MemberFilter)
@@ -511,12 +520,15 @@
         else:
             search_filter = from_MemberFilter
         search_filter.page = page
         params = asdict(search_filter)
         category = params.get("category")
         if category:
             raise Exception("sorry, you can not use category in this filter, try without")
+        limit = params.get("limit")
+        if 0 == limit:
+            raise Exception("sorry, but a limit if 0 does not make sense, be sensible")
         typeid = params.get("typeid")
         if typeid:
             raise Exception("sorry, you can not use typeid in this filter, try without")
         result = self.call_list_api('members/types', params=params)
         return result
```

### Comparing `dolibarrpy-0.2.7/dolibarrpy.egg-info/PKG-INFO` & `dolibarrpy-0.2.8/dolibarrpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.2.7/setup.py` & `dolibarrpy-0.2.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 import os
 
 setup(
     name='dolibarrpy',
     packages=['dolibarrpy'],
-    version="0.2.7",
+    version="0.2.8",
     license='MIT',
     description='Python wrapper for Dolibarr API',
     long_description='Python wrapper for Dolibarr',
     long_description_content_type='text/markdown',
     author='Jon Bendtsen',
     author_email='jon.bendtsen.github@jonb.dk',
     url='https://github.com/JonBendtsen/dolibarrpy.git',
```

