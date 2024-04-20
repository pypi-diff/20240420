# Comparing `tmp/scratchattach-1.6.8.tar.gz` & `tmp/scratchattach-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.6.8.tar", last modified: Sat Apr 20 01:09:13 2024, max compression
+gzip compressed data, was "scratchattach-1.6.9.tar", last modified: Sat Apr 20 01:15:13 2024, max compression
```

## Comparing `scratchattach-1.6.8.tar` & `scratchattach-1.6.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 01:09:13.095292 scratchattach-1.6.8/
--rw-rw-rw-   0        0        0     1101 2023-09-02 14:18:05.000000 scratchattach-1.6.8/LICENSE
--rw-rw-rw-   0        0        0     4267 2024-04-20 01:09:13.095292 scratchattach-1.6.8/PKG-INFO
--rw-rw-rw-   0        0        0     3534 2024-04-20 01:08:36.000000 scratchattach-1.6.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 01:09:13.079289 scratchattach-1.6.8/scratchattach/
--rw-rw-rw-   0        0        0     2719 2023-09-16 14:17:22.000000 scratchattach-1.6.8/scratchattach/__init__.py
--rw-rw-rw-   0        0        0    23390 2024-04-20 01:06:34.000000 scratchattach-1.6.8/scratchattach/cloud.py
--rw-rw-rw-   0        0        0    25262 2024-04-20 01:08:11.000000 scratchattach-1.6.8/scratchattach/cloud_requests.py
--rw-rw-rw-   0        0        0     2600 2024-04-16 18:08:07.000000 scratchattach-1.6.8/scratchattach/encoder.py
--rw-rw-rw-   0        0        0     4221 2023-10-25 12:34:35.000000 scratchattach-1.6.8/scratchattach/exceptions.py
--rw-rw-rw-   0        0        0    10508 2023-09-04 01:29:36.000000 scratchattach-1.6.8/scratchattach/forum.py
--rw-rw-rw-   0        0        0    31197 2024-04-16 18:33:18.000000 scratchattach-1.6.8/scratchattach/project.py
--rw-rw-rw-   0        0        0    22058 2024-04-19 12:52:22.000000 scratchattach-1.6.8/scratchattach/session.py
--rw-rw-rw-   0        0        0    20487 2024-04-16 18:08:07.000000 scratchattach-1.6.8/scratchattach/studio.py
--rw-rw-rw-   0        0        0    34892 2023-11-24 17:38:57.000000 scratchattach-1.6.8/scratchattach/user.py
-drwxrwxrwx   0        0        0        0 2024-04-20 01:09:13.094292 scratchattach-1.6.8/scratchattach.egg-info/
--rw-rw-rw-   0        0        0     4267 2024-04-20 01:09:12.000000 scratchattach-1.6.8/scratchattach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2024-04-20 01:09:13.000000 scratchattach-1.6.8/scratchattach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 01:09:12.000000 scratchattach-1.6.8/scratchattach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-20 01:09:12.000000 scratchattach-1.6.8/scratchattach.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-20 01:09:12.000000 scratchattach-1.6.8/scratchattach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 01:09:13.095292 scratchattach-1.6.8/setup.cfg
--rw-rw-rw-   0        0        0     1108 2024-04-20 01:08:44.000000 scratchattach-1.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 01:15:13.384319 scratchattach-1.6.9/
+-rw-rw-rw-   0        0        0     1101 2023-09-02 14:18:05.000000 scratchattach-1.6.9/LICENSE
+-rw-rw-rw-   0        0        0     4267 2024-04-20 01:15:13.383320 scratchattach-1.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3534 2024-04-20 01:08:36.000000 scratchattach-1.6.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 01:15:13.363314 scratchattach-1.6.9/scratchattach/
+-rw-rw-rw-   0        0        0     2719 2023-09-16 14:17:22.000000 scratchattach-1.6.9/scratchattach/__init__.py
+-rw-rw-rw-   0        0        0    23324 2024-04-20 01:14:35.000000 scratchattach-1.6.9/scratchattach/cloud.py
+-rw-rw-rw-   0        0        0    25262 2024-04-20 01:14:31.000000 scratchattach-1.6.9/scratchattach/cloud_requests.py
+-rw-rw-rw-   0        0        0     2600 2024-04-16 18:08:07.000000 scratchattach-1.6.9/scratchattach/encoder.py
+-rw-rw-rw-   0        0        0     4221 2023-10-25 12:34:35.000000 scratchattach-1.6.9/scratchattach/exceptions.py
+-rw-rw-rw-   0        0        0    10508 2023-09-04 01:29:36.000000 scratchattach-1.6.9/scratchattach/forum.py
+-rw-rw-rw-   0        0        0    31197 2024-04-16 18:33:18.000000 scratchattach-1.6.9/scratchattach/project.py
+-rw-rw-rw-   0        0        0    22058 2024-04-19 12:52:22.000000 scratchattach-1.6.9/scratchattach/session.py
+-rw-rw-rw-   0        0        0    20487 2024-04-16 18:08:07.000000 scratchattach-1.6.9/scratchattach/studio.py
+-rw-rw-rw-   0        0        0    34892 2023-11-24 17:38:57.000000 scratchattach-1.6.9/scratchattach/user.py
+drwxrwxrwx   0        0        0        0 2024-04-20 01:15:13.382319 scratchattach-1.6.9/scratchattach.egg-info/
+-rw-rw-rw-   0        0        0     4267 2024-04-20 01:15:13.000000 scratchattach-1.6.9/scratchattach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2024-04-20 01:15:13.000000 scratchattach-1.6.9/scratchattach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 01:15:13.000000 scratchattach-1.6.9/scratchattach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-20 01:15:13.000000 scratchattach-1.6.9/scratchattach.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-20 01:15:13.000000 scratchattach-1.6.9/scratchattach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 01:15:13.384319 scratchattach-1.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2024-04-20 01:15:00.000000 scratchattach-1.6.9/setup.py
```

### Comparing `scratchattach-1.6.8/LICENSE` & `scratchattach-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.8/PKG-INFO` & `scratchattach-1.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.6.8
+Version: 1.6.9
 Summary: An Scratch API Wrapper for scra tch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timkrome2006@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchattach-1.6.8/README.md` & `scratchattach-1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.8/scratchattach/__init__.py` & `scratchattach-1.6.9/scratchattach/__init__.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.8/scratchattach/cloud.py` & `scratchattach-1.6.9/scratchattach/cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
         except ValueError: #non-numeric project id (possible on turbowarp's cloud server)
             self.project_id = str(project_id)
         self._ratelimited_until = 0 #deals with the 0.1 second rate limit for cloud variable sets
         self._connect_timestamp = 0 #timestamp of when the cloud connection was opened
         self._ws_timeout = _ws_timeout
 
         # user agent information (for connecting to TurboWarp's cloud servers)
