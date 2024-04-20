# Comparing `tmp/dolibarrpy-0.2.4.tar.gz` & `tmp/dolibarrpy-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolibarrpy-0.2.4.tar", last modified: Sat Apr 20 15:13:39 2024, max compression
+gzip compressed data, was "dolibarrpy-0.2.5.tar", last modified: Sat Apr 20 16:05:03 2024, max compression
```

## Comparing `dolibarrpy-0.2.4.tar` & `dolibarrpy-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 15:13:39.047463 dolibarrpy-0.2.4/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.2.4/LICENSE.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 15:13:39.047625 dolibarrpy-0.2.4/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.2.4/README.md
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 15:13:39.045378 dolibarrpy-0.2.4/dolibarrpy/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)    12983 2024-04-20 15:13:29.000000 dolibarrpy-0.2.4/dolibarrpy/Dolibarrpy.py
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.2.4/dolibarrpy/__init__.py
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 15:13:39.047169 dolibarrpy-0.2.4/dolibarrpy.egg-info/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 15:13:39.000000 dolibarrpy-0.2.4/dolibarrpy.egg-info/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-20 15:13:39.000000 dolibarrpy-0.2.4/dolibarrpy.egg-info/SOURCES.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-20 15:13:39.000000 dolibarrpy-0.2.4/dolibarrpy.egg-info/dependency_links.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-20 15:13:39.000000 dolibarrpy-0.2.4/dolibarrpy.egg-info/top_level.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-20 15:13:39.048079 dolibarrpy-0.2.4/setup.cfg
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1040 2024-04-20 15:13:31.000000 dolibarrpy-0.2.4/setup.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 16:05:03.039609 dolibarrpy-0.2.5/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.2.5/LICENSE.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 16:05:03.039742 dolibarrpy-0.2.5/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.2.5/README.md
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 16:05:03.036744 dolibarrpy-0.2.5/dolibarrpy/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)    15042 2024-04-20 16:03:28.000000 dolibarrpy-0.2.5/dolibarrpy/Dolibarrpy.py
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.2.5/dolibarrpy/__init__.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-20 16:05:03.039348 dolibarrpy-0.2.5/dolibarrpy.egg-info/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      647 2024-04-20 16:05:03.000000 dolibarrpy-0.2.5/dolibarrpy.egg-info/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-20 16:05:03.000000 dolibarrpy-0.2.5/dolibarrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-20 16:05:03.000000 dolibarrpy-0.2.5/dolibarrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-20 16:05:03.000000 dolibarrpy-0.2.5/dolibarrpy.egg-info/top_level.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-20 16:05:03.040189 dolibarrpy-0.2.5/setup.cfg
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1040 2024-04-20 16:04:45.000000 dolibarrpy-0.2.5/setup.py
```

### Comparing `dolibarrpy-0.2.4/LICENSE.txt` & `dolibarrpy-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dolibarrpy-0.2.4/PKG-INFO` & `dolibarrpy-0.2.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.2.4/dolibarrpy/Dolibarrpy.py` & `dolibarrpy-0.2.5/dolibarrpy/Dolibarrpy.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,24 @@
     limit: Optional[int] = None
     page: Optional[int] = None
     thirdparty_ids: Optional[str] = None
     category: Optional[str] = None  # Type of category ('member', 'customer', 'supplier', 'product', 'contact')
     sqlfilters: Optional[str] = None    # Syntax example "(t.statut:=:1)
     properties: Optional[str] = None        # Restrict the data returned to theses properties. Ignored if empty. Comma separated list of properties names
 
+@dataclass
+class MemberFilter():
+    sortfield: Optional[str] = None
+    sortorder: Optional[str] = None
+    limit: Optional[int] = None
+    page: Optional[int] = None          # page number
+    typeid: Optional[str] = None        # only get members with this thirdparty_id
+    category: Optional[int] = None        # only get members with this status: draft | unpaid | paid | cancelled
+    sqlfilters: Optional[str] = None    # (t.email:like:'john.doe@example.com')
+    properties: Optional[str] = None    # Restrict the data returned to these properties. Ignored if empty. Comma separated list of properties names
 
 class Dolibarrpy():
     url = 'https://dolibarr.example.com/api/index.php/'
     token = 'your token'
     timeout = 16
     debug = False
 
@@ -46,14 +56,18 @@
         }
 
 
     def call_list_api(self, object, params={}):
         url = self.url + object
         headers = self.get_headers()
         response = requests.get(url, params=params, headers=headers, timeout=self.timeout)
+        if self.debug:
+            ic(url)
+            ic(params)
+            ic(response)
         try:
             result = json.loads(response.text)
         except:
             _logger.error('LIST API ERROR: ' + object)
             result = response.text
         return result
 
@@ -261,15 +275,15 @@
         result = self.call_get_api('factory', objid=objid)
         return result
 
     # PROJECTS
     def find_all_projects(self, with_status = ''):
         """
         Get projects with status
-        @param status: 0 => draft, 1 => open, 2=> closed
+        @param with_status: 0 => draft, 1 => open, 2=> closed
         @return: list of projects
         """
         all_projects=[]
         page = 0
         some_projects = self.find_some_projects(with_status, page)
         while some_projects:
             all_projects = all_projects + list(some_projects)
@@ -372,7 +386,48 @@
             return result
         elif email_msgid == '':
             raise Exception("email_msgid can not be empty")
         elif email_msgid is None:
             raise Exception("email_msgid can not be None")
         else:
             raise Exception("email_msgid is wrong")
+
+
+    # MEMBERS
+    def find_all_members(self, from_MemberFilter = None):
+        """
+        Get members with status
+        @param from_MemberFilter: 0 => draft, 1 => open, 2=> closed
+        @return: list of members
+        """
+        if self.debug:
+            ic()
+            ic(from_MemberFilter)
+        if from_MemberFilter is None:
+            search_filter = MemberFilter()
+        else:
+            search_filter = from_MemberFilter
+        all_members=[]
+        page = 0
+        some_members = self.find_some_members(search_filter, page)
+        while some_members:
+            all_members = all_members + list(some_members)
+            page += 1
+            some_members = self.find_some_members(search_filter, page)
+            if len(some_members) < 100:
+                all_members = all_members + list(some_members)
+                break
+        return all_members
+
+    def find_some_members(self, from_MemberFilter = None, page = 0):
+        if self.debug:
+            ic()
+            ic(page)
+            ic(from_MemberFilter)
+        if from_MemberFilter is None:
+            search_filter = MemberFilter()
+        else:
+            search_filter = from_MemberFilter
+        search_filter.page = page
+        params = asdict(search_filter)
+        result = self.call_list_api('members', params=params)
+        return result
```

### Comparing `dolibarrpy-0.2.4/dolibarrpy.egg-info/PKG-INFO` & `dolibarrpy-0.2.5/dolibarrpy.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: Python wrapper for Dolibarr
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.2.4/setup.py` & `dolibarrpy-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 import os
 
 setup(
     name='dolibarrpy',
     packages=['dolibarrpy'],
-    version="0.2.4",
+    version="0.2.5",
     license='MIT',
     description='Python wrapper for Dolibarr API',
     long_description='Python wrapper for Dolibarr',
     long_description_content_type='text/markdown',
     author='Jon Bendtsen',
     author_email='jon.bendtsen.github@jonb.dk',
     url='https://github.com/JonBendtsen/dolibarrpy.git',
```

