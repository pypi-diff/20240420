# Comparing `tmp/valor_client-0.21.3.tar.gz` & `tmp/valor_client-0.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valor_client-0.21.3.tar", last modified: Fri Apr 19 17:21:04 2024, max compression
+gzip compressed data, was "valor_client-0.22.0.tar", last modified: Fri Apr 19 18:06:04 2024, max compression
```

## Comparing `valor_client-0.21.3.tar` & `valor_client-0.22.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.637343 valor_client-0.21.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 17:21:00.000000 valor_client-0.21.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-19 17:21:04.637343 valor_client-0.21.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-19 17:21:00.000000 valor_client-0.21.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 17:21:04.637343 valor_client-0.21.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 17:21:00.000000 valor_client-0.21.3/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.629343 valor_client-0.21.3/unit-tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.629343 valor_client-0.21.3/unit-tests/coretypes/
--rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/coretypes/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/coretypes/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/coretypes/test_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.629343 valor_client-0.21.3/unit-tests/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/schemas/test_evaluation_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/schemas/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/schemas/test_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/schemas/test_label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.629343 valor_client-0.21.3/unit-tests/symbolic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.629343 valor_client-0.21.3/unit-tests/symbolic/collections/
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/symbolic/collections/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/symbolic/collections/test_static_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/symbolic/collections/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/symbolic/test_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.633343 valor_client-0.21.3/unit-tests/symbolic/types/
--rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/symbolic/types/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    38063 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/symbolic/types/test_symbolic_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-04-19 17:21:00.000000 valor_client-0.21.3/unit-tests/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.633343 valor_client-0.21.3/valor/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29003 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    53334 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/coretypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/metatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.633343 valor_client-0.21.3/valor/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/schemas/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/schemas/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.633343 valor_client-0.21.3/valor/schemas/symbolic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/schemas/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12738 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/schemas/symbolic/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/schemas/symbolic/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    58388 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/schemas/symbolic/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/type_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-04-19 17:21:00.000000 valor_client-0.21.3/valor/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:21:04.633343 valor_client-0.21.3/valor_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-19 17:21:04.000000 valor_client-0.21.3/valor_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-19 17:21:04.000000 valor_client-0.21.3/valor_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 17:21:04.000000 valor_client-0.21.3/valor_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 17:21:04.000000 valor_client-0.21.3/valor_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 17:21:04.000000 valor_client-0.21.3/valor_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:06:04.851289 valor_client-0.22.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 18:05:56.000000 valor_client-0.22.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-19 18:06:04.851289 valor_client-0.22.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-19 18:05:56.000000 valor_client-0.22.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 18:06:04.851289 valor_client-0.22.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 18:05:56.000000 valor_client-0.22.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:06:04.843289 valor_client-0.22.0/unit-tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-19 18:05:56.000000 valor_client-0.22.0/unit-tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:06:04.843289 valor_client-0.22.0/unit-tests/coretypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-04-19 18:05:56.000000 valor_client-0.22.0/unit-tests/coretypes/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-19 18:05:56.000000 valor_client-0.22.0/unit-tests/coretypes/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-19 18:05:56.000000 valor_client-0.22.0/unit-tests/coretypes/test_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:06:04.843289 valor_client-0.22.0/unit-tests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-19 18:05:56.000000 valor_client-0.22.0/unit-tests/schemas/test_evaluation_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-19 18:05:56.000000 valor_client-0.22.0/unit-tests/schemas/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-19 18:05:56.000000 valor_client-0.22.0/unit-tests/schemas/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-19 18:05:56.000000 valor_client-0.22.0/unit-tests/schemas/test_label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:06:04.843289 valor_client-0.22.0/unit-tests/symbolic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:06:04.843289 valor_client-0.22.0/unit-tests/symbolic/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-19 18:05:56.000000 valor_client-0.22.0/unit-tests/symbolic/collections/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-19 18:05:56.000000 valor_client-0.22.0/unit-tests/symbolic/collections/test_static_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-04-19 18:05:56.000000 valor_client-0.22.0/unit-tests/symbolic/collections/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-19 18:05:56.000000 valor_client-0.22.0/unit-tests/symbolic/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:06:04.843289 valor_client-0.22.0/unit-tests/symbolic/types/
+-rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-04-19 18:05:56.000000 valor_client-0.22.0/unit-tests/symbolic/types/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38063 2024-04-19 18:05:56.000000 valor_client-0.22.0/unit-tests/symbolic/types/test_symbolic_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-19 18:05:56.000000 valor_client-0.22.0/unit-tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-19 18:05:56.000000 valor_client-0.22.0/unit-tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-04-19 18:05:56.000000 valor_client-0.22.0/unit-tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:06:04.847289 valor_client-0.22.0/valor/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-19 18:05:56.000000 valor_client-0.22.0/valor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29003 2024-04-19 18:05:56.000000 valor_client-0.22.0/valor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53627 2024-04-19 18:05:56.000000 valor_client-0.22.0/valor/coretypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-19 18:05:56.000000 valor_client-0.22.0/valor/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-19 18:05:56.000000 valor_client-0.22.0/valor/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-04-19 18:05:56.000000 valor_client-0.22.0/valor/metatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:06:04.847289 valor_client-0.22.0/valor/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-19 18:05:56.000000 valor_client-0.22.0/valor/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-19 18:05:56.000000 valor_client-0.22.0/valor/schemas/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-04-19 18:05:56.000000 valor_client-0.22.0/valor/schemas/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:06:04.847289 valor_client-0.22.0/valor/schemas/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:05:56.000000 valor_client-0.22.0/valor/schemas/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12738 2024-04-19 18:05:56.000000 valor_client-0.22.0/valor/schemas/symbolic/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-19 18:05:56.000000 valor_client-0.22.0/valor/schemas/symbolic/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58388 2024-04-19 18:05:56.000000 valor_client-0.22.0/valor/schemas/symbolic/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-19 18:05:56.000000 valor_client-0.22.0/valor/type_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-04-19 18:05:56.000000 valor_client-0.22.0/valor/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:06:04.847289 valor_client-0.22.0/valor_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-19 18:06:04.000000 valor_client-0.22.0/valor_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-19 18:06:04.000000 valor_client-0.22.0/valor_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:06:04.000000 valor_client-0.22.0/valor_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 18:06:04.000000 valor_client-0.22.0/valor_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 18:06:04.000000 valor_client-0.22.0/valor_client.egg-info/top_level.txt
```

### Comparing `valor_client-0.21.3/LICENSE` & `valor_client-0.22.0/LICENSE`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/PKG-INFO` & `valor_client-0.22.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.21.3
+Version: 0.22.0
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor_client-0.21.3/pyproject.toml` & `valor_client-0.22.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/unit-tests/conftest.py` & `valor_client-0.22.0/unit-tests/conftest.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/unit-tests/coretypes/test_core.py` & `valor_client-0.22.0/unit-tests/coretypes/test_core.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/unit-tests/coretypes/test_evaluation.py` & `valor_client-0.22.0/unit-tests/coretypes/test_evaluation.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,14 +52,15 @@
             ),
         ],
         confusion_matrices=[],
         created_at=datetime.datetime(
             year=2024, month=1, day=1, microsecond=1
         ).strftime("%Y-%m-%dT%H:%M:%S.%fZ"),
         connection=Mock(),
+        meta={},
     ).to_dataframe()
 
     df_str = """                                        value
     evaluation                              1
     type parameters               label
     a    "n/a"                    n/a        0.99
     b    "n/a"                    n/a        0.30
```

