# Comparing `tmp/emerald_hws-0.0.7.tar.gz` & `tmp/emerald_hws-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emerald_hws-0.0.7.tar", last modified: Wed Apr 17 11:01:16 2024, max compression
+gzip compressed data, was "emerald_hws-0.0.8.tar", last modified: Sat Apr 20 10:19:22 2024, max compression
```

## Comparing `emerald_hws-0.0.7.tar` & `emerald_hws-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-17 11:01:16.951022 emerald_hws-0.0.7/
--rw-r--r--   0 ross       (501) staff       (20)     1072 2024-01-24 10:16:13.000000 emerald_hws-0.0.7/LICENSE
--rw-r--r--   0 ross       (501) staff       (20)      688 2024-04-17 11:01:16.950647 emerald_hws-0.0.7/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)       84 2024-01-24 10:15:13.000000 emerald_hws-0.0.7/README.md
--rw-r--r--   0 ross       (501) staff       (20)      818 2024-04-17 10:59:24.000000 emerald_hws-0.0.7/pyproject.toml
--rw-r--r--   0 ross       (501) staff       (20)       38 2024-04-17 11:01:16.951151 emerald_hws-0.0.7/setup.cfg
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-17 11:01:16.944107 emerald_hws-0.0.7/src/
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-17 11:01:16.947821 emerald_hws-0.0.7/src/emerald_hws/
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-17 11:01:16.949567 emerald_hws-0.0.7/src/emerald_hws/__assets__/
--rw-r--r--   0 ross       (501) staff       (20)     1424 2024-01-23 10:06:20.000000 emerald_hws-0.0.7/src/emerald_hws/__assets__/SFSRootCAG2.pem
--rw-r--r--   0 ross       (501) staff       (20)        1 2024-01-24 10:24:29.000000 emerald_hws-0.0.7/src/emerald_hws/__init__.py
--rw-r--r--   0 ross       (501) staff       (20)    13251 2024-04-17 10:56:27.000000 emerald_hws-0.0.7/src/emerald_hws/emeraldhws.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-17 11:01:16.950243 emerald_hws-0.0.7/src/emerald_hws.egg-info/
--rw-r--r--   0 ross       (501) staff       (20)      688 2024-04-17 11:01:16.000000 emerald_hws-0.0.7/src/emerald_hws.egg-info/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)      327 2024-04-17 11:01:16.000000 emerald_hws-0.0.7/src/emerald_hws.egg-info/SOURCES.txt
--rw-r--r--   0 ross       (501) staff       (20)        1 2024-04-17 11:01:16.000000 emerald_hws-0.0.7/src/emerald_hws.egg-info/dependency_links.txt
--rw-r--r--   0 ross       (501) staff       (20)       16 2024-04-17 11:01:16.000000 emerald_hws-0.0.7/src/emerald_hws.egg-info/requires.txt
--rw-r--r--   0 ross       (501) staff       (20)       12 2024-04-17 11:01:16.000000 emerald_hws-0.0.7/src/emerald_hws.egg-info/top_level.txt
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-20 10:19:22.739761 emerald_hws-0.0.8/
+-rw-r--r--   0 ross       (501) staff       (20)     1072 2024-01-24 10:16:13.000000 emerald_hws-0.0.8/LICENSE
+-rw-r--r--   0 ross       (501) staff       (20)      688 2024-04-20 10:19:22.739189 emerald_hws-0.0.8/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)       84 2024-01-24 10:15:13.000000 emerald_hws-0.0.8/README.md
+-rw-r--r--   0 ross       (501) staff       (20)      811 2024-04-20 10:18:44.000000 emerald_hws-0.0.8/pyproject.toml
+-rw-r--r--   0 ross       (501) staff       (20)       38 2024-04-20 10:19:22.739860 emerald_hws-0.0.8/setup.cfg
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-20 10:19:22.732246 emerald_hws-0.0.8/src/
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-20 10:19:22.735812 emerald_hws-0.0.8/src/emerald_hws/
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-20 10:19:22.737771 emerald_hws-0.0.8/src/emerald_hws/__assets__/
+-rw-r--r--   0 ross       (501) staff       (20)     1424 2024-01-23 10:06:20.000000 emerald_hws-0.0.8/src/emerald_hws/__assets__/SFSRootCAG2.pem
+-rw-r--r--   0 ross       (501) staff       (20)        1 2024-01-24 10:24:29.000000 emerald_hws-0.0.8/src/emerald_hws/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)    13892 2024-04-20 10:16:23.000000 emerald_hws-0.0.8/src/emerald_hws/emeraldhws.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-20 10:19:22.738524 emerald_hws-0.0.8/src/emerald_hws.egg-info/
+-rw-r--r--   0 ross       (501) staff       (20)      688 2024-04-20 10:19:22.000000 emerald_hws-0.0.8/src/emerald_hws.egg-info/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)      327 2024-04-20 10:19:22.000000 emerald_hws-0.0.8/src/emerald_hws.egg-info/SOURCES.txt
+-rw-r--r--   0 ross       (501) staff       (20)        1 2024-04-20 10:19:22.000000 emerald_hws-0.0.8/src/emerald_hws.egg-info/dependency_links.txt
+-rw-r--r--   0 ross       (501) staff       (20)       16 2024-04-20 10:19:22.000000 emerald_hws-0.0.8/src/emerald_hws.egg-info/requires.txt
+-rw-r--r--   0 ross       (501) staff       (20)       12 2024-04-20 10:19:22.000000 emerald_hws-0.0.8/src/emerald_hws.egg-info/top_level.txt
```

### Comparing `emerald_hws-0.0.7/LICENSE` & `emerald_hws-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `emerald_hws-0.0.7/PKG-INFO` & `emerald_hws-0.0.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emerald_hws
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package to manipulate and monitor Emerald Heat Pump Hot Water Systems
 Author-email: Ross Williamson <ross@inertia.net.nz>
 Project-URL: Homepage, https://github.com/ross-w/emerald_hws_py
 Project-URL: Bug Tracker, https://github.com/ross-w/emerald_hws_py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `emerald_hws-0.0.7/pyproject.toml` & `emerald_hws-0.0.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "emerald_hws"
