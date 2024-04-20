# Comparing `tmp/ml-indie-tools-0.9.8.tar.gz` & `tmp/ml-indie-tools-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-indie-tools-0.9.8.tar", last modified: Sat Nov 18 16:01:35 2023, max compression
+gzip compressed data, was "ml-indie-tools-0.9.9.tar", last modified: Sat Nov 18 16:07:13 2023, max compression
```

## Comparing `ml-indie-tools-0.9.8.tar` & `ml-indie-tools-0.9.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dsc       (1000) dsc       (1000)        0 2023-11-18 16:01:35.184542 ml-indie-tools-0.9.8/
--rw-r--r--   0 dsc       (1000) dsc       (1000)     1075 2023-09-12 21:35:18.000000 ml-indie-tools-0.9.8/LICENSE
--rw-r--r--   0 dsc       (1000) dsc       (1000)    16288 2023-11-18 16:01:35.184542 ml-indie-tools-0.9.8/PKG-INFO
--rw-r--r--   0 dsc       (1000) dsc       (1000)    14761 2023-11-18 09:37:39.000000 ml-indie-tools-0.9.8/README.md
--rw-r--r--   0 dsc       (1000) dsc       (1000)      182 2023-09-12 21:35:18.000000 ml-indie-tools-0.9.8/pyproject.toml
--rw-r--r--   0 dsc       (1000) dsc       (1000)       38 2023-11-18 16:01:35.184542 ml-indie-tools-0.9.8/setup.cfg
--rw-r--r--   0 dsc       (1000) dsc       (1000)      840 2023-11-18 15:59:38.000000 ml-indie-tools-0.9.8/setup.py
-drwxr-xr-x   0 dsc       (1000) dsc       (1000)        0 2023-11-18 16:01:35.184542 ml-indie-tools-0.9.8/src/
-drwxr-xr-x   0 dsc       (1000) dsc       (1000)        0 2023-11-18 16:01:35.184542 ml-indie-tools-0.9.8/src/ml_indie_tools/
--rw-r--r--   0 dsc       (1000) dsc       (1000)    24693 2023-09-12 21:35:18.000000 ml-indie-tools-0.9.8/src/ml_indie_tools/ALU_Dataset.py
--rw-r--r--   0 dsc       (1000) dsc       (1000)     5097 2023-09-12 21:35:18.000000 ml-indie-tools-0.9.8/src/ml_indie_tools/Calibre_Dataset.py
--rw-r--r--   0 dsc       (1000) dsc       (1000)     5164 2023-11-18 15:59:40.000000 ml-indie-tools-0.9.8/src/ml_indie_tools/Folder_Dataset.py
--rw-r--r--   0 dsc       (1000) dsc       (1000)    32596 2023-09-12 21:35:18.000000 ml-indie-tools-0.9.8/src/ml_indie_tools/Gutenberg_Dataset.py
--rw-r--r--   0 dsc       (1000) dsc       (1000)    40407 2023-11-18 09:37:39.000000 ml-indie-tools-0.9.8/src/ml_indie_tools/Text_Dataset.py
--rw-r--r--   0 dsc       (1000) dsc       (1000)        0 2023-09-12 21:35:18.000000 ml-indie-tools-0.9.8/src/ml_indie_tools/__init__.py
--rw-r--r--   0 dsc       (1000) dsc       (1000)    23659 2023-11-18 14:52:14.000000 ml-indie-tools-0.9.8/src/ml_indie_tools/env_tools.py
--rw-r--r--   0 dsc       (1000) dsc       (1000)    22299 2023-09-12 21:35:18.000000 ml-indie-tools-0.9.8/src/ml_indie_tools/keras_custom_layers.py
--rw-r--r--   0 dsc       (1000) dsc       (1000)    14074 2023-09-12 21:35:18.000000 ml-indie-tools-0.9.8/src/ml_indie_tools/pytorch_custom_layers.py
--rw-r--r--   0 dsc       (1000) dsc       (1000)     6073 2023-11-18 09:37:39.000000 ml-indie-tools-0.9.8/src/ml_indie_tools/pytorch_meta_tools.py
--rw-r--r--   0 dsc       (1000) dsc       (1000)    25476 2023-09-12 21:35:18.000000 ml-indie-tools-0.9.8/src/ml_indie_tools/pytorch_tr_compr_layers.py
--rw-r--r--   0 dsc       (1000) dsc       (1000)     3693 2023-09-12 21:35:18.000000 ml-indie-tools-0.9.8/src/ml_indie_tools/tuner.py
-drwxr-xr-x   0 dsc       (1000) dsc       (1000)        0 2023-11-18 16:01:35.184542 ml-indie-tools-0.9.8/src/ml_indie_tools.egg-info/
--rw-r--r--   0 dsc       (1000) dsc       (1000)    16288 2023-11-18 16:01:35.000000 ml-indie-tools-0.9.8/src/ml_indie_tools.egg-info/PKG-INFO
--rw-r--r--   0 dsc       (1000) dsc       (1000)      657 2023-11-18 16:01:35.000000 ml-indie-tools-0.9.8/src/ml_indie_tools.egg-info/SOURCES.txt
--rw-r--r--   0 dsc       (1000) dsc       (1000)        1 2023-11-18 16:01:35.000000 ml-indie-tools-0.9.8/src/ml_indie_tools.egg-info/dependency_links.txt
--rw-r--r--   0 dsc       (1000) dsc       (1000)       15 2023-11-18 16:01:35.000000 ml-indie-tools-0.9.8/src/ml_indie_tools.egg-info/top_level.txt
+drwxr-xr-x   0 dsc       (1000) dsc       (1000)        0 2023-11-18 16:07:13.089137 ml-indie-tools-0.9.9/
+-rw-r--r--   0 dsc       (1000) dsc       (1000)     1075 2023-09-12 21:35:18.000000 ml-indie-tools-0.9.9/LICENSE
+-rw-r--r--   0 dsc       (1000) dsc       (1000)    16288 2023-11-18 16:07:13.089137 ml-indie-tools-0.9.9/PKG-INFO
+-rw-r--r--   0 dsc       (1000) dsc       (1000)    14761 2023-11-18 09:37:39.000000 ml-indie-tools-0.9.9/README.md
+-rw-r--r--   0 dsc       (1000) dsc       (1000)      182 2023-09-12 21:35:18.000000 ml-indie-tools-0.9.9/pyproject.toml
+-rw-r--r--   0 dsc       (1000) dsc       (1000)       38 2023-11-18 16:07:13.089137 ml-indie-tools-0.9.9/setup.cfg
+-rw-r--r--   0 dsc       (1000) dsc       (1000)      840 2023-11-18 16:06:56.000000 ml-indie-tools-0.9.9/setup.py
+drwxr-xr-x   0 dsc       (1000) dsc       (1000)        0 2023-11-18 16:07:13.089137 ml-indie-tools-0.9.9/src/
+drwxr-xr-x   0 dsc       (1000) dsc       (1000)        0 2023-11-18 16:07:13.089137 ml-indie-tools-0.9.9/src/ml_indie_tools/
+-rw-r--r--   0 dsc       (1000) dsc       (1000)    24693 2023-09-12 21:35:18.000000 ml-indie-tools-0.9.9/src/ml_indie_tools/ALU_Dataset.py
+-rw-r--r--   0 dsc       (1000) dsc       (1000)     5097 2023-09-12 21:35:18.000000 ml-indie-tools-0.9.9/src/ml_indie_tools/Calibre_Dataset.py
+-rw-r--r--   0 dsc       (1000) dsc       (1000)     5174 2023-11-18 16:06:51.000000 ml-indie-tools-0.9.9/src/ml_indie_tools/Folder_Dataset.py
+-rw-r--r--   0 dsc       (1000) dsc       (1000)    32596 2023-09-12 21:35:18.000000 ml-indie-tools-0.9.9/src/ml_indie_tools/Gutenberg_Dataset.py
+-rw-r--r--   0 dsc       (1000) dsc       (1000)    40407 2023-11-18 09:37:39.000000 ml-indie-tools-0.9.9/src/ml_indie_tools/Text_Dataset.py
+-rw-r--r--   0 dsc       (1000) dsc       (1000)        0 2023-09-12 21:35:18.000000 ml-indie-tools-0.9.9/src/ml_indie_tools/__init__.py
+-rw-r--r--   0 dsc       (1000) dsc       (1000)    23659 2023-11-18 14:52:14.000000 ml-indie-tools-0.9.9/src/ml_indie_tools/env_tools.py
+-rw-r--r--   0 dsc       (1000) dsc       (1000)    22299 2023-09-12 21:35:18.000000 ml-indie-tools-0.9.9/src/ml_indie_tools/keras_custom_layers.py
+-rw-r--r--   0 dsc       (1000) dsc       (1000)    14074 2023-09-12 21:35:18.000000 ml-indie-tools-0.9.9/src/ml_indie_tools/pytorch_custom_layers.py
+-rw-r--r--   0 dsc       (1000) dsc       (1000)     6073 2023-11-18 09:37:39.000000 ml-indie-tools-0.9.9/src/ml_indie_tools/pytorch_meta_tools.py
+-rw-r--r--   0 dsc       (1000) dsc       (1000)    25476 2023-09-12 21:35:18.000000 ml-indie-tools-0.9.9/src/ml_indie_tools/pytorch_tr_compr_layers.py
+-rw-r--r--   0 dsc       (1000) dsc       (1000)     3693 2023-09-12 21:35:18.000000 ml-indie-tools-0.9.9/src/ml_indie_tools/tuner.py
+drwxr-xr-x   0 dsc       (1000) dsc       (1000)        0 2023-11-18 16:07:13.089137 ml-indie-tools-0.9.9/src/ml_indie_tools.egg-info/
+-rw-r--r--   0 dsc       (1000) dsc       (1000)    16288 2023-11-18 16:07:13.000000 ml-indie-tools-0.9.9/src/ml_indie_tools.egg-info/PKG-INFO
+-rw-r--r--   0 dsc       (1000) dsc       (1000)      657 2023-11-18 16:07:13.000000 ml-indie-tools-0.9.9/src/ml_indie_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 dsc       (1000) dsc       (1000)        1 2023-11-18 16:07:13.000000 ml-indie-tools-0.9.9/src/ml_indie_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 dsc       (1000) dsc       (1000)       15 2023-11-18 16:07:13.000000 ml-indie-tools-0.9.9/src/ml_indie_tools.egg-info/top_level.txt
```

### Comparing `ml-indie-tools-0.9.8/LICENSE` & `ml-indie-tools-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-indie-tools-0.9.8/PKG-INFO` & `ml-indie-tools-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-indie-tools
-Version: 0.9.8
+Version: 0.9.9
 Summary: A collection of tools for low-resource indie machine learning development
 Home-page: https://github.com/domschl/ml-indie-tools
 Author: Dominik Schlösser
 Author-email: dsc@dosc.net
 License: MIT License
         
         Copyright (c) 2021 Dominik Schlösser
