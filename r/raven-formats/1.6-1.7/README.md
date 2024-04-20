# Comparing `tmp/raven-formats-1.6.tar.gz` & `tmp/raven_formats-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raven-formats-1.6.tar", last modified: Tue Feb 21 19:09:41 2023, max compression
+gzip compressed data, was "raven_formats-1.7.tar", last modified: Sat Apr 20 11:42:53 2024, max compression
```

## Comparing `raven-formats-1.6.tar` & `raven_formats-1.7.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-02-21 19:09:41.418265 raven-formats-1.6/
--rw-rw-rw-   0        0        0     1093 2021-05-01 18:13:43.000000 raven-formats-1.6/LICENSE.md
--rw-rw-rw-   0        0        0       47 2021-05-03 15:30:30.000000 raven-formats-1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1941 2023-02-21 19:09:41.418265 raven-formats-1.6/PKG-INFO
--rw-rw-rw-   0        0        0      988 2021-05-02 10:29:05.000000 raven-formats-1.6/README.md
--rw-rw-rw-   0        0        0      108 2021-05-02 11:03:54.000000 raven-formats-1.6/pyproject.toml
--rw-rw-rw-   0        0        0     1128 2023-02-21 19:09:41.420064 raven-formats-1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-21 19:09:41.248811 raven-formats-1.6/src/
-drwxrwxrwx   0        0        0        0 2023-02-21 19:09:41.351921 raven-formats-1.6/src/raven_formats/
--rw-rw-rw-   0        0        0        0 2019-07-16 10:13:01.000000 raven-formats-1.6/src/raven_formats/__init__.py
--rw-rw-rw-   0        0        0     3070 2021-05-02 12:22:55.000000 raven-formats-1.6/src/raven_formats/adpcm.py
-drwxrwxrwx   0        0        0        0 2023-02-21 19:09:41.415637 raven-formats-1.6/src/raven_formats/data/
--rw-rw-rw-   0        0        0        0 2021-05-03 15:32:36.000000 raven-formats-1.6/src/raven_formats/data/__init__.py
--rw-rw-rw-   0        0        0   730800 2023-02-21 18:57:19.000000 raven-formats-1.6/src/raven_formats/data/zsnd_hashes.json
--rw-rw-rw-   0        0        0     8321 2023-02-21 18:57:43.000000 raven-formats-1.6/src/raven_formats/xmlb.py
--rw-rw-rw-   0        0        0    16927 2023-02-21 18:58:03.000000 raven-formats-1.6/src/raven_formats/zsnd.py
-drwxrwxrwx   0        0        0        0 2023-02-21 19:09:41.369064 raven-formats-1.6/src/raven_formats.egg-info/
--rw-rw-rw-   0        0        0     1941 2023-02-21 19:09:41.000000 raven-formats-1.6/src/raven_formats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-02-21 19:09:41.000000 raven-formats-1.6/src/raven_formats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-21 19:09:41.000000 raven-formats-1.6/src/raven_formats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-02-21 19:09:41.000000 raven-formats-1.6/src/raven_formats.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-02-21 19:09:41.000000 raven-formats-1.6/src/raven_formats.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 11:42:53.977658 raven_formats-1.7/
+-rw-rw-rw-   0        0        0     1093 2021-05-01 18:13:43.000000 raven_formats-1.7/LICENSE.md
+-rw-rw-rw-   0        0        0       47 2021-05-03 15:30:30.000000 raven_formats-1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2301 2024-04-20 11:42:53.977658 raven_formats-1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1348 2024-04-20 11:05:52.000000 raven_formats-1.7/README.md
+-rw-rw-rw-   0        0        0      108 2021-05-02 11:03:54.000000 raven_formats-1.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1157 2024-04-20 11:42:53.980648 raven_formats-1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-20 11:42:53.945154 raven_formats-1.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-20 11:42:53.960268 raven_formats-1.7/src/raven_formats/
+-rw-rw-rw-   0        0        0        0 2019-07-16 10:13:01.000000 raven_formats-1.7/src/raven_formats/__init__.py
+-rw-rw-rw-   0        0        0     3070 2021-05-02 12:22:55.000000 raven_formats-1.7/src/raven_formats/adpcm.py
+drwxrwxrwx   0        0        0        0 2024-04-20 11:42:53.973667 raven_formats-1.7/src/raven_formats/data/
+-rw-rw-rw-   0        0        0        0 2024-04-20 11:06:38.000000 raven_formats-1.7/src/raven_formats/data/__init__.py
+-rw-rw-rw-   0        0        0   730800 2024-04-20 11:06:39.000000 raven_formats-1.7/src/raven_formats/data/zsnd_hashes.json
+-rw-rw-rw-   0        0        0     2514 2024-04-20 11:23:29.000000 raven_formats-1.7/src/raven_formats/fb.py
+-rw-rw-rw-   0        0        0     8321 2023-04-14 10:38:45.000000 raven_formats-1.7/src/raven_formats/xmlb.py
+-rw-rw-rw-   0        0        0    16927 2023-02-21 18:58:03.000000 raven_formats-1.7/src/raven_formats/zsnd.py
+drwxrwxrwx   0        0        0        0 2024-04-20 11:42:53.976660 raven_formats-1.7/src/raven_formats.egg-info/
+-rw-rw-rw-   0        0        0     2301 2024-04-20 11:42:53.000000 raven_formats-1.7/src/raven_formats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2024-04-20 11:42:53.000000 raven_formats-1.7/src/raven_formats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 11:42:53.000000 raven_formats-1.7/src/raven_formats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      107 2024-04-20 11:42:53.000000 raven_formats-1.7/src/raven_formats.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-04-20 11:42:53.000000 raven_formats-1.7/src/raven_formats.egg-info/top_level.txt
```

### Comparing `raven-formats-1.6/LICENSE.md` & `raven_formats-1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `raven-formats-1.6/PKG-INFO` & `raven_formats-1.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raven-formats
-Version: 1.6
+Version: 1.7
 Summary: Tools to work with formats used by Raven Software in MUA/XML2 games
 Home-page: https://github.com/nikita488/raven-formats
 Author: nikita488
 Project-URL: Bug Tracker, https://github.com/nikita488/raven-formats/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -47,7 +47,20 @@
   input            input file (supports glob)
   output           output file (wildcards will be replaced by input file name)
 
 optional arguments:
   -h, --help       show this help message and exit
   -d, --decompile  decompile input ZSND file to JSON file
 ```
