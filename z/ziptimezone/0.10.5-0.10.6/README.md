# Comparing `tmp/ziptimezone-0.10.5.tar.gz` & `tmp/ziptimezone-0.10.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziptimezone-0.10.5.tar", max compression
+gzip compressed data, was "ziptimezone-0.10.6.tar", max compression
```

## Comparing `ziptimezone-0.10.5.tar` & `ziptimezone-0.10.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-0.10.5/LICENSE
--rw-r--r--   0        0        0      553 2024-04-20 12:56:05.853890 ziptimezone-0.10.5/pyproject.toml
--rw-r--r--   0        0        0      320 2024-04-20 11:29:25.216037 ziptimezone-0.10.5/README.md
--rw-r--r--   0        0        0     1017 2024-04-20 12:55:53.075094 ziptimezone-0.10.5/ziptimezone/__init__.py
--rw-r--r--   0        0        0     4299 2024-04-20 12:55:47.047536 ziptimezone-0.10.5/ziptimezone/core.py
--rw-r--r--   0        0        0     2762 2024-04-20 11:29:25.233383 ziptimezone-0.10.5/ziptimezone/data_manager.py
--rw-r--r--   0        0        0     1099 2024-04-20 12:33:29.828260 ziptimezone-0.10.5/ziptimezone/geocode.py
--rw-r--r--   0        0        0     1873 2024-04-20 11:29:25.238387 ziptimezone-0.10.5/ziptimezone/mappings.py
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 ziptimezone-0.10.5/PKG-INFO
+-rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-0.10.6/LICENSE
+-rw-r--r--   0        0        0      553 2024-04-20 13:00:22.056445 ziptimezone-0.10.6/pyproject.toml
+-rw-r--r--   0        0        0      320 2024-04-20 11:29:25.216037 ziptimezone-0.10.6/README.md
+-rw-r--r--   0        0        0     1017 2024-04-20 12:55:53.075094 ziptimezone-0.10.6/ziptimezone/__init__.py
+-rw-r--r--   0        0        0     4300 2024-04-20 13:00:07.957259 ziptimezone-0.10.6/ziptimezone/core.py
+-rw-r--r--   0        0        0     2762 2024-04-20 11:29:25.233383 ziptimezone-0.10.6/ziptimezone/data_manager.py
+-rw-r--r--   0        0        0     1099 2024-04-20 12:33:29.828260 ziptimezone-0.10.6/ziptimezone/geocode.py
+-rw-r--r--   0        0        0     1873 2024-04-20 11:29:25.238387 ziptimezone-0.10.6/ziptimezone/mappings.py
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 ziptimezone-0.10.6/PKG-INFO
```

### Comparing `ziptimezone-0.10.5/pyproject.toml` & `ziptimezone-0.10.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ziptimezone"
-version = "0.10.5"
+version = "0.10.6"
 description = "A package to convert ZIP codes to time zones and get geographic coordinates."
 readme = "README.md"
 authors = ["Manjunath Bettadapura <manjunathbettadapura412@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <4.0"
```

### Comparing `ziptimezone-0.10.5/ziptimezone/__init__.py` & `ziptimezone-0.10.6/ziptimezone/__init__.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.5/ziptimezone/core.py` & `ziptimezone-0.10.6/ziptimezone/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         return None, None
     
     zip_data = load_zip_data()
     location = zip_data.get(zip_code)
     #nomi = pgeocode.Nominatim(country)
     #location = nomi.query_postal_code(zip_code)
     
-    if location is not None #and not pd.isna(location.latitude) and not pd.isna(location.longitude):
+    if location is not None: #and not pd.isna(location.latitude) and not pd.isna(location.longitude):
         return location.latitude, location.longitude
     else:
         #raise ValueError(f"ZIP code {zip_code} not recognized.")
         return None, None
     
 def get_timezone_by_zip(zip_code):
     """
```

### Comparing `ziptimezone-0.10.5/ziptimezone/data_manager.py` & `ziptimezone-0.10.6/ziptimezone/data_manager.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.5/ziptimezone/geocode.py` & `ziptimezone-0.10.6/ziptimezone/geocode.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.5/ziptimezone/mappings.py` & `ziptimezone-0.10.6/ziptimezone/mappings.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.10.5/PKG-INFO` & `ziptimezone-0.10.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziptimezone
-Version: 0.10.5
+Version: 0.10.6
 Summary: A package to convert ZIP codes to time zones and get geographic coordinates.
 License: MIT
 Author: Manjunath Bettadapura
 Author-email: manjunathbettadapura412@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

