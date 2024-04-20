# Comparing `tmp/pyfastboot-1.3.8.tar.gz` & `tmp/pyfastboot-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfastboot-1.3.8.tar", last modified: Tue Mar 19 15:04:33 2024, max compression
+gzip compressed data, was "pyfastboot-1.3.9.tar", last modified: Tue Mar 26 03:06:11 2024, max compression
```

## Comparing `pyfastboot-1.3.8.tar` & `pyfastboot-1.3.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 15:04:33.024874 pyfastboot-1.3.8/
--rw-rw-rw-   0        0        0    10351 2024-02-27 10:30:38.000000 pyfastboot-1.3.8/LICENSE
--rw-rw-rw-   0        0        0     4642 2024-03-19 15:04:33.023704 pyfastboot-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     3806 2024-03-19 15:04:17.000000 pyfastboot-1.3.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-19 15:04:33.015976 pyfastboot-1.3.8/pyfastboot/
--rw-rw-rw-   0        0        0        0 2024-02-27 10:30:38.000000 pyfastboot-1.3.8/pyfastboot/__init__.py
--rw-rw-rw-   0        0        0    12910 2024-02-27 10:30:38.000000 pyfastboot-1.3.8/pyfastboot/common.py
--rw-rw-rw-   0        0        0     6050 2024-03-16 01:09:09.000000 pyfastboot-1.3.8/pyfastboot/common_cli.py
--rw-rw-rw-   0        0        0    40811 2024-03-19 15:02:49.000000 pyfastboot-1.3.8/pyfastboot/fastboot.py
--rw-rw-rw-   0        0        0     4070 2024-03-16 01:09:19.000000 pyfastboot-1.3.8/pyfastboot/fastboot_debug.py
--rw-rw-rw-   0        0        0     7099 2024-03-17 04:10:56.000000 pyfastboot-1.3.8/pyfastboot/fastboot_extras.py
--rw-rw-rw-   0        0        0     2478 2024-02-27 10:30:38.000000 pyfastboot-1.3.8/pyfastboot/usb_exceptions.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:04:33.022702 pyfastboot-1.3.8/pyfastboot.egg-info/
--rw-rw-rw-   0        0        0     4642 2024-03-19 15:04:32.000000 pyfastboot-1.3.8/pyfastboot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2024-03-19 15:04:33.000000 pyfastboot-1.3.8/pyfastboot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 15:04:32.000000 pyfastboot-1.3.8/pyfastboot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 15:04:32.000000 pyfastboot-1.3.8/pyfastboot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      656 2024-03-19 15:04:23.000000 pyfastboot-1.3.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-19 15:04:33.024874 pyfastboot-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0     2310 2024-03-19 14:42:54.000000 pyfastboot-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-26 03:06:11.071051 pyfastboot-1.3.9/
+-rw-rw-rw-   0        0        0    10351 2024-02-27 10:30:38.000000 pyfastboot-1.3.9/LICENSE
+-rw-rw-rw-   0        0        0     4756 2024-03-26 03:06:11.069874 pyfastboot-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3855 2024-03-26 03:06:03.000000 pyfastboot-1.3.9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-26 03:06:11.064227 pyfastboot-1.3.9/pyfastboot/
+-rw-rw-rw-   0        0        0        0 2024-02-27 10:30:38.000000 pyfastboot-1.3.9/pyfastboot/__init__.py
+-rw-rw-rw-   0        0        0    12917 2024-03-26 03:03:25.000000 pyfastboot-1.3.9/pyfastboot/common.py
+-rw-rw-rw-   0        0        0     6050 2024-03-16 01:09:09.000000 pyfastboot-1.3.9/pyfastboot/common_cli.py
+-rw-rw-rw-   0        0        0    40811 2024-03-19 15:02:49.000000 pyfastboot-1.3.9/pyfastboot/fastboot.py
+-rw-rw-rw-   0        0        0     4070 2024-03-16 01:09:19.000000 pyfastboot-1.3.9/pyfastboot/fastboot_debug.py
+-rw-rw-rw-   0        0        0     7099 2024-03-17 04:10:56.000000 pyfastboot-1.3.9/pyfastboot/fastboot_extras.py
+-rw-rw-rw-   0        0        0     2478 2024-02-27 10:30:38.000000 pyfastboot-1.3.9/pyfastboot/usb_exceptions.py
+drwxrwxrwx   0        0        0        0 2024-03-26 03:06:11.068824 pyfastboot-1.3.9/pyfastboot.egg-info/
+-rw-rw-rw-   0        0        0     4756 2024-03-26 03:06:11.000000 pyfastboot-1.3.9/pyfastboot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2024-03-26 03:06:11.000000 pyfastboot-1.3.9/pyfastboot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-26 03:06:11.000000 pyfastboot-1.3.9/pyfastboot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-03-26 03:06:11.000000 pyfastboot-1.3.9/pyfastboot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-26 03:06:11.000000 pyfastboot-1.3.9/pyfastboot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      711 2024-03-26 03:05:25.000000 pyfastboot-1.3.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-26 03:06:11.071051 pyfastboot-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     2310 2024-03-26 03:03:45.000000 pyfastboot-1.3.9/setup.py
```

### Comparing `pyfastboot-1.3.8/LICENSE` & `pyfastboot-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfastboot-1.3.8/PKG-INFO` & `pyfastboot-1.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfastboot
-Version: 1.3.8
+Version: 1.3.9
 Summary: A pure python implementation of the Android Fastboot protocols
 Home-page: https://github.com/HikariCalyx/python-fastboot
 Author: Hikari Calyx
 Author-email: Hikari Calyx <hikaricalyx@hikaricalyx.com>
 Maintainer: Hikari Calyx
 Maintainer-email: hikaricalyx@hikaricalyx.com
 Project-URL: Homepage, https://github.com/HikariCalyx/python-fastboot
