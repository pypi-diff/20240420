# Comparing `tmp/json_exporter-0.5.0.tar.gz` & `tmp/json_exporter-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_exporter-0.5.0.tar", last modified: Wed Dec 20 03:57:42 2023, max compression
+gzip compressed data, was "json_exporter-1.0.0.tar", last modified: Sat Apr 20 00:23:30 2024, max compression
```

## Comparing `json_exporter-0.5.0.tar` & `json_exporter-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2023-12-20 03:57:42.190376 json_exporter-0.5.0/
--rw-r--r--   0 desu      (1000) desu      (1000)    18092 2023-12-17 20:31:22.000000 json_exporter-0.5.0/LICENSE
--rw-r--r--   0 desu      (1000) desu      (1000)      499 2023-12-20 03:57:42.190376 json_exporter-0.5.0/PKG-INFO
--rw-r--r--   0 desu      (1000) desu      (1000)      641 2023-12-20 03:57:13.000000 json_exporter-0.5.0/pyproject.toml
--rw-r--r--   0 desu      (1000) desu      (1000)       38 2023-12-20 03:57:42.190376 json_exporter-0.5.0/setup.cfg
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2023-12-20 03:57:42.189376 json_exporter-0.5.0/src/
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2023-12-20 03:57:42.190376 json_exporter-0.5.0/src/json_exporter/
--rw-r--r--   0 desu      (1000) desu      (1000)       68 2023-12-17 21:40:29.000000 json_exporter-0.5.0/src/json_exporter/__init__.py
--rw-r--r--   0 desu      (1000) desu      (1000)     4527 2023-12-20 02:48:10.000000 json_exporter-0.5.0/src/json_exporter/json_endpoint.py
--rw-r--r--   0 desu      (1000) desu      (1000)     1203 2023-12-20 03:25:09.000000 json_exporter-0.5.0/src/json_exporter/json_exporter.py
--rw-r--r--   0 desu      (1000) desu      (1000)     1253 2023-12-18 22:35:14.000000 json_exporter-0.5.0/src/json_exporter/json_labels.py
--rw-r--r--   0 desu      (1000) desu      (1000)      776 2023-12-18 22:34:48.000000 json_exporter-0.5.0/src/json_exporter/json_metric.py
--rw-r--r--   0 desu      (1000) desu      (1000)     2093 2023-12-18 19:17:14.000000 json_exporter-0.5.0/src/json_exporter/main.py
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2023-12-20 03:57:42.190376 json_exporter-0.5.0/src/json_exporter.egg-info/
--rw-r--r--   0 desu      (1000) desu      (1000)      499 2023-12-20 03:57:42.000000 json_exporter-0.5.0/src/json_exporter.egg-info/PKG-INFO
--rw-r--r--   0 desu      (1000) desu      (1000)      462 2023-12-20 03:57:42.000000 json_exporter-0.5.0/src/json_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 desu      (1000) desu      (1000)        1 2023-12-20 03:57:42.000000 json_exporter-0.5.0/src/json_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 desu      (1000) desu      (1000)       58 2023-12-20 03:57:42.000000 json_exporter-0.5.0/src/json_exporter.egg-info/entry_points.txt
--rw-r--r--   0 desu      (1000) desu      (1000)       41 2023-12-20 03:57:42.000000 json_exporter-0.5.0/src/json_exporter.egg-info/requires.txt
--rw-r--r--   0 desu      (1000) desu      (1000)       14 2023-12-20 03:57:42.000000 json_exporter-0.5.0/src/json_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-20 00:23:30.611507 json_exporter-1.0.0/
+-rw-r--r--   0 desu      (1000) desu      (1000)    18092 2023-12-17 20:31:22.000000 json_exporter-1.0.0/LICENSE
+-rw-r--r--   0 desu      (1000) desu      (1000)     2747 2024-04-20 00:23:30.611507 json_exporter-1.0.0/PKG-INFO
+-rw-r--r--   0 desu      (1000) desu      (1000)      666 2024-04-20 00:20:35.000000 json_exporter-1.0.0/pyproject.toml
+-rw-r--r--   0 desu      (1000) desu      (1000)     2216 2024-01-19 23:45:27.000000 json_exporter-1.0.0/readme.md
+-rw-r--r--   0 desu      (1000) desu      (1000)       38 2024-04-20 00:23:30.611507 json_exporter-1.0.0/setup.cfg
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-20 00:23:30.610507 json_exporter-1.0.0/src/
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-20 00:23:30.610507 json_exporter-1.0.0/src/json_exporter/
+-rw-r--r--   0 desu      (1000) desu      (1000)       68 2023-12-17 21:40:29.000000 json_exporter-1.0.0/src/json_exporter/__init__.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     5672 2024-01-20 19:49:56.000000 json_exporter-1.0.0/src/json_exporter/json_endpoint.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     2383 2024-01-20 01:17:34.000000 json_exporter-1.0.0/src/json_exporter/json_exporter.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     1493 2024-01-19 23:13:01.000000 json_exporter-1.0.0/src/json_exporter/json_labels.py
+-rw-r--r--   0 desu      (1000) desu      (1000)      559 2024-01-11 04:22:57.000000 json_exporter-1.0.0/src/json_exporter/json_metric.py
+-rw-r--r--   0 desu      (1000) desu      (1000)      412 2024-01-20 19:30:29.000000 json_exporter-1.0.0/src/json_exporter/main.py
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-20 00:23:30.611507 json_exporter-1.0.0/src/json_exporter.egg-info/
+-rw-r--r--   0 desu      (1000) desu      (1000)     2747 2024-04-20 00:23:30.000000 json_exporter-1.0.0/src/json_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 desu      (1000) desu      (1000)      472 2024-04-20 00:23:30.000000 json_exporter-1.0.0/src/json_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 desu      (1000) desu      (1000)        1 2024-04-20 00:23:30.000000 json_exporter-1.0.0/src/json_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 desu      (1000) desu      (1000)       58 2024-04-20 00:23:30.000000 json_exporter-1.0.0/src/json_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 desu      (1000) desu      (1000)       56 2024-04-20 00:23:30.000000 json_exporter-1.0.0/src/json_exporter.egg-info/requires.txt
+-rw-r--r--   0 desu      (1000) desu      (1000)       14 2024-04-20 00:23:30.000000 json_exporter-1.0.0/src/json_exporter.egg-info/top_level.txt
```

### Comparing `json_exporter-0.5.0/LICENSE` & `json_exporter-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `json_exporter-0.5.0/pyproject.toml` & `json_exporter-1.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "json_exporter"
-version = "0.5.0"
+version = "1.0.0"
 authors = [
   { name="Desultory", email="dev@pyl.onl" },
 ]
 description = "A Python library for exporting JSON data as metrics for Prometheus"
 readme = "readme.md"
-requires-python = ">=3.9"
+requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "prometheus_exporter >= 0.7.0",
-    "zenlib >= 1.1.1"
+    "prometheus_exporter >= 1.0.0",
+    "aiohttp >= 3.9.1",
+    "zenlib >= 2.0.0"
 ]
 
 [project.scripts]
 json_exporter = "json_exporter.main:main"
```

