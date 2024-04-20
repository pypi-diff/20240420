# Comparing `tmp/feagi_connector-0.0.5.tar.gz` & `tmp/feagi_connector-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feagi_connector-0.0.5.tar", last modified: Wed Apr 17 16:41:53 2024, max compression
+gzip compressed data, was "feagi_connector-0.0.6.tar", last modified: Sat Apr 20 03:50:14 2024, max compression
```

## Comparing `feagi_connector-0.0.5.tar` & `feagi_connector-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:53.633633 feagi_connector-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-17 16:41:53.633633 feagi_connector-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:53.629633 feagi_connector-0.0.5/feagi_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/PIL_retina.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6091 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/actuators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    21468 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/feagi_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    20062 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/pns_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    25199 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/retina.py
--rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:53.629633 feagi_connector-0.0.5/feagi_connector/sensorimotor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/sensorimotor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/testing_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/feagi_connector/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 16:41:44.000000 feagi_connector-0.0.5/feagi_connector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:53.633633 feagi_connector-0.0.5/feagi_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-17 16:41:53.000000 feagi_connector-0.0.5/feagi_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-17 16:41:53.000000 feagi_connector-0.0.5/feagi_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:41:53.000000 feagi_connector-0.0.5/feagi_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-17 16:41:53.000000 feagi_connector-0.0.5/feagi_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 16:41:53.000000 feagi_connector-0.0.5/feagi_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-17 16:41:42.000000 feagi_connector-0.0.5/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      766 2024-04-17 16:41:53.633633 feagi_connector-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:50:14.554426 feagi_connector-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-20 03:50:04.000000 feagi_connector-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-20 03:50:14.554426 feagi_connector-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-20 03:50:04.000000 feagi_connector-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:50:14.554426 feagi_connector-0.0.6/feagi_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-20 03:50:04.000000 feagi_connector-0.0.6/feagi_connector/PIL_retina.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:50:04.000000 feagi_connector-0.0.6/feagi_connector/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6091 2024-04-20 03:50:04.000000 feagi_connector-0.0.6/feagi_connector/actuators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-20 03:50:04.000000 feagi_connector-0.0.6/feagi_connector/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21468 2024-04-20 03:50:04.000000 feagi_connector-0.0.6/feagi_connector/feagi_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20262 2024-04-20 03:50:04.000000 feagi_connector-0.0.6/feagi_connector/pns_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26080 2024-04-20 03:50:04.000000 feagi_connector-0.0.6/feagi_connector/retina.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-04-20 03:50:04.000000 feagi_connector-0.0.6/feagi_connector/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:50:14.554426 feagi_connector-0.0.6/feagi_connector/sensorimotor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:50:04.000000 feagi_connector-0.0.6/feagi_connector/sensorimotor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-20 03:50:04.000000 feagi_connector-0.0.6/feagi_connector/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-20 03:50:04.000000 feagi_connector-0.0.6/feagi_connector/testing_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-20 03:50:04.000000 feagi_connector-0.0.6/feagi_connector/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-20 03:50:04.000000 feagi_connector-0.0.6/feagi_connector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:50:14.554426 feagi_connector-0.0.6/feagi_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-20 03:50:14.000000 feagi_connector-0.0.6/feagi_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-20 03:50:14.000000 feagi_connector-0.0.6/feagi_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 03:50:14.000000 feagi_connector-0.0.6/feagi_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-20 03:50:14.000000 feagi_connector-0.0.6/feagi_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-20 03:50:14.000000 feagi_connector-0.0.6/feagi_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-20 03:50:04.000000 feagi_connector-0.0.6/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      784 2024-04-20 03:50:14.558426 feagi_connector-0.0.6/setup.cfg
```

### Comparing `feagi_connector-0.0.5/LICENSE` & `feagi_connector-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.5/PKG-INFO` & `feagi_connector-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi_connector
-Version: 0.0.5
+Version: 0.0.6
 Summary: Feagi agent to work with general and simulation robots
 Home-page: https://github.com/feagi/feagi-connector
 Author: Neuraville Inc.
 Author-email: info@feagi.org
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,14 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: numpy
 Requires-Dist: zmq
 Requires-Dist: numpy
 Requires-Dist: lz4
+Requires-Dist: websockets==12.0
 Requires-Dist: opencv-python==4.6.0.66; python_version < "3.8"
 
 # What is feagi-connector?
 The feagi-connector is the core of the Feagi agent and it serves multiple purposes. It works behind the scenes and serves as an API for Feagi.
 Keep in mind, you will need Feagi to connect with feagi_connector. Feagi can be running on a website, Docker, or locally on your computer. 
 
 If you would like to learn more about how to run Feagi, please visit: https://github.com/feagi/feagi/tree/staging
