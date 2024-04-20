# Comparing `tmp/dash_connectivity_viewer-2.2.3.tar.gz` & `tmp/dash_connectivity_viewer-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_connectivity_viewer-2.2.3.tar", last modified: Sat Apr 20 00:24:45 2024, max compression
+gzip compressed data, was "dash_connectivity_viewer-2.2.4.tar", last modified: Sat Apr 20 00:44:18 2024, max compression
```

## Comparing `dash_connectivity_viewer-2.2.3.tar` & `dash_connectivity_viewer-2.2.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-20 00:24:45.382693 dash_connectivity_viewer-2.2.3/
--rw-r--r--   0 caseysm    (501) staff       (20)     1842 2023-05-09 18:49:42.000000 dash_connectivity_viewer-2.2.3/LICENSE.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       71 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.3/MANIFEST.in
--rw-r--r--   0 caseysm    (501) staff       (20)      924 2024-04-20 00:24:45.382400 dash_connectivity_viewer-2.2.3/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)      216 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.3/README.md
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-20 00:24:45.364269 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/
--rw-r--r--   0 caseysm    (501) staff       (20)       22 2024-04-20 00:24:36.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/__init__.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-20 00:24:45.368553 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_connectivity/
--rw-r--r--   0 caseysm    (501) staff       (20)      568 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_connectivity/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    28773 2024-04-19 22:39:26.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_connectivity/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)     5451 2024-04-19 22:05:45.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_connectivity/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3453 2024-04-19 22:05:46.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py
--rw-r--r--   0 caseysm    (501) staff       (20)     6514 2024-04-19 22:05:47.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py
--rw-r--r--   0 caseysm    (501) staff       (20)       82 2024-04-19 22:05:47.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_connectivity/external_stylesheets.py
--rw-r--r--   0 caseysm    (501) staff       (20)    21326 2024-04-19 22:05:48.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_connectivity/layout.py
--rw-r--r--   0 caseysm    (501) staff       (20)     4467 2024-04-19 22:05:49.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-20 00:24:45.370791 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_table/
--rw-r--r--   0 caseysm    (501) staff       (20)      711 2024-04-19 22:05:51.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_table/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    16791 2024-04-19 22:05:52.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_table/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1348 2024-04-19 22:06:29.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_table/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)      210 2024-04-19 22:06:03.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_table/ct_utils.py
--rw-r--r--   0 caseysm    (501) staff       (20)    15432 2024-04-19 22:06:29.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_table/layout.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-20 00:24:45.380021 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/
--rw-r--r--   0 caseysm    (501) staff       (20)       18 2024-04-19 22:06:32.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)     5344 2024-04-20 00:07:24.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     2921 2024-04-19 22:06:34.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/dash_url_helper.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-20 00:24:45.380560 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/data/
--rw-r--r--   0 caseysm    (501) staff       (20)      144 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/data/height_bounds_v1.npy
--rw-r--r--   0 caseysm    (501) staff       (20)      168 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/data/layer_bounds_v1.npy
--rw-r--r--   0 caseysm    (501) staff       (20)    10434 2024-04-19 22:06:33.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/dataframe_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)      294 2024-04-19 22:06:35.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/external_stylesheets.py
--rw-r--r--   0 caseysm    (501) staff       (20)    14029 2024-04-19 22:06:37.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/link_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)     6041 2024-04-19 22:06:36.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/lookup_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)    12569 2024-04-20 00:23:39.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/neuron_data_base.py
--rw-r--r--   0 caseysm    (501) staff       (20)     4163 2024-04-19 22:06:38.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/schema_utils.py
--rw-r--r--   0 caseysm    (501) staff       (20)     4020 2024-04-19 22:06:40.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/table_lookup.py
--rw-r--r--   0 caseysm    (501) staff       (20)      765 2024-04-19 22:06:41.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/transform_utils.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-20 00:24:45.381611 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/connectivity_table/
--rw-r--r--   0 caseysm    (501) staff       (20)      591 2024-04-19 22:06:45.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/connectivity_table/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    15965 2024-04-19 22:06:46.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/connectivity_table/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)      523 2024-04-19 22:06:46.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/connectivity_table/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     9905 2024-04-19 22:06:47.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/connectivity_table/layout.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-20 00:24:45.382016 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer.egg-info/
--rw-r--r--   0 caseysm    (501) staff       (20)      924 2024-04-20 00:24:45.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer.egg-info/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)     1990 2024-04-20 00:24:45.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        1 2024-04-20 00:24:45.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      174 2024-04-20 00:24:45.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer.egg-info/requires.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       25 2024-04-20 00:24:45.000000 dash_connectivity_viewer-2.2.3/dash_connectivity_viewer.egg-info/top_level.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      174 2024-04-19 22:09:12.000000 dash_connectivity_viewer-2.2.3/requirements.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       38 2024-04-20 00:24:45.382742 dash_connectivity_viewer-2.2.3/setup.cfg
--rw-r--r--   0 caseysm    (501) staff       (20)     1153 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.3/setup.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-20 00:44:18.667519 dash_connectivity_viewer-2.2.4/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1842 2023-05-09 18:49:42.000000 dash_connectivity_viewer-2.2.4/LICENSE.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       71 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.4/MANIFEST.in
+-rw-r--r--   0 caseysm    (501) staff       (20)      924 2024-04-20 00:44:18.667262 dash_connectivity_viewer-2.2.4/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)      216 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.4/README.md
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-20 00:44:18.651556 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/
+-rw-r--r--   0 caseysm    (501) staff       (20)       22 2024-04-20 00:41:26.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/__init__.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-20 00:44:18.656331 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_connectivity/
+-rw-r--r--   0 caseysm    (501) staff       (20)      568 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_connectivity/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    28773 2024-04-19 22:39:26.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_connectivity/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     5451 2024-04-19 22:05:45.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_connectivity/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3453 2024-04-19 22:05:46.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     6514 2024-04-19 22:05:47.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py
+-rw-r--r--   0 caseysm    (501) staff       (20)       82 2024-04-19 22:05:47.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_connectivity/external_stylesheets.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    21326 2024-04-19 22:05:48.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_connectivity/layout.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     4467 2024-04-19 22:05:49.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-20 00:44:18.658743 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_table/
+-rw-r--r--   0 caseysm    (501) staff       (20)      711 2024-04-19 22:05:51.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_table/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    16791 2024-04-19 22:05:52.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_table/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     1348 2024-04-19 22:06:29.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_table/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      210 2024-04-19 22:06:03.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_table/ct_utils.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    15432 2024-04-19 22:06:29.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_table/layout.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-20 00:44:18.663692 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/
+-rw-r--r--   0 caseysm    (501) staff       (20)       18 2024-04-19 22:06:32.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     5344 2024-04-20 00:07:24.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     2921 2024-04-19 22:06:34.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/dash_url_helper.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-20 00:44:18.664441 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/data/
+-rw-r--r--   0 caseysm    (501) staff       (20)      144 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/data/height_bounds_v1.npy
+-rw-r--r--   0 caseysm    (501) staff       (20)      168 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/data/layer_bounds_v1.npy
+-rw-r--r--   0 caseysm    (501) staff       (20)    10434 2024-04-19 22:06:33.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/dataframe_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      294 2024-04-19 22:06:35.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/external_stylesheets.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    14029 2024-04-19 22:06:37.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/link_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     6041 2024-04-19 22:06:36.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/lookup_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    12569 2024-04-20 00:23:39.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/neuron_data_base.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     4163 2024-04-19 22:06:38.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/schema_utils.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     4077 2024-04-20 00:40:54.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/table_lookup.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      765 2024-04-19 22:06:41.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/transform_utils.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-20 00:44:18.666389 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/connectivity_table/
+-rw-r--r--   0 caseysm    (501) staff       (20)      591 2024-04-19 22:06:45.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/connectivity_table/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    15965 2024-04-19 22:06:46.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/connectivity_table/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      523 2024-04-19 22:06:46.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/connectivity_table/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     9905 2024-04-19 22:06:47.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/connectivity_table/layout.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-20 00:44:18.666921 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer.egg-info/
+-rw-r--r--   0 caseysm    (501) staff       (20)      924 2024-04-20 00:44:18.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)     1990 2024-04-20 00:44:18.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)        1 2024-04-20 00:44:18.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      174 2024-04-20 00:44:18.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer.egg-info/requires.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       25 2024-04-20 00:44:18.000000 dash_connectivity_viewer-2.2.4/dash_connectivity_viewer.egg-info/top_level.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      174 2024-04-19 22:09:12.000000 dash_connectivity_viewer-2.2.4/requirements.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       38 2024-04-20 00:44:18.667574 dash_connectivity_viewer-2.2.4/setup.cfg
+-rw-r--r--   0 caseysm    (501) staff       (20)     1153 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.4/setup.py
```

### Comparing `dash_connectivity_viewer-2.2.3/LICENSE.txt` & `dash_connectivity_viewer-2.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/PKG-INFO` & `dash_connectivity_viewer-2.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-connectivity-viewer
-Version: 2.2.3
+Version: 2.2.4
 Summary: Dash connectivity viewer for CAVE data
 Home-page: https://github.com/ceesem/dash-connectivity-viewer
 Author: Casey Schneider-Mizell
 Author-email: caseysm@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: nglui>=3
