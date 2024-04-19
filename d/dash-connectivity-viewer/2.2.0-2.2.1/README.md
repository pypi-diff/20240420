# Comparing `tmp/dash_connectivity_viewer-2.2.0.tar.gz` & `tmp/dash_connectivity_viewer-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_connectivity_viewer-2.2.0.tar", last modified: Fri Apr 19 01:36:21 2024, max compression
+gzip compressed data, was "dash_connectivity_viewer-2.2.1.tar", last modified: Fri Apr 19 20:22:34 2024, max compression
```

## Comparing `dash_connectivity_viewer-2.2.0.tar` & `dash_connectivity_viewer-2.2.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 01:36:21.221196 dash_connectivity_viewer-2.2.0/
--rw-r--r--   0 caseysm    (501) staff       (20)     1842 2023-05-09 18:49:42.000000 dash_connectivity_viewer-2.2.0/LICENSE.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       71 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.0/MANIFEST.in
--rw-r--r--   0 caseysm    (501) staff       (20)      928 2024-04-19 01:36:21.220889 dash_connectivity_viewer-2.2.0/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)      216 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.0/README.md
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 01:36:21.208639 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/
--rw-r--r--   0 caseysm    (501) staff       (20)       22 2024-04-19 01:36:06.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/__init__.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 01:36:21.212270 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/
--rw-r--r--   0 caseysm    (501) staff       (20)      568 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    28668 2024-04-18 20:23:56.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)     5453 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3461 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py
--rw-r--r--   0 caseysm    (501) staff       (20)     6514 2024-04-16 04:45:20.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py
--rw-r--r--   0 caseysm    (501) staff       (20)       82 2023-03-18 18:57:32.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/external_stylesheets.py
--rw-r--r--   0 caseysm    (501) staff       (20)    22319 2024-04-17 19:43:24.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/layout.py
--rw-r--r--   0 caseysm    (501) staff       (20)     4469 2023-05-24 07:29:35.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 01:36:21.213693 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_table/
--rw-r--r--   0 caseysm    (501) staff       (20)      711 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_table/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    16791 2024-04-18 20:56:02.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_table/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1347 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_table/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)      210 2023-02-08 23:15:09.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_table/ct_utils.py
--rw-r--r--   0 caseysm    (501) staff       (20)    15463 2024-04-18 19:37:35.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_table/layout.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 01:36:21.218172 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/
--rw-r--r--   0 caseysm    (501) staff       (20)       17 2023-04-13 06:43:13.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)     5357 2024-04-19 01:36:01.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     2914 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/dash_url_helper.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 01:36:21.218747 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/data/
--rw-r--r--   0 caseysm    (501) staff       (20)      144 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/data/height_bounds_v1.npy
--rw-r--r--   0 caseysm    (501) staff       (20)      168 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/data/layer_bounds_v1.npy
--rw-r--r--   0 caseysm    (501) staff       (20)    10434 2024-04-17 23:53:01.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/dataframe_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)      294 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/external_stylesheets.py
--rw-r--r--   0 caseysm    (501) staff       (20)    14029 2024-04-16 20:08:15.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/link_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)     6041 2024-04-18 01:08:17.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/lookup_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)    12472 2024-04-17 22:34:42.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/neuron_data_base.py
--rw-r--r--   0 caseysm    (501) staff       (20)     4163 2024-04-18 22:28:25.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/schema_utils.py
--rw-r--r--   0 caseysm    (501) staff       (20)     4020 2024-04-18 20:36:47.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/table_lookup.py
--rw-r--r--   0 caseysm    (501) staff       (20)      762 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/transform_utils.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 01:36:21.220101 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/connectivity_table/
--rw-r--r--   0 caseysm    (501) staff       (20)      591 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/connectivity_table/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    15965 2024-04-18 20:15:50.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/connectivity_table/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)      523 2023-02-08 23:15:09.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/connectivity_table/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     9905 2024-04-18 02:02:07.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/connectivity_table/layout.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 01:36:21.220527 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer.egg-info/
--rw-r--r--   0 caseysm    (501) staff       (20)      928 2024-04-19 01:36:21.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer.egg-info/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)     1990 2024-04-19 01:36:21.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        1 2024-04-19 01:36:21.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      178 2024-04-19 01:36:21.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer.egg-info/requires.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       25 2024-04-19 01:36:21.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer.egg-info/top_level.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      178 2024-04-16 00:28:06.000000 dash_connectivity_viewer-2.2.0/requirements.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       38 2024-04-19 01:36:21.221248 dash_connectivity_viewer-2.2.0/setup.cfg
--rw-r--r--   0 caseysm    (501) staff       (20)     1153 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.0/setup.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 20:22:34.286460 dash_connectivity_viewer-2.2.1/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1842 2023-05-09 18:49:42.000000 dash_connectivity_viewer-2.2.1/LICENSE.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       71 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.1/MANIFEST.in
+-rw-r--r--   0 caseysm    (501) staff       (20)      923 2024-04-19 20:22:34.286196 dash_connectivity_viewer-2.2.1/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)      216 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.1/README.md
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 20:22:34.275348 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/
+-rw-r--r--   0 caseysm    (501) staff       (20)       22 2024-04-19 20:22:24.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/__init__.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 20:22:34.278790 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/
+-rw-r--r--   0 caseysm    (501) staff       (20)      568 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    28668 2024-04-18 20:23:56.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     5453 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3461 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     6514 2024-04-16 04:45:20.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py
+-rw-r--r--   0 caseysm    (501) staff       (20)       82 2023-03-18 18:57:32.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/external_stylesheets.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    22319 2024-04-17 19:43:24.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/layout.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     4469 2023-05-24 07:29:35.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 20:22:34.280293 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_table/
+-rw-r--r--   0 caseysm    (501) staff       (20)      711 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_table/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    16791 2024-04-18 20:56:02.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_table/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     1347 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_table/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      210 2023-02-08 23:15:09.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_table/ct_utils.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    15463 2024-04-18 19:37:35.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_table/layout.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 20:22:34.283914 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/
+-rw-r--r--   0 caseysm    (501) staff       (20)       17 2023-04-13 06:43:13.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     5357 2024-04-19 01:36:01.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     2914 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/dash_url_helper.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 20:22:34.284358 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/data/
+-rw-r--r--   0 caseysm    (501) staff       (20)      144 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/data/height_bounds_v1.npy
+-rw-r--r--   0 caseysm    (501) staff       (20)      168 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/data/layer_bounds_v1.npy
+-rw-r--r--   0 caseysm    (501) staff       (20)    10434 2024-04-17 23:53:01.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/dataframe_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      294 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/external_stylesheets.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    14029 2024-04-16 20:08:15.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/link_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     6041 2024-04-18 01:08:17.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/lookup_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    12472 2024-04-17 22:34:42.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/neuron_data_base.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     4163 2024-04-18 22:28:25.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/schema_utils.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     4020 2024-04-18 20:36:47.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/table_lookup.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      762 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/transform_utils.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 20:22:34.285487 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/connectivity_table/
+-rw-r--r--   0 caseysm    (501) staff       (20)      591 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/connectivity_table/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    15965 2024-04-18 20:15:50.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/connectivity_table/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      523 2023-02-08 23:15:09.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/connectivity_table/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     9905 2024-04-18 02:02:07.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/connectivity_table/layout.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 20:22:34.285840 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer.egg-info/
+-rw-r--r--   0 caseysm    (501) staff       (20)      923 2024-04-19 20:22:34.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)     1990 2024-04-19 20:22:34.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)        1 2024-04-19 20:22:34.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      173 2024-04-19 20:22:34.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer.egg-info/requires.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       25 2024-04-19 20:22:34.000000 dash_connectivity_viewer-2.2.1/dash_connectivity_viewer.egg-info/top_level.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      173 2024-04-19 20:17:56.000000 dash_connectivity_viewer-2.2.1/requirements.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       38 2024-04-19 20:22:34.286516 dash_connectivity_viewer-2.2.1/setup.cfg
+-rw-r--r--   0 caseysm    (501) staff       (20)     1153 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.1/setup.py
```

### Comparing `dash_connectivity_viewer-2.2.0/LICENSE.txt` & `dash_connectivity_viewer-2.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/PKG-INFO` & `dash_connectivity_viewer-2.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dash-connectivity-viewer
-Version: 2.2.0
+Version: 2.2.1
 Summary: Dash connectivity viewer for CAVE data
 Home-page: https://github.com/ceesem/dash-connectivity-viewer
 Author: Casey Schneider-Mizell
 Author-email: caseysm@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: nglui>=2.14.2
