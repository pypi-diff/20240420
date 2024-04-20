# Comparing `tmp/miraie_ac-1.0.0.tar.gz` & `tmp/miraie_ac-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miraie_ac-1.0.0.tar", max compression
+gzip compressed data, was "miraie_ac-1.0.1.tar", max compression
```

## Comparing `miraie_ac-1.0.0.tar` & `miraie_ac-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1068 2024-04-20 11:12:24.000797 miraie_ac-1.0.0/LICENSE
--rw-r--r--   0        0        0      445 2024-04-20 11:12:24.000797 miraie_ac-1.0.0/README.md
--rw-r--r--   0        0        0      283 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/miraie_ac/__init__.py
--rw-r--r--   0        0        0     4714 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/miraie_ac/broker.py
--rw-r--r--   0        0        0      642 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/miraie_ac/constants.py
--rw-r--r--   0        0        0     4604 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/miraie_ac/device.py
--rw-r--r--   0        0        0      717 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/miraie_ac/enums.py
--rw-r--r--   0        0        0      336 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/miraie_ac/home.py
--rw-r--r--   0        0        0     7713 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/miraie_ac/hub.py
--rw-r--r--   0        0        0      352 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/miraie_ac/topic.py
--rw-r--r--   0        0        0      388 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/miraie_ac/user.py
--rw-r--r--   0        0        0      393 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/miraie_ac/utils.py
--rw-r--r--   0        0        0      413 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 miraie_ac-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/LICENSE
+-rw-r--r--   0        0        0      351 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/README.md
+-rw-r--r--   0        0        0      283 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/miraie_ac/__init__.py
+-rw-r--r--   0        0        0     5074 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/miraie_ac/broker.py
+-rw-r--r--   0        0        0      642 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/miraie_ac/constants.py
+-rw-r--r--   0        0        0     4739 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/miraie_ac/device.py
+-rw-r--r--   0        0        0      717 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/miraie_ac/enums.py
+-rw-r--r--   0        0        0      336 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/miraie_ac/home.py
+-rw-r--r--   0        0        0     7713 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/miraie_ac/hub.py
+-rw-r--r--   0        0        0      352 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/miraie_ac/topic.py
+-rw-r--r--   0        0        0      388 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/miraie_ac/user.py
+-rw-r--r--   0        0        0      393 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/miraie_ac/utils.py
+-rw-r--r--   0        0        0      413 2024-04-20 11:30:09.663689 miraie_ac-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      918 1970-01-01 00:00:00.000000 miraie_ac-1.0.1/PKG-INFO
```

### Comparing `miraie_ac-1.0.0/LICENSE` & `miraie_ac-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `miraie_ac-1.0.0/miraie_ac/broker.py` & `miraie_ac-1.0.1/miraie_ac/broker.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,7 +139,16 @@
         payload["acvs"] = mode.value
         return payload
 
     async def set_swing_mode(self, topic: str, mode: SwingMode):
         await self.client.publish(
             topic, json.dumps(self.build_swing_mode_payload(mode))
         )
+        
+    # Display Mode
+    def build_display_mode_payload(self, mode: DisplayMode):
+        payload = self.build_base_payload()
+        payload["acdc"] = str(mode.value)
+        return payload
+
+    async def set_display_mode(self, topic: str, mode: DisplayMode):
+        await self.client.publish(topic, json.dumps(self.build_display_mode_payload(mode)))
```

### Comparing `miraie_ac-1.0.0/miraie_ac/constants.py` & `miraie_ac-1.0.1/miraie_ac/constants.py`

 * *Files identical despite different names*

### Comparing `miraie_ac-1.0.0/miraie_ac/device.py` & `miraie_ac-1.0.1/miraie_ac/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,7 +137,10 @@
         await self.broker.set_fan_mode(self.control_topic, mode)
 
     async def set_preset_mode(self, mode: PresetMode):
         await self.broker.set_preset_mode(self.control_topic, mode)
 
     async def set_swing_mode(self, mode: SwingMode):
         await self.broker.set_swing_mode(self.control_topic, mode)
+        
+    async def set_display_mode(self, mode: DisplayMode):
+        await self.broker.set_display_mode(self.control_topic, mode)
```

### Comparing `miraie_ac-1.0.0/miraie_ac/enums.py` & `miraie_ac-1.0.1/miraie_ac/enums.py`

 * *Files identical despite different names*

### Comparing `miraie_ac-1.0.0/miraie_ac/hub.py` & `miraie_ac-1.0.1/miraie_ac/hub.py`

 * *Files identical despite different names*

### Comparing `miraie_ac-1.0.0/PKG-INFO` & `miraie_ac-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miraie-ac
-Version: 1.0.0
+Version: 1.0.1
 Summary: MirAIe-AC API for Python
 License: MIT
 Author: Raj Kishore
 Author-email: 40551183+rkzofficial@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,18 +13,14 @@
 Requires-Dist: aiomqtt (>=2.0.1,<3.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: certifi (>=2024.2.2,<2025.0.0)
 Description-Content-Type: text/markdown
 
 # MirAIe API for Python
 
-# Medium multiply
-
-A small demo library for a Medium publication about publishing libraries.
-
 ### Installation
 
 ```
 pip install miraie-ac
 ```
 
 ### Get started
```