```

### Comparing `ml-indie-tools-0.9.8/README.md` & `ml-indie-tools-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `ml-indie-tools-0.9.8/setup.py` & `ml-indie-tools-0.9.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ml-indie-tools",
-    version="0.9.8",
+    version="0.9.9",
     author="Dominik Schlösser",
     author_email="dsc@dosc.net",
     description="A collection of tools for low-resource indie machine learning development",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/domschl/ml-indie-tools",
     project_urls={"Bug Tracker": "https://github.com/domschl/ml-indie-tools/issues"},
```

### Comparing `ml-indie-tools-0.9.8/src/ml_indie_tools/ALU_Dataset.py` & `ml-indie-tools-0.9.9/src/ml_indie_tools/ALU_Dataset.py`

 * *Files identical despite different names*

### Comparing `ml-indie-tools-0.9.8/src/ml_indie_tools/Calibre_Dataset.py` & `ml-indie-tools-0.9.9/src/ml_indie_tools/Calibre_Dataset.py`

 * *Files identical despite different names*

### Comparing `ml-indie-tools-0.9.8/src/ml_indie_tools/Folder_Dataset.py` & `ml-indie-tools-0.9.9/src/ml_indie_tools/Folder_Dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                     }
                     if use_aliases is True:
                         rec["alias"] = f"FL{index}"
 
                     with open(filename, "r", encoding="utf-8") as f:
                         rec["text"] = f.read()
                     self.records += [rec]