+Requires-Dist: nglui>=3
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: seaborn
 Requires-Dist: flask
 Requires-Dist: dash>=2
 Requires-Dist: dash_bootstrap_components>=1
 Requires-Dist: cachetools
```

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/__init__.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/callbacks.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/callbacks.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/config.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/config.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/layout.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/layout.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_table/__init__.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_table/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_table/callbacks.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_table/callbacks.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_table/config.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_table/config.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_table/layout.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/cell_type_table/layout.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/config.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/config.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/dash_url_helper.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/dash_url_helper.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/dataframe_utilities.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/dataframe_utilities.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/link_utilities.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/link_utilities.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/lookup_utilities.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/lookup_utilities.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/neuron_data_base.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/neuron_data_base.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/schema_utils.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/table_lookup.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/table_lookup.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/transform_utils.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/common/transform_utils.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/connectivity_table/__init__.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/connectivity_table/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/connectivity_table/callbacks.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/connectivity_table/callbacks.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/connectivity_table/config.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/connectivity_table/config.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/connectivity_table/layout.py` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer/connectivity_table/layout.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer.egg-info/PKG-INFO` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dash-connectivity-viewer
-Version: 2.2.0
+Version: 2.2.1
 Summary: Dash connectivity viewer for CAVE data
 Home-page: https://github.com/ceesem/dash-connectivity-viewer
 Author: Casey Schneider-Mizell
 Author-email: caseysm@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: nglui>=2.14.2
+Requires-Dist: nglui>=3
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: seaborn
 Requires-Dist: flask
 Requires-Dist: dash>=2
 Requires-Dist: dash_bootstrap_components>=1
 Requires-Dist: cachetools
```

### Comparing `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer.egg-info/SOURCES.txt` & `dash_connectivity_viewer-2.2.1/dash_connectivity_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.0/setup.py` & `dash_connectivity_viewer-2.2.1/setup.py`

 * *Files identical despite different names*