@@ -13,14 +13,16 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: libusb1>=1.0.16
+Requires-Dist: progressbar>=2.3
 
 pyfastboot
 ==========
 
 This is a modified version for specific project usage - for example, service permission granting program for all Nokia phones.
 
 For ADB implementation, see [adb_shell](https://github.com/JeffLIrion/adb_shell).
@@ -126,14 +128,18 @@
   * libusb1 (1.0.16+)
   * python-libusb1 (1.2.0+)
   * `fastboot.zip` (optional):
     * python-progressbar (2.3+)
 
 ### History
 
+#### 1.3.9
+
+* Fixed the dependencies issue.
+
 #### 1.3.8
 
 * Added support for Unisoc "flashing unlock_bootloader" function (UnisocUnlockBootloader())
 * Added support for vbmeta processing
 * Fixed issue of GetIdentifierToken function
 
 #### 1.3.6
```

### Comparing `pyfastboot-1.3.8/README.md` & `pyfastboot-1.3.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -106,14 +106,18 @@
   * libusb1 (1.0.16+)
   * python-libusb1 (1.2.0+)
   * `fastboot.zip` (optional):
     * python-progressbar (2.3+)
 
 ### History
 
+#### 1.3.9
+
+* Fixed the dependencies issue.
+
 #### 1.3.8
 
 * Added support for Unisoc "flashing unlock_bootloader" function (UnisocUnlockBootloader())
 * Added support for vbmeta processing
 * Fixed issue of GetIdentifierToken function
 
 #### 1.3.6
```

### Comparing `pyfastboot-1.3.8/pyfastboot/common.py` & `pyfastboot-1.3.9/pyfastboot/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import threading
 import weakref
 import select
 
 import libusb1
 import usb1
 
-from adb import usb_exceptions
+from pyfastboot import usb_exceptions
 
 DEFAULT_TIMEOUT_MS = 10000
 
 _LOG = logging.getLogger('android_usb')
 
 
 def GetInterface(setting):
```

### Comparing `pyfastboot-1.3.8/pyfastboot/common_cli.py` & `pyfastboot-1.3.9/pyfastboot/common_cli.py`

 * *Files identical despite different names*

### Comparing `pyfastboot-1.3.8/pyfastboot/fastboot.py` & `pyfastboot-1.3.9/pyfastboot/fastboot.py`

 * *Files identical despite different names*

### Comparing `pyfastboot-1.3.8/pyfastboot/fastboot_debug.py` & `pyfastboot-1.3.9/pyfastboot/fastboot_debug.py`

 * *Files identical despite different names*

### Comparing `pyfastboot-1.3.8/pyfastboot/fastboot_extras.py` & `pyfastboot-1.3.9/pyfastboot/fastboot_extras.py`

 * *Files identical despite different names*

### Comparing `pyfastboot-1.3.8/pyfastboot/usb_exceptions.py` & `pyfastboot-1.3.9/pyfastboot/usb_exceptions.py`

 * *Files identical despite different names*

### Comparing `pyfastboot-1.3.8/pyfastboot.egg-info/PKG-INFO` & `pyfastboot-1.3.9/pyfastboot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfastboot
-Version: 1.3.8
+Version: 1.3.9
 Summary: A pure python implementation of the Android Fastboot protocols
 Home-page: https://github.com/HikariCalyx/python-fastboot
 Author: Hikari Calyx
 Author-email: Hikari Calyx <hikaricalyx@hikaricalyx.com>
 Maintainer: Hikari Calyx
 Maintainer-email: hikaricalyx@hikaricalyx.com
 Project-URL: Homepage, https://github.com/HikariCalyx/python-fastboot
@@ -13,14 +13,16 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: libusb1>=1.0.16
+Requires-Dist: progressbar>=2.3
 
 pyfastboot
 ==========
 
 This is a modified version for specific project usage - for example, service permission granting program for all Nokia phones.
 
 For ADB implementation, see [adb_shell](https://github.com/JeffLIrion/adb_shell).
@@ -126,14 +128,18 @@
   * libusb1 (1.0.16+)
   * python-libusb1 (1.2.0+)
   * `fastboot.zip` (optional):
     * python-progressbar (2.3+)
 
 ### History
 
+#### 1.3.9
+
+* Fixed the dependencies issue.
+
 #### 1.3.8
 
 * Added support for Unisoc "flashing unlock_bootloader" function (UnisocUnlockBootloader())
 * Added support for vbmeta processing
 * Fixed issue of GetIdentifierToken function
 
 #### 1.3.6
```

### Comparing `pyfastboot-1.3.8/setup.py` & `pyfastboot-1.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from setuptools import setup
 
 
 setup(
     name = 'pyfastboot',
     packages = ['pyfastboot'],
-    version = '1.3.7',
+    version = '1.3.9',
     author = 'Hikari Calyx',
     author_email = 'hikaricalyx@hikaricalyx.com',
     maintainer = 'Hikari Calyx',
     maintainer_email = 'hikaricalyx@hikaricalyx.com',
     url = 'https://github.com/HikariCalyx/python-fastboot',
     description = 'A pure python implementation of the Android Fastboot protocols',
     long_description = '''
```

