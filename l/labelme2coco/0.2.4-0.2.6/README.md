# Comparing `tmp/labelme2coco-0.2.4.tar.gz` & `tmp/labelme2coco-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelme2coco-0.2.4.tar", last modified: Tue Mar 14 14:27:50 2023, max compression
+gzip compressed data, was "labelme2coco-0.2.6.tar", last modified: Sat Apr 20 12:26:09 2024, max compression
```

## Comparing `labelme2coco-0.2.4.tar` & `labelme2coco-0.2.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:27:50.679819 labelme2coco-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-14 14:27:33.000000 labelme2coco-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-03-14 14:27:50.679819 labelme2coco-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-03-14 14:27:33.000000 labelme2coco-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:27:50.679819 labelme2coco-0.2.4/labelme2coco/
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-03-14 14:27:33.000000 labelme2coco-0.2.4/labelme2coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-14 14:27:33.000000 labelme2coco-0.2.4/labelme2coco/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-03-14 14:27:33.000000 labelme2coco-0.2.4/labelme2coco/labelme2coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-03-14 14:27:33.000000 labelme2coco-0.2.4/labelme2coco/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:27:50.679819 labelme2coco-0.2.4/labelme2coco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-03-14 14:27:50.000000 labelme2coco-0.2.4/labelme2coco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-14 14:27:50.000000 labelme2coco-0.2.4/labelme2coco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 14:27:50.000000 labelme2coco-0.2.4/labelme2coco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-14 14:27:50.000000 labelme2coco-0.2.4/labelme2coco.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-14 14:27:50.000000 labelme2coco-0.2.4/labelme2coco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-14 14:27:50.000000 labelme2coco-0.2.4/labelme2coco.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-14 14:27:33.000000 labelme2coco-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-14 14:27:50.683819 labelme2coco-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-03-14 14:27:33.000000 labelme2coco-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:27:50.679819 labelme2coco-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:27:33.000000 labelme2coco-0.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-03-14 14:27:33.000000 labelme2coco-0.2.4/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:09.395553 labelme2coco-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-20 12:26:00.000000 labelme2coco-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-20 12:26:09.395553 labelme2coco-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-20 12:26:00.000000 labelme2coco-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:09.395553 labelme2coco-0.2.6/labelme2coco/
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-20 12:26:00.000000 labelme2coco-0.2.6/labelme2coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-20 12:26:00.000000 labelme2coco-0.2.6/labelme2coco/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-04-20 12:26:00.000000 labelme2coco-0.2.6/labelme2coco/labelme2coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-20 12:26:00.000000 labelme2coco-0.2.6/labelme2coco/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:09.395553 labelme2coco-0.2.6/labelme2coco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-20 12:26:09.000000 labelme2coco-0.2.6/labelme2coco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-20 12:26:09.000000 labelme2coco-0.2.6/labelme2coco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 12:26:09.000000 labelme2coco-0.2.6/labelme2coco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-20 12:26:09.000000 labelme2coco-0.2.6/labelme2coco.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-20 12:26:09.000000 labelme2coco-0.2.6/labelme2coco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-20 12:26:09.000000 labelme2coco-0.2.6/labelme2coco.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-20 12:26:00.000000 labelme2coco-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-20 12:26:09.395553 labelme2coco-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-20 12:26:00.000000 labelme2coco-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:09.395553 labelme2coco-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 12:26:00.000000 labelme2coco-0.2.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-20 12:26:00.000000 labelme2coco-0.2.6/tests/test_unit.py
```

### Comparing `labelme2coco-0.2.4/LICENSE` & `labelme2coco-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `labelme2coco-0.2.4/PKG-INFO` & `labelme2coco-0.2.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: labelme2coco
-Version: 0.2.4
-Summary: Convert labelme annotations into coco format in one step
-Home-page: https://github.com/fcakyon/labelme2coco
-Author: Fatih Cagatay Akyon
-Author-email: 
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
 <h1>
   labelme2coco
 </h1>
 
 <a href="https://pepy.tech/project/labelme2coco"><img src="https://pepy.tech/badge/labelme2coco" alt="downloads"></a>
 <a href="https://badge.fury.io/py/labelme2coco"><img src="https://badge.fury.io/py/labelme2coco.svg" alt="pypi version"></a>
@@ -49,14 +35,18 @@
 labelme2coco path/to/labelme/dir
 ```
 
 ```python
 labelme2coco path/to/labelme/dir --train_split_rate 0.85
 ```
 
