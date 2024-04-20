# Comparing `tmp/dash_connectivity_viewer-2.2.1.tar.gz` & `tmp/dash_connectivity_viewer-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_connectivity_viewer-2.2.1.tar", last modified: Fri Apr 19 20:22:34 2024, max compression
+gzip compressed data, was "dash_connectivity_viewer-2.2.2.tar", last modified: Fri Apr 19 22:45:27 2024, max compression
```

## Comparing `dash_connectivity_viewer-2.2.1.tar` & `dash_connectivity_viewer-2.2.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 20:22:34.286460 dash_connectivity_viewer-2.2.1/
--rw-r--r--   0 caseysm    (501) staff       (20)     1842 2023-05-09 18:49:42.000000 dash_connectivity_viewer-2.2.1/LICENSE.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       71 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.1/MANIFEST.in
--rw-r--r--   0 caseysm    (501) staff       (20)      923 2024-04-19 20:22:34.286196 dash_connectivity_viewer-2.2.1/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)      216 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.1/README.md
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 20:22:34.275348 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/
--rw-r--r--   0 caseysm    (501) staff       (20)       22 2024-04-19 20:22:24.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/__init__.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 20:22:34.278790 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/
--rw-r--r--   0 caseysm    (501) staff       (20)      568 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    28668 2024-04-18 20:23:56.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)     5453 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3461 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py
--rw-r--r--   0 caseysm    (501) staff       (20)     6514 2024-04-16 04:45:20.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py
--rw-r--r--   0 caseysm    (501) staff       (20)       82 2023-03-18 18:57:32.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/external_stylesheets.py
--rw-r--r--   0 caseysm    (501) staff       (20)    22319 2024-04-17 19:43:24.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/layout.py
--rw-r--r--   0 caseysm    (501) staff       (20)     4469 2023-05-24 07:29:35.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 20:22:34.280293 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_table/
--rw-r--r--   0 caseysm    (501) staff       (20)      711 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_table/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    16791 2024-04-18 20:56:02.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_table/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1347 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_table/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)      210 2023-02-08 23:15:09.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_table/ct_utils.py
--rw-r--r--   0 caseysm    (501) staff       (20)    15463 2024-04-18 19:37:35.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_table/layout.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 20:22:34.283914 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/
--rw-r--r--   0 caseysm    (501) staff       (20)       17 2023-04-13 06:43:13.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)     5357 2024-04-19 01:36:01.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     2914 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/dash_url_helper.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 20:22:34.284358 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/data/
--rw-r--r--   0 caseysm    (501) staff       (20)      144 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/data/height_bounds_v1.npy
--rw-r--r--   0 caseysm    (501) staff       (20)      168 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/data/layer_bounds_v1.npy
--rw-r--r--   0 caseysm    (501) staff       (20)    10434 2024-04-17 23:53:01.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/dataframe_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)      294 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/external_stylesheets.py
--rw-r--r--   0 caseysm    (501) staff       (20)    14029 2024-04-16 20:08:15.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/link_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)     6041 2024-04-18 01:08:17.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/lookup_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)    12472 2024-04-17 22:34:42.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/neuron_data_base.py
--rw-r--r--   0 caseysm    (501) staff       (20)     4163 2024-04-18 22:28:25.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/schema_utils.py
--rw-r--r--   0 caseysm    (501) staff       (20)     4020 2024-04-18 20:36:47.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/table_lookup.py
--rw-r--r--   0 caseysm    (501) staff       (20)      762 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/transform_utils.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 20:22:34.285487 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/connectivity_table/
--rw-r--r--   0 caseysm    (501) staff       (20)      591 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/connectivity_table/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    15965 2024-04-18 20:15:50.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/connectivity_table/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)      523 2023-02-08 23:15:09.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/connectivity_table/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     9905 2024-04-18 02:02:07.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/connectivity_table/layout.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 20:22:34.285840 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer.egg-info/
--rw-r--r--   0 caseysm    (501) staff       (20)      923 2024-04-19 20:22:34.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer.egg-info/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)     1990 2024-04-19 20:22:34.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        1 2024-04-19 20:22:34.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      173 2024-04-19 20:22:34.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer.egg-info/requires.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       25 2024-04-19 20:22:34.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer.egg-info/top_level.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      173 2024-04-19 20:17:56.000000 dash_connectivity_viewer-2.2.1/requirements.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       38 2024-04-19 20:22:34.286516 dash_connectivity_viewer-2.2.1/setup.cfg
--rw-r--r--   0 caseysm    (501) staff       (20)     1153 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.1/setup.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 22:45:27.863309 dash_connectivity_viewer-2.2.2/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1842 2023-05-09 18:49:42.000000 dash_connectivity_viewer-2.2.2/LICENSE.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       71 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.2/MANIFEST.in
+-rw-r--r--   0 caseysm    (501) staff       (20)      924 2024-04-19 22:45:27.863016 dash_connectivity_viewer-2.2.2/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)      216 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.2/README.md
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 22:45:27.848547 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/
+-rw-r--r--   0 caseysm    (501) staff       (20)       22 2024-04-19 22:45:15.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/__init__.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 22:45:27.852495 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_connectivity/
+-rw-r--r--   0 caseysm    (501) staff       (20)      568 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_connectivity/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    28773 2024-04-19 22:39:26.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_connectivity/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     5451 2024-04-19 22:05:45.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_connectivity/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3453 2024-04-19 22:05:46.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     6514 2024-04-19 22:05:47.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py
+-rw-r--r--   0 caseysm    (501) staff       (20)       82 2024-04-19 22:05:47.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_connectivity/external_stylesheets.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    21326 2024-04-19 22:05:48.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_connectivity/layout.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     4467 2024-04-19 22:05:49.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 22:45:27.854349 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_table/
+-rw-r--r--   0 caseysm    (501) staff       (20)      711 2024-04-19 22:05:51.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_table/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    16791 2024-04-19 22:05:52.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_table/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     1348 2024-04-19 22:06:29.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_table/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      210 2024-04-19 22:06:03.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_table/ct_utils.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    15432 2024-04-19 22:06:29.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_table/layout.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 22:45:27.860627 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/
+-rw-r--r--   0 caseysm    (501) staff       (20)       18 2024-04-19 22:06:32.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     5357 2024-04-19 22:06:34.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     2921 2024-04-19 22:06:34.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/dash_url_helper.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 22:45:27.861159 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/data/
+-rw-r--r--   0 caseysm    (501) staff       (20)      144 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/data/height_bounds_v1.npy
+-rw-r--r--   0 caseysm    (501) staff       (20)      168 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/data/layer_bounds_v1.npy
+-rw-r--r--   0 caseysm    (501) staff       (20)    10434 2024-04-19 22:06:33.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/dataframe_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      294 2024-04-19 22:06:35.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/external_stylesheets.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    14029 2024-04-19 22:06:37.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/link_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     6041 2024-04-19 22:06:36.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/lookup_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    12472 2024-04-19 22:06:39.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/neuron_data_base.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     4163 2024-04-19 22:06:38.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/schema_utils.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     4020 2024-04-19 22:06:40.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/table_lookup.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      765 2024-04-19 22:06:41.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/transform_utils.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 22:45:27.862271 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/connectivity_table/
+-rw-r--r--   0 caseysm    (501) staff       (20)      591 2024-04-19 22:06:45.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/connectivity_table/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    15965 2024-04-19 22:06:46.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/connectivity_table/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      523 2024-04-19 22:06:46.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/connectivity_table/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     9905 2024-04-19 22:06:47.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/connectivity_table/layout.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 22:45:27.862677 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer.egg-info/
+-rw-r--r--   0 caseysm    (501) staff       (20)      924 2024-04-19 22:45:27.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)     1990 2024-04-19 22:45:27.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)        1 2024-04-19 22:45:27.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      174 2024-04-19 22:45:27.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer.egg-info/requires.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       25 2024-04-19 22:45:27.000000 dash_connectivity_viewer-2.2.2/dash_connectivity_viewer.egg-info/top_level.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      174 2024-04-19 22:09:12.000000 dash_connectivity_viewer-2.2.2/requirements.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       38 2024-04-19 22:45:27.863360 dash_connectivity_viewer-2.2.2/setup.cfg
+-rw-r--r--   0 caseysm    (501) staff       (20)     1153 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.2/setup.py
```

### Comparing `dash_connectivity_viewer-2.2.1/LICENSE.txt` & `dash_connectivity_viewer-2.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.1/PKG-INFO` & `dash_connectivity_viewer-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-connectivity-viewer
-Version: 2.2.1
+Version: 2.2.2
 Summary: Dash connectivity viewer for CAVE data
 Home-page: https://github.com/ceesem/dash-connectivity-viewer
 Author: Casey Schneider-Mizell
 Author-email: caseysm@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: nglui>=3
