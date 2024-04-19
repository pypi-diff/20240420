# Comparing `tmp/caveclient-5.8.1.tar.gz` & `tmp/caveclient-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caveclient-5.8.1.tar", last modified: Thu Aug  3 22:45:58 2023, max compression
+gzip compressed data, was "caveclient-5.9.0.tar", last modified: Mon Aug 14 19:41:25 2023, max compression
```

## Comparing `caveclient-5.8.1.tar` & `caveclient-5.9.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-08-03 22:45:58.250184 caveclient-5.8.1/
--rw-r--r--   0 caseysm    (501) staff       (20)       24 2022-11-15 00:41:20.000000 caveclient-5.8.1/MANIFEST.in
--rw-r--r--   0 caseysm    (501) staff       (20)      342 2023-08-03 22:45:58.250016 caveclient-5.8.1/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)      537 2023-03-22 21:09:19.000000 caveclient-5.8.1/README.rst
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-08-03 22:45:58.245400 caveclient-5.8.1/caveclient/
--rw-r--r--   0 caseysm    (501) staff       (20)       63 2023-08-03 22:45:45.000000 caveclient-5.8.1/caveclient/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    33307 2023-02-17 19:19:53.000000 caveclient-5.8.1/caveclient/annotationengine.py
--rw-r--r--   0 caseysm    (501) staff       (20)    11864 2023-03-24 05:23:36.000000 caveclient-5.8.1/caveclient/auth.py
--rw-r--r--   0 caseysm    (501) staff       (20)     8125 2023-02-17 19:19:53.000000 caveclient-5.8.1/caveclient/base.py
--rw-r--r--   0 caseysm    (501) staff       (20)    39497 2023-06-22 19:17:19.000000 caveclient-5.8.1/caveclient/chunkedgraph.py
--rw-r--r--   0 caseysm    (501) staff       (20)     2769 2023-03-30 03:58:01.000000 caveclient-5.8.1/caveclient/datastack_lookup.py
--rw-r--r--   0 caseysm    (501) staff       (20)     2784 2022-11-15 00:41:20.000000 caveclient-5.8.1/caveclient/emannotationschemas.py
--rw-r--r--   0 caseysm    (501) staff       (20)    11066 2023-05-12 17:27:56.000000 caveclient-5.8.1/caveclient/endpoints.py
--rw-r--r--   0 caseysm    (501) staff       (20)     2407 2023-06-22 19:17:19.000000 caveclient-5.8.1/caveclient/format_utils.py
--rw-r--r--   0 caseysm    (501) staff       (20)    18573 2023-03-30 03:58:01.000000 caveclient-5.8.1/caveclient/frameworkclient.py
--rw-r--r--   0 caseysm    (501) staff       (20)    16314 2023-06-22 19:17:19.000000 caveclient-5.8.1/caveclient/infoservice.py
--rw-r--r--   0 caseysm    (501) staff       (20)     6256 2022-11-15 00:41:20.000000 caveclient-5.8.1/caveclient/jsonservice.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3943 2023-08-03 20:03:52.000000 caveclient-5.8.1/caveclient/l2cache.py
--rw-r--r--   0 caseysm    (501) staff       (20)    91591 2023-08-03 20:03:52.000000 caveclient-5.8.1/caveclient/materializationengine.py
--rw-r--r--   0 caseysm    (501) staff       (20)      778 2023-06-22 19:17:19.000000 caveclient-5.8.1/caveclient/mytimer.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1519 2022-11-15 00:41:20.000000 caveclient-5.8.1/caveclient/session_config.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-08-03 22:45:58.247316 caveclient-5.8.1/caveclient/tools/
--rw-r--r--   0 caseysm    (501) staff       (20)        0 2022-11-15 00:41:20.000000 caveclient-5.8.1/caveclient/tools/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1153 2022-11-15 00:41:20.000000 caveclient-5.8.1/caveclient/tools/caching.py
--rw-r--r--   0 caseysm    (501) staff       (20)     7893 2023-04-19 21:09:35.000000 caveclient-5.8.1/caveclient/tools/stage.py
--rw-r--r--   0 caseysm    (501) staff       (20)    19421 2023-08-03 22:45:27.000000 caveclient-5.8.1/caveclient/tools/table_manager.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-08-03 22:45:58.246421 caveclient-5.8.1/caveclient.egg-info/
--rw-r--r--   0 caseysm    (501) staff       (20)      342 2023-08-03 22:45:58.000000 caveclient-5.8.1/caveclient.egg-info/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)      904 2023-08-03 22:45:58.000000 caveclient-5.8.1/caveclient.egg-info/SOURCES.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-08-03 22:45:58.000000 caveclient-5.8.1/caveclient.egg-info/dependency_links.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      119 2023-08-03 22:45:58.000000 caveclient-5.8.1/caveclient.egg-info/requires.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       17 2023-08-03 22:45:58.000000 caveclient-5.8.1/caveclient.egg-info/top_level.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      118 2023-06-22 19:17:19.000000 caveclient-5.8.1/requirements.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-08-03 22:45:58.250235 caveclient-5.8.1/setup.cfg
--rw-r--r--   0 caseysm    (501) staff       (20)     1128 2022-11-15 00:41:20.000000 caveclient-5.8.1/setup.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-08-03 22:45:58.249212 caveclient-5.8.1/tests/
--rw-r--r--   0 caseysm    (501) staff       (20)        0 2022-11-15 00:41:20.000000 caveclient-5.8.1/tests/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1471 2023-03-30 03:58:01.000000 caveclient-5.8.1/tests/conftest.py
--rw-r--r--   0 caseysm    (501) staff       (20)     6627 2022-11-15 00:41:20.000000 caveclient-5.8.1/tests/test_annotation.py
--rw-r--r--   0 caseysm    (501) staff       (20)    30468 2022-11-15 00:41:20.000000 caveclient-5.8.1/tests/test_chunkedgraph.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1958 2022-11-15 00:41:20.000000 caveclient-5.8.1/tests/test_infoservice.py
--rw-r--r--   0 caseysm    (501) staff       (20)    18399 2023-02-17 19:19:53.000000 caveclient-5.8.1/tests/test_materialization.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-08-14 19:41:25.820028 caveclient-5.9.0/
+-rw-r--r--   0 forrestc   (503) staff       (20)       24 2020-02-28 17:30:55.000000 caveclient-5.9.0/MANIFEST.in
+-rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-08-14 19:41:25.819714 caveclient-5.9.0/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      537 2023-04-23 20:02:55.000000 caveclient-5.9.0/README.rst
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-08-14 19:41:25.800775 caveclient-5.9.0/caveclient/
+-rw-r--r--   0 forrestc   (503) staff       (20)       63 2023-08-14 19:41:21.000000 caveclient-5.9.0/caveclient/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    33307 2023-02-09 16:57:03.000000 caveclient-5.9.0/caveclient/annotationengine.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    11864 2023-01-27 00:36:02.000000 caveclient-5.9.0/caveclient/auth.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     8346 2023-08-14 19:41:07.000000 caveclient-5.9.0/caveclient/base.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    39497 2023-06-02 20:24:45.000000 caveclient-5.9.0/caveclient/chunkedgraph.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2769 2023-04-23 20:02:55.000000 caveclient-5.9.0/caveclient/datastack_lookup.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2784 2022-12-21 20:12:16.000000 caveclient-5.9.0/caveclient/emannotationschemas.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    11066 2023-04-29 14:05:03.000000 caveclient-5.9.0/caveclient/endpoints.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2407 2023-05-10 16:28:45.000000 caveclient-5.9.0/caveclient/format_utils.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18573 2023-04-23 20:02:55.000000 caveclient-5.9.0/caveclient/frameworkclient.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    16314 2023-05-10 16:28:45.000000 caveclient-5.9.0/caveclient/infoservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6290 2023-08-14 19:41:07.000000 caveclient-5.9.0/caveclient/jsonservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     3943 2023-06-07 19:45:31.000000 caveclient-5.9.0/caveclient/l2cache.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    93283 2023-08-14 19:41:07.000000 caveclient-5.9.0/caveclient/materializationengine.py
+-rw-r--r--   0 forrestc   (503) staff       (20)      778 2023-05-19 14:30:34.000000 caveclient-5.9.0/caveclient/mytimer.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1519 2021-09-20 22:23:45.000000 caveclient-5.9.0/caveclient/session_config.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-08-14 19:41:25.807713 caveclient-5.9.0/caveclient/tools/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-12-21 20:12:16.000000 caveclient-5.9.0/caveclient/tools/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1153 2022-12-21 20:12:16.000000 caveclient-5.9.0/caveclient/tools/caching.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     7893 2022-12-21 20:12:16.000000 caveclient-5.9.0/caveclient/tools/stage.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    19421 2023-08-07 20:07:24.000000 caveclient-5.9.0/caveclient/tools/table_manager.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-08-14 19:41:25.803161 caveclient-5.9.0/caveclient.egg-info/
+-rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-08-14 19:41:25.000000 caveclient-5.9.0/caveclient.egg-info/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      904 2023-08-14 19:41:25.000000 caveclient-5.9.0/caveclient.egg-info/SOURCES.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-08-14 19:41:25.000000 caveclient-5.9.0/caveclient.egg-info/dependency_links.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      119 2023-08-14 19:41:25.000000 caveclient-5.9.0/caveclient.egg-info/requires.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       17 2023-08-14 19:41:25.000000 caveclient-5.9.0/caveclient.egg-info/top_level.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      118 2023-05-10 03:33:26.000000 caveclient-5.9.0/requirements.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       38 2023-08-14 19:41:25.820111 caveclient-5.9.0/setup.cfg
+-rw-r--r--   0 forrestc   (503) staff       (20)     1128 2022-12-21 20:12:16.000000 caveclient-5.9.0/setup.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-08-14 19:41:25.818925 caveclient-5.9.0/tests/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-04-20 22:19:21.000000 caveclient-5.9.0/tests/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1471 2023-04-23 20:02:55.000000 caveclient-5.9.0/tests/conftest.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6627 2022-12-21 20:12:16.000000 caveclient-5.9.0/tests/test_annotation.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    30468 2022-12-21 20:12:16.000000 caveclient-5.9.0/tests/test_chunkedgraph.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1958 2022-12-21 20:12:16.000000 caveclient-5.9.0/tests/test_infoservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18277 2023-08-14 19:41:07.000000 caveclient-5.9.0/tests/test_materialization.py
```

### Comparing `caveclient-5.8.1/README.rst` & `caveclient-5.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/caveclient/annotationengine.py` & `caveclient-5.9.0/caveclient/annotationengine.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/caveclient/auth.py` & `caveclient-5.9.0/caveclient/auth.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/caveclient/base.py` & `caveclient-5.9.0/caveclient/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 import pandas as pd
 
 
 class BaseEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.ndarray) or isinstance(obj, pd.Series):
             return obj.tolist()
