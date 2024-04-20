# Comparing `tmp/aghplctools-4.8.6.tar.gz` & `tmp/aghplctools-4.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aghplctools-4.8.6.tar", last modified: Wed Aug 17 20:42:21 2022, max compression
+gzip compressed data, was "aghplctools-4.8.8.tar", last modified: Sat Apr 20 00:23:34 2024, max compression
```

## Comparing `aghplctools-4.8.6.tar` & `aghplctools-4.8.8.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-17 20:42:21.904347 aghplctools-4.8.6/
--rw-rw-rw-   0 root         (0) root         (0)     1063 2022-08-17 20:42:08.000000 aghplctools-4.8.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2014 2022-08-17 20:42:21.902346 aghplctools-4.8.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1130 2022-08-17 20:42:08.000000 aghplctools-4.8.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-17 20:42:21.889345 aghplctools-4.8.6/aghplctools/
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-08-17 20:42:08.000000 aghplctools-4.8.6/aghplctools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2022-08-17 20:42:08.000000 aghplctools-4.8.6/aghplctools/batch.py
--rw-rw-rw-   0 root         (0) root         (0)     1291 2022-08-17 20:42:08.000000 aghplctools-4.8.6/aghplctools/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-17 20:42:21.897346 aghplctools-4.8.6/aghplctools/data/
--rw-rw-rw-   0 root         (0) root         (0)      297 2022-08-17 20:42:08.000000 aghplctools-4.8.6/aghplctools/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6848 2022-08-17 20:42:08.000000 aghplctools-4.8.6/aghplctools/data/batch.py
--rw-rw-rw-   0 root         (0) root         (0)    54185 2022-08-17 20:42:08.000000 aghplctools-4.8.6/aghplctools/data/sample.py
--rw-rw-rw-   0 root         (0) root         (0)     8407 2022-08-17 20:42:08.000000 aghplctools-4.8.6/aghplctools/data/time_course.py
--rw-rw-rw-   0 root         (0) root         (0)      303 2022-08-17 20:42:08.000000 aghplctools-4.8.6/aghplctools/data_types.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2022-08-17 20:42:08.000000 aghplctools-4.8.6/aghplctools/hplc.py
--rw-rw-rw-   0 root         (0) root         (0)     1883 2022-08-17 20:42:08.000000 aghplctools-4.8.6/aghplctools/indirect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-17 20:42:21.902346 aghplctools-4.8.6/aghplctools/ingestion/
--rw-rw-rw-   0 root         (0) root         (0)      222 2022-08-17 20:42:08.000000 aghplctools-4.8.6/aghplctools/ingestion/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4560 2022-08-17 20:42:08.000000 aghplctools-4.8.6/aghplctools/ingestion/csv.py
--rw-rw-rw-   0 root         (0) root         (0)     9180 2022-08-17 20:42:08.000000 aghplctools-4.8.6/aghplctools/ingestion/text.py
--rw-rw-rw-   0 root         (0) root         (0)    26910 2022-08-17 20:42:08.000000 aghplctools-4.8.6/aghplctools/local_paths.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-17 20:42:21.894346 aghplctools-4.8.6/aghplctools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2014 2022-08-17 20:42:21.000000 aghplctools-4.8.6/aghplctools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      571 2022-08-17 20:42:21.000000 aghplctools-4.8.6/aghplctools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-17 20:42:21.000000 aghplctools-4.8.6/aghplctools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       97 2022-08-17 20:42:21.000000 aghplctools-4.8.6/aghplctools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-08-17 20:42:21.000000 aghplctools-4.8.6/aghplctools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-17 20:42:21.904347 aghplctools-4.8.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1506 2022-08-17 20:42:09.000000 aghplctools-4.8.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 00:23:34.616286 aghplctools-4.8.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-04-20 00:23:19.000000 aghplctools-4.8.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2216 2024-04-20 00:23:34.615285 aghplctools-4.8.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2024-04-20 00:23:19.000000 aghplctools-4.8.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 00:23:34.602285 aghplctools-4.8.8/aghplctools/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-20 00:23:19.000000 aghplctools-4.8.8/aghplctools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2024-04-20 00:23:19.000000 aghplctools-4.8.8/aghplctools/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2024-04-20 00:23:19.000000 aghplctools-4.8.8/aghplctools/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 00:23:34.605286 aghplctools-4.8.8/aghplctools/data/
+-rw-rw-rw-   0 root         (0) root         (0)      297 2024-04-20 00:23:19.000000 aghplctools-4.8.8/aghplctools/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6848 2024-04-20 00:23:19.000000 aghplctools-4.8.8/aghplctools/data/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)    54185 2024-04-20 00:23:19.000000 aghplctools-4.8.8/aghplctools/data/sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     8407 2024-04-20 00:23:19.000000 aghplctools-4.8.8/aghplctools/data/time_course.py
+-rw-rw-rw-   0 root         (0) root         (0)      303 2024-04-20 00:23:19.000000 aghplctools-4.8.8/aghplctools/data_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-04-20 00:23:19.000000 aghplctools-4.8.8/aghplctools/hplc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1883 2024-04-20 00:23:19.000000 aghplctools-4.8.8/aghplctools/indirect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 00:23:34.606286 aghplctools-4.8.8/aghplctools/ingestion/
+-rw-rw-rw-   0 root         (0) root         (0)      222 2024-04-20 00:23:19.000000 aghplctools-4.8.8/aghplctools/ingestion/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4560 2024-04-20 00:23:19.000000 aghplctools-4.8.8/aghplctools/ingestion/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)     9180 2024-04-20 00:23:19.000000 aghplctools-4.8.8/aghplctools/ingestion/text.py
+-rw-rw-rw-   0 root         (0) root         (0)    27050 2024-04-20 00:23:19.000000 aghplctools-4.8.8/aghplctools/local_paths.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 00:23:34.615285 aghplctools-4.8.8/aghplctools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2216 2024-04-20 00:23:34.000000 aghplctools-4.8.8/aghplctools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      669 2024-04-20 00:23:34.000000 aghplctools-4.8.8/aghplctools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 00:23:34.000000 aghplctools-4.8.8/aghplctools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2024-04-20 00:23:34.000000 aghplctools-4.8.8/aghplctools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-20 00:23:34.000000 aghplctools-4.8.8/aghplctools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 00:23:34.616286 aghplctools-4.8.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1506 2024-04-20 00:23:19.000000 aghplctools-4.8.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 00:23:34.608286 aghplctools-4.8.8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    12332 2024-04-20 00:23:19.000000 aghplctools-4.8.8/tests/test_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1958 2024-04-20 00:23:19.000000 aghplctools-4.8.8/tests/test_di_extraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     1208 2024-04-20 00:23:19.000000 aghplctools-4.8.8/tests/test_ingestion.py
+-rw-rw-rw-   0 root         (0) root         (0)     2459 2024-04-20 00:23:19.000000 aghplctools-4.8.8/tests/test_local_system.py
```

### Comparing `aghplctools-4.8.6/LICENSE` & `aghplctools-4.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aghplctools-4.8.6/PKG-INFO` & `aghplctools-4.8.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aghplctools
-Version: 4.8.6
+Version: 4.8.8
 Summary: Interaction package for Agilent ChemStation report files
 Home-page: https://gitlab.com/heingroup/aghplctools
 Author: Lars Yunker / Hein Group
 License: Copyright 2019 Lars Yunker / Hein Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
         documentation files (the "Software"), to deal in the Software without restriction, including without limitation