### Comparing `valor_client-0.21.3/unit-tests/coretypes/test_filtering.py` & `valor_client-0.22.0/unit-tests/coretypes/test_filtering.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/unit-tests/schemas/test_filters.py` & `valor_client-0.22.0/unit-tests/schemas/test_filters.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/unit-tests/schemas/test_geojson.py` & `valor_client-0.22.0/unit-tests/schemas/test_geojson.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/unit-tests/schemas/test_label.py` & `valor_client-0.22.0/unit-tests/schemas/test_label.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/unit-tests/symbolic/collections/test_dictionary.py` & `valor_client-0.22.0/unit-tests/symbolic/collections/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/unit-tests/symbolic/collections/test_static_collection.py` & `valor_client-0.22.0/unit-tests/symbolic/collections/test_static_collection.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/unit-tests/symbolic/collections/test_structures.py` & `valor_client-0.22.0/unit-tests/symbolic/collections/test_structures.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/unit-tests/symbolic/test_operators.py` & `valor_client-0.22.0/unit-tests/symbolic/test_operators.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/unit-tests/symbolic/types/test_schemas.py` & `valor_client-0.22.0/unit-tests/symbolic/types/test_schemas.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/unit-tests/symbolic/types/test_symbolic_types.py` & `valor_client-0.22.0/unit-tests/symbolic/types/test_symbolic_types.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/unit-tests/test_client.py` & `valor_client-0.22.0/unit-tests/test_client.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/unit-tests/test_viz.py` & `valor_client-0.22.0/unit-tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/valor/__init__.py` & `valor_client-0.22.0/valor/__init__.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/valor/client.py` & `valor_client-0.22.0/valor/client.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/valor/coretypes.py` & `valor_client-0.22.0/valor/coretypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,14 +206,16 @@
             The filter used to select the datums for evaluation.
         status : EvaluationStatus
             The status of the evaluation.
         metrics : List[dict]
             A list of metric dictionaries returned by the job.
         confusion_matrices : List[dict]
             A list of confusion matrix dictionaries returned by the job.