+
+#### FB Compile/Decompile
+```
+usage: fb.py [-h] [-d] input output
+
+positional arguments:
+  input            input file (supports glob)
+  output           output file (wildcards will be replaced by input file name)
+
+optional arguments:
+  -h, --help       show this help message and exit
+  -d, --decompile  decompile input FB file to JSON file
+```
```

### Comparing `raven-formats-1.6/setup.cfg` & `raven_formats-1.7/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2072 6176 656e 2d66 6f72 6d61 7473   = raven-formats
-00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 360d  ..version = 1.6.
+00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 370d  ..version = 1.7.
 00000030: 0a61 7574 686f 7220 3d20 6e69 6b69 7461  .author = nikita
 00000040: 3438 380d 0a64 6573 6372 6970 7469 6f6e  488..description
 00000050: 203d 2054 6f6f 6c73 2074 6f20 776f 726b   = Tools to work
 00000060: 2077 6974 6820 666f 726d 6174 7320 7573   with formats us
 00000070: 6564 2062 7920 5261 7665 6e20 536f 6674  ed by Raven Soft
 00000080: 7761 7265 2069 6e20 4d55 412f 584d 4c32  ware in MUA/XML2
 00000090: 2067 616d 6573 0d0a 6c6f 6e67 5f64 6573   games..long_des
@@ -61,11 +61,13 @@
 000003c0: 6865 7265 203d 2073 7263 0d0a 0d0a 5b6f  here = src....[o
 000003d0: 7074 696f 6e73 2e65 6e74 7279 5f70 6f69  ptions.entry_poi
 000003e0: 6e74 735d 0d0a 636f 6e73 6f6c 655f 7363  nts]..console_sc
 000003f0: 7269 7074 7320 3d20 0d0a 0978 6d6c 6220  ripts = ...xmlb 
 00000400: 3d20 7261 7665 6e5f 666f 726d 6174 732e  = raven_formats.
 00000410: 786d 6c62 3a6d 6169 6e0d 0a09 7a73 6e64  xmlb:main...zsnd
 00000420: 203d 2072 6176 656e 5f66 6f72 6d61 7473   = raven_formats
-00000430: 2e7a 736e 643a 6d61 696e 0d0a 0d0a 5b65  .zsnd:main....[e
-00000440: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-00000450: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-00000460: 203d 2030 0d0a 0d0a                       = 0....
+00000430: 2e7a 736e 643a 6d61 696e 0d0a 0966 6220  .zsnd:main...fb 
+00000440: 3d20 7261 7665 6e5f 666f 726d 6174 732e  = raven_formats.
+00000450: 6662 3a6d 6169 6e0d 0a0d 0a5b 6567 675f  fb:main....[egg_
+00000460: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000470: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+00000480: 300d 0a0d 0a                             0....
```

### Comparing `raven-formats-1.6/src/raven_formats/adpcm.py` & `raven_formats-1.7/src/raven_formats/adpcm.py`

 * *Files identical despite different names*

### Comparing `raven-formats-1.6/src/raven_formats/data/zsnd_hashes.json` & `raven_formats-1.7/src/raven_formats/data/zsnd_hashes.json`

 * *Files identical despite different names*

### Comparing `raven-formats-1.6/src/raven_formats/xmlb.py` & `raven_formats-1.7/src/raven_formats/xmlb.py`

 * *Files identical despite different names*

### Comparing `raven-formats-1.6/src/raven_formats/zsnd.py` & `raven_formats-1.7/src/raven_formats/zsnd.py`

 * *Files identical despite different names*

### Comparing `raven-formats-1.6/src/raven_formats.egg-info/PKG-INFO` & `raven_formats-1.7/src/raven_formats.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raven-formats
-Version: 1.6
+Version: 1.7
 Summary: Tools to work with formats used by Raven Software in MUA/XML2 games
 Home-page: https://github.com/nikita488/raven-formats
 Author: nikita488
 Project-URL: Bug Tracker, https://github.com/nikita488/raven-formats/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -47,7 +47,20 @@
   input            input file (supports glob)
   output           output file (wildcards will be replaced by input file name)
 
 optional arguments:
   -h, --help       show this help message and exit
   -d, --decompile  decompile input ZSND file to JSON file
 ```
+
+#### FB Compile/Decompile
+```
+usage: fb.py [-h] [-d] input output
+
+positional arguments:
+  input            input file (supports glob)
+  output           output file (wildcards will be replaced by input file name)
+
+optional arguments:
+  -h, --help       show this help message and exit
+  -d, --decompile  decompile input FB file to JSON file
+```
```

