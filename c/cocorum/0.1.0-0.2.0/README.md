# Comparing `tmp/cocorum-0.1.0.tar.gz` & `tmp/cocorum-0.2.0.tar.gz`

## Comparing `cocorum-0.1.0.tar` & `cocorum-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 cocorum-0.1.0/requirements.txt
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cocorum-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    16166 2020-02-02 00:00:00.000000 cocorum-0.1.0/src/cocorum/__init__.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 cocorum-0.1.0/src/cocorum/localvars.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cocorum-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 cocorum-0.1.0/README.md
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 cocorum-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 cocorum-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cocorum-0.2.0/requirements.txt
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cocorum-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    17442 2020-02-02 00:00:00.000000 cocorum-0.2.0/src/cocorum/__init__.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 cocorum-0.2.0/src/cocorum/localvars.py
+-rw-r--r--   0        0        0    12924 2020-02-02 00:00:00.000000 cocorum-0.2.0/src/cocorum/ssechat.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 cocorum-0.2.0/src/cocorum/utils.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cocorum-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 cocorum-0.2.0/README.md
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 cocorum-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 cocorum-0.2.0/PKG-INFO
```

### Comparing `cocorum-0.1.0/.github/workflows/python-publish.yml` & `cocorum-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cocorum-0.1.0/src/cocorum/__init__.py` & `cocorum-0.2.0/src/cocorum/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,15 @@
 #S.D.G.
 
 import requests
 import time
 import calendar
 
 from .localvars import *
-
-def parse_timestamp(timestamp):
-    """Parse a Rumble timestamp to seconds since Epoch"""
-    return calendar.timegm(time.strptime(timestamp[:-6], TIMESTAMP_FORMAT)) #Trims off the 6 TODO characters at the end
+from .utils import *
 
 class RumbleAPISubObj(object):
     """Abstract class for a Rumble API object"""
     def __init__(self, json):
         """Pass the JSON block for a single Rumble API subobject"""
         self._json = json
     def __getitem__(self, key):
@@ -28,15 +25,15 @@
         self._json = json
         self.__profile_pic = None
 
     def __eq__(self, other):
         """Is this follower equal to another"""
         if type(other) == str: #Check if the compared string is our username
             return self.username == other
-        if type(other) == type(self): #Check if the compared follower has our username
+        if hasattr(other, "username"): #Check if the compared object has a username and if it matches our own
             return self.username == other.username
 
     def __str__(self):
         """Follower as a string"""
         return self.username
 
     @property
@@ -76,18 +73,20 @@
         """Is this subscriber equal to another"""
         if type(other) == str: #Check if the compared string is our username
             return self.username == other
         if type(other) in (int, float): #check if the compared number is our amount in cents
             return self.amount_cents == other
         if type(other) == type(self): #Check if the compared subscriber has the same username and amount
             return (self.username, self.amount_cents) == (other.username, other.amount_cents)
+        if hasattr(other, "username"): #Check if the compared object has a username and if it matches our own
+            return self.username == other.username
 
     @property
     def user(self):
-        """TODO"""
+        """AFAIK this is being deprecated, use username instead"""
         return self["user"]
 
     @property
     def amount_cents(self):
         """The total subscription amount in cents"""
         return self["amount_cents"]
 
@@ -133,16 +132,18 @@
 
     def __eq__(self, other):
         """Is this stream equal to another"""
         if type(other) == str: #Check if the compared string is our stream ID
             return self.stream_id == other
         if type(other) in (int, float): #check if the compared number is our chat ID (linked to stream ID)
             return self.chat_id == other
-        if type(other) == type(self): #Check if the compared stream has the same stream ID
+        if hasattr(other, "stream_id"): #Check if the compared object has the same stream ID
             return self.stream_id == other.stream_id
+        if hasattr(other, "chat_id"): #Check if the compared object has the same chat ID
+            return self.stream_id == other.chat_id
 
     def __str__(self):
         """The livestream in string form"""
         return self.stream_id
 
     def __getitem__(self, key):
         """Return a key from the JSON, refreshing if necessary"""