@@ -12,15 +12,15 @@
 Requires-Dist: numpy
 Requires-Dist: seaborn
 Requires-Dist: flask
 Requires-Dist: dash>=2
 Requires-Dist: dash_bootstrap_components>=1
 Requires-Dist: cachetools
 Requires-Dist: requests
-Requires-Dist: caveclient>=5.7.0
+Requires-Dist: caveclient>=5.20.0
 Requires-Dist: dfbridge>=0.0.2
 Requires-Dist: plotly>=5
 Requires-Dist: loguru
 Requires-Dist: orjson
 Requires-Dist: standard-transform>=1
 
 # dash-connectivity-viewer
```

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/__init__.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_connectivity/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/callbacks.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_connectivity/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime
 import pytz
 import numpy as np
 from functools import partial
+import traceback
 
 from dash import dcc, html, callback_context
 from dash.dependencies import Input, Output, State
 
 from .config import TypedConnectivityConfig
 from ..common.link_utilities import (
     generate_statebuilder,
@@ -360,14 +361,15 @@
             )
             if version is None:
                 version = client.materialize.version
             info_cache = client.info.info_cache[datastack_name]
             info_cache["global_server"] = client.server_address
 
         except Exception as e:
+            print(traceback.format_exc())
             return (
                 html.Div(str(e)),
                 "danger",
                 "",
                 [],
                 [],
                 "Output",
@@ -513,14 +515,15 @@
             if c.debug:
                 print(f"Failed on datastack {datastack_name}!")
                 print(
                     "\n",
                     info_cache,
                     "\n",
                 )
+                print(traceback.format_exc())
             return (
                 html.Div(str(e)),
                 "danger",
                 "",
                 [],
                 [],
                 "Output",
```

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/config.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_connectivity/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,37 +124,36 @@
             ]
             + self.aggregation_columns
             + [self.num_soma_col]
         )
 
         self.show_plots = config.get("ct_conn_show_plots", True)
         self.show_depth_plots = config.get("ct_conn_show_depth_plots", True)