```

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_connectivity/__init__.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_connectivity/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_connectivity/callbacks.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_connectivity/callbacks.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_connectivity/config.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_connectivity/config.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_connectivity/layout.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_connectivity/layout.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_table/__init__.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_table/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_table/callbacks.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_table/callbacks.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_table/config.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_table/config.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/cell_type_table/layout.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/cell_type_table/layout.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/config.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/config.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/dash_url_helper.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/dash_url_helper.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/dataframe_utilities.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/dataframe_utilities.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/link_utilities.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/link_utilities.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/lookup_utilities.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/lookup_utilities.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/neuron_data_base.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/neuron_data_base.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/schema_utils.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/table_lookup.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/table_lookup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,16 @@
         pt, add_cols = get_table_info(table_name, self._client)
         config = RegisterTable(pt, add_cols, config)
         self.config = config
         self._cell_type_bridge_schema = _table_schema(config)
 
         if config.soma_table is None:
             soma_table = self._client.info.get_datastack_info().get("soma_table")
+        else:
+            soma_table = config.soma_table
 
         self._soma_table = soma_table
         self._table_name = table_name
 
         self._data = None
         self._data_resolution = config.data_resolution
```

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/common/transform_utils.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/common/transform_utils.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/connectivity_table/__init__.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/connectivity_table/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/connectivity_table/callbacks.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/connectivity_table/callbacks.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/connectivity_table/config.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/connectivity_table/config.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer/connectivity_table/layout.py` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer/connectivity_table/layout.py`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer.egg-info/PKG-INFO` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-connectivity-viewer
-Version: 2.2.3
+Version: 2.2.4
 Summary: Dash connectivity viewer for CAVE data
 Home-page: https://github.com/ceesem/dash-connectivity-viewer
 Author: Casey Schneider-Mizell
 Author-email: caseysm@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: nglui>=3
```

### Comparing `dash_connectivity_viewer-2.2.3/dash_connectivity_viewer.egg-info/SOURCES.txt` & `dash_connectivity_viewer-2.2.4/dash_connectivity_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash_connectivity_viewer-2.2.3/setup.py` & `dash_connectivity_viewer-2.2.4/setup.py`

 * *Files identical despite different names*

