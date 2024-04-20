# Comparing `tmp/pyrealsense2-2.55.1.6481-cp311-cp311-manylinux1_x86_64.whl.zip` & `tmp/pyrealsense2-2.9.1-cp36-cp36m-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,18 @@
-Zip file size: 3453746 bytes, number of entries: 14
--rw-r--r--  2.0 unx       86 b- defN 24-Apr-20 17:36 pyrealsense2/__init__.py
--rw-r--r--  2.0 unx       28 b- defN 24-Apr-20 17:36 pyrealsense2/_version.py
--rwxr-xr-x  2.0 unx 10465136 b- defN 24-Apr-20 17:36 pyrealsense2/pyrealsense2.cpython-311-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   493824 b- defN 24-Apr-20 17:36 pyrealsense2/pyrsutils.cpython-311-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx     3627 b- defN 24-Apr-20 17:34 pyrealsense2-2.55.1.6481.data/scripts/align-depth2color.py
--rwxr-xr-x  2.0 unx     1623 b- defN 24-Apr-20 17:34 pyrealsense2-2.55.1.6481.data/scripts/export_ply_example.py
--rwxr-xr-x  2.0 unx     2491 b- defN 24-Apr-20 17:34 pyrealsense2-2.55.1.6481.data/scripts/opencv_viewer_example.py
--rwxr-xr-x  2.0 unx     4340 b- defN 24-Apr-20 17:34 pyrealsense2-2.55.1.6481.data/scripts/python-rs400-advanced-mode-example.py
--rwxr-xr-x  2.0 unx     1929 b- defN 24-Apr-20 17:34 pyrealsense2-2.55.1.6481.data/scripts/python-tutorial-1-depth.py
--rw-r--r--  2.0 unx    11352 b- defN 24-Apr-20 17:36 pyrealsense2-2.55.1.6481.dist-info/LICENSE
--rw-r--r--  2.0 unx     1846 b- defN 24-Apr-20 17:36 pyrealsense2-2.55.1.6481.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 24-Apr-20 17:36 pyrealsense2-2.55.1.6481.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-Apr-20 17:36 pyrealsense2-2.55.1.6481.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1435 b- defN 24-Apr-20 17:36 pyrealsense2-2.55.1.6481.dist-info/RECORD
-14 files, 10987835 bytes uncompressed, 3451278 bytes compressed:  68.6%
+Zip file size: 7784250 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat       61 b- defN 18-Feb-06 14:31 pyrealsense2/__init__.py
+-rw-rw-rw-  2.0 fat       21 b- defN 18-Feb-06 14:31 pyrealsense2/_version.py
+-rw-rw-rw-  2.0 fat  8748032 b- defN 18-Feb-06 14:34 pyrealsense2/pybackend2.cp36-win_amd64.pyd
+-rw-rw-rw-  2.0 fat  8239104 b- defN 18-Feb-06 14:37 pyrealsense2/pyrealsense2.cp36-win_amd64.pyd
+-rw-rw-rw-  2.0 fat 20058624 b- defN 18-Feb-06 14:36 pyrealsense2/realsense2.dll
+-rw-rw-rw-  2.0 fat     2938 b- defN 18-Feb-06 14:31 pyrealsense2-2.9.1.data/scripts/align-depth2color.py
+-rw-rw-rw-  2.0 fat     1209 b- defN 18-Feb-06 14:31 pyrealsense2-2.9.1.data/scripts/export_ply_example.py
+-rw-rw-rw-  2.0 fat     1535 b- defN 18-Feb-06 14:31 pyrealsense2-2.9.1.data/scripts/opencv_viewer_example.py
+-rw-rw-rw-  2.0 fat     4046 b- defN 18-Feb-06 14:31 pyrealsense2-2.9.1.data/scripts/python-rs400-advanced-mode-example.py
+-rw-rw-rw-  2.0 fat     1779 b- defN 18-Feb-06 14:31 pyrealsense2-2.9.1.data/scripts/python-tutorial-1-depth.py
+-rw-rw-rw-  2.0 fat      455 b- defN 18-Feb-06 14:37 pyrealsense2-2.9.1.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat     1413 b- defN 18-Feb-06 14:37 pyrealsense2-2.9.1.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat       13 b- defN 18-Feb-06 14:37 pyrealsense2-2.9.1.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat      106 b- defN 18-Feb-06 14:37 pyrealsense2-2.9.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1872 b- defN 18-Feb-06 14:37 pyrealsense2-2.9.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat     1559 b- defN 18-Feb-06 14:37 pyrealsense2-2.9.1.dist-info/RECORD
+16 files, 37062767 bytes uncompressed, 7781646 bytes compressed:  79.0%
```

## zipnote {}

```diff
@@ -1,43 +1,49 @@
 Filename: pyrealsense2/__init__.py
 Comment: 
 
 Filename: pyrealsense2/_version.py
 Comment: 
 
