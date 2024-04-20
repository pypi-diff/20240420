# Comparing `tmp/scratchattach-1.6.6.tar.gz` & `tmp/scratchattach-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.6.6.tar", last modified: Fri Apr 19 13:11:25 2024, max compression
+gzip compressed data, was "scratchattach-1.6.7.tar", last modified: Fri Apr 19 17:44:47 2024, max compression
```

## Comparing `scratchattach-1.6.6.tar` & `scratchattach-1.6.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 13:11:25.965941 scratchattach-1.6.6/
--rw-rw-rw-   0        0        0     1101 2023-09-02 14:18:05.000000 scratchattach-1.6.6/LICENSE
--rw-rw-rw-   0        0        0     4042 2024-04-19 13:11:25.965941 scratchattach-1.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     3309 2023-09-04 01:43:11.000000 scratchattach-1.6.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 13:11:25.948937 scratchattach-1.6.6/scratchattach/
--rw-rw-rw-   0        0        0     2719 2023-09-16 14:17:22.000000 scratchattach-1.6.6/scratchattach/__init__.py
--rw-rw-rw-   0        0        0    22391 2024-04-19 13:08:19.000000 scratchattach-1.6.6/scratchattach/cloud.py
--rw-rw-rw-   0        0        0    25085 2024-04-19 13:04:10.000000 scratchattach-1.6.6/scratchattach/cloud_requests.py
--rw-rw-rw-   0        0        0     2600 2024-04-16 18:08:07.000000 scratchattach-1.6.6/scratchattach/encoder.py
--rw-rw-rw-   0        0        0     4221 2023-10-25 12:34:35.000000 scratchattach-1.6.6/scratchattach/exceptions.py
--rw-rw-rw-   0        0        0    10508 2023-09-04 01:29:36.000000 scratchattach-1.6.6/scratchattach/forum.py
--rw-rw-rw-   0        0        0    31197 2024-04-16 18:33:18.000000 scratchattach-1.6.6/scratchattach/project.py
--rw-rw-rw-   0        0        0    22058 2024-04-19 12:52:22.000000 scratchattach-1.6.6/scratchattach/session.py
--rw-rw-rw-   0        0        0    20487 2024-04-16 18:08:07.000000 scratchattach-1.6.6/scratchattach/studio.py
--rw-rw-rw-   0        0        0    34892 2023-11-24 17:38:57.000000 scratchattach-1.6.6/scratchattach/user.py
-drwxrwxrwx   0        0        0        0 2024-04-19 13:11:25.964941 scratchattach-1.6.6/scratchattach.egg-info/
--rw-rw-rw-   0        0        0     4042 2024-04-19 13:11:25.000000 scratchattach-1.6.6/scratchattach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2024-04-19 13:11:25.000000 scratchattach-1.6.6/scratchattach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 13:11:25.000000 scratchattach-1.6.6/scratchattach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-19 13:11:25.000000 scratchattach-1.6.6/scratchattach.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-19 13:11:25.000000 scratchattach-1.6.6/scratchattach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 13:11:25.965941 scratchattach-1.6.6/setup.cfg
--rw-rw-rw-   0        0        0     1108 2024-04-19 12:33:08.000000 scratchattach-1.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:44:47.994082 scratchattach-1.6.7/
+-rw-rw-rw-   0        0        0     1101 2023-09-02 14:18:05.000000 scratchattach-1.6.7/LICENSE
+-rw-rw-rw-   0        0        0     4042 2024-04-19 17:44:47.994082 scratchattach-1.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3309 2023-09-04 01:43:11.000000 scratchattach-1.6.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 17:44:47.976951 scratchattach-1.6.7/scratchattach/
+-rw-rw-rw-   0        0        0     2719 2023-09-16 14:17:22.000000 scratchattach-1.6.7/scratchattach/__init__.py
+-rw-rw-rw-   0        0        0    23213 2024-04-19 17:44:12.000000 scratchattach-1.6.7/scratchattach/cloud.py
+-rw-rw-rw-   0        0        0    25211 2024-04-19 17:43:38.000000 scratchattach-1.6.7/scratchattach/cloud_requests.py
+-rw-rw-rw-   0        0        0     2600 2024-04-16 18:08:07.000000 scratchattach-1.6.7/scratchattach/encoder.py
+-rw-rw-rw-   0        0        0     4221 2023-10-25 12:34:35.000000 scratchattach-1.6.7/scratchattach/exceptions.py
+-rw-rw-rw-   0        0        0    10508 2023-09-04 01:29:36.000000 scratchattach-1.6.7/scratchattach/forum.py
+-rw-rw-rw-   0        0        0    31197 2024-04-16 18:33:18.000000 scratchattach-1.6.7/scratchattach/project.py
+-rw-rw-rw-   0        0        0    22058 2024-04-19 12:52:22.000000 scratchattach-1.6.7/scratchattach/session.py
+-rw-rw-rw-   0        0        0    20487 2024-04-16 18:08:07.000000 scratchattach-1.6.7/scratchattach/studio.py
+-rw-rw-rw-   0        0        0    34892 2023-11-24 17:38:57.000000 scratchattach-1.6.7/scratchattach/user.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:44:47.992080 scratchattach-1.6.7/scratchattach.egg-info/
+-rw-rw-rw-   0        0        0     4042 2024-04-19 17:44:47.000000 scratchattach-1.6.7/scratchattach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2024-04-19 17:44:47.000000 scratchattach-1.6.7/scratchattach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 17:44:47.000000 scratchattach-1.6.7/scratchattach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-19 17:44:47.000000 scratchattach-1.6.7/scratchattach.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-19 17:44:47.000000 scratchattach-1.6.7/scratchattach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 17:44:47.994082 scratchattach-1.6.7/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2024-04-19 17:44:40.000000 scratchattach-1.6.7/setup.py
```

### Comparing `scratchattach-1.6.6/LICENSE` & `scratchattach-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.6/PKG-INFO` & `scratchattach-1.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.6.6
+Version: 1.6.7
 Summary: An Scratch API Wrapper for scra tch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timkrome2006@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchattach-1.6.6/README.md` & `scratchattach-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.6/scratchattach/__init__.py` & `scratchattach-1.6.7/scratchattach/__init__.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.6/scratchattach/cloud.py` & `scratchattach-1.6.7/scratchattach/cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -332,14 +332,15 @@
     """
     def __init__(self, project_id, **entries):
         self.__dict__.update(entries)
         if not "purpose" in entries:
             self.purpose = ""
         if not "contact" in entries:
             self.contact = ""
+            print("Warning: You connected to TurboWarp's cloud without giving the `contact` argument.\nTurboWarp would like to you to identify yourself by providing a way you can be contacted (like your Scratch account for example): TwCloudEvents('project_id', contact='your_contact_info')\nThis is optional at the moment, but it helps TurboWarp to understand who is using their cloud service.")
         cloud_connection = TwCloudConnection(project_id=project_id, purpose=self.purpose, contact=self.contact)
         self.data = []
         self._thread = None
         self.running = False
         self._events = {}
         self.connection = cloud_connection
 
@@ -543,18 +544,21 @@
     Connects to TurboWarp's cloud websocket.
 
     Args:
         project_id (str)
     
     Keyword Arguments:
         purpose (str): (optional) Provide information about what you're using TurboWarp's cloud server for
-        contact (str): (optional) Provide an email address or another way you can be contacted
+        contact (str): (optional) Provide your Scratch account or another way you can be contacted
 
     Returns:
         scratchattach.cloud.TwCloudConnection: An object that represents a connection to TurboWarp's cloud server
     """
     if project_id is None:
         project_id = project_id_arg
     if project_id is None:
         return None
 