+        if isinstance(obj, set):
+            return list(obj)
         if isinstance(obj, np.uint64):
             return int(obj)
         if isinstance(obj, np.int64):
             return int(obj)
         if isinstance(obj, (datetime.datetime, datetime.date)):
             return obj.isoformat()
         return json.JSONEncoder.default(self, obj)
@@ -57,14 +59,19 @@
         if r.status_code == 403:
             if json_data:
                 if "error" in json_data.keys():
                     if json_data["error"] == "missing_tos":
                         webbrowser.open(json_data["data"]["tos_form_url"])
 
     elif 500 <= r.status_code < 600:
+        try:
+            d = json.loads(r.content)
+            reason = d.get("message", reason)
+        except json.decoder.JSONDecodeError:
+            pass
         http_error_msg = "%s Server Error: %s for url: %s content:%s" % (
             r.status_code,
             reason,
             r.url,
             r.content,
         )
```

### Comparing `caveclient-5.8.1/caveclient/chunkedgraph.py` & `caveclient-5.9.0/caveclient/chunkedgraph.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/caveclient/datastack_lookup.py` & `caveclient-5.9.0/caveclient/datastack_lookup.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/caveclient/emannotationschemas.py` & `caveclient-5.9.0/caveclient/emannotationschemas.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/caveclient/endpoints.py` & `caveclient-5.9.0/caveclient/endpoints.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/caveclient/format_utils.py` & `caveclient-5.9.0/caveclient/format_utils.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/caveclient/frameworkclient.py` & `caveclient-5.9.0/caveclient/frameworkclient.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/caveclient/infoservice.py` & `caveclient-5.9.0/caveclient/infoservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/caveclient/jsonservice.py` & `caveclient-5.9.0/caveclient/jsonservice.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .base import (
     ClientBase,
+    BaseEncoder,
     _api_versions,
     _api_endpoints,
     handle_response,
 )
 from .auth import AuthClient
 from .endpoints import (
     jsonservice_common,
@@ -160,15 +161,15 @@
         if state_id is None:
             url = self._endpoints["upload_state"].format_map(url_mapping)
         else:
             url_mapping = self.default_url_mapping
             url_mapping["state_id"] = state_id
             url = self._endpoints["upload_state_w_id"].format_map(url_mapping)
 
-        response = self.session.post(url, data=json.dumps(json_state))
+        response = self.session.post(url, data=json.dumps(json_state, cls=BaseEncoder))
         handle_response(response, as_json=False)
         response_re = re.search(".*\/(\d+)", str(response.content))
         return int(response_re.groups()[0])
 
     def build_neuroglancer_url(self, state_id, ngl_url=None):
         """Build a URL for a Neuroglancer deployment that will automatically retrieve specified state.
         If the datastack is specified, this is prepopulated from the info file field "viewer_site".
```

### Comparing `caveclient-5.8.1/caveclient/l2cache.py` & `caveclient-5.9.0/caveclient/l2cache.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/caveclient/materializationengine.py` & `caveclient-5.9.0/caveclient/materializationengine.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,35 @@
 import logging
 
 logger = logging.getLogger(__name__)
 
 SERVER_KEY = "me_server_address"
 
 
+def deserialize_query_response(response):
+    """Deserialize pyarrow responses"""
+    content_type = response.headers.get("Content-Type")
+    if content_type == "data.arrow":
+        with pa.ipc.open_stream(response.content) as reader:
+            df = reader.read_pandas()
+        return df
+    elif content_type == "x-application/pyarrow":
+        try:
+            return pa.deserialize(response.content)
+        except NameError:
+            (
+                "Deserialization of this request requires an older version of Pyarrow (version 3 works).\
+                Update Materialization Deployment or locally downgrade Pyarrow."
+            )
+    else:
+        raise ValueError(
+            f'Unknown response type: {response.headers.get("Content-Type")}'
+        )
+
+
 def convert_position_columns(df, given_resolution, desired_resolution):
     """function to take a dataframe with x,y,z position columns and convert
     them to the desired resolution from the given resolution
 
     Args:
         df (pd.DataFrame): dataframe to alter
         given_resolution (Iterable[float]): what the given resolution is
@@ -280,21 +301,20 @@
         endpoint_mapping = self.default_url_mapping
         endpoint_mapping["datastack_name"] = datastack_name
         url = self._endpoints["versions"].format_map(endpoint_mapping)
         response = self.session.get(url)
         self.raise_for_status(response)
         return response.json()
 
-
     @property
     def tables(self):
         if self._tables is None:
             self._tables = TableManager(self.fc)
         return self._tables
-    
+
     @property
     def views(self):
         if self._views is None:
             self._views = ViewManager(self.fc)
         return self._views
 
     def get_tables(self, datastack_name=None, version=None):
@@ -478,22 +498,26 @@
         filter_spatial_dict,
         return_pyarrow,
         split_positions,
         offset,
         limit,
         desired_resolution,
         use_view=False,
+        random_sample: float = None,
     ):
         endpoint_mapping = self.default_url_mapping
         endpoint_mapping["datastack_name"] = datastack_name
         endpoint_mapping["version"] = version
         data = {}
         query_args = {}
         query_args["return_pyarrow"] = return_pyarrow
