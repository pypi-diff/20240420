# Comparing `tmp/flake8_json-23.7.0.tar.gz` & `tmp/flake8_json-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_json-23.7.0.tar", last modified: Tue Jul  4 21:57:08 2023, max compression
+gzip compressed data, was "flake8_json-24.4.0.tar", last modified: Sat Apr 20 18:01:02 2024, max compression
```

## Comparing `flake8_json-23.7.0.tar` & `flake8_json-24.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-04 21:57:08.323271 flake8_json-23.7.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1113 2023-07-04 21:37:55.000000 flake8_json-23.7.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1703 2023-07-04 21:57:08.323271 flake8_json-23.7.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      879 2023-07-04 21:55:26.000000 flake8_json-23.7.0/README.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1196 2023-07-04 21:57:08.323271 flake8_json-23.7.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)      167 2023-07-04 21:37:55.000000 flake8_json-23.7.0/setup.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-04 21:57:08.319271 flake8_json-23.7.0/src/
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-04 21:57:08.323271 flake8_json-23.7.0/src/flake8_json.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1703 2023-07-04 21:57:08.000000 flake8_json-23.7.0/src/flake8_json.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      310 2023-07-04 21:57:08.000000 flake8_json-23.7.0/src/flake8_json.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-07-04 21:57:08.000000 flake8_json-23.7.0/src/flake8_json.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)      186 2023-07-04 21:57:08.000000 flake8_json-23.7.0/src/flake8_json.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       21 2023-07-04 21:57:08.000000 flake8_json-23.7.0/src/flake8_json.egg-info/top_level.txt
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-04 21:57:08.323271 flake8_json-23.7.0/src/flake8_json_reporter/
--rw-r--r--   0 asottile  (1000) asottile  (1000)       58 2023-07-04 21:55:56.000000 flake8_json-23.7.0/src/flake8_json_reporter/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6287 2023-07-04 21:55:26.000000 flake8_json-23.7.0/src/flake8_json_reporter/reporters.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-04-20 18:01:02.251049 flake8_json-24.4.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1113 2024-04-20 17:55:47.000000 flake8_json-24.4.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1703 2024-04-20 18:01:02.251049 flake8_json-24.4.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      879 2024-04-20 17:55:47.000000 flake8_json-24.4.0/README.rst
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1196 2024-04-20 18:01:02.255049 flake8_json-24.4.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      167 2024-04-20 17:55:47.000000 flake8_json-24.4.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-04-20 18:01:02.251049 flake8_json-24.4.0/src/
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-04-20 18:01:02.251049 flake8_json-24.4.0/src/flake8_json.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1703 2024-04-20 18:01:02.000000 flake8_json-24.4.0/src/flake8_json.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      310 2024-04-20 18:01:02.000000 flake8_json-24.4.0/src/flake8_json.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2024-04-20 18:01:02.000000 flake8_json-24.4.0/src/flake8_json.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      186 2024-04-20 18:01:02.000000 flake8_json-24.4.0/src/flake8_json.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       21 2024-04-20 18:01:02.000000 flake8_json-24.4.0/src/flake8_json.egg-info/top_level.txt
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-04-20 18:01:02.251049 flake8_json-24.4.0/src/flake8_json_reporter/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       58 2024-04-20 18:00:06.000000 flake8_json-24.4.0/src/flake8_json_reporter/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6432 2024-04-20 17:59:31.000000 flake8_json-24.4.0/src/flake8_json_reporter/reporters.py
```

### Comparing `flake8_json-23.7.0/LICENSE` & `flake8_json-24.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_json-23.7.0/PKG-INFO` & `flake8_json-24.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8_json
-Version: 23.7.0
+Version: 24.4.0
 Summary: JSON Formatting Reporter plugin for Flake8
 Home-page: https://github.com/pycqa/flake8-json
 Author: Ian Stapleton Cordasco
 Author-email: graffatcolmingov@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `flake8_json-23.7.0/README.rst` & `flake8_json-24.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `flake8_json-23.7.0/setup.cfg` & `flake8_json-24.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `flake8_json-23.7.0/src/flake8_json.egg-info/PKG-INFO` & `flake8_json-24.4.0/src/flake8_json.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-json
-Version: 23.7.0
+Version: 24.4.0
 Summary: JSON Formatting Reporter plugin for Flake8
 Home-page: https://github.com/pycqa/flake8-json
 Author: Ian Stapleton Cordasco
 Author-email: graffatcolmingov@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `flake8_json-23.7.0/src/flake8_json_reporter/reporters.py` & `flake8_json-24.4.0/src/flake8_json_reporter/reporters.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         super().start()
         self.write_line("{")
         self.files_reported_count = 0
 
     def stop(self):
         """Override the default to finish printing JSON."""
         self.write_line("}")
+        super().stop()
 
     def beginning(self, filename):
         """We're starting a new file."""
         json_filename = json.dumps(filename)
         if self.files_reported_count > 0:
             self.write_line(f", {json_filename}: [")
         else:
@@ -79,14 +80,16 @@
     """Pretty-printing JSON formatter."""
 
     def stop(self):
         """Override the default to finish printing JSON."""
         if self.files_reported_count > 0:
             self.write_line("\n")
         self.write_line("}\n")
+        # DefaultJSON.stop would write and extra close brace
+        base.BaseFormatter.stop(self)
 
     def beginning(self, filename):
         """We're starting a new file."""
         if self.files_reported_count > 0:
             self.write_line(",\n")
             self.write_line(f"  {json.dumps(filename)}: [")
         else:
@@ -135,14 +138,15 @@
         super().start()
         self.write_line("{")
         self.files_reported_count = 0
 
     def stop(self):
         """Override the default to finish printing JSON."""
         self.write_line("}")
+        super().stop()
 
     def beginning(self, filename):
         """We're starting a new file."""
         json_filename = json.dumps(filename)
         if self.files_reported_count > 0:
             self.write_line(f", {json_filename}: [")
         else:
```

