# Comparing `tmp/ziptimezone-0.10.1.tar.gz` & `tmp/ziptimezone-0.10.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziptimezone-0.10.1.tar", max compression
+gzip compressed data, was "ziptimezone-0.10.2.tar", max compression
```

## Comparing `ziptimezone-0.10.1.tar` & `ziptimezone-0.10.2.tar`

### file list

```diff
@@ -1,11 +1,9 @@
--rw-r--r--   0        0        0        1 2024-04-18 17:39:45.000000 ziptimezone-0.10.1/LICENSE
--rw-r--r--   0        0        0      252 2024-04-19 21:47:29.146818 ziptimezone-0.10.1/README.md
--rw-r--r--   0        0        0      489 2024-04-19 21:47:34.870778 ziptimezone-0.10.1/pyproject.toml
--rw-r--r--   0        0        0      969 2024-04-18 17:39:45.000000 ziptimezone-0.10.1/ziptimezone/__init__.py
--rw-r--r--   0        0        0     1365 2024-04-19 15:38:14.654911 ziptimezone-0.10.1/ziptimezone/core copy.py
--rw-r--r--   0        0        0     3056 2024-04-19 20:45:15.084480 ziptimezone-0.10.1/ziptimezone/core.py
--rw-r--r--   0        0        0        0 2024-04-19 15:41:48.857464 ziptimezone-0.10.1/ziptimezone/data/.gitkeep
--rw-r--r--   0        0        0     2697 2024-04-19 15:57:50.850984 ziptimezone-0.10.1/ziptimezone/data_manager.py
--rw-r--r--   0        0        0     1050 2024-04-18 19:09:15.017940 ziptimezone-0.10.1/ziptimezone/geocode.py
--rw-r--r--   0        0        0     1825 2024-04-18 17:39:45.000000 ziptimezone-0.10.1/ziptimezone/mappings.py
--rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 ziptimezone-0.10.1/PKG-INFO
+-rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-0.10.2/LICENSE
+-rw-r--r--   0        0        0      529 2024-04-20 11:56:28.072753 ziptimezone-0.10.2/pyproject.toml
+-rw-r--r--   0        0        0      320 2024-04-20 11:29:25.216037 ziptimezone-0.10.2/README.md
+-rw-r--r--   0        0        0      994 2024-04-20 11:29:25.228270 ziptimezone-0.10.2/ziptimezone/__init__.py
+-rw-r--r--   0        0        0     3128 2024-04-20 11:29:25.229297 ziptimezone-0.10.2/ziptimezone/core.py
+-rw-r--r--   0        0        0     2762 2024-04-20 11:29:25.233383 ziptimezone-0.10.2/ziptimezone/data_manager.py
+-rw-r--r--   0        0        0     1110 2024-04-20 11:52:46.868177 ziptimezone-0.10.2/ziptimezone/geocode.py
+-rw-r--r--   0        0        0     1873 2024-04-20 11:29:25.238387 ziptimezone-0.10.2/ziptimezone/mappings.py
+-rw-r--r--   0        0        0     1091 1970-01-01 00:00:00.000000 ziptimezone-0.10.2/PKG-INFO
```

### Comparing `ziptimezone-0.10.1/ziptimezone/__init__.py` & `ziptimezone-0.10.2/ziptimezone/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-"""
-The ziptimezone package provides utilities for converting ZIP codes to time zones
-and retrieving geographic coordinates (latitude and longitude) based on ZIP codes.
-
-This package includes:
-- `get_timezone_by_zip`: Function to convert a ZIP code into a timezone name.
-- `map_timezone_to_region`: Function to map detailed timezone names to broader, 
-  more general region names (e.g., 'Eastern', 'Central').
-- `get_lat_long`: Function to retrieve the latitude and longitude for a given ZIP code.
-
-Example usage:
-from ziptimezone import get_timezone_by_zip, get_lat_long_for_zip
-
-# Get the timezone of a ZIP code
-timezone = get_timezone_by_zip('85260')
-
-# Get the latitude and longitude of a ZIP code
-latitude, longitude = get_lat_long_for_zip('02138')
-"""
-
-from .core import get_timezone_by_zip
-from .mappings import map_timezone_to_region
-from .geocode import get_lat_long_for_zip
-
-__all__ = ['get_timezone_by_zip', 'map_timezone_to_region', 'get_lat_long_for_zip']
+"""
+The ziptimezone package provides utilities for converting ZIP codes to time zones
+and retrieving geographic coordinates (latitude and longitude) based on ZIP codes.
+
+This package includes:
+- `get_timezone_by_zip`: Function to convert a ZIP code into a timezone name.
+- `map_timezone_to_region`: Function to map detailed timezone names to broader, 
+  more general region names (e.g., 'Eastern', 'Central').
+- `get_lat_long`: Function to retrieve the latitude and longitude for a given ZIP code.
+
+Example usage:
+from ziptimezone import get_timezone_by_zip, get_lat_long_for_zip
+
+# Get the timezone of a ZIP code
+timezone = get_timezone_by_zip('85260')
+
+# Get the latitude and longitude of a ZIP code
+latitude, longitude = get_lat_long_for_zip('02138')
+"""
+
+from .core import get_timezone_by_zip
+from .mappings import map_timezone_to_region
+from .geocode import get_lat_long_for_zip
+
+__all__ = ['get_timezone_by_zip', 'map_timezone_to_region', 'get_lat_long_for_zip']
```

### Comparing `ziptimezone-0.10.1/ziptimezone/core.py` & `ziptimezone-0.10.2/ziptimezone/core.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-from timezonefinder import TimezoneFinder
-import csv
-from .data_manager import get_data_file_path
-from .mappings import map_timezone_to_region
-'''
-def load_zip_data():
-    """
-    Loads ZIP code data from a CSV file into a dictionary.
-
-    Returns:
-        dict: A dictionary where the keys are ZIP codes and the values are dictionaries with
-              latitude and longitude.
-    """
-    file_path = get_data_file_path()
-    with open(file_path, newline='', encoding='utf-8') as csvfile:
-        reader = csv.DictReader(csvfile, fieldnames=['country_code', 'postal_code', 'place_name', 'admin_name1',
-                                                     'admin_code1', 'admin_name2', 'admin_code2', 'admin_name3',
-                                                     'admin_code3', 'latitude', 'longitude', 'accuracy'], delimiter='\t')
-        zip_data = {row['postal_code']: row for row in reader}
-    return zip_data
-'''
-loaded_zip_data = None
-
-def load_zip_data():
-    """
-    Loads ZIP code data from a CSV file into a dictionary if it is not already loaded.
-
-    Returns:
-        dict: A dictionary where the keys are ZIP codes and the values are dictionaries with
-              latitude and longitude.
-    """
-    global loaded_zip_data
-    if loaded_zip_data is not None:
-        return loaded_zip_data
-
-    file_path = get_data_file_path()
-    with open(file_path, newline='', encoding='utf-8') as csvfile:
-        reader = csv.DictReader(csvfile, fieldnames=['country_code', 'postal_code', 'place_name', 'admin_name1',
-                                                     'admin_code1', 'admin_name2', 'admin_code2', 'admin_name3',
-                                                     'admin_code3', 'latitude', 'longitude', 'accuracy'], delimiter='\t')
-        loaded_zip_data = {row['postal_code']: row for row in reader}
-    return loaded_zip_data
-
-def get_timezone_by_zip(zip_code):
-    """
-    Retrieve the timezone based on the provided ZIP code from locally stored data.
-
-    This function uses geographic coordinates obtained from a ZIP code stored in a local file
-    to determine the corresponding timezone using the TimezoneFinder library.
-
-    Parameters:
-        zip_code (str): The ZIP code for which the timezone is requested.
-
-    Returns:
-        str: The timezone string (e.g., 'America/New_York') if found,
-             returns 'Unknown' if the timezone cannot be determined.
-
-    Raises:
-        ValueError: If no geographic coordinates can be determined for the given ZIP code.
-    """
-    zip_data = load_zip_data()
-    location = zip_data.get(zip_code)
-
-    if location and location['latitude'] and location['longitude']:
-        latitude, longitude = float(location['latitude']), float(location['longitude'])
-        tf = TimezoneFinder()
-        timezone = tf.timezone_at(lat=latitude, lng=longitude)
-        if timezone:
-            return map_timezone_to_region(timezone)
-        else:
-            return 'Unknown'
-    else:
+from timezonefinder import TimezoneFinder
+import csv
+from .data_manager import get_data_file_path
+from .mappings import map_timezone_to_region
+'''
+def load_zip_data():
+    """
+    Loads ZIP code data from a CSV file into a dictionary.
+
+    Returns:
+        dict: A dictionary where the keys are ZIP codes and the values are dictionaries with
+              latitude and longitude.
+    """
+    file_path = get_data_file_path()
+    with open(file_path, newline='', encoding='utf-8') as csvfile:
+        reader = csv.DictReader(csvfile, fieldnames=['country_code', 'postal_code', 'place_name', 'admin_name1',
+                                                     'admin_code1', 'admin_name2', 'admin_code2', 'admin_name3',
+                                                     'admin_code3', 'latitude', 'longitude', 'accuracy'], delimiter='\t')
+        zip_data = {row['postal_code']: row for row in reader}
+    return zip_data
+'''
+loaded_zip_data = None
+
+def load_zip_data():
+    """
+    Loads ZIP code data from a CSV file into a dictionary if it is not already loaded.
+
+    Returns:
+        dict: A dictionary where the keys are ZIP codes and the values are dictionaries with
+              latitude and longitude.
+    """
+    global loaded_zip_data
+    if loaded_zip_data is not None:
+        return loaded_zip_data
+
+    file_path = get_data_file_path()
+    with open(file_path, newline='', encoding='utf-8') as csvfile:
+        reader = csv.DictReader(csvfile, fieldnames=['country_code', 'postal_code', 'place_name', 'admin_name1',
+                                                     'admin_code1', 'admin_name2', 'admin_code2', 'admin_name3',
+                                                     'admin_code3', 'latitude', 'longitude', 'accuracy'], delimiter='\t')
+        loaded_zip_data = {row['postal_code']: row for row in reader}
+    return loaded_zip_data
+
+def get_timezone_by_zip(zip_code):
+    """
+    Retrieve the timezone based on the provided ZIP code from locally stored data.
+
+    This function uses geographic coordinates obtained from a ZIP code stored in a local file
+    to determine the corresponding timezone using the TimezoneFinder library.
+
+    Parameters:
+        zip_code (str): The ZIP code for which the timezone is requested.
+
+    Returns:
+        str: The timezone string (e.g., 'America/New_York') if found,
+             returns 'Unknown' if the timezone cannot be determined.
+
+    Raises:
+        ValueError: If no geographic coordinates can be determined for the given ZIP code.
+    """
+    zip_data = load_zip_data()
+    location = zip_data.get(zip_code)
+
+    if location and location['latitude'] and location['longitude']:
+        latitude, longitude = float(location['latitude']), float(location['longitude'])
+        tf = TimezoneFinder()
+        timezone = tf.timezone_at(lat=latitude, lng=longitude)
+        if timezone:
+            return map_timezone_to_region(timezone)
+        else:
+            return 'Unknown'
+    else:
         raise ValueError(f"No valid geographic coordinates found for ZIP code {zip_code}.")