+        query_args["arrow_format"] = return_pyarrow
         query_args["split_positions"] = split_positions
+        if random_sample:
+            query_args["random_sample"] = random_sample
         if len(tables) == 1:
             if use_view:
                 endpoint_mapping["view_name"] = tables[0]
                 url = self._endpoints["view_query"].format_map(endpoint_mapping)
             else:
                 endpoint_mapping["table_name"] = tables[0]
                 url = self._endpoints["simple_query"].format_map(endpoint_mapping)
@@ -531,15 +555,15 @@
                 )
         if limit is not None:
             assert limit > 0
             data["limit"] = limit
         if desired_resolution is not None:
             data["desired_resolution"] = desired_resolution
         if return_pyarrow:
-            encoding = ""
+            encoding = "zstd"
         else:
             encoding = "gzip"
 
         return url, data, query_args, encoding
 
     def _resolve_merge_reference(
         self, merge_reference, table, datastack_name, materialization_version
@@ -587,14 +611,15 @@
         split_positions: bool = False,
         materialization_version: int = None,
         timestamp: datetime = None,
         metadata: bool = True,
         merge_reference: bool = True,
         desired_resolution: Iterable = None,
         get_counts: bool = False,
+        random_sample: float = None,
     ):
         """generic query on materialization tables
 
         Args:
             table: 'str'
 
             filter_in_dict (dict , optional):
@@ -630,14 +655,15 @@
                 If True (and return_df is also True), return table and query metadata in the df.attr dictionary.
             merge_reference: (bool, optional) : toggle to automatically join reference table
                 If True, metadata will be queries and if its a reference table it will perform a join
                 on the reference table to return the rows of that
             desired_resolution: (Iterable[float], Optional) : desired resolution you want all spatial points returned in
                 If None, defaults to one specified in client, if that is None then points are returned
                 as stored in the table and should be in the resolution specified in the table metadata
+            random_sample: (float, optional) : percentage of rows to sample from table (0-100) float.
         Returns:
         pd.DataFrame: a pandas dataframe of results of query
 
         """
         if desired_resolution is None:
             desired_resolution = self.desired_resolution
         if timestamp is not None:
