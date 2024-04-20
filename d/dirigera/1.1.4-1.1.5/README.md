# Comparing `tmp/dirigera-1.1.4.tar.gz` & `tmp/dirigera-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirigera-1.1.4.tar", last modified: Thu Apr 18 20:12:29 2024, max compression
+gzip compressed data, was "dirigera-1.1.5.tar", last modified: Sat Apr 20 08:49:56 2024, max compression
```

## Comparing `dirigera-1.1.4.tar` & `dirigera-1.1.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:29.901203 dirigera-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-18 20:12:25.000000 dirigera-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-04-18 20:12:29.901203 dirigera-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-04-18 20:12:25.000000 dirigera-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-18 20:12:25.000000 dirigera-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:12:29.901203 dirigera-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-18 20:12:25.000000 dirigera-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:29.893203 dirigera-1.1.4/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:25.000000 dirigera-1.1.4/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:29.893203 dirigera-1.1.4/src/dirigera/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 20:12:25.000000 dirigera-1.1.4/src/dirigera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:29.897203 dirigera-1.1.4/src/dirigera/devices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:25.000000 dirigera-1.1.4/src/dirigera/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-18 20:12:25.000000 dirigera-1.1.4/src/dirigera/devices/air_purifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-18 20:12:25.000000 dirigera-1.1.4/src/dirigera/devices/base_ikea_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-18 20:12:25.000000 dirigera-1.1.4/src/dirigera/devices/blinds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-18 20:12:25.000000 dirigera-1.1.4/src/dirigera/devices/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-18 20:12:25.000000 dirigera-1.1.4/src/dirigera/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-18 20:12:25.000000 dirigera-1.1.4/src/dirigera/devices/environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-18 20:12:25.000000 dirigera-1.1.4/src/dirigera/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-18 20:12:25.000000 dirigera-1.1.4/src/dirigera/devices/motion_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-18 20:12:25.000000 dirigera-1.1.4/src/dirigera/devices/open_close_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-18 20:12:25.000000 dirigera-1.1.4/src/dirigera/devices/outlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-18 20:12:25.000000 dirigera-1.1.4/src/dirigera/devices/scene.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-18 20:12:25.000000 dirigera-1.1.4/src/dirigera/devices/water_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:29.897203 dirigera-1.1.4/src/dirigera/hub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:25.000000 dirigera-1.1.4/src/dirigera/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-18 20:12:25.000000 dirigera-1.1.4/src/dirigera/hub/abstract_smart_home_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-18 20:12:25.000000 dirigera-1.1.4/src/dirigera/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    15813 2024-04-18 20:12:25.000000 dirigera-1.1.4/src/dirigera/hub/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-18 20:12:25.000000 dirigera-1.1.4/src/dirigera/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:29.901203 dirigera-1.1.4/src/dirigera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-04-18 20:12:29.000000 dirigera-1.1.4/src/dirigera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-18 20:12:29.000000 dirigera-1.1.4/src/dirigera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:12:29.000000 dirigera-1.1.4/src/dirigera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-18 20:12:29.000000 dirigera-1.1.4/src/dirigera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-18 20:12:29.000000 dirigera-1.1.4/src/dirigera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 20:12:29.000000 dirigera-1.1.4/src/dirigera.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:12:29.901203 dirigera-1.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-18 20:12:25.000000 dirigera-1.1.4/tests/test_air_purifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-18 20:12:25.000000 dirigera-1.1.4/tests/test_blinds.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-18 20:12:25.000000 dirigera-1.1.4/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-18 20:12:25.000000 dirigera-1.1.4/tests/test_environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-04-18 20:12:25.000000 dirigera-1.1.4/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-18 20:12:25.000000 dirigera-1.1.4/tests/test_motion_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-18 20:12:25.000000 dirigera-1.1.4/tests/test_open_close_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-18 20:12:25.000000 dirigera-1.1.4/tests/test_outlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-18 20:12:25.000000 dirigera-1.1.4/tests/test_scenes.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-18 20:12:25.000000 dirigera-1.1.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-18 20:12:25.000000 dirigera-1.1.4/tests/test_water_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:49:56.037443 dirigera-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-20 08:49:52.000000 dirigera-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-04-20 08:49:56.037443 dirigera-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13383 2024-04-20 08:49:52.000000 dirigera-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-20 08:49:52.000000 dirigera-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 08:49:56.037443 dirigera-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-20 08:49:52.000000 dirigera-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:49:56.029443 dirigera-1.1.5/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:49:56.029443 dirigera-1.1.5/src/dirigera/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:49:56.033443 dirigera-1.1.5/src/dirigera/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/air_purifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/base_ikea_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/blinds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/motion_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/open_close_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/outlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/devices/water_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:49:56.033443 dirigera-1.1.5/src/dirigera/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/hub/abstract_smart_home_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15813 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/hub/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-20 08:49:52.000000 dirigera-1.1.5/src/dirigera/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:49:56.033443 dirigera-1.1.5/src/dirigera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-04-20 08:49:56.000000 dirigera-1.1.5/src/dirigera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-20 08:49:56.000000 dirigera-1.1.5/src/dirigera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 08:49:56.000000 dirigera-1.1.5/src/dirigera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-20 08:49:56.000000 dirigera-1.1.5/src/dirigera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-20 08:49:56.000000 dirigera-1.1.5/src/dirigera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-20 08:49:56.000000 dirigera-1.1.5/src/dirigera.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:49:56.033443 dirigera-1.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_air_purifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_blinds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_motion_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_open_close_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_outlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_scenes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-20 08:49:52.000000 dirigera-1.1.5/tests/test_water_sensor.py
```

### Comparing `dirigera-1.1.4/LICENSE` & `dirigera-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/PKG-INFO` & `dirigera-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 1.1.4
+Version: 1.1.5
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -113,14 +113,15 @@
 
 All available devices (Light, Controller, Outlet, ...) consist of the core data defined in [device.py](./src/dirigera/devices/device.py):
 
 ### Core Device Data
 
 ```python
 id: str
+relation_id: Optional[str] = None
 type: str
 device_type: str
 created_at: datetime.datetime
 is_reachable: bool
 last_seen: datetime.datetime
 attributes: Attributes
 capabilities: Capabilities
@@ -304,14 +305,15 @@
 ```
 
 The controller object has the following attributes (additional to the core attributes):
 
 ```python
 is_on: bool
 battery_percentage: Optional[int] = None
+switch_label: Optional[str] = None
 ```
 
 Available methods for controller are:
 
 ```python
 controller.set_name(name="kitchen remote 1")
 ```
