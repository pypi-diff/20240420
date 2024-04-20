# Comparing `tmp/miraie_ac-1.0.1.tar.gz` & `tmp/miraie_ac-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miraie_ac-1.0.1.tar", max compression
+gzip compressed data, was "miraie_ac-1.0.2.tar", max compression
```

## Comparing `miraie_ac-1.0.1.tar` & `miraie_ac-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1068 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/LICENSE
--rw-r--r--   0        0        0      351 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/README.md
--rw-r--r--   0        0        0      283 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/miraie_ac/__init__.py
--rw-r--r--   0        0        0     5074 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/miraie_ac/broker.py
--rw-r--r--   0        0        0      642 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/miraie_ac/constants.py
--rw-r--r--   0        0        0     4739 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/miraie_ac/device.py
--rw-r--r--   0        0        0      717 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/miraie_ac/enums.py
--rw-r--r--   0        0        0      336 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/miraie_ac/home.py
--rw-r--r--   0        0        0     7713 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/miraie_ac/hub.py
--rw-r--r--   0        0        0      352 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/miraie_ac/topic.py
--rw-r--r--   0        0        0      388 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/miraie_ac/user.py
--rw-r--r--   0        0        0      393 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/miraie_ac/utils.py
--rw-r--r--   0        0        0      413 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      918 1970-01-01 00:00:00.000000 miraie_ac-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-20 14:40:57.330434 miraie_ac-1.0.2/LICENSE
+-rw-r--r--   0        0        0      351 2024-04-20 14:40:57.330434 miraie_ac-1.0.2/README.md
+-rw-r--r--   0        0        0      283 2024-04-20 14:40:57.330434 miraie_ac-1.0.2/miraie_ac/__init__.py
+-rw-r--r--   0        0        0     5101 2024-04-20 14:40:57.330434 miraie_ac-1.0.2/miraie_ac/broker.py
+-rw-r--r--   0        0        0      642 2024-04-20 14:40:57.330434 miraie_ac-1.0.2/miraie_ac/constants.py
+-rw-r--r--   0        0        0     4739 2024-04-20 14:40:57.330434 miraie_ac-1.0.2/miraie_ac/device.py
+-rw-r--r--   0        0        0      717 2024-04-20 14:40:57.330434 miraie_ac-1.0.2/miraie_ac/enums.py
+-rw-r--r--   0        0        0      336 2024-04-20 14:40:57.330434 miraie_ac-1.0.2/miraie_ac/home.py
+-rw-r--r--   0        0        0     7713 2024-04-20 14:40:57.330434 miraie_ac-1.0.2/miraie_ac/hub.py
+-rw-r--r--   0        0        0      352 2024-04-20 14:40:57.330434 miraie_ac-1.0.2/miraie_ac/topic.py
+-rw-r--r--   0        0        0      388 2024-04-20 14:40:57.330434 miraie_ac-1.0.2/miraie_ac/user.py
+-rw-r--r--   0        0        0      393 2024-04-20 14:40:57.330434 miraie_ac-1.0.2/miraie_ac/utils.py
+-rw-r--r--   0        0        0      413 2024-04-20 14:40:57.330434 miraie_ac-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      918 1970-01-01 00:00:00.000000 miraie_ac-1.0.2/PKG-INFO
```

### Comparing `miraie_ac-1.0.1/LICENSE` & `miraie_ac-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `miraie_ac-1.0.1/miraie_ac/broker.py` & `miraie_ac-1.0.2/miraie_ac/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from aiomqtt import Client, Message, MqttError
 import asyncio
 import ssl
 import certifi
 import random
 import json
-from .enums import PowerMode, HVACMode, FanMode, PresetMode, SwingMode
+from .enums import PowerMode, HVACMode, FanMode, PresetMode, SwingMode, DisplayMode
 from .user import User
 
 
 class MirAIeBroker:
     host = "mqtt.miraie.in"
     port = 8883
     use_ssl = True
@@ -139,16 +139,18 @@
         payload["acvs"] = mode.value
         return payload
 
     async def set_swing_mode(self, topic: str, mode: SwingMode):
         await self.client.publish(
             topic, json.dumps(self.build_swing_mode_payload(mode))
         )
-        
+
     # Display Mode
     def build_display_mode_payload(self, mode: DisplayMode):
         payload = self.build_base_payload()
         payload["acdc"] = str(mode.value)
         return payload
 
     async def set_display_mode(self, topic: str, mode: DisplayMode):
-        await self.client.publish(topic, json.dumps(self.build_display_mode_payload(mode)))
+        await self.client.publish(
+            topic, json.dumps(self.build_display_mode_payload(mode))
+        )
```

### Comparing `miraie_ac-1.0.1/miraie_ac/constants.py` & `miraie_ac-1.0.2/miraie_ac/constants.py`

 * *Files identical despite different names*

### Comparing `miraie_ac-1.0.1/miraie_ac/device.py` & `miraie_ac-1.0.2/miraie_ac/device.py`

 * *Files identical despite different names*

### Comparing `miraie_ac-1.0.1/miraie_ac/enums.py` & `miraie_ac-1.0.2/miraie_ac/enums.py`

 * *Files identical despite different names*

### Comparing `miraie_ac-1.0.1/miraie_ac/hub.py` & `miraie_ac-1.0.2/miraie_ac/hub.py`

 * *Files identical despite different names*

### Comparing `miraie_ac-1.0.1/PKG-INFO` & `miraie_ac-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miraie-ac
-Version: 1.0.1
+Version: 1.0.2
 Summary: MirAIe-AC API for Python
 License: MIT
 Author: Raj Kishore
 Author-email: 40551183+rkzofficial@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