@@ -656,14 +682,15 @@
                     limit=limit,
                     datastack_name=datastack_name,
                     split_positions=split_positions,
                     post_filter=True,
                     metadata=metadata,
                     merge_reference=merge_reference,
                     desired_resolution=desired_resolution,
+                    random_sample=random_sample,
                 )
         if materialization_version is None:
             materialization_version = self.version
         if datastack_name is None:
             datastack_name = self.datastack_name
 
         tables, suffix_map = self._resolve_merge_reference(
@@ -681,31 +708,34 @@
             {table: filter_equal_dict} if filter_equal_dict is not None else None,
             {table: filter_spatial_dict} if filter_spatial_dict is not None else None,
             return_df,
             True,
             offset,
             limit,
             desired_resolution,
+            random_sample=random_sample,
         )
         if get_counts:
             query_args["count"] = True
+
+        headers = {"Content-Type": "application/json", "Accept-Encoding": encoding}
+
         response = self.session.post(
             url,
             data=json.dumps(data, cls=BaseEncoder),
-            headers={"Content-Type": "application/json", "Accept-Encoding": encoding},
+            headers=headers,
             params=query_args,
             stream=~return_df,
         )
         self.raise_for_status(response)
         if return_df:
             with warnings.catch_warnings():
                 warnings.simplefilter(action="ignore", category=FutureWarning)
                 warnings.simplefilter(action="ignore", category=DeprecationWarning)
