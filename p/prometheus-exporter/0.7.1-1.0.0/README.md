# Comparing `tmp/prometheus_exporter-0.7.1.tar.gz` & `tmp/prometheus_exporter-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus_exporter-0.7.1.tar", last modified: Wed Dec 20 05:19:34 2023, max compression
+gzip compressed data, was "prometheus_exporter-1.0.0.tar", last modified: Sat Apr 20 00:22:48 2024, max compression
```

## Comparing `prometheus_exporter-0.7.1.tar` & `prometheus_exporter-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2023-12-20 05:19:34.265360 prometheus_exporter-0.7.1/
--rw-r--r--   0 desu      (1000) desu      (1000)    18092 2023-12-18 21:55:59.000000 prometheus_exporter-0.7.1/LICENSE
--rw-r--r--   0 desu      (1000) desu      (1000)      459 2023-12-20 05:19:34.265360 prometheus_exporter-0.7.1/PKG-INFO
--rw-r--r--   0 desu      (1000) desu      (1000)      619 2023-12-20 05:16:58.000000 prometheus_exporter-0.7.1/pyproject.toml
--rw-r--r--   0 desu      (1000) desu      (1000)       38 2023-12-20 05:19:34.265360 prometheus_exporter-0.7.1/setup.cfg
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2023-12-20 05:19:34.264360 prometheus_exporter-0.7.1/src/
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2023-12-20 05:19:34.264360 prometheus_exporter-0.7.1/src/prometheus_exporter/
--rw-r--r--   0 desu      (1000) desu      (1000)      193 2023-12-20 03:24:53.000000 prometheus_exporter-0.7.1/src/prometheus_exporter/__init__.py
--rw-r--r--   0 desu      (1000) desu      (1000)     2129 2023-12-20 05:08:34.000000 prometheus_exporter-0.7.1/src/prometheus_exporter/cached_exporter.py
--rw-r--r--   0 desu      (1000) desu      (1000)     4949 2023-12-20 02:59:02.000000 prometheus_exporter-0.7.1/src/prometheus_exporter/exporter.py
--rw-r--r--   0 desu      (1000) desu      (1000)     1883 2023-12-18 22:00:52.000000 prometheus_exporter-0.7.1/src/prometheus_exporter/labels.py
--rw-r--r--   0 desu      (1000) desu      (1000)     2089 2023-12-18 22:31:29.000000 prometheus_exporter-0.7.1/src/prometheus_exporter/main.py
--rw-r--r--   0 desu      (1000) desu      (1000)     1948 2023-12-20 05:13:31.000000 prometheus_exporter-0.7.1/src/prometheus_exporter/metric.py
--rw-r--r--   0 desu      (1000) desu      (1000)     2664 2023-12-18 21:59:44.000000 prometheus_exporter-0.7.1/src/prometheus_exporter/prometheus_request.py
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2023-12-20 05:19:34.265360 prometheus_exporter-0.7.1/src/prometheus_exporter.egg-info/
--rw-r--r--   0 desu      (1000) desu      (1000)      459 2023-12-20 05:19:34.000000 prometheus_exporter-0.7.1/src/prometheus_exporter.egg-info/PKG-INFO
--rw-r--r--   0 desu      (1000) desu      (1000)      567 2023-12-20 05:19:34.000000 prometheus_exporter-0.7.1/src/prometheus_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 desu      (1000) desu      (1000)        1 2023-12-20 05:19:34.000000 prometheus_exporter-0.7.1/src/prometheus_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 desu      (1000) desu      (1000)       70 2023-12-20 05:19:34.000000 prometheus_exporter-0.7.1/src/prometheus_exporter.egg-info/entry_points.txt
--rw-r--r--   0 desu      (1000) desu      (1000)       14 2023-12-20 05:19:34.000000 prometheus_exporter-0.7.1/src/prometheus_exporter.egg-info/requires.txt
--rw-r--r--   0 desu      (1000) desu      (1000)       20 2023-12-20 05:19:34.000000 prometheus_exporter-0.7.1/src/prometheus_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-20 00:22:48.768008 prometheus_exporter-1.0.0/
+-rw-r--r--   0 desu      (1000) desu      (1000)    18092 2023-12-18 21:55:59.000000 prometheus_exporter-1.0.0/LICENSE
+-rw-r--r--   0 desu      (1000) desu      (1000)     2126 2024-04-20 00:22:48.768008 prometheus_exporter-1.0.0/PKG-INFO
+-rw-r--r--   0 desu      (1000) desu      (1000)      643 2024-04-20 00:19:41.000000 prometheus_exporter-1.0.0/pyproject.toml
+-rw-r--r--   0 desu      (1000) desu      (1000)     1636 2024-01-18 18:02:07.000000 prometheus_exporter-1.0.0/readme.md
+-rw-r--r--   0 desu      (1000) desu      (1000)       38 2024-04-20 00:22:48.768008 prometheus_exporter-1.0.0/setup.cfg
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-20 00:22:48.767008 prometheus_exporter-1.0.0/src/
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-20 00:22:48.767008 prometheus_exporter-1.0.0/src/prometheus_exporter/
+-rw-r--r--   0 desu      (1000) desu      (1000)      565 2024-01-20 18:53:36.000000 prometheus_exporter-1.0.0/src/prometheus_exporter/__init__.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     3211 2024-01-19 23:41:35.000000 prometheus_exporter-1.0.0/src/prometheus_exporter/cached_exporter.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     5054 2024-01-19 03:22:37.000000 prometheus_exporter-1.0.0/src/prometheus_exporter/exporter.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     1398 2024-01-18 17:48:26.000000 prometheus_exporter-1.0.0/src/prometheus_exporter/labels.py
+-rw-r--r--   0 desu      (1000) desu      (1000)      368 2024-01-20 18:50:14.000000 prometheus_exporter-1.0.0/src/prometheus_exporter/main.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     2661 2024-01-19 22:51:05.000000 prometheus_exporter-1.0.0/src/prometheus_exporter/metric.py
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-20 00:22:48.768008 prometheus_exporter-1.0.0/src/prometheus_exporter.egg-info/
+-rw-r--r--   0 desu      (1000) desu      (1000)     2126 2024-04-20 00:22:48.000000 prometheus_exporter-1.0.0/src/prometheus_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 desu      (1000) desu      (1000)      531 2024-04-20 00:22:48.000000 prometheus_exporter-1.0.0/src/prometheus_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 desu      (1000) desu      (1000)        1 2024-04-20 00:22:48.000000 prometheus_exporter-1.0.0/src/prometheus_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 desu      (1000) desu      (1000)       70 2024-04-20 00:22:48.000000 prometheus_exporter-1.0.0/src/prometheus_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 desu      (1000) desu      (1000)       29 2024-04-20 00:22:48.000000 prometheus_exporter-1.0.0/src/prometheus_exporter.egg-info/requires.txt
+-rw-r--r--   0 desu      (1000) desu      (1000)       20 2024-04-20 00:22:48.000000 prometheus_exporter-1.0.0/src/prometheus_exporter.egg-info/top_level.txt
```

### Comparing `prometheus_exporter-0.7.1/LICENSE` & `prometheus_exporter-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus_exporter-0.7.1/pyproject.toml` & `prometheus_exporter-1.0.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prometheus_exporter"
-version = "0.7.1"
+version = "1.0.0"
 authors = [
   { name="Desultory", email="dev@pyl.onl" },
 ]
 description = "A Python library for exporting data as metrics for Prometheus"
 readme = "readme.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "zenlib >= 1.1.1"
