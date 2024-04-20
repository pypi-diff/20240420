# Comparing `tmp/ziptimezone-0.10.7.tar.gz` & `tmp/ziptimezone-0.10.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziptimezone-0.10.7.tar", max compression
+gzip compressed data, was "ziptimezone-0.10.8.tar", max compression
```

## Comparing `ziptimezone-0.10.7.tar` & `ziptimezone-0.10.8.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-0.10.7/LICENSE
--rw-r--r--   0        0        0      553 2024-04-20 14:57:54.673324 ziptimezone-0.10.7/pyproject.toml
--rw-r--r--   0        0        0      320 2024-04-20 11:29:25.216037 ziptimezone-0.10.7/README.md
--rw-r--r--   0        0        0     1063 2024-04-20 14:57:15.703877 ziptimezone-0.10.7/ziptimezone/__init__.py
--rw-r--r--   0        0        0     4137 2024-04-20 14:54:53.516662 ziptimezone-0.10.7/ziptimezone/core.py
--rw-r--r--   0        0        0     2762 2024-04-20 11:29:25.233383 ziptimezone-0.10.7/ziptimezone/data_manager.py
--rw-r--r--   0        0        0     1099 2024-04-20 12:33:29.828260 ziptimezone-0.10.7/ziptimezone/geocode.py
--rw-r--r--   0        0        0     1873 2024-04-20 11:29:25.238387 ziptimezone-0.10.7/ziptimezone/mappings.py
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 ziptimezone-0.10.7/PKG-INFO
+-rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-0.10.8/LICENSE
+-rw-r--r--   0        0        0      553 2024-04-20 20:39:01.001177 ziptimezone-0.10.8/pyproject.toml
+-rw-r--r--   0        0        0      320 2024-04-20 11:29:25.216037 ziptimezone-0.10.8/README.md
+-rw-r--r--   0        0        0     1156 2024-04-20 17:39:07.779806 ziptimezone-0.10.8/ziptimezone/__init__.py
+-rw-r--r--   0        0        0     1908 2024-04-20 17:38:55.281645 ziptimezone-0.10.8/ziptimezone/batch_processor.py
+-rw-r--r--   0        0        0     1777 2024-04-20 17:22:42.377535 ziptimezone-0.10.8/ziptimezone/core.py
+-rw-r--r--   0        0        0     2780 2024-04-20 20:35:18.371359 ziptimezone-0.10.8/ziptimezone/data_manager.py
+-rw-r--r--   0        0        0     1099 2024-04-20 12:33:29.828260 ziptimezone-0.10.8/ziptimezone/geocode.py
+-rw-r--r--   0        0        0     1297 2024-04-20 17:32:08.297733 ziptimezone-0.10.8/ziptimezone/globals.py
+-rw-r--r--   0        0        0     1873 2024-04-20 11:29:25.238387 ziptimezone-0.10.8/ziptimezone/mappings.py
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 ziptimezone-0.10.8/PKG-INFO
```

### Comparing `ziptimezone-0.10.7/pyproject.toml` & `ziptimezone-0.10.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ziptimezone"
-version = "0.10.7"
+version = "0.10.8"
 description = "A package to convert ZIP codes to time zones and get geographic coordinates."
 readme = "README.md"
 authors = ["Manjunath Bettadapura <manjunathbettadapura412@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <4.0"
```

### Comparing `ziptimezone-0.10.7/ziptimezone/__init__.py` & `ziptimezone-0.10.8/ziptimezone/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,12 +15,13 @@
 timezone = get_timezone_by_zip('85260')
 
 # Get the latitude and longitude of a ZIP code
 latitude, longitude = get_lat_long_for_zip('02138')
 """
 
 from .core import get_timezone_by_zip, get_lat_long_for_zip
-from .data_manager import setup_zip_code_data
+from .data_manager import refresh_data_if_needed
+from .batch_processor import get_timezone_for_many_zips
 ##from .mappings import map_timezone_to_region
 #from .geocode import get_lat_long_for_zip
 
-__all__ = ['get_timezone_by_zip', 'setup_zip_code_data', 'get_lat_long_for_zip']
+__all__ = ['get_timezone_by_zip', 'refresh_data_if_needed', 'get_lat_long_for_zip', 'get_timezone_for_many_zips']
```

### Comparing `ziptimezone-0.10.7/ziptimezone/data_manager.py` & `ziptimezone-0.10.8/ziptimezone/data_manager.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,74 @@
+# data_manager.py
 import os
 import requests
 import zipfile
 import logging
+import shutil
+from .globals import load_zip_data, get_loaded_zip_data
 
-# Setup basic configuration for logging
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
-def download_and_extract_zip_data(file_path, data_url):
+def download_and_extract_zip_data(data_url, data_directory):
     """
-    Downloads a ZIP file from the specified URL and extracts its contents into a predefined path.
+    Downloads and extracts ZIP code data, then loads it into memory.
 
-    Args:
-        file_path (str): The full path where the extracted file will be stored. The ZIP file will be temporarily stored in the same location.
-        data_url (str): The URL from which to download the ZIP file containing the data.
-
-    Ensures that if the data file at the file_path does not exist, it is downloaded and extracted.
-    If the data file already exists, no action is taken.
+    Parameters:
+        data_url (str): URL from which to download the ZIP file.
+        data_directory (str): Directory to store and extract data.
     """
+    file_path = os.path.join(data_directory, 'US.txt')
     if not os.path.exists(file_path):
         zip_path = file_path + '.zip'
         logging.info("Downloading ZIP code data...")
         try:
             response = requests.get(data_url)
-            response.raise_for_status()  # Ensure the download succeeded
+            response.raise_for_status()
             with open(zip_path, 'wb') as f:
                 f.write(response.content)
-
-            # Extract ZIP file
             with zipfile.ZipFile(zip_path, 'r') as zip_ref:
-                zip_ref.extractall(os.path.dirname(file_path))
-            os.remove(zip_path)  # Remove the zip file after extraction
-
+                zip_ref.extractall(data_directory)
+            os.remove(zip_path)
             logging.info("Data downloaded and extracted successfully.")
-        except requests.RequestException as e:
-            logging.error(f"Failed to download the data: {e}")
-        except zipfile.BadZipFile:
-            logging.error("Failed to extract the ZIP file because it was corrupted.")
         except Exception as e:
             logging.error(f"An error occurred: {e}")
-    else:
-        logging.info("Data already exists.")
+            return
+
+    load_zip_data(file_path)  # Load data into the global variable
 
 def get_data_file_path():
     """
     Constructs the file path for storing the data file within the package.
 
     Returns:
         str: The file path where the data file should be stored. This path points to a directory 'data' at the same level as this script.
     """
-    data_directory = os.path.join(os.path.dirname(__file__), '..', 'data')
+    data_directory = os.path.join(os.path.dirname(__file__), '..', 'ziptimezone_data')
     os.makedirs(data_directory, exist_ok=True)
-    return os.path.join(data_directory, 'US.txt')
+    return data_directory
 
-def setup_zip_code_data():
-    """Function can be called on demand to download and setup ZIP code data."""
-    file_path = get_data_file_path()
+def refresh_data_if_needed():
+    """
+    Ensures that ZIP code data is loaded upon initial import or application startup.
+    This can also be called later if needed. Deletes existing data directory if it exists,
+    and re-downloads and extracts the ZIP file.
+    """
+    data_directory = get_data_file_path()
+    
+    # Check if the directory exists and remove it if it does
+    if os.path.exists(data_directory):
+        shutil.rmtree(data_directory)
+        print(f"Existing data directory {data_directory} removed.")
+    
+    # Recreate the directory
+    os.makedirs(data_directory, exist_ok=True)
+    print(f"Data directory {data_directory} created.")
+    
+    # URL for the ZIP file to download
     data_url = 'https://download.geonames.org/export/zip/US.zip'
-    download_and_extract_zip_data(file_path, data_url)
+    
+    # Download and extract the ZIP file
+    download_and_extract_zip_data(data_url, data_directory)
+    print("Data downloaded and extracted successfully.")
 
 if __name__ != '__main__':
-    #file_path = get_data_file_path()
-    #data_url = 'https://download.geonames.org/export/zip/US.zip'
-    #download_and_extract_zip_data(file_path, data_url)
-    setup_zip_code_data()
+    refresh_data_if_needed()
```

### Comparing `ziptimezone-0.10.7/ziptimezone/geocode.py` & `ziptimezone-0.10.8/ziptimezone/geocode.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.7/ziptimezone/mappings.py` & `ziptimezone-0.10.8/ziptimezone/mappings.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.7/PKG-INFO` & `ziptimezone-0.10.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziptimezone
-Version: 0.10.7
+Version: 0.10.8
 Summary: A package to convert ZIP codes to time zones and get geographic coordinates.
 License: MIT
 Author: Manjunath Bettadapura
 Author-email: manjunathbettadapura412@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