### Comparing `json_exporter-0.5.0/src/json_exporter/json_exporter.py` & `json_exporter-1.0.0/src/json_exporter/json_exporter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,54 @@
-"""
-JSON exporter class
-"""
+from prometheus_exporter import Exporter
+from asyncio import TaskGroup
 
-from prometheus_exporter import Exporter, cached_exporter
 
-
-@cached_exporter
 class JSONExporter(Exporter):
-    """
-    JSON exporter class for prometheus metrics.
-    """
-    endpoints = []
-
+    """ JSON exporter class for prometheus metrics. """
     def __init__(self, *args, **kwargs):
-        kwargs['port'] = kwargs.pop('port', 9809)
+        self.endpoints = []
+        kwargs['listen_port'] = kwargs.pop('listen_port', 9809)
         super().__init__(*args, **kwargs)
 
     def read_config(self):
-        """ Override to read json.headers and json_endpoint from the config """
+        """ Ensure JSON config is defined, use that to define endpoints, which will then read the config. """
         super().read_config()
         if 'json' not in self.config:
             raise ValueError("No json config defined.")
 
         from .json_endpoint import JSONEndpoint
         # Iterate over each defined endpoint
-        for endpoint_name, config in self.config['json'].items():
-            self.endpoints.append(JSONEndpoint(name=endpoint_name,
-                                               **config, logger=self.logger, _log_init=False))
+        for endpoint_name in self.config['json']:
+            self.endpoints.append(JSONEndpoint(name=endpoint_name, config_file=self.config_file,
+                                               logger=self.logger, _log_init=False))
+
+    def get_labels(self):
+        """ Get labels from each endpoint, add them together """
+        labels = self.labels.copy()
+        for endpoint in self.endpoints:
+            labels |= endpoint.labels
+        return labels
 