-Filename: pyrealsense2/pyrealsense2.cpython-311-x86_64-linux-gnu.so
+Filename: pyrealsense2/pybackend2.cp36-win_amd64.pyd
 Comment: 
 
-Filename: pyrealsense2/pyrsutils.cpython-311-x86_64-linux-gnu.so
+Filename: pyrealsense2/pyrealsense2.cp36-win_amd64.pyd
 Comment: 
 
-Filename: pyrealsense2-2.55.1.6481.data/scripts/align-depth2color.py
+Filename: pyrealsense2/realsense2.dll
 Comment: 
 
-Filename: pyrealsense2-2.55.1.6481.data/scripts/export_ply_example.py
+Filename: pyrealsense2-2.9.1.data/scripts/align-depth2color.py
 Comment: 
 
-Filename: pyrealsense2-2.55.1.6481.data/scripts/opencv_viewer_example.py
+Filename: pyrealsense2-2.9.1.data/scripts/export_ply_example.py
 Comment: 
 
-Filename: pyrealsense2-2.55.1.6481.data/scripts/python-rs400-advanced-mode-example.py
+Filename: pyrealsense2-2.9.1.data/scripts/opencv_viewer_example.py
 Comment: 
 
-Filename: pyrealsense2-2.55.1.6481.data/scripts/python-tutorial-1-depth.py
+Filename: pyrealsense2-2.9.1.data/scripts/python-rs400-advanced-mode-example.py
 Comment: 
 
-Filename: pyrealsense2-2.55.1.6481.dist-info/LICENSE
+Filename: pyrealsense2-2.9.1.data/scripts/python-tutorial-1-depth.py
 Comment: 
 
-Filename: pyrealsense2-2.55.1.6481.dist-info/METADATA
+Filename: pyrealsense2-2.9.1.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: pyrealsense2-2.55.1.6481.dist-info/WHEEL
+Filename: pyrealsense2-2.9.1.dist-info/metadata.json
 Comment: 
 
-Filename: pyrealsense2-2.55.1.6481.dist-info/top_level.txt
+Filename: pyrealsense2-2.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyrealsense2-2.55.1.6481.dist-info/RECORD
+Filename: pyrealsense2-2.9.1.dist-info/WHEEL
+Comment: 
+
+Filename: pyrealsense2-2.9.1.dist-info/METADATA
+Comment: 
+
+Filename: pyrealsense2-2.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyrealsense2/__init__.py

```diff
@@ -1,2 +1,2 @@
-# py libs (pyd/so) should be copied to pyrealsense2 folder
+from ._version import __version__
 from .pyrealsense2 import *
```

## pyrealsense2/_version.py

```diff
@@ -1 +1 @@
-__version__ = "2.55.1.6481"
+__version__ = "2.9.1"
```

## Comparing `pyrealsense2-2.55.1.6481.data/scripts/opencv_viewer_example.py` & `pyrealsense2-2.9.1.data/scripts/opencv_viewer_example.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,30 +8,14 @@
 import pyrealsense2 as rs
 import numpy as np
 import cv2
 
 # Configure depth and color streams
 pipeline = rs.pipeline()
 config = rs.config()
-
-# Get device product line for setting a supporting resolution
-pipeline_wrapper = rs.pipeline_wrapper(pipeline)
-pipeline_profile = config.resolve(pipeline_wrapper)
-device = pipeline_profile.get_device()
-device_product_line = str(device.get_info(rs.camera_info.product_line))
-
-found_rgb = False
-for s in device.sensors:
-    if s.get_info(rs.camera_info.name) == 'RGB Camera':
-        found_rgb = True
-        break
-if not found_rgb:
-    print("The demo requires Depth camera with Color sensor")
-    exit(0)
-
 config.enable_stream(rs.stream.depth, 640, 480, rs.format.z16, 30)
 config.enable_stream(rs.stream.color, 640, 480, rs.format.bgr8, 30)
 
 # Start streaming
 pipeline.start(config)
 
 try:
@@ -47,26 +31,19 @@
         # Convert images to numpy arrays
         depth_image = np.asanyarray(depth_frame.get_data())
         color_image = np.asanyarray(color_frame.get_data())
 
         # Apply colormap on depth image (image must be converted to 8-bit per pixel first)
         depth_colormap = cv2.applyColorMap(cv2.convertScaleAbs(depth_image, alpha=0.03), cv2.COLORMAP_JET)
 
-        depth_colormap_dim = depth_colormap.shape
-        color_colormap_dim = color_image.shape
-
-        # If depth and color resolutions are different, resize color image to match depth image for display
-        if depth_colormap_dim != color_colormap_dim:
-            resized_color_image = cv2.resize(color_image, dsize=(depth_colormap_dim[1], depth_colormap_dim[0]), interpolation=cv2.INTER_AREA)
-            images = np.hstack((resized_color_image, depth_colormap))
-        else:
-            images = np.hstack((color_image, depth_colormap))
+        # Stack both images horizontally
+        images = np.hstack((color_image, depth_colormap))
 
         # Show images
         cv2.namedWindow('RealSense', cv2.WINDOW_AUTOSIZE)
         cv2.imshow('RealSense', images)
         cv2.waitKey(1)
 
 finally:
 
     # Stop streaming