-                df = pa.deserialize(response.content)
-                df = df.copy()
+                df = deserialize_query_response(response)
                 if desired_resolution is not None:
                     if not response.headers.get("dataframe_resolution", None):
 
                         if len(desired_resolution) != 3:
                             raise ValueError(
                                 "desired resolution needs to be of length 3, for xyz"
                             )
@@ -757,14 +787,15 @@
         suffixes: list = None,
         datastack_name: str = None,
         return_df: bool = True,
         split_positions: bool = False,
         materialization_version: int = None,
         metadata: bool = True,
         desired_resolution: Iterable = None,
+        random_sample: float = None,
     ):
         """generic query on materialization tables
 
          Args:
              tables: list of lists with length 2 or 'str'
                  list of two lists: first entries are table names, second
                                     entries are the columns used for the join
@@ -801,15 +832,15 @@
                  default False, if False data is returned as one column with [x,y,z] array (slower)
              materialization_version (int, optional): version to query.
                  If None defaults to one specified in client.
              metadata: (bool, optional) : toggle to return metadata
                  If True (and return_df is also True), return table and query metadata in the df.attr dictionary.
              desired_resolution (Iterable, optional):
                  What resolution to convert position columns to. Defaults to None will use defaults.
-
+             random_sample: (float, optional) : percentage of rows to sample from table (0-100) float.
         Returns:
              pd.DataFrame: a pandas dataframe of results of query
 
         """
         if materialization_version is None:
             materialization_version = self.version
         if datastack_name is None:
@@ -827,29 +858,30 @@
             filter_equal_dict,
             filter_spatial_dict,
             return_df,
             True,
             offset,
             limit,
             desired_resolution,
+            random_sample=random_sample,
         )
 
         response = self.session.post(
             url,
             data=json.dumps(data, cls=BaseEncoder),
             headers={"Content-Type": "application/json", "Accept-Encoding": encoding},
             params=query_args,
             stream=~return_df,
         )
         self.raise_for_status(response)
         if return_df:
             with warnings.catch_warnings():
                 warnings.simplefilter(action="ignore", category=FutureWarning)
                 warnings.simplefilter(action="ignore", category=DeprecationWarning)
