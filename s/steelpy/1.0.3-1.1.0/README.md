# Comparing `tmp/steelpy-1.0.3.tar.gz` & `tmp/steelpy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steelpy-1.0.3.tar", max compression
+gzip compressed data, was "steelpy-1.1.0.tar", max compression
```

## Comparing `steelpy-1.0.3.tar` & `steelpy-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11558 2024-04-19 18:22:07.234406 steelpy-1.0.3/license.txt
--rw-r--r--   0        0        0      488 2024-04-19 23:35:14.187279 steelpy-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1492 2024-04-19 19:58:03.690260 steelpy-1.0.3/README.md
--rw-r--r--   0        0        0       25 2024-04-19 18:22:07.236819 steelpy-1.0.3/steelpy/__init__.py
--rw-r--r--   0        0        0     6395 2024-04-19 19:33:04.046419 steelpy-1.0.3/steelpy/shape files/C_shapes.csv
--rw-r--r--   0        0        0    68640 2024-04-19 19:33:04.110419 steelpy-1.0.3/steelpy/shape files/DBL_L_shapes.csv
--rw-r--r--   0        0        0     3691 2024-04-19 19:33:04.120417 steelpy-1.0.3/steelpy/shape files/HP_shapes.csv
--rw-r--r--   0        0        0    18400 2024-04-19 19:33:04.142418 steelpy-1.0.3/steelpy/shape files/HSS_R_shapes.csv
--rw-r--r--   0        0        0    57121 2024-04-19 19:33:04.198419 steelpy-1.0.3/steelpy/shape files/HSS_shapes.csv
--rw-r--r--   0        0        0    30922 2024-04-19 19:33:04.233418 steelpy-1.0.3/steelpy/shape files/L_shapes.csv
--rw-r--r--   0        0        0     2731 2024-04-19 19:33:04.266418 steelpy-1.0.3/steelpy/shape files/M_shapes.csv
--rw-r--r--   0        0        0     7798 2024-04-19 19:33:04.248425 steelpy-1.0.3/steelpy/shape files/MC_shapes.csv
--rw-r--r--   0        0        0     1910 2024-04-19 19:33:04.257419 steelpy-1.0.3/steelpy/shape files/MT_shapes.csv
--rw-r--r--   0        0        0     4747 2024-04-19 19:33:04.277418 steelpy-1.0.3/steelpy/shape files/PIPE_shapes.csv
--rw-r--r--   0        0        0     4496 2024-04-19 19:33:04.298421 steelpy-1.0.3/steelpy/shape files/S_shapes.csv
--rw-r--r--   0        0        0     3520 2024-04-19 19:33:04.286419 steelpy-1.0.3/steelpy/shape files/ST_shapes.csv
--rw-r--r--   0        0        0    50760 2024-04-19 19:33:04.414427 steelpy-1.0.3/steelpy/shape files/W_shapes.csv
--rw-r--r--   0        0        0    42703 2024-04-19 19:33:04.345417 steelpy-1.0.3/steelpy/shape files/WT_shapes.csv
--rw-r--r--   0        0        0     2828 2024-04-19 23:27:37.506649 steelpy-1.0.3/steelpy/steelpy.py
--rw-r--r--   0        0        0     2163 1970-01-01 00:00:00.000000 steelpy-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-04-19 18:22:07.234406 steelpy-1.1.0/license.txt
+-rw-r--r--   0        0        0      488 2024-04-20 02:14:25.935583 steelpy-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3068 2024-04-20 02:14:25.935583 steelpy-1.1.0/README.md
+-rw-r--r--   0        0        0       25 2024-04-19 18:22:07.236819 steelpy-1.1.0/steelpy/__init__.py
+-rw-r--r--   0        0        0     6395 2024-04-19 23:40:49.312818 steelpy-1.1.0/steelpy/shape files/C_shapes.csv
+-rw-r--r--   0        0        0    68640 2024-04-19 23:40:49.313818 steelpy-1.1.0/steelpy/shape files/DBL_L_shapes.csv
+-rw-r--r--   0        0        0     3691 2024-04-19 23:40:49.314818 steelpy-1.1.0/steelpy/shape files/HP_shapes.csv
+-rw-r--r--   0        0        0    18400 2024-04-19 23:40:49.314818 steelpy-1.1.0/steelpy/shape files/HSS_R_shapes.csv
+-rw-r--r--   0        0        0    57121 2024-04-19 23:40:49.315816 steelpy-1.1.0/steelpy/shape files/HSS_shapes.csv
+-rw-r--r--   0        0        0    30922 2024-04-19 23:40:49.315816 steelpy-1.1.0/steelpy/shape files/L_shapes.csv
+-rw-r--r--   0        0        0     2731 2024-04-19 23:40:49.316817 steelpy-1.1.0/steelpy/shape files/M_shapes.csv
+-rw-r--r--   0        0        0     7798 2024-04-19 23:40:49.316817 steelpy-1.1.0/steelpy/shape files/MC_shapes.csv
+-rw-r--r--   0        0        0     1910 2024-04-19 23:40:49.316817 steelpy-1.1.0/steelpy/shape files/MT_shapes.csv
+-rw-r--r--   0        0        0     4747 2024-04-19 23:40:49.317820 steelpy-1.1.0/steelpy/shape files/PIPE_shapes.csv
+-rw-r--r--   0        0        0     4496 2024-04-19 23:40:49.318817 steelpy-1.1.0/steelpy/shape files/S_shapes.csv
+-rw-r--r--   0        0        0     3520 2024-04-19 23:40:49.317820 steelpy-1.1.0/steelpy/shape files/ST_shapes.csv
+-rw-r--r--   0        0        0    50760 2024-04-19 23:40:49.319872 steelpy-1.1.0/steelpy/shape files/W_shapes.csv
+-rw-r--r--   0        0        0    42703 2024-04-19 23:40:49.318817 steelpy-1.1.0/steelpy/shape files/WT_shapes.csv
+-rw-r--r--   0        0        0     4467 2024-04-20 02:14:25.936638 steelpy-1.1.0/steelpy/steelpy.py
+-rw-r--r--   0        0        0     3708 1970-01-01 00:00:00.000000 steelpy-1.1.0/PKG-INFO
```

### Comparing `steelpy-1.0.3/license.txt` & `steelpy-1.1.0/license.txt`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.3/steelpy/shape files/C_shapes.csv` & `steelpy-1.1.0/steelpy/shape files/C_shapes.csv`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.3/steelpy/shape files/DBL_L_shapes.csv` & `steelpy-1.1.0/steelpy/shape files/DBL_L_shapes.csv`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.3/steelpy/shape files/HP_shapes.csv` & `steelpy-1.1.0/steelpy/shape files/HP_shapes.csv`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.3/steelpy/shape files/HSS_R_shapes.csv` & `steelpy-1.1.0/steelpy/shape files/HSS_R_shapes.csv`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.3/steelpy/shape files/HSS_shapes.csv` & `steelpy-1.1.0/steelpy/shape files/HSS_shapes.csv`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.3/steelpy/shape files/L_shapes.csv` & `steelpy-1.1.0/steelpy/shape files/L_shapes.csv`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.3/steelpy/shape files/M_shapes.csv` & `steelpy-1.1.0/steelpy/shape files/M_shapes.csv`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.3/steelpy/shape files/MC_shapes.csv` & `steelpy-1.1.0/steelpy/shape files/MC_shapes.csv`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.3/steelpy/shape files/MT_shapes.csv` & `steelpy-1.1.0/steelpy/shape files/MT_shapes.csv`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.3/steelpy/shape files/PIPE_shapes.csv` & `steelpy-1.1.0/steelpy/shape files/PIPE_shapes.csv`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.3/steelpy/shape files/S_shapes.csv` & `steelpy-1.1.0/steelpy/shape files/S_shapes.csv`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.3/steelpy/shape files/ST_shapes.csv` & `steelpy-1.1.0/steelpy/shape files/ST_shapes.csv`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.3/steelpy/shape files/W_shapes.csv` & `steelpy-1.1.0/steelpy/shape files/W_shapes.csv`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.3/steelpy/shape files/WT_shapes.csv` & `steelpy-1.1.0/steelpy/shape files/WT_shapes.csv`

 * *Files identical despite different names*