```

### Comparing `feagi_connector-0.0.5/README.md` & `feagi_connector-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.5/feagi_connector/PIL_retina.py` & `feagi_connector-0.0.6/feagi_connector/PIL_retina.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.5/feagi_connector/actuators.py` & `feagi_connector-0.0.6/feagi_connector/actuators.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.5/feagi_connector/configuration.py` & `feagi_connector-0.0.6/feagi_connector/configuration.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.5/feagi_connector/feagi_interface.py` & `feagi_connector-0.0.6/feagi_connector/feagi_interface.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.5/feagi_connector/pns_gateway.py` & `feagi_connector-0.0.6/feagi_connector/pns_gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,19 +37,20 @@
 
 def generate_feagi_data(rgb, msg_counter, date, message_to_feagi):
     """
     This function generates data for Feagi by combining RGB values, message counter, and date into
     the provided message.
     """
     try:
-        if "data" not in message_to_feagi:
-            message_to_feagi["data"] = dict()
-        if "sensory_data" not in message_to_feagi["data"]:
-            message_to_feagi["data"]["sensory_data"] = dict()
-        message_to_feagi["data"]["sensory_data"]['camera'] = rgb['camera']
+        if rgb:
+            if "data" not in message_to_feagi:
+                message_to_feagi["data"] = dict()
+            if "sensory_data" not in message_to_feagi["data"]:
+                message_to_feagi["data"]["sensory_data"] = dict()
+            message_to_feagi["data"]["sensory_data"]['camera'] = rgb['camera']
     except Exception as e:
         print("ERROR: ", e)
     message_to_feagi['timestamp'] = date
     message_to_feagi['counter'] = msg_counter
     return message_to_feagi
 
 
@@ -69,19 +70,22 @@
 
 
 def signals_from_feagi(feagi_opu_channel):
     """ get OPU from FEAGI """
     return router.fetch_feagi(feagi_opu_channel)
 
 
-def signals_to_feagi(message_to_feagi, feagi_ipu_channel, agent_settings):
+def signals_to_feagi(message_to_feagi, feagi_ipu_channel, agent_settings, feagi_settings):
     """
     Sends data to FEAGI through the router.py
     """
-    router.send_feagi(message_to_feagi, feagi_ipu_channel, agent_settings)
+    if 'magic_link' not in feagi_settings:
+        router.send_feagi(message_to_feagi, feagi_ipu_channel, agent_settings)
+    else:
+        router.websocket_send(message_to_feagi)
 
 
 def grab_geometry():
     """
     To get the size of vision cortical areas (e.g., C, TL, TM...)
     """
     return router.fetch_geometry()
@@ -265,14 +269,15 @@
             full_list_dimension = fetch_full_dimensions()
             response = full_list_dimension
             resize_list = retina.obtain_cortical_vision_size(capabilities['camera']["index"],
                                                              response)
             previous_genome_timestamp = message_from_feagi["genome_changed"]
         current_tracker = obtain_genome_number(genome_tracker, message_from_feagi)
         if len(resize_list) == 0:
+            response = full_list_dimension
             resize_list = retina.obtain_cortical_vision_size(capabilities['camera']["index"],
                                                              response)
         if genome_tracker != current_tracker:
             full_list_dimension = fetch_full_dimensions()
             genome_tracker = current_tracker
```

### Comparing `feagi_connector-0.0.5/feagi_connector/retina.py` & `feagi_connector-0.0.6/feagi_connector/retina.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from feagi_connector import router
 from time import sleep
 import asyncio
 import zmq.asyncio
 
 genome_tracker = 0
 previous_genome_timestamp = 0
