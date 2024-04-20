# Comparing `tmp/ziptimezone-0.10.0.tar.gz` & `tmp/ziptimezone-0.10.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziptimezone-0.10.0.tar", max compression
+gzip compressed data, was "ziptimezone-0.10.1.tar", max compression
```

## Comparing `ziptimezone-0.10.0.tar` & `ziptimezone-0.10.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        1 2024-04-18 17:39:45.000000 ziptimezone-0.10.0/LICENSE
--rw-r--r--   0        0        0      298 2024-04-18 20:05:12.524095 ziptimezone-0.10.0/README.md
--rw-r--r--   0        0        0      489 2024-04-19 21:46:25.067269 ziptimezone-0.10.0/pyproject.toml
--rw-r--r--   0        0        0      969 2024-04-18 17:39:45.000000 ziptimezone-0.10.0/ziptimezone/__init__.py
--rw-r--r--   0        0        0     1365 2024-04-19 15:38:14.654911 ziptimezone-0.10.0/ziptimezone/core copy.py
--rw-r--r--   0        0        0     3056 2024-04-19 20:45:15.084480 ziptimezone-0.10.0/ziptimezone/core.py
--rw-r--r--   0        0        0        0 2024-04-19 15:41:48.857464 ziptimezone-0.10.0/ziptimezone/data/.gitkeep
--rw-r--r--   0        0        0     2697 2024-04-19 15:57:50.850984 ziptimezone-0.10.0/ziptimezone/data_manager.py
--rw-r--r--   0        0        0     1050 2024-04-18 19:09:15.017940 ziptimezone-0.10.0/ziptimezone/geocode.py
--rw-r--r--   0        0        0     1825 2024-04-18 17:39:45.000000 ziptimezone-0.10.0/ziptimezone/mappings.py
--rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 ziptimezone-0.10.0/PKG-INFO
+-rw-r--r--   0        0        0        1 2024-04-18 17:39:45.000000 ziptimezone-0.10.1/LICENSE
+-rw-r--r--   0        0        0      252 2024-04-19 21:47:29.146818 ziptimezone-0.10.1/README.md
+-rw-r--r--   0        0        0      489 2024-04-19 21:47:34.870778 ziptimezone-0.10.1/pyproject.toml
+-rw-r--r--   0        0        0      969 2024-04-18 17:39:45.000000 ziptimezone-0.10.1/ziptimezone/__init__.py
+-rw-r--r--   0        0        0     1365 2024-04-19 15:38:14.654911 ziptimezone-0.10.1/ziptimezone/core copy.py
+-rw-r--r--   0        0        0     3056 2024-04-19 20:45:15.084480 ziptimezone-0.10.1/ziptimezone/core.py
+-rw-r--r--   0        0        0        0 2024-04-19 15:41:48.857464 ziptimezone-0.10.1/ziptimezone/data/.gitkeep
+-rw-r--r--   0        0        0     2697 2024-04-19 15:57:50.850984 ziptimezone-0.10.1/ziptimezone/data_manager.py
+-rw-r--r--   0        0        0     1050 2024-04-18 19:09:15.017940 ziptimezone-0.10.1/ziptimezone/geocode.py
+-rw-r--r--   0        0        0     1825 2024-04-18 17:39:45.000000 ziptimezone-0.10.1/ziptimezone/mappings.py
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 ziptimezone-0.10.1/PKG-INFO
```

### Comparing `ziptimezone-0.10.0/ziptimezone/__init__.py` & `ziptimezone-0.10.1/ziptimezone/__init__.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.0/ziptimezone/core copy.py` & `ziptimezone-0.10.1/ziptimezone/core copy.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.0/ziptimezone/core.py` & `ziptimezone-0.10.1/ziptimezone/core.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.0/ziptimezone/data_manager.py` & `ziptimezone-0.10.1/ziptimezone/data_manager.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.0/ziptimezone/geocode.py` & `ziptimezone-0.10.1/ziptimezone/geocode.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.0/ziptimezone/mappings.py` & `ziptimezone-0.10.1/ziptimezone/mappings.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.0/PKG-INFO` & `ziptimezone-0.10.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ziptimezone
-Version: 0.10.0
+Version: 0.10.1
 Summary: A package to convert ZIP codes to time zones and get geographic coordinates.
 License: MIT
 Author: Manjunath Bettadapura
 Author-email: manjunathbettadapura412@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: timezonefinder (==6.5.0)
 Description-Content-Type: text/markdown
 
-### This is basically a simple wrapper around pgeocode and timezonefinder packages.
+### Uses geonames and timezonefinder.
 ### Convenience functions to get:
 ### 1. The latitude and longitude for a given US or Puerto Rico Zip Code
 ### 2. The more commonly identifiable timezone for a given zipcode(ex: Eastern, Central, Mountain, et al)
```