+```python
+labelme2coco path/to/labelme/dir --category_id_start 1
+```
+
 ### Advanced Usage
 
 ```python
 # import package
 import labelme2coco
 
 # set directory that contains labelme annotations and image files
@@ -64,16 +54,19 @@
 
 # set export dir
 export_dir = "tests/data/"
 
 # set train split rate
 train_split_rate = 0.85
 
+# set category ID start value
+category_id_start = 1
+
 # convert labelme annotations to coco
-labelme2coco.convert(labelme_folder, export_dir, train_split_rate)
+labelme2coco.convert(labelme_folder, export_dir, train_split_rate, category_id_start=category_id_start)
 ```
 
 ```python
 # import functions
 from labelme2coco import get_coco_from_labelme_folder, save_json
 
 # set labelme training data directory
@@ -81,19 +74,22 @@
 
 # set labelme validation data directory
 labelme_val_folder = "tests/data/labelme_annot"
 
 # set path for coco json to be saved
 export_dir = "tests/data/"
 
+# set category ID start value
+category_id_start = 1
+
 # create train coco object
-train_coco = get_coco_from_labelme_folder(labelme_train_folder)
+train_coco = get_coco_from_labelme_folder(labelme_train_folder, category_id_start=category_id_start)
 
 # export train coco json
 save_json(train_coco.json, export_dir+"train.json")
 
 # create val coco object
-val_coco = get_coco_from_labelme_folder(labelme_val_folder, coco_category_list=train_coco.json_categories)
+val_coco = get_coco_from_labelme_folder(labelme_val_folder, coco_category_list=train_coco.json_categories, category_id_start=category_id_start)
 
 # export val coco json
 save_json(val_coco.json, export_dir+"val.json")
 ```
```

#### html2text {}

```diff
@@ -1,36 +1,34 @@
-Metadata-Version: 2.1 Name: labelme2coco Version: 0.2.4 Summary: Convert
-labelme annotations into coco format in one step Home-page: https://github.com/
-fcakyon/labelme2coco Author: Fatih Cagatay Akyon Author-email: Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
-Description-Content-Type: text/markdown License-File: LICENSE
                           ************ llaabbeellmmee22ccooccoo ************
                          _[_d_o_w_n_l_o_a_d_s_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_c_i_]
                                _[_f_c_a_k_y_o_n_ _t_w_i_t_t_e_r_]
   _**_**_**_ _AA_ _ll_ii_gg_hh_tt_ww_ee_ii_gg_hh_tt_ _pp_aa_cc_kk_aa_gg_ee_ _ff_oo_rr_ _cc_oo_nn_vv_ee_rr_tt_ii_nn_gg_ _yy_oo_uu_rr_ _ll_aa_bb_ee_ll_mm_ee_ _aa_nn_nn_oo_tt_aa_tt_ii_oo_nn_ss_ _ii_nn_tt_oo_ _CC_OO_CC_OO
                          _oo_bb_jj_ee_cc_tt_ _dd_ee_tt_ee_cc_tt_ii_oo_nn_ _ff_oo_rr_mm_aa_tt_.._ _**_**_**
                                _**_**_**_ _[[_tt_ee_aa_ss_ee_rr_]]_ _**_**_**
 ## Convert LabelMe annotations to COCO format in one step [labelme](https://
 github.com/wkentaro/labelme) is a widely used is a graphical image annotation
 tool that supports classification, segmentation, instance segmentation and
 object detection formats. However, widely used frameworks/models such as
 Yolact/Solo, Detectron, MMDetection etc. requires COCO formatted annotations.
 You can use this package to convert labelme annotations to COCO format. ##
 Getting started ### Installation ``` pip install -U labelme2coco ``` ### Basic
 Usage ```python labelme2coco path/to/labelme/dir ``` ```python labelme2coco
-path/to/labelme/dir --train_split_rate 0.85 ``` ### Advanced Usage ```python #
-import package import labelme2coco # set directory that contains labelme
-annotations and image files labelme_folder = "tests/data/labelme_annot" # set
-export dir export_dir = "tests/data/" # set train split rate train_split_rate =
-0.85 # convert labelme annotations to coco labelme2coco.convert(labelme_folder,
-export_dir, train_split_rate) ``` ```python # import functions from
+path/to/labelme/dir --train_split_rate 0.85 ``` ```python labelme2coco path/to/
+labelme/dir --category_id_start 1 ``` ### Advanced Usage ```python # import
+package import labelme2coco # set directory that contains labelme annotations
+and image files labelme_folder = "tests/data/labelme_annot" # set export dir
+export_dir = "tests/data/" # set train split rate train_split_rate = 0.85 # set
+category ID start value category_id_start = 1 # convert labelme annotations to
+coco labelme2coco.convert(labelme_folder, export_dir, train_split_rate,
+category_id_start=category_id_start) ``` ```python # import functions from
 labelme2coco import get_coco_from_labelme_folder, save_json # set labelme
 training data directory labelme_train_folder = "tests/data/labelme_annot" # set
 labelme validation data directory labelme_val_folder = "tests/data/
 labelme_annot" # set path for coco json to be saved export_dir = "tests/data/
