# Comparing `tmp/pan_ztp_patcher-0.2.7.tar.gz` & `tmp/pan_ztp_patcher-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pan_ztp_patcher-0.2.7.tar", max compression
+gzip compressed data, was "pan_ztp_patcher-0.2.8.tar", max compression
```

## Comparing `pan_ztp_patcher-0.2.7.tar` & `pan_ztp_patcher-0.2.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2024-04-19 23:37:12.329777 pan_ztp_patcher-0.2.7/LICENSE
--rw-r--r--   0        0        0     3524 2024-04-19 23:37:12.329777 pan_ztp_patcher-0.2.7/README.md
--rw-r--r--   0        0        0        0 2024-04-19 23:37:12.329777 pan_ztp_patcher-0.2.7/pan_ztp_patcher/__init__.py
--rw-r--r--   0        0        0    13855 2024-04-19 23:37:12.329777 pan_ztp_patcher-0.2.7/pan_ztp_patcher/app.py
--rw-r--r--   0        0        0     1026 2024-04-19 23:37:12.329777 pan_ztp_patcher-0.2.7/pan_ztp_patcher/utils.py
--rw-r--r--   0        0        0    37511 2024-04-19 23:37:12.329777 pan_ztp_patcher-0.2.7/pan_ztp_patcher/ztp_patcher.py
--rw-r--r--   0        0        0      597 2024-04-19 23:37:12.329777 pan_ztp_patcher-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     4164 1970-01-01 00:00:00.000000 pan_ztp_patcher-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-19 23:42:26.745535 pan_ztp_patcher-0.2.8/LICENSE
+-rw-r--r--   0        0        0     3524 2024-04-19 23:42:26.745535 pan_ztp_patcher-0.2.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 23:42:26.745535 pan_ztp_patcher-0.2.8/pan_ztp_patcher/__init__.py
+-rw-r--r--   0        0        0    13855 2024-04-19 23:42:26.745535 pan_ztp_patcher-0.2.8/pan_ztp_patcher/app.py
+-rw-r--r--   0        0        0     1026 2024-04-19 23:42:26.745535 pan_ztp_patcher-0.2.8/pan_ztp_patcher/utils.py
+-rw-r--r--   0        0        0    37511 2024-04-19 23:42:26.745535 pan_ztp_patcher-0.2.8/pan_ztp_patcher/ztp_patcher.py
+-rw-r--r--   0        0        0      597 2024-04-19 23:42:26.745535 pan_ztp_patcher-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     4164 1970-01-01 00:00:00.000000 pan_ztp_patcher-0.2.8/PKG-INFO
```

### Comparing `pan_ztp_patcher-0.2.7/LICENSE` & `pan_ztp_patcher-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pan_ztp_patcher-0.2.7/README.md` & `pan_ztp_patcher-0.2.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 - Configured network settings on the Raspberry Pi's Ethernet interface to 192.168.1.2/24.
 
 ## Installation
 
 Install the PAN-OS ZTP Patcher via pip:
 
 ```bash
-pip install pan_ztp_patcher
+pip install pan-ztp-patcher
 ```
 
 ## Usage
 
 Run the ZTP Patcher with the following command structure, providing the necessary parameters:
 
 ### Parameters
```

### Comparing `pan_ztp_patcher-0.2.7/pan_ztp_patcher/app.py` & `pan_ztp_patcher-0.2.8/pan_ztp_patcher/app.py`

 * *Files identical despite different names*

### Comparing `pan_ztp_patcher-0.2.7/pan_ztp_patcher/utils.py` & `pan_ztp_patcher-0.2.8/pan_ztp_patcher/utils.py`

 * *Files identical despite different names*

### Comparing `pan_ztp_patcher-0.2.7/pan_ztp_patcher/ztp_patcher.py` & `pan_ztp_patcher-0.2.8/pan_ztp_patcher/ztp_patcher.py`

 * *Files identical despite different names*

### Comparing `pan_ztp_patcher-0.2.7/pyproject.toml` & `pan_ztp_patcher-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pan-ztp-patcher"
-version = "0.2.7"
+version = "0.2.8"
 description = "Update content version on PAN-OS firewalls"
 authors = ["Calvin Remsburg <cremsburg.dev@gmail.com>"]
 license = "Apache2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 ztp_patcher = "pan_ztp_patcher.app:main"
```

### Comparing `pan_ztp_patcher-0.2.7/PKG-INFO` & `pan_ztp_patcher-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pan-ztp-patcher
-Version: 0.2.7
+Version: 0.2.8
 Summary: Update content version on PAN-OS firewalls
 License: Apache2.0
 Author: Calvin Remsburg
 Author-email: cremsburg.dev@gmail.com
 Requires-Python: >=3.8.1
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -38,15 +38,15 @@
 - Configured network settings on the Raspberry Pi's Ethernet interface to 192.168.1.2/24.
 
 ## Installation
 
 Install the PAN-OS ZTP Patcher via pip:
 
 ```bash
-pip install pan_ztp_patcher
+pip install pan-ztp-patcher
 ```
 
 ## Usage
 
 Run the ZTP Patcher with the following command structure, providing the necessary parameters:
 
 ### Parameters
```