-                    index = index + 1
+                    self.index = self.index + 1
                     cur_index = cur_index + 1
         self.log.info(
             f"Loaded {cur_index} records from folder, grand total is now {len(self.records)} records."
         )
         return
 
     def get_records(self):
```

### Comparing `ml-indie-tools-0.9.8/src/ml_indie_tools/Gutenberg_Dataset.py` & `ml-indie-tools-0.9.9/src/ml_indie_tools/Gutenberg_Dataset.py`

 * *Files identical despite different names*

### Comparing `ml-indie-tools-0.9.8/src/ml_indie_tools/Text_Dataset.py` & `ml-indie-tools-0.9.9/src/ml_indie_tools/Text_Dataset.py`

 * *Files identical despite different names*

### Comparing `ml-indie-tools-0.9.8/src/ml_indie_tools/env_tools.py` & `ml-indie-tools-0.9.9/src/ml_indie_tools/env_tools.py`

 * *Files identical despite different names*

### Comparing `ml-indie-tools-0.9.8/src/ml_indie_tools/keras_custom_layers.py` & `ml-indie-tools-0.9.9/src/ml_indie_tools/keras_custom_layers.py`

 * *Files identical despite different names*

### Comparing `ml-indie-tools-0.9.8/src/ml_indie_tools/pytorch_custom_layers.py` & `ml-indie-tools-0.9.9/src/ml_indie_tools/pytorch_custom_layers.py`

 * *Files identical despite different names*

### Comparing `ml-indie-tools-0.9.8/src/ml_indie_tools/pytorch_meta_tools.py` & `ml-indie-tools-0.9.9/src/ml_indie_tools/pytorch_meta_tools.py`

 * *Files identical despite different names*

### Comparing `ml-indie-tools-0.9.8/src/ml_indie_tools/pytorch_tr_compr_layers.py` & `ml-indie-tools-0.9.9/src/ml_indie_tools/pytorch_tr_compr_layers.py`

 * *Files identical despite different names*

### Comparing `ml-indie-tools-0.9.8/src/ml_indie_tools/tuner.py` & `ml-indie-tools-0.9.9/src/ml_indie_tools/tuner.py`

 * *Files identical despite different names*

### Comparing `ml-indie-tools-0.9.8/src/ml_indie_tools.egg-info/PKG-INFO` & `ml-indie-tools-0.9.9/src/ml_indie_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-indie-tools
-Version: 0.9.8
+Version: 0.9.9
 Summary: A collection of tools for low-resource indie machine learning development
 Home-page: https://github.com/domschl/ml-indie-tools
 Author: Dominik Schlösser
 Author-email: dsc@dosc.net
 License: MIT License
         
         Copyright (c) 2021 Dominik Schlösser
```

### Comparing `ml-indie-tools-0.9.8/src/ml_indie_tools.egg-info/SOURCES.txt` & `ml-indie-tools-0.9.9/src/ml_indie_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