+    "zenlib >= 2.0.0",
+    "aiohttp >= 3.9.1"
 ]
 
 [project.scripts]
 prometheus_exporter = "prometheus_exporter.main:main"
```

### Comparing `prometheus_exporter-0.7.1/src/prometheus_exporter/cached_exporter.py` & `prometheus_exporter-1.0.0/src/prometheus_exporter/cached_exporter.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,27 +27,42 @@
                     raise ValueError("cache_life must be a positive integer")
                 self.logger.info("Setting cache_life to: %ds", value)
             super().__setattr__(name, value)
 
         def read_config(self):
             """ Override read_config to add cache_life """
             super().read_config()
-            if 'cache_life' in self.config:
-                self.cache_life = self.config['cache_life']
+            if hasattr(self, 'cache_life'):
+                self.logger.debug("Cache life already set to: %ds", self.cache_life)
+                return
+            self.cache_life = self.config.get('cache_life', 60)
+            self.logger.info("Set cache_life to: %d seconds", self.cache_life)
 
-        def get_metrics(self):
+        async def get_metrics(self, label_filter={}):
             """ Get metrics from the exporter, caching the result. """
+            for key, value in label_filter.items():
+                if key not in self.labels and self.labels[key] != value:
+                    self.logger.debug("Label filter check failed: %s != %s", self.labels, label_filter)
+                    return
             from time import time