+        meta: dict[str, str | float | dict], optional
+            A dictionary of metadata describing the evaluation run.
         """
         if not connection:
             connection = get_connection()
         self.conn = connection
         self.update(**kwargs)
 
     def update(
@@ -223,14 +225,15 @@
         model_name: str,
         datum_filter: Filter,
         parameters: EvaluationParameters,
         status: EvaluationStatus,
         metrics: List[Dict],
         confusion_matrices: List[Dict],
         created_at: str,
+        meta: dict[str, str | float | dict] | None,
         **kwargs,
     ):
         self.id = id
         self.model_name = model_name
         self.datum_filter = (
             Filter(**datum_filter)
             if isinstance(datum_filter, dict)
@@ -239,14 +242,15 @@
         self.parameters = (
             EvaluationParameters(**parameters)
             if isinstance(parameters, dict)
             else parameters
         )
         self.status = EvaluationStatus(status)
         self.metrics = metrics
+        self.meta = meta
         self.confusion_matrices = confusion_matrices
         self.kwargs = kwargs
         self.ignored_pred_labels: Optional[List[Label]] = None
         self.missing_pred_labels: Optional[List[Label]] = None
         self.created_at = datetime.datetime.strptime(
             created_at, "%Y-%m-%dT%H:%M:%S.%fZ"
         ).replace(tzinfo=datetime.timezone.utc)
@@ -319,14 +323,15 @@
             "id": self.id,
             "model_name": self.model_name,
             "datum_filter": asdict(self.datum_filter),
             "parameters": asdict(self.parameters),
             "status": self.status.value,
             "metrics": self.metrics,
             "confusion_matrices": self.confusion_matrices,
+            "meta": self.meta,
             **self.kwargs,
         }
 
     def to_dataframe(
         self,
         stratify_by: Optional[Tuple[str, str]] = None,
     ):
@@ -926,14 +931,15 @@
             model_names=[self.get_name()],
             datum_filter=datum_filter,
             parameters=EvaluationParameters(
                 task_type=TaskType.CLASSIFICATION,
                 label_map=self._create_label_map(label_map=label_map),
                 compute_pr_curves=compute_pr_curves,
             ),
+            meta={},
         )
 
         # create evaluation
         evaluation = Client(self.conn).evaluate(request)
         if len(evaluation) != 1:
             raise RuntimeError
         return evaluation[0]
@@ -999,14 +1005,15 @@
             pr_curve_iou_threshold=pr_curve_iou_threshold,
         )
         datum_filter = self._format_constraints(datasets, filter_by)
         request = EvaluationRequest(
             model_names=[self.get_name()],
             datum_filter=datum_filter,
             parameters=parameters,
+            meta={},
         )
 
         # create evaluation
         evaluation = Client(self.conn).evaluate(request)
         if len(evaluation) != 1:
             raise RuntimeError
         return evaluation[0]
@@ -1039,14 +1046,15 @@
         request = EvaluationRequest(
             model_names=[self.get_name()],
             datum_filter=datum_filter,
             parameters=EvaluationParameters(
                 task_type=TaskType.SEMANTIC_SEGMENTATION,
                 label_map=self._create_label_map(label_map=label_map),
             ),
+            meta={},
         )
 
         # create evaluation
         evaluation = Client(self.conn).evaluate(request)
         if len(evaluation) != 1:
             raise RuntimeError
         return evaluation[0]
```

### Comparing `valor_client-0.21.3/valor/enums.py` & `valor_client-0.22.0/valor/enums.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/valor/exceptions.py` & `valor_client-0.22.0/valor/exceptions.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/valor/metatypes.py` & `valor_client-0.22.0/valor/metatypes.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/valor/schemas/__init__.py` & `valor_client-0.22.0/valor/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/valor/schemas/evaluation.py` & `valor_client-0.22.0/valor/schemas/evaluation.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,18 +50,21 @@
     ----------
     model_names : List[str]
         The list of models we want to evaluate by name.
     datum_filter : schemas.Filter
         The filter object used to define what the model(s) is evaluating against.
     parameters : EvaluationParameters
         Any parameters that are used to modify an evaluation method.
+    meta: dict[str, str | float | dict], optional
+        Metadata about the evaluation run.
     """
 
     model_names: Union[str, List[str]]
     datum_filter: Filter
     parameters: EvaluationParameters
+    meta: Optional[dict]
 
     def __post_init__(self):
         if isinstance(self.datum_filter, dict):
             self.datum_filter = Filter(**self.datum_filter)
         if isinstance(self.parameters, dict):
             self.parameters = EvaluationParameters(**self.parameters)
```

### Comparing `valor_client-0.21.3/valor/schemas/filters.py` & `valor_client-0.22.0/valor/schemas/filters.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/valor/schemas/symbolic/collections.py` & `valor_client-0.22.0/valor/schemas/symbolic/collections.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/valor/schemas/symbolic/operators.py` & `valor_client-0.22.0/valor/schemas/symbolic/operators.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/valor/schemas/symbolic/types.py` & `valor_client-0.22.0/valor/schemas/symbolic/types.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/valor/type_checks.py` & `valor_client-0.22.0/valor/type_checks.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/valor/viz.py` & `valor_client-0.22.0/valor/viz.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.21.3/valor_client.egg-info/PKG-INFO` & `valor_client-0.22.0/valor_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.21.3
+Version: 0.22.0
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor_client-0.21.3/valor_client.egg-info/SOURCES.txt` & `valor_client-0.22.0/valor_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

