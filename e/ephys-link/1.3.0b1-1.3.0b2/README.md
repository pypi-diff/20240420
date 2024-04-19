# Comparing `tmp/ephys_link-1.3.0b1.tar.gz` & `tmp/ephys_link-1.3.0b2.tar.gz`

## Comparing `ephys_link-1.3.0b1.tar` & `ephys_link-1.3.0b2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/ephys_link.spec
--rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/assets/icon.ico
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/scripts/__init__.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/scripts/move_tester.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/__init__.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/__main__.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/common.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/emergency_stop.py
--rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/gui.py
--rw-r--r--   0        0        0    19432 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/platform_handler.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/platform_manipulator.py
--rw-r--r--   0        0        0    16641 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/server.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/platforms/__init__.py
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/platforms/new_scale_handler.py
--rw-r--r--   0        0        0    11877 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/platforms/new_scale_manipulator.py
--rw-r--r--   0        0        0     7692 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/platforms/new_scale_pathfinder_handler.py
--rw-r--r--   0        0        0     5843 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/platforms/sensapex_handler.py
--rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/platforms/sensapex_manipulator.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/platforms/ump3_handler.py
--rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/platforms/ump3_manipulator.py
--rw-r--r--   0        0        0   810232 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/resources/CP210xManufacturing.dll
--rw-r--r--   0        0        0   155136 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/resources/NstMotorCtrl.dll
--rw-r--r--   0        0        0   469752 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/resources/SiUSBXp.dll
--rw-r--r--   0        0        0   316316 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/src/ephys_link/resources/libum.dll
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/tests/__init__.py
--rw-r--r--   0        0        0     6484 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/LICENSE
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/README.md
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/pyproject.toml
--rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 ephys_link-1.3.0b1/PKG-INFO
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/ephys_link.spec
+-rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/assets/icon.ico
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/scripts/__init__.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/scripts/move_tester.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/src/ephys_link/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/src/ephys_link/__init__.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/src/ephys_link/__main__.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/src/ephys_link/common.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/src/ephys_link/emergency_stop.py
+-rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/src/ephys_link/gui.py
+-rw-r--r--   0        0        0    19432 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/src/ephys_link/platform_handler.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/src/ephys_link/platform_manipulator.py
+-rw-r--r--   0        0        0    16641 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/src/ephys_link/server.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/src/ephys_link/platforms/__init__.py
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/src/ephys_link/platforms/new_scale_handler.py
+-rw-r--r--   0        0        0    11877 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/src/ephys_link/platforms/new_scale_manipulator.py
+-rw-r--r--   0        0        0     7692 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/src/ephys_link/platforms/new_scale_pathfinder_handler.py
+-rw-r--r--   0        0        0     5843 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/src/ephys_link/platforms/sensapex_handler.py
+-rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/src/ephys_link/platforms/sensapex_manipulator.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/src/ephys_link/platforms/ump3_handler.py
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/src/ephys_link/platforms/ump3_manipulator.py
+-rw-r--r--   0        0        0   810232 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/src/ephys_link/resources/CP210xManufacturing.dll
+-rw-r--r--   0        0        0   155136 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/src/ephys_link/resources/NstMotorCtrl.dll
+-rw-r--r--   0        0        0   469752 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/src/ephys_link/resources/SiUSBXp.dll
+-rw-r--r--   0        0        0   316316 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/src/ephys_link/resources/libum.dll
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/tests/__init__.py
+-rw-r--r--   0        0        0     6484 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/LICENSE
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/README.md
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/pyproject.toml
+-rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 ephys_link-1.3.0b2/PKG-INFO
```

### Comparing `ephys_link-1.3.0b1/ephys_link.spec` & `ephys_link-1.3.0b2/ephys_link.spec`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/assets/icon.ico` & `ephys_link-1.3.0b2/assets/icon.ico`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/scripts/move_tester.py` & `ephys_link-1.3.0b2/scripts/move_tester.py`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/src/ephys_link/__main__.py` & `ephys_link-1.3.0b2/src/ephys_link/__main__.py`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/src/ephys_link/common.py` & `ephys_link-1.3.0b2/src/ephys_link/common.py`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/src/ephys_link/emergency_stop.py` & `ephys_link-1.3.0b2/src/ephys_link/emergency_stop.py`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/src/ephys_link/gui.py` & `ephys_link-1.3.0b2/src/ephys_link/gui.py`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/src/ephys_link/platform_handler.py` & `ephys_link-1.3.0b2/src/ephys_link/platform_handler.py`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/src/ephys_link/platform_manipulator.py` & `ephys_link-1.3.0b2/src/ephys_link/platform_manipulator.py`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/src/ephys_link/server.py` & `ephys_link-1.3.0b2/src/ephys_link/server.py`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/src/ephys_link/platforms/new_scale_handler.py` & `ephys_link-1.3.0b2/src/ephys_link/platforms/new_scale_handler.py`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/src/ephys_link/platforms/new_scale_manipulator.py` & `ephys_link-1.3.0b2/src/ephys_link/platforms/new_scale_manipulator.py`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/src/ephys_link/platforms/new_scale_pathfinder_handler.py` & `ephys_link-1.3.0b2/src/ephys_link/platforms/new_scale_pathfinder_handler.py`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/src/ephys_link/platforms/sensapex_handler.py` & `ephys_link-1.3.0b2/src/ephys_link/platforms/sensapex_handler.py`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/src/ephys_link/platforms/sensapex_manipulator.py` & `ephys_link-1.3.0b2/src/ephys_link/platforms/sensapex_manipulator.py`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/src/ephys_link/platforms/ump3_handler.py` & `ephys_link-1.3.0b2/src/ephys_link/platforms/ump3_handler.py`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/src/ephys_link/platforms/ump3_manipulator.py` & `ephys_link-1.3.0b2/src/ephys_link/platforms/ump3_manipulator.py`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/src/ephys_link/resources/CP210xManufacturing.dll` & `ephys_link-1.3.0b2/src/ephys_link/resources/CP210xManufacturing.dll`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/src/ephys_link/resources/NstMotorCtrl.dll` & `ephys_link-1.3.0b2/src/ephys_link/resources/NstMotorCtrl.dll`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/src/ephys_link/resources/SiUSBXp.dll` & `ephys_link-1.3.0b2/src/ephys_link/resources/SiUSBXp.dll`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/src/ephys_link/resources/libum.dll` & `ephys_link-1.3.0b2/src/ephys_link/resources/libum.dll`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/.gitignore` & `ephys_link-1.3.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/LICENSE` & `ephys_link-1.3.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/README.md` & `ephys_link-1.3.0b2/README.md`

 * *Files identical despite different names*