-            if not hasattr(self, '_cached_metrics') or time() - self._cache_time >= self.cache_life:
-                self._cache_time = time()
-                self._cached_metrics = super().get_metrics()
+            cache_time = time() - getattr(self, '_cache_time', 0)
+            name = getattr(self, 'name', self.__class__.__name__)
+            self.logger.debug("[%s] Cache time: %d" % (name, cache_time))
+            if not hasattr(self, '_cached_metrics') or cache_time >= self.cache_life:
+                self.metrics = []
+                if new_metrics := await super().get_metrics(label_filter=label_filter):
+                    self.metrics = new_metrics
+                    self._cached_metrics = new_metrics
+                    self._cache_time = time()
+                elif hasattr(self, '_cached_metrics'):
+                    self.logger.warning("[%s] Exporter returned no metrics, returning cached metrics" % name)
+                    self.metrics = self._cached_metrics
             else:
-                self.logger.info("Returning cached metrics.")
-                self.logger.debug("Cached metrics: %s", self._cached_metrics)
-            return self._cached_metrics
+                self.logger.log(5, "[%s] Returning cached metrics: %s" % (name, self._cached_metrics))
+                self.metrics = self._cached_metrics
 
-    CachedExporter.__name__ = cls.__name__
+    CachedExporter.__name__ = f"Cached{cls.__name__}"
     CachedExporter.__module__ = cls.__module__
-    CachedExporter.__qualname__ = cls.__qualname__
+    CachedExporter.__qualname__ = cls.__qualname__.replace(cls.__name__, CachedExporter.__name__)
     CachedExporter.__doc__ = cls.__doc__
 
     return CachedExporter
```

### Comparing `prometheus_exporter-0.7.1/src/prometheus_exporter/exporter.py` & `prometheus_exporter-1.0.0/src/prometheus_exporter/exporter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,118 +1,115 @@
 """
 Basic exporter class for prometheus metrics.
-Runs a ThreadingHTTPServer with a PrometheusRequest handler.
 The PrometheusRequest handler processes requests from Promotheus, by default returns server.export().
 The server.export() method goes through all defined metrics and returns them as a string.
 If a dict is passed to the export method, it will be used to filter by that label.
 """
 
-from http.server import ThreadingHTTPServer
+from aiohttp.web import Application, Response, get
+from asyncio import ensure_future, all_tasks
 from pathlib import Path
+from signal import signal, SIGHUP, SIGINT
 
-from zenlib.logging import loggify
+from zenlib.logging import ClassLogger
 
 from .labels import Labels
 from .metric import Metric
-from .prometheus_request import PrometheusRequest
 
 DEFAULT_IP = '127.0.0.1'
 DEFAULT_PORT = 9999
 
 
