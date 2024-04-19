# Comparing `tmp/steelpy-1.0.2.tar.gz` & `tmp/steelpy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steelpy-1.0.2.tar", max compression
+gzip compressed data, was "steelpy-1.0.3.tar", max compression
```

## Comparing `steelpy-1.0.2.tar` & `steelpy-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,20 @@
--rw-r--r--   0        0        0    11558 2024-04-15 00:15:35.250711 steelpy-1.0.2/license.txt
--rw-r--r--   0        0        0      488 2024-04-18 00:21:27.687556 steelpy-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1491 2024-04-14 19:17:05.548477 steelpy-1.0.2/README.md
--rw-r--r--   0        0        0       25 2024-04-15 00:07:30.681181 steelpy-1.0.2/steelpy/__init__.py
--rw-r--r--   0        0        0    11358 2024-04-17 23:35:29.126753 steelpy-1.0.2/steelpy/LICENSE.md
--rw-r--r--   0        0        0       10 2024-04-17 23:35:29.126753 steelpy-1.0.2/steelpy/README.md
--rw-r--r--   0        0        0     6148 2024-04-13 14:24:11.525081 steelpy-1.0.2/steelpy/shape files/.DS_Store
--rw-r--r--   0        0        0    11454 2024-04-13 14:22:22.387676 steelpy-1.0.2/steelpy/shape files/C_shapes.xlsx
--rw-r--r--   0        0        0    55958 2024-04-13 14:22:22.517421 steelpy-1.0.2/steelpy/shape files/DBL_L_shapes.xlsx
--rw-r--r--   0        0        0     8761 2024-04-13 14:22:22.531852 steelpy-1.0.2/steelpy/shape files/HP_shapes.xlsx
--rw-r--r--   0        0        0    19577 2024-04-13 14:22:22.685953 steelpy-1.0.2/steelpy/shape files/HSS_R_shapes.xlsx
--rw-r--r--   0        0        0    53674 2024-04-13 14:22:22.648944 steelpy-1.0.2/steelpy/shape files/HSS_shapes.xlsx
--rw-r--r--   0        0        0    32880 2024-04-13 14:22:22.749414 steelpy-1.0.2/steelpy/shape files/L_shapes.xlsx
--rw-r--r--   0        0        0     7785 2024-04-13 14:22:22.761931 steelpy-1.0.2/steelpy/shape files/M_shapes.xlsx
--rw-r--r--   0        0        0    12974 2024-04-13 14:22:22.783967 steelpy-1.0.2/steelpy/shape files/MC_shapes.xlsx
--rw-r--r--   0        0        0     6841 2024-04-13 14:22:22.794757 steelpy-1.0.2/steelpy/shape files/MT_shapes.xlsx
--rw-r--r--   0        0        0     9052 2024-04-13 14:22:22.809959 steelpy-1.0.2/steelpy/shape files/PIPE_shapes.xlsx
--rw-r--r--   0        0        0     9556 2024-04-13 14:22:22.825993 steelpy-1.0.2/steelpy/shape files/S_shapes.xlsx
--rw-r--r--   0        0        0     8516 2024-04-13 14:22:22.839824 steelpy-1.0.2/steelpy/shape files/ST_shapes.xlsx
--rw-r--r--   0        0        0    51977 2024-04-13 14:22:22.946043 steelpy-1.0.2/steelpy/shape files/W_shapes.xlsx
--rw-r--r--   0        0        0    46395 2024-04-13 14:22:23.030673 steelpy-1.0.2/steelpy/shape files/WT_shapes.xlsx
--rw-r--r--   0        0        0     1885 2024-04-18 00:05:46.187099 steelpy-1.0.2/steelpy/steelpy.py
--rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 steelpy-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-04-19 18:22:07.234406 steelpy-1.0.3/license.txt
+-rw-r--r--   0        0        0      488 2024-04-19 23:35:14.187279 steelpy-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1492 2024-04-19 19:58:03.690260 steelpy-1.0.3/README.md
+-rw-r--r--   0        0        0       25 2024-04-19 18:22:07.236819 steelpy-1.0.3/steelpy/__init__.py
+-rw-r--r--   0        0        0     6395 2024-04-19 19:33:04.046419 steelpy-1.0.3/steelpy/shape files/C_shapes.csv
+-rw-r--r--   0        0        0    68640 2024-04-19 19:33:04.110419 steelpy-1.0.3/steelpy/shape files/DBL_L_shapes.csv
+-rw-r--r--   0        0        0     3691 2024-04-19 19:33:04.120417 steelpy-1.0.3/steelpy/shape files/HP_shapes.csv
+-rw-r--r--   0        0        0    18400 2024-04-19 19:33:04.142418 steelpy-1.0.3/steelpy/shape files/HSS_R_shapes.csv
+-rw-r--r--   0        0        0    57121 2024-04-19 19:33:04.198419 steelpy-1.0.3/steelpy/shape files/HSS_shapes.csv
+-rw-r--r--   0        0        0    30922 2024-04-19 19:33:04.233418 steelpy-1.0.3/steelpy/shape files/L_shapes.csv
+-rw-r--r--   0        0        0     2731 2024-04-19 19:33:04.266418 steelpy-1.0.3/steelpy/shape files/M_shapes.csv
+-rw-r--r--   0        0        0     7798 2024-04-19 19:33:04.248425 steelpy-1.0.3/steelpy/shape files/MC_shapes.csv
+-rw-r--r--   0        0        0     1910 2024-04-19 19:33:04.257419 steelpy-1.0.3/steelpy/shape files/MT_shapes.csv
+-rw-r--r--   0        0        0     4747 2024-04-19 19:33:04.277418 steelpy-1.0.3/steelpy/shape files/PIPE_shapes.csv
+-rw-r--r--   0        0        0     4496 2024-04-19 19:33:04.298421 steelpy-1.0.3/steelpy/shape files/S_shapes.csv
+-rw-r--r--   0        0        0     3520 2024-04-19 19:33:04.286419 steelpy-1.0.3/steelpy/shape files/ST_shapes.csv
+-rw-r--r--   0        0        0    50760 2024-04-19 19:33:04.414427 steelpy-1.0.3/steelpy/shape files/W_shapes.csv
+-rw-r--r--   0        0        0    42703 2024-04-19 19:33:04.345417 steelpy-1.0.3/steelpy/shape files/WT_shapes.csv
+-rw-r--r--   0        0        0     2828 2024-04-19 23:27:37.506649 steelpy-1.0.3/steelpy/steelpy.py
+-rw-r--r--   0        0        0     2163 1970-01-01 00:00:00.000000 steelpy-1.0.3/PKG-INFO
```

### Comparing `steelpy-1.0.2/license.txt` & `steelpy-1.0.3/license.txt`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.2/README.md` & `steelpy-1.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -33,24 +33,24 @@
 aisc.MT_shapes
 aisc.PIPE_shapes
 aisc.S_shapes
 aisc.ST_shapes
 aisc.W_shapes
 aisc.WT_shapes
 ```
