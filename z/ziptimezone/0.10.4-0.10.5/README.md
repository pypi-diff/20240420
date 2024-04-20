# Comparing `tmp/ziptimezone-0.10.4.tar.gz` & `tmp/ziptimezone-0.10.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziptimezone-0.10.4.tar", max compression
+gzip compressed data, was "ziptimezone-0.10.5.tar", max compression
```

## Comparing `ziptimezone-0.10.4.tar` & `ziptimezone-0.10.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-0.10.4/LICENSE
--rw-r--r--   0        0        0      553 2024-04-20 12:31:22.652365 ziptimezone-0.10.4/pyproject.toml
--rw-r--r--   0        0        0      320 2024-04-20 11:29:25.216037 ziptimezone-0.10.4/README.md
--rw-r--r--   0        0        0      994 2024-04-20 11:29:25.228270 ziptimezone-0.10.4/ziptimezone/__init__.py
--rw-r--r--   0        0        0     3128 2024-04-20 11:29:25.229297 ziptimezone-0.10.4/ziptimezone/core.py
--rw-r--r--   0        0        0     2762 2024-04-20 11:29:25.233383 ziptimezone-0.10.4/ziptimezone/data_manager.py
--rw-r--r--   0        0        0     1099 2024-04-20 12:33:29.828260 ziptimezone-0.10.4/ziptimezone/geocode.py
--rw-r--r--   0        0        0     1873 2024-04-20 11:29:25.238387 ziptimezone-0.10.4/ziptimezone/mappings.py
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 ziptimezone-0.10.4/PKG-INFO
+-rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-0.10.5/LICENSE
+-rw-r--r--   0        0        0      553 2024-04-20 12:56:05.853890 ziptimezone-0.10.5/pyproject.toml
+-rw-r--r--   0        0        0      320 2024-04-20 11:29:25.216037 ziptimezone-0.10.5/README.md
+-rw-r--r--   0        0        0     1017 2024-04-20 12:55:53.075094 ziptimezone-0.10.5/ziptimezone/__init__.py
+-rw-r--r--   0        0        0     4299 2024-04-20 12:55:47.047536 ziptimezone-0.10.5/ziptimezone/core.py
+-rw-r--r--   0        0        0     2762 2024-04-20 11:29:25.233383 ziptimezone-0.10.5/ziptimezone/data_manager.py
+-rw-r--r--   0        0        0     1099 2024-04-20 12:33:29.828260 ziptimezone-0.10.5/ziptimezone/geocode.py
+-rw-r--r--   0        0        0     1873 2024-04-20 11:29:25.238387 ziptimezone-0.10.5/ziptimezone/mappings.py
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 ziptimezone-0.10.5/PKG-INFO
```

### Comparing `ziptimezone-0.10.4/pyproject.toml` & `ziptimezone-0.10.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ziptimezone"
-version = "0.10.4"
+version = "0.10.5"
 description = "A package to convert ZIP codes to time zones and get geographic coordinates."
 readme = "README.md"
 authors = ["Manjunath Bettadapura <manjunathbettadapura412@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <4.0"
```

### Comparing `ziptimezone-0.10.4/ziptimezone/__init__.py` & `ziptimezone-0.10.5/ziptimezone/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 # Get the timezone of a ZIP code
 timezone = get_timezone_by_zip('85260')
 
 # Get the latitude and longitude of a ZIP code
 latitude, longitude = get_lat_long_for_zip('02138')
 """
 
-from .core import get_timezone_by_zip
+from .core import get_timezone_by_zip, get_lat_long_for_zip
 from .mappings import map_timezone_to_region
-from .geocode import get_lat_long_for_zip
+#from .geocode import get_lat_long_for_zip
 
 __all__ = ['get_timezone_by_zip', 'map_timezone_to_region', 'get_lat_long_for_zip']
```

### Comparing `ziptimezone-0.10.4/ziptimezone/core.py` & `ziptimezone-0.10.5/ziptimezone/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -37,14 +37,44 @@
     with open(file_path, newline='', encoding='utf-8') as csvfile:
         reader = csv.DictReader(csvfile, fieldnames=['country_code', 'postal_code', 'place_name', 'admin_name1',
                                                      'admin_code1', 'admin_name2', 'admin_code2', 'admin_name3',
                                                      'admin_code3', 'latitude', 'longitude', 'accuracy'], delimiter='\t')
         loaded_zip_data = {row['postal_code']: row for row in reader}
     return loaded_zip_data
 
+def get_lat_long_for_zip(zip_code, country='US'):
+    """
+    Retrieve the latitude and longitude for a given ZIP code.
+
+    Parameters:
+        zip_code (str): The ZIP code for which geographic coordinates are requested.
+        country (str): Country code to refine the search, default is 'US'.
+
+    Returns:
+        tuple: A tuple containing latitude and longitude (float, float) if found, otherwise (None, None).
+
+    Raises:
+        ValueError: If the zip_code is not recognized.
+    """
+    
+    if not isinstance(zip_code, str) or zip_code.strip() == '':
+        # Return None if the zip_code is not a string or is an empty string.
+        return None, None
+    
+    zip_data = load_zip_data()
+    location = zip_data.get(zip_code)
+    #nomi = pgeocode.Nominatim(country)
+    #location = nomi.query_postal_code(zip_code)
+    
+    if location is not None #and not pd.isna(location.latitude) and not pd.isna(location.longitude):
+        return location.latitude, location.longitude
+    else:
+        #raise ValueError(f"ZIP code {zip_code} not recognized.")
+        return None, None
+    
 def get_timezone_by_zip(zip_code):
     """
     Retrieve the timezone based on the provided ZIP code from locally stored data.
 
     This function uses geographic coordinates obtained from a ZIP code stored in a local file
     to determine the corresponding timezone using the TimezoneFinder library.
 
@@ -54,17 +84,17 @@
     Returns:
         str: The timezone string (e.g., 'America/New_York') if found,
              returns 'Unknown' if the timezone cannot be determined.
 
     Raises:
         ValueError: If no geographic coordinates can be determined for the given ZIP code.
     """
-    zip_data = load_zip_data()
-    location = zip_data.get(zip_code)
-
+    #zip_data = load_zip_data()
+    #location = zip_data.get(zip_code)
+    location = get_lat_long_for_zip(zip_code)
     if location and location['latitude'] and location['longitude']:
         latitude, longitude = float(location['latitude']), float(location['longitude'])
         tf = TimezoneFinder()
         timezone = tf.timezone_at(lat=latitude, lng=longitude)
         if timezone:
             return map_timezone_to_region(timezone)
         else:
```

### Comparing `ziptimezone-0.10.4/ziptimezone/data_manager.py` & `ziptimezone-0.10.5/ziptimezone/data_manager.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.4/ziptimezone/geocode.py` & `ziptimezone-0.10.5/ziptimezone/geocode.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.4/ziptimezone/mappings.py` & `ziptimezone-0.10.5/ziptimezone/mappings.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.4/PKG-INFO` & `ziptimezone-0.10.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziptimezone
-Version: 0.10.4
+Version: 0.10.5
 Summary: A package to convert ZIP codes to time zones and get geographic coordinates.
 License: MIT
 Author: Manjunath Bettadapura
 Author-email: manjunathbettadapura412@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