+    if contact == "":
+        print("Warning: You connected to TurboWarp's cloud without giving the `contact` argument.\nTurboWarp would like to you to identify yourself by providing a way you can be contacted (like your Scratch account for example): connect_tw_cloud('project_id', contact='your_contact_info')\nThis is optional at the moment, but it helps TurboWarp to understand who is using their cloud service.")
+
     return TwCloudConnection(project_id = project_id, purpose=purpose, contact=contact)
```

### Comparing `scratchattach-1.6.6/scratchattach/cloud_requests.py` & `scratchattach-1.6.7/scratchattach/cloud_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -552,16 +552,14 @@
     Framework (inspired by discord.py) that allows TurboWarp cloud variables and Python to communicate. More information: https://github.com/TimMcCool/scratchattach/wiki/Cloud-Requests
     """
     def __init__(self,
                  cloud_connection,
                  *,
                  used_cloud_vars=["1", "2", "3", "4", "5", "6", "7", "8", "9"],
                  ignore_exceptions=True,
-                 purpose="",
-                 contact="",
                  _force_reconnect = False, # this argument is no longer used and only exists for backwards compatibility
                  _packet_length=98800):
         print(
             "\033[1mIf you use CloudRequests in your Scratch project, please credit TimMcCool!\033[0m"
         )
         if _packet_length > 98800:
             warnings.warn(
@@ -571,16 +569,20 @@
         self.connection = cloud_connection
         self.project_id = cloud_connection.project_id
 
         self.ignore_exceptions = ignore_exceptions
         self.packet_length = _packet_length
 
         # user agent data
-        self.purpose = purpose
-        self.contact = contact
+        if isinstance(cloud_connection, cloud.TwCloudConnection):
+            self.purpose = cloud_connection.purpose
+            self.contact = cloud_connection.contact
+        else:
+            self.purpose = ""
+            self.contact = ""
 
         self.init_attributes()
 
     def get_requester(self):
         return None
 
     def run(self,
```

### Comparing `scratchattach-1.6.6/scratchattach/encoder.py` & `scratchattach-1.6.7/scratchattach/encoder.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.6/scratchattach/exceptions.py` & `scratchattach-1.6.7/scratchattach/exceptions.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.6/scratchattach/forum.py` & `scratchattach-1.6.7/scratchattach/forum.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.6/scratchattach/project.py` & `scratchattach-1.6.7/scratchattach/project.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.6/scratchattach/session.py` & `scratchattach-1.6.7/scratchattach/session.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.6/scratchattach/studio.py` & `scratchattach-1.6.7/scratchattach/studio.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.6/scratchattach/user.py` & `scratchattach-1.6.7/scratchattach/user.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.6/scratchattach.egg-info/PKG-INFO` & `scratchattach-1.6.7/scratchattach.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.6.6
+Version: 1.6.7
 Summary: An Scratch API Wrapper for scra tch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timkrome2006@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchattach-1.6.6/setup.py` & `scratchattach-1.6.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.6.6'
+VERSION = '1.6.7'
 DESCRIPTION = 'An Scratch API Wrapper for scra tch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchattach",
     version=VERSION,
```