-" # create train coco object train_coco = get_coco_from_labelme_folder
-(labelme_train_folder) # export train coco json save_json(train_coco.json,
-export_dir+"train.json") # create val coco object val_coco =
+" # set category ID start value category_id_start = 1 # create train coco
+object train_coco = get_coco_from_labelme_folder(labelme_train_folder,
+category_id_start=category_id_start) # export train coco json save_json
+(train_coco.json, export_dir+"train.json") # create val coco object val_coco =
 get_coco_from_labelme_folder(labelme_val_folder,
-coco_category_list=train_coco.json_categories) # export val coco json save_json
+coco_category_list=train_coco.json_categories,
+category_id_start=category_id_start) # export val coco json save_json
 (val_coco.json, export_dir+"val.json") ```
```

### Comparing `labelme2coco-0.2.4/README.md` & `labelme2coco-0.2.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: labelme2coco
+Version: 0.2.6
+Summary: Convert labelme annotations into coco format in one step
+Home-page: https://github.com/fcakyon/labelme2coco
+Author: Fatih Cagatay Akyon
+Author-email: 
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: sahi>=0.8.19
+Requires-Dist: jsonschema>=2.6.0
+
 <div align="center">
 <h1>
   labelme2coco
 </h1>
 
 <a href="https://pepy.tech/project/labelme2coco"><img src="https://pepy.tech/badge/labelme2coco" alt="downloads"></a>
 <a href="https://badge.fury.io/py/labelme2coco"><img src="https://badge.fury.io/py/labelme2coco.svg" alt="pypi version"></a>
@@ -35,14 +51,18 @@
 labelme2coco path/to/labelme/dir
 ```
 
 ```python
 labelme2coco path/to/labelme/dir --train_split_rate 0.85
 ```
 
+```python
+labelme2coco path/to/labelme/dir --category_id_start 1
+```
+
 ### Advanced Usage
 
 ```python
 # import package
 import labelme2coco
 
 # set directory that contains labelme annotations and image files
@@ -50,16 +70,19 @@
 
 # set export dir
 export_dir = "tests/data/"
 
 # set train split rate
 train_split_rate = 0.85
 
+# set category ID start value
+category_id_start = 1
+
 # convert labelme annotations to coco
-labelme2coco.convert(labelme_folder, export_dir, train_split_rate)
+labelme2coco.convert(labelme_folder, export_dir, train_split_rate, category_id_start=category_id_start)
 ```
 
 ```python
 # import functions
 from labelme2coco import get_coco_from_labelme_folder, save_json
 
 # set labelme training data directory
@@ -67,19 +90,22 @@
 
 # set labelme validation data directory
 labelme_val_folder = "tests/data/labelme_annot"
 
 # set path for coco json to be saved
 export_dir = "tests/data/"
 
+# set category ID start value
+category_id_start = 1
+
 # create train coco object
-train_coco = get_coco_from_labelme_folder(labelme_train_folder)
+train_coco = get_coco_from_labelme_folder(labelme_train_folder, category_id_start=category_id_start)
 
 # export train coco json
 save_json(train_coco.json, export_dir+"train.json")
 
 # create val coco object
-val_coco = get_coco_from_labelme_folder(labelme_val_folder, coco_category_list=train_coco.json_categories)
+val_coco = get_coco_from_labelme_folder(labelme_val_folder, coco_category_list=train_coco.json_categories, category_id_start=category_id_start)
 
 # export val coco json
 save_json(val_coco.json, export_dir+"val.json")
 ```
```

#### html2text {}

