# Comparing `tmp/scratchattach-1.6.9.tar.gz` & `tmp/scratchattach-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.6.9.tar", last modified: Sat Apr 20 01:15:13 2024, max compression
+gzip compressed data, was "scratchattach-1.7.0.tar", last modified: Sat Apr 20 01:31:44 2024, max compression
```

## Comparing `scratchattach-1.6.9.tar` & `scratchattach-1.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 01:15:13.384319 scratchattach-1.6.9/
--rw-rw-rw-   0        0        0     1101 2023-09-02 14:18:05.000000 scratchattach-1.6.9/LICENSE
--rw-rw-rw-   0        0        0     4267 2024-04-20 01:15:13.383320 scratchattach-1.6.9/PKG-INFO
--rw-rw-rw-   0        0        0     3534 2024-04-20 01:08:36.000000 scratchattach-1.6.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 01:15:13.363314 scratchattach-1.6.9/scratchattach/
--rw-rw-rw-   0        0        0     2719 2023-09-16 14:17:22.000000 scratchattach-1.6.9/scratchattach/__init__.py
--rw-rw-rw-   0        0        0    23324 2024-04-20 01:14:35.000000 scratchattach-1.6.9/scratchattach/cloud.py
--rw-rw-rw-   0        0        0    25262 2024-04-20 01:14:31.000000 scratchattach-1.6.9/scratchattach/cloud_requests.py
--rw-rw-rw-   0        0        0     2600 2024-04-16 18:08:07.000000 scratchattach-1.6.9/scratchattach/encoder.py
--rw-rw-rw-   0        0        0     4221 2023-10-25 12:34:35.000000 scratchattach-1.6.9/scratchattach/exceptions.py
--rw-rw-rw-   0        0        0    10508 2023-09-04 01:29:36.000000 scratchattach-1.6.9/scratchattach/forum.py
--rw-rw-rw-   0        0        0    31197 2024-04-16 18:33:18.000000 scratchattach-1.6.9/scratchattach/project.py
--rw-rw-rw-   0        0        0    22058 2024-04-19 12:52:22.000000 scratchattach-1.6.9/scratchattach/session.py
--rw-rw-rw-   0        0        0    20487 2024-04-16 18:08:07.000000 scratchattach-1.6.9/scratchattach/studio.py
--rw-rw-rw-   0        0        0    34892 2023-11-24 17:38:57.000000 scratchattach-1.6.9/scratchattach/user.py
-drwxrwxrwx   0        0        0        0 2024-04-20 01:15:13.382319 scratchattach-1.6.9/scratchattach.egg-info/
--rw-rw-rw-   0        0        0     4267 2024-04-20 01:15:13.000000 scratchattach-1.6.9/scratchattach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2024-04-20 01:15:13.000000 scratchattach-1.6.9/scratchattach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 01:15:13.000000 scratchattach-1.6.9/scratchattach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-20 01:15:13.000000 scratchattach-1.6.9/scratchattach.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-20 01:15:13.000000 scratchattach-1.6.9/scratchattach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 01:15:13.384319 scratchattach-1.6.9/setup.cfg
--rw-rw-rw-   0        0        0     1108 2024-04-20 01:15:00.000000 scratchattach-1.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 01:31:44.246796 scratchattach-1.7.0/
+-rw-rw-rw-   0        0        0     1101 2023-09-02 14:18:05.000000 scratchattach-1.7.0/LICENSE
+-rw-rw-rw-   0        0        0     4267 2024-04-20 01:31:44.246796 scratchattach-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3534 2024-04-20 01:08:36.000000 scratchattach-1.7.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 01:31:44.229791 scratchattach-1.7.0/scratchattach/
+-rw-rw-rw-   0        0        0     2719 2023-09-16 14:17:22.000000 scratchattach-1.7.0/scratchattach/__init__.py
+-rw-rw-rw-   0        0        0    23324 2024-04-20 01:14:35.000000 scratchattach-1.7.0/scratchattach/cloud.py
+-rw-rw-rw-   0        0        0    25376 2024-04-20 01:30:55.000000 scratchattach-1.7.0/scratchattach/cloud_requests.py
+-rw-rw-rw-   0        0        0     2600 2024-04-16 18:08:07.000000 scratchattach-1.7.0/scratchattach/encoder.py
+-rw-rw-rw-   0        0        0     4221 2023-10-25 12:34:35.000000 scratchattach-1.7.0/scratchattach/exceptions.py
+-rw-rw-rw-   0        0        0    10508 2023-09-04 01:29:36.000000 scratchattach-1.7.0/scratchattach/forum.py
+-rw-rw-rw-   0        0        0    31197 2024-04-16 18:33:18.000000 scratchattach-1.7.0/scratchattach/project.py
+-rw-rw-rw-   0        0        0    22058 2024-04-19 12:52:22.000000 scratchattach-1.7.0/scratchattach/session.py
+-rw-rw-rw-   0        0        0    20487 2024-04-16 18:08:07.000000 scratchattach-1.7.0/scratchattach/studio.py
+-rw-rw-rw-   0        0        0    34892 2023-11-24 17:38:57.000000 scratchattach-1.7.0/scratchattach/user.py
+drwxrwxrwx   0        0        0        0 2024-04-20 01:31:44.245795 scratchattach-1.7.0/scratchattach.egg-info/
+-rw-rw-rw-   0        0        0     4267 2024-04-20 01:31:44.000000 scratchattach-1.7.0/scratchattach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2024-04-20 01:31:44.000000 scratchattach-1.7.0/scratchattach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 01:31:44.000000 scratchattach-1.7.0/scratchattach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-20 01:31:44.000000 scratchattach-1.7.0/scratchattach.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-20 01:31:44.000000 scratchattach-1.7.0/scratchattach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 01:31:44.246796 scratchattach-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2024-04-20 01:31:31.000000 scratchattach-1.7.0/setup.py
```

### Comparing `scratchattach-1.6.9/LICENSE` & `scratchattach-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.9/PKG-INFO` & `scratchattach-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.6.9
+Version: 1.7.0
 Summary: An Scratch API Wrapper for scra tch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timkrome2006@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchattach-1.6.9/README.md` & `scratchattach-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.9/scratchattach/__init__.py` & `scratchattach-1.7.0/scratchattach/__init__.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.9/scratchattach/cloud.py` & `scratchattach-1.7.0/scratchattach/cloud.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.9/scratchattach/cloud_requests.py` & `scratchattach-1.7.0/scratchattach/cloud_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,17 @@
             return None
 
     def _respond(self, request_id, response, limit, *, validation=2222):
         """
         Sends back the request response to the Scratch project
         """
 