-        self.null_cell_type_label = config.get('null_cell_type_label', "No Type")
+        self.null_cell_type_label = config.get("null_cell_type_label", "No Type")
 
         # self.layer_bnds = np.load(f"{data_path}/layer_bounds_v1.npy")
         # self.height_bnds = np.load(f"{data_path}/height_bounds_v1.npy")
-        self.height_bnds = config.get('height_bounds', [])
+        self.height_bnds = config.get("height_bounds", [])
         if self.height_bnds is not None:
             self.height_bnds = np.array(self.height_bnds)
-        self.layer_bnds = config.get('layer_bounds', [])
+        self.layer_bnds = config.get("layer_bounds", [])
         if self.layer_bnds is not None:
             self.layer_bnds = np.array(self.layer_bnds)
-        self.layer_labels = config.get('layer_labels', [])
+        self.layer_labels = config.get("layer_labels", [])
 
         if self.layer_bnds is not None and self.height_bnds is not None:
             ticklocs = np.concatenate(
                 [self.height_bnds[0:1], self.layer_bnds, self.height_bnds[1:]]
             )
         else:
             ticklocs = np.array([])
 
         if self.layer_labels is None:
             self.layer_labels = self.layer_bnds.astype(str)
 
-
         dendrite_color = config.get("ct_conn_dendrite_color", (0.894, 0.102, 0.110))
         axon_color = config.get("ct_conn_axon_color", (0.227, 0.459, 0.718))
 
         e_color_palette = config.get("ct_conn_e_palette", "RdPu")
         i_color_palette = config.get("ct_conn_i_palette", "Greens")
         u_color_palette = config.get("ct_conn_u_palette", "Greys")
         base_ind = int(config.get("ct_conn_palette_base", 6))