```diff
@@ -1,30 +1,41 @@
+Metadata-Version: 2.1 Name: labelme2coco Version: 0.2.6 Summary: Convert
+labelme annotations into coco format in one step Home-page: https://github.com/
+fcakyon/labelme2coco Author: Fatih Cagatay Akyon Author-email: Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+sahi>=0.8.19 Requires-Dist: jsonschema>=2.6.0
                           ************ llaabbeellmmee22ccooccoo ************
                          _[_d_o_w_n_l_o_a_d_s_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_c_i_]
                                _[_f_c_a_k_y_o_n_ _t_w_i_t_t_e_r_]
   _**_**_**_ _AA_ _ll_ii_gg_hh_tt_ww_ee_ii_gg_hh_tt_ _pp_aa_cc_kk_aa_gg_ee_ _ff_oo_rr_ _cc_oo_nn_vv_ee_rr_tt_ii_nn_gg_ _yy_oo_uu_rr_ _ll_aa_bb_ee_ll_mm_ee_ _aa_nn_nn_oo_tt_aa_tt_ii_oo_nn_ss_ _ii_nn_tt_oo_ _CC_OO_CC_OO
                          _oo_bb_jj_ee_cc_tt_ _dd_ee_tt_ee_cc_tt_ii_oo_nn_ _ff_oo_rr_mm_aa_tt_.._ _**_**_**
                                _**_**_**_ _[[_tt_ee_aa_ss_ee_rr_]]_ _**_**_**
 ## Convert LabelMe annotations to COCO format in one step [labelme](https://
 github.com/wkentaro/labelme) is a widely used is a graphical image annotation
 tool that supports classification, segmentation, instance segmentation and
 object detection formats. However, widely used frameworks/models such as
 Yolact/Solo, Detectron, MMDetection etc. requires COCO formatted annotations.
 You can use this package to convert labelme annotations to COCO format. ##
 Getting started ### Installation ``` pip install -U labelme2coco ``` ### Basic
 Usage ```python labelme2coco path/to/labelme/dir ``` ```python labelme2coco
-path/to/labelme/dir --train_split_rate 0.85 ``` ### Advanced Usage ```python #
-import package import labelme2coco # set directory that contains labelme
-annotations and image files labelme_folder = "tests/data/labelme_annot" # set
-export dir export_dir = "tests/data/" # set train split rate train_split_rate =
-0.85 # convert labelme annotations to coco labelme2coco.convert(labelme_folder,
-export_dir, train_split_rate) ``` ```python # import functions from
+path/to/labelme/dir --train_split_rate 0.85 ``` ```python labelme2coco path/to/
+labelme/dir --category_id_start 1 ``` ### Advanced Usage ```python # import
+package import labelme2coco # set directory that contains labelme annotations
+and image files labelme_folder = "tests/data/labelme_annot" # set export dir
+export_dir = "tests/data/" # set train split rate train_split_rate = 0.85 # set
+category ID start value category_id_start = 1 # convert labelme annotations to
+coco labelme2coco.convert(labelme_folder, export_dir, train_split_rate,
+category_id_start=category_id_start) ``` ```python # import functions from
 labelme2coco import get_coco_from_labelme_folder, save_json # set labelme
 training data directory labelme_train_folder = "tests/data/labelme_annot" # set
 labelme validation data directory labelme_val_folder = "tests/data/
 labelme_annot" # set path for coco json to be saved export_dir = "tests/data/
-" # create train coco object train_coco = get_coco_from_labelme_folder
-(labelme_train_folder) # export train coco json save_json(train_coco.json,
-export_dir+"train.json") # create val coco object val_coco =
+" # set category ID start value category_id_start = 1 # create train coco
+object train_coco = get_coco_from_labelme_folder(labelme_train_folder,
+category_id_start=category_id_start) # export train coco json save_json
+(train_coco.json, export_dir+"train.json") # create val coco object val_coco =
 get_coco_from_labelme_folder(labelme_val_folder,
-coco_category_list=train_coco.json_categories) # export val coco json save_json
+coco_category_list=train_coco.json_categories,
+category_id_start=category_id_start) # export val coco json save_json
 (val_coco.json, export_dir+"val.json") ```
```

### Comparing `labelme2coco-0.2.4/labelme2coco/__init__.py` & `labelme2coco-0.2.6/labelme2coco/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import absolute_import
 
-__version__ = "0.2.4"
+__version__ = "0.2.6"
 
 import logging
 import os
 from pathlib import Path
 
 from sahi.utils.file import save_json
 
