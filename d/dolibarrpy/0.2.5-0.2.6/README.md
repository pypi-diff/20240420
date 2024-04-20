# Comparing `tmp/dolibarrpy-0.2.5.tar.gz` & `tmp/dolibarrpy-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolibarrpy-0.2.5.tar", last modified: Sat Apr 20 16:05:03 2024, max compression
+gzip compressed data, was "dolibarrpy-0.2.6.tar", last modified: Sat Apr 20 16:41:33 2024, max compression
```

## Comparing `dolibarrpy-0.2.5.tar` & `dolibarrpy-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 16:05:03.039609 dolibarrpy-0.2.5/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.2.5/LICENSE.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 16:05:03.039742 dolibarrpy-0.2.5/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.2.5/README.md
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 16:05:03.036744 dolibarrpy-0.2.5/dolibarrpy/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)    15042 2024-04-20 16:03:28.000000 dolibarrpy-0.2.5/dolibarrpy/Dolibarrpy.py
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.2.5/dolibarrpy/__init__.py
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 16:05:03.039348 dolibarrpy-0.2.5/dolibarrpy.egg-info/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 16:05:03.000000 dolibarrpy-0.2.5/dolibarrpy.egg-info/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-20 16:05:03.000000 dolibarrpy-0.2.5/dolibarrpy.egg-info/SOURCES.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-20 16:05:03.000000 dolibarrpy-0.2.5/dolibarrpy.egg-info/dependency_links.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-20 16:05:03.000000 dolibarrpy-0.2.5/dolibarrpy.egg-info/top_level.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-20 16:05:03.040189 dolibarrpy-0.2.5/setup.cfg
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1040 2024-04-20 16:04:45.000000 dolibarrpy-0.2.5/setup.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 16:41:33.044214 dolibarrpy-0.2.6/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.2.6/LICENSE.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 16:41:33.044354 dolibarrpy-0.2.6/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.2.6/README.md
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 16:41:33.042163 dolibarrpy-0.2.6/dolibarrpy/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)    16360 2024-04-20 16:40:16.000000 dolibarrpy-0.2.6/dolibarrpy/Dolibarrpy.py
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.2.6/dolibarrpy/__init__.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 16:41:33.043937 dolibarrpy-0.2.6/dolibarrpy.egg-info/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 16:41:33.000000 dolibarrpy-0.2.6/dolibarrpy.egg-info/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-20 16:41:33.000000 dolibarrpy-0.2.6/dolibarrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-20 16:41:33.000000 dolibarrpy-0.2.6/dolibarrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-20 16:41:33.000000 dolibarrpy-0.2.6/dolibarrpy.egg-info/top_level.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-20 16:41:33.044796 dolibarrpy-0.2.6/setup.cfg
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1040 2024-04-20 16:16:52.000000 dolibarrpy-0.2.6/setup.py
```

### Comparing `dolibarrpy-0.2.5/LICENSE.txt` & `dolibarrpy-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dolibarrpy-0.2.5/PKG-INFO` & `dolibarrpy-0.2.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.2.5/dolibarrpy/Dolibarrpy.py` & `dolibarrpy-0.2.6/dolibarrpy/Dolibarrpy.py`

 * *Files 5% similar despite different names*

```diff
@@ -426,8 +426,52 @@
         if from_MemberFilter is None:
             search_filter = MemberFilter()
         else:
             search_filter = from_MemberFilter
         search_filter.page = page
         params = asdict(search_filter)
         result = self.call_list_api('members', params=params)
-        return result
+        return result
+
+    def get_member_by_mid(self, objid):
+        """
+        Get member based on member id
+        @return: member
+        """
+        result = self.call_get_api('members', objid=objid)
+        return result
+
+    def get_member_subscriptions_by_mid(self, objid):
+        """
+        Get member subscriptions based on member id
+        @return: list of member subscriptions
+        """
+        objid = str(objid) + '/subscriptions'
+        result = self.call_get_api('members', objid)
+        return result
+
+    def get_member_by_thirdparty_id(self, objid):
+        """
+        Get member based on thirdparty id
+        @return: member
+        """
+        objid = 'thirdparty/' + str(objid)
+        result = self.call_get_api('members', objid)
+        return result
+
+    def get_member_by_thirdparty_barcode(self, barcode):
+        """
+        Get member based on thirdparty barcode
+        @return: member
+        """
+        objid = 'thirdparty/barcode/' + str(barcode)
+        result = self.call_get_api('members', objid)
+        return result
+
+    def get_member_by_thirdparty_email(self, email):
+        """
+        Get member based on thirdparty email
+        @return: member
+        """
+        objid = 'thirdparty/email/' + str(email)
+        result = self.call_get_api('members', objid)
+        return result
```

### Comparing `dolibarrpy-0.2.5/dolibarrpy.egg-info/PKG-INFO` & `dolibarrpy-0.2.6/dolibarrpy.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.2.5/setup.py` & `dolibarrpy-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 import os
 
 setup(
     name='dolibarrpy',
     packages=['dolibarrpy'],
-    version="0.2.5",
+    version="0.2.6",
     license='MIT',
     description='Python wrapper for Dolibarr API',
     long_description='Python wrapper for Dolibarr',
     long_description_content_type='text/markdown',
     author='Jon Bendtsen',
     author_email='jon.bendtsen.github@jonb.dk',
     url='https://github.com/JonBendtsen/dolibarrpy.git',
```