-    def get_metrics(self):
+    async def get_metrics(self, label_filter={}):
         """ Get metrics list from each endpoint, add them together """
-        metric_list = []
+        metric_list = await super().get_metrics(label_filter=label_filter)
+
+        async with TaskGroup() as tg:
+            for endpoint in self.endpoints:
+                if filtered_endpoints := label_filter.get('endpoint', None):
+                    if endpoint.name not in filtered_endpoints:
+                        self.logger.debug("Skipping filtered endpoint: %s", endpoint.name)
+                        continue
+                self.logger.debug("Creating data task for: %s", endpoint.name)
+                tg.create_task(endpoint.get_metrics(label_filter=label_filter))
+
         for endpoint in self.endpoints:
-            endpoint.get_data()
-            metric_list.extend(endpoint.metrics)
-        return metric_list + super().get_metrics()
+            if filtered_endpoints := label_filter.get('endpoint', None):
+                if endpoint.name not in filtered_endpoints:
+                    self.logger.log(5, "Skipping metrics for filtered endpoint: %s", endpoint.name)
+                    continue
+            if metrics := getattr(endpoint, 'metrics', None):
+                metric_list += metrics
+
+        self.logger.debug("Got %d metrics", len(metric_list))
+        self.metrics = metric_list
+        return metric_list
```

### Comparing `json_exporter-0.5.0/src/json_exporter/json_labels.py` & `json_exporter-1.0.0/src/json_exporter/json_labels.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 JSON label class.
 Like Labels, but resolves the value from json data.
 """
 
 from prometheus_exporter import Labels
 
 
+class MissingJSONKey(Exception):
+    def __init__(self, key):
+        super().__init__("JSON path not defined for: %s" % key)
+        self.key = key
+
+
 class JSONLabels(Labels):
     """
     JSON Labels class
 
     Each JSONLabels must be defined with JSON Data and JSON Paths.
     The JSON data is the data used to pull data from.
     The JSON Paths is a dictionary of label names, where the value
@@ -22,19 +28,20 @@
 
         # Create empty labels for each json path
         for name in self.json_paths:
             if name not in self:
                 self[name] = self[name]
 
     def __getitem__(self, name):
-        """
-        Gets an item value based on the json_data and json_paths
-        """
+        """ Gets an item value based on the json_data and json_paths """
         if name not in self.json_paths:
             raise ValueError("JSON path not defined for: %s" % name)
 
         value = self.data.copy()
         for key in self.json_paths[name].split('.'):
-            value = value[key]
+            try:
+                value = value[key]
+            except KeyError as e:
+                raise MissingJSONKey(name) from e
         self.logger.debug("[%s]Resolved JSON data from path: %s -> %a" % (name, self.json_paths[name], value))
         return value
```

### Comparing `json_exporter-0.5.0/src/json_exporter/json_metric.py` & `json_exporter-1.0.0/src/json_exporter/json_metric.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,19 @@
-"""
-JSON prometheus metric class
-"""
-
 from prometheus_exporter import Metric
 
 
 class JSONMetric(Metric):
-    """
-    JSON prometheus metric class.
-    """
+    """ JSON prometheus metric class. """
     def __init__(self, name, json_data, json_path, *args, **kwargs):
         super().__init__(name, *args, **kwargs)
         self.data = json_data
         self.json_path = json_path
 
-    def _get_value(self):
+    def _value(self):
         """ Get value based on json request """
+        if not hasattr(self, 'data'):
+            return
+
         data = self.data.copy()
         for portion in self.json_path.split('.'):
             data = data.get(portion)
         return data
-
-    def __getattribute__(self, name):
-        """ Get value based on json request """
-        if name == 'value' and hasattr(self, 'data'):
-            return self._get_value()
-
-        return super().__getattribute__(name)
```