@@ -21,22 +21,24 @@
 
 
 def convert(
     labelme_folder: str,
     export_dir: str = "runs/labelme2coco/",
     train_split_rate: float = 1,
     skip_labels: List[str] = [],
+    category_id_start: int = 0,
 ):
     """
     Args:
         labelme_folder: folder that contains labelme annotations and image files
         export_dir: path for coco jsons to be exported
         train_split_rate: ration fo train split
+        category_id_start: starting value for category IDs (default: 0)
     """
-    coco = get_coco_from_labelme_folder(labelme_folder, skip_labels=skip_labels)
+    coco = get_coco_from_labelme_folder(labelme_folder, skip_labels=skip_labels, category_id_start=category_id_start)
     if train_split_rate < 1:
         result = coco.split_coco_as_train_val(train_split_rate)
         # export train split
         save_path = str(Path(export_dir) / "train.json")
         save_json(result["train_coco"].json, save_path)
         logger.info(f"Training split in COCO format is exported to {save_path}")
         # export val split
```

### Comparing `labelme2coco-0.2.4/labelme2coco/labelme2coco.py` & `labelme2coco-0.2.6/labelme2coco/labelme2coco.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     def __init__(self):
         raise RuntimeError(
             "Use labelme2coco.convert() or labelme2coco.get_coco_from_labelme_folder() instead."
         )
 
 
 def get_coco_from_labelme_folder(
-    labelme_folder: str, coco_category_list: List = None, skip_labels: List[str] = []
+    labelme_folder: str, coco_category_list: List = None, skip_labels: List[str] = [], category_id_start: int = 0
 ) -> Coco:
     """
     Args:
         labelme_folder: folder that contains labelme annotations and image files
         coco_category_list: start from a predefined coco cateory list
     """
     # get json list
@@ -33,27 +33,29 @@
     if coco_category_list is not None:
         coco.add_categories_from_coco_category_list(coco_category_list)
 
     if len(skip_labels) > 0:
         print(f"Will skip the following annotated labels: {skip_labels}")
 
     # parse labelme annotations
-    category_ind = 0
+    # depending on cli arguments, will start counting at 1
+    category_ind = category_id_start
     for json_path in tqdm(
         labelme_json_list, "Converting labelme annotations to COCO format"
     ):
+        # Taken from https://github.com/fcakyon/labelme2coco/pull/17
         data = load_json(json_path)
         # get image size
-        image_path = str(Path(labelme_folder) / data["imagePath"])
+        image_path = str(Path(json_path).parent / data["imagePath"])
         # use the image sizes provided by labelme (they already account for
         # things such as EXIF orientation)
         width = data["imageWidth"]
         height = data["imageHeight"]
         # init coco image
-        coco_image = CocoImage(file_name=data["imagePath"], height=height, width=width)
+        coco_image = CocoImage(file_name=image_path, height=height, width=width)
         # iterate over annotations
         for shape in data["shapes"]:
             # set category name and id
             category_name = shape["label"]
             if category_name in skip_labels:
                 continue
             category_id = None
@@ -65,31 +67,35 @@
                     category_id = coco_category_id
                     break
             # add category if not present
             if category_id is None:
                 category_id = category_ind
                 coco.add_category(CocoCategory(id=category_id, name=category_name))
                 category_ind += 1
-            
-            # circles and lines to segmentation
+
+            # convert circles, lines, and points to bbox/segmentation
             if shape["shape_type"] == "circle":
-                (cx,cy), (x1,y1) = shape["points"]
-                r = np.linalg.norm(np.array([x1-cx,y1-cy]))
-                angles = np.linspace(0,2*np.pi,50*(int(r)+1))
+                (cx, cy), (x1, y1) = shape["points"]
+                r = np.linalg.norm(np.array([x1 - cx, y1 - cy]))
+                angles = np.linspace(0, 2 * np.pi, 50 * (int(r) + 1))
                 x = cx + r * np.cos(angles)
                 y = cy + r * np.sin(angles)
-                points = np.rint(np.append(x,y).reshape(-1,2,order='F'))
+                points = np.rint(np.append(x, y).reshape(-1, 2, order='F'))
                 _, index = np.unique(points, return_index=True, axis=0)
                 shape["points"] = points[np.sort(index)]
                 shape["shape_type"] = "polygon"
             elif shape["shape_type"] == "line":