@@ -154,15 +155,15 @@
     def stream_id(self):
         """The livestream ID"""
         return self["id"]
 
     @property
     def chat_id(self):
         """The livestream chat ID"""
-        return int(self.stream_id, 36)
+        return id_stream_to_chat(self.stream_id)
 
     @property
     def title(self):
         """The title of the livestream"""
         return self["title"]
 
     @property
@@ -218,14 +219,18 @@
     """A single message in a Rumble livestream chat"""
     def __eq__(self, other):
         """Is this message equal to another"""
         if type(other) == str: #Check if the compared string is our message
             return self.text == other
         if type(other) == type(self): #Check if the compared message has the same username and text
             return (self.username, self.text) == (other.username, other.text)
+        if hasattr(other, "text"): #Check if the compared object has the same text
+            if hasattr(other, "username"): #Check if the compared object has the same username
+                return (self.username, self.text) == (other.username, other.text)
+            return self.text == other.text #the other object had no username attribute
 
     def __str__(self):
         """Follower as a string"""
         return self.text
 
     @property
     def text(self):
@@ -246,14 +251,20 @@
     """A single rant in a Rumble livestream chat"""
     def __eq__(self, other):
         """Is this category equal to another"""
         if type(other) == str: #Check if the compared string is our message
             return self.text == other
         if type(other) == type(self): #Check if the compared rant has the same username, amount, and text
             return (self.username, self.amount_cents, self.text) == (other.username, other.amount_cents, other.text)
+        if hasattr(other, "text"): #Check if the compared object has the same text
+            if hasattr(other, "username"): #Check if the compared object has the same username
+                if hasattr(other, "amount_cents"): #Check if the compared object has the same amount
+                    return (self.username, self.amount_cents, self.text) == (other.username, other.amount_cents, other.text)
+                return (self.username, self.text) == (other.username, other.text) #Other object has no amount_cents attribute
+            return self.text == other.text #Other object had no username attribute
 
     @property
     def expires_on(self):
         """When the rant will expire, in seconds since the Epoch UTC"""
         return self["expires_on"]
 
     @property
@@ -413,55 +424,55 @@
     def channel_name(self):
         """The channel name, if we are a channel"""
         return self["channel_name"]
 
     @property
     def num_followers(self):
         """The number of followers of this user or channel"""
-        return self["num_followers"]
+        return self["followers"]["num_followers"]
 
     @property
     def num_followers_total(self):
         """The total number of followers of this account across all channels"""
-        return self["num_followers_total"]
+        return self["followers"]["num_followers_total"]
 
     @property
     def latest_follower(self):
         """The latest follower of this user or channel"""
-        if not self["latest_follower"]:
+        if not self["followers"]["latest_follower"]:
             return None #No-one has followed this user or channel yet
-        return RumbleFollower(self["latest_follower"])
+        return RumbleFollower(self["followers"]["latest_follower"])
 
     @property
     def recent_followers(self):
         """A list (technically a shallow generator object) of recent followers"""
-        data = self["recent_followers"].copy().values()
+        data = self["followers"]["recent_followers"].copy()
         return [RumbleFollower(json_block) for json_block in data]
 
     @property
     def num_subscribers(self):
         """The number of subscribers of this user or channel"""
-        return self["num_subscribers"]
+        return self["subscribers"]["num_subscribers"]
 
     @property
     def num_subscribers_total(self):
         """The total number of subscribers of this account across all channels"""
-        return self["num_subscribers_total"]
+        return self["subscribers"]["num_subscribers_total"]
 
     @property
     def latest_subscriber(self):
         """The latest subscriber of this user or channel"""
-        if not self["latest_subscriber"]:
+        if not self["subscribers"]["latest_subscriber"]:
             return None #No-one has subscribed to this user or channel yet
-        return RumbleSubscriber(self["latest_subscriber"])
+        return RumbleSubscriber(self["subscribers"]["latest_subscriber"])
 
     @property
     def recent_subscribers(self):
         """A list (technically a shallow generator object) of recent subscribers"""