-@loggify
-class Exporter(ThreadingHTTPServer):
+class Exporter(ClassLogger):
     """
     Basic prometheus metric exporter class.
-    Extends the ThreadingHTTPServer class.
-    Forces use of the PrometheusRequest RequestHandlerClass.
     Reads a config.toml file to read the server port and ip.
-    If 'ip' and 'port' are passed as kwargs, they will override the config file.
 
     When metrics are added from the config, they are added to self.metrics.
     Labels can be supplied as a dict as an argument, and in the config file.
     """
     def __init__(self, config_file='config.toml', labels=Labels(), *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self.labels = Labels(dict_items=labels, logger=self.logger, _log_init=False)
-        self.metrics = []
         self.config_file = Path(config_file)
+        signal(SIGHUP, lambda *args: self.read_config())
         self.read_config()
+        self.listen_ip = kwargs.get('listen_ip', self.config.get('listen_ip', DEFAULT_IP))
+        self.listen_port = kwargs.get('listen_port', self.config.get('listen_port', DEFAULT_PORT))
 
-        kwargs['RequestHandlerClass'] = PrometheusRequest
-        ip = kwargs.pop('ip') if 'ip' in kwargs else self.config.get('listen_ip', DEFAULT_IP)
-        port = kwargs.pop('port') if 'port' in kwargs else self.config.get('listen_port', DEFAULT_PORT)
-        kwargs['server_address'] = (ip, port)
-
-        self.logger.info("Exporter server address: %s:%d" % (*kwargs['server_address'], ))
-
-        super().__init__(*args, **kwargs)
+        self.app = Application(logger=self.logger)
+        signal(SIGINT, lambda *args: ensure_future(self.app.shutdown()))
+        self.app.add_routes([get('/metrics', self.handle_metrics)])
+        self.app.on_shutdown.append(self.on_shutdown)
 
     def __setattr__(self, name, value):
-        if name == 'labels' and not isinstance(value, Labels):
-            raise ValueError("Labels must be a dict.")
+        if name == 'labels':
+            assert isinstance(value, Labels), "Labels must be a 'Labels' object."
         super().__setattr__(name, value)
 
+    async def on_shutdown(self, app):
+        self.logger.info("Shutting down exporter server")
+        for task in all_tasks():
+            if task.get_coro().__name__ == '_run_app':
+                self.logger.debug("Skipping app task: %s", task)
+                continue
+            self.logger.info("Cancelling task: %s", task)
+            task.cancel()
+
+    def get_labels(self):
+        return self.labels.copy()
+
+    async def get_metrics(self, *args, **kwargs):
+        self.metrics = []
+        self.add_config_metrics(log_bump=10)
+        return self.metrics.copy()
+
     def read_config(self):
         """ Reads the config file defined in self.config_file """
         from tomllib import load
         with open(self.config_file, 'rb') as config:
             self.config = load(config)
 
         self.logger.info("Read config file: %s", self.config_file)
-        self.labels.update(self.config.get('labels', {}))
+        self.labels |= self.config.get('labels', {})
 
-        self.add_config_metrics()
+    def start(self):
+        """ Starts the exporter server. """
+        from aiohttp import web
+        self.logger.info("Exporter server address: %s:%d" % (self.listen_ip, self.listen_port))
+        web.run_app(self.app, host=self.listen_ip, port=self.listen_port)
+
+    async def handle_metrics(self, request, *args, **kwargs):
+        params = dict([p.split('=') for p in request.query_string.split('&')]) if request.query_string else {}
+        self.logger.debug("[%s] Handling metrics request: %s" % (request.remote, request.query_string))
+        response = Response(text=await self.export(params))
+        self.logger.info("[%s (%s)] Sending response: <%d> Length: %d" % (request.remote, request.query_string,
+                                                                          response.status, response.content_length))
+        return response
 
-    def add_config_metrics(self):
+    def add_config_metrics(self, log_bump=0):
         """ Adds all metrics defined in the config to the exporter. """
         for name, values in self.config.get('metrics', {}).items():
-            kwargs = {'metric_type': values.pop('type'), 'labels': self.labels.copy(),
+            kwargs = {'metric_type': values.get('type'), 'labels': self.get_labels(),
                       'logger': self.logger, '_log_init': False}
 
             # Add labels specified under the metric to ones in the exporter
             if labels := values.pop('labels', None):
                 kwargs['labels'].update(labels)
 
-            self.logger.info("Adding metric: %s", name)
+            self.logger.log(20 - log_bump, "Adding metric: %s", name)
             self.metrics.append(Metric(name=name, **kwargs, **values))
 
-    def get_metrics(self):
-        """ Gets all defined metrics. """
-        return [metric for metric in self.metrics]
-
-    def _filter_metrics(self, metrics, label_filter):
-        """ Filters a list of metrics by a label_filter. """
-        filtered_metrics = []
-        for label_name, label_value in label_filter.items():
-            if label_name not in self.labels.global_labels:
-                raise ValueError("Unknown label: %s" % label_name)
-            if label_value not in self.labels.global_labels[label_name]:
-                raise ValueError("[%s] Unknown label value: %s" % (label_name, label_value))
-
-            # If metrics have already been filtered, filter them again so labels act as an "and" filter.
-            if filtered_metrics:
-                metrics = filtered_metrics
-                filtered_metrics = []
-
-            for metric in metrics:
-                if label_name in metric.labels and metric.labels[label_name] == label_value:
-                    filtered_metrics.append(metric)
-
-        return filtered_metrics
-
-    def export(self, label_filter=None):
-        """
-        Go through metrics in self.metrics, turn them into a metric string for prometheus.
-        If a label_filter is passed, only return metrics that match the label_filter.
-        """
-        metrics = self.get_metrics()
-        if label_filter:
-            metrics = self._filter_metrics(metrics, label_filter)
-        return "\n".join([str(metric) for metric in metrics])
-
-    def handle_error(self, request, client_address):
-        """ Handle errors in the request handler. """
-        from sys import exc_info
-        from traceback import format_exception
-        self.logger.warning("[%s:%d] Error in request: %s" % (*client_address, exc_info()[1]))
-        exc = format_exception(*exc_info())
-        self.logger.debug(''.join(exc).replace(r'\n', '\n'))
+    async def export(self, label_filter={}):
+        """ Gets metrics using self.metrics Turns them into a metric string for prometheus. """
+        output = ""
+        for metric in await self.get_metrics(label_filter=label_filter):
+            self.logger.log(5, "Checking metric: %s", metric)
+            if metric.check_labels(label_filter) and metric.value is not None:
+                output += f'{metric}\n'
+
+        self.logger.debug("Exporting metrics:\n%s", output)
+        return output
+
+    def __str__(self):
+        metric_data = '\n'.join([str(metric) for metric in self.metrics])
+        return f"<Exporter host={self.listen_ip}:{self.listen_port} metrics={len(self.metrics)}>\n{metric_data}"
```

### Comparing `prometheus_exporter-0.7.1/src/prometheus_exporter/metric.py` & `prometheus_exporter-1.0.0/src/prometheus_exporter/metric.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,43 +13,60 @@
     GAUGE = 'gauge'
     UNTYPED = 'untyped'
 
 
 @loggify
 class Metric:
     """
-    A class used to represent a prometheus metric.
+    Represents a Prometheus metric.
     Labels can be added to the metric by passing a dictionary as the labels argument.
     The value defaults to 0.
+    The metric type defaults to 'untyped'.
     """
     def __init__(self, name, value=0, metric_type='untyped', help=None, labels=Labels(), *args, **kwargs):
         self.name = name
         self.type = metric_type
         self.help = help
         self.labels = Labels(labels, logger=self.logger, _log_init=False)
         self.value = value
 
+    def check_labels(self, label_filter):
+        """
+        Check if the metric labels match the label filter.
+        label_filter can be a dictionary or a Labels object.
+        """
+        self.logger.log(5, 'Checking labels: %s' % label_filter)
+        for label, value in label_filter.items():
+            if label not in self.labels or self.labels[label] != value:
+                return False
+        return True
+
     def __setattr__(self, name, value):
         """
         Ensure name is not changed after creation.
-        Warn if the name is already in use.
         Turn spaces in the name into underscores.
         Set the metric type based on the MetricTypes enum.
         """
         if name == 'name':
             if hasattr(self, 'name'):
                 raise AttributeError('Cannot change metric name')
             value = value.replace(' ', '_')
         elif name == 'type':
-            value = MetricTypes[value.upper()]
+            value = MetricTypes[value.upper()] if value else MetricTypes.UNTYPED
         elif name == 'value':
             if not isinstance(value, (int, float)):
                 raise TypeError('Value must be an integer or float')
         super().__setattr__(name, value)
 
+    def __getattribute__(self, name):
+        """ Return the result of value() if the method exists, otherwise return the attribute """
+        if name == 'value' and hasattr(self, '_value'):
+            return self._value()
+        return super().__getattribute__(name)
+
     def __str__(self):
         """ Get a string representation of the metric for Prometheus """
         # Start by adding the help text if it exists
         if self.help:
             out_str = f'# HELP {self.name} {self.help}\n'
         else:
             out_str = ''
```

### Comparing `prometheus_exporter-0.7.1/src/prometheus_exporter.egg-info/SOURCES.txt` & `prometheus_exporter-1.0.0/src/prometheus_exporter.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 LICENSE
 pyproject.toml
+readme.md
 src/prometheus_exporter/__init__.py
 src/prometheus_exporter/cached_exporter.py
 src/prometheus_exporter/exporter.py
 src/prometheus_exporter/labels.py
 src/prometheus_exporter/main.py
 src/prometheus_exporter/metric.py
-src/prometheus_exporter/prometheus_request.py
 src/prometheus_exporter.egg-info/PKG-INFO
 src/prometheus_exporter.egg-info/SOURCES.txt
 src/prometheus_exporter.egg-info/dependency_links.txt
 src/prometheus_exporter.egg-info/entry_points.txt
 src/prometheus_exporter.egg-info/requires.txt
 src/prometheus_exporter.egg-info/top_level.txt
```