-                (x1,y1), (x2,y2) = shape["points"]
-                shape["points"] = [x1,y1,x2,y2,x2+1e-3,y2+1e-3,x1+1e-3,y1+1e-3]
+                (x1, y1), (x2, y2) = shape["points"]
+                shape["points"] = [x1, y1, x2, y2, x2 + 1e-3, y2 + 1e-3, x1 + 1e-3, y1 + 1e-3]
                 shape["shape_type"] = "polygon"
-            
+            elif shape["shape_type"] == "point":
+                (x1, y1) = shape["points"][0]
+                shape["points"] = [[x1, y1], [x1 + 1, y1 + 1]]
+                shape["shape_type"] = "rectangle"
+
             # parse bbox/segmentation
             if shape["shape_type"] == "rectangle":
                 x1 = shape["points"][0][0]
                 y1 = shape["points"][0][1]
                 x2 = shape["points"][1][0]
                 y2 = shape["points"][1][1]
                 coco_annotation = CocoAnnotation(
@@ -112,8 +118,8 @@
         coco.add_image(coco_image)
 
     return coco
 
 
 if __name__ == "__main__":
     labelme_folder = "tests/data/labelme_annot"
-    coco = get_coco_from_labelme_folder(labelme_folder)
+    coco = get_coco_from_labelme_folder(labelme_folder)
```

### Comparing `labelme2coco-0.2.4/labelme2coco/utils.py` & `labelme2coco-0.2.6/labelme2coco/utils.py`

 * *Files identical despite different names*

### Comparing `labelme2coco-0.2.4/labelme2coco.egg-info/PKG-INFO` & `labelme2coco-0.2.6/labelme2coco.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: labelme2coco
-Version: 0.2.4
+Version: 0.2.6
 Summary: Convert labelme annotations into coco format in one step
 Home-page: https://github.com/fcakyon/labelme2coco
 Author: Fatih Cagatay Akyon
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: sahi>=0.8.19
+Requires-Dist: jsonschema>=2.6.0
 
 <div align="center">
 <h1>
   labelme2coco
 </h1>
 
 <a href="https://pepy.tech/project/labelme2coco"><img src="https://pepy.tech/badge/labelme2coco" alt="downloads"></a>
@@ -49,14 +51,18 @@
 labelme2coco path/to/labelme/dir
 ```
 
 ```python
 labelme2coco path/to/labelme/dir --train_split_rate 0.85
 ```
 
+```python
+labelme2coco path/to/labelme/dir --category_id_start 1
+```
+
 ### Advanced Usage
 
 ```python
 # import package
 import labelme2coco
 
 # set directory that contains labelme annotations and image files
@@ -64,16 +70,19 @@
 
 # set export dir
 export_dir = "tests/data/"
 
 # set train split rate
 train_split_rate = 0.85
 
+# set category ID start value
+category_id_start = 1
+
 # convert labelme annotations to coco
-labelme2coco.convert(labelme_folder, export_dir, train_split_rate)
+labelme2coco.convert(labelme_folder, export_dir, train_split_rate, category_id_start=category_id_start)
 ```
 
 ```python
 # import functions
 from labelme2coco import get_coco_from_labelme_folder, save_json
 
 # set labelme training data directory
@@ -81,19 +90,22 @@
 
 # set labelme validation data directory
 labelme_val_folder = "tests/data/labelme_annot"
 
 # set path for coco json to be saved
 export_dir = "tests/data/"
 
+# set category ID start value
+category_id_start = 1
+
 # create train coco object
-train_coco = get_coco_from_labelme_folder(labelme_train_folder)
+train_coco = get_coco_from_labelme_folder(labelme_train_folder, category_id_start=category_id_start)
 
 # export train coco json
 save_json(train_coco.json, export_dir+"train.json")
 
 # create val coco object
-val_coco = get_coco_from_labelme_folder(labelme_val_folder, coco_category_list=train_coco.json_categories)
+val_coco = get_coco_from_labelme_folder(labelme_val_folder, coco_category_list=train_coco.json_categories, category_id_start=category_id_start)
 
 # export val coco json
 save_json(val_coco.json, export_dir+"val.json")
 ```
```

#### html2text {}

```diff
@@ -1,36 +1,41 @@
-Metadata-Version: 2.1 Name: labelme2coco Version: 0.2.4 Summary: Convert
+Metadata-Version: 2.1 Name: labelme2coco Version: 0.2.6 Summary: Convert
 labelme annotations into coco format in one step Home-page: https://github.com/
 fcakyon/labelme2coco Author: Fatih Cagatay Akyon Author-email: Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
-Description-Content-Type: text/markdown License-File: LICENSE
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+sahi>=0.8.19 Requires-Dist: jsonschema>=2.6.0
                           ************ llaabbeellmmee22ccooccoo ************
                          _[_d_o_w_n_l_o_a_d_s_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_c_i_]
                                _[_f_c_a_k_y_o_n_ _t_w_i_t_t_e_r_]
   _**_**_**_ _AA_ _ll_ii_gg_hh_tt_ww_ee_ii_gg_hh_tt_ _pp_aa_cc_kk_aa_gg_ee_ _ff_oo_rr_ _cc_oo_nn_vv_ee_rr_tt_ii_nn_gg_ _yy_oo_uu_rr_ _ll_aa_bb_ee_ll_mm_ee_ _aa_nn_nn_oo_tt_aa_tt_ii_oo_nn_ss_ _ii_nn_tt_oo_ _CC_OO_CC_OO
                          _oo_bb_jj_ee_cc_tt_ _dd_ee_tt_ee_cc_tt_ii_oo_nn_ _ff_oo_rr_mm_aa_tt_.._ _**_**_**
                                _**_**_**_ _[[_tt_ee_aa_ss_ee_rr_]]_ _**_**_**
 ## Convert LabelMe annotations to COCO format in one step [labelme](https://
 github.com/wkentaro/labelme) is a widely used is a graphical image annotation
 tool that supports classification, segmentation, instance segmentation and
 object detection formats. However, widely used frameworks/models such as
 Yolact/Solo, Detectron, MMDetection etc. requires COCO formatted annotations.
 You can use this package to convert labelme annotations to COCO format. ##
 Getting started ### Installation ``` pip install -U labelme2coco ``` ### Basic
 Usage ```python labelme2coco path/to/labelme/dir ``` ```python labelme2coco
-path/to/labelme/dir --train_split_rate 0.85 ``` ### Advanced Usage ```python #
-import package import labelme2coco # set directory that contains labelme
-annotations and image files labelme_folder = "tests/data/labelme_annot" # set
-export dir export_dir = "tests/data/" # set train split rate train_split_rate =
-0.85 # convert labelme annotations to coco labelme2coco.convert(labelme_folder,
-export_dir, train_split_rate) ``` ```python # import functions from
+path/to/labelme/dir --train_split_rate 0.85 ``` ```python labelme2coco path/to/
+labelme/dir --category_id_start 1 ``` ### Advanced Usage ```python # import
+package import labelme2coco # set directory that contains labelme annotations
+and image files labelme_folder = "tests/data/labelme_annot" # set export dir
+export_dir = "tests/data/" # set train split rate train_split_rate = 0.85 # set
+category ID start value category_id_start = 1 # convert labelme annotations to
+coco labelme2coco.convert(labelme_folder, export_dir, train_split_rate,
+category_id_start=category_id_start) ``` ```python # import functions from
 labelme2coco import get_coco_from_labelme_folder, save_json # set labelme
 training data directory labelme_train_folder = "tests/data/labelme_annot" # set
 labelme validation data directory labelme_val_folder = "tests/data/
 labelme_annot" # set path for coco json to be saved export_dir = "tests/data/
-" # create train coco object train_coco = get_coco_from_labelme_folder
-(labelme_train_folder) # export train coco json save_json(train_coco.json,
-export_dir+"train.json") # create val coco object val_coco =
+" # set category ID start value category_id_start = 1 # create train coco
+object train_coco = get_coco_from_labelme_folder(labelme_train_folder,
+category_id_start=category_id_start) # export train coco json save_json
+(train_coco.json, export_dir+"train.json") # create val coco object val_coco =
 get_coco_from_labelme_folder(labelme_val_folder,
-coco_category_list=train_coco.json_categories) # export val coco json save_json
+coco_category_list=train_coco.json_categories,
+category_id_start=category_id_start) # export val coco json save_json
 (val_coco.json, export_dir+"val.json") ```
```

### Comparing `labelme2coco-0.2.4/setup.py` & `labelme2coco-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `labelme2coco-0.2.4/tests/test_unit.py` & `labelme2coco-0.2.6/tests/test_unit.py`

 * *Files identical despite different names*