-version = "0.0.7"
-dependencies = [
-  "boto3",
-  "awsiotsdk"
-]
-authors = [
-  { name="Ross Williamson", email="ross@inertia.net.nz" },
-]
+version = "0.0.8"
+dependencies = ["boto3", "awsiotsdk"]
+authors = [{ name = "Ross Williamson", email = "ross@inertia.net.nz" }]
 description = "A package to manipulate and monitor Emerald Heat Pump Hot Water Systems"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `emerald_hws-0.0.7/src/emerald_hws/__assets__/SFSRootCAG2.pem` & `emerald_hws-0.0.8/src/emerald_hws/__assets__/SFSRootCAG2.pem`

 * *Files identical despite different names*

### Comparing `emerald_hws-0.0.7/src/emerald_hws/emeraldhws.py` & `emerald_hws-0.0.8/src/emerald_hws/emeraldhws.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import requests
 import os
 import logging
 import boto3
 import random
+import threading
 from awsiot import mqtt5_client_builder, mqtt_connection_builder
 from awscrt import mqtt5, http, auth, io
 
 
 class EmeraldHWS():
     """ Implementation of the web API for Emerald Heat Pump Hot Water Systems
     """
@@ -17,25 +18,27 @@
         "user-agent":       "EmeraldPlanet/2.5.3 (com.emerald-ems.customer; build:5; iOS 17.2.1) Alamofire/5.4.1",
         "accept-language":  "en-GB;q=1.0, en-AU;q=0.9",
     }
 
     MQTT_HOST = "a13v32g67itvz9-ats.iot.ap-southeast-2.amazonaws.com"
     COGNITO_IDENTITY_POOL_ID = "ap-southeast-2:f5bbb02c-c00e-4f10-acb3-e7d1b05268e8"
 
-    def __init__(self, email, password):
+    def __init__(self, email, password, update_callback=None):
         """ Initialise the API client
         :param email: The email address for logging into the Emerald app
         :param password: The password for the supplied user account
+        :param update_callback: Optional callback function to be called when an update is available
         """
 
         self.email = email
         self.password = password
         self.token = ""
         self.properties = {}
         self.logger = logging.getLogger()
+        self.update_callback = update_callback
 
     def getLoginToken(self):
         """ Performs an API request to get a token from the API
         """
         url = "https://api.emerald-ems.com.au/api/v1/customer/sign-in"
 
         payload = {
@@ -74,14 +77,23 @@
 
         if post_response_json.get("code") == 200:
             self.logger.debug("emeraldhws: Successfully logged into Emerald API")
             self.properties = post_response_json.get("info").get("property")
         else:
             raise Exception("Unable to fetch properties from Emerald API")
 
+    def reconnectMQTT(self):
+        """ Stops an existing MQTT connection and creates a new one
+        """
+
+        self.logger.debug("emeraldhws: awsiot: Tearing down and reconnecting to prevent stale connection")
+        self.mqttClient.stop()
+        self.connectMQTT()
+        self.subscribeAllHWS()
+
     def connectMQTT(self):
         """ Establishes a connection to Amazon IOT core's MQTT service
         """
 
         cert_path = os.path.join(os.path.dirname(__file__), '__assets__', 'SFSRootCAG2.pem')
         identityPoolID = self.COGNITO_IDENTITY_POOL_ID
         region = self.MQTT_HOST.split('.')[2]
@@ -109,14 +121,15 @@
             on_lifecycle_disconnection = self.on_lifecycle_disconnection,
             on_lifecycle_connection_failure = self.on_lifecycle_connection_failure,
             on_publish_received = self.mqttCallback
         )
 
         client.start()
         self.mqttClient = client
+        threading.Timer(43200.0, self.reconnectMQTT).start() # 12 hours
 
     def mqttDecodeUpdate(self, topic, payload):
         """ Attempt to decode a received MQTT message and direct appropriately
         :param topic: MQTT topic
         :param payload: MQTT payload
         """
         json_payload = json.loads(payload.decode("utf-8"))
@@ -184,14 +197,16 @@
         """
 
         for properties in self.properties:
             heat_pumps = properties.get('heat_pump', [])
             for heat_pump in heat_pumps:
                 if heat_pump['id'] == id:
                     heat_pump['last_state'][key] = value
+        if self.update_callback != None:
+            self.update_callback()
 
     def subscribeForUpdates(self, id):
         """ Subscribes to the MQTT topics for the supplied HWS
         :param id: The UUID of the requested HWS
         """
         if not self.mqttClient:
             self.connectMQTT()
```

### Comparing `emerald_hws-0.0.7/src/emerald_hws.egg-info/PKG-INFO` & `emerald_hws-0.0.8/src/emerald_hws.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emerald_hws
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package to manipulate and monitor Emerald Heat Pump Hot Water Systems
 Author-email: Ross Williamson <ross@inertia.net.nz>
 Project-URL: Homepage, https://github.com/ross-w/emerald_hws_py
 Project-URL: Bug Tracker, https://github.com/ross-w/emerald_hws_py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