+current_dimension_list = {}
 
 
 def get_device_of_vision(device):
     """
     Obtain the camera source and bind it using the provided address.
 
     Args:
@@ -320,57 +321,72 @@
         feagi_data = create_feagi_data(thresholded, current, previous.shape)
         return dict(feagi_data)
     else:
         return {}
 
 
 def get_full_dimension_of_cortical_area(cortical_name):
-    return pns.resize_list[cortical_name][0] * pns.resize_list[cortical_name][1] * \
-           pns.resize_list[cortical_name][2]
+    global current_dimension_list
+    return current_dimension_list[cortical_name][0] * current_dimension_list[cortical_name][1] * \
+           current_dimension_list[cortical_name][2]
 
 def process_visual_stimuli(raw_frame, capabilities,
                                  previous_frame_data,
                                  rgb, actual_capabilities, compare_image=True):
+    global current_dimension_list
     capabilities = pns.create_runtime_default_list(capabilities, actual_capabilities)
     if pns.resize_list:
+        current_dimension_list = pns.resize_list
         if capabilities["camera"]["mirror"]:
             raw_frame = cv2.flip(raw_frame, 1)
         region_coordinates = vision_region_coordinates(frame_width=raw_frame.shape[1],
                                                        frame_height=raw_frame.shape[0],
                                                        x1=abs(capabilities['camera']['gaze_control']['0']),
                                                        x2=abs(capabilities['camera']['pupil_control']['0']),
                                                        y1=abs(capabilities['camera']['gaze_control']['1']),
                                                        y2=abs(capabilities['camera']['pupil_control']['1']),
                                                        camera_index=capabilities['camera']['index'],
-                                                       size_list=pns.resize_list)
+                                                       size_list=current_dimension_list)
         segmented_frame_data = split_vision_regions(coordinates=region_coordinates,
                                                     raw_frame_data=raw_frame)
         compressed_data = dict()
         for cortical in segmented_frame_data:
             compressed_data[cortical] = effect(downsize_regions(segmented_frame_data[cortical],
-                                                                pns.resize_list[cortical]), capabilities)
+                                                                current_dimension_list[cortical]), capabilities)
         vision_dict = dict()
 
         # for segment in compressed_data:
         #     cv2.imshow(segment, compressed_data[segment])
         if cv2.waitKey(30) & 0xFF == ord('q'):
             pass
         for get_region in compressed_data:
-            if pns.resize_list[get_region][2] == 3:
+            if current_dimension_list[get_region][2] == 3:
                 if previous_frame_data != {}:
-                    vision_dict[get_region] = change_detector(
-                        previous_frame_data[get_region],
-                        compressed_data[get_region],
-                        capabilities, compare_image, get_region)
+                    if get_region in previous_frame_data:
+                        vision_dict[get_region] = change_detector(
+                            previous_frame_data[get_region],
+                            compressed_data[get_region],
+                            capabilities, compare_image, get_region)
+                    else:
+                        vision_dict[get_region] = change_detector(
+                            np.zeros((3, 3, 3)),
+                            compressed_data[get_region],
+                            capabilities, compare_image, get_region)
             else:
                 if previous_frame_data != {}:
-                    vision_dict[get_region] = change_detector_grayscale(
-                        previous_frame_data[get_region],
-                        compressed_data[get_region],
-                        capabilities, compare_image, get_region)
+                    if get_region in previous_frame_data:
+                        vision_dict[get_region] = change_detector_grayscale(
+                            previous_frame_data[get_region],
+                            compressed_data[get_region],
+                            capabilities, compare_image, get_region)
+                    else:
+                        vision_dict[get_region] = change_detector_grayscale(
+                            np.zeros((3, 3, 3)),
+                            compressed_data[get_region],
+                            capabilities, compare_image, get_region)
         previous_frame_data = compressed_data
         rgb['camera'] = vision_dict
         return previous_frame_data, rgb, capabilities
     return pns.resize_list, pns.resize_list, capabilities  # sending empty dict
 
 
 def obtain_cortical_vision_size(camera_index, response):
```

### Comparing `feagi_connector-0.0.5/feagi_connector/router.py` & `feagi_connector-0.0.6/feagi_connector/router.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.5/feagi_connector/sensors.py` & `feagi_connector-0.0.6/feagi_connector/sensors.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.5/feagi_connector/testing_mode.py` & `feagi_connector-0.0.6/feagi_connector/testing_mode.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.5/feagi_connector/trainer.py` & `feagi_connector-0.0.6/feagi_connector/trainer.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.5/feagi_connector.egg-info/PKG-INFO` & `feagi_connector-0.0.6/feagi_connector.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi_connector
-Version: 0.0.5
+Version: 0.0.6
 Summary: Feagi agent to work with general and simulation robots
 Home-page: https://github.com/feagi/feagi-connector
 Author: Neuraville Inc.
 Author-email: info@feagi.org
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,14 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: numpy
 Requires-Dist: zmq
 Requires-Dist: numpy
 Requires-Dist: lz4
+Requires-Dist: websockets==12.0
 Requires-Dist: opencv-python==4.6.0.66; python_version < "3.8"
 
 # What is feagi-connector?
 The feagi-connector is the core of the Feagi agent and it serves multiple purposes. It works behind the scenes and serves as an API for Feagi.
 Keep in mind, you will need Feagi to connect with feagi_connector. Feagi can be running on a website, Docker, or locally on your computer. 
 
 If you would like to learn more about how to run Feagi, please visit: https://github.com/feagi/feagi/tree/staging
```

### Comparing `feagi_connector-0.0.5/feagi_connector.egg-info/SOURCES.txt` & `feagi_connector-0.0.6/feagi_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.5/setup.cfg` & `feagi_connector-0.0.6/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = feagi_connector
-version = 0.0.5
+version = 0.0.6
 author = Neuraville Inc.
 author_email = info@feagi.org
 description = Feagi agent to work with general and simulation robots
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/feagi/feagi-connector
 project_urls = 
@@ -21,14 +21,15 @@
 python_requires = >=3.6
 install_requires = 
 	requests
 	numpy
 	zmq
 	numpy
 	lz4
+	websockets==12.0
 	opencv-python==4.6.0.66; python_version<"3.8"
 
 [options.packages.find]
 where = .
 
 [egg_info]
 tag_build =
```