-From there, specific profiles and properties are queried in a similar manner:
+From there, specific sections and properties are queried in a similar manner:
 ```
 beam = aisc.W_shapes.W12X26
 Fy = 50
 Aw = beam.d * beam.tw
 Cv = 1.0
 Vn = 0.6*Fy*Aw*Cv
 ```
-Shapes with fractions, hyphens or decimal points in their names are queried by replacing each with underscore:
+Sections with fractions, hyphens or decimal points in their names are queried by replacing each with underscore:
 ```
 aisc.C_shapes.C12X20_7
 aisc.L_shapes.L4X4X1_4
 aisc.W_shapes.W6X8_5
 ```
-Values are consistent with the AISC Steel Construction Manual, 16th Ed. and use the imperial system (inches, lbs).  .xlsx files for each library of shapes is saved in steelpy > shape files and can be referenced for the available shape profiles and associated properties.
+Values are consistent with the AISC Steel Construction Manual, 16th Ed. and use the imperial system (inches, lbs).  .csv files for each library of shapes is saved in steelpy > shape files and can be referenced for the available shape profiles and associated properties.
```

### Comparing `steelpy-1.0.2/PKG-INFO` & `steelpy-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steelpy
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple library for section properties of AISC steel shapes
 License: Apache-2.0
 Keywords: steel,AISC,engineering,shapes_AISC,AISC Shapes Database v16.0
 Author: evanfaler
 Author-email: emfaler@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -52,25 +52,25 @@
 aisc.MT_shapes
 aisc.PIPE_shapes
 aisc.S_shapes
 aisc.ST_shapes
 aisc.W_shapes
 aisc.WT_shapes
 ```
-From there, specific profiles and properties are queried in a similar manner:
+From there, specific sections and properties are queried in a similar manner:
 ```
 beam = aisc.W_shapes.W12X26
 Fy = 50
 Aw = beam.d * beam.tw
 Cv = 1.0
 Vn = 0.6*Fy*Aw*Cv
 ```
-Shapes with fractions, hyphens or decimal points in their names are queried by replacing each with underscore:
+Sections with fractions, hyphens or decimal points in their names are queried by replacing each with underscore:
 ```
 aisc.C_shapes.C12X20_7
 aisc.L_shapes.L4X4X1_4
 aisc.W_shapes.W6X8_5
 ```
-Values are consistent with the AISC Steel Construction Manual, 16th Ed. and use the imperial system (inches, lbs).  .xlsx files for each library of shapes is saved in steelpy > shape files and can be referenced for the available shape profiles and associated properties.
+Values are consistent with the AISC Steel Construction Manual, 16th Ed. and use the imperial system (inches, lbs).  .csv files for each library of shapes is saved in steelpy > shape files and can be referenced for the available shape profiles and associated properties.
```