-        if self.idle_since + 8 < time.time() or self.force_reconnect:
+        if (self.idle_since + 8 < time.time() and not isinstance(self.connection, cloud.TwCloudConnection)
+            ) or self.force_reconnect:
+            self.connection.close()
             self.connection._connect(cloud_host=self.connection.cloud_host)
             self.connection._handshake()
 
         remaining_response = str(response)
 
         i = 0
         while not remaining_response == "":
```

### Comparing `scratchattach-1.6.9/scratchattach/encoder.py` & `scratchattach-1.7.0/scratchattach/encoder.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.9/scratchattach/exceptions.py` & `scratchattach-1.7.0/scratchattach/exceptions.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.9/scratchattach/forum.py` & `scratchattach-1.7.0/scratchattach/forum.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.9/scratchattach/project.py` & `scratchattach-1.7.0/scratchattach/project.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.9/scratchattach/session.py` & `scratchattach-1.7.0/scratchattach/session.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.9/scratchattach/studio.py` & `scratchattach-1.7.0/scratchattach/studio.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.9/scratchattach/user.py` & `scratchattach-1.7.0/scratchattach/user.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.9/scratchattach.egg-info/PKG-INFO` & `scratchattach-1.7.0/scratchattach.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.6.9
+Version: 1.7.0
 Summary: An Scratch API Wrapper for scra tch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timkrome2006@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchattach-1.6.9/setup.py` & `scratchattach-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.6.9'
+VERSION = '1.7.0'
 DESCRIPTION = 'An Scratch API Wrapper for scra tch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchattach",
     version=VERSION,
```