-                df = pa.deserialize(response.content)
+                df = deserialize_query_response(response)
 
             if metadata:
                 attrs = self._assemble_attributes(
                     tables,
                     suffixes=suffixes,
                     desired_resolution=response.headers.get(
                         "dataframe_resolution", desired_resolution
@@ -918,15 +950,15 @@
                 too_old_str = ""
             if len(roots_too_recent) > 0:
                 too_recent_str = f"{roots_too_recent} are too recent, "
             else:
                 too_recent_str = ""
 
             raise ValueError(
-                f"Timestamp incompatible with IDs: {too_old_str}{too_recent_str}use chunkedgraph client to find valid ID(s)"
+                f"Timestamp incompatible with IDs: {too_old_str}{too_recent_str} use chunkedgraph client to find valid ID(s)"
             )
 
         id_mapping = self.cg_client.get_past_ids(
             root_ids, timestamp_past=timestamp_past, timestamp_future=timestamp
         )
         for filter_dict in filters:
             if filter_dict is None:
@@ -1219,16 +1251,15 @@
         if desired_resolution is None:
             desired_resolution = self.desired_resolution
 
         with MyTimeIt("deserialize"):
             with warnings.catch_warnings():
                 warnings.simplefilter(action="ignore", category=FutureWarning)
                 warnings.simplefilter(action="ignore", category=DeprecationWarning)
-                df = pa.deserialize(response.content)
-                df = df.copy()
+                df = deserialize_query_response(response)
                 if desired_resolution is not None:
 
                     if len(desired_resolution) != 3:
                         raise ValueError(
                             "desired resolution needs to be of length 3, for xyz"
                         )
                     vox_res = self.get_table_metadata(
@@ -1280,14 +1311,15 @@
         limit: int = None,
         datastack_name: str = None,
         split_positions: bool = False,
         post_filter: bool = True,
         metadata: bool = True,
         merge_reference: bool = True,
         desired_resolution: Iterable = None,
+        random_sample: float = None,
     ):
         """generic query on materialization tables
 
         Args:
             table: 'str'
             timestamp (datetime.datetime): time to materialize (in utc)
                 pass datetime.datetime.utcnow() for present time
@@ -1325,15 +1357,15 @@
                 If True (and return_df is also True), return table and query metadata in the df.attr dictionary.
             merge_reference: (bool, optional) : toggle to automatically join reference table
                 If True, metadata will be queries and if its a reference table it will perform a join
                 on the reference table to return the rows of that
             desired_resolution: (Iterable[float], Optional) : desired resolution you want all spatial points returned in
                 If None, defaults to one specified in client, if that is None then points are returned
                 as stored in the table and should be in the resolution specified in the table metadata
-
+            random_sample: (float, optional) : percentage of rows to sample from table (0-100) float.
         Returns:
         pd.DataFrame: a pandas dataframe of results of query
 
         """
         timestamp = convert_timestamp(timestamp)
         return_df = True
         if self.cg_client is None:
@@ -1367,14 +1399,15 @@
                             datastack_name=datastack_name,
                             split_positions=split_positions,
                             materialization_version=materialization_version,
                             metadata=metadata,
                             merge_reference=merge_reference,
                             desired_resolution=desired_resolution,
                             return_df=True,
+                            random_sample=random_sample,
                         )
                     else:
                         timestamp_start = ts
             # if none of the available versions are before
             # this timestamp, then we cannot support the query
             if materialization_version is None:
                 raise (
@@ -1428,14 +1461,15 @@
                 if filter_spatial_dict is not None
                 else None,
                 True,
                 True,
                 offset,
                 limit,
                 desired_resolution,
+                random_sample=random_sample,
             )
             logger.debug(f"query_args: {query_args}")
             logger.debug(f"query data: {data}")
         with MyTimeIt("query materialize"):
             response = self.session.post(
                 url,
                 data=json.dumps(data, cls=BaseEncoder),
@@ -1452,16 +1486,15 @@
         if desired_resolution is None:
             desired_resolution = self.desired_resolution
 
         with MyTimeIt("deserialize"):
             with warnings.catch_warnings():
                 warnings.simplefilter(action="ignore", category=FutureWarning)
                 warnings.simplefilter(action="ignore", category=DeprecationWarning)
-                df = pa.deserialize(response.content)
-                df = df.copy()
+                df = deserialize_query_response(response)
                 if desired_resolution is not None:
                     if not response.headers.get("dataframe_resolution", None):
 
                         if len(desired_resolution) != 3:
                             raise ValueError(
                                 "desired resolution needs to be of length 3, for xyz"
                             )
@@ -1873,16 +1906,15 @@
         )
         self.raise_for_status(response)
 
         with MyTimeIt("deserialize"):
             with warnings.catch_warnings():
                 warnings.simplefilter(action="ignore", category=FutureWarning)
                 warnings.simplefilter(action="ignore", category=DeprecationWarning)
-                df = pa.deserialize(response.content)
-                df = df.copy()
+                df = deserialize_query_response(response)
                 if desired_resolution is not None:
                     if not response.headers.get("dataframe_resolution", None):
 
                         if len(desired_resolution) != 3:
                             raise ValueError(
                                 "desired resolution needs to be of length 3, for xyz"
                             )
@@ -2057,14 +2089,15 @@
         return_df: bool = True,
         split_positions: bool = False,
         materialization_version: int = None,
         metadata: bool = True,
         merge_reference: bool = True,
         desired_resolution: Iterable = None,
         get_counts: bool = False,
+        random_sample: float = None,
     ):
         """generic query on a view
 
             Args:
             table: 'str'
 
             filter_in_dict (dict , optional):
@@ -2098,14 +2131,15 @@
                 If True (and return_df is also True), return table and query metadata in the df.attr dictionary.
             merge_reference: (bool, optional) : toggle to automatically join reference table
                 If True, metadata will be queries and if its a reference table it will perform a join
                 on the reference table to return the rows of that
             desired_resolution: (Iterable[float], Optional) : desired resolution you want all spatial points returned in
                 If None, defaults to one specified in client, if that is None then points are returned
                 as stored in the table and should be in the resolution specified in the table metadata
+            random_sample: (float, optional) : if given, will do a tablesample of the table with the given fraction (0-100)
         Returns:
         pd.DataFrame: a pandas dataframe of results of query
         """
 
         if desired_resolution is None:
             desired_resolution = self.desired_resolution
         if materialization_version is None:
@@ -2127,14 +2161,15 @@
             else None,
             return_df,
             True,
             offset,
             limit,
             desired_resolution,
             use_view=True,