### Comparing `ephys_link-1.3.0b1/pyproject.toml` & `ephys_link-1.3.0b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "Operating System :: Microsoft :: Windows",
     "Intended Audience :: End Users/Desktop",
     "Intended Audience :: Healthcare Industry",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Medical Science Apps.",
 ]
 dependencies = [
-    "aiohttp==3.9.3",
+    "aiohttp==3.9.4",
     "platformdirs==4.2.0",
     "pyserial==3.5",
     "python-socketio==5.11.2",
     "pythonnet==3.0.3",
     "requests==2.31.0",
     "sensapex==1.400.0",
     "vbl-aquarium==0.0.12"
@@ -57,15 +57,15 @@
 exclude = ["/.github", "/.idea"]
 
 [tool.hatch.envs.default]
 python = "3.12"
 dependencies = [
     "coverage[toml]>=6.5",
     "pytest",
-    "python-socketio[client]==5.11.1",
+    "python-socketio[client]==5.11.2",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
     "- coverage combine",
     "coverage report",
```

### Comparing `ephys_link-1.3.0b1/PKG-INFO` & `ephys_link-1.3.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ephys-link
-Version: 1.3.0b1
+Version: 1.3.0b2
 Summary: A Python Socket.IO server that allows any Socket.IO-compliant application to communicate with manipulators used in electrophysiology experiments.
 Project-URL: Documentation, https://virtualbrainlab.org/ephys_link/installation_and_use.html
 Project-URL: Issues, https://github.com/VirtualBrainLab/ephys-link/issues
 Project-URL: Source, https://github.com/VirtualBrainLab/ephys-link
 Author-email: Kenneth Yang <kjy5@uw.edu>
 Maintainer-email: Kenneth Yang <kjy5@uw.edu>
 License-Expression: GPL-3.0-only
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: <3.13,>=3.8
-Requires-Dist: aiohttp==3.9.3
+Requires-Dist: aiohttp==3.9.4
 Requires-Dist: platformdirs==4.2.0
 Requires-Dist: pyserial==3.5
 Requires-Dist: python-socketio==5.11.2
 Requires-Dist: pythonnet==3.0.3
 Requires-Dist: requests==2.31.0
 Requires-Dist: sensapex==1.400.0
 Requires-Dist: vbl-aquarium==0.0.12
```