```

### Comparing `dirigera-1.1.4/README.md` & `dirigera-1.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 
 All available devices (Light, Controller, Outlet, ...) consist of the core data defined in [device.py](./src/dirigera/devices/device.py):
 
 ### Core Device Data
 
 ```python
 id: str
+relation_id: Optional[str] = None
 type: str
 device_type: str
 created_at: datetime.datetime
 is_reachable: bool
 last_seen: datetime.datetime
 attributes: Attributes
 capabilities: Capabilities
@@ -257,14 +258,15 @@
 ```
 
 The controller object has the following attributes (additional to the core attributes):
 
 ```python
 is_on: bool
 battery_percentage: Optional[int] = None
+switch_label: Optional[str] = None
 ```
 
 Available methods for controller are:
 
 ```python
 controller.set_name(name="kitchen remote 1")
 ```
```

### Comparing `dirigera-1.1.4/pyproject.toml` & `dirigera-1.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dirigera"
-version = "1.1.4"
+version = "1.1.5"
 description = "An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub"
 readme = "README.md"
 authors = [{ name = "Leggin", email = "legginsun@gmail.com" }]
 license = { file = "LICENSE" }
 keywords = [
     "python",
     "iot",
```

### Comparing `dirigera-1.1.4/src/dirigera/devices/air_purifier.py` & `dirigera-1.1.5/src/dirigera/devices/air_purifier.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/src/dirigera/devices/blinds.py` & `dirigera-1.1.5/src/dirigera/devices/blinds.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/src/dirigera/devices/controller.py` & `dirigera-1.1.5/src/dirigera/devices/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .device import Attributes, Device
 from ..hub.abstract_smart_home_hub import AbstractSmartHomeHub
 
 
 class ControllerAttributes(Attributes):
     is_on: bool
     battery_percentage: Optional[int] = None
+    switch_label: Optional[str] = None
 
 
 class Controller(Device):
     dirigera_client: AbstractSmartHomeHub
     attributes: ControllerAttributes
 
     def reload(self) -> Controller:
```

### Comparing `dirigera-1.1.4/src/dirigera/devices/device.py` & `dirigera-1.1.5/src/dirigera/devices/device.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/src/dirigera/devices/environment_sensor.py` & `dirigera-1.1.5/src/dirigera/devices/environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/src/dirigera/devices/light.py` & `dirigera-1.1.5/src/dirigera/devices/light.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/src/dirigera/devices/motion_sensor.py` & `dirigera-1.1.5/src/dirigera/devices/motion_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/src/dirigera/devices/open_close_sensor.py` & `dirigera-1.1.5/src/dirigera/devices/open_close_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/src/dirigera/devices/outlet.py` & `dirigera-1.1.5/src/dirigera/devices/outlet.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/src/dirigera/devices/scene.py` & `dirigera-1.1.5/src/dirigera/devices/scene.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     attributes: Optional[ActionAttributes] = None
 
 
 class SceneType(Enum):
     USER_SCENE = "userScene"
     CUSTOM_SCENE = "customScene"
     PLAYLIST_SCENE = "playlistScene"
+    WAKEUP_SCENE = "wakeUpScene"
 
 
 class Scene(BaseIkeaModel):
     dirigera_client: AbstractSmartHomeHub
     id: str
     type: SceneType
     info: Info
```

### Comparing `dirigera-1.1.4/src/dirigera/devices/water_sensor.py` & `dirigera-1.1.5/src/dirigera/devices/water_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/src/dirigera/hub/abstract_smart_home_hub.py` & `dirigera-1.1.5/src/dirigera/hub/abstract_smart_home_hub.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/src/dirigera/hub/auth.py` & `dirigera-1.1.5/src/dirigera/hub/auth.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/src/dirigera/hub/hub.py` & `dirigera-1.1.5/src/dirigera/hub/hub.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/src/dirigera.egg-info/PKG-INFO` & `dirigera-1.1.5/src/dirigera.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 1.1.4
+Version: 1.1.5
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -113,14 +113,15 @@
 
 All available devices (Light, Controller, Outlet, ...) consist of the core data defined in [device.py](./src/dirigera/devices/device.py):
 
 ### Core Device Data
 
 ```python
 id: str
+relation_id: Optional[str] = None
 type: str
 device_type: str
 created_at: datetime.datetime
 is_reachable: bool
 last_seen: datetime.datetime
 attributes: Attributes
 capabilities: Capabilities
@@ -304,14 +305,15 @@
 ```
 
 The controller object has the following attributes (additional to the core attributes):
 
 ```python
 is_on: bool
 battery_percentage: Optional[int] = None
+switch_label: Optional[str] = None
 ```
 
 Available methods for controller are:
 
 ```python
 controller.set_name(name="kitchen remote 1")
 ```
```

### Comparing `dirigera-1.1.4/src/dirigera.egg-info/SOURCES.txt` & `dirigera-1.1.5/src/dirigera.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/tests/test_air_purifier.py` & `dirigera-1.1.5/tests/test_air_purifier.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/tests/test_blinds.py` & `dirigera-1.1.5/tests/test_blinds.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/tests/test_controller.py` & `dirigera-1.1.5/tests/test_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,18 @@
         "deviceSet": [],
         "remoteLinks": [],
         "isHidden": False
     }
 
     controller = dict_to_controller(somrig_button_1, fake_client)
     assert controller.relation_id == somrig_button_1["relationId"]
