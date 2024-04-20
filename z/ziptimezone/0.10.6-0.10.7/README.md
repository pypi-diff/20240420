# Comparing `tmp/ziptimezone-0.10.6.tar.gz` & `tmp/ziptimezone-0.10.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziptimezone-0.10.6.tar", max compression
+gzip compressed data, was "ziptimezone-0.10.7.tar", max compression
```

## Comparing `ziptimezone-0.10.6.tar` & `ziptimezone-0.10.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-0.10.6/LICENSE
--rw-r--r--   0        0        0      553 2024-04-20 13:00:22.056445 ziptimezone-0.10.6/pyproject.toml
--rw-r--r--   0        0        0      320 2024-04-20 11:29:25.216037 ziptimezone-0.10.6/README.md
--rw-r--r--   0        0        0     1017 2024-04-20 12:55:53.075094 ziptimezone-0.10.6/ziptimezone/__init__.py
--rw-r--r--   0        0        0     4300 2024-04-20 13:00:07.957259 ziptimezone-0.10.6/ziptimezone/core.py
--rw-r--r--   0        0        0     2762 2024-04-20 11:29:25.233383 ziptimezone-0.10.6/ziptimezone/data_manager.py
--rw-r--r--   0        0        0     1099 2024-04-20 12:33:29.828260 ziptimezone-0.10.6/ziptimezone/geocode.py
--rw-r--r--   0        0        0     1873 2024-04-20 11:29:25.238387 ziptimezone-0.10.6/ziptimezone/mappings.py
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 ziptimezone-0.10.6/PKG-INFO
+-rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-0.10.7/LICENSE
+-rw-r--r--   0        0        0      553 2024-04-20 14:57:54.673324 ziptimezone-0.10.7/pyproject.toml
+-rw-r--r--   0        0        0      320 2024-04-20 11:29:25.216037 ziptimezone-0.10.7/README.md
+-rw-r--r--   0        0        0     1063 2024-04-20 14:57:15.703877 ziptimezone-0.10.7/ziptimezone/__init__.py
+-rw-r--r--   0        0        0     4137 2024-04-20 14:54:53.516662 ziptimezone-0.10.7/ziptimezone/core.py
+-rw-r--r--   0        0        0     2762 2024-04-20 11:29:25.233383 ziptimezone-0.10.7/ziptimezone/data_manager.py
+-rw-r--r--   0        0        0     1099 2024-04-20 12:33:29.828260 ziptimezone-0.10.7/ziptimezone/geocode.py
+-rw-r--r--   0        0        0     1873 2024-04-20 11:29:25.238387 ziptimezone-0.10.7/ziptimezone/mappings.py
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 ziptimezone-0.10.7/PKG-INFO
```

### Comparing `ziptimezone-0.10.6/pyproject.toml` & `ziptimezone-0.10.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "ziptimezone"
-version = "0.10.6"
+version = "0.10.7"
 description = "A package to convert ZIP codes to time zones and get geographic coordinates."
 readme = "README.md"
 authors = ["Manjunath Bettadapura <manjunathbettadapura412@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = ">=3.8, <4.0"
+python = ">=3.9, <4.0"
 requests = "^2.31.0"
 #pgeocode = "^0.5.0"
 timezonefinder = ">=6.1.5, 6.5.0"
 pandas = ">=1.3.3, 2.2.2"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `ziptimezone-0.10.6/ziptimezone/__init__.py` & `ziptimezone-0.10.7/ziptimezone/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,11 +15,12 @@
 timezone = get_timezone_by_zip('85260')
 
 # Get the latitude and longitude of a ZIP code
 latitude, longitude = get_lat_long_for_zip('02138')
 """
 
 from .core import get_timezone_by_zip, get_lat_long_for_zip
-from .mappings import map_timezone_to_region
+from .data_manager import setup_zip_code_data
+##from .mappings import map_timezone_to_region
 #from .geocode import get_lat_long_for_zip
 
-__all__ = ['get_timezone_by_zip', 'map_timezone_to_region', 'get_lat_long_for_zip']
+__all__ = ['get_timezone_by_zip', 'setup_zip_code_data', 'get_lat_long_for_zip']
```

### Comparing `ziptimezone-0.10.6/ziptimezone/core.py` & `ziptimezone-0.10.7/ziptimezone/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,21 +58,18 @@
     
     if not isinstance(zip_code, str) or zip_code.strip() == '':
         # Return None if the zip_code is not a string or is an empty string.
         return None, None
     
     zip_data = load_zip_data()
     location = zip_data.get(zip_code)
-    #nomi = pgeocode.Nominatim(country)
-    #location = nomi.query_postal_code(zip_code)
     
-    if location is not None: #and not pd.isna(location.latitude) and not pd.isna(location.longitude):
-        return location.latitude, location.longitude
+    if location is not None and location['latitude'] is not None and location['longitude'] is not None: #pd.isna(location.latitude) and not pd.isna(location.longitude):
+        return location['latitude'], location['longitude']
     else:
-        #raise ValueError(f"ZIP code {zip_code} not recognized.")
         return None, None
     
 def get_timezone_by_zip(zip_code):
     """
     Retrieve the timezone based on the provided ZIP code from locally stored data.
 
     This function uses geographic coordinates obtained from a ZIP code stored in a local file
@@ -84,20 +81,18 @@
     Returns:
         str: The timezone string (e.g., 'America/New_York') if found,
              returns 'Unknown' if the timezone cannot be determined.
 
     Raises:
         ValueError: If no geographic coordinates can be determined for the given ZIP code.
     """
-    #zip_data = load_zip_data()
-    #location = zip_data.get(zip_code)
-    location = get_lat_long_for_zip(zip_code)
-    if location and location['latitude'] and location['longitude']:
-        latitude, longitude = float(location['latitude']), float(location['longitude'])
-        tf = TimezoneFinder()
-        timezone = tf.timezone_at(lat=latitude, lng=longitude)
+    latitude, longitude = get_lat_long_for_zip(zip_code)
+    if latitude and longitude:
+        tf = TimezoneFinder(in_memory=True)
+        timezone = tf.timezone_at(lat=float(latitude), lng=float(longitude))
         if timezone:
             return map_timezone_to_region(timezone)
         else:
             return 'Unknown'
     else:
-        raise ValueError(f"No valid geographic coordinates found for ZIP code {zip_code}.")
+        #raise ValueError(f"No valid geographic coordinates found for ZIP code {zip_code}.")
+        return f"No valid geographic coordinates for ZIP Code {zip_code} in US"
```

### Comparing `ziptimezone-0.10.6/ziptimezone/data_manager.py` & `ziptimezone-0.10.7/ziptimezone/data_manager.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.6/ziptimezone/geocode.py` & `ziptimezone-0.10.7/ziptimezone/geocode.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.6/ziptimezone/mappings.py` & `ziptimezone-0.10.7/ziptimezone/mappings.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.6/PKG-INFO` & `ziptimezone-0.10.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: ziptimezone
-Version: 0.10.6
+Version: 0.10.7
 Summary: A package to convert ZIP codes to time zones and get geographic coordinates.
 License: MIT
 Author: Manjunath Bettadapura
 Author-email: manjunathbettadapura412@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (==2.2.2)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: timezonefinder (==6.5.0)
```

