# Comparing `tmp/napari_findaureus-0.0.1.tar.gz` & `tmp/napari_findaureus-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_findaureus-0.0.1.tar", last modified: Sat Apr 20 09:16:14 2024, max compression
+gzip compressed data, was "napari_findaureus-0.0.2.tar", last modified: Sat Apr 20 09:50:33 2024, max compression
```

## Comparing `napari_findaureus-0.0.1.tar` & `napari_findaureus-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:16:14.573939 napari_findaureus-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-20 09:16:01.000000 napari_findaureus-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-20 09:16:01.000000 napari_findaureus-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-20 09:16:14.573939 napari_findaureus-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-20 09:16:01.000000 napari_findaureus-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-20 09:16:01.000000 napari_findaureus-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-20 09:16:14.573939 napari_findaureus-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:16:14.569939 napari_findaureus-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:16:14.569939 napari_findaureus-0.0.1/src/findaureus/
--rw-r--r--   0 runner    (1001) docker     (127)    19555 2024-04-20 09:16:01.000000 napari_findaureus-0.0.1/src/findaureus/Module_Class.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-20 09:16:01.000000 napari_findaureus-0.0.1/src/findaureus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-20 09:16:01.000000 napari_findaureus-0.0.1/src/findaureus/_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-20 09:16:01.000000 napari_findaureus-0.0.1/src/findaureus/_sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:16:14.569939 napari_findaureus-0.0.1/src/findaureus/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 09:16:01.000000 napari_findaureus-0.0.1/src/findaureus/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-20 09:16:01.000000 napari_findaureus-0.0.1/src/findaureus/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-20 09:16:01.000000 napari_findaureus-0.0.1/src/findaureus/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-20 09:16:01.000000 napari_findaureus-0.0.1/src/findaureus/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-20 09:16:01.000000 napari_findaureus-0.0.1/src/findaureus/_tests/test_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10645 2024-04-20 09:16:01.000000 napari_findaureus-0.0.1/src/findaureus/_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-20 09:16:01.000000 napari_findaureus-0.0.1/src/findaureus/_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-20 09:16:01.000000 napari_findaureus-0.0.1/src/findaureus/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:16:14.573939 napari_findaureus-0.0.1/src/napari_findaureus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-20 09:16:14.000000 napari_findaureus-0.0.1/src/napari_findaureus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-20 09:16:14.000000 napari_findaureus-0.0.1/src/napari_findaureus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 09:16:14.000000 napari_findaureus-0.0.1/src/napari_findaureus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-20 09:16:14.000000 napari_findaureus-0.0.1/src/napari_findaureus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 09:16:14.000000 napari_findaureus-0.0.1/src/napari_findaureus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 09:16:14.000000 napari_findaureus-0.0.1/src/napari_findaureus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:50:33.184801 napari_findaureus-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-20 09:50:21.000000 napari_findaureus-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-20 09:50:21.000000 napari_findaureus-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-04-20 09:50:33.184801 napari_findaureus-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-20 09:50:21.000000 napari_findaureus-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-20 09:50:22.000000 napari_findaureus-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-20 09:50:33.184801 napari_findaureus-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:50:33.180801 napari_findaureus-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:50:33.180801 napari_findaureus-0.0.2/src/findaureus/
+-rw-r--r--   0 runner    (1001) docker     (127)    19555 2024-04-20 09:50:22.000000 napari_findaureus-0.0.2/src/findaureus/Module_Class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-20 09:50:22.000000 napari_findaureus-0.0.2/src/findaureus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-20 09:50:22.000000 napari_findaureus-0.0.2/src/findaureus/_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-20 09:50:22.000000 napari_findaureus-0.0.2/src/findaureus/_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:50:33.184801 napari_findaureus-0.0.2/src/findaureus/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 09:50:22.000000 napari_findaureus-0.0.2/src/findaureus/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-20 09:50:22.000000 napari_findaureus-0.0.2/src/findaureus/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-20 09:50:22.000000 napari_findaureus-0.0.2/src/findaureus/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-20 09:50:22.000000 napari_findaureus-0.0.2/src/findaureus/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-20 09:50:22.000000 napari_findaureus-0.0.2/src/findaureus/_tests/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10645 2024-04-20 09:50:22.000000 napari_findaureus-0.0.2/src/findaureus/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-20 09:50:22.000000 napari_findaureus-0.0.2/src/findaureus/_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-20 09:50:22.000000 napari_findaureus-0.0.2/src/findaureus/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:50:33.184801 napari_findaureus-0.0.2/src/napari_findaureus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-04-20 09:50:33.000000 napari_findaureus-0.0.2/src/napari_findaureus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-20 09:50:33.000000 napari_findaureus-0.0.2/src/napari_findaureus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 09:50:33.000000 napari_findaureus-0.0.2/src/napari_findaureus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-20 09:50:33.000000 napari_findaureus-0.0.2/src/napari_findaureus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 09:50:33.000000 napari_findaureus-0.0.2/src/napari_findaureus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 09:50:33.000000 napari_findaureus-0.0.2/src/napari_findaureus.egg-info/top_level.txt
```

### Comparing `napari_findaureus-0.0.1/LICENSE` & `napari_findaureus-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_findaureus-0.0.1/PKG-INFO` & `napari_findaureus-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-findaureus
-Version: 0.0.1
+Version: 0.0.2
 Summary: Locate bacteria in CLSM obtained infected bone tissue images
 Author: Shibarjun Mandal
 Author-email: shibarjunmandal@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