@@ -27,7 +27,14 @@
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib>=3.0.3
+Requires-Dist: tqdm
+Requires-Dist: unithandler>=1.3.3
+Requires-Dist: openpyxl>=2.6.2
+Requires-Dist: hein_utilities>=3.5
+Requires-Dist: aston>=0.7.0
```

### Comparing `aghplctools-4.8.6/README.md` & `aghplctools-4.8.8/README.md`

 * *Files identical despite different names*

### Comparing `aghplctools-4.8.6/aghplctools/config.py` & `aghplctools-4.8.8/aghplctools/config.py`

 * *Files identical despite different names*

### Comparing `aghplctools-4.8.6/aghplctools/data/batch.py` & `aghplctools-4.8.8/aghplctools/data/batch.py`

 * *Files identical despite different names*

### Comparing `aghplctools-4.8.6/aghplctools/data/sample.py` & `aghplctools-4.8.8/aghplctools/data/sample.py`

 * *Files identical despite different names*

### Comparing `aghplctools-4.8.6/aghplctools/data/time_course.py` & `aghplctools-4.8.8/aghplctools/data/time_course.py`

 * *Files identical despite different names*

### Comparing `aghplctools-4.8.6/aghplctools/indirect.py` & `aghplctools-4.8.8/aghplctools/indirect.py`

 * *Files identical despite different names*

### Comparing `aghplctools-4.8.6/aghplctools/ingestion/csv.py` & `aghplctools-4.8.8/aghplctools/ingestion/csv.py`

 * *Files identical despite different names*

### Comparing `aghplctools-4.8.6/aghplctools/ingestion/text.py` & `aghplctools-4.8.8/aghplctools/ingestion/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     'Peak': {  # peak index
         '#': '[ ]+(?P<Peak>[\d]+)',  # number
     },
     'RetTime': {  # retention time
         '[min]': '(?P<RetTime>[\d]+.[\d]+)',  # minutes
     },
     'Type': {  # peak type
-        '': '(?P<Type>[A-Z]{1,2}(?: [A-Z]{1,2})*)',
+        '': '(?P<Type>[A-Z]{1,3}(?: [A-Z]{1,3})*)',
     },
     'Width': {  # peak width
         '[min]': '(?P<Width>[\d]+.[\d]+[e+-]*[\d]+)',
     },
     'Area': {  # peak area
         '[mAU*s]': '(?P<Area>[\d]+.[\d]+[e+-]*[\d]+)',  # area units
         '%': '(?P<percent>[\d]+.[\d]+[e+-]*[\d]+)',  # percent
```

### Comparing `aghplctools-4.8.6/aghplctools/local_paths.py` & `aghplctools-4.8.8/aghplctools/local_paths.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,16 +244,20 @@
         :return: current file number, current file name
         """
         with open(path, 'rt', encoding='utf16') as f:
             contents = f.read()
         match = _acq_re.search(contents)
         if match is None:
             raise ValueError(f'The contents of ACQUIRING.TXT could not be parsed: {contents}')
+        try:
+            number = int(match.group('file_number'))
+        except TypeError:  # will not be defined for C.01.05 specifications
+            number = 1
         return (
-            int(match.group('file_number')),
+            number,
             match.group('file_name')
         )
 
     def _clear_acquiring(self):
         """clears acquiring status if the instance is currently acquiring"""
         if self._acquiring_path is not None:
             self._acquiring_path = None
```

### Comparing `aghplctools-4.8.6/aghplctools.egg-info/PKG-INFO` & `aghplctools-4.8.8/aghplctools.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aghplctools
-Version: 4.8.6
+Version: 4.8.8
 Summary: Interaction package for Agilent ChemStation report files
 Home-page: https://gitlab.com/heingroup/aghplctools
 Author: Lars Yunker / Hein Group
 License: Copyright 2019 Lars Yunker / Hein Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
         documentation files (the "Software"), to deal in the Software without restriction, including without limitation
@@ -27,7 +27,14 @@
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib>=3.0.3
+Requires-Dist: tqdm
+Requires-Dist: unithandler>=1.3.3
+Requires-Dist: openpyxl>=2.6.2
+Requires-Dist: hein_utilities>=3.5
+Requires-Dist: aston>=0.7.0
```

### Comparing `aghplctools-4.8.6/aghplctools.egg-info/SOURCES.txt` & `aghplctools-4.8.8/aghplctools.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -15,8 +15,12 @@
 aghplctools.egg-info/top_level.txt
 aghplctools/data/__init__.py
 aghplctools/data/batch.py
 aghplctools/data/sample.py
 aghplctools/data/time_course.py
 aghplctools/ingestion/__init__.py
 aghplctools/ingestion/csv.py
-aghplctools/ingestion/text.py
+aghplctools/ingestion/text.py
+tests/test_data.py
+tests/test_di_extraction.py
+tests/test_ingestion.py
+tests/test_local_system.py
```

### Comparing `aghplctools-4.8.6/setup.py` & `aghplctools-4.8.8/setup.py`

 * *Files identical despite different names*