-        self.user_agent_purpose = purpose
-        self.user_agent_contact = contact
+        self.purpose = purpose
+        self.contact = contact
 
         self.websocket = websocket.WebSocket()
         self._connect(cloud_host=cloud_host)
         self._handshake()
         self.cloud_host = cloud_host
         self.allow_non_numeric = _allow_non_numeric #TurboWarp only. If this is true, turbowarp cloud variables can be set to non-numeric values (if the cloud_host wss allows it)
 
@@ -164,16 +164,16 @@
 
     def _connect(self, *, cloud_host=None):
         try:
             if cloud_host is None:
                 cloud_host = "wss://clouddata.turbowarp.org/"
                 self.cloud_host = cloud_host
             purpose_string = ""
-            if self.user_agent_purpose != "" or self.user_agent_contact != "":
-                purpose_string = f" (Purpose:{self.user_agent_purpose}; Contact:{self.user_agent_contact})"
+            if self.purpose != "" or self.contact != "":
+                purpose_string = f" (Purpose:{self.purpose}; Contact:{self.contact})"
             self.websocket.connect(
                 cloud_host,
                 enable_multithread=True,
                 timeout = self._ws_timeout,
                 header = {"User-Agent":f"scratchattach/1.6.6{purpose_string}" if self._ws_timeout is None else f"scratchattach/1.6.6 (short-term connection){purpose_string}"}
             )
         except Exception:
```

### Comparing `scratchattach-1.6.8/scratchattach/cloud_requests.py` & `scratchattach-1.6.9/scratchattach/cloud_requests.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.8/scratchattach/encoder.py` & `scratchattach-1.6.9/scratchattach/encoder.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.8/scratchattach/exceptions.py` & `scratchattach-1.6.9/scratchattach/exceptions.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.8/scratchattach/forum.py` & `scratchattach-1.6.9/scratchattach/forum.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.8/scratchattach/project.py` & `scratchattach-1.6.9/scratchattach/project.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.8/scratchattach/session.py` & `scratchattach-1.6.9/scratchattach/session.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.8/scratchattach/studio.py` & `scratchattach-1.6.9/scratchattach/studio.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.8/scratchattach/user.py` & `scratchattach-1.6.9/scratchattach/user.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.8/scratchattach.egg-info/PKG-INFO` & `scratchattach-1.6.9/scratchattach.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.6.8
+Version: 1.6.9
 Summary: An Scratch API Wrapper for scra tch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timkrome2006@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchattach-1.6.8/setup.py` & `scratchattach-1.6.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.6.8'
+VERSION = '1.6.9'
 DESCRIPTION = 'An Scratch API Wrapper for scra tch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchattach",
     version=VERSION,
```