-    pipeline.stop()
+    pipeline.stop()
```

## Comparing `pyrealsense2-2.55.1.6481.data/scripts/python-rs400-advanced-mode-example.py` & `pyrealsense2-2.9.1.data/scripts/python-rs400-advanced-mode-example.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 #####################################################
 
 # First import the library
 import pyrealsense2 as rs
 import time
 import json
 
-DS5_product_ids = ["0AD1", "0AD2", "0AD3", "0AD4", "0AD5", "0AF6", "0AFE", "0AFF", "0B00", "0B01", "0B03", "0B07", "0B3A", "0B5C", "0B5B"]
+DS5_product_ids = ["0AD1", "0AD2", "0AD3", "0AD4", "0AD5", "0AF6", "0AFE", "0AFF", "0B00", "0B01", "0B03", "0B07"]
 
 def find_device_that_supports_advanced_mode() :
     ctx = rs.context()
     ds5_dev = rs.device()
     devices = ctx.query_devices();
     for dev in devices:
         if dev.supports(rs.camera_info.product_id) and str(dev.get_info(rs.camera_info.product_id)) in DS5_product_ids:
             if dev.supports(rs.camera_info.name):
                 print("Found device that supports advanced mode:", dev.get_info(rs.camera_info.name))
             return dev
-    raise Exception("No D400 product line device that supports advanced mode was found")
+    raise Exception("No device that supports advanced mode was found")
 
 try:
     dev = find_device_that_supports_advanced_mode()
     advnc_mode = rs.rs400_advanced_mode(dev)
     print("Advanced mode is", "enabled" if advnc_mode.is_enabled() else "disabled")
 
     # Loop until we successfully enable advanced mode
@@ -70,18 +70,15 @@
 
     # Serialize all controls to a Json string
     serialized_string = advnc_mode.serialize_json()
     print("Controls as JSON: \n", serialized_string)
     as_json_object = json.loads(serialized_string)
 
     # We can also load controls from a json string
-    # For Python 2, the values in 'as_json_object' dict need to be converted from unicode object to utf-8
-    if type(next(iter(as_json_object))) != str:
-        as_json_object = {k.encode('utf-8'): v.encode("utf-8") for k, v in as_json_object.items()}
     # The C++ JSON parser requires double-quotes for the json object so we need
-    # to replace the single quote of the pythonic json to double-quotes
+    #  to replace the single quote of the pythonic json to double-quotes
     json_string = str(as_json_object).replace("'", '\"')
     advnc_mode.load_json(json_string)
 
 except Exception as e:
     print(e)
     pass
```

## Comparing `pyrealsense2-2.55.1.6481.data/scripts/python-tutorial-1-depth.py` & `pyrealsense2-2.9.1.data/scripts/python-tutorial-1-depth.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,21 +7,15 @@
 
 # First import the library
 import pyrealsense2 as rs
 
 try:
     # Create a context object. This object owns the handles to all connected realsense devices
     pipeline = rs.pipeline()
-
-    # Configure streams
-    config = rs.config()
-    config.enable_stream(rs.stream.depth, 640, 480, rs.format.z16, 30)
-
-    # Start streaming
-    pipeline.start(config)
+    pipeline.start()
 
     while True:
         # This call waits until a new coherent set of frames is available on a device
         # Calls to get_frame_data(...) and get_frame_timestamp(...) on a device will return stable values until wait_for_frames(...) is called
         frames = pipeline.wait_for_frames()
         depth = frames.get_depth_frame()
         if not depth: continue
```

## Comparing `pyrealsense2-2.55.1.6481.dist-info/METADATA` & `pyrealsense2-2.9.1.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.0
 Name: pyrealsense2
-Version: 2.55.1.6481
+Version: 2.9.1
 Summary: Python Wrapper for Intel Realsense SDK 2.0.
 Home-page: https://github.com/IntelRealSense/librealsense
 Author: Intel(R) RealSense(TM)
 Author-email: realsense@intel.com
 License: Apache License, Version 2.0
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-License-File: LICENSE
 
 Python Wrapper for Intel RealSense SDK 2.0
 ==========================================
 
 The python wrapper for Intel RealSense SDK 2.0 provides the C++ to Python binding required to access the SDK.
 
 Quick start
@@ -46,7 +47,9 @@
   try:
     for i in range(0, 100):
       frames = pipe.wait_for_frames()
       for f in frames:
         print(f.profile)
   finally:
       pipe.stop()
+
+
```