@@ -43,15 +43,15 @@
 Requires-Dist: napari; extra == "testing"
 Requires-Dist: pyqt5; extra == "testing"
 
 # napari-findaureus
 
 "Findaureus" is now available to use in napari.
 <p align="center">
-<img src = https://github.com/shibarjun/napari-findaureus/blob/main/docs/napari-findaureus.png />
+<img src = "https://github.com/shibarjun/napari-findaureus/blob/main/docs/napari-findaureus.png" />
 </p>
 
 Findaureus is a tool designed to identify bacteria in infected bone tissue images obtained via Confocal Laser Scanning Microscopy (CLSM). This tool can be accessed independently [here](https://github.com/shibarjun/Findaureus). Findaureus has been integrated as a plugin for napari. In addition to its bacteria-locating algorithm, the napari viewer provides improved visualization features, in 2D and 3D perspectives.
 
 ----------------------------------
 ## Installation
 ### Windows/Linux
@@ -89,15 +89,15 @@
 3. Navigate to the “Plugins” menu and select the `napari-findaureus` option to activate the widget.
 4. In the viewer, identify the bacteria channel from the "layer list," which is specified in the image file name, and select it.
 5. Once the bacteria channel is selected, click on the `Find bacteria!` button.
 6. The widget will display the image-related data and bacteria count. If you need additional help, click on the `Instruction` button in the widget.
 7. Before you proceed to another image, reset the viewer by clicking on the `Reset` button provided in the widget.
 
 <p align="center">
-<img src = https://github.com/shibarjun/napari-findaureus/blob/main/docs/napari-findaureus.gif />
+<img src = "https://github.com/shibarjun/napari-findaureus/blob/main/docs/napari-findaureus.gif" />
 </p>
 
 Enjoy exploring the fascinating world of bacteria in mouse bone tissues!
 
 ----------------------------------
 ## Contributing
 We welcome and appreciate all contributions to the `napari-findaureus` project! Whether it's reporting bugs, suggesting new features, improving documentation, or writing code, your involvement is greatly valued.
```

### Comparing `napari_findaureus-0.0.1/README.md` & `napari_findaureus-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # napari-findaureus
 
 "Findaureus" is now available to use in napari.
 <p align="center">
-<img src = https://github.com/shibarjun/napari-findaureus/blob/main/docs/napari-findaureus.png />
+<img src = "https://github.com/shibarjun/napari-findaureus/blob/main/docs/napari-findaureus.png" />
 </p>
 
 Findaureus is a tool designed to identify bacteria in infected bone tissue images obtained via Confocal Laser Scanning Microscopy (CLSM). This tool can be accessed independently [here](https://github.com/shibarjun/Findaureus). Findaureus has been integrated as a plugin for napari. In addition to its bacteria-locating algorithm, the napari viewer provides improved visualization features, in 2D and 3D perspectives.
 
 ----------------------------------
 ## Installation
 ### Windows/Linux
@@ -44,15 +44,15 @@
 3. Navigate to the “Plugins” menu and select the `napari-findaureus` option to activate the widget.
 4. In the viewer, identify the bacteria channel from the "layer list," which is specified in the image file name, and select it.
 5. Once the bacteria channel is selected, click on the `Find bacteria!` button.
 6. The widget will display the image-related data and bacteria count. If you need additional help, click on the `Instruction` button in the widget.
 7. Before you proceed to another image, reset the viewer by clicking on the `Reset` button provided in the widget.
 
 <p align="center">
-<img src = https://github.com/shibarjun/napari-findaureus/blob/main/docs/napari-findaureus.gif />
+<img src = "https://github.com/shibarjun/napari-findaureus/blob/main/docs/napari-findaureus.gif" />
 </p>
 
 Enjoy exploring the fascinating world of bacteria in mouse bone tissues!
 
 ----------------------------------
 ## Contributing
 We welcome and appreciate all contributions to the `napari-findaureus` project! Whether it's reporting bugs, suggesting new features, improving documentation, or writing code, your involvement is greatly valued.
```

### Comparing `napari_findaureus-0.0.1/pyproject.toml` & `napari_findaureus-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari_findaureus-0.0.1/setup.cfg` & `napari_findaureus-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari_findaureus-0.0.1/src/findaureus/Module_Class.py` & `napari_findaureus-0.0.2/src/findaureus/Module_Class.py`

 * *Files identical despite different names*

### Comparing `napari_findaureus-0.0.1/src/findaureus/_reader.py` & `napari_findaureus-0.0.2/src/findaureus/_reader.py`

 * *Files identical despite different names*

### Comparing `napari_findaureus-0.0.1/src/findaureus/_sample_data.py` & `napari_findaureus-0.0.2/src/findaureus/_sample_data.py`

 * *Files identical despite different names*

### Comparing `napari_findaureus-0.0.1/src/findaureus/_tests/test_reader.py` & `napari_findaureus-0.0.2/src/findaureus/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari_findaureus-0.0.1/src/findaureus/_tests/test_widget.py` & `napari_findaureus-0.0.2/src/findaureus/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_findaureus-0.0.1/src/findaureus/_widget.py` & `napari_findaureus-0.0.2/src/findaureus/_widget.py`

 * *Files identical despite different names*

### Comparing `napari_findaureus-0.0.1/src/findaureus/_writer.py` & `napari_findaureus-0.0.2/src/findaureus/_writer.py`

 * *Files identical despite different names*

### Comparing `napari_findaureus-0.0.1/src/findaureus/napari.yaml` & `napari_findaureus-0.0.2/src/findaureus/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_findaureus-0.0.1/src/napari_findaureus.egg-info/PKG-INFO` & `napari_findaureus-0.0.2/src/napari_findaureus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-findaureus
-Version: 0.0.1
+Version: 0.0.2
 Summary: Locate bacteria in CLSM obtained infected bone tissue images
 Author: Shibarjun Mandal
 Author-email: shibarjunmandal@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
@@ -43,15 +43,15 @@
 Requires-Dist: napari; extra == "testing"
 Requires-Dist: pyqt5; extra == "testing"
 
 # napari-findaureus
 
 "Findaureus" is now available to use in napari.
 <p align="center">
-<img src = https://github.com/shibarjun/napari-findaureus/blob/main/docs/napari-findaureus.png />
+<img src = "https://github.com/shibarjun/napari-findaureus/blob/main/docs/napari-findaureus.png" />
 </p>
 
 Findaureus is a tool designed to identify bacteria in infected bone tissue images obtained via Confocal Laser Scanning Microscopy (CLSM). This tool can be accessed independently [here](https://github.com/shibarjun/Findaureus). Findaureus has been integrated as a plugin for napari. In addition to its bacteria-locating algorithm, the napari viewer provides improved visualization features, in 2D and 3D perspectives.
 
 ----------------------------------
 ## Installation
 ### Windows/Linux
@@ -89,15 +89,15 @@
 3. Navigate to the “Plugins” menu and select the `napari-findaureus` option to activate the widget.
 4. In the viewer, identify the bacteria channel from the "layer list," which is specified in the image file name, and select it.
 5. Once the bacteria channel is selected, click on the `Find bacteria!` button.
 6. The widget will display the image-related data and bacteria count. If you need additional help, click on the `Instruction` button in the widget.
 7. Before you proceed to another image, reset the viewer by clicking on the `Reset` button provided in the widget.
 
 <p align="center">
-<img src = https://github.com/shibarjun/napari-findaureus/blob/main/docs/napari-findaureus.gif />
+<img src = "https://github.com/shibarjun/napari-findaureus/blob/main/docs/napari-findaureus.gif" />
 </p>
 
 Enjoy exploring the fascinating world of bacteria in mouse bone tissues!
 
 ----------------------------------
 ## Contributing
 We welcome and appreciate all contributions to the `napari-findaureus` project! Whether it's reporting bugs, suggesting new features, improving documentation, or writing code, your involvement is greatly valued.
```

### Comparing `napari_findaureus-0.0.1/src/napari_findaureus.egg-info/SOURCES.txt` & `napari_findaureus-0.0.2/src/napari_findaureus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