-        data = self["recent_subscribers"].copy().values()
+        data = self["subscribers"]["recent_subscribers"].copy()
         return [RumbleSubscriber(json_block) for json_block in data]
 
     @property
     def livestreams(self):
         """A dictionairy of our livestreams"""
         self.check_refresh()
         return self.__livestreams
```

### Comparing `cocorum-0.1.0/LICENSE.txt` & `cocorum-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cocorum-0.1.0/pyproject.toml` & `cocorum-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cocorum"
-version = "0.1.0"
+version = "0.2.0"
 keywords = ["rumble", "api", "wrapper", "livestream"]
 authors = [
   { name="Wilbur Jaywright", email="zargulthewizard@outlook.com" },
 ]
 description = "An unofficial Python wrapper for the Rumble Live Stream API v1.0 (beta)"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
   "requests",
+  "sseclient", #Only for the Rumble chat SSE stream
   ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
     "Development Status :: 3 - Alpha",
 ]
 
 [project.urls]
 Homepage = "https://github.com/thelabcat/rumble-api-wrapper-py"
 Issues = "https://github.com/thelabcat/rumble-api-wrapper-py/issues"
-"Rumble API docs" = "https://rumblefaq.groovehq.com/help/how-to-use-rumble-s-live-stream-api"
+"Rumble Live Stream API docs" = "https://rumblefaq.groovehq.com/help/how-to-use-rumble-s-live-stream-api"
```

### Comparing `cocorum-0.1.0/PKG-INFO` & `cocorum-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.3
 Name: cocorum
-Version: 0.1.0
+Version: 0.2.0
 Summary: An unofficial Python wrapper for the Rumble Live Stream API v1.0 (beta)
 Project-URL: Homepage, https://github.com/thelabcat/rumble-api-wrapper-py
 Project-URL: Issues, https://github.com/thelabcat/rumble-api-wrapper-py/issues
-Project-URL: Rumble API docs, https://rumblefaq.groovehq.com/help/how-to-use-rumble-s-live-stream-api
+Project-URL: Rumble Live Stream API docs, https://rumblefaq.groovehq.com/help/how-to-use-rumble-s-live-stream-api
 Author-email: Wilbur Jaywright <zargulthewizard@outlook.com>
 License-File: LICENSE.txt
 Keywords: api,livestream,rumble,wrapper
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: requests
+Requires-Dist: sseclient
 Description-Content-Type: text/markdown
 
 # Cocorum: Rumble Live Stream API Python Wrapper
 A Python wrapper for the Rumble Live Stream API v1.0 (beta), with some quality of live additions, such as:
 - Automatic refresh when past the refresh_rate delay when querying any non_static property.
 - All timespamps are parsed to seconds since Epoch, UTC timezone.
 - Chat has new_messages and new_rants properties that return only messages and rants since the last time they were read.
@@ -46,12 +47,30 @@
     if livestream.visibility != STREAM_VIS_PUBLIC:
         print("Stream is not public.")
     message = livestream.chat.latest_message #None if there are no messages yet
     if message:
         print(message.username, "said", message)
 ```
 
+## Experimental SSE chat submodule
+This part of cocorum is not part of the official Rumble Livestream API, but may provide a more reliable method of ensuring all chat messages are received.
+
+```
+from cocorum import ssechat
+
+chat = ssechat.SSEChat(chat_id = CHAT_ID)
+#Do chat.mailbox = [] here to erase messages that were still visible before we connected
+
+msg = True
+while msg:
+    msg = chat.next_chat_message() #Hangs until a new message arrives
+    print(msg.user.username, ":", msg)
+
+print("Chat has closed.")
+```
+
+## Conclusion
 Hope this helps!
 
 I, Wilbur Jaywright, and my brand, Marswide BGL, have no official association with Rumble Corp. beyond that of a normal user and/or channel on the Rumble Video platform. This wrapper is not officially endorsed by Rumble Corp. or its subsidiaries.
 
 S.D.G.
```

