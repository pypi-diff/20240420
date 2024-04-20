# Comparing `tmp/ziptimezone-0.10.2.tar.gz` & `tmp/ziptimezone-0.10.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziptimezone-0.10.2.tar", max compression
+gzip compressed data, was "ziptimezone-0.10.3.tar", max compression
```

## Comparing `ziptimezone-0.10.2.tar` & `ziptimezone-0.10.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-0.10.2/LICENSE
--rw-r--r--   0        0        0      529 2024-04-20 11:56:28.072753 ziptimezone-0.10.2/pyproject.toml
--rw-r--r--   0        0        0      320 2024-04-20 11:29:25.216037 ziptimezone-0.10.2/README.md
--rw-r--r--   0        0        0      994 2024-04-20 11:29:25.228270 ziptimezone-0.10.2/ziptimezone/__init__.py
--rw-r--r--   0        0        0     3128 2024-04-20 11:29:25.229297 ziptimezone-0.10.2/ziptimezone/core.py
--rw-r--r--   0        0        0     2762 2024-04-20 11:29:25.233383 ziptimezone-0.10.2/ziptimezone/data_manager.py
--rw-r--r--   0        0        0     1110 2024-04-20 11:52:46.868177 ziptimezone-0.10.2/ziptimezone/geocode.py
--rw-r--r--   0        0        0     1873 2024-04-20 11:29:25.238387 ziptimezone-0.10.2/ziptimezone/mappings.py
--rw-r--r--   0        0        0     1091 1970-01-01 00:00:00.000000 ziptimezone-0.10.2/PKG-INFO
+-rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-0.10.3/LICENSE
+-rw-r--r--   0        0        0      553 2024-04-20 12:20:27.045870 ziptimezone-0.10.3/pyproject.toml
+-rw-r--r--   0        0        0      320 2024-04-20 11:29:25.216037 ziptimezone-0.10.3/README.md
+-rw-r--r--   0        0        0      994 2024-04-20 11:29:25.228270 ziptimezone-0.10.3/ziptimezone/__init__.py
+-rw-r--r--   0        0        0     3128 2024-04-20 11:29:25.229297 ziptimezone-0.10.3/ziptimezone/core.py
+-rw-r--r--   0        0        0     2762 2024-04-20 11:29:25.233383 ziptimezone-0.10.3/ziptimezone/data_manager.py
+-rw-r--r--   0        0        0     1110 2024-04-20 11:52:46.868177 ziptimezone-0.10.3/ziptimezone/geocode.py
+-rw-r--r--   0        0        0     1873 2024-04-20 11:29:25.238387 ziptimezone-0.10.3/ziptimezone/mappings.py
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 ziptimezone-0.10.3/PKG-INFO
```

### Comparing `ziptimezone-0.10.2/pyproject.toml` & `ziptimezone-0.10.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "ziptimezone"
-version = "0.10.2"
+version = "0.10.3"
 description = "A package to convert ZIP codes to time zones and get geographic coordinates."
 readme = "README.md"
 authors = ["Manjunath Bettadapura <manjunathbettadapura412@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.8, <4.0"
 requests = "^2.31.0"
 #pgeocode = "^0.5.0"
-timezonefinder = "6.5.0"
-pandas = "^2.2.2"
+timezonefinder = ">=6.1.5, 6.5.0"
+pandas = ">=1.3.3, 2.5.0"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ziptimezone-0.10.2/ziptimezone/__init__.py` & `ziptimezone-0.10.3/ziptimezone/__init__.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.2/ziptimezone/core.py` & `ziptimezone-0.10.3/ziptimezone/core.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.2/ziptimezone/data_manager.py` & `ziptimezone-0.10.3/ziptimezone/data_manager.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.2/ziptimezone/geocode.py` & `ziptimezone-0.10.3/ziptimezone/geocode.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.2/ziptimezone/mappings.py` & `ziptimezone-0.10.3/ziptimezone/mappings.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.2/PKG-INFO` & `ziptimezone-0.10.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ziptimezone
-Version: 0.10.2
+Version: 0.10.3
 Summary: A package to convert ZIP codes to time zones and get geographic coordinates.
 License: MIT
 Author: Manjunath Bettadapura
 Author-email: manjunathbettadapura412@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: pandas (==2.5.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: timezonefinder (==6.5.0)
 Description-Content-Type: text/markdown
 
 #### This uses zip_code, latitude and longitude data from geonames and timezonefinder packages.
 #### Convenience functions to get:
 ##### 1. The latitude and longitude for a given US or Puerto Rico Zip Code
```