@@ -165,8 +164,7 @@
             e_color_palette,
             i_color_palette,
             u_color_palette,
             base_ind=base_ind,
             tick_locs=ticklocs,
             tick_labels=["L1", "L2/3", "L4", "L5", "L6", "WM", ""],
         )
-
```

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 from .cortex_plots import *
 
 bg_color = "White"
 plotly_template = "plotly_white"
 
+
 def bar_fig_df(df, config, color_column, width=450, height=350):
     bar = bar_plot_df(df, config, color_column)
 
     fig = go.Figure()
     fig.add_trace(bar)
-        
+
     fig.update_layout(
         autosize=True,
         height=height,
         width=width,
         paper_bgcolor=bg_color,
         template=plotly_template,
         showlegend=False,
         margin=dict(l=20, r=20, t=20, b=20),
     )
 
     return fig
 
 
 def violin_fig(ndat, height=350, width=200):
-
     fig = go.Figure()
 
     violin_post = post_violin_plot(ndat)
     violin_pre = pre_violin_plot(ndat)
     fig.add_trace(violin_post)
     fig.add_trace(violin_pre)
 
@@ -49,14 +49,15 @@
         ticklabelposition="outside bottom",
         range=ndat.config.height_bnds.astype(int)[::-1].tolist(),
         gridcolor="#CCC",
         gridwidth=2,
     )
     return fig
 
+
 def scatter_fig_df(df, config, color_column, width=350, height=350):
     fig = go.Figure()
     scatter = synapse_soma_scatterplot(df, config, color_column)
     fig.add_traces(scatter)
 
     fig.update_layout(
         xaxis_title="Soma Depth",
@@ -88,15 +89,14 @@
         scaleanchor="x",
         scaleratio=1,
     )
     return fig
 
 
 def scatter_fig(ndat, color_column, width=350, height=350):
-
     fig = go.Figure()
     scatter = synapse_soma_scatterplot(
         ndat,
         ndat.config.synapse_depth_column,
         ndat.config.soma_depth_column,
         color_column,
     )
```

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/layout.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_connectivity/layout.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,34 +65,14 @@
                                     style={
                                         "margin-left": "12px",
                                         "font-size": "12px",
                                     },
                                     clearable=False,
                                 )
                             ),