+            random_sample=random_sample,
         )
         if get_counts:
             query_args["count"] = True
         response = self.session.post(
             url,
             data=json.dumps(data, cls=BaseEncoder),
             headers={"Content-Type": "application/json", "Accept-Encoding": encoding},
@@ -2142,16 +2177,15 @@
             stream=~return_df,
         )
         self.raise_for_status(response)
         if return_df:
             with warnings.catch_warnings():
                 warnings.simplefilter(action="ignore", category=FutureWarning)
                 warnings.simplefilter(action="ignore", category=DeprecationWarning)
-                df = pa.deserialize(response.content)
-                df = df.copy()
+                df = deserialize_query_response(response)
 
             if metadata:
                 attrs = self._assemble_attributes(
                     [view_name],
                     is_view=True,
                     filters={
                         "inclusive": filter_in_dict,
```

### Comparing `caveclient-5.8.1/caveclient/mytimer.py` & `caveclient-5.9.0/caveclient/mytimer.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/caveclient/session_config.py` & `caveclient-5.9.0/caveclient/session_config.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/caveclient/tools/caching.py` & `caveclient-5.9.0/caveclient/tools/caching.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/caveclient/tools/stage.py` & `caveclient-5.9.0/caveclient/tools/stage.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/caveclient/tools/table_manager.py` & `caveclient-5.9.0/caveclient/tools/table_manager.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/caveclient.egg-info/SOURCES.txt` & `caveclient-5.9.0/caveclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/setup.py` & `caveclient-5.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/tests/conftest.py` & `caveclient-5.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/tests/test_annotation.py` & `caveclient-5.9.0/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/tests/test_chunkedgraph.py` & `caveclient-5.9.0/tests/test_chunkedgraph.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/tests/test_infoservice.py` & `caveclient-5.9.0/tests/test_infoservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.8.1/tests/test_materialization.py` & `caveclient-5.9.0/tests/test_materialization.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import pandas as pd
 import responses
 import pyarrow as pa
 from urllib.parse import urlencode
 from .conftest import test_info, TEST_LOCAL_SERVER, TEST_DATASTACK
 import datetime
 import numpy as np
+from io import BytesIO
 
 
 def test_info_d(myclient):
     info = myclient.info.get_datastack_info()
     assert info == test_info
 
 
@@ -25,14 +26,23 @@
     return match
 
 
 class TestChunkedgraphException(Exception):
     """Error to raise is bad values make it to chunkedgraph"""
 
 
+def serialize_dataframe(df, compression="zstd"):
+    batch = pa.RecordBatch.from_pandas(df)
+    sink = pa.BufferOutputStream()
+    opt = pa.ipc.IpcWriteOptions(compression=compression)
+    with pa.ipc.new_stream(sink, batch.schema, options=opt) as writer:
+        writer.write_batch(batch)
+    return BytesIO(sink.getvalue().to_pybytes()).getvalue()
+
+
 class TestMatclient:
     default_mapping = {
         "me_server_address": TEST_LOCAL_SERVER,
         "cg_server_address": TEST_LOCAL_SERVER,
         "table_id": test_info["segmentation_source"].split("/")[-1],
         "datastack_name": TEST_DATASTACK,
         "table_name": test_info["synapse_table"],
@@ -85,15 +95,19 @@
         responses.add(responses.GET, url=versionurl, json=[1], status=200)
 
         url = self.endpoints["simple_query"].format_map(endpoint_mapping)
         syn_md_url = self.endpoints["metadata"].format_map(endpoint_mapping)
 
         responses.add(responses.GET, url=syn_md_url, json=self.synapse_metadata)
 
-        query_d = {"return_pyarrow": True, "split_positions": True}
+        query_d = {
+            "return_pyarrow": True,
+            "split_positions": True,
+            "arrow_format": True,
+        }
         query_string = urlencode(query_d)
         url = url + "?" + query_string
         correct_query_data = {
             "filter_in_dict": {test_info["synapse_table"]: {"pre_pt_root_id": [500]}},
             "filter_notin_dict": {
                 test_info["synapse_table"]: {"post_pt_root_id": [501]}
             },
@@ -117,32 +131,28 @@
         res = [4, 4, 40]
         xyz = ["_x", "_y", "_z"]
         for col in pos_cols:
             for r, d in zip(res, xyz):
                 cx = col + d
                 df_pos[cx] = df_pos[cx] * r
 
-        context = pa.default_serialization_context()
-        serialized = context.serialize(df)
-
         responses.add(
             responses.POST,
             url=url,
-            body=serialized.to_buffer().to_pybytes(),
-            headers={"content-type": "x-application/pyarrow"},
+            body=serialize_dataframe(df),
+            content_type="data.arrow",
             match=[responses.json_params_matcher(correct_query_data)],
         )
-        context = pa.default_serialization_context()
-        pos_serialized = context.serialize(df_pos)
+
         responses.add(
             responses.POST,
             url=url,
-            body=pos_serialized.to_buffer().to_pybytes(),
+            body=serialize_dataframe(df_pos),
+            content_type="data.arrow",
             headers={
-                "content-type": "x-application/pyarrow",
                 "dataframe_resolution": "1, 1, 1",
             },
             match=[
                 responses.json_params_matcher(
                     correct_query_data_with_desired_resolution
                 )
             ],
@@ -328,50 +338,48 @@
         )
         mocker.patch(
             "caveclient.chunkedgraph.ChunkedGraphClientV1.get_root_timestamps",
             mock_get_root_timestamps,
         )
         df = pd.read_pickle("tests/test_data/live_query_before.pkl")
 
-        context = pa.default_serialization_context()
-        serialized = context.serialize(df)
         correct_query_data = {
             "filter_in_dict": {
                 test_info["synapse_table"]: {"pre_pt_root_id": [100, 103]}
             }
         }
         responses.add(
             responses.POST,
             url=url,
-            body=serialized.to_buffer().to_pybytes(),
-            headers={"content-type": "x-application/pyarrow"},
+            body=serialize_dataframe(df),
+            content_type="data.arrow",
             match=[responses.json_params_matcher(correct_query_data)],
         )
         correct_query_data = {
             "filter_in_dict": {
                 test_info["synapse_table"]: {"post_pt_root_id": [100, 101, 102]}
             }
         }
         responses.add(
             responses.POST,
             url=url,
-            body=serialized.to_buffer().to_pybytes(),
-            headers={"content-type": "x-application/pyarrow"},
+            content_type="data.arrow",
+            body=serialize_dataframe(df),
             match=[responses.json_params_matcher(correct_query_data)],
         )
         correct_query_data = {
             "filter_in_dict": {
                 test_info["synapse_table"]: {"post_pt_root_id": [101, 102]}
             }
         }
         responses.add(
             responses.POST,
             url=url,
-            body=serialized.to_buffer().to_pybytes(),
-            headers={"content-type": "x-application/pyarrow"},
+            body=serialize_dataframe(df),
+            content_type="data.arrow",
             match=[responses.json_params_matcher(correct_query_data)],
         )
 
         dfq = myclient.materialize.live_query(
             test_info["synapse_table"],
             good_time,
             filter_in_dict={"pre_pt_root_id": [201, 103]},
@@ -397,47 +405,49 @@
             filter_equal_dict={"post_pt_root_id": 203},
         )
         dfr = pd.read_pickle("tests/test_data/live_query_after3.pkl")
         assert np.all(dfq.pre_pt_root_id == dfr.pre_pt_root_id)
         assert np.all(dfq.post_pt_root_id == dfr.post_pt_root_id)
 
         df_ct = pd.read_pickle("tests/test_data/cell_types.pkl")
-        context = pa.default_serialization_context()
-        serialized = context.serialize(df_ct)
 
         endpoint_mapping["table_name"] = "cell_types"
         url = self.endpoints["simple_query"].format_map(endpoint_mapping)
-        query_d = {"return_pyarrow": True, "split_positions": True}
+        query_d = {
+            "return_pyarrow": True,
+            "split_positions": True,
+            "arrow_format": True,
+        }
         query_string = urlencode(query_d)
         url = url + "?" + query_string
 
         meta_url = self.endpoints["metadata"].format_map(endpoint_mapping)
         responses.add(responses.GET, url=meta_url, json=self.table_metadata)
 
         correct_query_data = {}
         responses.add(
             responses.POST,
             url=url,
-            body=serialized.to_buffer().to_pybytes(),
-            headers={"content-type": "x-application/pyarrow"},
+            body=serialize_dataframe(df_ct),
+            content_type="data.arrow",
             match=[responses.json_params_matcher(correct_query_data)],
         )
         dfq = myclient.materialize.live_query(
             "cell_types", good_time, split_positions=True
         )
 
         correct_ct = pd.read_pickle("tests/test_data/cell_types_live.pkl")
         assert np.all(correct_ct.pt_root_id == dfq.pt_root_id)
 
         correct_query_data = {"filter_equal_dict": {"cell_types": {"cell_type": "BC"}}}
         responses.add(
             responses.POST,
             url=url,
-            body=serialized.to_buffer().to_pybytes(),
-            headers={"content-type": "x-application/pyarrow"},
+            body=serialize_dataframe(df_ct),
+            content_type="data.arrow",
             match=[responses.json_params_matcher(correct_query_data)],
         )
         dfq = myclient.materialize.live_query(
             "cell_types",
             good_time,
             filter_equal_dict={"cell_type": "BC"},
             split_positions=True,
```

