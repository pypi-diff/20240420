# Comparing `tmp/miraie-ac-0.2.9.tar.gz` & `tmp/miraie_ac-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miraie-ac-0.2.9.tar", last modified: Mon Nov 14 14:53:57 2022, max compression
+gzip compressed data, was "miraie_ac-1.0.0.tar", max compression
```

## Comparing `miraie-ac-0.2.9.tar` & `miraie_ac-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-11-14 14:53:57.654069 miraie-ac-0.2.9/
--rw-rw-rw-   0        0        0     1089 2022-11-14 08:12:24.000000 miraie-ac-0.2.9/LICENSE
--rw-rw-rw-   0        0        0      738 2022-11-14 14:53:57.654069 miraie-ac-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0      471 2022-11-14 11:24:06.000000 miraie-ac-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2022-11-14 14:53:57.636007 miraie-ac-0.2.9/miraie_ac/
--rw-rw-rw-   0        0        0      295 2022-11-14 13:55:24.000000 miraie-ac-0.2.9/miraie_ac/__init__.py
--rw-rw-rw-   0        0        0     4629 2022-11-14 14:33:23.000000 miraie-ac-0.2.9/miraie_ac/broker.py
--rw-rw-rw-   0        0        0      649 2022-11-14 08:12:24.000000 miraie-ac-0.2.9/miraie_ac/constants.py
--rw-rw-rw-   0        0        0     4568 2022-11-14 14:50:13.000000 miraie-ac-0.2.9/miraie_ac/device.py
--rw-rw-rw-   0        0        0      770 2022-11-14 14:02:53.000000 miraie-ac-0.2.9/miraie_ac/enums.py
--rw-rw-rw-   0        0        0      351 2022-11-14 08:12:24.000000 miraie-ac-0.2.9/miraie_ac/home.py
--rw-rw-rw-   0        0        0     6903 2022-11-14 14:53:33.000000 miraie-ac-0.2.9/miraie_ac/hub.py
--rw-rw-rw-   0        0        0      363 2022-11-14 08:12:24.000000 miraie-ac-0.2.9/miraie_ac/topic.py
--rw-rw-rw-   0        0        0      368 2022-11-14 08:12:24.000000 miraie-ac-0.2.9/miraie_ac/user.py
-drwxrwxrwx   0        0        0        0 2022-11-14 14:53:57.653057 miraie-ac-0.2.9/miraie_ac.egg-info/
--rw-rw-rw-   0        0        0      738 2022-11-14 14:53:57.000000 miraie-ac-0.2.9/miraie_ac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2022-11-14 14:53:57.000000 miraie-ac-0.2.9/miraie_ac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-14 14:53:57.000000 miraie-ac-0.2.9/miraie_ac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-11-14 14:53:57.000000 miraie-ac-0.2.9/miraie_ac.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-14 14:53:57.655068 miraie-ac-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0      972 2022-11-14 14:53:52.000000 miraie-ac-0.2.9/setup.py
+-rw-r--r--   0        0        0     1068 2024-04-20 11:12:24.000797 miraie_ac-1.0.0/LICENSE
+-rw-r--r--   0        0        0      445 2024-04-20 11:12:24.000797 miraie_ac-1.0.0/README.md
+-rw-r--r--   0        0        0      283 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/miraie_ac/__init__.py
+-rw-r--r--   0        0        0     4714 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/miraie_ac/broker.py
+-rw-r--r--   0        0        0      642 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/miraie_ac/constants.py
+-rw-r--r--   0        0        0     4604 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/miraie_ac/device.py
+-rw-r--r--   0        0        0      717 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/miraie_ac/enums.py
+-rw-r--r--   0        0        0      336 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/miraie_ac/home.py
+-rw-r--r--   0        0        0     7713 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/miraie_ac/hub.py
+-rw-r--r--   0        0        0      352 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/miraie_ac/topic.py
+-rw-r--r--   0        0        0      388 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/miraie_ac/user.py
+-rw-r--r--   0        0        0      393 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/miraie_ac/utils.py
+-rw-r--r--   0        0        0      413 2024-04-20 11:12:24.004797 miraie_ac-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 miraie_ac-1.0.0/PKG-INFO
```

### Comparing `miraie-ac-0.2.9/miraie_ac/broker.py` & `miraie_ac-1.0.0/miraie_ac/broker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,145 +1,145 @@
-from paho.mqtt import client as mqtt
-import ssl
-import certifi
-import random
-import json
-from .enums import *
-
-
-class MirAIeBroker:
-    host = "mqtt.miraie.in"
-    port = 8883
-    use_ssl = True
-    client_id = f"ha-mirae-mqtt-{random.randint(0, 1000)}"
-
-    def __init__(self) -> None:
-        self.status_callbacks: dict[str, list[callable]] = {}
-
-    def register_device_callback(self, topic: str, callback):
-        self.status_callbacks[topic] = callback
-
-    def remove_device_callback(self, topic: str):
-        self.status_callbacks.pop(topic, None)
-
-    def set_topics(self, topics: list[str]):
-        self.commandTopics = topics
-
-    def on_connect(self, client: mqtt.Client, userdata, flags, rc):
-        # Subscribe to all command topics
-        for topic in self.commandTopics:
-            client.subscribe(topic)
-
-    def on_message(self, client: mqtt.Client, userdata, msg):
-        parsed = json.loads(msg.payload.decode("utf-8"))
-
-        func = self.status_callbacks.get(msg.topic)
-        func(parsed)
-
-    def on_disconnect(self, client: mqtt.Client, userdata, rc):
-        if rc != 0:
-            client.reconnect()
-
-    def on_log(self, client, userdata, level, buf):
-        print("log: ", buf)
-
-    def connect(self, username: str, password: str):
-        # Create MQTT client
-        client = mqtt.Client(
-            self.client_id,
-            True,
-        )
-
-        # Set username and password
-        client.username_pw_set(username, password)
-
-        if self.use_ssl:
-            # Create ssl context with TLSv1
-            context = ssl.create_default_context(cafile=certifi.where())
-            client.tls_set_context(context)
-            client.tls_insecure_set(True)
-
-        # Set callbacks
-        client.on_connect = self.on_connect
-        client.on_message = self.on_message
-        client.on_disconnect = self.on_disconnect
-        # client.on_log = self.on_log
-
-        # Connect to MQTT broker
-        client.connect(self.host, self.port, 60)
-
-        # Start network loop
-        self.client = client
-        self.client.loop_start()
-
-    def build_base_payload(self):
-        return {
-            "ki": 1,
-            "cnt": "an",
-            "sid": "1",
-        }
-
-    # Power
-    def build_power_payload(self, power: PowerMode):
-        payload = self.build_base_payload()
-        payload["ps"] = str(power)
-        return payload
-
-    def set_power(self, topic: str, power: PowerMode):
-        self.client.publish(topic, json.dumps(self.build_power_payload(power)))
-
-    # Temperature
-    def build_temperature_payload(self, temperature: float):
-        payload = self.build_base_payload()
-        payload["actmp"] = str(temperature)
-        return payload
-
-    def set_temperature(self, topic: str, temperature: float):
-        self.client.publish(
-            topic, json.dumps(self.build_temperature_payload(temperature))
-        )
-
-    # HVAC Mode
-    def build_hvac_mode_payload(self, mode: HVACMode):
-        payload = self.build_base_payload()
-        payload["acmd"] = str(mode)
-        return payload
-
-    def set_hvac_mode(self, topic: str, mode: HVACMode):
-        self.client.publish(topic, json.dumps(self.build_hvac_mode_payload(mode)))
-
-    # Fan Mode
-    def build_fan_mode_payload(self, mode: FanMode):
-        payload = self.build_base_payload()
-        payload["acfs"] = str(mode)
-        return payload
-
-    def set_fan_mode(self, topic: str, mode: FanMode):
-        self.client.publish(topic, json.dumps(self.build_fan_mode_payload(mode)))
-
-    # Preset Mode
-    def build_preset_mode_payload(self, mode: PresetMode):
-        payload = self.build_base_payload()
-
-        if mode == PresetMode.NONE:
-            payload["acem"] = "off"
-            payload["acpm"] = "off"
-        elif mode == PresetMode.ECO:
-            payload["acem"] = "on"
-            payload["acpm"] = "off"
-            payload["actmp"] = 26.0
-        elif mode == PresetMode.BOOST:
-            payload["acem"] = "off"
-            payload["acpm"] = "on"
-        return payload
-
-    def set_preset_mode(self, topic: str, mode: PresetMode):
-        self.client.publish(topic, json.dumps(self.build_preset_mode_payload(mode)))
-
-    # Swing Mode
-    def build_swing_mode_payload(self, mode: SwingMode):
-        payload = self.build_base_payload()
-        payload["acvs"] = mode
-        return payload
-
-    def set_swing_mode(self, topic: str, mode: SwingMode):
-        self.client.publish(topic, json.dumps(self.build_swing_mode_payload(mode)))
+from aiomqtt import Client, Message, MqttError
+import asyncio
+import ssl
+import certifi
+import random
+import json
+from .enums import PowerMode, HVACMode, FanMode, PresetMode, SwingMode
+from .user import User
+
+
+class MirAIeBroker:
+    host = "mqtt.miraie.in"
+    port = 8883
+    use_ssl = True
+    client_id = f"ha-mirae-mqtt-{random.randint(0, 1000)}"
+    reconnect_interval = 5  # In seconds
+
+    def __init__(self) -> None:
+        self.status_callbacks: dict[str, callable] = {}
+
+    def register_device_callback(self, topic: str, callback):
+        self.status_callbacks[topic] = callback
+
+    def remove_device_callback(self, topic: str):
+        self.status_callbacks.pop(topic, None)
+
+    def set_topics(self, topics: list[str]):
+        self.commandTopics = topics
+
+    async def on_connect(self):
+        for topic in self.commandTopics:
+            print("Subscribing to topic: ", topic)
+            await self.client.subscribe(topic)
+
+    def on_message(self, message: Message):
+        parsed = json.loads(message.payload.decode("utf-8"))
+        func = self.status_callbacks.get(message.topic.value)
+        func(parsed)
+
+    async def connect(self, username: str, access_token: User, get_token):
+        # Set on_token_expire callback
+        password = access_token
+
+        context = None
+
+        if self.use_ssl:
+            context = ssl.create_default_context(cafile=certifi.where())
+
+        while True:
+            try:
+                async with Client(
+                    hostname=self.host,
+                    port=self.port,
+                    username=username,
+                    password=password,
+                    tls_context=context,
+                ) as client:
+                    self.client = client
+                    await self.on_connect()
+                    async for message in client.messages:
+                        self.on_message(message)
+
+            except MqttError as error:
+                print(
+                    f'Error "{error}". Reconnecting in {self.reconnect_interval} seconds.'
+                )
+                password = await get_token()
+                await asyncio.sleep(self.reconnect_interval)
+
+    def build_base_payload(self):
+        return {
+            "ki": 1,
+            "cnt": "an",
+            "sid": "1",
+        }
+
+    # Power
+    def build_power_payload(self, power: PowerMode):
+        payload = self.build_base_payload()
+        payload["ps"] = str(power.value)
+        return payload
+
+    async def set_power(self, topic: str, power: PowerMode):
+        await self.client.publish(topic, json.dumps(self.build_power_payload(power)))
+
+    # Temperature
+    def build_temperature_payload(self, temperature: float):
+        payload = self.build_base_payload()
+        payload["actmp"] = str(temperature)
+        return payload
+
+    async def set_temperature(self, topic: str, temperature: float):
+        await self.client.publish(
+            topic, json.dumps(self.build_temperature_payload(temperature))
+        )
+
+    # HVAC Mode
+    def build_hvac_mode_payload(self, mode: HVACMode):
+        payload = self.build_base_payload()
+        payload["acmd"] = str(mode.value)
+        return payload
+
+    async def set_hvac_mode(self, topic: str, mode: HVACMode):
+        await self.client.publish(topic, json.dumps(self.build_hvac_mode_payload(mode)))
+
+    # Fan Mode
+    def build_fan_mode_payload(self, mode: FanMode):
+        payload = self.build_base_payload()
+        payload["acfs"] = str(mode.value)
+        return payload
+
+    async def set_fan_mode(self, topic: str, mode: FanMode):
+        await self.client.publish(topic, json.dumps(self.build_fan_mode_payload(mode)))
+
+    # Preset Mode
+    def build_preset_mode_payload(self, mode: PresetMode):
+        payload = self.build_base_payload()
+
+        if mode == PresetMode.NONE:
+            payload["acem"] = "off"
+            payload["acpm"] = "off"
+        elif mode == PresetMode.ECO:
+            payload["acem"] = "on"
+            payload["acpm"] = "off"
+            payload["actmp"] = 26.0
+        elif mode == PresetMode.BOOST:
+            payload["acem"] = "off"
+            payload["acpm"] = "on"
+        return payload
+
+    async def set_preset_mode(self, topic: str, mode: PresetMode):
+        await self.client.publish(
+            topic, json.dumps(self.build_preset_mode_payload(mode))
+        )
+
+    # Swing Mode
+    def build_swing_mode_payload(self, mode: SwingMode):
+        payload = self.build_base_payload()
+        payload["acvs"] = mode.value
+        return payload
+
+    async def set_swing_mode(self, topic: str, mode: SwingMode):
+        await self.client.publish(
+            topic, json.dumps(self.build_swing_mode_payload(mode))
+        )
```

### Comparing `miraie-ac-0.2.9/miraie_ac/constants.py` & `miraie_ac-1.0.0/miraie_ac/constants.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-httpClientId = "PBcMcfG19njNCL8AOgvRzIC8AjQa"
-loginUrl = "https://auth.miraie.in/simplifi/v1/userManagement/login"
-homesUrl = "https://app.miraie.in/simplifi/v1/homeManagement/homes"
-statusUrl = "https://app.miraie.in/simplifi/v1/deviceManagement/devices/{deviceId}/mobile/status"
-deviceDetailsUrl = "https://app.miraie.in/simplifi/v1/deviceManagement/devices/deviceId"
-monthlyPwrConsUrl = "https://app.miraie.in/simplifi/v1/powerConsumption/devices/{deviceId}?grain=Monthly&startDate={date}&endDate={date}"
-dailyPwrConsUrl = "https://app.miraie.in/simplifi/v1/powerConsumption/devices/{deviceId}?grain=Daily&startDate={date}&endDate={date}"
+httpClientId = "PBcMcfG19njNCL8AOgvRzIC8AjQa"
+loginUrl = "https://auth.miraie.in/simplifi/v1/userManagement/login"
+homesUrl = "https://app.miraie.in/simplifi/v1/homeManagement/homes"
+statusUrl = "https://app.miraie.in/simplifi/v1/deviceManagement/devices/{deviceId}/mobile/status"
+deviceDetailsUrl = "https://app.miraie.in/simplifi/v1/deviceManagement/devices/deviceId"
+monthlyPwrConsUrl = "https://app.miraie.in/simplifi/v1/powerConsumption/devices/{deviceId}?grain=Monthly&startDate={date}&endDate={date}"
+dailyPwrConsUrl = "https://app.miraie.in/simplifi/v1/powerConsumption/devices/{deviceId}?grain=Daily&startDate={date}&endDate={date}"
```