+    assert (
+        controller.attributes.switch_label
+        == somrig_button_1["attributes"]["switchLabel"]
+    )
 
     somrig_button_2: Dict[str, Any] = {
         "id": "1111aaaa-1111-1111-aa11-1a1aa1a111a1_2",
         "relationId": "1111aaaa-1111-1111-aa11-1a1aa1a111a1",
         "type": "controller",
         "deviceType": "shortcutController",
         "createdAt": "2024-04-12T20:50:26.000Z",
@@ -206,7 +210,11 @@
         "deviceSet": [],
         "remoteLinks": [],
         "isHidden": False
     }
 
     controller = dict_to_controller(somrig_button_2, fake_client)
     assert controller.relation_id == somrig_button_2["relationId"]
+    assert (
+        controller.attributes.switch_label
+        == somrig_button_2["attributes"]["switchLabel"]
+    )
```

### Comparing `dirigera-1.1.4/tests/test_environment_sensor.py` & `dirigera-1.1.5/tests/test_environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/tests/test_light.py` & `dirigera-1.1.5/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/tests/test_motion_sensor.py` & `dirigera-1.1.5/tests/test_motion_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/tests/test_open_close_sensor.py` & `dirigera-1.1.5/tests/test_open_close_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/tests/test_outlet.py` & `dirigera-1.1.5/tests/test_outlet.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/tests/test_scenes.py` & `dirigera-1.1.5/tests/test_scenes.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/tests/test_utils.py` & `dirigera-1.1.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.4/tests/test_water_sensor.py` & `dirigera-1.1.5/tests/test_water_sensor.py`

 * *Files identical despite different names*