-                            # dbc.Checklist(
-                            #     **create_component_kwargs(
-                            #         state,
-                            #         id_inner="live-query-toggle",
-                            #         options=[
-                            #             {
-                            #                 "label": "Live Query",
-                            #                 "value": 1,
-                            #             },
-                            #         ],
-                            #         value=[
-                            #             1,
-                            #         ],
-                            #         switch=True,
-                            #         style={
-                            #             "bottom-margin": "10px",
-                            #             "font-size": "16px",
-                            #         },
-                            #     )
-                            # ),
                         ],
                         width={"size": 1, "offset": 1},
                         align="center",
                     ),
                     dbc.Col(
                         dbc.Button(
                             children="Submit",
```

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import numpy as np
 from ..common.schema_utils import get_table_info
 from ..common.table_lookup import TableViewer
 from ..common.neuron_data_base import NeuronData
 from ..common.transform_utils import extract_depth, compute_depth_y
 from ..common.config import RegisterTable
 
-ALLOW_COLUMN_TYPES_DISCRETE = ['integer', 'boolean', 'string']
+ALLOW_COLUMN_TYPES_DISCRETE = ["integer", "boolean", "string"]
+
+
 class NeuronDataCortex(NeuronData):
     def __init__(
         self,
         object_id,
         client,
         config,
         value_table=None,
@@ -28,21 +30,23 @@
             id_type=id_type,
             is_live=is_live,
         )
         self.value_table = value_table
         self._value_data = None
         self._value_columns = None
         self._app_name = None
-    
+
     @property
     def aligned_volume(self):
-        return self.client.info.get_datastack_info()['aligned_volume']['name']
+        return self.client.info.get_datastack_info()["aligned_volume"]["name"]
 
     def create_table_viewer(self, root_ids):
-        pt, vals = get_table_info(self.value_table, self.client, allow_types=ALLOW_COLUMN_TYPES_DISCRETE)
+        pt, vals = get_table_info(
+            self.value_table, self.client, allow_types=ALLOW_COLUMN_TYPES_DISCRETE
+        )
         cfg = RegisterTable(pt, vals, self.config)
         return TableViewer(
             self.value_table,
             self.client,
             cfg,
             timestamp=self.timestamp,
             id_query=root_ids,
@@ -84,15 +88,15 @@
         val_df = self.value_data
         if val_df is None:
             return df
         else:
             return df.merge(
                 val_df,
                 on=self.config.root_id_col,
-                how='left',
+                how="left",
             )
 
     def partners_in_plus(self):
         return self._decorate_partner_dataframe(self.partners_in())
 
     def partners_out_plus(self):
         return self._decorate_partner_dataframe(self.partners_out())
@@ -130,10 +134,8 @@
                     syn_df,
                     self.config.synapse_depth_column,
                     self.config.syn_pt_position,
                     self.aligned_volume,
                 )
 
     def soma_depth(self):
-        return compute_depth_y(
-            self.soma_location(), self.aligned_volume
-        )
+        return compute_depth_y(self.soma_location(), self.aligned_volume)
```

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_table/__init__.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_table/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_table/callbacks.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_table/callbacks.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_table/config.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_table/config.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -35,8 +35,8 @@
     def ct_table_columns(self):
         return (
             [
                 self.root_id_col,
             ]
             + self.value_columns
             + self.ct_cell_type_pt_position_split
-        )
+        )
```

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_table/layout.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/cell_type_table/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import DefaultDict
 from dash import html
 from dash import dash_table
 from dash import dcc
 import dash_bootstrap_components as dbc
 import flask
 
 from ..common.dash_url_helper import create_component_kwargs, State
```

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/config.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/config.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/dash_url_helper.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/dash_url_helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,64 +3,66 @@
 import re
 from typing import Dict, Callable, Any
 from urllib.parse import urlparse, parse_qsl, urlencode, quote
 
 import dash
 from dash.dependencies import Input, Output, ALL
 
-_COMPONENT_ID_TYPE = 'url_helper'
+_COMPONENT_ID_TYPE = "url_helper"
 
 """
 definition: {id_inner: {property: your_value}}
 NOTE here we use id_inner, NOT the real id (which is a dict)
 """
 State = Dict[str, Dict[str, Any]]
 
 
-def create_component_kwargs(state: State, id_inner: str, **raw_kwargs) -> Dict[str, Any]:
+def create_component_kwargs(
+    state: State, id_inner: str, **raw_kwargs
+) -> Dict[str, Any]:
     # noinspection PyDictCreation
     kwargs = {**raw_kwargs}
 
     # create "id"
-    kwargs['id'] = {
-        'type': _COMPONENT_ID_TYPE,
-        'id_inner': id_inner,
+    kwargs["id"] = {
+        "type": _COMPONENT_ID_TYPE,
+        "id_inner": id_inner,
     }
 
     # apply default value
     if id_inner in state:
         param_key_dict = state[id_inner]
         kwargs.update(param_key_dict)
 
     return kwargs
 
 
-_ID_PARAM_SEP = '::'
+_ID_PARAM_SEP = "::"
 
 
 def _parse_url_to_state(href: str) -> State:
     parse_result = urlparse(href)
     query_string = parse_qsl(parse_result.query)
 
     state = {}
     for key, value in query_string:
         if _ID_PARAM_SEP in key:
             id, param = key.split(_ID_PARAM_SEP)
         else:
-            id, param = key, 'value'
+            id, param = key, "value"
         try:
             state.setdefault(id, {})[param] = ast.literal_eval(value)
         except SyntaxError:
             state.setdefault(id, {})[param] = value
 
     return state
 
 
 def _param_string(id_inner: str, property: str) -> str:
-    return id_inner if property == 'value' else id_inner + _ID_PARAM_SEP + property
+    return id_inner if property == "value" else id_inner + _ID_PARAM_SEP + property
 
 
 _RE_SINGLE_QUOTED = re.compile("^'|'$")
 
 
 def _myrepr(o: str) -> str:
     """Optional but chrome URL bar hates "'" """
@@ -70,39 +72,39 @@
 
 def setup(app: dash.Dash, page_layout: Callable[[State], Any]):
     """
     NOTE ref: https://github.com/plotly/dash/issues/188
     """
 
     @app.callback(
-        Output('page-layout', 'children'),
-        inputs=[Input('url', 'href')],
+        Output("page-layout", "children"),
+        inputs=[Input("url", "href")],
     )
     def page_load(href: str):
         if not href:
             return []
 
         state = _parse_url_to_state(href)
         return page_layout(state)
 
     @app.callback(
-        Output('url', 'search'),
+        Output("url", "search"),
         # NOTE currently only support property="value"...
-        Input({'type': _COMPONENT_ID_TYPE, 'id_inner': ALL}, 'value'),
+        Input({"type": _COMPONENT_ID_TYPE, "id_inner": ALL}, "value"),
     )
     def update_url_state(values):
         """Updates URL from component values."""
 
         state = {}
 
         # https://dash.plotly.com/pattern-matching-callbacks
         inputs = dash.callback_context.inputs_list[0]
         for input in inputs:
-            id = input['id']
+            id = input["id"]
             assert isinstance(id, Dict)
-            assert id['type'] == _COMPONENT_ID_TYPE
-            id_inner = id['id_inner']
-            state[_param_string(id_inner, input['property'])] = _myrepr(input['value'])
+            assert id["type"] == _COMPONENT_ID_TYPE
+            id_inner = id["id_inner"]
+            state[_param_string(id_inner, input["property"])] = _myrepr(input["value"])
 
         params = urlencode(state, safe="%/:?~#+!$,;'@()*[]\"", quote_via=quote)
 
-        return f'?{params}'
+        return f"?{params}"
```

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/dataframe_utilities.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/dataframe_utilities.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/link_utilities.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/link_utilities.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/lookup_utilities.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/lookup_utilities.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/neuron_data_base.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/neuron_data_base.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/schema_utils.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/table_lookup.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/table_lookup.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/transform_utils.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/common/transform_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from collections import defaultdict
 import standard_transform
 
 transform_lookup = defaultdict(standard_transform.identity_transform)
-transform_lookup['minnie65_phase3'] = standard_transform.minnie_transform_nm()
-transform_lookup['v1dd'] = standard_transform.v1dd_transform_nm()
+transform_lookup["minnie65_phase3"] = standard_transform.minnie_transform_nm()
+transform_lookup["v1dd"] = standard_transform.v1dd_transform_nm()
+
 
 def get_transform(aligned_volume):
     return transform_lookup[aligned_volume]
 
+
 def extract_depth(df, depth_column, position_column, aligned_volume):
     if len(df) == 0:
         df[depth_column] = None
         return df
     tform = get_transform(aligned_volume)
-    df[depth_column] = tform.apply_dataframe(position_column, df, projection='y')
+    df[depth_column] = tform.apply_dataframe(position_column, df, projection="y")
     return df
 
+
 def compute_depth_y(pt, aligned_volume):
     tform = get_transform(aligned_volume)
-    return tform.apply_project('y', pt)
+    return tform.apply_project("y", pt)
```

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/connectivity_table/__init__.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/connectivity_table/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/connectivity_table/callbacks.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/connectivity_table/callbacks.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/connectivity_table/config.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/connectivity_table/config.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/connectivity_table/layout.py` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer/connectivity_table/layout.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer.egg-info/PKG-INFO` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-connectivity-viewer
-Version: 2.2.1
+Version: 2.2.2
 Summary: Dash connectivity viewer for CAVE data
 Home-page: https://github.com/ceesem/dash-connectivity-viewer
 Author: Casey Schneider-Mizell
 Author-email: caseysm@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: nglui>=3
@@ -12,15 +12,15 @@
 Requires-Dist: numpy
 Requires-Dist: seaborn
 Requires-Dist: flask
 Requires-Dist: dash>=2
 Requires-Dist: dash_bootstrap_components>=1
 Requires-Dist: cachetools
 Requires-Dist: requests
-Requires-Dist: caveclient>=5.7.0
+Requires-Dist: caveclient>=5.20.0
 Requires-Dist: dfbridge>=0.0.2
 Requires-Dist: plotly>=5
 Requires-Dist: loguru
 Requires-Dist: orjson
 Requires-Dist: standard-transform>=1
 
 # dash-connectivity-viewer
```

### Comparing `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer.egg-info/SOURCES.txt` & `dash_connectivity_viewer-2.2.2/dash_connectivity_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.1/setup.py` & `dash_connectivity_viewer-2.2.2/setup.py`

 * *Files identical despite different names*