```

### Comparing `ziptimezone-0.10.1/ziptimezone/data_manager.py` & `ziptimezone-0.10.2/ziptimezone/data_manager.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-import os
-import requests
-import zipfile
-import logging
-
-# Setup basic configuration for logging
-logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
-
-def download_and_extract_zip_data(file_path, data_url):
-    """
-    Downloads a ZIP file from the specified URL and extracts its contents into a predefined path.
-
-    Args:
-        file_path (str): The full path where the extracted file will be stored. The ZIP file will be temporarily stored in the same location.
-        data_url (str): The URL from which to download the ZIP file containing the data.
-
-    Ensures that if the data file at the file_path does not exist, it is downloaded and extracted.
-    If the data file already exists, no action is taken.
-    """
-    if not os.path.exists(file_path):
-        zip_path = file_path + '.zip'
-        logging.info("Downloading ZIP code data...")
-        try:
-            response = requests.get(data_url)
-            response.raise_for_status()  # Ensure the download succeeded
-            with open(zip_path, 'wb') as f:
-                f.write(response.content)
-
-            # Extract ZIP file
-            with zipfile.ZipFile(zip_path, 'r') as zip_ref:
-                zip_ref.extractall(os.path.dirname(file_path))
-            os.remove(zip_path)  # Remove the zip file after extraction
-
-            logging.info("Data downloaded and extracted successfully.")
-        except requests.RequestException as e:
-            logging.error(f"Failed to download the data: {e}")
-        except zipfile.BadZipFile:
-            logging.error("Failed to extract the ZIP file because it was corrupted.")
-        except Exception as e:
-            logging.error(f"An error occurred: {e}")
-    else:
-        logging.info("Data already exists.")
-
-def get_data_file_path():
-    """
-    Constructs the file path for storing the data file within the package.
-
-    Returns:
-        str: The file path where the data file should be stored. This path points to a directory 'data' at the same level as this script.
-    """
-    data_directory = os.path.join(os.path.dirname(__file__), '..', 'data')
-    os.makedirs(data_directory, exist_ok=True)
-    return os.path.join(data_directory, 'US.txt')
-
-def setup_zip_code_data():
-    """Function can be called on demand to download and setup ZIP code data."""
-    file_path = get_data_file_path()
-    data_url = 'https://download.geonames.org/export/zip/US.zip'
-    download_and_extract_zip_data(file_path, data_url)
-
-if __name__ != '__main__':
-    #file_path = get_data_file_path()
-    #data_url = 'https://download.geonames.org/export/zip/US.zip'
-    #download_and_extract_zip_data(file_path, data_url)
-    setup_zip_code_data()
+import os
+import requests
+import zipfile
+import logging
+
+# Setup basic configuration for logging
+logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+
+def download_and_extract_zip_data(file_path, data_url):
+    """
+    Downloads a ZIP file from the specified URL and extracts its contents into a predefined path.
+
+    Args:
+        file_path (str): The full path where the extracted file will be stored. The ZIP file will be temporarily stored in the same location.
+        data_url (str): The URL from which to download the ZIP file containing the data.
+
+    Ensures that if the data file at the file_path does not exist, it is downloaded and extracted.
+    If the data file already exists, no action is taken.
+    """
+    if not os.path.exists(file_path):
+        zip_path = file_path + '.zip'
+        logging.info("Downloading ZIP code data...")
+        try:
+            response = requests.get(data_url)
+            response.raise_for_status()  # Ensure the download succeeded
+            with open(zip_path, 'wb') as f:
+                f.write(response.content)
+
+            # Extract ZIP file
+            with zipfile.ZipFile(zip_path, 'r') as zip_ref:
+                zip_ref.extractall(os.path.dirname(file_path))
+            os.remove(zip_path)  # Remove the zip file after extraction
+
+            logging.info("Data downloaded and extracted successfully.")
+        except requests.RequestException as e:
+            logging.error(f"Failed to download the data: {e}")
+        except zipfile.BadZipFile:
+            logging.error("Failed to extract the ZIP file because it was corrupted.")
+        except Exception as e:
+            logging.error(f"An error occurred: {e}")
+    else:
+        logging.info("Data already exists.")
+
+def get_data_file_path():
+    """
+    Constructs the file path for storing the data file within the package.
+
+    Returns:
+        str: The file path where the data file should be stored. This path points to a directory 'data' at the same level as this script.
+    """
+    data_directory = os.path.join(os.path.dirname(__file__), '..', 'data')
+    os.makedirs(data_directory, exist_ok=True)
+    return os.path.join(data_directory, 'US.txt')
+
+def setup_zip_code_data():
+    """Function can be called on demand to download and setup ZIP code data."""
+    file_path = get_data_file_path()
+    data_url = 'https://download.geonames.org/export/zip/US.zip'
+    download_and_extract_zip_data(file_path, data_url)
+
+if __name__ != '__main__':
+    #file_path = get_data_file_path()
+    #data_url = 'https://download.geonames.org/export/zip/US.zip'
+    #download_and_extract_zip_data(file_path, data_url)
+    setup_zip_code_data()
```

### Comparing `ziptimezone-0.10.1/ziptimezone/geocode.py` & `ziptimezone-0.10.2/ziptimezone/geocode.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-import pgeocode
-import pandas as pd
-
-def get_lat_long_for_zip(zip_code, country='US'):
-    """
-    Retrieve the latitude and longitude for a given ZIP code.
-
-    Parameters:
-        zip_code (str): The ZIP code for which geographic coordinates are requested.
-        country (str): Country code to refine the search, default is 'US'.
-
-    Returns:
-        tuple: A tuple containing latitude and longitude (float, float) if found, otherwise (None, None).
-
-    Raises:
-        ValueError: If the zip_code is not recognized.
-    """
-
-    if not isinstance(zip_code, str) or zip_code.strip() == '':
-        # Return None if the zip_code is not a string or is an empty string.
-        return None, None
-    
-    nomi = pgeocode.Nominatim(country)
-    location = nomi.query_postal_code(zip_code)
-    
-    if location is not None and not pd.isna(location.latitude) and not pd.isna(location.longitude):
-        return location.latitude, location.longitude
-    else:
-        #raise ValueError(f"ZIP code {zip_code} not recognized.")
-        return None, None
+#import pgeocode
+#import pandas as pd
+
+#def get_lat_long_for_zip(zip_code, country='US'):
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
+    '''
+    if not isinstance(zip_code, str) or zip_code.strip() == '':
+        # Return None if the zip_code is not a string or is an empty string.
+        return None, None
+    
+    nomi = pgeocode.Nominatim(country)
+    location = nomi.query_postal_code(zip_code)
+    
+    if location is not None and not pd.isna(location.latitude) and not pd.isna(location.longitude):
+        return location.latitude, location.longitude
+    else:
+        #raise ValueError(f"ZIP code {zip_code} not recognized.")
+        return None, None
+    '''
+#    pass
```

### Comparing `ziptimezone-0.10.1/ziptimezone/mappings.py` & `ziptimezone-0.10.2/ziptimezone/mappings.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-def map_timezone_to_region(timezone):
-    """
-    Maps a detailed timezone name to a more general region name.
-
-    Currently it is set to popular regions in US and PR
-
-    This function uses a predefined mapping to convert timezone identifiers
-    like 'America/New_York' into more generally understood regional names
-    such as 'Eastern', 'Central', etc.
-
-    Parameters:
-        timezone (str): The detailed timezone identifier to be mapped.
-
-    Returns:
-        str: A general region name (e.g., 'Eastern'), or 'Unknown' if the
-             timezone is not recognized or not included in the mapping.
-
-    Example:
-        >>> map_timezone_to_region('America/New_York')
-        'Eastern'
-    """
-    mapping = {
-        'America/New_York': 'Eastern',
-        'America/Detroit': 'Eastern',
-        'America/Kentucky/Louisville': 'Eastern',
-        'America/Kentucky/Monticello': 'Eastern',
-        'America/Indiana/Indianapolis': 'Eastern',
-        'America/Indiana/Vincennes': 'Eastern',
-        'America/Indiana/Winamac': 'Eastern',
-        'America/Indiana/Marengo': 'Eastern',
-        'America/Indiana/Petersburg': 'Eastern',
-        'America/Indiana/Vevay': 'Eastern',
-        'America/Chicago': 'Central',
-        'America/Indiana/Tell_City': 'Central',
-        'America/Indiana/Knox': 'Central',
-        'America/Menominee': 'Central',
-        'America/North_Dakota/Center': 'Central',
-        'America/North_Dakota/New_Salem': 'Central',
-        'America/North_Dakota/Beulah': 'Central',
-        'America/Denver': 'Mountain',
-        'America/Boise': 'Mountain',
-        'America/Phoenix': 'Mountain',
-        'America/Los_Angeles': 'Pacific',
-        'America/Anchorage': 'Alaska',
-        'Pacific/Honolulu': 'Hawaii',
-        'America/Puerto_Rico': 'Atlantic'
-    }
-    return mapping.get(timezone, 'Unknown')
+def map_timezone_to_region(timezone):
+    """
+    Maps a detailed timezone name to a more general region name.
+
+    Currently it is set to popular regions in US and PR
+
+    This function uses a predefined mapping to convert timezone identifiers
+    like 'America/New_York' into more generally understood regional names
+    such as 'Eastern', 'Central', etc.
+
+    Parameters:
+        timezone (str): The detailed timezone identifier to be mapped.
+
+    Returns:
+        str: A general region name (e.g., 'Eastern'), or 'Unknown' if the
+             timezone is not recognized or not included in the mapping.
+
+    Example:
+        >>> map_timezone_to_region('America/New_York')
+        'Eastern'
+    """
+    mapping = {
+        'America/New_York': 'Eastern',
+        'America/Detroit': 'Eastern',
+        'America/Kentucky/Louisville': 'Eastern',
+        'America/Kentucky/Monticello': 'Eastern',
+        'America/Indiana/Indianapolis': 'Eastern',
+        'America/Indiana/Vincennes': 'Eastern',
+        'America/Indiana/Winamac': 'Eastern',
+        'America/Indiana/Marengo': 'Eastern',
+        'America/Indiana/Petersburg': 'Eastern',
+        'America/Indiana/Vevay': 'Eastern',
+        'America/Chicago': 'Central',
+        'America/Indiana/Tell_City': 'Central',
+        'America/Indiana/Knox': 'Central',
+        'America/Menominee': 'Central',
+        'America/North_Dakota/Center': 'Central',
+        'America/North_Dakota/New_Salem': 'Central',
+        'America/North_Dakota/Beulah': 'Central',
+        'America/Denver': 'Mountain',
+        'America/Boise': 'Mountain',
+        'America/Phoenix': 'Mountain',
+        'America/Los_Angeles': 'Pacific',
+        'America/Anchorage': 'Alaska',
+        'Pacific/Honolulu': 'Hawaii',
+        'America/Puerto_Rico': 'Atlantic'
+    }
+    return mapping.get(timezone, 'Unknown')
```

### Comparing `ziptimezone-0.10.1/PKG-INFO` & `ziptimezone-0.10.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: ziptimezone
-Version: 0.10.1
+Version: 0.10.2
 Summary: A package to convert ZIP codes to time zones and get geographic coordinates.
 License: MIT
 Author: Manjunath Bettadapura
 Author-email: manjunathbettadapura412@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: timezonefinder (==6.5.0)
 Description-Content-Type: text/markdown
 
-### Uses geonames and timezonefinder.
-### Convenience functions to get:
-### 1. The latitude and longitude for a given US or Puerto Rico Zip Code
-### 2. The more commonly identifiable timezone for a given zipcode(ex: Eastern, Central, Mountain, et al)
+#### This uses zip_code, latitude and longitude data from geonames and timezonefinder packages.
+#### Convenience functions to get:
+##### 1. The latitude and longitude for a given US or Puerto Rico Zip Code
+##### 2. The more commonly identifiable timezone for a given zipcode(ex: Eastern, Central, Mountain, et al)
```

