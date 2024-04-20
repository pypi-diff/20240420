# Comparing `tmp/scratchattach-1.6.7.tar.gz` & `tmp/scratchattach-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.6.7.tar", last modified: Fri Apr 19 17:44:47 2024, max compression
+gzip compressed data, was "scratchattach-1.6.8.tar", last modified: Sat Apr 20 01:09:13 2024, max compression
```

## Comparing `scratchattach-1.6.7.tar` & `scratchattach-1.6.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 17:44:47.994082 scratchattach-1.6.7/
--rw-rw-rw-   0        0        0     1101 2023-09-02 14:18:05.000000 scratchattach-1.6.7/LICENSE
--rw-rw-rw-   0        0        0     4042 2024-04-19 17:44:47.994082 scratchattach-1.6.7/PKG-INFO
--rw-rw-rw-   0        0        0     3309 2023-09-04 01:43:11.000000 scratchattach-1.6.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 17:44:47.976951 scratchattach-1.6.7/scratchattach/
--rw-rw-rw-   0        0        0     2719 2023-09-16 14:17:22.000000 scratchattach-1.6.7/scratchattach/__init__.py
--rw-rw-rw-   0        0        0    23213 2024-04-19 17:44:12.000000 scratchattach-1.6.7/scratchattach/cloud.py
--rw-rw-rw-   0        0        0    25211 2024-04-19 17:43:38.000000 scratchattach-1.6.7/scratchattach/cloud_requests.py
--rw-rw-rw-   0        0        0     2600 2024-04-16 18:08:07.000000 scratchattach-1.6.7/scratchattach/encoder.py
--rw-rw-rw-   0        0        0     4221 2023-10-25 12:34:35.000000 scratchattach-1.6.7/scratchattach/exceptions.py
--rw-rw-rw-   0        0        0    10508 2023-09-04 01:29:36.000000 scratchattach-1.6.7/scratchattach/forum.py
--rw-rw-rw-   0        0        0    31197 2024-04-16 18:33:18.000000 scratchattach-1.6.7/scratchattach/project.py
--rw-rw-rw-   0        0        0    22058 2024-04-19 12:52:22.000000 scratchattach-1.6.7/scratchattach/session.py
--rw-rw-rw-   0        0        0    20487 2024-04-16 18:08:07.000000 scratchattach-1.6.7/scratchattach/studio.py
--rw-rw-rw-   0        0        0    34892 2023-11-24 17:38:57.000000 scratchattach-1.6.7/scratchattach/user.py
-drwxrwxrwx   0        0        0        0 2024-04-19 17:44:47.992080 scratchattach-1.6.7/scratchattach.egg-info/
--rw-rw-rw-   0        0        0     4042 2024-04-19 17:44:47.000000 scratchattach-1.6.7/scratchattach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2024-04-19 17:44:47.000000 scratchattach-1.6.7/scratchattach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 17:44:47.000000 scratchattach-1.6.7/scratchattach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-19 17:44:47.000000 scratchattach-1.6.7/scratchattach.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-19 17:44:47.000000 scratchattach-1.6.7/scratchattach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 17:44:47.994082 scratchattach-1.6.7/setup.cfg
--rw-rw-rw-   0        0        0     1108 2024-04-19 17:44:40.000000 scratchattach-1.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 01:09:13.095292 scratchattach-1.6.8/
+-rw-rw-rw-   0        0        0     1101 2023-09-02 14:18:05.000000 scratchattach-1.6.8/LICENSE
+-rw-rw-rw-   0        0        0     4267 2024-04-20 01:09:13.095292 scratchattach-1.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3534 2024-04-20 01:08:36.000000 scratchattach-1.6.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 01:09:13.079289 scratchattach-1.6.8/scratchattach/
+-rw-rw-rw-   0        0        0     2719 2023-09-16 14:17:22.000000 scratchattach-1.6.8/scratchattach/__init__.py
+-rw-rw-rw-   0        0        0    23390 2024-04-20 01:06:34.000000 scratchattach-1.6.8/scratchattach/cloud.py
+-rw-rw-rw-   0        0        0    25262 2024-04-20 01:08:11.000000 scratchattach-1.6.8/scratchattach/cloud_requests.py
+-rw-rw-rw-   0        0        0     2600 2024-04-16 18:08:07.000000 scratchattach-1.6.8/scratchattach/encoder.py
+-rw-rw-rw-   0        0        0     4221 2023-10-25 12:34:35.000000 scratchattach-1.6.8/scratchattach/exceptions.py
+-rw-rw-rw-   0        0        0    10508 2023-09-04 01:29:36.000000 scratchattach-1.6.8/scratchattach/forum.py
+-rw-rw-rw-   0        0        0    31197 2024-04-16 18:33:18.000000 scratchattach-1.6.8/scratchattach/project.py
+-rw-rw-rw-   0        0        0    22058 2024-04-19 12:52:22.000000 scratchattach-1.6.8/scratchattach/session.py
+-rw-rw-rw-   0        0        0    20487 2024-04-16 18:08:07.000000 scratchattach-1.6.8/scratchattach/studio.py
+-rw-rw-rw-   0        0        0    34892 2023-11-24 17:38:57.000000 scratchattach-1.6.8/scratchattach/user.py
+drwxrwxrwx   0        0        0        0 2024-04-20 01:09:13.094292 scratchattach-1.6.8/scratchattach.egg-info/
+-rw-rw-rw-   0        0        0     4267 2024-04-20 01:09:12.000000 scratchattach-1.6.8/scratchattach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2024-04-20 01:09:13.000000 scratchattach-1.6.8/scratchattach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 01:09:12.000000 scratchattach-1.6.8/scratchattach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-20 01:09:12.000000 scratchattach-1.6.8/scratchattach.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-20 01:09:12.000000 scratchattach-1.6.8/scratchattach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 01:09:13.095292 scratchattach-1.6.8/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2024-04-20 01:08:44.000000 scratchattach-1.6.8/setup.py
```

### Comparing `scratchattach-1.6.7/LICENSE` & `scratchattach-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.7/PKG-INFO` & `scratchattach-1.6.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.6.7
+Version: 1.6.8
 Summary: An Scratch API Wrapper for scra tch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timkrome2006@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -32,75 +32,79 @@
 # Links
 
 - **[Documentation](https://github.com/TimMcCool/scratchattach/wiki)**
 - [Extended documentation (WIP)](https://scratchattach.readthedocs.io/en/latest/)
 - [Examples](https://github.com/TimMcCool/scratchattach/wiki/Examples)
 - [Change log](https://github.com/TimMcCool/scratchattach/blob/main/CHANGELOG.md)
 
-# Contributors
-
-- Allmost all code by TimMcCool.
-- See the GitHub repository for full list of contributors.
-- Create a pull request to contribute code yourself.
+Report bugs by opening an issue on this repository. If you need help or guideance, leave a comment in the [official forum topic](https://scratch.mit.edu/discuss/topic/603418/
+). Projects made using scratchattach can be added to [this Scratch studio](https://scratch.mit.edu/studios/31478892/).
 
-# Support
+# Example usage
 
-If you need help with your code, leave a comment in the [official forum topic](https://scratch.mit.edu/discuss/topic/603418/
-) on [TimMcCool's Scratch
-profile](https://scratch.mit.edu/users/TimMcCool/) or open an issue on the github repo
+```py
+import scratchattach as scratch3
 
-# Installation
+session = scratch3.login("username", "password")
+conn = session.connect_cloud("project_id")
 
-Run the following command in your command prompt
-/ shell:
-```
-pip install -U scratchattach
+conn.set_var("variable", value)
 ```
 
-**OR**
+**[More examples](https://github.com/TimMcCool/scratchattach/wiki/Examples)**
 
-Add this to your Python code:
-```python
-import os
+# Getting started
 
-os.system("pip install -U scratchattach")
-```
+**Installation:**
 
-# Logging in  `scratch3.Session`
+Run the following command in your command prompt / shell:
+
+```
+pip install -U scratchattach
+```
 
 **Logging in with username / password:**
 
 ```python
 import scratchattach as scratch3
 
 session = scratch3.login("username", "password")
 ```
 
-`login()` returns a `Session` object that saves your login
-
-**Logging in with a sessionId:**
-*You can get your session id from your browser's cookies. [More information](https://github.com/TimMcCool/scratchattach/wiki/Get-your-session-id)*
+`login()` returns a `Session` object that saves your login.
 
+**Logging in with a sessionId:** *You can get your session id from your browser's cookies. [More information](https://github.com/TimMcCool/scratchattach/wiki/Get-your-session-id)*
 ```python
 import scratchattach as scratch3
 
 session = scratch3.Session("sessionId", username="username") #The username field is case sensitive
 ```
 
-**All scratchattach features are documented in the [documentation](https://github.com/TimMcCool/scratchattach/wiki#logging-in).**
-
-# Cloud variables  `scratch3.CloudConnection`
-
 **Connect to the Scratch cloud:**
 
 ```python
 conn = session.connect_cloud("project_id")
 ```
 
 **Get / Set a cloud var:**
 
 ```python
 value = scratch3.get_var("project_id", "variable")
 conn.set_var("variable", "value") #the variable name is specified without the cloud emoji
 ```
 
+**Follow a user / love a project:**
+
+```python
+user_to_follow = session.connect_user("username")
+user_to_follow.follow()
+project_to_love = session.connect_project("project_id")
+project_to_love.love()
+```
+
 **All scratchattach features are documented in the [documentation](https://github.com/TimMcCool/scratchattach/wiki/#cloud-variables).**
+
+# Contributors
+
+- Allmost all code by TimMcCool.
+- See the GitHub repository for full list of contributors.
+- Create a pull request to contribute code yourself.
```

### Comparing `scratchattach-1.6.7/README.md` & `scratchattach-1.6.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -15,75 +15,79 @@
 # Links
 
 - **[Documentation](https://github.com/TimMcCool/scratchattach/wiki)**
 - [Extended documentation (WIP)](https://scratchattach.readthedocs.io/en/latest/)
 - [Examples](https://github.com/TimMcCool/scratchattach/wiki/Examples)
 - [Change log](https://github.com/TimMcCool/scratchattach/blob/main/CHANGELOG.md)
 
-# Contributors
-
-- Allmost all code by TimMcCool.
-- See the GitHub repository for full list of contributors.
-- Create a pull request to contribute code yourself.
+Report bugs by opening an issue on this repository. If you need help or guideance, leave a comment in the [official forum topic](https://scratch.mit.edu/discuss/topic/603418/
+). Projects made using scratchattach can be added to [this Scratch studio](https://scratch.mit.edu/studios/31478892/).
 
-# Support
+# Example usage
 
-If you need help with your code, leave a comment in the [official forum topic](https://scratch.mit.edu/discuss/topic/603418/
-) on [TimMcCool's Scratch
-profile](https://scratch.mit.edu/users/TimMcCool/) or open an issue on the github repo
+```py
+import scratchattach as scratch3
 
-# Installation
+session = scratch3.login("username", "password")
+conn = session.connect_cloud("project_id")
 
-Run the following command in your command prompt
-/ shell:
-```
-pip install -U scratchattach
+conn.set_var("variable", value)
 ```
 
-**OR**
+**[More examples](https://github.com/TimMcCool/scratchattach/wiki/Examples)**
 
-Add this to your Python code:
-```python
-import os
+# Getting started
 
-os.system("pip install -U scratchattach")
-```
+**Installation:**
 
-# Logging in  `scratch3.Session`
+Run the following command in your command prompt / shell:
+
+```
+pip install -U scratchattach
+```
 
 **Logging in with username / password:**
 
 ```python
 import scratchattach as scratch3
 
 session = scratch3.login("username", "password")
 ```
 
-`login()` returns a `Session` object that saves your login
-
-**Logging in with a sessionId:**
-*You can get your session id from your browser's cookies. [More information](https://github.com/TimMcCool/scratchattach/wiki/Get-your-session-id)*
+`login()` returns a `Session` object that saves your login.
 
+**Logging in with a sessionId:** *You can get your session id from your browser's cookies. [More information](https://github.com/TimMcCool/scratchattach/wiki/Get-your-session-id)*
 ```python
 import scratchattach as scratch3
 
 session = scratch3.Session("sessionId", username="username") #The username field is case sensitive
 ```
 
-**All scratchattach features are documented in the [documentation](https://github.com/TimMcCool/scratchattach/wiki#logging-in).**
-
-# Cloud variables  `scratch3.CloudConnection`
-
 **Connect to the Scratch cloud:**
 
 ```python
 conn = session.connect_cloud("project_id")
 ```
 
 **Get / Set a cloud var:**
 
 ```python
 value = scratch3.get_var("project_id", "variable")
 conn.set_var("variable", "value") #the variable name is specified without the cloud emoji
 ```
 
+**Follow a user / love a project:**
+
+```python
+user_to_follow = session.connect_user("username")
+user_to_follow.follow()
+project_to_love = session.connect_project("project_id")
+project_to_love.love()
+```
+
 **All scratchattach features are documented in the [documentation](https://github.com/TimMcCool/scratchattach/wiki/#cloud-variables).**
+
+# Contributors
+
+- Allmost all code by TimMcCool.
+- See the GitHub repository for full list of contributors.
+- Create a pull request to contribute code yourself.
```

### Comparing `scratchattach-1.6.7/scratchattach/__init__.py` & `scratchattach-1.6.8/scratchattach/__init__.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.7/scratchattach/cloud.py` & `scratchattach-1.6.8/scratchattach/cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,18 +30,21 @@
 
         self.websocket = websocket.WebSocket()
         self._connect(cloud_host=cloud_host)
         self._handshake()
         self.cloud_host = cloud_host
         self.allow_non_numeric = _allow_non_numeric #TurboWarp only. If this is true, turbowarp cloud variables can be set to non-numeric values (if the cloud_host wss allows it)
 
+        self.is_closed = False # set to True after self.disconnect() is called
+
     def _send_packet(self, packet):
         self.websocket.send(json.dumps(packet) + "\n")
 
     def disconnect(self):
+        self.is_closed = True
         self.websocket.close()
 
     def _handshake(self):
         try:
             self._send_packet(
                 {"method": "handshake", "user": self._username, "project_id": self.project_id}
             )
@@ -139,14 +142,15 @@
                     self._connect(cloud_host=self.cloud_host)
                     self._handshake()
                 except Exception as e:
                     raise exceptions.ConnectionError("Connection lost while setting cloud variable.", str(e))
 
             time.sleep(0.1)
             self.set_var(variable, value)
+        self.is_closed = False
         self._ratelimited_until = time.time()
 
 class TwCloudConnection(_CloudMixin):
     """
     Represents a connection to TurboWarp's cloud variable server or a custom cloud variable server that behaves like TurboWarp's.
 
     Attributes:
@@ -170,14 +174,15 @@
                 cloud_host,
                 enable_multithread=True,
                 timeout = self._ws_timeout,
                 header = {"User-Agent":f"scratchattach/1.6.6{purpose_string}" if self._ws_timeout is None else f"scratchattach/1.6.6 (short-term connection){purpose_string}"}
             )
         except Exception:
             raise(exceptions.ConnectionError)
+        self.is_closed = False
         self._connect_timestamp = time.time()
 
 
     def set_var(self, variable, value):
         """
         Sets a cloud variable.
```

### Comparing `scratchattach-1.6.7/scratchattach/cloud_requests.py` & `scratchattach-1.6.8/scratchattach/cloud_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,16 +398,17 @@
         # Prepares the cloud events:
 
         def on_set(event):
             if event.name == "TO_HOST":
                 self.ws_data.append(event)
 
         try:
-            self.connection._connect(cloud_host=self.connection.cloud_host)
-            self.connection._handshake()
+            if self.connection.is_closed:
+                self.connection._connect(cloud_host=self.connection.cloud_host)
+                self.connection._handshake()
         except Exception:
             self.call_event("on_disconnect")
 
         self.idle_since = time.time()
         self.responded_request_ids = []
 
         if self.requests == []:
```

### Comparing `scratchattach-1.6.7/scratchattach/encoder.py` & `scratchattach-1.6.8/scratchattach/encoder.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.7/scratchattach/exceptions.py` & `scratchattach-1.6.8/scratchattach/exceptions.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.7/scratchattach/forum.py` & `scratchattach-1.6.8/scratchattach/forum.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.7/scratchattach/project.py` & `scratchattach-1.6.8/scratchattach/project.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.7/scratchattach/session.py` & `scratchattach-1.6.8/scratchattach/session.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.7/scratchattach/studio.py` & `scratchattach-1.6.8/scratchattach/studio.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.7/scratchattach/user.py` & `scratchattach-1.6.8/scratchattach/user.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.6.7/scratchattach.egg-info/PKG-INFO` & `scratchattach-1.6.8/scratchattach.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.6.7
+Version: 1.6.8
 Summary: An Scratch API Wrapper for scra tch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timkrome2006@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -32,75 +32,79 @@
 # Links
 
 - **[Documentation](https://github.com/TimMcCool/scratchattach/wiki)**
 - [Extended documentation (WIP)](https://scratchattach.readthedocs.io/en/latest/)
 - [Examples](https://github.com/TimMcCool/scratchattach/wiki/Examples)
 - [Change log](https://github.com/TimMcCool/scratchattach/blob/main/CHANGELOG.md)
 
-# Contributors
-
-- Allmost all code by TimMcCool.
-- See the GitHub repository for full list of contributors.
-- Create a pull request to contribute code yourself.
+Report bugs by opening an issue on this repository. If you need help or guideance, leave a comment in the [official forum topic](https://scratch.mit.edu/discuss/topic/603418/
+). Projects made using scratchattach can be added to [this Scratch studio](https://scratch.mit.edu/studios/31478892/).
 
-# Support
+# Example usage
 
-If you need help with your code, leave a comment in the [official forum topic](https://scratch.mit.edu/discuss/topic/603418/
-) on [TimMcCool's Scratch
-profile](https://scratch.mit.edu/users/TimMcCool/) or open an issue on the github repo
+```py
+import scratchattach as scratch3
 
-# Installation
+session = scratch3.login("username", "password")
+conn = session.connect_cloud("project_id")
 
-Run the following command in your command prompt
-/ shell:
-```
-pip install -U scratchattach
+conn.set_var("variable", value)
 ```
 
-**OR**
+**[More examples](https://github.com/TimMcCool/scratchattach/wiki/Examples)**
 
-Add this to your Python code:
-```python
-import os
+# Getting started
 
-os.system("pip install -U scratchattach")
-```
+**Installation:**
 
-# Logging in  `scratch3.Session`
+Run the following command in your command prompt / shell:
+
+```
+pip install -U scratchattach
+```
 
 **Logging in with username / password:**
 
 ```python
 import scratchattach as scratch3
 
 session = scratch3.login("username", "password")
 ```
 
-`login()` returns a `Session` object that saves your login
-
-**Logging in with a sessionId:**
-*You can get your session id from your browser's cookies. [More information](https://github.com/TimMcCool/scratchattach/wiki/Get-your-session-id)*
+`login()` returns a `Session` object that saves your login.
 
+**Logging in with a sessionId:** *You can get your session id from your browser's cookies. [More information](https://github.com/TimMcCool/scratchattach/wiki/Get-your-session-id)*
 ```python
 import scratchattach as scratch3
 
 session = scratch3.Session("sessionId", username="username") #The username field is case sensitive
 ```
 
-**All scratchattach features are documented in the [documentation](https://github.com/TimMcCool/scratchattach/wiki#logging-in).**
-
-# Cloud variables  `scratch3.CloudConnection`
-
 **Connect to the Scratch cloud:**
 
 ```python
 conn = session.connect_cloud("project_id")
 ```
 
 **Get / Set a cloud var:**
 
 ```python
 value = scratch3.get_var("project_id", "variable")
 conn.set_var("variable", "value") #the variable name is specified without the cloud emoji
 ```
 
+**Follow a user / love a project:**
+
+```python
+user_to_follow = session.connect_user("username")
+user_to_follow.follow()
+project_to_love = session.connect_project("project_id")
+project_to_love.love()
+```
+
 **All scratchattach features are documented in the [documentation](https://github.com/TimMcCool/scratchattach/wiki/#cloud-variables).**
+
+# Contributors
+
+- Allmost all code by TimMcCool.
+- See the GitHub repository for full list of contributors.
+- Create a pull request to contribute code yourself.
```

### Comparing `scratchattach-1.6.7/setup.py` & `scratchattach-1.6.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.6.7'
+VERSION = '1.6.8'
 DESCRIPTION = 'An Scratch API Wrapper for scra tch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchattach",
     version=VERSION,
```

