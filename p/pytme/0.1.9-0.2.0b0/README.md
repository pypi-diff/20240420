# Comparing `tmp/pytme-0.1.9.tar.gz` & `tmp/pytme-0.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytme-0.1.9.tar", last modified: Sun Mar  3 21:07:03 2024, max compression
+gzip compressed data, was "pytme-0.2.0b0.tar", last modified: Sat Apr 20 17:25:09 2024, max compression
```

## Comparing `pytme-0.1.9.tar` & `pytme-0.2.0b0.tar`

### file list

```diff
@@ -1,65 +1,70 @@
-drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-03-03 21:07:03.157364 pytme-0.1.9/
--rw-r--r--   0 vmaurer    (502) staff       (20)    18467 2023-10-21 17:18:54.000000 pytme-0.1.9/LICENSE
--rw-r--r--   0 vmaurer    (502) staff       (20)     1354 2024-03-03 13:30:23.000000 pytme-0.1.9/MANIFEST.in
--rw-r--r--   0 vmaurer    (502) staff       (20)     2112 2024-03-03 21:07:03.157127 pytme-0.1.9/PKG-INFO
--rw-r--r--   0 vmaurer    (502) staff       (20)     1348 2024-03-03 13:30:23.000000 pytme-0.1.9/README.md
--rw-r--r--   0 vmaurer    (502) staff       (20)     1210 2024-03-03 21:06:21.000000 pytme-0.1.9/pyproject.toml
-drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-03-03 21:07:03.156792 pytme-0.1.9/pytme.egg-info/
--rw-r--r--   0 vmaurer    (502) staff       (20)     1157 2024-03-03 21:07:03.000000 pytme-0.1.9/pytme.egg-info/SOURCES.txt
-drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-03-03 21:07:03.072829 pytme-0.1.9/scripts/
--rw-r--r--   0 vmaurer    (502) staff       (20)        0 2023-12-11 19:10:01.000000 pytme-0.1.9/scripts/__init__.py
--rwxr-xr-x   0 vmaurer    (502) staff       (20)     2768 2024-01-17 20:33:54.000000 pytme-0.1.9/scripts/estimate_ram_usage.py
--rwxr-xr-x   0 vmaurer    (502) staff       (20)    25744 2024-02-21 17:25:38.000000 pytme-0.1.9/scripts/match_template.py
--rwxr-xr-x   0 vmaurer    (502) staff       (20)    21939 2024-02-25 20:53:39.000000 pytme-0.1.9/scripts/postprocess.py
--rwxr-xr-x   0 vmaurer    (502) staff       (20)     2528 2023-10-17 21:34:50.000000 pytme-0.1.9/scripts/preprocess.py
--rwxr-xr-x   0 vmaurer    (502) staff       (20)    29001 2024-02-29 16:38:38.000000 pytme-0.1.9/scripts/preprocessor_gui.py
--rw-r--r--   0 vmaurer    (502) staff       (20)       38 2024-03-03 21:07:03.157422 pytme-0.1.9/setup.cfg
--rw-r--r--   0 vmaurer    (502) staff       (20)     1846 2024-03-03 13:30:23.000000 pytme-0.1.9/setup.py
-drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-03-03 21:07:03.073298 pytme-0.1.9/src/
--rw-r--r--   0 vmaurer    (502) staff       (20)    12901 2023-10-22 10:25:03.000000 pytme-0.1.9/src/extensions.cpp
-drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-03-03 21:07:03.079617 pytme-0.1.9/tme/
--rw-r--r--   0 vmaurer    (502) staff       (20)      212 2023-10-15 10:07:58.000000 pytme-0.1.9/tme/__init__.py
--rw-r--r--   0 vmaurer    (502) staff       (20)       22 2024-03-03 21:06:14.000000 pytme-0.1.9/tme/__version__.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    39188 2024-02-05 17:01:32.000000 pytme-0.1.9/tme/analyzer.py
-drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-03-03 21:07:03.081892 pytme-0.1.9/tme/backends/
--rw-r--r--   0 vmaurer    (502) staff       (20)     4366 2024-01-17 13:29:37.000000 pytme-0.1.9/tme/backends/__init__.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    10648 2024-02-01 18:19:37.000000 pytme-0.1.9/tme/backends/cupy_backend.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    29311 2024-01-17 20:33:54.000000 pytme-0.1.9/tme/backends/matching_backend.py
--rw-r--r--   0 vmaurer    (502) staff       (20)     8467 2024-01-17 20:33:54.000000 pytme-0.1.9/tme/backends/mlx_backend.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    26200 2024-02-29 16:39:57.000000 pytme-0.1.9/tme/backends/npfftw_backend.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    17978 2024-02-05 16:48:44.000000 pytme-0.1.9/tme/backends/pytorch_backend.py
-drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-03-03 21:07:03.156453 pytme-0.1.9/tme/data/
--rw-r--r--   0 vmaurer    (502) staff       (20)        0 2023-10-21 17:05:05.000000 pytme-0.1.9/tme/data/__init__.py
--rw-r--r--   0 vmaurer    (502) staff       (20)   296768 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/c48n309.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)   506048 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/c48n527.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)     8768 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/c48n9.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)     1088 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/c48u1.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)  1107008 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/c48u1153.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)  1153088 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/c48u1201.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)  1575488 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/c48u1641.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)   173888 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/c48u181.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)  2130368 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/c48u2219.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)    26048 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/c48u27.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)  2829248 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/c48u2947.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)  3583808 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/c48u3733.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)  4559168 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/c48u4749.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)  5643968 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/c48u5879.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)  6826688 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/c48u7111.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)   782528 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/c48u815.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)    79808 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/c48u83.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)  8303168 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/c48u8649.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)     2528 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/c600v.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)    14528 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/c600vc.npy
--rw-r--r--   0 vmaurer    (502) staff       (20)      750 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/metadata.yaml
--rwxr-xr-x   0 vmaurer    (502) staff       (20)     1333 2023-03-19 10:37:24.000000 pytme-0.1.9/tme/data/quat_to_numpy.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    84326 2024-02-19 15:11:48.000000 pytme-0.1.9/tme/density.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    23625 2023-10-17 21:31:49.000000 pytme-0.1.9/tme/helpers.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    22243 2024-03-03 13:29:40.000000 pytme-0.1.9/tme/matching_data.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    54874 2024-03-02 16:33:41.000000 pytme-0.1.9/tme/matching_exhaustive.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    11245 2023-12-11 19:08:42.000000 pytme-0.1.9/tme/matching_memory.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    37388 2023-11-23 14:13:49.000000 pytme-0.1.9/tme/matching_optimization.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    37227 2024-03-01 11:25:24.000000 pytme-0.1.9/tme/matching_utils.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    13887 2024-01-25 20:44:11.000000 pytme-0.1.9/tme/parser.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    50631 2024-02-19 15:11:48.000000 pytme-0.1.9/tme/preprocessor.py
--rw-r--r--   0 vmaurer    (502) staff       (20)    54134 2023-12-04 12:00:08.000000 pytme-0.1.9/tme/structure.py
--rw-r--r--   0 vmaurer    (502) staff       (20)      295 2024-01-17 13:38:48.000000 pytme-0.1.9/tme/types.py
+drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-20 17:25:09.230805 pytme-0.2.0b0/
+-rw-r--r--   0 vmaurer    (502) staff       (20)    18467 2023-10-21 17:18:54.000000 pytme-0.2.0b0/LICENSE
+-rw-r--r--   0 vmaurer    (502) staff       (20)     1411 2024-04-20 17:06:53.000000 pytme-0.2.0b0/MANIFEST.in
+-rw-r--r--   0 vmaurer    (502) staff       (20)     2163 2024-04-20 17:25:09.230580 pytme-0.2.0b0/PKG-INFO
+-rw-r--r--   0 vmaurer    (502) staff       (20)     1348 2024-04-20 17:06:53.000000 pytme-0.2.0b0/README.md
+-rw-r--r--   0 vmaurer    (502) staff       (20)     1243 2024-04-20 17:06:53.000000 pytme-0.2.0b0/pyproject.toml
+drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-20 17:25:09.230302 pytme-0.2.0b0/pytme.egg-info/
+-rw-r--r--   0 vmaurer    (502) staff       (20)     1295 2024-04-20 17:25:09.000000 pytme-0.2.0b0/pytme.egg-info/SOURCES.txt
+drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-20 17:25:09.152687 pytme-0.2.0b0/scripts/
+-rw-r--r--   0 vmaurer    (502) staff       (20)        0 2023-12-11 19:10:01.000000 pytme-0.2.0b0/scripts/__init__.py
+-rwxr-xr-x   0 vmaurer    (502) staff       (20)     2768 2024-01-17 20:33:54.000000 pytme-0.2.0b0/scripts/estimate_ram_usage.py
+-rwxr-xr-x   0 vmaurer    (502) staff       (20)     6871 2024-04-12 21:15:08.000000 pytme-0.2.0b0/scripts/extract_candidates.py
+-rwxr-xr-x   0 vmaurer    (502) staff       (20)    26664 2024-04-20 16:07:07.000000 pytme-0.2.0b0/scripts/match_template.py
+-rwxr-xr-x   0 vmaurer    (502) staff       (20)    28989 2024-04-12 21:04:56.000000 pytme-0.2.0b0/scripts/match_template_filters.py
+-rwxr-xr-x   0 vmaurer    (502) staff       (20)    21012 2024-04-12 21:11:31.000000 pytme-0.2.0b0/scripts/postprocess.py
+-rwxr-xr-x   0 vmaurer    (502) staff       (20)     2528 2023-10-17 21:34:50.000000 pytme-0.2.0b0/scripts/preprocess.py
+-rwxr-xr-x   0 vmaurer    (502) staff       (20)    35190 2024-04-04 15:36:03.000000 pytme-0.2.0b0/scripts/preprocessor_gui.py
+-rwxr-xr-x   0 vmaurer    (502) staff       (20)     7077 2024-03-04 16:26:50.000000 pytme-0.2.0b0/scripts/refine_matches.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)       38 2024-04-20 17:25:09.230847 pytme-0.2.0b0/setup.cfg
+-rw-r--r--   0 vmaurer    (502) staff       (20)     1846 2024-04-20 17:06:53.000000 pytme-0.2.0b0/setup.py
+drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-20 17:25:09.153081 pytme-0.2.0b0/src/
+-rw-r--r--   0 vmaurer    (502) staff       (20)    12912 2024-04-07 20:40:48.000000 pytme-0.2.0b0/src/extensions.cpp
+drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-20 17:25:09.156102 pytme-0.2.0b0/tme/
+-rw-r--r--   0 vmaurer    (502) staff       (20)      251 2024-04-17 07:48:39.000000 pytme-0.2.0b0/tme/__init__.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)       23 2024-04-20 16:16:07.000000 pytme-0.2.0b0/tme/__version__.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    55632 2024-04-20 14:56:49.000000 pytme-0.2.0b0/tme/analyzer.py
+drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-20 17:25:09.158240 pytme-0.2.0b0/tme/backends/
+-rw-r--r--   0 vmaurer    (502) staff       (20)     4366 2024-01-17 13:29:37.000000 pytme-0.2.0b0/tme/backends/__init__.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    13145 2024-04-20 16:51:24.000000 pytme-0.2.0b0/tme/backends/cupy_backend.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    29311 2024-01-17 20:33:54.000000 pytme-0.2.0b0/tme/backends/matching_backend.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)     8467 2024-01-17 20:33:54.000000 pytme-0.2.0b0/tme/backends/mlx_backend.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    27451 2024-04-20 12:48:22.000000 pytme-0.2.0b0/tme/backends/npfftw_backend.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    18293 2024-04-20 12:48:41.000000 pytme-0.2.0b0/tme/backends/pytorch_backend.py
+drwxr-xr-x   0 vmaurer    (502) staff       (20)        0 2024-04-20 17:25:09.228452 pytme-0.2.0b0/tme/data/
+-rw-r--r--   0 vmaurer    (502) staff       (20)        0 2023-10-21 17:05:05.000000 pytme-0.2.0b0/tme/data/__init__.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)   296768 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48n309.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)   506048 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48n527.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)     8768 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48n9.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)     1088 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u1.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)  1107008 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u1153.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)  1153088 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u1201.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)  1575488 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u1641.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)   173888 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u181.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)  2130368 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u2219.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)    26048 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u27.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)  2829248 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u2947.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)  3583808 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u3733.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)  4559168 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u4749.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)  5643968 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u5879.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)  6826688 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u7111.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)   782528 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u815.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)    79808 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u83.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)  8303168 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c48u8649.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)     2528 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c600v.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)    14528 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/c600vc.npy
+-rw-r--r--   0 vmaurer    (502) staff       (20)      750 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/metadata.yaml
+-rwxr-xr-x   0 vmaurer    (502) staff       (20)     1333 2023-03-19 10:37:24.000000 pytme-0.2.0b0/tme/data/quat_to_numpy.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    87856 2024-04-20 16:08:44.000000 pytme-0.2.0b0/tme/density.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    23625 2023-10-17 21:31:49.000000 pytme-0.2.0b0/tme/helpers.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)     6725 2024-03-29 15:18:59.000000 pytme-0.2.0b0/tme/matching_constrained.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    24135 2024-04-20 13:45:53.000000 pytme-0.2.0b0/tme/matching_data.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    59531 2024-04-20 16:09:35.000000 pytme-0.2.0b0/tme/matching_exhaustive.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    11273 2024-04-05 10:38:07.000000 pytme-0.2.0b0/tme/matching_memory.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    41138 2024-04-18 21:23:50.000000 pytme-0.2.0b0/tme/matching_optimization.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    42504 2024-04-20 16:45:46.000000 pytme-0.2.0b0/tme/matching_utils.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    19118 2024-04-18 21:23:50.000000 pytme-0.2.0b0/tme/orientations.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    13887 2024-01-25 20:44:11.000000 pytme-0.2.0b0/tme/parser.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    50760 2024-04-17 07:45:43.000000 pytme-0.2.0b0/tme/preprocessor.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)    52465 2024-04-18 15:47:36.000000 pytme-0.2.0b0/tme/structure.py
+-rw-r--r--   0 vmaurer    (502) staff       (20)      295 2024-01-17 13:38:48.000000 pytme-0.2.0b0/tme/types.py
```

### Comparing `pytme-0.1.9/LICENSE` & `pytme-0.2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/MANIFEST.in` & `pytme-0.2.0b0/MANIFEST.in`

 * *Files 6% similar despite different names*

```diff
@@ -56,16 +56,18 @@
 prune target/
 
 # Other exclusions
 global-exclude .DS_Store
 global-exclude .gitconfig
 global-exclude *.pickle
 prune tme/temp
+prune tme/preprocessing
 global-exclude doc/compileApiReference.sh
 prune public
 global-exclude tme/matching_backend.py
 prune doc/_build
 prune doc/reference/api
 global-exclude tme/scoring.py
 global-exclude tme/package.py
+global-exclude tme/transforms.py
 global-exclude tme/tests/test_packaging.py
 global-exclude scripts/match_template_devel.py
```

### Comparing `pytme-0.1.9/PKG-INFO` & `pytme-0.2.0b0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytme
-Version: 0.1.9
+Version: 0.2.0b0
 Summary: Python Template Matching Engine
 Author: Valentin Maurer
 Author-email: Valentin Maurer <valentin.maurer@embl-hamburg.de>
 License: Proprietary
 Project-URL: Homepage, https://github.com/KosinskiLab/pyTME
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,16 @@
 Requires-Dist: PyWavelets>=1.2.0
 Requires-Dist: PyYAML>=6.0
 Requires-Dist: scikit-image>=0.19.0
 Requires-Dist: scikit_learn>=1.2.1
 Requires-Dist: scipy>=1.9.1
 Requires-Dist: pybind11
 Requires-Dist: psutil
+Requires-Dist: tifffile[all]
+Requires-Dist: h5py
 
 # Python Template Matching Engine (PyTME)
 
 A software for template matching on electron microscopy data.
 
 📖 **[Official Documentation](https://kosinskilab.github.io/pyTME/)** | 🚀 **[Installation Guide](https://kosinskilab.github.io/pyTME/quickstart/installation.html)** | 📚 **[API Reference](https://kosinskilab.github.io/pyTME/reference/index.html)**
```

### Comparing `pytme-0.1.9/README.md` & `pytme-0.2.0b0/README.md`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/pyproject.toml` & `pytme-0.2.0b0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name="pytme"
 authors = [
   { name = "Valentin Maurer", email = "valentin.maurer@embl-hamburg.de" },
 ]
-version="0.1.9"
+version="0.2.0b"
 description="Python Template Matching Engine"
 readme="README.md"
 requires-python = ">=3.11"
 dependencies=[
     "mrcfile>=1.4.3",
     "numpy>=1.22.2",
     "pyfftw>=0.13.1",
@@ -19,14 +19,16 @@
     "PyWavelets>=1.2.0",
     "PyYAML>=6.0",
     "scikit-image>=0.19.0",
     "scikit_learn>=1.2.1",
     "scipy>=1.9.1",
     "pybind11",
     "psutil",
+    "tifffile[all]",
+    "h5py"
 ]
 license = {text = "Proprietary"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
```

### Comparing `pytme-0.1.9/pytme.egg-info/SOURCES.txt` & `pytme-0.2.0b0/pytme.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 scripts/__init__.py
 scripts/estimate_ram_usage.py
+scripts/extract_candidates.py
 scripts/match_template.py
+scripts/match_template_filters.py
 scripts/postprocess.py
 scripts/preprocess.py
 scripts/preprocessor_gui.py
+scripts/refine_matches.py
 src/extensions.cpp
 tme/__init__.py
 tme/__version__.py
 tme/analyzer.py
 tme/density.py
 tme/helpers.py
+tme/matching_constrained.py
 tme/matching_data.py
 tme/matching_exhaustive.py
 tme/matching_memory.py
 tme/matching_optimization.py
 tme/matching_utils.py
+tme/orientations.py
 tme/parser.py
 tme/preprocessor.py
 tme/structure.py
 tme/types.py
 tme/backends/__init__.py
 tme/backends/cupy_backend.py
 tme/backends/matching_backend.py
```

### Comparing `pytme-0.1.9/scripts/estimate_ram_usage.py` & `pytme-0.2.0b0/scripts/estimate_ram_usage.py`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/scripts/match_template.py` & `pytme-0.2.0b0/scripts/match_template_filters.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,34 +7,36 @@
 """
 import os
 import argparse
 import warnings
 import importlib.util
 from sys import exit
 from time import time
+from typing import Tuple
 from copy import deepcopy
 from os.path import abspath
 
 import numpy as np
 
-from tme import Density, Preprocessor, __version__
+from tme import Density, __version__
 from tme.matching_utils import (
     get_rotation_matrices,
     compute_parallelization_schedule,
     euler_from_rotationmatrix,
     scramble_phases,
     generate_tempfile_name,
     write_pickle,
 )
 from tme.matching_exhaustive import scan_subsets, MATCHING_EXHAUSTIVE_REGISTER
 from tme.matching_data import MatchingData
 from tme.analyzer import (
     MaxScoreOverRotations,
     PeakCallerMaximumFilter,
 )
+from tme.preprocessing import Compose
 from tme.backends import backend
 
 
 def get_func_fullname(func) -> str:
     """Returns the full name of the given function, including its module."""
     return f"<function '{func.__module__}.{func.__name__}'>"
 
@@ -148,263 +150,290 @@
         data_mask.adjust_box(box)
 
     return True
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Perform template matching.")
-    parser.add_argument(
+
+    io_group = parser.add_argument_group("Input / Output")
+    io_group.add_argument(
         "-m",
         "--target",
         dest="target",
         type=str,
         required=True,
-        help="Path to a target in CCP4/MRC format.",
+        help="Path to a target in CCP4/MRC, EM, H5 or another format supported by "
+        "tme.density.Density.from_file "
+        "https://kosinskilab.github.io/pyTME/reference/api/tme.density.Density.from_file.html",
     )
-    parser.add_argument(
+    io_group.add_argument(
         "--target_mask",
         dest="target_mask",
         type=str,
         required=False,
-        help="Path to a mask for the target target in CCP4/MRC format.",
-    )
-    parser.add_argument(
-        "--cutoff_target",
-        dest="cutoff_target",
-        type=float,
-        required=False,
-        help="Target contour level (used for cropping).",
-        default=None,
+        help="Path to a mask for the target in a supported format (see target).",
     )
-    parser.add_argument(
-        "--cutoff_template",
-        dest="cutoff_template",
-        type=float,
-        required=False,
-        help="Template contour level (used for cropping).",
-        default=None,
-    )
-    parser.add_argument(
-        "--no_centering",
-        dest="no_centering",
-        action="store_true",
-        help="If set, assumes the template is centered and omits centering.",
-    )
-    parser.add_argument(
+    io_group.add_argument(
         "-i",
         "--template",
         dest="template",
         type=str,
         required=True,
-        help="Path to a template in PDB/MMCIF or CCP4/MRC format.",
+        help="Path to a template in PDB/MMCIF or other supported formats (see target).",
     )
-    parser.add_argument(
+    io_group.add_argument(
         "--template_mask",
         dest="template_mask",
         type=str,
         required=False,
-        help="Path to a mask for the template in CCP4/MRC format.",
+        help="Path to a mask for the template in a supported format (see target).",
     )
-    parser.add_argument(
+    io_group.add_argument(
         "-o",
+        "--output",
         dest="output",
         type=str,
         required=False,
         default="output.pickle",
-        help="Path to output pickle file.",
+        help="Path to the output pickle file.",
     )
-    parser.add_argument(
+    io_group.add_argument(
+        "--invert_target_contrast",
+        dest="invert_target_contrast",
+        action="store_true",
+        default=False,
+        help="Invert the target's contrast and rescale linearly between zero and one. "
+        "This option is intended for targets where templates to-be-matched have "
+        "negative values, e.g. tomograms.",
+    )
+    io_group.add_argument(
+        "--scramble_phases",
+        dest="scramble_phases",
+        action="store_true",
+        default=False,
+        help="Phase scramble the template to generate a noise score background.",
+    )
+
+    scoring_group = parser.add_argument_group("Scoring")
+    scoring_group.add_argument(
         "-s",
         dest="score",
         type=str,
         default="FLCSphericalMask",
+        choices=list(MATCHING_EXHAUSTIVE_REGISTER.keys()),
         help="Template matching scoring function.",
-        choices=MATCHING_EXHAUSTIVE_REGISTER.keys(),
-    )
-    parser.add_argument(
-        "-n",
-        dest="cores",
-        required=False,
-        type=int,
-        default=4,
-        help="Number of cores used for template matching.",
-    )
-    parser.add_argument(
-        "-r",
-        "--ram",
-        dest="memory",
-        required=False,
-        type=int,
-        default=None,
-        help="Amount of memory that can be used in bytes.",
     )
-    parser.add_argument(
-        "--memory_scaling",
-        dest="memory_scaling",
-        required=False,
-        type=check_positive,
-        default=0.85,
-        help="Fraction of available memory that can be used."
-        "Defaults to 0.85. Ignored if --ram is set",
-    )
-    parser.add_argument(
+    scoring_group.add_argument(
         "-a",
         dest="angular_sampling",
         type=check_positive,
         default=40.0,
         help="Angular sampling rate for template matching. "
         "A lower number yields more rotations. Values >= 180 sample only the identity.",
     )
-    parser.add_argument(
-        "-p",
-        dest="peak_calling",
-        action="store_true",
-        default=False,
-        help="When set perform peak calling instead of score aggregation.",
+
+    computation_group = parser.add_argument_group("Computation")
+    computation_group.add_argument(
+        "-n",
+        dest="cores",
+        required=False,
+        type=int,
+        default=4,
+        help="Number of cores used for template matching.",
     )
-    parser.add_argument(
+    computation_group.add_argument(
         "--use_gpu",
         dest="use_gpu",
         action="store_true",
         default=False,
         help="Whether to perform computations on the GPU.",
     )
-    parser.add_argument(
+    computation_group.add_argument(
         "--gpu_indices",
         dest="gpu_indices",
         type=str,
         default=None,
         help="Comma-separated list of GPU indices to use. For example,"
         " 0,1 for the first and second GPU. Only used if --use_gpu is set."
         " If not provided but --use_gpu is set, CUDA_VISIBLE_DEVICES will"
         " be respected.",
     )
-    parser.add_argument(
-        "--invert_target_contrast",
-        dest="invert_target_contrast",
-        action="store_true",
-        default=False,
-        help="Invert the target contrast via multiplication with negative one and"
-        " linear rescaling between zero and one. Note that this might lead to"
-        " different baseline scores of individual target splits when using"
-        " unnormalized scores. This option is intended for targets, where the"
-        " object to-be-matched has negative values, i.e. tomograms.",
-    )
-    parser.add_argument(
-        "--no_edge_padding",
-        dest="no_edge_padding",
-        action="store_true",
-        default=False,
-        help="Whether to pad the edges of the target. This is useful, if the target"
-        " has a well defined bounding box, e.g. a density map.",
-    )
-    parser.add_argument(
-        "--no_fourier_padding",
-        dest="no_fourier_padding",
-        action="store_true",
-        default=False,
-        help="Whether input arrays should be zero-padded to the full convolution shape"
-        " for numerical stability. When working with very large targets such as"
-        " tomograms it is safe to use this flag and benefit from the performance gain.",
-    )
-    parser.add_argument(
-        "--scramble_phases",
-        dest="scramble_phases",
-        action="store_true",
-        default=False,
-        help="Whether to phase scramble the template for subsequent normalization.",
-    )
-    parser.add_argument(
-        "--interpolation_order",
-        dest="interpolation_order",
+    computation_group.add_argument(
+        "-r",
+        "--ram",
+        dest="memory",
         required=False,
         type=int,
-        default=3,
-        help="Spline interpolation used during rotations. If less than zero"
-        " no interpolation is performed.",
+        default=None,
+        help="Amount of memory that can be used in bytes.",
+    )
+    computation_group.add_argument(
+        "--memory_scaling",
+        dest="memory_scaling",
+        required=False,
+        type=float,
+        default=0.85,
+        help="Fraction of available memory that can be used. Defaults to 0.85 and is "
+        "ignored if --ram is set",
     )
-    parser.add_argument(
+    computation_group.add_argument(
         "--use_mixed_precision",
         dest="use_mixed_precision",
         action="store_true",
         default=False,
         help="Use float16 for real values operations where possible.",
     )
-    parser.add_argument(
+    computation_group.add_argument(
         "--use_memmap",
         dest="use_memmap",
         action="store_true",
         default=False,
-        help="Use memmaps to offload large data objects to disk. This is"
-        " particularly useful for large inputs when using --use_gpu..",
+        help="Use memmaps to offload large data objects to disk. "
+        "Particularly useful for large inputs in combination with --use_gpu.",
     )
-    parser.add_argument(
+    computation_group.add_argument(
         "--temp_directory",
         dest="temp_directory",
         default=None,
-        help="Directory for temporary objects. Faster I/O typically improves runtime.",
+        help="Directory for temporary objects. Faster I/O improves runtime.",
+    )
+
+    filter_group = parser.add_argument_group("Filters")
+    filter_group.add_argument(
+        "--lowpass",
+        dest="lowpass",
+        type=float,
+        required=False,
+        help="Resolution to lowpass filter template and target to in the same unit "
+        "as the sampling rate of template and target (typically Ångstrom).",
     )
-    parser.add_argument(
-        "--gaussian_sigma",
-        dest="gaussian_sigma",
+    filter_group.add_argument(
+        "--highpass",
+        dest="highpass",
         type=float,
         required=False,
-        help="Sigma parameter for Gaussian filtering the template.",
+        help="Resolution to highpass filter template and target to in the same unit "
+        "as the sampling rate of template and target (typically Ångstrom).",
     )
-    parser.add_argument(
-        "--bandpass_band",
-        dest="bandpass_band",
+    filter_group.add_argument(
+        "--whiten_spectrum",
+        dest="whiten_spectrum",
+        action="store_true",
+        default=False,
+        help="Apply spectral whitening to template and target based on target spectrum.",
+    )
+    filter_group.add_argument(
+        "--wedge_axes",
+        dest="wedge_axes",
         type=str,
         required=False,
-        help="Comma separated start and stop frequency for bandpass filtering the"
-        " template, e.g. 0.1, 0.5",
+        default="0,2",
+        help="Indices of wedge opening and tilt axis, e.g. 0,2 for a wedge that is open "
+        "in z-direction and tilted over the x axis.",
     )
-    parser.add_argument(
-        "--bandpass_smooth",
-        dest="bandpass_smooth",
-        type=float,
+    filter_group.add_argument(
+        "--tilt_angles",
+        dest="tilt_angles",
+        type=str,
         required=False,
         default=None,
-        help="Smooth parameter for the bandpass filter.",
-    )
-    parser.add_argument(
-        "--tilt_range",
-        dest="tilt_range",
+        help="Path to a file with angles and corresponding doses, or comma separated "
+        "start and stop stage tilt angle, e.g. 50,45, which yields a continuous wedge "
+        "mask. Alternatively, a tilt step size can be specified like 50,45:5.0 to "
+        "sample 5.0 degree tilt angle steps.",
+    )
+    filter_group.add_argument(
+        "--tilt_weighting",
+        dest="tilt_weighting",
         type=str,
         required=False,
-        help="Comma separated start and stop stage tilt angle, e.g. '50,45'. Used"
-        " to create a wedge mask to be applied to the template.",
-    )
-    parser.add_argument(
-        "--tilt_step",
-        dest="tilt_step",
-        type=float,
+        choices=["angle", "relion", "grigorieff"],
+        default=None,
+        help="Weighting scheme used to reweight individual tilts. Available options: "
+        "angle (cosine based weighting), "
+        "relion (relion formalism for wedge weighting ),"
+        "grigorieff (exposure filter as defined in Grant and Grigorieff 2015)."
+        "",
+    )
+    filter_group.add_argument(
+        "--ctf_file",
+        dest="ctf_file",
+        type=str,
         required=False,
         default=None,
-        help="Step size between tilts, e.g. '5'. When set the wedge mask"
-        " reflects the individual tilts, otherwise a continuous mask is used.",
+        help="Path to a file with CTF parameters.",
     )
-    parser.add_argument(
-        "--wedge_axes",
-        dest="wedge_axes",
-        type=str,
+
+    performance_group = parser.add_argument_group("Performance")
+    performance_group.add_argument(
+        "--cutoff_target",
+        dest="cutoff_target",
+        type=float,
         required=False,
-        default="0,2",
-        help="Axis index of wedge opening and tilt axis, e.g. 0,2 for a wedge that is open in"
-        " z and tilted over x.",
+        default=None,
+        help="Target contour level (used for cropping).",
     )
-    parser.add_argument(
-        "--wedge_smooth",
-        dest="wedge_smooth",
+    performance_group.add_argument(
+        "--cutoff_template",
+        dest="cutoff_template",
         type=float,
         required=False,
         default=None,
-        help="Gaussian sigma used to smooth the wedge mask.",
+        help="Template contour level (used for cropping).",
+    )
+    performance_group.add_argument(
+        "--no_centering",
+        dest="no_centering",
+        action="store_true",
+        help="Assumes the template is already centered and omits centering.",
+    )
+    performance_group.add_argument(
+        "--no_edge_padding",
+        dest="no_edge_padding",
+        action="store_true",
+        default=False,
+        help="Whether to not pad the edges of the target. Can be set if the target"
+        " has a well defined bounding box, e.g. a masked reconstruction.",
+    )
+    performance_group.add_argument(
+        "--no_fourier_padding",
+        dest="no_fourier_padding",
+        action="store_true",
+        default=False,
+        help="Whether input arrays should not be zero-padded to full convolution shape "
+        "for numerical stability. When working with very large targets, e.g. tomograms, "
+        "it is safe to use this flag and benefit from the performance gain.",
+    )
+    performance_group.add_argument(
+        "--interpolation_order",
+        dest="interpolation_order",
+        required=False,
+        type=int,
+        default=3,
+        help="Spline interpolation used for template rotations. If less than zero "
+        "no interpolation is performed.",
     )
 
+    analyzer_group = parser.add_argument_group("Analyzer")
+    analyzer_group.add_argument(
+        "--score_threshold",
+        dest="score_threshold",
+        required=False,
+        type=float,
+        default=0,
+        help="Minimum template matching scores to consider for analysis.",
+    )
+    analyzer_group.add_argument(
+        "-p",
+        dest="peak_calling",
+        action="store_true",
+        default=False,
+        help="Perform peak calling instead of score aggregation.",
+    )
     args = parser.parse_args()
 
     if args.interpolation_order < 0:
         args.interpolation_order = None
 
     if args.temp_directory is None:
         default = abspath(".")
@@ -434,17 +463,104 @@
                 "Assuming device 0.",
             )
             os.environ["CUDA_VISIBLE_DEVICES"] = "0"
         args.gpu_indices = [
             int(x) for x in os.environ["CUDA_VISIBLE_DEVICES"].split(",")
         ]
 
+    if args.wedge_axes is not None:
+        args.wedge_axes = [int(x) for x in args.wedge_axes.split(",")]
+
+    if args.tilt_angles is not None and args.wedge_axes is None:
+        raise ValueError("Wedge axes have to be specified with tilt angles.")
+
+    if args.ctf_file is not None and args.wedge_axes is None:
+        raise ValueError("Wedge axes have to be specified with CTF parameters.")
+    if args.ctf_file is not None and args.tilt_angles is None:
+        raise ValueError("Angles have to be specified with CTF parameters.")
+
     return args
 
 
+def setup_filter(args, template: Density, target: Density) -> Tuple[Compose, Compose]:
+    from tme.preprocessing import LinearWhiteningFilter, BandPassFilter
+
+    template_filter, target_filter = [], []
+    if args.tilt_angles is not None:
+        from tme.preprocessing.tilt_series import (
+            Wedge,
+            WedgeReconstructed,
+            ReconstructFromTilt,
+        )
+
+        try:
+            wedge = Wedge.from_file(args.tilt_angles)
+            wedge.weight_type = args.tilt_weighting
+        except FileNotFoundError:
+            tilt_step = None
+            tilt_start, tilt_stop = args.tilt_angles.split(",")
+            if ":" in tilt_stop:
+                tilt_stop, tilt_step = tilt_stop.split(":")
+            tilt_start, tilt_stop = float(tilt_start), float(tilt_stop)
+            tilt_angles = None
+            if tilt_step is not None:
+                tilt_step = float(tilt_step)
+                tilt_angles = np.arange(
+                    -tilt_start, tilt_stop + tilt_step, tilt_step
+                ).tolist()
+            wedge = WedgeReconstructed(
+                angles=tilt_angles,
+                start_tilt=tilt_start,
+                stop_tilt=tilt_stop,
+            )
+        wedge.opening_axis = args.wedge_axes[0]
+        wedge.tilt_axis = args.wedge_axes[1]
+        wedge.sampling_rate = template.sampling_rate
+        template_filter.append(wedge)
+        if not isinstance(wedge, WedgeReconstructed):
+            template_filter.append(ReconstructFromTilt())
+
+    if args.ctf_file is not None:
+        from tme.preprocessing.tilt_series import CTF
+
+        ctf = CTF.from_file(args.ctf_file)
+        ctf.tilt_axis = args.wedge_axes[1]
+        ctf.opening_axis = args.wedge_axes[0]
+        template_filter.append(ctf)
+        if isinstance(template_filter[-1], ReconstructFromTilt):
+            template_filter.insert(-1, ctf)
+        else:
+            template_filter.insert(0, ctf)
+            template_filter.isnert(1, ReconstructFromTilt())
+
+    if args.lowpass or args.highpass is not None:
+        from tme.preprocessing import BandPassFilter
+
+        bandpass = BandPassFilter(
+            use_gaussian=True,
+            lowpass=args.lowpass,
+            highpass=args.highpass,
+            sampling_rate=template.sampling_rate,
+        )
+        template_filter.append(bandpass)
+        target_filter.append(bandpass)
+
+    if args.whiten_spectrum:
+        from tme.preprocessing import LinearWhiteningFilter
+
+        whitening_filter = LinearWhiteningFilter()
+        template_filter.append(whitening_filter)
+        target_filter.append(whitening_filter)
+
+    template_filter = Compose(template_filter) if len(template_filter) else None
+    target_filter = Compose(target_filter) if len(target_filter) else None
+
+    return template_filter, target_filter
+
+
 def main():
     args = parse_args()
     print_entry()
 
     target = Density.from_file(args.target, use_memmap=True)
 
     try:
@@ -510,59 +626,14 @@
         data={
             "Initial Shape": initial_shape,
             "Sampling Rate": tuple(np.round(template.sampling_rate, 2)),
             "Final Shape": template.shape,
         },
     )
 
-    template_filter = {}
-    if args.gaussian_sigma is not None:
-        template.data = Preprocessor().gaussian_filter(
-            sigma=args.gaussian_sigma, template=template.data
-        )
-
-    if args.bandpass_band is not None:
-        bandpass_start, bandpass_stop = [
-            float(x) for x in args.bandpass_band.split(",")
-        ]
-        if args.bandpass_smooth is None:
-            args.bandpass_smooth = 0
-
-        template_filter["bandpass_mask"] = {
-            "minimum_frequency": bandpass_start,
-            "maximum_frequency": bandpass_stop,
-            "gaussian_sigma": args.bandpass_smooth,
-        }
-
-    if args.tilt_range is not None:
-        args.wedge_smooth if args.wedge_smooth is not None else 0
-        tilt_start, tilt_stop = [float(x) for x in args.tilt_range.split(",")]
-        opening_axis, tilt_axis = [int(x) for x in args.wedge_axes.split(",")]
-
-        if args.tilt_step is not None:
-            template_filter["step_wedge_mask"] = {
-                "start_tilt": tilt_start,
-                "stop_tilt": tilt_stop,
-                "tilt_step": args.tilt_step,
-                "sigma": args.wedge_smooth,
-                "opening_axis": opening_axis,
-                "tilt_axis": tilt_axis,
-                "omit_negative_frequencies": True,
-            }
-        else:
-            template_filter["continuous_wedge_mask"] = {
-                "start_tilt": tilt_start,
-                "stop_tilt": tilt_stop,
-                "tilt_axis": tilt_axis,
-                "opening_axis": opening_axis,
-                "infinite_plane": True,
-                "sigma": args.wedge_smooth,
-                "omit_negative_frequencies": True,
-            }
-
     if template_mask is None:
         template_mask = template.empty
         if not args.no_centering:
             enclosing_box = template.minimum_enclosing_box(
                 0, use_geometric_center=False
             )
             template_mask.adjust_box(enclosing_box)
@@ -669,30 +740,33 @@
         print(
             "Found no suitable parallelization schedule. Consider increasing"
             " available RAM or decreasing number of cores."
         )
         exit(-1)
 
     analyzer_args = {
-        "score_threshold": 0,
+        "score_threshold": args.score_threshold,
         "number_of_peaks": 1000,
         "convolution_mode": "valid",
         "use_memmap": args.use_memmap,
     }
 
     matching_setup, matching_score = MATCHING_EXHAUSTIVE_REGISTER[args.score]
     matching_data = MatchingData(target=target, template=template.data)
     matching_data.rotations = get_rotation_matrices(
         angular_sampling=args.angular_sampling, dim=target.data.ndim
     )
     if args.angular_sampling >= 180:
         ndim = target.data.ndim
         matching_data.rotations = np.eye(ndim).reshape(1, ndim, ndim)
 
+    template_filter, target_filter = setup_filter(args, template, target)
     matching_data.template_filter = template_filter
+    matching_data.target_filter = target_filter
+
     matching_data._invert_target = args.invert_target_contrast
     if target_mask is not None:
         matching_data.target_mask = target_mask
     if template_mask is not None:
         matching_data.template_mask = template_mask.data
 
     n_splits = np.prod(list(splits.values()))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytme-0.1.9/scripts/postprocess.py` & `pytme-0.2.0b0/tme/orientations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,129 +1,29 @@
 #!python3
-""" CLI to simplify analysing the output of match_template.py.
+""" Handle template matching peaks and convert between formats.
 
-    Copyright (c) 2023 European Molecular Biology Laboratory
+    Copyright (c) 2024 European Molecular Biology Laboratory
 
     Author: Valentin Maurer <valentin.maurer@embl-hamburg.de>
 """
-from os import getcwd
-from os.path import join
-import argparse
-from sys import exit
-from typing import List, Tuple
-from os.path import splitext
+import re
+from collections import deque
 from dataclasses import dataclass
+from typing import List, Tuple, Dict
 
 import numpy as np
 from scipy.spatial.transform import Rotation
-from numpy.typing import NDArray
-
-from tme import Density, Structure
-from tme.analyzer import (
-    PeakCallerSort,
-    PeakCallerMaximumFilter,
-    PeakCallerFast,
-    PeakCallerRecursiveMasking,
-    PeakCallerScipy,
-)
-from tme.matching_utils import (
-    load_pickle,
-    euler_to_rotationmatrix,
-    euler_from_rotationmatrix,
-    centered_mask,
-)
-
-PEAK_CALLERS = {
-    "PeakCallerSort": PeakCallerSort,
-    "PeakCallerMaximumFilter": PeakCallerMaximumFilter,
-    "PeakCallerFast": PeakCallerFast,
-    "PeakCallerRecursiveMasking": PeakCallerRecursiveMasking,
-    "PeakCallerScipy": PeakCallerScipy,
-}
-
-
-def parse_args():
-    parser = argparse.ArgumentParser(
-        description="Peak Calling for Template Matching Outputs"
-    )
-    parser.add_argument(
-        "--input_file",
-        required=True,
-        help="Path to the output of match_template.py.",
-    )
-    parser.add_argument(
-        "--output_prefix",
-        required=True,
-        help="Prefix for the output file name. Extension depends on output_format.",
-    )
-    parser.add_argument(
-        "--number_of_peaks",
-        type=int,
-        default=1000,
-        help="Number of peaks to consider. Note, this is the number of called peaks "
-        ", subject to min_distance and min_boundary_distance filtering. Therefore, the "
-        "returned number of peaks will be at most equal to number_of_peaks. "
-        "Ignored when --orientations is provided.",
-    )
-    parser.add_argument(
-        "--min_distance",
-        type=int,
-        default=5,
-        help="Minimum distance between peaks. Ignored when --orientations is provided.",
-    )
-    parser.add_argument(
-        "--min_boundary_distance",
-        type=int,
-        default=0,
-        help="Minimum distance from target boundaries. Ignored when --orientations "
-        "is provided.",
-    )
-    parser.add_argument(
-        "--mask_edges",
-        action="store_true",
-        default=False,
-        help="Whether to mask edges of the input score array according to the template shape."
-        "Uses twice the value of --min_boundary_distance if boht are provided.",
-    )
-    parser.add_argument(
-        "--wedge_mask",
-        type=str,
-        default=None,
-        help="Path to Fourier space mask. Only considered if output_format is relion.",
-    )
-    parser.add_argument(
-        "--peak_caller",
-        choices=list(PEAK_CALLERS.keys()),
-        default="PeakCallerScipy",
-        help="Peak caller to use for analysis. Ignored if input_file contains peaks or when "
-        "--orientations is provided.",
-    )
-    parser.add_argument(
-        "--orientations",
-        default=None,
-        help="Path to orientations file to overwrite orientations computed from"
-        " match_template.py output.",
-    )
-    parser.add_argument(
-        "--output_format",
-        choices=["orientations", "alignment", "extraction", "relion"],
-        default="orientations",
-        help="Choose the output format. Available formats are: "
-        "orientations (translation, rotation, and score), "
-        "alignment (aligned template to target based on orientations), "
-        "extraction (extract regions around peaks from targets, i.e. subtomograms). "
-        "relion (perform extraction step and generate corresponding star files).",
-    )
-    args = parser.parse_args()
-
-    return args
 
 
 @dataclass
 class Orientations:
+    """
+    Handle template matching peaks and convert between formats.
+    """
+
     #: Return a numpy array with translations of each orientation (n x d).
     translations: np.ndarray
 
     #: Return a numpy array with euler angles of each orientation in zxy format (n x d).
     rotations: np.ndarray
 
     #: Return a numpy array with the score of each orientation (n, ).
@@ -164,36 +64,43 @@
             "rotations",
             "scores",
             "details",
         )
         kwargs = {attr: getattr(self, attr)[indices] for attr in attributes}
         return self.__class__(**kwargs)
 
-    def to_file(self, filename: str, file_format: type, **kwargs) -> None:
+    def to_file(self, filename: str, file_format: type = None, **kwargs) -> None:
         """
         Save the current class instance to a file in the specified format.
 
         Parameters
         ----------
         filename : str
             The name of the file where the orientations will be saved.
-        file_format : type
+        file_format : type, optional
             The format in which to save the orientations. Supported formats are 'text' and 'relion'.
         **kwargs : dict
             Additional keyword arguments specific to the file format.
 
         Raises
         ------
         ValueError
             If an unsupported file format is specified.
         """
         mapping = {
             "text": self._to_text,
             "relion": self._to_relion_star,
+            "dynamo": self._to_dynamo_tbl,
         }
+        if file_format is None:
+            file_format = "text"
+            if filename.lower().endswith(".star"):
+                file_format = "relion"
+            elif filename.lower().endswith(".tbl"):
+                file_format = "dynamo"
 
         func = mapping.get(file_format, None)
         if func is None:
             raise ValueError(
                 f"{file_format} not implemented. Supported are {','.join(mapping.keys())}."
             )
 
@@ -222,14 +129,89 @@
                 translation_string = "\t".join([str(x) for x in translation])
                 angle_string = "\t".join([str(x) for x in angles])
                 _ = ofile.write(
                     f"{translation_string}\t{angle_string}\t{score}\t{detail}\n"
                 )
         return None
 
+    def _to_dynamo_tbl(
+        self,
+        filename: str,
+        name_prefix: str = None,
+        sampling_rate: float = 1.0,
+        subtomogram_size: int = 0,
+    ) -> None:
+        """
+        Save orientations in Dynamo's tbl file format.
+
+        Parameters
+        ----------
+        filename : str
+            The name of the file to save the orientations.
+        sampling_rate : float, optional
+            Subtomogram sampling rate in angstrom per voxel
+
+        Notes
+        -----
+        The file is saved with a standard header used in Dynamo tbl files
+        outlined in [1]_. Each row corresponds to a particular partice.
+
+        References
+        ----------
+        .. [1]  https://wiki.dynamo.biozentrum.unibas.ch/w/index.php/Table
+
+        The file is saved with a standard header used in Dynamo STAR files.
+        Each row in the file corresponds to an orientation.
+        """
+        with open(filename, mode="w", encoding="utf-8") as ofile:
+            for index, (translation, rotation, score, detail) in enumerate(self):
+                rotation = Rotation.from_euler("zyx", rotation, degrees=True)
+                rotation = rotation.as_euler(seq="xyx", degrees=True)
+                out = [
+                    index,
+                    1,
+                    0,
+                    0,
+                    0,
+                    0,
+                    *rotation,
+                    self.scores[index],
+                    self.scores[index],
+                    0,
+                    0,
+                    # Wedge parameters
+                    -90,
+                    90,
+                    -60,
+                    60,
+                    0,
+                    0,
+                    0,
+                    0,
+                    0,
+                    0,
+                    # Coordinate in original volume
+                    *translation[::-1],
+                    0,
+                    0,
+                    0,
+                    0,
+                    0,
+                    0,
+                    0,
+                    0,
+                    sampling_rate,
+                    3,
+                    0,
+                    0,
+                ]
+                _ = ofile.write(" ".join([str(x) for x in out]) + "\n")
+
+        return None
+
     def _to_relion_star(
         self,
         filename: str,
         name_prefix: str = None,
         ctf_image: str = None,
         sampling_rate: float = 1.0,
         subtomogram_size: int = 0,
@@ -319,40 +301,44 @@
                 _ = ofile.write(
                     f"{translation_string}\t{name}\t{angle_string}\t1{ctf_image}\n"
                 )
 
         return None
 
     @classmethod
-    def from_file(cls, filename: str, file_format: type, **kwargs) -> "Orientations":
+    def from_file(
+        cls, filename: str, file_format: type = None, **kwargs
+    ) -> "Orientations":
         """
         Create an instance of :py:class:`Orientations` from a file.
 
         Parameters
         ----------
         filename : str
             The name of the file from which to read the orientations.
-        file_format : type
+        file_format : type, optional
             The format of the file. Currently, only 'text' format is supported.
         **kwargs : dict
             Additional keyword arguments specific to the file format.
 
         Returns
         -------
         :py:class:`Orientations`
             An instance of :py:class:`Orientations` populated with data from the file.
 
         Raises
         ------
         ValueError
             If an unsupported file format is specified.
         """
-        mapping = {
-            "text": cls._from_text,
-        }
+        mapping = {"text": cls._from_text, "relion": cls._from_relion_star}
+        if file_format is None:
+            file_format = "text"
+            if filename.lower().endswith(".star"):
+                file_format = "relion"
 
         func = mapping.get(file_format, None)
         if func is None:
             raise ValueError(
                 f"{file_format} not implemented. Supported are {','.join(mapping.keys())}."
             )
 
@@ -407,219 +393,169 @@
         translation = np.vstack(translation).astype(int)
         rotation = np.vstack(rotation).astype(float)
         score = np.array(score).astype(float)
         detail = np.array(detail).astype(float)
 
         return translation, rotation, score, detail
 
+    @staticmethod
+    def _parse_star(filename: str, delimiter: str = None) -> Dict:
+        pattern = re.compile(r"\s*#.*")
+        with open(filename, mode="r", encoding="utf-8") as infile:
+            data = infile.read()
 
-def load_template(filepath: str, sampling_rate: NDArray) -> "Density":
-    try:
-        template = Density.from_file(filepath)
-        template, _ = template.centered(0)
-        center_of_mass = template.center_of_mass(template.data)
-    except ValueError:
-        template = Structure.from_file(filepath)
-        center_of_mass = template.center_of_mass()[::-1]
-        template = Density.from_structure(template, sampling_rate=sampling_rate)
-
-    return template, center_of_mass
-
-
-def main():
-    args = parse_args()
-    data = load_pickle(args.input_file)
-
-    meta = data[-1]
-    target_origin, _, sampling_rate, cli_args = meta
-
-    if args.orientations is not None:
-        orientations = Orientations.from_file(
-            filename=args.orientations, file_format="text"
-        )
+        data = deque(filter(lambda line: line and line[0] != "#", data.split("\n")))
 
-    else:
-        translations, rotations, scores, details = [], [], [], []
-        # Output is MaxScoreOverRotations
-        if data[0].ndim == data[2].ndim:
-            scores, offset, rotation_array, rotation_mapping, meta = data
-            if args.mask_edges:
-                template, center_of_mass = load_template(
-                    cli_args.template, sampling_rate=sampling_rate
-                )
-                if not cli_args.no_centering:
-                    template, *_ = template.centered(0)
-                mask_size = template.shape
-                if args.min_boundary_distance > 0:
-                    mask_size = 2 * args.min_boundary_distance
-                scores = centered_mask(scores, np.subtract(scores.shape, mask_size) + 1)
-
-            peak_caller = PEAK_CALLERS[args.peak_caller](
-                number_of_peaks=args.number_of_peaks,
-                min_distance=args.min_distance,
-                min_boundary_distance=args.min_boundary_distance,
-            )
-            peak_caller(scores, rotation_matrix=np.eye(3))
-            candidates = peak_caller.merge(
-                candidates=[tuple(peak_caller)],
-                number_of_peaks=args.number_of_peaks,
-                min_distance=args.min_distance,
-                min_boundary_distance=args.min_boundary_distance,
-            )
-            if len(candidates) == 0:
-                exit(
-                    "Found no peaks. Try reducing min_distance or min_boundary_distance."
-                )
+        ret, category, block = {}, None, []
+        while data:
+            line = data.popleft()
+
+            if line.startswith("data") and not line.startswith("_"):
+                if category != line and category is not None:
+                    headers = list(ret[category].keys())
+                    headers = [pattern.sub("", x) for x in headers]
+                    ret[category] = {
+                        header: list(column)
+                        for header, column in zip(headers, zip(*block))
+                    }
+                    block.clear()
+                category = line
+                if category not in ret:
+                    ret[category] = {}
+                continue
 
-            for translation, _, score, detail in zip(*candidates):
-                rotations.append(rotation_mapping[rotation_array[tuple(translation)]])
+            if line.startswith("_"):
+                ret[category][line] = []
+                continue
 
-        else:
-            candidates = data
-            translation, rotation, score, detail, *_ = data
-            for i in range(translation.shape[0]):
-                rotations.append(euler_from_rotationmatrix(rotation[i]))
-
-        rotations = np.vstack(rotations).astype(float)
-        translations, scores, details = candidates[0], candidates[2], candidates[3]
-        orientations = Orientations(
-            translations=translations,
-            rotations=rotations,
-            scores=scores,
-            details=details,
-        )
+            if line.startswith("loop"):
+                continue
 
-    if args.output_format == "orientations":
-        orientations.to_file(filename=f"{args.output_prefix}.tsv", file_format="text")
-        exit(0)
-
-    _, template_extension = splitext(cli_args.template)
-    template, center_of_mass = load_template(
-        filepath=cli_args.template, sampling_rate=sampling_rate
-    )
-    template_is_density, index = isinstance(template, Density), 0
-
-    if args.output_format == "relion":
-        new_shape = np.add(template.shape, np.mod(template.shape, 2))
-        new_shape = np.repeat(new_shape.max(), new_shape.size).astype(int)
-        print(f"Padding template from {template.shape} to {new_shape} for RELION.")
-        template.pad(new_shape)
-
-    if args.output_format in ("extraction", "relion"):
-        target = Density.from_file(cli_args.target)
-
-        if not np.all(np.divide(target.shape, template.shape) > 2):
-            print(
-                "Target might be too small relative to template to extract"
-                " meaningful particles."
-                f" Target : {target.shape}, template : {template.shape}."
-            )
+            line_split = line.split(delimiter)
+            if len(line_split):
+                block.append(line_split)
+
+        headers = list(ret[category].keys())
+        headers = [pattern.sub("", x) for x in headers]
+        ret[category] = {
+            header: list(column) for header, column in zip(headers, zip(*block))
+        }
+        return ret
 
-        peaks = orientations.translations.astype(int)
-        max_shape = np.max(template.shape).astype(int)
-        half_shape = max_shape // 2
-
-        left_pad = half_shape
-        right_pad = np.add(half_shape, max_shape % 2)
-        starts = np.subtract(peaks, left_pad)
-        stops = np.add(peaks, right_pad)
-
-        candidate_starts = np.maximum(starts, 0).astype(int)
-        candidate_stops = np.minimum(stops, target.shape).astype(int)
-        keep_peaks = (
-            np.sum(
-                np.multiply(starts == candidate_starts, stops == candidate_stops),
-                axis=1,
-            )
-            == peaks.shape[1]
+    @classmethod
+    def _from_relion_star(
+        cls, filename: str, delimiter: str = None
+    ) -> Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
+        ret = cls._parse_star(filename=filename, delimiter=delimiter)
+        ret = ret["data_particles"]
+
+        translation = (
+            np.vstack(
+                (ret["_rlnCoordinateZ"], ret["_rlnCoordinateY"], ret["_rlnCoordinateX"])
+            )
+            .astype(np.float32)
+            .astype(int)
+            .T
         )
 
-        orientations = orientations[keep_peaks]
-        working_directory = getcwd()
-        if args.output_format == "relion":
-            orientations.to_file(
-                filename=f"{args.output_prefix}.star",
-                file_format="relion",
-                name_prefix=join(working_directory, args.output_prefix),
-                ctf_image=args.wedge_mask,
-                sampling_rate=target.sampling_rate.max(),
-                subtomogram_size=template.shape[0],
-            )
+        rotation = (
+            np.vstack((ret["_rlnAngleRot"], ret["_rlnAngleTilt"], ret["_rlnAnglePsi"]))
+            .astype(np.float32)
+            .T
+        )
+
+        rotation = Rotation.from_euler("xyx", rotation, degrees=True)
+        rotation = rotation.as_euler(seq="zyx", degrees=True)
+        score = np.ones(translation.shape[0])
+        detail = np.ones(translation.shape[0]) * 1
+
+        return translation, rotation, score, detail
+
+    def get_extraction_slices(
+        self,
+        target_shape: Tuple[int],
+        extraction_shape: Tuple[int],
+        drop_out_of_box: bool = False,
+        return_orientations: bool = False,
+    ) -> "Orientations":
+        """
+        Calculate slices for extracting regions of interest within a larger array.
+
+        Parameters
+        ----------
+        target_shape : Tuple[int]
+            The shape of the target array within which regions are to be extracted.
+        extraction_shape : Tuple[int]
+            The shape of the regions to be extracted.
+        drop_out_of_box : bool, optional
+            If True, drop regions that extend beyond the target array boundary, by default False.
+        return_orientations : bool, optional
+            If True, return orientations along with slices, by default False.
 
-        peaks = peaks[keep_peaks,]
-        starts = starts[keep_peaks,]
-        stops = stops[keep_peaks,]
-        candidate_starts = candidate_starts[keep_peaks,]
-        candidate_stops = candidate_stops[keep_peaks,]
-
-        if not len(peaks):
-            print(
-                "No peak remaining after filtering. Started with"
-                f" {orientations.translations.shape[0]} filtered to {peaks.shape[0]}."
-                " Consider reducing min_distance, increase num_peaks or use"
-                " a different peak caller."
+        Returns
+        -------
+        Union[Tuple[List[slice]], Tuple["Orientations", List[slice], List[slice]]]
+            If return_orientations is False, returns a tuple containing slices for candidate
+            regions and observation regions.
+            If return_orientations is True, returns a tuple containing orientations along
+            with slices for candidate regions and observation regions.
+
+        Raises
+        ------
+        SystemExit
+            If no peak remains after filtering, indicating an error.
+        """
+        left_pad = np.divide(extraction_shape, 2).astype(int)
+        right_pad = np.add(left_pad, np.mod(extraction_shape, 2)).astype(int)
+
+        obs_start = np.subtract(self.translations, left_pad)
+        obs_stop = np.add(self.translations, right_pad)
+
+        cand_start = np.subtract(np.maximum(obs_start, 0), obs_start)
+        cand_stop = np.subtract(obs_stop, np.minimum(obs_stop, target_shape))
+        cand_stop = np.subtract(extraction_shape, cand_stop)
+        obs_start = np.maximum(obs_start, 0)
+        obs_stop = np.minimum(obs_stop, target_shape)
+
+        subset = self
+        if drop_out_of_box:
+            stops = np.subtract(cand_stop, extraction_shape)
+            keep_peaks = (
+                np.sum(
+                    np.multiply(cand_start == 0, stops == 0),
+                    axis=1,
+                )
+                == self.translations.shape[1]
             )
-            exit(-1)
+            n_remaining = keep_peaks.sum()
+            if n_remaining == 0:
+                print(
+                    "No peak remaining after filtering. Started with"
+                    f" {self.translations.shape[0]} filtered to {n_remaining}."
+                    " Consider reducing min_distance, increase num_peaks or use"
+                    " a different peak caller."
+                )
+                exit(-1)
+
+            cand_start = cand_start[keep_peaks,]
+            cand_stop = cand_stop[keep_peaks,]
+            obs_start = obs_start[keep_peaks,]
+            obs_stop = obs_stop[keep_peaks,]
+            subset = self[keep_peaks]
 
-        observation_starts = np.subtract(candidate_starts, starts).astype(int)
-        observation_stops = np.subtract(np.add(max_shape, candidate_stops), stops)
-        observation_stops = observation_stops.astype(int)
+        cand_start, cand_stop = cand_start.astype(int), cand_stop.astype(int)
+        obs_start, obs_stop = obs_start.astype(int), obs_stop.astype(int)
 
         candidate_slices = [
             tuple(slice(s, e) for s, e in zip(start_row, stop_row))
-            for start_row, stop_row in zip(candidate_starts, candidate_stops)
+            for start_row, stop_row in zip(cand_start, cand_stop)
         ]
 
         observation_slices = [
             tuple(slice(s, e) for s, e in zip(start_row, stop_row))
-            for start_row, stop_row in zip(observation_starts, observation_stops)
+            for start_row, stop_row in zip(obs_start, obs_stop)
         ]
-        observations = np.zeros(
-            (len(candidate_slices), max_shape, max_shape, max_shape)
-        )
-
-        slices = zip(candidate_slices, observation_slices)
-        for idx, (cand_slice, obs_slice) in enumerate(slices):
-            observations[idx][:] = np.mean(target.data[cand_slice])
-            observations[idx][obs_slice] = target.data[cand_slice]
-
-        for index in range(observations.shape[0]):
-            out_density = Density(
-                data=observations[index],
-                sampling_rate=sampling_rate,
-                origin=candidate_starts[index] * sampling_rate,
-            )
-            # out_density.data = out_density.data * template_mask.data
-            out_density.to_file(
-                join(working_directory, f"{args.output_prefix}_{index}.mrc")
-            )
-
-        exit(0)
-
-    for translation, angles, *_ in orientations:
-        rotation_matrix = euler_to_rotationmatrix(angles)
-
-        if template_is_density:
-            translation = np.subtract(translation, center_of_mass)
-            transformed_template = template.rigid_transform(
-                rotation_matrix=rotation_matrix
-            )
-            new_origin = np.add(target_origin / sampling_rate, translation)
-            transformed_template.origin = np.multiply(new_origin, sampling_rate)
-        else:
-            new_center_of_mass = np.add(
-                np.multiply(translation, sampling_rate), target_origin
-            )
-            translation = np.subtract(new_center_of_mass, center_of_mass)
-            transformed_template = template.rigid_transform(
-                translation=translation[::-1],
-                rotation_matrix=rotation_matrix[::-1, ::-1],
-            )
-        # template_extension should contain the extension '.'
-        transformed_template.to_file(
-            f"{args.output_prefix}_{index}{template_extension}"
-        )
-        index += 1
 
+        if return_orientations:
+            return subset, candidate_slices, observation_slices
 
-if __name__ == "__main__":
-    main()
+        return candidate_slices, observation_slices
```

### Comparing `pytme-0.1.9/scripts/preprocess.py` & `pytme-0.2.0b0/scripts/preprocess.py`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/scripts/preprocessor_gui.py` & `pytme-0.2.0b0/scripts/preprocessor_gui.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from napari.utils.events import EventedList
 
 from magicgui import widgets
 from qtpy.QtWidgets import QFileDialog
 from numpy.typing import NDArray
 
 from tme import Preprocessor, Density
-from tme.matching_utils import create_mask
+from tme.matching_utils import create_mask, load_pickle
 
 preprocessor = Preprocessor()
 SLIDER_MIN, SLIDER_MAX = 0, 25
 
 
 def gaussian_filter(template: NDArray, sigma: float, **kwargs: dict) -> NDArray:
     return preprocessor.gaussian_filter(template=template, sigma=sigma, **kwargs)
@@ -412,15 +412,20 @@
                 metadata["filter_parameters"] = []
             metadata["filter_parameters"].append({filter_name: kwargs.copy()})
             metadata["used_filter"] = filter_name
             new_layer.metadata = metadata
 
 
 def sphere_mask(
-    template: NDArray, center_x: float, center_y: float, center_z: float, radius: float
+    template: NDArray,
+    center_x: float,
+    center_y: float,
+    center_z: float,
+    radius: float,
+    **kwargs,
 ) -> NDArray:
     return create_mask(
         mask_type="ellipse",
         shape=template.shape,
         center=(center_x, center_y, center_z),
         radius=radius,
     )
@@ -430,14 +435,15 @@
     template: NDArray,
     center_x: float,
     center_y: float,
     center_z: float,
     radius_x: float,
     radius_y: float,
     radius_z: float,
+    **kwargs,
 ) -> NDArray:
     return create_mask(
         mask_type="ellipse",
         shape=template.shape,
         center=(center_x, center_y, center_z),
         radius=(radius_x, radius_y, radius_z),
     )
@@ -447,14 +453,15 @@
     template: NDArray,
     center_x: float,
     center_y: float,
     center_z: float,
     height_x: int,
     height_y: int,
     height_z: int,
+    **kwargs,
 ) -> NDArray:
     return create_mask(
         mask_type="box",
         shape=template.shape,
         center=(center_x, center_y, center_z),
         height=(height_x, height_y, height_z),
     )
@@ -465,14 +472,15 @@
     symmetry_axis: int,
     center_x: float,
     center_y: float,
     center_z: float,
     inner_radius: float,
     outer_radius: float,
     height: int,
+    **kwargs,
 ) -> NDArray:
     return create_mask(
         mask_type="tube",
         shape=template.shape,
         symmetry_axis=symmetry_axis,
         base_center=(center_x, center_y, center_z),
         inner_radius=inner_radius,
@@ -488,14 +496,15 @@
     tilt_step: float = 0,
     opening_axis: int = 0,
     tilt_axis: int = 2,
     gaussian_sigma: float = 0,
     omit_negative_frequencies: bool = False,
     extrude_plane: bool = True,
     infinite_plane: bool = True,
+    **kwargs,
 ) -> NDArray:
     if tilt_step <= 0:
         wedge_mask = preprocessor.continuous_wedge_mask(
             start_tilt=tilt_start,
             stop_tilt=tilt_stop,
             tilt_axis=tilt_axis,
             opening_axis=opening_axis,
@@ -520,36 +529,50 @@
     )
 
     wedge_mask = np.fft.fftshift(wedge_mask)
     return wedge_mask
 
 
 def threshold_mask(
-    template: NDArray, standard_deviation: float = 5.0, invert: bool = False
+    template: NDArray, standard_deviation: float = 5.0, invert: bool = False, **kwargs
 ) -> NDArray:
     template_mean = template.mean()
     template_deviation = standard_deviation * template.std()
     upper = template_mean + template_deviation
     lower = template_mean - template_deviation
     mask = np.logical_and(template > lower, template < upper)
     if invert:
         np.invert(mask, out=mask)
 
     return mask
 
 
-def lowpass_mask(template: NDArray, sigma: float = 1.0):
+def lowpass_mask(template: NDArray, sigma: float = 1.0, **kwargs):
     template = template / template.max()
     template = (template > np.exp(-2)) * 128.0
     template = preprocessor.gaussian_filter(template=template, sigma=sigma)
     mask = template > np.exp(-2)
 
     return mask
 
 
+def shape_mask(template, shapes_layer, expansion_dim):
+    ret = np.zeros_like(template)
+    mask_shape = tuple(x for i, x in enumerate(template.shape) if i != expansion_dim)
+    masks = shapes_layer.to_masks(mask_shape=mask_shape)
+    for index, shape_type in enumerate(shapes_layer.shape_type):
+        mask = np.expand_dims(masks[index], axis=expansion_dim)
+        mask = np.repeat(
+            mask, repeats=template.shape[expansion_dim], axis=expansion_dim
+        )
+        np.logical_or(ret, mask, out=ret)
+
+    return ret
+
+
 class MaskWidget(widgets.Container):
     def __init__(self, viewer):
         super().__init__(layout="vertical")
 
         self.viewer = viewer
         self.action_widgets = []
 
@@ -560,14 +583,15 @@
             "Sphere": sphere_mask,
             "Ellipsoid": ellipsod_mask,
             "Tube": tube_mask,
             "Box": box_mask,
             "Wedge": wedge_mask,
             "Threshold": threshold_mask,
             "Lowpass": lowpass_mask,
+            "Shape": shape_mask,
         }
 
         self.method_dropdown = widgets.ComboBox(
             name="Choose Mask", choices=list(self.methods.keys())
         )
         self.method_dropdown.changed.connect(self._on_method_changed)
 
@@ -577,68 +601,37 @@
 
         self.adapt_button = widgets.PushButton(text="Adapt to layer", enabled=False)
         self.adapt_button.changed.connect(self._update_initial_values)
         self.viewer.layers.selection.events.active.connect(
             self._update_action_button_state
         )
 
-        self.align_button = widgets.PushButton(text="Align to axis", enabled=False)
-        self.align_button.changed.connect(self._align_with_axis)
         self.density_field = widgets.Label()
         # self.density_field.value = f"Positive Density in Mask: {0:.2f}%"
 
+        self.shapes_layer_dropdown = widgets.ComboBox(
+            name="shapes_layer", choices=self._get_shape_layers()
+        )
+        self.viewer.layers.events.inserted.connect(self._update_shape_layer_choices)
+        self.viewer.layers.events.removed.connect(self._update_shape_layer_choices)
+
         self.append(self.method_dropdown)
         self.append(self.adapt_button)
         self.append(self.percentile_range_edit)
 
-        self.append(self.align_button)
         self.append(self.action_button)
         self.append(self.density_field)
 
         # Create GUI for initially selected filtering method
         self._on_method_changed(None)
 
     def _update_action_button_state(self, event):
-        self.align_button.enabled = bool(self.viewer.layers.selection.active)
         self.action_button.enabled = bool(self.viewer.layers.selection.active)
         self.adapt_button.enabled = bool(self.viewer.layers.selection.active)
 
-    def _align_with_axis(self):
-        active_layer = self.viewer.layers.selection.active
-
-        if active_layer.metadata.get("is_aligned", False):
-            return
-
-        coords = np.array(np.where(active_layer.data > 0)).T
-        centered_coords = coords - np.mean(coords, axis=0)
-        cov_matrix = np.cov(centered_coords, rowvar=False)
-
-        eigenvalues, eigenvectors = np.linalg.eigh(cov_matrix)
-        principal_eigenvector = eigenvectors[:, np.argmax(eigenvalues)]
-
-        rotation_axis = np.cross(principal_eigenvector, [1, 0, 0])
-        rotation_angle = np.arccos(np.dot(principal_eigenvector, [1, 0, 0]))
-        k = rotation_axis / np.linalg.norm(rotation_axis)
-        K = np.array([[0, -k[2], k[1]], [k[2], 0, -k[0]], [-k[1], k[0], 0]])
-        rotation_matrix = np.eye(3)
-        rotation_matrix += np.sin(rotation_angle) * K
-        rotation_matrix += (1 - np.cos(rotation_angle)) * np.dot(K, K)
-
-        rotated_data = Density.rotate_array(
-            arr=active_layer.data,
-            rotation_matrix=rotation_matrix,
-            use_geometric_center=False,
-            order=1,
-        )
-        eps = np.finfo(rotated_data.dtype).eps
-        rotated_data[rotated_data < eps] = 0
-
-        active_layer.metadata["is_aligned"] = True
-        active_layer.data = rotated_data
-
     def _update_initial_values(self, event=None):
         active_layer = self.viewer.layers.selection.active
 
         data = active_layer.data.copy()
         cutoff = np.quantile(data, self.percentile_range_edit.value / 100)
         data[data < cutoff] = 0
 
@@ -669,25 +662,51 @@
 
     def _on_method_changed(self, event=None):
         for widget in self.action_widgets:
             self.remove(widget)
         self.action_widgets.clear()
 
         function = self.methods.get(self.method_dropdown.value)
-        widgets = widgets_from_function(function)
-        for widget in widgets:
+        function_widgets = widgets_from_function(function)
+        for widget in function_widgets:
             self.action_widgets.append(widget)
             self.insert(1, widget)
 
+        for name, param in inspect.signature(function).parameters.items():
+            if name == "shapes_layer":
+                self.action_widgets.append(self.shapes_layer_dropdown)
+                self.insert(1, self.shapes_layer_dropdown)
+
+    def _get_shape_layers(self):
+        layers = [
+            layer.name
+            for layer in self.viewer.layers
+            if isinstance(layer, napari.layers.Shapes)
+        ]
+        return layers
+
+    def _update_shape_layer_choices(self, event):
+        """Update the choices in the shapes layer dropdown."""
+        self.shapes_layer_dropdown.choices = self._get_shape_layers()
+
     def _action(self):
         function = self.methods.get(self.method_dropdown.value)
 
         selected_layer = self.viewer.layers.selection.active
         kwargs = {widget.name: widget.value for widget in self.action_widgets}
+
+        if "shapes_layer" in kwargs:
+            layer_name = kwargs["shapes_layer"]
+            if layer_name not in self.viewer.layers:
+                return None
+            kwargs["shapes_layer"] = self.viewer.layers[layer_name]
+            kwargs["expansion_dim"] = self.viewer.dims.order[0]
+
         processed_data = function(template=selected_layer.data, **kwargs)
+
         new_layer_name = f"{selected_layer.name} ({self.method_dropdown.value})"
 
         if new_layer_name in self.viewer.layers:
             selected_layer = self.viewer.layers[new_layer_name]
 
         processed_data = processed_data.astype(np.float32)
         metadata = selected_layer.metadata
@@ -701,22 +720,122 @@
             )
             metadata = selected_layer.metadata.copy()
             metadata["filter_parameters"] = {self.method_dropdown.value: kwargs.copy()}
             metadata["mask"] = self.method_dropdown.value
             metadata["origin_layer"] = selected_layer.name
             new_layer.metadata = metadata
 
-        origin_layer = metadata["origin_layer"]
-        if origin_layer in self.viewer.layers:
-            origin_layer = self.viewer.layers[origin_layer]
-            if np.allclose(origin_layer.data.shape, processed_data.shape):
-                in_mask = np.sum(np.fmax(origin_layer.data * processed_data, 0))
-                in_mask /= np.sum(np.fmax(origin_layer.data, 0))
-                in_mask *= 100
-                self.density_field.value = f"Positive Density in Mask: {in_mask:.2f}%"
+            if self.method_dropdown.value == "Shape":
+                new_layer.metadata = {}
+
+        # origin_layer = metadata["origin_layer"]
+        # if origin_layer in self.viewer.layers:
+        #     origin_layer = self.viewer.layers[origin_layer]
+        #     if np.allclose(origin_layer.data.shape, processed_data.shape):
+        #         in_mask = np.sum(np.fmax(origin_layer.data * processed_data, 0))
+        #         in_mask /= np.sum(np.fmax(origin_layer.data, 0))
+        #         in_mask *= 100
+        #         self.density_field.value = f"Positive Density in Mask: {in_mask:.2f}%"
+
+
+class AlignmentWidget(widgets.Container):
+    def __init__(self, viewer):
+        super().__init__(layout="vertical")
+
+        self.viewer = viewer
+
+        align_button = widgets.PushButton(text="Align to axis", enabled=True)
+        self.align_axis = widgets.ComboBox(
+            value=None, nullable=True, choices=self._get_active_layer_dims
+        )
+        self.viewer.layers.selection.events.changed.connect(self._update_align_axis)
+
+        align_button.changed.connect(self._align_with_axis)
+        container = widgets.Container(
+            widgets=[align_button, self.align_axis], layout="horizontal"
+        )
+        self.append(container)
+
+        rot90 = widgets.PushButton(text="Rotate 90", enabled=True)
+        rotneg90 = widgets.PushButton(text="Rotate -90", enabled=True)
+
+        rot90.changed.connect(self._rot90)
+        rotneg90.changed.connect(self._rotneg90)
+
+        container = widgets.Container(widgets=[rot90, rotneg90], layout="horizontal")
+        self.append(container)
+
+    def _rot90(self, swap_axes: bool = False):
+        active_layer = self.viewer.layers.selection.active
+        if active_layer is None:
+            return None
+        elif self.viewer.dims.ndisplay != 2:
+            return None
+
+        align_axis = self.align_axis.value
+        if self.align_axis.value is None:
+            align_axis = self.viewer.dims.order[0]
+
+        axes = [
+            align_axis,
+            *[i for i in range(len(self.viewer.dims.order)) if i != align_axis],
+        ][:2]
+        axes = axes[::-1] if swap_axes else axes
+        active_layer.data = np.rot90(active_layer.data, k=1, axes=axes)
+
+    def _rotneg90(self):
+        return self._rot90(swap_axes=True)
+
+    def _get_active_layer_dims(self, *args):
+        active_layer = self.viewer.layers.selection.active
+        if active_layer is None:
+            return ()
+        return [i for i in range(active_layer.data.ndim)]
+
+    def _update_align_axis(self, *args):
+        self.align_axis.choices = self._get_active_layer_dims()
+
+    def _align_with_axis(self):
+        active_layer = self.viewer.layers.selection.active
+
+        if self.align_axis.value is None:
+            return None
+
+        if active_layer.metadata.get("is_aligned", None) == self.align_axis.value:
+            return None
+
+        alignment_axis = np.zeros(active_layer.data.ndim)
+        alignment_axis[int(self.align_axis.value)] = 1
+
+        coords = np.array(np.where(active_layer.data > 0)).T
+        centered_coords = coords - np.mean(coords, axis=0)
+        cov_matrix = np.cov(centered_coords, rowvar=False)
+
+        eigenvalues, eigenvectors = np.linalg.eigh(cov_matrix)
+        principal_eigenvector = eigenvectors[:, np.argmax(eigenvalues)]
+
+        rotation_axis = np.cross(principal_eigenvector, alignment_axis)
+        rotation_angle = np.arccos(np.dot(principal_eigenvector, alignment_axis))
+        k = rotation_axis / np.linalg.norm(rotation_axis)
+        K = np.array([[0, -k[2], k[1]], [k[2], 0, -k[0]], [-k[1], k[0], 0]])
+        rotation_matrix = np.eye(3)
+        rotation_matrix += np.sin(rotation_angle) * K
+        rotation_matrix += (1 - np.cos(rotation_angle)) * np.dot(K, K)
+
+        rotated_data = Density.rotate_array(
+            arr=active_layer.data,
+            rotation_matrix=rotation_matrix,
+            use_geometric_center=False,
+            order=1,
+        )
+        eps = np.finfo(rotated_data.dtype).eps
+        rotated_data[rotated_data < eps] = 0
+
+        active_layer.metadata["is_aligned"] = int(self.align_axis.value)
+        active_layer.data = rotated_data
 
 
 class ExportWidget(widgets.Container):
     def __init__(self, viewer):
         super().__init__(layout="vertical")
 
         self.viewer = viewer
@@ -799,24 +918,44 @@
             self.native,
             "Save Point Cloud File...",
             "",
             "TSV Files (*.tsv);;All Files (*)",
             options=options,
         )
 
-        if filename:
-            layer = self.viewer.layers.selection.active
-            if layer and isinstance(layer, napari.layers.Points):
-                original_dataframe = self.dataframes.get(layer.name, pd.DataFrame())
-
-                export_data = pd.DataFrame(layer.data, columns=["z", "y", "x"])
-                merged_data = pd.merge(
-                    export_data, original_dataframe, on=["z", "y", "x"], how="left"
-                )
-                merged_data.to_csv(filename, sep="\t", index=False)
+        if not filename:
+            return None
+
+        layer = self.viewer.layers.selection.active
+        if layer and isinstance(layer, napari.layers.Points):
+            original_dataframe = self.dataframes.get(
+                layer.name, pd.DataFrame(columns=["z", "y", "x"])
+            )
+
+            export_data = pd.DataFrame(layer.data, columns=["z", "y", "x"])
+            merged_data = pd.merge(
+                export_data, original_dataframe, on=["z", "y", "x"], how="left"
+            )
+
+            merged_data["z"] = merged_data["z"].astype(int)
+            merged_data["y"] = merged_data["y"].astype(int)
+            merged_data["x"] = merged_data["x"].astype(int)
+
+            euler_columns = ["euler_z", "euler_y", "euler_x"]
+            for col in euler_columns:
+                if col not in merged_data.columns:
+                    continue
+                merged_data[col] = merged_data[col].fillna(0)
+
+            if "score" in merged_data.columns:
+                merged_data["score"] = merged_data["score"].fillna(1)
+            if "detail" in merged_data.columns:
+                merged_data["detail"] = merged_data["detail"].fillna(2)
+
+            merged_data.to_csv(filename, sep="\t", index=False)
 
     def _get_load_path(self, event):
         options = QFileDialog.Options()
         filename, _ = QFileDialog.getOpenFileName(
             self.native,
             "Open Point Cloud File...",
             "",
@@ -826,14 +965,21 @@
         if filename:
             self._load_point_cloud(filename)
 
     def _load_point_cloud(self, filename):
         dataframe = pd.read_csv(filename, sep="\t")
         points = dataframe[["z", "y", "x"]].values
         layer_name = filename.split("/")[-1]
+
+        if "score" not in dataframe.columns:
+            dataframe["score"] = 1
+
+        if "detail" not in dataframe.columns:
+            dataframe["detail"] = -2
+
         point_properties = {
             "score": np.array(dataframe["score"].values),
             "detail": np.array(dataframe["detail"].values),
         }
         point_properties["score_scaled"] = np.log1p(
             point_properties["score"] - point_properties["score"].min()
         )
@@ -845,25 +991,63 @@
             face_color="score_scaled",
             face_colormap="turbo",
             name=layer_name,
         )
         self.dataframes[layer_name] = dataframe
 
 
+class MatchingWidget(widgets.Container):
+    def __init__(self, viewer):
+        super().__init__(layout="vertical")
+
+        self.viewer = viewer
+        self.dataframes = {}
+
+        self.import_button = widgets.PushButton(name="Import", text="Import Pickle")
+        self.import_button.clicked.connect(self._get_load_path)
+
+        self.append(self.import_button)
+
+    def _get_load_path(self, event):
+        options = QFileDialog.Options()
+        filename, _ = QFileDialog.getOpenFileName(
+            self.native,
+            "Open Pickle File...",
+            "",
+            "Pickle Files (*.pickle);;All Files (*)",
+            options=options,
+        )
+        if filename:
+            self._load_data(filename)
+
+    def _load_data(self, filename):
+        data = load_pickle(filename)
+
+        _ = self.viewer.add_image(data=data[2], name="Rotations", colormap="orange")
+
+        _ = self.viewer.add_image(data=data[0], name="Scores", colormap="turbo")
+
+
 def main():
     viewer = napari.Viewer()
 
     filter_widget = FilterWidget(preprocessor, viewer)
     mask_widget = MaskWidget(viewer)
     export_widget = ExportWidget(viewer)
     point_cloud = PointCloudWidget(viewer)
+    matching_widget = MatchingWidget(viewer)
+    alignment_widget = AlignmentWidget(viewer)
 
     viewer.window.add_dock_widget(widget=filter_widget, name="Preprocess", area="right")
+    viewer.window.add_dock_widget(
+        widget=alignment_widget, name="Alignment", area="right"
+    )
     viewer.window.add_dock_widget(widget=mask_widget, name="Mask", area="right")
     viewer.window.add_dock_widget(widget=point_cloud, name="PointCloud", area="left")
+    viewer.window.add_dock_widget(widget=matching_widget, name="Matching", area="left")
 
     viewer.window.add_dock_widget(widget=export_widget, name="Export", area="right")
 
     napari.run()
 
 
 def parse_args():
```

### Comparing `pytme-0.1.9/setup.py` & `pytme-0.2.0b0/setup.py`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/src/extensions.cpp` & `pytme-0.2.0b0/src/extensions.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -96,19 +96,19 @@
     candidate_indices.push_back(0);
 
     for (int i = 1; i < n; ++i) {
         bool is_candidate = true;
         ik = i * k;
         for (int candidate_index : candidate_indices) {
             jk = candidate_index * k;
-            T distance = std::abs(coordinates_data[ik] - coordinates_data[jk]);
+            T distance = std::pow(coordinates_data[ik] - coordinates_data[jk], 2);
             for (int p = 1; p < k; ++p) {
-                distance = std::max(distance,
-                    std::abs(coordinates_data[ik + p] - coordinates_data[jk + p]));
+                distance += std::pow(coordinates_data[ik + p] - coordinates_data[jk + p], 2);
             }
+            distance = std::sqrt(distance);
             if (distance <= min_distance) {
                 is_candidate = false;
                 break;
             }
         }
         if (is_candidate) {
             candidate_indices.push_back(i);
```

### Comparing `pytme-0.1.9/tme/analyzer.py` & `pytme-0.2.0b0/tme/analyzer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Implements classes to analyze score spaces from systematic fitting.
+""" Implements classes to analyze outputs from exhaustive template matching.
 
     Copyright (c) 2023 European Molecular Biology Laboratory
 
     Author: Valentin Maurer <valentin.maurer@embl-hamburg.de>
 """
 from time import sleep
 from typing import Tuple, List, Dict
@@ -11,40 +11,59 @@
 from multiprocessing import RawValue, Manager, Lock
 
 import numpy as np
 from numpy.typing import NDArray
 from scipy.stats import entropy
 from sklearn.cluster import DBSCAN
 from skimage.feature import peak_local_max
-
-from .extensions import max_index_by_label, online_statistics
+from skimage.registration._phase_cross_correlation import _upsampled_dft
+from .extensions import max_index_by_label, online_statistics, find_candidate_indices
 from .matching_utils import (
     split_numpy_array_slices,
     array_to_memmap,
     generate_tempfile_name,
+    euler_to_rotationmatrix,
+    apply_convolution_mode,
 )
-
 from .backends import backend
 
 
-def filter_points_indices(coordinates: NDArray, min_distance: Tuple[int]):
-    if min_distance <= 0:
-        return backend.arange(coordinates.shape[0])
+def filter_points_indices_bucket(
+    coordinates: NDArray, min_distance: Tuple[int]
+) -> NDArray:
+    coordinates = backend.subtract(coordinates, backend.min(coordinates, axis=0))
     bucket_indices = backend.astype(backend.divide(coordinates, min_distance), int)
     multiplier = backend.power(
         backend.max(bucket_indices, axis=0) + 1, backend.arange(bucket_indices.shape[1])
     )
     backend.multiply(bucket_indices, multiplier, out=bucket_indices)
     flattened_indices = backend.sum(bucket_indices, axis=1)
     _, unique_indices = backend.unique(flattened_indices, return_index=True)
     unique_indices = unique_indices[backend.argsort(unique_indices)]
     return unique_indices
 
 
-def filter_points(coordinates: NDArray, min_distance: Tuple[int]):
+def filter_points_indices(
+    coordinates: NDArray, min_distance: float, bucket_cutoff: int = 1e4
+) -> NDArray:
+    if min_distance <= 0:
+        return backend.arange(coordinates.shape[0])
+
+    if isinstance(coordinates, np.ndarray):
+        return find_candidate_indices(coordinates, min_distance)
+    elif coordinates.shape[0] > bucket_cutoff:
+        return filter_points_indices_bucket(coordinates, min_distance)
+    distances = np.linalg.norm(coordinates[:, None] - coordinates, axis=-1)
+    distances = np.tril(distances)
+    keep = np.sum(distances > min_distance, axis=1)
+    indices = np.arange(coordinates.shape[0])
+    return indices[keep == indices]
+
+
+def filter_points(coordinates: NDArray, min_distance: Tuple[int]) -> NDArray:
     unique_indices = filter_points_indices(coordinates, min_distance)
     coordinates = coordinates[unique_indices]
     return coordinates
 
 
 class PeakCaller(ABC):
     """
@@ -91,36 +110,45 @@
             )
 
         self.peak_list = []
         self.min_distance = min_distance
         self.min_boundary_distance = min_boundary_distance
         self.number_of_peaks = number_of_peaks
 
+        # Postprocesing arguments
+        self.fourier_shift = kwargs.get("fourier_shift", None)
+        self.convolution_mode = kwargs.get("convolution_mode", None)
+        self.targetshape = kwargs.get("targetshape", None)
+        self.templateshape = kwargs.get("templateshape", None)
+
     def __iter__(self):
         """
         Returns a generator to list objects containing translation,
         rotation, score and details of a given candidate.
         """
         self.peak_list = [backend.to_cpu_array(arr) for arr in self.peak_list]
         yield from self.peak_list
 
     def __call__(
-        self, score_space: NDArray, rotation_matrix: NDArray, **kwargs
+        self,
+        score_space: NDArray,
+        rotation_matrix: NDArray,
+        **kwargs,
     ) -> None:
         """
         Update the internal parameter store based on input array.
 
         Parameters
         ----------
         score_space : NDArray
             Array containing the score space.
         rotation_matrix : NDArray
             Rotation matrix used to obtain the score array.
         **kwargs
-            Additional keyword arguments.
+            Optional keyword arguments passed to :py:meth:`PeakCaller.call_peak`.
         """
         peak_positions, peak_details = self.call_peaks(
             score_space=score_space, rotation_matrix=rotation_matrix, **kwargs
         )
 
         if peak_positions is None:
             return None
@@ -155,19 +183,20 @@
             )
 
         rotations = backend.repeat(
             rotation_matrix.reshape(1, *rotation_matrix.shape),
             peak_positions.shape[0],
             axis=0,
         )
+        peak_scores = score_space[tuple(peak_positions.T)]
 
         self._update(
             peak_positions=peak_positions,
             peak_details=peak_details,
-            peak_scores=score_space[tuple(peak_positions.T)],
+            peak_scores=peak_scores,
             rotations=rotations,
             **kwargs,
         )
 
     @abstractmethod
     def call_peaks(
         self, score_space: NDArray, rotation_matrix: NDArray, **kwargs
@@ -186,18 +215,16 @@
         minimum_score : float
             Minimum score value to consider.
         min_distance : float
             Minimum distance between maxima.
 
         Returns
         -------
-        NDArray
-            Array of peak coordiantes.
-        NDArray
-            Array of peak details.
+        Tuple[NDArray, NDArray]
+            Array of peak coordinates and peak details.
         """
 
     @classmethod
     def merge(cls, candidates=List[List], **kwargs) -> NDArray:
         """
         Merge multiple instances of :py:class:`PeakCaller`.
 
@@ -227,14 +254,87 @@
                 peak_details=backend.to_backend_array(peak_details),
                 peak_scores=backend.to_backend_array(peak_scores),
                 rotations=backend.to_backend_array(rotations),
                 **kwargs,
             )
         return tuple(base)
 
+    @staticmethod
+    def oversample_peaks(
+        score_space: NDArray, peak_positions: NDArray, oversampling_factor: int = 8
+    ):
+        """
+        Refines peaks positions in the corresponding score space.
+
+        Parameters
+        ----------
+        score_space : NDArray
+            The d-dimensional array representing the score space.
+        peak_positions : NDArray
+            An array of shape (n, d) containing the peak coordinates
+            to be refined, where n is the number of peaks and d is the
+            dimensionality of the score space.
+        oversampling_factor : int, optional
+            The oversampling factor for Fourier transforms. Defaults to 8.
+
+        Returns
+        -------
+        NDArray
+            An array of shape (n, d) containing the refined subpixel
+            coordinates of the peaks.
+
+        Notes
+        -----
+        Floating point peak positions are determined by oversampling the
+        score_space around peak_positions. The accuracy
+        of refinement scales with 1 / oversampling_factor.
+
+        References
+        ----------
+        .. [1]  https://scikit-image.org/docs/stable/api/skimage.registration.html
+        .. [2]  Manuel Guizar-Sicairos, Samuel T. Thurman, and
+                James R. Fienup, “Efficient subpixel image registration
+                algorithms,” Optics Letters 33, 156-158 (2008).
+                DOI:10.1364/OL.33.000156
+
+        """
+        score_space = backend.to_numpy_array(score_space)
+        peak_positions = backend.to_numpy_array(peak_positions)
+
+        peak_positions = np.round(
+            np.divide(
+                np.multiply(peak_positions, oversampling_factor), oversampling_factor
+            )
+        )
+        upsampled_region_size = np.ceil(np.multiply(oversampling_factor, 1.5))
+        dftshift = np.round(np.divide(upsampled_region_size, 2.0))
+        sample_region_offset = np.subtract(
+            dftshift, np.multiply(peak_positions, oversampling_factor)
+        )
+
+        score_space_ft = np.fft.fftn(score_space).conj()
+        for index in range(sample_region_offset.shape[0]):
+            cross_correlation_upsampled = _upsampled_dft(
+                data=score_space_ft,
+                upsampled_region_size=upsampled_region_size,
+                upsample_factor=oversampling_factor,
+                axis_offsets=sample_region_offset[index],
+            ).conj()
+
+            maxima = np.unravel_index(
+                np.argmax(np.abs(cross_correlation_upsampled)),
+                cross_correlation_upsampled.shape,
+            )
+            maxima = np.divide(np.subtract(maxima, dftshift), oversampling_factor)
+            peak_positions[index] = np.add(peak_positions[index], maxima)
+
+        peak_positions = backend.to_backend_array(peak_positions)
+
+        return peak_positions
+
     def _update(
         self,
         peak_positions: NDArray,
         peak_details: NDArray,
         peak_scores: NDArray,
         rotations: NDArray,
         **kwargs,
@@ -283,94 +383,154 @@
         ]
 
         self.peak_list[0] = peaks[final_order,]
         self.peak_list[1] = rotations[final_order,]
         self.peak_list[2] = peak_scores[final_order]
         self.peak_list[3] = peak_details[final_order]
 
+    def _postprocess(
+        self, fourier_shift, convolution_mode, targetshape, templateshape, **kwargs
+    ):
+        peak_positions = self.peak_list[0]
+        if not len(peak_positions):
+            return self
+
+        if targetshape is None or templateshape is None:
+            return self
+
+        # Remove padding to next fast fourier length
+        score_space_shape = backend.add(targetshape, templateshape) - 1
+
+        if fourier_shift is not None:
+            peak_positions = backend.add(peak_positions, fourier_shift)
+            backend.divide(peak_positions, score_space_shape).astype(int)
+
+            backend.subtract(
+                peak_positions,
+                backend.multiply(
+                    backend.divide(peak_positions, score_space_shape).astype(int),
+                    score_space_shape
+                ),
+                out = peak_positions
+            )
+
+        if convolution_mode is None:
+            return None
+
+        if convolution_mode == "full":
+            output_shape = score_space_shape
+        elif convolution_mode == "same":
+            output_shape = targetshape
+        elif convolution_mode == "valid":
+            output_shape = backend.add(
+                backend.subtract(targetshape, templateshape),
+                backend.mod(templateshape, 2)
+            )
+
+        output_shape = backend.to_backend_array(output_shape)
+        starts = backend.divide(
+            backend.subtract(score_space_shape, output_shape),
+            2
+        )
+        starts = backend.astype(starts, int)
+        stops = backend.add(starts, output_shape)
+
+        valid_peaks = (
+            backend.sum(
+                backend.multiply(
+                    peak_positions > starts,
+                    peak_positions <= stops
+                ),
+                axis=1,
+            )
+            == peak_positions.shape[1]
+        )
+        self.peak_list[0] = backend.subtract(peak_positions, starts)
+        self.peak_list = [x[valid_peaks] for x in self.peak_list]
+        return self
 
 class PeakCallerSort(PeakCaller):
     """
     A :py:class:`PeakCaller` subclass that first selects ``number_of_peaks``
     highest scores and subsequently filters local maxima to suffice a distance
     from one another of ``min_distance``.
 
     """
 
     def call_peaks(
-        self, score_space: NDArray, rotation_matrix: NDArray, **kwargs
+        self, score_space: NDArray, minimum_score: float = None, **kwargs
     ) -> Tuple[NDArray, NDArray]:
         """
         Call peaks in the score space.
 
         Parameters
         ----------
         score_space : NDArray
             Data array of scores.
         minimum_score : float
-            Minimum score value to consider.
-        min_distance : float
-            Minimum distance between maxima.
+            Minimum score value to consider. If provided, superseeds limit given
+            by :py:attr:`PeakCaller.number_of_peaks`.
 
         Returns
         -------
-        NDArray
-            Array of peak coordiantes.
-        NDArray
-            Array of peak details.
+        Tuple[NDArray, NDArray]
+            Array of peak coordinates and peak details.
         """
         flat_score_space = score_space.reshape(-1)
         k = min(self.number_of_peaks, backend.size(flat_score_space))
 
+        if minimum_score is not None:
+            k = backend.sum(score_space >= minimum_score)
+
         top_k_indices, *_ = backend.topk_indices(flat_score_space, k)
 
         coordinates = backend.unravel_index(top_k_indices, score_space.shape)
         coordinates = backend.transpose(backend.stack(coordinates))
 
         peaks = filter_points(coordinates, self.min_distance)
         return peaks, None
 
 
 class PeakCallerMaximumFilter(PeakCaller):
     """
     Find local maxima by applying a maximum filter and enforcing a distance
-    constraint subseqquently. This is similar to the strategy implemented in
+    constraint subsequently. This is similar to the strategy implemented in
     skimage.feature.peak_local_max.
     """
 
     def call_peaks(
-        self, score_space: NDArray, rotation_matrix: NDArray, **kwargs
+        self, score_space: NDArray, minimum_score: float = None, **kwargs
     ) -> Tuple[NDArray, NDArray]:
         """
         Call peaks in the score space.
 
         Parameters
         ----------
         score_space : NDArray
             Data array of scores.
         minimum_score : float
-            Minimum score value to consider.
-        min_distance : float
-            Minimum distance between maxima.
+            Minimum score value to consider. If provided, superseeds limit given
+            by :py:attr:`PeakCaller.number_of_peaks`.
 
         Returns
         -------
-        NDArray
-            Array of peak coordiantes.
-        NDArray
-            Array of peak details.
+        Tuple[NDArray, NDArray]
+            Array of peak coordinates and peak details.
         """
         peaks = backend.max_filter_coordinates(score_space, self.min_distance)
 
+        scores = score_space[tuple(peaks.T)]
+
         input_candidates = min(
             self.number_of_peaks, peaks.shape[0] - 1, backend.size(score_space) - 1
         )
-        top_indices = backend.topk_indices(
-            score_space[tuple(peaks.T)], input_candidates
-        )
+        if minimum_score is not None:
+            input_candidates = backend.sum(scores >= minimum_score)
+
+        top_indices = backend.topk_indices(scores, input_candidates)
         peaks = peaks[top_indices]
 
         return peaks, None
 
 
 class PeakCallerFast(PeakCaller):
     """
@@ -378,34 +538,31 @@
     and determiens maximum value for each. In a second pass, all local maxima
     that are not the local maxima in a ``min_distance`` square centered around them
     are removed.
 
     """
 
     def call_peaks(
-        self, score_space: NDArray, rotation_matrix: NDArray, **kwargs
+        self, score_space: NDArray, minimum_score: float = None, **kwargs
     ) -> Tuple[NDArray, NDArray]:
         """
         Call peaks in the score space.
 
         Parameters
         ----------
         score_space : NDArray
             Data array of scores.
         minimum_score : float
-            Minimum score value to consider.
-        min_distance : float
-            Minimum distance between maxima.
+            Minimum score value to consider. If provided, superseeds limit given
+            by :py:attr:`PeakCaller.number_of_peaks`.
 
         Returns
         -------
-        NDArray
-            Array of peak coordiantes.
-        NDArray
-            Array of peak details.
+        Tuple[NDArray, NDArray]
+            Array of peak coordinates and peak details.
         """
         splits = {
             axis: score_space.shape[axis] // self.min_distance
             for axis in range(score_space.ndim)
         }
         slices = split_numpy_array_slices(score_space.shape, splits)
 
@@ -453,85 +610,255 @@
 class PeakCallerRecursiveMasking(PeakCaller):
     """
     Identifies peaks iteratively by selecting the top score and masking
     a region around it.
     """
 
     def call_peaks(
-        self, score_space: NDArray, rotation_matrix: NDArray, **kwargs
+        self,
+        score_space: NDArray,
+        rotation_matrix: NDArray,
+        mask: NDArray = None,
+        minimum_score: float = None,
+        rotation_space: NDArray = None,
+        rotation_mapping: Dict = None,
+        **kwargs,
     ) -> Tuple[NDArray, NDArray]:
         """
         Call peaks in the score space.
 
         Parameters
         ----------
         score_space : NDArray
             Data array of scores.
+        rotation_matrix : NDArray
+            Rotation matrix.
+        mask : NDArray, optional
+            Mask array, by default None.
+        rotation_space : NDArray, optional
+            Rotation space array, by default None.
+        rotation_mapping : Dict optional
+            Dictionary mapping values in rotation_space to Euler angles.
+            By default None
         minimum_score : float
-            Minimum score value to consider.
-        min_distance : float
-            Minimum distance between maxima.
+            Minimum score value to consider. If provided, superseeds limit given
+            by :py:attr:`PeakCaller.number_of_peaks`.
 
         Returns
         -------
-        NDArray
-            Array of peak coordiantes.
-        NDArray
-            Array of peak details.
-        """
-        score_box = tuple(self.min_distance for _ in range(score_space.ndim))
-        coordinates = []
+        Tuple[NDArray, NDArray]
+            Array of peak coordinates and peak details.
+
+        Notes
+        -----
+        By default, scores are masked using a box with edge length self.min_distance.
+        If mask is provided, elements around each peak will be multiplied by the mask
+        values. If rotation_space and rotation_mapping is provided, the respective
+        rotation will be applied to the mask, otherwise rotation_matrix is used.
+        """
+        coordinates, masking_function = [], self._mask_scores_rotate
+
+        if mask is None:
+            masking_function = self._mask_scores_box
+            shape = tuple(self.min_distance for _ in range(score_space.ndim))
+            mask = backend.zeros(shape, dtype=backend._default_dtype)
+
+        rotated_template = backend.zeros(mask.shape, dtype=mask.dtype)
+
+        peak_limit = self.number_of_peaks
+        if minimum_score is not None:
+            peak_limit = backend.size(score_space)
+        else:
+            minimum_score = backend.min(score_space) - 1
+
         while True:
             backend.argmax(score_space)
-            max_coord = backend.unravel_index(
+            peak = backend.unravel_index(
                 indices=backend.argmax(score_space), shape=score_space.shape
             )
-            coordinates.append(max_coord)
-            start = backend.maximum(backend.subtract(max_coord, score_box), 0)
-            stop = backend.minimum(backend.add(max_coord, score_box), score_space.shape)
-            start, stop = backend.astype(start, int), backend.astype(stop, int)
-            coords = tuple(slice(*pos) for pos in zip(start, stop))
-            score_space[coords] = 0
-            if len(coordinates) >= self.number_of_peaks:
+            if score_space[tuple(peak)] < minimum_score:
+                break
+
+            coordinates.append(peak)
+
+            current_rotation_matrix = self._get_rotation_matrix(
+                peak=peak,
+                rotation_space=rotation_space,
+                rotation_mapping=rotation_mapping,
+                rotation_matrix=rotation_matrix,
+            )
+
+            masking_function(
+                score_space=score_space,
+                rotation_matrix=current_rotation_matrix,
+                peak=peak,
+                mask=mask,
+                rotated_template=rotated_template,
+            )
+
+            if len(coordinates) >= peak_limit:
                 break
+
         peaks = backend.to_backend_array(coordinates)
         return peaks, None
 
+    @staticmethod
+    def _get_rotation_matrix(
+        peak: NDArray,
+        rotation_space: NDArray,
+        rotation_mapping: NDArray,
+        rotation_matrix: NDArray,
+    ) -> NDArray:
+        """
+        Get rotation matrix based on peak and rotation data.
+
+        Parameters
+        ----------
+        peak : NDArray
+            Peak coordinates.
+        rotation_space : NDArray
+            Rotation space array.
+        rotation_mapping : Dict
+            Dictionary mapping values in rotation_space to Euler angles.
+        rotation_matrix : NDArray
+            Current rotation matrix.
+
+        Returns
+        -------
+        NDArray
+            Rotation matrix.
+        """
+        if rotation_space is None or rotation_mapping is None:
+            return rotation_matrix
+
+        rotation = rotation_mapping[rotation_space[tuple(peak)]]
+
+        rotation_matrix = backend.to_backend_array(
+            euler_to_rotationmatrix(backend.to_numpy_array(rotation))
+        )
+        return rotation_matrix
+
+    @staticmethod
+    def _mask_scores_box(
+        score_space: NDArray, peak: NDArray, mask: NDArray, **kwargs: Dict
+    ) -> None:
+        """
+        Mask scores in a box around a peak.
+
+        Parameters
+        ----------
+        score_space : NDArray
+            Data array of scores.
+        peak : NDArray
+            Peak coordinates.
+        mask : NDArray
+            Mask array.
+        """
+        start = backend.maximum(backend.subtract(peak, mask.shape), 0)
+        stop = backend.minimum(backend.add(peak, mask.shape), score_space.shape)
+        start, stop = backend.astype(start, int), backend.astype(stop, int)
+        coords = tuple(slice(*pos) for pos in zip(start, stop))
+        score_space[coords] = 0
+        return None
+
+    @staticmethod
+    def _mask_scores_rotate(
+        score_space: NDArray,
+        peak: NDArray,
+        mask: NDArray,
+        rotated_template: NDArray,
+        rotation_matrix: NDArray,
+        **kwargs: Dict,
+    ) -> None:
+        """
+        Mask score_space using mask rotation around a peak.
+
+        Parameters
+        ----------
+        score_space : NDArray
+            Data array of scores.
+        peak : NDArray
+            Peak coordinates.
+        mask : NDArray
+            Mask array.
+        rotated_template : NDArray
+            Empty array to write mask rotations to.
+        rotation_matrix : NDArray
+            Rotation matrix.
+        """
+        left_pad = backend.divide(mask.shape, 2).astype(int)
+        right_pad = backend.add(left_pad, backend.mod(mask.shape, 2).astype(int))
+
+        score_start = backend.subtract(peak, left_pad)
+        score_stop = backend.add(peak, right_pad)
+
+        template_start = backend.subtract(backend.maximum(score_start, 0), score_start)
+        template_stop = backend.subtract(
+            score_stop, backend.minimum(score_stop, score_space.shape)
+        )
+        template_stop = backend.subtract(mask.shape, template_stop)
+
+        score_start = backend.maximum(score_start, 0)
+        score_stop = backend.minimum(score_stop, score_space.shape)
+        score_start = backend.astype(score_start, int)
+        score_stop = backend.astype(score_stop, int)
+
+        template_start = backend.astype(template_start, int)
+        template_stop = backend.astype(template_stop, int)
+        coords_score = tuple(slice(*pos) for pos in zip(score_start, score_stop))
+        coords_template = tuple(
+            slice(*pos) for pos in zip(template_start, template_stop)
+        )
+
+        rotated_template.fill(0)
+        backend.rotate_array(
+            arr=mask, rotation_matrix=rotation_matrix, order=1, out=rotated_template
+        )
+
+        score_space[coords_score] = backend.multiply(
+            score_space[coords_score], (rotated_template[coords_template] <= 0.1)
+        )
+        return None
+
 
 class PeakCallerScipy(PeakCaller):
     """
     Peak calling using skimage.feature.peak_local_max to compute local maxima.
     """
 
     def call_peaks(
-        self, score_space: NDArray, rotation_matrix: NDArray, **kwargs
+        self, score_space: NDArray, minimum_score: float = None, **kwargs
     ) -> Tuple[NDArray, NDArray]:
         """
         Call peaks in the score space.
 
         Parameters
         ----------
         score_space : NDArray
             Data array of scores.
         minimum_score : float
-            Minimum score value to consider.
-        min_distance : float
-            Minimum distance between maxima.
+            Minimum score value to consider. If provided, superseeds limit given
+            by :py:attr:`PeakCaller.number_of_peaks`.
 
         Returns
         -------
-        NDArray
-            Array of peak coordiantes.
-        NDArray
-            Array of peak details.
+        Tuple[NDArray, NDArray]
+            Array of peak coordinates and peak details.
         """
+
+        score_space = backend.to_numpy_array(score_space)
+        num_peaks = self.number_of_peaks
+        if minimum_score is not None:
+            num_peaks = np.inf
+
         peaks = peak_local_max(
             score_space,
-            num_peaks=self.number_of_peaks,
+            num_peaks=num_peaks,
             min_distance=self.min_distance,
+            threshold_abs=minimum_score,
         )
         return peaks, None
 
 
 class PeakClustering(PeakCallerSort):
     """
     Use DBScan clustering to identify more reliable peaks.
@@ -875,16 +1202,76 @@
         self.translation_offset = backend.astype(translation_offset, int)
         self.score_space_shape = score_space_shape
         self.rotation_space_dtype = rotation_space_dtype
         self.score_space_dtype = score_space_dtype
 
         self.use_memmap = use_memmap
         self.lock = Manager().Lock() if thread_safe else nullcontext()
+        self.lock_is_nullcontext = isinstance(self.score_space, type(backend.zeros((1))))
         self.observed_rotations = Manager().dict() if thread_safe else {}
 
+
+    def _postprocess(self,
+        fourier_shift,
+        convolution_mode,
+        targetshape,
+        templateshape,
+        shared_memory_handler=None,
+        **kwargs
+        ):
+        internal_scores = backend.sharedarr_to_arr(
+            shape=self.score_space_shape,
+            dtype=self.score_space_dtype,
+            shm=self.score_space,
+        )
+        internal_rotations = backend.sharedarr_to_arr(
+            shape=self.score_space_shape,
+            dtype=self.rotation_space_dtype,
+            shm=self.rotations,
+        )
+
+        if fourier_shift is not None:
+            axis = tuple(i for i in range(len(fourier_shift)))
+            internal_scores = backend.roll(
+                internal_scores,
+                shift=fourier_shift,
+                axis=axis
+            )
+            internal_rotations = backend.roll(
+                internal_rotations,
+                shift=fourier_shift,
+                axis=axis
+            )
+
+        if convolution_mode is not None:
+            internal_scores = apply_convolution_mode(
+                internal_scores,
+                convolution_mode=convolution_mode,
+                s1=targetshape,
+                s2=templateshape
+            )
+            internal_rotations = apply_convolution_mode(
+                internal_rotations,
+                convolution_mode=convolution_mode,
+                s1=targetshape,
+                s2=templateshape
+            )
+
+        self.score_space_shape = internal_scores.shape
+        self.score_space = backend.arr_to_sharedarr(
+            internal_scores,
+            shared_memory_handler
+        )
+        self.rotations = backend.arr_to_sharedarr(
+            internal_rotations,
+            shared_memory_handler
+        )
+        return self
+
+
     def __iter__(self):
         internal_scores = backend.sharedarr_to_arr(
             shape=self.score_space_shape,
             dtype=self.score_space_dtype,
             shm=self.score_space,
         )
         internal_rotations = backend.sharedarr_to_arr(
@@ -934,32 +1321,47 @@
         score_space : ndarray
             Numpy array containing the score space.
         rotation_matrix : ndarray
             Square matrix describing the current rotation.
         **kwargs
             Arbitrary keyword arguments.
         """
+        rotation = backend.tobytes(rotation_matrix)
+        rotation_index = self.observed_rotations.setdefault(
+            rotation, len(self.observed_rotations)
+        )
+
+        if self.lock_is_nullcontext:
+            backend.max_score_over_rotations(
+                score_space=score_space,
+                internal_scores=self.score_space,
+                internal_rotations=self.rotations,
+                rotation_index=rotation_index,
+            )
+            return None
+
         with self.lock:
-            rotation = backend.tobytes(rotation_matrix)
-            if rotation not in self.observed_rotations:
-                self.observed_rotations[rotation] = len(self.observed_rotations)
-            rotation_index = self.observed_rotations[rotation]
             internal_scores = backend.sharedarr_to_arr(
                 shape=self.score_space_shape,
                 dtype=self.score_space_dtype,
                 shm=self.score_space,
             )
             internal_rotations = backend.sharedarr_to_arr(
                 shape=self.score_space_shape,
                 dtype=self.rotation_space_dtype,
                 shm=self.rotations,
             )
-            indices = score_space > internal_scores
-            internal_scores[indices] = score_space[indices]
-            internal_rotations[indices] = rotation_index
+
+            backend.max_score_over_rotations(
+                score_space=score_space,
+                internal_scores=internal_scores,
+                internal_rotations=internal_rotations,
+                rotation_index=rotation_index,
+            )
+            return None
 
     @classmethod
     def merge(cls, param_stores=List[Tuple], **kwargs) -> Tuple[NDArray]:
         """
         Merges multiple instances of :py:class:`MaxScoreOverRotations`.
 
         Parameters
@@ -1003,22 +1405,30 @@
         if use_memmap:
             scores_out_filename = generate_tempfile_name()
             rotations_out_filename = generate_tempfile_name()
 
             scores_out = np.memmap(
                 scores_out_filename, mode="w+", shape=base_max, dtype=scores_out_dtype
             )
+            scores_out.fill(kwargs.get("score_threshold", 0))
+            scores_out.flush()
             rotations_out = np.memmap(
                 rotations_out_filename,
                 mode="w+",
                 shape=base_max,
                 dtype=rotations_out_dtype,
             )
+            rotations_out.fill(-1)
+            rotations_out.flush()
         else:
-            scores_out = np.zeros(base_max, dtype=scores_out_dtype)
+            scores_out = np.full(
+                base_max,
+                fill_value=kwargs.get("score_threshold", 0),
+                dtype=scores_out_dtype,
+            )
             rotations_out = np.full(base_max, fill_value=-1, dtype=rotations_out_dtype)
 
         for i in range(len(param_stores)):
             if param_stores[i] is None:
                 continue
 
             if use_memmap:
@@ -1075,14 +1485,69 @@
             scores_out,
             np.zeros(scores_out.ndim, dtype=int),
             rotations_out,
             new_rotation_mapping,
         )
 
 
+class _MaxScoreOverTranslations(MaxScoreOverRotations):
+    """
+    Obtain the maximum translation score over various rotations.
+
+    Attributes
+    ----------
+    score_space : NDArray
+        The score space for the observed rotations.
+    rotations : NDArray
+        The rotation identifiers for each score.
+    translation_offset : NDArray, optional
+        The offset applied during translation.
+    observed_rotations : int
+        Count of observed rotations.
+    use_memmap : bool, optional
+        Whether to offload internal data arrays to disk
+    thread_safe: bool, optional
+        Whether access to internal data arrays should be thread safe
+    """
+
+    def __call__(
+        self, score_space: NDArray, rotation_matrix: NDArray, **kwargs
+    ) -> None:
+        """
+        Update internal parameter store based on `score_space`.
+
+        Parameters
+        ----------
+        score_space : ndarray
+            Numpy array containing the score space.
+        rotation_matrix : ndarray
+            Square matrix describing the current rotation.
+        **kwargs
+            Arbitrary keyword arguments.
+        """
+        from tme.matching_utils import centered_mask
+
+        with self.lock:
+            rotation = backend.tobytes(rotation_matrix)
+            if rotation not in self.observed_rotations:
+                self.observed_rotations[rotation] = len(self.observed_rotations)
+            score_space = centered_mask(score_space, kwargs["template_shape"])
+            rotation_index = self.observed_rotations[rotation]
+            internal_scores = backend.sharedarr_to_arr(
+                shape=self.score_space_shape,
+                dtype=self.score_space_dtype,
+                shm=self.score_space,
+            )
+            max_score = score_space.max(axis=(1, 2, 3))
+            mean_score = score_space.mean(axis=(1, 2, 3))
+            std_score = score_space.std(axis=(1, 2, 3))
+            z_score = (max_score - mean_score) / std_score
+            internal_scores[rotation_index] = z_score
+
+
 class MemmapHandler:
     """
     Create numpy memmap objects to write score spaces to.
 
     This is useful in cases where not the entire score space is sampled at once.
 
     Parameters
@@ -1178,7 +1643,9 @@
         Returns
         -------
         str
             String representation of the rotation matrix.
         """
         rotation_string = "_".join(rotation_matrix.ravel().astype(str))
         return self._path_translation[rotation_string]
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytme-0.1.9/tme/backends/__init__.py` & `pytme-0.2.0b0/tme/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/backends/cupy_backend.py` & `pytme-0.2.0b0/tme/backends/cupy_backend.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 import numpy as np
 from numpy.typing import NDArray
 
 from .npfftw_backend import NumpyFFTWBackend
 from ..types import CupyArray
 
+PLAN_CACHE = {}
+
 
 class CupyBackend(NumpyFFTWBackend):
     """
     A cupy based backend for template matching
     """
 
     def __init__(
@@ -40,14 +42,23 @@
             complex_dtype=complex_dtype,
             default_dtype_int=default_dtype_int,
         )
         self.get_fft_plan = get_fft_plan
         self.affine_transform = affine_transform
         self.maximum_filter = maximum_filter
 
+        floating = f"float{self.datatype_bytes(default_dtype) * 8}"
+        integer = f"int{self.datatype_bytes(default_dtype_int) * 8}"
+        self._max_score_over_rotations = self._array_backend.ElementwiseKernel(
+            f"{floating} internal_scores, {floating} scores, {integer} rot_index",
+            f"{floating} out1, {integer} rotations",
+            "if (internal_scores < scores) {out1 = scores; rotations = rot_index;}",
+            "max_score_over_rotations",
+        )
+
     def to_backend_array(self, arr: NDArray) -> CupyArray:
         current_device = self._array_backend.cuda.device.get_device_id()
         if (
             isinstance(arr, self._array_backend.ndarray)
             and arr.device.id == current_device
         ):
             return arr
@@ -56,15 +67,15 @@
     def to_numpy_array(self, arr: CupyArray) -> NDArray:
         return self._array_backend.asnumpy(arr)
 
     def to_cpu_array(self, arr: NDArray) -> NDArray:
         return self.to_numpy_array(arr)
 
     def sharedarr_to_arr(
-        self, shape: Tuple[int], dtype: str, shm: CupyArray
+        self, shm: CupyArray, shape: Tuple[int], dtype: str
     ) -> CupyArray:
         return shm
 
     @staticmethod
     def arr_to_sharedarr(
         arr: CupyArray, shared_memory_handler: type = None
     ) -> CupyArray:
@@ -105,59 +116,72 @@
     def build_fft(
         self,
         fast_shape: Tuple[int],
         fast_ft_shape: Tuple[int],
         real_dtype: type,
         complex_dtype: type,
         fftargs: Dict = {},
-        temp_real: NDArray = None,
-        temp_fft: NDArray = None,
+        inverse_fast_shape: Tuple[int] = None,
+        **kwargs,
     ) -> Tuple[Callable, Callable]:
         """
         Build pyFFTW builder functions.
 
         Parameters
         ----------
         fast_shape : tuple
             Tuple of integers corresponding to fast convolution shape
-            (see `compute_convolution_shapes`).
+            (see :py:meth:`CupyBackend.compute_convolution_shapes`).
         fast_ft_shape : tuple
             Tuple of integers corresponding to the shape of the fourier
-            transform array (see `compute_convolution_shapes`).
+            transform array (see :py:meth:`CupyBackend.compute_convolution_shapes`).
         real_dtype : dtype
             Numpy dtype of the inverse fourier transform.
         complex_dtype : dtype
             Numpy dtype of the fourier transform.
+        inverse_fast_shape : tuple, optional
+            Output shape of the inverse Fourier transform. By default fast_shape.
         fftargs : dict, optional
             Dictionary passed to pyFFTW builders.
-        temp_real : NDArray, optional
-            Temporary real numpy array, by default None.
-        temp_fft : NDArray, optional
-            Temporary fft numpy array, by default None.
+        **kwargs: dict, optional
+            Unused keyword arguments.
 
         Returns
         -------
         tuple
             Tupple containing callable rfft and irfft object.
         """
-
-        if temp_real is None:
-            temp_real = self.preallocate_array(fast_shape, real_dtype)
-        if temp_fft is None:
-            temp_fft = self.preallocate_array(fast_ft_shape, complex_dtype)
-
         cache = self._array_backend.fft.config.get_plan_cache()
         cache.set_size(2)
 
+        current_device = self._array_backend.cuda.device.get_device_id()
+
+        previous_transform = [fast_shape, fast_ft_shape]
+        if current_device in PLAN_CACHE:
+            previous_transform = PLAN_CACHE[current_device]
+
+        real_diff, cmplx_diff = True, True
+        if len(fast_shape) == len(previous_transform[0]):
+            real_diff = self.sum(self.subtract(fast_shape, previous_transform[0])) != 0
+        if len(fast_ft_shape) == len(previous_transform[1]):
+            cmplx_diff = (
+                self.sum(self.subtract(fast_ft_shape, previous_transform[1])) != 0
+            )
+
+        if real_diff or cmplx_diff:
+            cache.clear()
+
         def rfftn(arr: CupyArray, out: CupyArray) -> None:
             out[:] = self.fft.rfftn(arr)[:]
 
         def irfftn(arr: CupyArray, out: CupyArray) -> None:
             out[:] = self.fft.irfftn(arr)[:]
 
+        PLAN_CACHE[current_device] = [fast_shape, fast_ft_shape]
+
         return rfftn, irfftn
 
     def compute_convolution_shapes(
         self, arr1_shape: Tuple[int], arr2_shape: Tuple[int]
     ) -> Tuple[Tuple[int], Tuple[int], Tuple[int]]:
         ret = super().compute_convolution_shapes(arr1_shape, arr2_shape)
         convolution_shape, fast_shape, fast_ft_shape = ret
@@ -173,14 +197,25 @@
         score_box = tuple(min_distance for _ in range(score_space.ndim))
         max_filter = self.maximum_filter(score_space, size=score_box, mode="constant")
         max_filter = max_filter == score_space
 
         peaks = self._array_backend.array(self._array_backend.nonzero(max_filter)).T
         return peaks
 
+    # The default methods in Cupy were oddly slow
+    def var(self, a, *args, **kwargs):
+        out = a - self._array_backend.mean(a, *args, **kwargs)
+        self._array_backend.square(out, out)
+        out = self._array_backend.mean(out, *args, **kwargs)
+        return out
+
+    def std(self, a, *args, **kwargs):
+        out = self.var(a, *args, **kwargs)
+        return self._array_backend.sqrt(out)
+
     def rotate_array(
         self,
         arr: CupyArray,
         rotation_matrix: CupyArray,
         arr_mask: CupyArray = None,
         translation: CupyArray = None,
         use_geometric_center: bool = False,
@@ -307,7 +342,37 @@
 
         Returns
         -------
         int
             Number of available GPU devices.
         """
         return self._array_backend.cuda.runtime.getDeviceCount()
+
+    def max_score_over_rotations(
+        self,
+        score_space: CupyArray,
+        internal_scores: CupyArray,
+        internal_rotations: CupyArray,
+        rotation_index: int,
+    ):
+        """
+        Modify internal_scores and internal_rotations inplace with scores and rotation
+        index respectively, wherever score_sapce is larger than internal scores.
+
+        Parameters
+        ----------
+        score_space : CupyArray
+            The score space to compare against internal_scores.
+        internal_scores : CupyArray
+            The internal scores to update with maximum scores.
+        internal_rotations : CupyArray
+            The internal rotations corresponding to the maximum scores.
+        rotation_index : int
+            The index representing the current rotation.
+        """
+        self._max_score_over_rotations(
+            internal_scores,
+            score_space,
+            rotation_index,
+            internal_scores,
+            internal_rotations,
+        )
```

### Comparing `pytme-0.1.9/tme/backends/matching_backend.py` & `pytme-0.2.0b0/tme/backends/matching_backend.py`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/backends/mlx_backend.py` & `pytme-0.2.0b0/tme/backends/mlx_backend.py`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/backends/npfftw_backend.py` & `pytme-0.2.0b0/tme/backends/npfftw_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -252,15 +252,15 @@
         NDArray
             Byte-aligned array of zeros with specified shape and dtype.
         """
         arr = zeros_aligned(shape, dtype=dtype, n=simd_alignment)
         return arr
 
     def sharedarr_to_arr(
-        self, shape: Tuple[int], dtype: str, shm: shared_memory.SharedMemory
+        self, shm: shared_memory.SharedMemory, shape: Tuple[int], dtype: str
     ) -> NDArray:
         """
         Returns an array of given shape and dtype from shared memory location.
 
         Parameters
         ----------
         shape : tuple
@@ -337,14 +337,15 @@
     def build_fft(
         self,
         fast_shape: Tuple[int],
         fast_ft_shape: Tuple[int],
         real_dtype: type,
         complex_dtype: type,
         fftargs: Dict = {},
+        inverse_fast_shape: Tuple[int] = None,
         temp_real: NDArray = None,
         temp_fft: NDArray = None,
     ) -> Tuple[FFTW, FFTW]:
         """
         Build pyFFTW builder functions.
 
         Parameters
@@ -355,14 +356,16 @@
         fast_ft_shape : tuple
             Tuple of integers corresponding to the shape of the fourier
             transform array (see `compute_convolution_shapes`).
         real_dtype : dtype
             Numpy dtype of the inverse fourier transform.
         complex_dtype : dtype
             Numpy dtype of the fourier transform.
+        inverse_fast_shape : tuple, optional
+            Output shape of the inverse Fourier transform. By default fast_shape.
         fftargs : dict, optional
             Dictionary passed to pyFFTW builders.
         temp_real : NDArray, optional
             Temporary real numpy array, by default None.
         temp_fft : NDArray, optional
             Temporary fft numpy array, by default None.
 
@@ -372,14 +375,16 @@
             Tuple containing callable pyFFTW objects for forward and inverse
             fourier transform.
         """
         if temp_real is None:
             temp_real = self.preallocate_array(fast_shape, real_dtype)
         if temp_fft is None:
             temp_fft = self.preallocate_array(fast_ft_shape, complex_dtype)
+        if inverse_fast_shape is None:
+            inverse_fast_shape = fast_shape
 
         default_values = {
             "planner_effort": "FFTW_MEASURE",
             "auto_align_input": False,
             "auto_contiguous": False,
             "avoid_copy": True,
             "overwrite_input": True,
@@ -391,15 +396,15 @@
             fftargs[key] = default_values[key]
 
         rfftn = rfftn_builder(temp_real, s=fast_shape, **fftargs)
 
         overwrite_input = None
         if "overwrite_input" in fftargs:
             overwrite_input = fftargs.pop("overwrite_input")
-        irfftn = irfftn_builder(temp_fft, s=fast_shape, **fftargs)
+        irfftn = irfftn_builder(temp_fft, s=inverse_fast_shape, **fftargs)
 
         if overwrite_input is not None:
             fftargs["overwrite_input"] = overwrite_input
         return rfftn, irfftn
 
     def extract_center(self, arr: NDArray, newshape: Tuple[int]) -> NDArray:
         """
@@ -752,7 +757,33 @@
 
         Returns
         -------
         NDArray
             Reversed array.
         """
         return arr[(slice(None, None, -1),) * arr.ndim]
+
+    def max_score_over_rotations(
+        self,
+        score_space: NDArray,
+        internal_scores: NDArray,
+        internal_rotations: NDArray,
+        rotation_index: int,
+    ) -> None:
+        """
+        Modify internal_scores and internal_rotations inplace with scores and rotation
+        index respectively, wherever score_sapce is larger than internal scores.
+
+        Parameters
+        ----------
+        score_space : numpy.ndarray
+            The score space to compare against internal_scores.
+        internal_scores : numpy.ndarray
+            The internal scores to update with maximum scores.
+        internal_rotations : numpy.ndarray
+            The internal rotations corresponding to the maximum scores.
+        rotation_index : int
+            The index representing the current rotation.
+        """
+        indices = score_space > internal_scores
+        internal_scores[indices] = score_space[indices]
+        internal_rotations[indices] = rotation_index
```

### Comparing `pytme-0.1.9/tme/backends/pytorch_backend.py` & `pytme-0.2.0b0/tme/backends/pytorch_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,15 +233,15 @@
         coordinates = self.transpose(self.stack(coordinates))
         return coordinates
 
     def repeat(self, *args, **kwargs):
         return self._array_backend.repeat_interleave(*args, **kwargs)
 
     def sharedarr_to_arr(
-        self, shape: Tuple[int], dtype: str, shm: TorchTensor
+        self, shm: TorchTensor, shape: Tuple[int], dtype: str
     ) -> TorchTensor:
         if self.device == "cuda":
             return shm
 
         required_size = int(self._array_backend.prod(self.to_backend_array(shape)))
 
         ret = self._array_backend.frombuffer(shm.buf, dtype=dtype)[
@@ -381,43 +381,51 @@
                 return out
             case 2:
                 return out_mask
             case 3:
                 return out, out_mask
 
     def build_fft(
-        self, fast_shape: Tuple[int], fast_ft_shape: Tuple[int], **kwargs
+        self,
+        fast_shape: Tuple[int],
+        fast_ft_shape: Tuple[int],
+        inverse_fast_shape: Tuple[int] = None,
+        **kwargs,
     ) -> Tuple[Callable, Callable]:
         """
         Build fft builder functions.
 
         Parameters
         ----------
         fast_shape : tuple
             Tuple of integers corresponding to fast convolution shape
-            (see `compute_convolution_shapes`).
+            (see :py:meth:`PytorchBackend.compute_convolution_shapes`).
         fast_ft_shape : tuple
-            Tuple of integers corresponding to the shape of the fourier
-            transform array (see `compute_convolution_shapes`).
+            Tuple of integers corresponding to the shape of the Fourier
+            transform array (see :py:meth:`PytorchBackend.compute_convolution_shapes`).
+        inverse_fast_shape : tuple, optional
+            Output shape of the inverse Fourier transform. By default fast_shape.
         **kwargs : dict, optional
-            Additional parameters that are not used for now.
+            Unused keyword arguments.
 
         Returns
         -------
         tuple
             Tupple containing callable rfft and irfft object.
         """
+        if inverse_fast_shape is None:
+            inverse_fast_shape = fast_shape
 
         def rfftn(
             arr: TorchTensor, out: TorchTensor, shape: Tuple[int] = fast_shape
         ) -> None:
             return self._array_backend.fft.rfftn(arr, s=shape, out=out)
 
         def irfftn(
-            arr: TorchTensor, out: TorchTensor, shape: Tuple[int] = fast_shape
+            arr: TorchTensor, out: TorchTensor, shape: Tuple[int] = inverse_fast_shape
         ) -> None:
             return self._array_backend.fft.irfftn(arr, s=shape, out=out)
 
         return rfftn, irfftn
 
     def _affine_transform(
         self,
```

### Comparing `pytme-0.1.9/tme/data/c48n309.npy` & `pytme-0.2.0b0/tme/data/c48n309.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/data/c48n527.npy` & `pytme-0.2.0b0/tme/data/c48n527.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/data/c48n9.npy` & `pytme-0.2.0b0/tme/data/c48n9.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/data/c48u1.npy` & `pytme-0.2.0b0/tme/data/c48u1.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/data/c48u1153.npy` & `pytme-0.2.0b0/tme/data/c48u1153.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/data/c48u1201.npy` & `pytme-0.2.0b0/tme/data/c48u1201.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/data/c48u1641.npy` & `pytme-0.2.0b0/tme/data/c48u1641.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/data/c48u181.npy` & `pytme-0.2.0b0/tme/data/c48u181.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/data/c48u2219.npy` & `pytme-0.2.0b0/tme/data/c48u2219.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/data/c48u27.npy` & `pytme-0.2.0b0/tme/data/c48u27.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/data/c48u2947.npy` & `pytme-0.2.0b0/tme/data/c48u2947.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/data/c48u3733.npy` & `pytme-0.2.0b0/tme/data/c48u3733.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/data/c48u4749.npy` & `pytme-0.2.0b0/tme/data/c48u4749.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/data/c48u5879.npy` & `pytme-0.2.0b0/tme/data/c48u5879.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/data/c48u7111.npy` & `pytme-0.2.0b0/tme/data/c48u7111.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/data/c48u815.npy` & `pytme-0.2.0b0/tme/data/c48u815.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/data/c48u83.npy` & `pytme-0.2.0b0/tme/data/c48u83.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/data/c48u8649.npy` & `pytme-0.2.0b0/tme/data/c48u8649.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/data/c600v.npy` & `pytme-0.2.0b0/tme/data/c600v.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/data/c600vc.npy` & `pytme-0.2.0b0/tme/data/c600vc.npy`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/data/metadata.yaml` & `pytme-0.2.0b0/tme/data/metadata.yaml`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/data/quat_to_numpy.py` & `pytme-0.2.0b0/tme/data/quat_to_numpy.py`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/density.py` & `pytme-0.2.0b0/tme/density.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-""" Implements class to represent electron density maps.
+""" Representation of N-dimensional densities
 
     Copyright (c) 2023 European Molecular Biology Laboratory
 
     Author: Valentin Maurer <valentin.maurer@embl-hamburg.de>
 """
 
 import warnings
 from io import BytesIO
 from copy import deepcopy
 from gzip import open as gzip_open
 from typing import Tuple, Dict, Set
 from os.path import splitext, basename
 
+import h5py
 import mrcfile
 import numpy as np
 import skimage.io as skio
 
 from scipy.ndimage import (
     laplace,
     generic_gradient_magnitude,
     minimum_filter,
     sobel,
     binary_erosion,
     zoom,
 )
 from scipy.spatial import ConvexHull
 
-from .matching_optimization import FitRefinement
 from .structure import Structure
 from .matching_utils import (
     minimum_enclosing_box,
     array_to_memmap,
     memmap_to_array,
 )
 from .types import NDArray
@@ -125,16 +125,16 @@
     ) -> "Density":
         """
         Reads in a file and converts it into :py:class:`Density` instance.
 
         Parameters
         ----------
         filename : str
-            Path to a file in CCP4/MRC, EM or a format supported by skimage.io.imread.
-            The file can be gzip compressed.
+            Path to a file in CCP4/MRC, EM, HDF5 or a format supported by
+            skimage.io.imread. The file can be gzip compressed.
         subset : tuple of slices, optional
             Slices representing the desired subset along each dimension.
         use_memmap : bool, optional
             Whether the Density objects data attribute should be memmory mapped.
 
         Returns
         -------
@@ -181,63 +181,62 @@
         to use skimage.io.imread to read the file [3]_. This fallback does not extract
         origin or sampling_rate information from the file:
 
         >>> Density.from_file("/path/to/other_format.tif")
 
         Notes
         -----
-        If ``filename`` ends with ".em" or ".em.gz" the method will parse it as EM file.
-        Otherwise it defaults to the CCP4/MRC format and on failure, switches to
+        If ``filename`` ends with ".em" or ".em.gz" the method will parse it as EM file,
+        if it ends with "h5" or "h5.gz" the method will parse the file as HDF5.
+        Otherwise the method defaults to the CCP4/MRC format and on failure, switches to
         :obj:`skimage.io.imread` regardless of the extension. Currently, the later does not
         extract origin or sampling_rate information from the file.
 
         See Also
         --------
         :py:meth:`Density.to_file`
 
         """
         try:
             func = cls._load_mrc
-            if filename.endswith(".em") or filename.endswith(".em.gz"):
+            if filename.endswith("em") or filename.endswith("em.gz"):
                 func = cls._load_em
+            elif filename.endswith("h5") or filename.endswith("h5.gz"):
+                func = cls._load_hdf5
             data, origin, sampling_rate, meta = func(
                 filename=filename, subset=subset, use_memmap=use_memmap
             )
         except ValueError:
             data, origin, sampling_rate, meta = cls._load_skio(filename=filename)
             if subset is not None:
                 cls._validate_slices(slices=subset, shape=data.shape)
                 data = data[subset].copy()
 
         return cls(data=data, origin=origin, sampling_rate=sampling_rate, metadata=meta)
 
     @classmethod
     def _load_mrc(
         cls, filename: str, subset: Tuple[int] = None, use_memmap: bool = False
-    ) -> Tuple[NDArray]:
+    ) -> Tuple[NDArray, NDArray, NDArray, Dict]:
         """
         Extracts data from a CCP4/MRC file.
 
         Parameters
         ----------
         filename : str
             Path to a file in CCP4/MRC format.
         subset : tuple of slices, optional
             Slices representing the desired subset along each dimension.
         use_memmap : bool, optional
             Whether the Density objects data attribute should be memmory mapped.
 
         Returns
         -------
-        NDArray
-            The data attribute of the CCP4/MRC file.
-        NDArray
-            The coordinate origin of the data.
-        NDArray
-            The sampling rate of the data.
+        Tuple[NDArray, NDArray, NDArray, Dict]
+            File data, coordinate origin, sampling rate array and metadata dictionary.
 
         References
         ----------
         .. [1] Burnley T, Palmer C & Winn M (2017) Recent developments in the
             CCP-EM software suite. Acta Cryst. D73:469–477.
             doi: 10.1107/S2059798317007859
 
@@ -351,47 +350,43 @@
             start = np.take(start, crs_index)
 
         return data, origin, sampling_rate, metadata
 
     @classmethod
     def _load_em(
         cls, filename: str, subset: Tuple[int] = None, use_memmap: bool = False
-    ) -> Tuple[NDArray]:
+    ) -> Tuple[NDArray, NDArray, NDArray, Dict]:
         """
         Extracts data from a EM file.
 
         Parameters
         ----------
         filename : str
             Path to a file in EM format.
         subset : tuple of slices, optional
             Slices representing the desired subset along each dimension.
         use_memmap : bool, optional
             Whether the Density objects data attribute should be memmory mapped.
 
         Returns
         -------
-        NDArray
-            The data attribute of the EM file.
-        NDArray
-            The coordinate origin of the data.
-        NDArray
-            The sampling rate of the data.
+        Tuple[NDArray, NDArray, NDArray, Dict]
+            File data, coordinate origin, sampling rate array and metadata dictionary.
 
         References
         ----------
         .. [1] Nickell S. et al, Journal of Structural Biology, 2005.
 
         Warns
         -----
-            Warns if the pixel size is zero.
+            If the sampling rate is zero.
 
         Notes
         -----
-        A pixel size of zero will be treated as missing value and changed to one. This
+        A sampling rate of zero will be treated as missing value and changed to one. This
         function does not yet extract an origin like :py:meth:`Density._load_mrc`.
 
         See Also
         --------
         :py:meth:`Density.from_file`
         """
         DATA_TYPE_CODING = {
@@ -479,18 +474,23 @@
 
         n_dims = len(shape)
         if len(slices) != n_dims:
             raise ValueError(
                 f"Expected length of slices : {n_dims}, got : {len(slices)}"
             )
 
-        if any([slices[i].stop > shape[i] for i in range(n_dims)]):
+        if any(
+            [
+                slices[i].stop > shape[i] or slices[i].start > shape[i]
+                for i in range(n_dims)
+            ]
+        ):
             raise ValueError(f"Subset exceeds data dimensions ({shape}).")
 
-        if any([slices[i].stop < 0 for i in range(n_dims)]):
+        if any([slices[i].stop < 0 or slices[i].start < 0 for i in range(n_dims)]):
             raise ValueError("Subsets have to be non-negative.")
 
     @classmethod
     def _read_binary_subset(
         cls,
         filename: str,
         slices: Tuple[slice],
@@ -556,31 +556,27 @@
                     f.seek(offset)
                     row = np.frombuffer(f.read(row_bytes), dtype=dtype)
                     subset_data[z - slices[0].start, y - slices[1].start] = row
 
         return subset_data
 
     @staticmethod
-    def _load_skio(filename: str) -> Tuple[NDArray]:
+    def _load_skio(filename: str) -> Tuple[NDArray, NDArray, NDArray, Dict]:
         """
         Uses :obj:`skimage.io.imread` to extract data from filename [1]_.
 
         Parameters
         ----------
         filename : str
             Path to a file whose format is supported by :obj:`skimage.io.imread`.
 
         Returns
         -------
-        NDArray
-            The data attribute of the file.
-        NDArray
-            The coordinate origin of the data.
-        NDArray
-            The sampling rate of the data.
+        Tuple[NDArray, NDArray, NDArray, Dict]
+            File data, coordinate origin, sampling rate array and metadata dictionary.
 
         References
         ----------
         .. [1] https://scikit-image.org/docs/stable/api/skimage.io.html
 
         Warns
         -----
@@ -597,14 +593,59 @@
 
         data = skio.imread(swap)
         warnings.warn(
             "origin and sampling_rate are not yet extracted from non CCP4/MRC files."
         )
         return data, np.zeros(data.ndim), np.ones(data.ndim), {}
 
+    @staticmethod
+    def _load_hdf5(
+        filename: str, subset: Tuple[slice], use_memmap: bool = False, **kwargs
+    ) -> "Density":
+        """
+        Extracts data from an H5 file.
+
+        Parameters
+        ----------
+        filename : str
+            Path to a file in CCP4/MRC format.
+        subset : tuple of slices, optional
+            Slices representing the desired subset along each dimension.
+        use_memmap : bool, optional
+            Whether the Density objects data attribute should be memmory mapped.
+
+        Returns
+        -------
+        Density
+            An instance of the Density class populated with the data from the HDF5 file.
+
+        See Also
+        --------
+        :py:meth:`Density._save_hdf5`
+        """
+        subset = ... if subset is None else subset
+
+        with h5py.File(filename, mode="r") as infile:
+            data = infile["data"]
+            data_attributes = [
+                infile["data"].id.get_offset(),
+                infile["data"].shape,
+                infile["data"].dtype,
+            ]
+            origin = infile["origin"][...].copy()
+            sampling_rate = infile["sampling_rate"][...].copy()
+            metadata = {key: val for key, val in infile.attrs.items()}
+            if not use_memmap:
+                return data[subset], origin, sampling_rate, metadata
+
+        offset, shape, dtype = data_attributes
+        data = np.memmap(filename, dtype=dtype, shape=shape, offset=offset)[subset]
+
+        return data, origin, sampling_rate, metadata
+
     @classmethod
     def from_structure(
         cls,
         filename_or_structure: str,
         shape: Tuple[int] = None,
         sampling_rate: NDArray = np.ones(1),
         origin: Tuple[float] = None,
@@ -794,34 +835,36 @@
 
         >>> data = np.random.rand(50,50)
         >>> dens = Density(data = data, origin = (0, 0), sampling_rate = (1, 1))
         >>> dens.to_file("example.tiff")
 
         Notes
         -----
-        If ``filename`` ends with ".em" or ".em.gz", the method will create an EM file.
-        Otherwise, it defaults to the CCP4/MRC format, and on failure, falls back
-        to :obj:`skimage.io.imsave`.
+        If ``filename`` ends with "em" or "em.gz" will create an EM file, "h5" or
+        "h5.gz" will create a HDF5 file. Otherwise, the method defaults to the CCP4/MRC
+        format, and on failure, falls back to :obj:`skimage.io.imsave`.
 
         See Also
         --------
         :py:meth:`Density.from_file`
         """
         if gzip:
             filename = filename if filename.endswith(".gz") else f"{filename}.gz"
 
         try:
             func = self._save_mrc
-            if filename.endswith(".em") or filename.endswith(".em.gz"):
+            if filename.endswith("em") or filename.endswith("em.gz"):
                 func = self._save_em
+            elif filename.endswith("h5") or filename.endswith("h5.gz"):
+                func = self._save_hdf5
             _ = func(filename=filename, gzip=gzip)
         except ValueError:
             _ = self._save_skio(filename=filename, gzip=gzip)
 
-    def _save_mrc(self, filename: str, gzip: bool) -> None:
+    def _save_mrc(self, filename: str, gzip: bool = False) -> None:
         """
         Writes current class instance to disk as mrc file.
 
         Parameters
         ----------
         filename : str
             Path to write to.
@@ -839,28 +882,24 @@
                 np.divide(self.origin, self.sampling_rate)
             )
             # mrcfile library expects origin to be in xyz format
             mrc.header.mapc, mrc.header.mapr, mrc.header.maps = (1, 2, 3)
             mrc.header["origin"] = tuple(self.origin[::-1])
             mrc.voxel_size = tuple(self.sampling_rate[::-1])
 
-    def _save_em(self, filename: str, gzip: bool) -> None:
+    def _save_em(self, filename: str, gzip: bool = False) -> None:
         """
         Writes data to disk as an .em file.
 
         Parameters
         ----------
         filename : str
-            Path to write the .em file to.
-        data : NDArray
-            Data to be saved.
-        origin : NDArray
-            Coordinate origin of the data.
-        sampling_rate : NDArray
-            Sampling rate of the data.
+            Path to write to.
+        gzip : bool, optional
+            If True, the output will be gzip compressed.
 
         References
         ----------
         .. [1] Nickell S. et al, Journal of Structural Biology, 2005.
         """
         DATA_TYPE_MAPPING = {
             np.dtype(np.int8): 1,
@@ -882,15 +921,15 @@
             f.write(b" " * 80)
             user_params = np.zeros(40, dtype="<i4")
             user_params[6] = int(self.sampling_rate[0] * 1000)
             f.write(user_params.tobytes())
             f.write(b" " * 256)
             f.write(self.data.tobytes())
 
-    def _save_skio(self, filename: str, gzip: bool) -> None:
+    def _save_skio(self, filename: str, gzip: bool = False) -> None:
         """
         Uses :obj:`skimage.io.imsave` to write data to filename [1]_.
 
         Parameters
         ----------
         filename : str
             Path to write to with a format supported by :obj:`skimage.io.imsave`.
@@ -900,20 +939,62 @@
         References
         ----------
         .. [1] https://scikit-image.org/docs/stable/api/skimage.io.html
         """
         swap, kwargs = filename, {}
         if gzip:
             swap = BytesIO()
-            kwargs["format"] = splitext(basename(filename.replace(".gz", "")))[1]
+            kwargs["format"] = splitext(basename(filename.replace(".gz", "")))[
+                1
+            ].replace(".", "")
         skio.imsave(fname=swap, arr=self.data.astype("float32"), **kwargs)
         if gzip:
             with gzip_open(filename, "wb") as outfile:
                 outfile.write(swap.getvalue())
 
+    def _save_hdf5(self, filename: str, gzip: bool = False) -> None:
+        """
+        Saves the Density instance data to an HDF5 file, with optional compression.
+
+        Parameters
+        ----------
+        filename : str
+            Path to write to.
+        gzip : bool, optional
+            If True, the output will be gzip compressed.
+
+        See Also
+        --------
+        :py:meth:`Density._load_hdf5`
+        """
+        compression = "gzip" if gzip else None
+        with h5py.File(filename, mode="w") as f:
+            f.create_dataset(
+                "data",
+                data=self.data,
+                shape=self.data.shape,
+                dtype=self.data.dtype,
+                compression=compression,
+            )
+            f.create_dataset("origin", data=self.origin)
+            f.create_dataset("sampling_rate", data=self.sampling_rate)
+
+            self.metadata["mean"] = self.metadata.get("mean", 0)
+            self.metadata["std"] = self.metadata.get("std", 0)
+            self.metadata["min"] = self.metadata.get("min", 0)
+            self.metadata["max"] = self.metadata.get("max", 0)
+            if type(self.data) != np.memmap:
+                self.metadata["mean"] = self.data.mean()
+                self.metadata["std"] = self.data.std()
+                self.metadata["min"] = self.data.min()
+                self.metadata["max"] = self.data.max()
+
+            for key, val in self.metadata.items():
+                f.attrs[key] = val
+
     @property
     def empty(self) -> "Density":
         """
         Returns a copy of the current class instance with all elements in
         :py:attr:`Density.data` set to zero. :py:attr:`Density.origin` and
         :py:attr:`Density.sampling_rate` will be copied, while
         :py:attr:`Density.metadata` will be initialized to contain min, max,
@@ -1094,15 +1175,21 @@
         origin = np.asarray(origin)
         origin = np.repeat(origin, self.data.ndim // origin.size)
         self._origin = origin
 
     @property
     def sampling_rate(self) -> NDArray:
         """
-        Returns sampling rate along data axis.
+        Returns the value of the current instance's :py:attr:`Density.sampling_rate`
+        attribute.
+
+        Returns
+        -------
+        NDArray
+            Sampling rate along axis.
         """
         return self._sampling_rate
 
     @sampling_rate.setter
     def sampling_rate(self, sampling_rate: NDArray) -> None:
         """
         Sets the sampling rate of the class instance.
@@ -1110,15 +1197,20 @@
         sampling_rate = np.asarray(sampling_rate)
         sampling_rate = np.repeat(sampling_rate, self.data.ndim // sampling_rate.size)
         self._sampling_rate = sampling_rate
 
     @property
     def metadata(self) -> Dict:
         """
-        Returns dictionary with metadata information, empty by default.
+        Returns the current instance's :py:attr:`Density.metadata` dictionary attribute.
+
+        Returns
+        -------
+        Dict
+            Metadata dictionary. Empty by default.
         """
         return self._metadata
 
     @metadata.setter
     def metadata(self, metadata: Dict) -> None:
         """
         Sets the metadata of the class instance.
@@ -2064,89 +2156,90 @@
     ) -> Tuple["Density", NDArray, NDArray, NDArray]:
         """
         Aligns two :py:class:`Density` instances target and template and returns
         the aligned template.
 
         If voxel sizes of target and template dont match coordinates are scaled
         to the numerically smaller voxel size. Instances are prealigned based on their
-        center of mass. Finally :py:class:`tme.matching_optimization.FitRefinement` is
+        center of mass. Finally :py:meth:`tme.matching_optimization.optimize_match` is
         used to determine translation and rotation to map template to target.
 
         Parameters
         ----------
         target : Density
             The target map for alignment.
         template : Density
             The template that should be aligned to the target.
         cutoff_target : float, optional
             The cutoff value for the target map, by default 0.
         cutoff_template : float, optional
             The cutoff value for the template map, by default 0.
         scoring_method : str, optional
             The scoring method to use for alignment. See
-            :py:class:`tme.matching_optimization.FitRefinement` for available methods,
+            :py:class:`tme.matching_optimization.create_score_object` for available methods,
             by default "NormalizedCrossCorrelation".
 
         Returns
         -------
         Tuple
             Tuple containing template aligned to target as :py:class:`Density` object,
             translation in voxels and rotation matrix used for the transformation.
 
         Notes
         -----
         No densities below cutoff_template are present in the returned Density object.
         """
+        from .matching_optimization import optimize_match, create_score_object
+
         target_sampling_rate = np.array(target.sampling_rate)
         template_sampling_rate = np.array(template.sampling_rate)
 
         target_sampling_rate = np.repeat(
             target_sampling_rate, target.data.ndim // target_sampling_rate.size
         )
         template_sampling_rate = np.repeat(
             template_sampling_rate, template.data.ndim // template_sampling_rate.size
         )
-
         if not np.allclose(target_sampling_rate, template_sampling_rate):
             print(
                 "Voxel size of target and template do not match. "
                 "Using smaller voxel size for refinement."
             )
 
         target_coordinates = target.to_pointcloud(cutoff_target)
-        target_weights = target.data[tuple(target_coordinates)]
 
         template_coordinates = template.to_pointcloud(cutoff_template)
         template_weights = template.data[tuple(template_coordinates)]
 
         refinement_sampling_rate = np.minimum(
             target_sampling_rate, template_sampling_rate
         )
         target_scaling = np.divide(target_sampling_rate, refinement_sampling_rate)
         template_scaling = np.divide(template_sampling_rate, refinement_sampling_rate)
         target_coordinates = target_coordinates * target_scaling[:, None]
         template_coordinates = template_coordinates * template_scaling[:, None]
 
-        target_mass_center = cls.center_of_mass(target.data, cutoff_target)
-        template_mass_center = cls.center_of_mass(template.data, cutoff_template)
         mass_center_difference = np.subtract(
-            target_mass_center, template_mass_center
+            cls.center_of_mass(target.data, cutoff_target),
+            cls.center_of_mass(template.data, cutoff_template),
         ).astype(int)
         template_coordinates += mass_center_difference[:, None]
 
-        matcher = FitRefinement()
-        translation, rotation_matrix, score = matcher.refine(
-            target_coordinates=target_coordinates,
+        score_object = create_score_object(
+            score=scoring_method,
+            target=target.data,
             template_coordinates=template_coordinates,
-            target_weights=target_weights,
             template_weights=template_weights,
-            scoring_class=scoring_method,
             sampling_rate=np.ones(template.data.ndim),
         )
 
+        translation, rotation_matrix, score = optimize_match(
+            score_object=score_object, optimization_method="basinhopping"
+        )
+
         translation += mass_center_difference
         translation = np.divide(translation, template_scaling)
 
         template.sampling_rate = template_sampling_rate.copy()
         ret = template.rigid_transform(
             rotation_matrix=rotation_matrix, use_geometric_center=False
         )
@@ -2165,30 +2258,30 @@
     ) -> Tuple["Structure", NDArray, NDArray]:
         """
         Aligns a :py:class:`tme.structure.Structure` template to :py:class:`Density`
         target and returns an aligned :py:class:`tme.structure.Structure` instance.
 
         If voxel sizes of target and template dont match coordinates are scaled
         to the numerically smaller voxel size. Prealignment is done by center's
-        of mass. Finally :py:class:`tme.matching_optimization.FitRefinement` is used to
+        of mass. Finally :py:class:`tme.matching_optimization.optimize_match` is used to
         determine translation and rotation to match a template to target.
 
         Parameters
         ----------
         target : Density
             The target map for template matching.
         template : Structure
             The template that should be aligned to the target.
         cutoff_target : float, optional
             The cutoff value for the target map, by default 0.
         cutoff_template : float, optional
             The cutoff value for the template map, by default 0.
         scoring_method : str, optional
             The scoring method to use for template matching. See
-            :py:class:`tme.matching_optimization.FitRefinement` for available methods,
+            :py:class:`tme.matching_optimization.create_score_object` for available methods,
             by default "NormalizedCrossCorrelation".
 
         Returns
         -------
         Structure
             Tuple containing template aligned to target as
             :py:class:`tme.structure.Structure` object, translation and rotation
```

### Comparing `pytme-0.1.9/tme/helpers.py` & `pytme-0.2.0b0/tme/helpers.py`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/matching_data.py` & `pytme-0.2.0b0/tme/matching_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,17 @@
         self._target_pad = np.zeros(len(target.shape), dtype=int)
         self._template_pad = np.zeros(len(template.shape), dtype=int)
 
         self.template_filter = {}
         self.target_filter = {}
 
         self._invert_target = False
+        self._rotations = None
+
+        self._set_batch_dimension()
 
     @staticmethod
     def _shape_to_slice(shape: Tuple[int]):
         return tuple(slice(0, dim) for dim in shape)
 
     @classmethod
     def _slice_to_mesh(cls, slice_variable: (slice,), shape: (int,)):
@@ -145,21 +148,21 @@
                     arr.filename, mode="r", shape=arr.shape, dtype=arr.dtype
                 )
             arr = np.asarray(arr[*arr_mesh])
 
         def _warn_on_mismatch(
             expectation: float, computation: float, name: str
         ) -> float:
-            expectation, computation = float(expectation), float(computation)
             if expectation is None:
                 expectation = computation
+            expectation, computation = float(expectation), float(computation)
 
             if abs(computation) > abs(expectation):
                 warnings.warn(
-                    f"Computed {name} value is more extreme than value specified in file"
+                    f"Computed {name} value is more extreme than value in file header"
                     f" (|{computation}| > |{expectation}|). This may lead to issues"
                     " with padding and contrast inversion."
                 )
 
             return expectation
 
         padding = tuple(
@@ -172,19 +175,17 @@
         ret = np.pad(arr, padding, mode="reflect")
 
         if invert:
             arr_min = _warn_on_mismatch(arr_min, arr.min(), "min")
             arr_max = _warn_on_mismatch(arr_max, arr.max(), "max")
 
             # Avoid in-place operation in case ret is not floating point
-            ret = np.divide(
-                np.subtract(-ret, arr_min),
-                np.subtract(arr_max, arr_min)
+            ret = (
+                -np.divide(np.subtract(ret, arr_min), np.subtract(arr_max, arr_min)) + 1
             )
-
         return ret
 
     def subset_by_slice(
         self,
         target_slice: Tuple[slice] = None,
         template_slice: Tuple[slice] = None,
         target_pad: NDArray = None,
@@ -219,22 +220,24 @@
             target_slice = self._shape_to_slice(target_shape)
         if template_slice is None:
             template_slice = self._shape_to_slice(template_shape)
 
         if target_pad is None:
             target_pad = np.zeros(len(self._target.shape), dtype=int)
         if template_pad is None:
-            template_pad = np.zeros(len(self._target.shape), dtype=int)
+            template_pad = np.zeros(len(self._template.shape), dtype=int)
 
-        indices = compute_full_convolution_index(
-            outer_shape=self._target.shape,
-            inner_shape=self._template.shape,
-            outer_split=target_slice,
-            inner_split=template_slice,
-        )
+        indices = None
+        if len(self._target.shape) == len(self._template.shape):
+            indices = compute_full_convolution_index(
+                outer_shape=self._target.shape,
+                inner_shape=self._template.shape,
+                outer_split=target_slice,
+                inner_split=template_slice,
+            )
 
         target_subset = self.subset_array(
             arr=self._target,
             arr_slice=target_slice,
             padding=target_pad,
             invert=self._invert_target,
         )
@@ -242,21 +245,27 @@
         template_subset = self.subset_array(
             arr=self._template,
             arr_slice=template_slice,
             padding=template_pad,
         )
         ret = self.__class__(target=target_subset, template=template_subset)
 
-        ret._translation_offset = np.add(
-            [x.start for x in target_slice],
-            [x.start for x in template_slice],
-        )
-        ret.template_filter = self.template_filter
+        target_offset = np.zeros(len(self._output_target_shape), dtype=int)
+        target_offset[(target_offset.size - len(target_slice)) :] = [
+            x.start for x in target_slice
+        ]
+        template_offset = np.zeros(len(self._output_target_shape), dtype=int)
+        template_offset[(template_offset.size - len(template_slice)) :] = [
+            x.start for x in template_slice
+        ]
+        ret._translation_offset = np.add(target_offset, template_offset)
 
-        ret.rotations, ret.indices = self.rotations, indices
+        ret.template_filter = self.template_filter
+        ret.target_filter = self.target_filter
+        ret._rotations, ret.indices = self.rotations, indices
         ret._target_pad, ret._template_pad = target_pad, template_pad
         ret._invert_target = self._invert_target
 
         if self._target_mask is not None:
             ret.target_mask = self.subset_array(
                 arr=self._target_mask, arr_slice=target_slice, padding=target_pad
             )
@@ -278,18 +287,22 @@
 
         return ret
 
     def to_backend(self) -> None:
         """
         Transfer the class instance's numpy arrays to the current backend.
         """
+        backend_arr = type(backend.zeros((1), dtype=backend._default_dtype))
         for attr_name, attr_value in vars(self).items():
             if isinstance(attr_value, np.ndarray):
                 converted_array = backend.to_backend_array(attr_value.copy())
                 setattr(self, attr_name, converted_array)
+            elif isinstance(attr_value, backend_arr):
+                converted_array = backend.to_backend_array(attr_value)
+                setattr(self, attr_name, converted_array)
 
         self._default_dtype = backend._default_dtype
         self._complex_dtype = backend._complex_dtype
 
     def _set_batch_dimension(
         self, target_dims: Tuple[int] = None, template_dims: Tuple[int] = None
     ) -> None:
@@ -423,21 +436,21 @@
 
         Returns
         -------
         ArrayLike
             An array indicating the padding for each dimension of the target.
         """
         target_padding = backend.zeros(
-            len(self.target.shape), dtype=backend._default_dtype_int
+            len(self._output_target_shape), dtype=backend._default_dtype_int
         )
 
         if pad_target:
             backend.subtract(
-                self._template.shape,
-                backend.mod(self._template.shape, 2),
+                self._output_template_shape,
+                backend.mod(self._output_template_shape, 2),
                 out=target_padding,
             )
             if hasattr(self, "_is_target_batch"):
                 target_padding[self._is_target_batch] = 0
 
         return target_padding
 
@@ -471,28 +484,38 @@
             target_shape = self._output_target_shape
         target_shape = backend.to_backend_array(target_shape)
 
         fourier_pad = backend.to_backend_array(template_shape)
         fourier_shift = backend.zeros(len(fourier_pad))
 
         if not pad_fourier:
-            fourier_pad = backend.full(shape=len(fourier_pad), fill_value=1, dtype=int)
+            fourier_pad = backend.full(
+                shape=(len(fourier_pad),),
+                fill_value=1,
+                dtype=backend._default_dtype_int,
+            )
 
         fourier_pad = backend.to_backend_array(fourier_pad)
         if hasattr(self, "_batch_mask"):
             batch_mask = backend.to_backend_array(self._batch_mask)
             fourier_pad[batch_mask] = 1
 
-        ret = backend.compute_convolution_shapes(target_shape, fourier_pad)
+        pad_shape = backend.maximum(target_shape, template_shape)
+        ret = backend.compute_convolution_shapes(pad_shape, fourier_pad)
         convolution_shape, fast_shape, fast_ft_shape = ret
         if not pad_fourier:
             fourier_shift = 1 - backend.astype(backend.divide(template_shape, 2), int)
             fourier_shift -= backend.mod(template_shape, 2)
             shape_diff = backend.subtract(fast_shape, convolution_shape)
             shape_diff = backend.astype(backend.divide(shape_diff, 2), int)
+
+            if hasattr(self, "_batch_mask"):
+                batch_mask = backend.to_backend_array(self._batch_mask)
+                shape_diff[batch_mask] = 0
+
             backend.add(fourier_shift, shape_diff, out=fourier_shift)
 
         return fast_shape, fast_ft_shape, fourier_shift
 
     @property
     def rotations(self):
         """Return stored rotation matrices.."""
@@ -519,23 +542,29 @@
             raise ValueError("Rotations have to be a rank 2 or 3 array.")
         self._rotations = rotations.astype(self._default_dtype)
 
     @property
     def target(self):
         """Returns the target NDArray."""
         if isinstance(self._target, Density):
-            return self._target.data
-        return self._target
+            target = self._target.data
+        else:
+            target = self._target
+        out_shape = backend.to_numpy_array(self._output_target_shape)
+        return target.reshape(tuple(int(x) for x in out_shape))
 
     @property
     def template(self):
         """Returns the reversed template NDArray."""
+        template = self._template
         if isinstance(self._template, Density):
-            return backend.reverse(self._template.data)
-        return backend.reverse(self._template)
+            template = self._template.data
+        template = backend.reverse(template)
+        out_shape = backend.to_numpy_array(self._output_template_shape)
+        return template.reshape(tuple(int(x) for x in out_shape))
 
     @template.setter
     def template(self, template: NDArray):
         """
         Set the template array. If not already defined, also initializes
         :py:attr:`MatchingData.template_mask` to an uninformative mask filled with
         ones.
@@ -554,17 +583,23 @@
         if type(template) == Density:
             template = template.data
         self._template = template.astype(self._default_dtype, copy=False)
 
     @property
     def target_mask(self):
         """Returns the target mask NDArray."""
+        target_mask = self._target_mask
         if isinstance(self._target_mask, Density):
-            return self._target_mask.data
-        return self._target_mask
+            target_mask = self._target_mask.data
+
+        if target_mask is not None:
+            out_shape = backend.to_numpy_array(self._output_target_shape)
+            target_mask = target_mask.reshape(tuple(int(x) for x in out_shape))
+
+        return target_mask
 
     @target_mask.setter
     def target_mask(self, mask: NDArray):
         """Sets the target mask."""
         if not np.all(self.target.shape == mask.shape):
             raise ValueError("Target and its mask have to have the same shape.")
 
@@ -583,17 +618,23 @@
         Set the template mask array after reversing it.
 
         Parameters
         ----------
         template : NDArray
             Array to set as the template.
         """
+        mask = self._template_mask
         if isinstance(self._template_mask, Density):
-            return backend.reverse(self._template_mask.data)
-        return backend.reverse(self._template_mask)
+            mask = self._template_mask.data
+
+        if mask is not None:
+            mask = backend.reverse(mask)
+            out_shape = backend.to_numpy_array(self._output_template_shape)
+            mask = mask.reshape(tuple(int(x) for x in out_shape))
+        return mask
 
     @template_mask.setter
     def template_mask(self, mask: NDArray):
         """Returns the reversed template mask NDArray."""
         if not np.all(self._templateshape[::-1] == mask.shape):
             raise ValueError("Target and its mask have to have the same shape.")
```

### Comparing `pytme-0.1.9/tme/matching_exhaustive.py` & `pytme-0.2.0b0/tme/matching_exhaustive.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from .matching_utils import (
     apply_convolution_mode,
     handle_traceback,
     split_numpy_array_slices,
     conditional_execute,
 )
 from .matching_memory import MatchingMemoryUsage, MATCHING_MEMORY_REGISTRY
+# from .preprocessing import Compose
 from .preprocessor import Preprocessor
 from .matching_data import MatchingData
 from .backends import backend
 from .types import NDArray, CallbackClass
 
 os.environ["MKL_NUM_THREADS"] = "1"
 os.environ["OMP_NUM_THREADS"] = "1"
@@ -39,14 +40,66 @@
 def _run_inner(backend_name, backend_args, **kwargs):
     from tme.backends import backend
 
     backend.change_backend(backend_name, **backend_args)
     return scan(**kwargs)
 
 
+def normalize_under_mask(template: NDArray, mask: NDArray, mask_intensity) -> None:
+    """
+    Standardizes the values in in template by subtracting the mean and dividing by the
+    standard deviation based on the elements in mask. Subsequently, the template is
+    multiplied by the mask.
+
+    Parameters
+    ----------
+    template : NDArray
+        The data array to be normalized. This array is modified in-place.
+    mask : NDArray
+        A boolean array of the same shape as `template`. True values indicate the positions in `template`
+        to consider for normalization.
+    mask_intensity : float
+        Mask intensity used to compute expectations.
+
+    References
+    ----------
+    .. [1]  T. Hrabe, Y. Chen, S. Pfeffer, L. Kuhn Cuellar, A.-V. Mangold,
+            and F. Förster, J. Struct. Biol. 178, 177 (2012).
+    .. [2]  M. L. Chaillet, G. van der Schot, I. Gubins, S. Roet,
+            R. C. Veltkamp, and F. Förster, Int. J. Mol. Sci. 24,
+            13375 (2023)
+
+    Returns
+    -------
+    None
+        This function modifies `template` in-place and does not return any value.
+    """
+    masked_mean = backend.sum(backend.multiply(template, mask))
+    masked_mean = backend.divide(masked_mean, mask_intensity)
+    masked_std = backend.sum(backend.multiply(backend.square(template), mask))
+    masked_std = backend.subtract(
+        masked_std / mask_intensity, backend.square(masked_mean)
+    )
+    masked_std = backend.sqrt(backend.maximum(masked_std, 0))
+
+    backend.subtract(template, masked_mean, out=template)
+    backend.divide(template, masked_std, out=template)
+    backend.multiply(template, mask, out=template)
+    return None
+
+
+def apply_filter(ft_template, template_filter):
+    # This is an approximation to applying the mask, irfftn, normalize, rfftn
+    std_before = backend.std(ft_template)
+    backend.multiply(ft_template, template_filter, out=ft_template)
+    backend.multiply(
+        ft_template, std_before / backend.std(ft_template), out=ft_template
+    )
+
+
 def cc_setup(
     rfftn: Callable,
     irfftn: Callable,
     template: NDArray,
     target: NDArray,
     fast_shape: Tuple[int],
     fast_ft_shape: Tuple[int],
@@ -208,21 +261,20 @@
     target_pad, ft_target2, ft_window_template = None, None, None
 
     # Normalizing constants
     n_observations = backend.sum(template_mask)
     template_mean = backend.sum(backend.multiply(template, template_mask))
     template_mean = backend.divide(template_mean, n_observations)
     template_ssd = backend.sum(
-        backend.square(backend.multiply(
-            backend.multiply(template, template_mean),
-            template_mask
-        ))
+        backend.square(
+            backend.multiply(backend.multiply(template, template_mean), template_mask)
+        )
     )
     template_volume = np.prod(template.shape)
-    backend.multiply(template, template_mask, out = template)
+    backend.multiply(template, template_mask, out=template)
 
     # Final numerator is score - numerator2
     numerator2 = backend.multiply(target_window_sum, template_mean)
 
     # Compute denominator
     backend.multiply(target_window_sum, target_window_sum, out=target_window_sum)
     backend.divide(target_window_sum, template_volume, out=target_window_sum)
@@ -310,57 +362,14 @@
     :py:meth:`corr_scoring`.
     :py:class:`tme.matching_optimization.NormalizedCrossCorrelationMean`.
     """
     kwargs["template"] = kwargs["template"] - kwargs["template"].mean()
     return corr_setup(**kwargs)
 
 
-def _normalize_under_mask(template: NDArray, mask: NDArray, mask_intensity) -> None:
-    """
-    Standardizes the values in in template by subtracting the mean and dividing by the
-    standard deviation based on the elements in mask. Subsequently, the template is
-    multiplied by the mask.
-
-    Parameters
-    ----------
-    template : NDArray
-        The data array to be normalized. This array is modified in-place.
-    mask : NDArray
-        A boolean array of the same shape as `template`. True values indicate the positions in `template`
-        to consider for normalization.
-    mask_intensity : float
-        Mask intensity used to compute expectations.
-
-    References
-    ----------
-    .. [1]  T. Hrabe, Y. Chen, S. Pfeffer, L. Kuhn Cuellar, A.-V. Mangold,
-            and F. Förster, J. Struct. Biol. 178, 177 (2012).
-    .. [2]  M. L. Chaillet, G. van der Schot, I. Gubins, S. Roet,
-            R. C. Veltkamp, and F. Förster, Int. J. Mol. Sci. 24,
-            13375 (2023)
-
-    Returns
-    -------
-    None
-        This function modifies `template` in-place and does not return any value.
-    """
-    masked_mean = backend.sum(backend.multiply(template, mask))
-    masked_mean = backend.divide(masked_mean, mask_intensity)
-    masked_std = backend.sum(backend.multiply(backend.square(template), mask))
-    masked_std = backend.subtract(
-        masked_std / mask_intensity, backend.square(masked_mean)
-    )
-    masked_std = backend.sqrt(backend.maximum(masked_std, 0))
-
-    backend.subtract(template, masked_mean, out=template)
-    backend.divide(template, masked_std, out=template)
-    backend.multiply(template, mask, out=template)
-    return None
-
-
 def flc_setup(
     rfftn: Callable,
     irfftn: Callable,
     template: NDArray,
     template_mask: NDArray,
     target: NDArray,
     fast_shape: Tuple[int],
@@ -415,15 +424,15 @@
     ft_target = backend.arr_to_sharedarr(
         arr=ft_target, shared_memory_handler=shared_memory_handler
     )
     ft_target2 = backend.arr_to_sharedarr(
         arr=ft_target2, shared_memory_handler=shared_memory_handler
     )
 
-    _normalize_under_mask(
+    normalize_under_mask(
         template=template, mask=template_mask, mask_intensity=backend.sum(template_mask)
     )
 
     template_buffer = backend.arr_to_sharedarr(
         arr=template, shared_memory_handler=shared_memory_handler
     )
     template_mask_buffer = backend.arr_to_sharedarr(
@@ -537,15 +546,15 @@
 
     tol = 1e3 * eps * backend.max(backend.abs(temp))
     nonzero_indices = temp > tol
 
     backend.fill(temp2, 0)
     temp2[nonzero_indices] = 1 / temp[nonzero_indices]
 
-    _normalize_under_mask(
+    normalize_under_mask(
         template=template, mask=template_mask, mask_intensity=backend.sum(template_mask)
     )
 
     template_buffer = backend.arr_to_sharedarr(
         arr=template, shared_memory_handler=shared_memory_handler
     )
     template_mask_buffer = backend.arr_to_sharedarr(
@@ -724,18 +733,14 @@
         Tuple containing a pointer to the fourier tranform of the target,
         its shape, and its datatype.
     inv_denominator : Tuple[type, Tuple[int], type]
         Tuple containing a pointer to the inverse denominator data, its shape, and its
         datatype.
     numerator2 : Tuple[type, Tuple[int], type]
         Tuple containing a pointer to the numerator2 data, its shape, and its datatype.
-    targetshape : Tuple[int]
-        The shape of the target.
-    templateshape : Tuple[int]
-        The shape of the template.
     fast_shape : Tuple[int]
         The shape for fast Fourier transform.
     fast_ft_shape : Tuple[int]
         The shape for fast Fourier transform of the target.
     rotations : NDArray
         Array containing the rotation matrices to be applied on the template.
     real_dtype : type
@@ -746,16 +751,14 @@
         A callable class or function for processing the results after each
         rotation.
     callback_class_args : Dict
         Dictionary of arguments to be passed to the callback class if it's
         instantiable.
     interpolation_order : int
         The order of interpolation to be used while rotating the template.
-    convolution_mode : str, optional
-        Mode to use for convolution, default is "full".
     **kwargs :
         Additional arguments to be passed to the function.
 
     Returns
     -------
     CallbackClass
         If callback_class was provided an instance of callback_class otherwise None.
@@ -763,45 +766,31 @@
     See Also
     --------
     :py:meth:`cc_setup`
     :py:meth:`corr_setup`
     :py:meth:`cam_setup`
     :py:meth:`flcSphericalMask_setup`
     """
-    template_buffer, template_shape, template_dtype = template
-    ft_target_buffer, ft_target_shape, ft_target_dtype = ft_target
-    inv_denominator_buffer, inv_denominator_pointer_shape, _ = inv_denominator
-    numerator2_buffer, numerator2_shape, _ = numerator2
-    filter_buffer, filter_shape, filter_dtype = template_filter
-
+    callback = callback_class
     if callback_class is not None and isinstance(callback_class, type):
         callback = callback_class(**callback_class_args)
-    elif not isinstance(callback_class, type):
-        callback = callback_class
 
-    # Retrieve objects from shared memory
-    template = backend.sharedarr_to_arr(template_shape, template_dtype, template_buffer)
-    ft_target = backend.sharedarr_to_arr(
-        ft_target_shape, ft_target_dtype, ft_target_buffer
-    )
-    inv_denominator = backend.sharedarr_to_arr(
-        inv_denominator_pointer_shape, template_dtype, inv_denominator_buffer
-    )
-    numerator2 = backend.sharedarr_to_arr(
-        numerator2_shape, template_dtype, numerator2_buffer
-    )
-    template_filter = backend.sharedarr_to_arr(
-        filter_shape, filter_dtype, filter_buffer
-    )
+    template_buffer, template_shape, template_dtype = template
+    template = backend.sharedarr_to_arr(template_buffer, template_shape, template_dtype)
+    ft_target = backend.sharedarr_to_arr(*ft_target)
+    inv_denominator = backend.sharedarr_to_arr(*inv_denominator)
+    numerator2 = backend.sharedarr_to_arr(*numerator2)
+    template_filter = backend.sharedarr_to_arr(*template_filter)
 
     norm_template, template_mask, mask_sum = False, 1, 1
     if "template_mask" in kwargs:
-        template_mask = backend.sharedarr_to_arr(template_shape, template_dtype, kwargs["template_mask"][0])
+        template_mask = backend.sharedarr_to_arr(
+            kwargs["template_mask"][0], template_shape, template_dtype
+        )
         norm_template, mask_sum = True, backend.sum(template_mask)
-    norm_template = conditional_execute(_normalize_under_mask, norm_template)
 
     arr = backend.preallocate_array(fast_shape, real_dtype)
     ft_temp = backend.preallocate_array(fast_ft_shape, complex_dtype)
 
     rfftn, irfftn = backend.build_fft(
         fast_shape=fast_shape,
         fast_ft_shape=fast_ft_shape,
@@ -812,64 +801,52 @@
         temp_fft=ft_temp,
     )
 
     norm_numerator = (backend.sum(numerator2) != 0) & (backend.size(numerator2) != 1)
     norm_denominator = (backend.sum(inv_denominator) != 1) & (
         backend.size(inv_denominator) != 1
     )
-    filter_template = backend.size(template_filter) != 0
 
+    norm_template = conditional_execute(normalize_under_mask, norm_template)
+    callback_func = conditional_execute(callback, callback_class is not None)
     norm_func_numerator = conditional_execute(backend.subtract, norm_numerator)
     norm_func_denominator = conditional_execute(backend.multiply, norm_denominator)
-    template_filter_func = conditional_execute(backend.multiply, filter_template)
-
-    axis = tuple(range(arr.ndim))
-    fourier_shift = callback_class_args.get("fourier_shift", backend.zeros(arr.ndim))
-    fourier_shift_scores = backend.sum(fourier_shift != 0) != 0
+    template_filter_func = conditional_execute(
+        apply_filter, backend.size(template_filter) != 1
+    )
 
-    template_sum = backend.sum(template)
     unpadded_slice = tuple(slice(0, stop) for stop in template.shape)
     for index in range(rotations.shape[0]):
         rotation = rotations[index]
         backend.fill(arr, 0)
         backend.rotate_array(
             arr=template,
             rotation_matrix=rotation,
             out=arr,
             use_geometric_center=False,
             order=interpolation_order,
         )
-        rotation_norm = template_sum / backend.sum(arr)
-        backend.multiply(arr, rotation_norm, out=arr)
+
         norm_template(arr[unpadded_slice], template_mask, mask_sum)
 
         rfftn(arr, ft_temp)
-        template_filter_func(ft_temp, template_filter, out=ft_temp)
-
+        template_filter_func(ft_template=ft_temp, template_filter=template_filter)
         backend.multiply(ft_target, ft_temp, out=ft_temp)
         irfftn(ft_temp, arr)
 
         norm_func_numerator(arr, numerator2, out=arr)
         norm_func_denominator(arr, inv_denominator, out=arr)
 
-        if fourier_shift_scores:
-            arr = backend.roll(arr, shift=fourier_shift, axis=axis)
-
-        score = apply_convolution_mode(
-            arr, convolution_mode=convolution_mode, s1=targetshape, s2=templateshape
+        callback_func(
+            arr,
+            rotation_matrix=rotation,
+            rotation_index=index,
+            **callback_class_args,
         )
 
-        if callback_class is not None:
-            callback(
-                score,
-                rotation_matrix=rotation,
-                rotation_index=index,
-                **callback_class_args,
-            )
-
     return callback
 
 
 def flc_scoring(
     template: Tuple[type, Tuple[int], type],
     template_mask: Tuple[type, Tuple[int], type],
     ft_target: Tuple[type, Tuple[int], type],
@@ -909,40 +886,23 @@
     References
     ----------
     .. [1]  W. Wan, S. Khavnekar, J. Wagner, P. Erdmann, and W. Baumeister
             Microsc. Microanal. 26, 2516 (2020)
     .. [2]  T. Hrabe, Y. Chen, S. Pfeffer, L. Kuhn Cuellar, A.-V. Mangold,
             and F. Förster, J. Struct. Biol. 178, 177 (2012).
     """
-    template_buffer, template_shape, template_dtype = template
-    template_mask_buffer, *_ = template_mask
-    filter_buffer, filter_shape, filter_dtype = template_filter
-
-    ft_target_buffer, ft_target_shape, ft_target_dtype = ft_target
-    ft_target2_buffer, *_ = ft_target2
-
+    callback = callback_class
     if callback_class is not None and isinstance(callback_class, type):
         callback = callback_class(**callback_class_args)
-    elif not isinstance(callback_class, type):
-        callback = callback_class
 
-    # Retrieve objects from shared memory
-    template = backend.sharedarr_to_arr(template_shape, template_dtype, template_buffer)
-    template_mask = backend.sharedarr_to_arr(
-        template_shape, template_dtype, template_mask_buffer
-    )
-    ft_target = backend.sharedarr_to_arr(
-        ft_target_shape, ft_target_dtype, ft_target_buffer
-    )
-    ft_target2 = backend.sharedarr_to_arr(
-        ft_target_shape, ft_target_dtype, ft_target2_buffer
-    )
-    template_filter = backend.sharedarr_to_arr(
-        filter_shape, filter_dtype, filter_buffer
-    )
+    template = backend.sharedarr_to_arr(*template)
+    template_mask = backend.sharedarr_to_arr(*template_mask)
+    ft_target = backend.sharedarr_to_arr(*ft_target)
+    ft_target2 = backend.sharedarr_to_arr(*ft_target2)
+    template_filter = backend.sharedarr_to_arr(*template_filter)
 
     arr = backend.preallocate_array(fast_shape, real_dtype)
     temp = backend.preallocate_array(fast_shape, real_dtype)
     temp2 = backend.preallocate_array(fast_shape, real_dtype)
 
     ft_temp = backend.preallocate_array(fast_ft_shape, complex_dtype)
     ft_denom = backend.preallocate_array(fast_ft_shape, complex_dtype)
@@ -953,20 +913,18 @@
         real_dtype=real_dtype,
         complex_dtype=complex_dtype,
         fftargs=kwargs.get("fftargs", {}),
         temp_real=arr,
         temp_fft=ft_temp,
     )
     eps = backend.eps(real_dtype)
-    filter_template = backend.size(template_filter) != 0
-    template_filter_func = conditional_execute(backend.multiply, filter_template)
-
-    axis = tuple(range(arr.ndim))
-    fourier_shift = callback_class_args.get("fourier_shift", backend.zeros(arr.ndim))
-    fourier_shift_scores = backend.sum(fourier_shift != 0) != 0
+    template_filter_func = conditional_execute(
+        apply_filter, backend.size(template_filter) != 1
+    )
+    callback_func = conditional_execute(callback, callback_class is not None)
 
     unpadded_slice = tuple(slice(0, stop) for stop in template.shape)
     for index in range(rotations.shape[0]):
         rotation = rotations[index]
         backend.fill(arr, 0)
         backend.fill(temp, 0)
         backend.rotate_array(
@@ -977,15 +935,15 @@
             out_mask=temp,
             use_geometric_center=False,
             order=interpolation_order,
         )
         # Given the amount of FFTs, might aswell normalize properly
         n_observations = backend.sum(temp)
 
-        _normalize_under_mask(
+        normalize_under_mask(
             template=arr[unpadded_slice],
             mask=temp[unpadded_slice],
             mask_intensity=n_observations,
         )
 
         rfftn(temp, ft_temp)
 
@@ -1000,40 +958,178 @@
 
         backend.subtract(temp2, temp, out=temp)
         backend.maximum(temp, 0.0, out=temp)
         backend.sqrt(temp, out=temp)
         backend.multiply(temp, n_observations, out=temp)
 
         rfftn(arr, ft_temp)
-        template_filter_func(ft_temp, template_filter, out=ft_temp)
+        template_filter_func(ft_template=ft_temp, template_filter=template_filter)
         backend.multiply(ft_target, ft_temp, out=ft_temp)
         irfftn(ft_temp, arr)
 
         tol = tol = 1e3 * eps * backend.max(backend.abs(temp))
         nonzero_indices = temp > tol
         backend.fill(temp2, 0)
         temp2[nonzero_indices] = arr[nonzero_indices] / temp[nonzero_indices]
 
-        convolution_mode = kwargs.get("convolution_mode", "full")
+        callback_func(
+            temp2,
+            rotation_matrix=rotation,
+            rotation_index=index,
+            **callback_class_args,
+        )
+
+    return callback
+
+
+def flc_scoring2(
+    template: Tuple[type, Tuple[int], type],
+    template_mask: Tuple[type, Tuple[int], type],
+    ft_target: Tuple[type, Tuple[int], type],
+    ft_target2: Tuple[type, Tuple[int], type],
+    template_filter: Tuple[type, Tuple[int], type],
+    targetshape: Tuple[int],
+    templateshape: Tuple[int],
+    fast_shape: Tuple[int],
+    fast_ft_shape: Tuple[int],
+    rotations: NDArray,
+    real_dtype: type,
+    complex_dtype: type,
+    callback_class: CallbackClass,
+    callback_class_args: Dict,
+    interpolation_order: int,
+    **kwargs,
+) -> CallbackClass:
+    """
+    Computes a normalized cross-correlation score of a target f a template g
+    and a mask m:
+
+    .. math::
+
+        \\frac{CC(f, \\frac{g*m - \\overline{g*m}}{\\sigma_{g*m}})}
+        {N_m * \\sqrt{
+            \\frac{CC(f^2, m)}{N_m} - (\\frac{CC(f, m)}{N_m})^2}
+        }
 
-        if fourier_shift_scores:
-            temp2 = backend.roll(temp2, shift=fourier_shift, axis=axis)
+    Where:
+
+    .. math::
 
-        score = apply_convolution_mode(
-            temp2, convolution_mode=convolution_mode, s1=targetshape, s2=templateshape
+        CC(f,g) = \\mathcal{F}^{-1}(\\mathcal{F}(f) \\cdot \\mathcal{F}(g)^*)
+
+    and Nm is the number of voxels within the template mask m.
+
+    References
+    ----------
+    .. [1]  W. Wan, S. Khavnekar, J. Wagner, P. Erdmann, and W. Baumeister
+            Microsc. Microanal. 26, 2516 (2020)
+    .. [2]  T. Hrabe, Y. Chen, S. Pfeffer, L. Kuhn Cuellar, A.-V. Mangold,
+            and F. Förster, J. Struct. Biol. 178, 177 (2012).
+    """
+    callback = callback_class
+    if callback_class is not None and isinstance(callback_class, type):
+        callback = callback_class(**callback_class_args)
+
+    # Retrieve objects from shared memory
+    template = backend.sharedarr_to_arr(*template)
+    template_mask = backend.sharedarr_to_arr(*template_mask)
+    ft_target = backend.sharedarr_to_arr(*ft_target)
+    ft_target2 = backend.sharedarr_to_arr(*ft_target2)
+    template_filter = backend.sharedarr_to_arr(*template_filter)
+
+    arr = backend.preallocate_array(fast_shape, real_dtype)
+    temp = backend.preallocate_array(fast_shape, real_dtype)
+    temp2 = backend.preallocate_array(fast_shape, real_dtype)
+
+    ft_temp = backend.preallocate_array(fast_ft_shape, complex_dtype)
+    ft_denom = backend.preallocate_array(fast_ft_shape, complex_dtype)
+
+    eps = backend.eps(real_dtype)
+    template_filter_func = conditional_execute(
+        apply_filter, backend.size(template_filter) != 1
+    )
+    callback_func = conditional_execute(callback, callback_class is not None)
+
+    squeeze_axis = tuple(i for i, x in enumerate(template.shape) if x == 1)
+    squeeze = tuple(
+        slice(0, stop) if i not in squeeze_axis else 0
+        for i, stop in enumerate(template.shape)
+    )
+    squeeze_fast = tuple(
+        slice(0, stop) if i not in squeeze_axis else 0
+        for i, stop in enumerate(fast_shape)
+    )
+    squeeze_fast_ft = tuple(
+        slice(0, stop) if i not in squeeze_axis else 0
+        for i, stop in enumerate(fast_ft_shape)
+    )
+
+    rfftn, irfftn = backend.build_fft(
+        fast_shape=temp[squeeze_fast].shape,
+        fast_ft_shape=fast_ft_shape,
+        real_dtype=real_dtype,
+        complex_dtype=complex_dtype,
+        fftargs=kwargs.get("fftargs", {}),
+        inverse_fast_shape=fast_shape,
+        temp_real=arr[squeeze_fast],
+        temp_fft=ft_temp,
+    )
+    for index in range(rotations.shape[0]):
+        rotation = rotations[index]
+        backend.fill(arr, 0)
+        backend.fill(temp, 0)
+        backend.rotate_array(
+            arr=template[squeeze],
+            arr_mask=template_mask[squeeze],
+            rotation_matrix=rotation,
+            out=arr[squeeze],
+            out_mask=temp[squeeze],
+            use_geometric_center=False,
+            order=interpolation_order,
         )
+        # Given the amount of FFTs, might aswell normalize properly
+        n_observations = backend.sum(temp)
 
-        if callback_class is not None:
-            callback(
-                score,
-                rotation_matrix=rotation,
-                rotation_index=index,
-                **callback_class_args,
-            )
+        normalize_under_mask(
+            template=arr[squeeze],
+            mask=temp[squeeze],
+            mask_intensity=n_observations,
+        )
+        rfftn(temp[squeeze_fast], ft_temp[squeeze_fast_ft])
 
+        backend.multiply(ft_target, ft_temp[squeeze_fast_ft], out=ft_denom)
+        irfftn(ft_denom, temp)
+        backend.divide(temp, n_observations, out=temp)
+        backend.square(temp, out=temp)
+
+        backend.multiply(ft_target2, ft_temp[squeeze_fast_ft], out=ft_denom)
+        irfftn(ft_denom, temp2)
+        backend.divide(temp2, n_observations, out=temp2)
+
+        backend.subtract(temp2, temp, out=temp)
+        backend.maximum(temp, 0.0, out=temp)
+        backend.sqrt(temp, out=temp)
+        backend.multiply(temp, n_observations, out=temp)
+
+        rfftn(arr[squeeze_fast], ft_temp[squeeze_fast_ft])
+        template_filter_func(ft_template=ft_temp, template_filter=template_filter)
+        backend.multiply(ft_target, ft_temp[squeeze_fast_ft], out=ft_denom)
+        irfftn(ft_denom, arr)
+
+        tol = tol = 1e3 * eps * backend.max(backend.abs(temp))
+        nonzero_indices = temp > tol
+        backend.fill(temp2, 0)
+        temp2[nonzero_indices] = arr[nonzero_indices] / temp[nonzero_indices]
+
+        callback_func(
+            temp2,
+            rotation_matrix=rotation,
+            rotation_index=index,
+            **callback_class_args,
+        )
     return callback
 
 
 def mcc_scoring(
     template: Tuple[type, Tuple[int], type],
     template_mask: Tuple[type, Tuple[int], type],
     ft_target: Tuple[type, Tuple[int], type],
@@ -1079,43 +1175,26 @@
     .. [1]  Masked FFT registration, Dirk Padfield, CVPR 2010 conference
     .. [2]  https://scikit-image.org/docs/stable/api/skimage.registration.html
 
     See Also
     --------
     :py:class:`tme.matching_optimization.MaskedCrossCorrelation`
     """
-    template_buffer, template_shape, template_dtype = template
-    ft_target_buffer, ft_target_shape, ft_target_dtype = ft_target
-    ft_target2_buffer, ft_target_shape, ft_target_dtype = ft_target2
-    template_mask_buffer, _, _ = template
-    ft_target_mask_buffer, _, _ = ft_target
-    filter_buffer, filter_shape, filter_dtype = template_filter
-
+    callback = callback_class
     if callback_class is not None and isinstance(callback_class, type):
         callback = callback_class(**callback_class_args)
-    elif not isinstance(callback_class, type):
-        callback = callback_class
 
     # Retrieve objects from shared memory
-    template = backend.sharedarr_to_arr(template_shape, template_dtype, template_buffer)
-    target_ft = backend.sharedarr_to_arr(
-        ft_target_shape, ft_target_dtype, ft_target_buffer
-    )
-    target_ft2 = backend.sharedarr_to_arr(
-        ft_target_shape, ft_target_dtype, ft_target2_buffer
-    )
-    template_mask = backend.sharedarr_to_arr(
-        template_shape, template_dtype, template_mask_buffer
-    )
-    target_mask_ft = backend.sharedarr_to_arr(
-        ft_target_shape, ft_target_dtype, ft_target_mask_buffer
-    )
-    template_filter = backend.sharedarr_to_arr(
-        filter_shape, filter_dtype, filter_buffer
-    )
+    template_buffer, template_shape, template_dtype = template
+    template = backend.sharedarr_to_arr(*template)
+    target_ft = backend.sharedarr_to_arr(*ft_target)
+    target_ft2 = backend.sharedarr_to_arr(*ft_target2)
+    template_mask = backend.sharedarr_to_arr(*template_mask)
+    target_mask_ft = backend.sharedarr_to_arr(*ft_target_mask)
+    template_filter = backend.sharedarr_to_arr(*template_filter)
 
     axes = tuple(range(template.ndim))
     eps = backend.eps(real_dtype)
 
     # Allocate score and process specific arrays
     template_rot = backend.preallocate_array(fast_shape, real_dtype)
     mask_overlap = backend.preallocate_array(fast_shape, real_dtype)
@@ -1132,22 +1211,18 @@
         real_dtype=real_dtype,
         complex_dtype=complex_dtype,
         fftargs=kwargs.get("fftargs", {}),
         temp_real=numerator,
         temp_fft=temp_ft,
     )
 
-    filter_template = backend.size(template_filter) != 0
-    template_filter_func = conditional_execute(backend.multiply, filter_template)
-
-    axis = tuple(range(template.ndim))
-    fourier_shift = callback_class_args.get(
-        "fourier_shift", backend.zeros(template.ndim)
+    template_filter_func = conditional_execute(
+        apply_filter, backend.size(template_filter) != 1
     )
-    fourier_shift_scores = backend.sum(fourier_shift != 0) != 0
+    callback_func = conditional_execute(callback, callback_class is not None)
 
     # Calculate scores across all rotations
     for index in range(rotations.shape[0]):
         rotation = rotations[index]
         backend.fill(template_rot, 0)
         backend.fill(temp, 0)
 
@@ -1161,15 +1236,15 @@
             order=interpolation_order,
         )
 
         backend.multiply(template_rot, temp > 0, out=template_rot)
 
         # template_rot_ft
         rfftn(template_rot, temp_ft)
-        template_filter_func(temp_ft, template_filter, out=temp_ft)
+        template_filter_func(ft_template=temp_ft, template_filter=template_filter)
         irfftn(target_mask_ft * temp_ft, temp2)
         irfftn(target_ft * temp_ft, numerator)
 
         # temp template_mask_rot | temp_ft template_mask_rot_ft
         # Calculate overlap of masks at every point in the convolution.
         # Locations with high overlap should not be taken into account.
         rfftn(temp, temp_ft)
@@ -1217,33 +1292,77 @@
         backend.clip(temp, a_min=-1, a_max=1, out=temp)
 
         # Apply overlap ratio threshold
         number_px_threshold = overlap_ratio * backend.max(
             mask_overlap, axis=axes, keepdims=True
         )
         temp[mask_overlap < number_px_threshold] = 0.0
-        convolution_mode = kwargs.get("convolution_mode", "full")
-
-        if fourier_shift_scores:
-            temp = backend.roll(temp, shift=fourier_shift, axis=axis)
 
-        score = apply_convolution_mode(
-            temp, convolution_mode=convolution_mode, s1=targetshape, s2=templateshape
+        callback_func(
+            temp,
+            rotation_matrix=rotation,
+            rotation_index=index,
+            **callback_class_args,
         )
-        if callback_class is not None:
-            callback(
-                score,
-                rotation_matrix=rotation,
-                rotation_index=index,
-                **callback_class_args,
-            )
 
     return callback
 
 
+def _setup_template_filter(
+    matching_data: MatchingData,
+    rfftn: Callable,
+    irfftn: Callable,
+    fast_shape: Tuple[int],
+    fast_ft_shape: Tuple[int],
+):
+    filter_template = isinstance(matching_data.template_filter, Compose)
+    filter_target = isinstance(matching_data.target_filter, Compose)
+
+    template_filter = backend.full(
+        shape=(1,), fill_value=1, dtype=backend._default_dtype
+    )
+
+    if not filter_template and not filter_target:
+        return template_filter
+
+    target_temp = backend.astype(
+        backend.topleft_pad(matching_data.target, fast_shape), backend._default_dtype
+    )
+    target_temp_ft = backend.preallocate_array(fast_ft_shape, backend._complex_dtype)
+    rfftn(target_temp, target_temp_ft)
+
+    if isinstance(matching_data.template_filter, Compose):
+        template_filter = matching_data.template_filter(
+            shape=fast_shape,
+            return_real_fourier=True,
+            shape_is_real_fourier=False,
+            data_rfft=target_temp_ft,
+        )
+        template_filter = template_filter["data"]
+        template_filter[tuple(0 for _ in range(template_filter.ndim))] = 0
+
+    if isinstance(matching_data.target_filter, Compose):
+        target_filter = matching_data.target_filter(
+            shape=fast_shape,
+            return_real_fourier=True,
+            shape_is_real_fourier=False,
+            data_rfft=target_temp_ft,
+            weight_type=None,
+        )
+        target_filter = target_filter["data"]
+        backend.multiply(target_temp_ft, target_filter, out=target_temp_ft)
+
+        irfftn(target_temp_ft, target_temp)
+        matching_data._target = backend.topleft_pad(
+            target_temp, matching_data.target.shape
+        )
+
+    return template_filter
+
+
 def device_memory_handler(func: Callable):
     """Decorator function providing SharedMemory Handler."""
 
     @wraps(func)
     def inner_function(*args, **kwargs):
         return_value = None
         last_type, last_value, last_traceback = sys.exc_info()
@@ -1306,38 +1425,46 @@
         Additional arguments.
 
     Returns
     -------
     Tuple
         The merged results from callback_class if provided otherwise None.
     """
+    matching_data.to_backend()
     shape_diff = backend.subtract(
-        matching_data._target.shape, matching_data._template.shape
+        matching_data._output_target_shape, matching_data._output_template_shape
     )
+    shape_diff = backend.multiply(shape_diff, ~matching_data._batch_mask)
     if backend.sum(shape_diff < 0) and not pad_fourier:
         warnings.warn(
             "Target is larger than template and Fourier padding is turned off."
             " This can lead to shifted results. You can swap template and target, or"
             " zero-pad the target."
         )
-
-    matching_data.to_backend()
-
     fast_shape, fast_ft_shape, fourier_shift = matching_data.fourier_padding(
         pad_fourier=pad_fourier
     )
 
     callback_class_args["fourier_shift"] = fourier_shift
     rfftn, irfftn = backend.build_fft(
         fast_shape=fast_shape,
         fast_ft_shape=fast_ft_shape,
         real_dtype=matching_data._default_dtype,
         complex_dtype=matching_data._complex_dtype,
         fftargs=fftargs,
     )
+
+    # template_filter = _setup_template_filter(
+    #     matching_data=matching_data,
+    #     rfftn=rfftn,
+    #     irfftn=irfftn,
+    #     fast_shape=fast_shape,
+    #     fast_ft_shape=fast_ft_shape,
+    # )
+
     setup = matching_setup(
         rfftn=rfftn,
         irfftn=irfftn,
         template=matching_data.template,
         template_mask=matching_data.template_mask,
         target=matching_data.target,
         target_mask=matching_data.target_mask,
@@ -1347,30 +1474,30 @@
         complex_dtype=matching_data._complex_dtype,
         callback_class=callback_class,
         callback_class_args=callback_class_args,
         **kwargs,
     )
     rfftn, irfftn = None, None
 
+
     template_filter, preprocessor = None, Preprocessor()
     for method, parameters in matching_data.template_filter.items():
         parameters["shape"] = fast_shape
         parameters["omit_negative_frequencies"] = True
         out = preprocessor.apply_method(method=method, parameters=parameters)
         if template_filter is None:
             template_filter = out
         np.multiply(template_filter, out, out=template_filter)
 
     if template_filter is None:
         template_filter = backend.full(
             shape=(1,), fill_value=1, dtype=backend._default_dtype
         )
-    else:
-        template_filter = backend.to_backend_array(template_filter)
 
+    template_filter = backend.to_backend_array(template_filter)
     template_filter = backend.astype(template_filter, backend._default_dtype)
     template_filter_buffer = backend.arr_to_sharedarr(
         arr=template_filter,
         shared_memory_handler=kwargs.get("shared_memory_handler", None),
     )
     setup["template_filter"] = (
         template_filter_buffer,
@@ -1384,22 +1511,29 @@
     callback_class_args["thread_safe"] = n_jobs > 1
     callback_class_args["gpu_index"] = kwargs.get("gpu_index", -1)
 
     n_callback_classes = max(n_jobs // jobs_per_callback_class, 1)
     callback_class = setup.pop("callback_class", callback_class)
     callback_class_args = setup.pop("callback_class_args", callback_class_args)
     callback_classes = [callback_class for _ in range(n_callback_classes)]
+
+    convolution_mode = "same"
+    if backend.sum(backend.to_backend_array(matching_data._target_pad)) > 0:
+        convolution_mode = "valid"
+
+
+    callback_class_args["fourier_shift"] = fourier_shift
+    callback_class_args["convolution_mode"] = convolution_mode
+    callback_class_args["targetshape"] = setup["targetshape"]
+    callback_class_args["templateshape"] = setup["templateshape"]
+
     if callback_class == MaxScoreOverRotations:
-        score_space_shape = backend.subtract(
-            matching_data.target.shape,
-            matching_data._target_pad,
-        )
         callback_classes = [
             class_name(
-                score_space_shape=score_space_shape,
+                score_space_shape=fast_shape,
                 score_space_dtype=matching_data._default_dtype,
                 shared_memory_handler=kwargs.get("shared_memory_handler", None),
                 rotation_space_dtype=backend._default_dtype_int,
                 **callback_class_args,
             )
             for class_name in callback_classes
         ]
@@ -1431,18 +1565,24 @@
             callback_class=callback_classes[index % n_callback_classes],
             callback_class_args=callback_class_args,
             **setup,
         )
         for index, rotation in enumerate(rotation_list)
     )
 
+    callbacks = callbacks[0:n_callback_classes]
     callbacks = [
-        tuple(callback)
-        for callback in callbacks[0:n_callback_classes]
-        if callback is not None
+        tuple(callback._postprocess(
+            fourier_shift = fourier_shift,
+            convolution_mode = convolution_mode,
+            targetshape = setup["targetshape"],
+            templateshape = setup["templateshape"],
+            shared_memory_handler=kwargs.get("shared_memory_handler", None)
+        )) if hasattr(callback, "_postprocess") else tuple(callback)
+        for callback in callbacks if callback is not None
     ]
     backend.free_cache()
 
     merged_callback = None
     if callback_class is not None:
         merged_callback = callback_class.merge(
             callbacks,
@@ -1545,28 +1685,31 @@
             product(target_splits, template_splits)
         )
     )
 
     matching_data._target, matching_data._template = None, None
     matching_data._target_mask, matching_data._template_mask = None, None
 
+    candidates = None
     if callback_class is not None:
         candidates = callback_class.merge(
             results, **callback_class_args, inner_merge=False
         )
-        return candidates
+
+    return candidates
 
 
 MATCHING_EXHAUSTIVE_REGISTER = {
     "CC": (cc_setup, corr_scoring),
     "LCC": (lcc_setup, corr_scoring),
     "CORR": (corr_setup, corr_scoring),
     "CAM": (cam_setup, corr_scoring),
     "FLCSphericalMask": (flcSphericalMask_setup, corr_scoring),
     "FLC": (flc_setup, flc_scoring),
+    "FLC2": (flc_setup, flc_scoring2),
     "MCC": (mcc_setup, mcc_scoring),
 }
 
 
 def register_matching_exhaustive(
     matching: str,
     matching_setup: Callable,
```

### Comparing `pytme-0.1.9/tme/matching_memory.py` & `pytme-0.2.0b0/tme/matching_memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,14 +272,15 @@
     "CC": CCMemoryUsage,
     "LCC": LCCMemoryUsage,
     "CORR": CORRMemoryUsage,
     "CAM": CAMMemoryUsage,
     "MCC": MCCMemoryUsage,
     "FLCSphericalMask": FLCSphericalMaskMemoryUsage,
     "FLC": FLCMemoryUsage,
+    "FLC2": FLCMemoryUsage,
     "MaxScoreOverRotations": MaxScoreOverRotationsMemoryUsage,
     "PeakCallerMaximumFilter": PeakCallerMaximumFilterMemoryUsage,
     "cupy": CupyBackendMemoryUsage,
     "pytorch": CupyBackendMemoryUsage,
 }
```

### Comparing `pytme-0.1.9/tme/matching_optimization.py` & `pytme-0.2.0b0/tme/matching_optimization.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,173 +11,462 @@
 
 import numpy as np
 from numpy.typing import NDArray
 from scipy.optimize import (
     differential_evolution,
     LinearConstraint,
     basinhopping,
+    minimize,
 )
-from scipy.ndimage import laplace
+from scipy.ndimage import laplace, map_coordinates
 from scipy.spatial import KDTree
 
+from .types import ArrayLike
+from .backends import backend
+from .matching_data import MatchingData
 from .matching_utils import rigid_transform, euler_to_rotationmatrix
+from .matching_exhaustive import normalize_under_mask
 
 
-class MatchCoordinatesToDensity(ABC):
+def _format_rigid_transform(x: Tuple[float]) -> Tuple[ArrayLike, ArrayLike]:
     """
-    A class to template match coordinate sets.
+    Returns a formated rigid transform definition.
 
     Parameters
     ----------
-    target_coordinates : NDArray
-        The coordinates of the target.
+    x : tuple of float
+        Even-length tuple where the first half represents translations and the
+        second half Euler angles in zyx convention for each dimension.
+
+    Returns
+    -------
+    Tuple[ArrayLike, ArrayLike]
+        Translation of length [d, ] and rotation matrix with dimension [d x d].
+    """
+    split = len(x) // 2
+    translation, angles = x[:split], x[split:]
+
+    translation = backend.to_backend_array(translation)
+    rotation_matrix = euler_to_rotationmatrix(backend.to_numpy_array(angles))
+    rotation_matrix = backend.to_backend_array(rotation_matrix)
+
+    return translation, rotation_matrix
+
+
+class _MatchDensityToDensity(ABC):
+    """
+    Parameters
+    ----------
+    target : array_like
+        The target density array.
+    template : array_like
+        The template density array.
+    template_mask : array_like, optional
+        Mask array for the template density.
+    target_mask : array_like, optional
+        Mask array for the target density.
+    pad_target_edges : bool, optional
+        Whether to pad the edges of the target density array. Default is False.
+    pad_fourier : bool, optional
+        Whether to pad the Fourier transform of the target and template densities.
+    rotate_mask : bool, optional
+        Whether to rotate the mask arrays along with the densities. Default is True.
+    interpolation_order : int, optional
+        The interpolation order for rigid transforms. Default is 1.
+    negate_score : bool, optional
+        Whether the final score should be multiplied by negative one. Default is True.
+    **kwargs : Dict, optional
+        Keyword arguments propagated to downstream functions.
+    """
+
+    def __init__(
+        self,
+        target: ArrayLike,
+        template: ArrayLike,
+        template_mask: ArrayLike = None,
+        target_mask: ArrayLike = None,
+        pad_target_edges: bool = False,
+        pad_fourier: bool = False,
+        rotate_mask: bool = True,
+        interpolation_order: int = 1,
+        negate_score: bool = True,
+        **kwargs: Dict,
+    ):
+        self.rotate_mask = rotate_mask
+        self.interpolation_order = interpolation_order
+
+        matching_data = MatchingData(target=target, template=template)
+        if template_mask is not None:
+            matching_data.template_mask = template_mask
+        if target_mask is not None:
+            matching_data.target_mask = target_mask
+
+        target_pad = matching_data.target_padding(pad_target=pad_target_edges)
+        matching_data = matching_data.subset_by_slice(target_pad=target_pad)
+
+        fast_shape, fast_ft_shape, fourier_shift = matching_data.fourier_padding(
+            pad_fourier=pad_fourier
+        )
+
+        self.target = backend.topleft_pad(matching_data.target, fast_shape)
+        self.target_mask = matching_data.target_mask
+
+        self.template = matching_data.template
+        self.template_rot = backend.preallocate_array(
+            fast_shape, backend._default_dtype
+        )
+
+        self.template_mask, self.template_mask_rot = 1, 1
+        rotate_mask = False if matching_data.template_mask is None else rotate_mask
+        if matching_data.template_mask is not None:
+            self.template_mask = matching_data.template_mask
+            self.template_mask_rot = backend.topleft_pad(
+                matching_data.template_mask, fast_shape
+            )
+
+        self.score_sign = -1 if negate_score else 1
+
+        if hasattr(self, "_post_init"):
+            self._post_init(**kwargs)
+
+    @staticmethod
+    def rigid_transform(
+        arr,
+        rotation_matrix,
+        translation,
+        arr_mask=None,
+        out=None,
+        out_mask=None,
+        order: int = 1,
+        use_geometric_center: bool = False,
+    ):
+        rotate_mask = arr_mask is not None
+        return_type = (out is None) + 2 * rotate_mask * (out_mask is None)
+        translation = np.zeros(arr.ndim) if translation is None else translation
+
+        center = np.floor(np.array(arr.shape) / 2)[:, None]
+        grid = np.indices(arr.shape, dtype=np.float32).reshape(arr.ndim, -1)
+        np.subtract(grid, center, out=grid)
+        np.matmul(rotation_matrix.T, grid, out=grid)
+        np.add(grid, center, out=grid)
+
+        if out is None:
+            out = np.zeros_like(arr)
+
+        map_coordinates(arr, grid, order=order, output=out.ravel())
+
+        if out_mask is None and arr_mask is not None:
+            out_mask = np.zeros_like(arr_mask)
+
+        if arr_mask is not None:
+            map_coordinates(arr_mask, grid, order=order, output=out_mask.ravel())
+
+        match return_type:
+            case 0:
+                return None
+            case 1:
+                return out
+            case 2:
+                return out_mask
+            case 3:
+                return out, out_mask
+
+    def score_translation(self, x: Tuple[float]) -> float:
+        """
+        Computes the score after a given translation.
+
+        Parameters
+        ----------
+        x : tuple of float
+            Tuple representing the translation transformation in each dimension.
+
+        Returns
+        -------
+        float
+            The score obtained for the translation transformation.
+        """
+        return self.score((*x, *[0 for _ in range(len(x))]))
+
+    def score_angles(self, x: Tuple[float]) -> float:
+        """
+        Computes the score after a given rotation.
+
+        Parameters
+        ----------
+        x : tuple of float
+            Tuple of Euler angles in zyx convention for each dimension.
+
+        Returns
+        -------
+        float
+            The score obtained for the rotation transformation.
+        """
+        return self.score((*[0 for _ in range(len(x))], *x))
+
+    def score(self, x: Tuple[float]) -> float:
+        """
+        Compute the matching score for the given transformation parameters.
+
+        Parameters
+        ----------
+        x : tuple of float
+            Even-length tuple where the first half represents translations and the
+            second half Euler angles in zyx convention for each dimension.
+
+        Returns
+        -------
+        float
+            The matching score obtained for the transformation.
+        """
+        translation, rotation_matrix = _format_rigid_transform(x)
+        kw_dict = {
+            "arr": self.template,
+            "rotation_matrix": rotation_matrix,
+            "translation": translation,
+            "out": self.template_rot,
+            "use_geometric_center": False,
+            "order": self.interpolation_order,
+        }
+        if self.rotate_mask:
+            kw_dict["arr_mask"] = self.template_mask
+            kw_dict["out_mask"] = self.template_mask_rot
+
+        self.rigid_transform(**kw_dict)
+
+        return self()
+
+    @abstractmethod
+    def __call__(self) -> float:
+        """Returns the score of the current configuration."""
+
+
+class _MatchCoordinatesToDensity(_MatchDensityToDensity):
+    """
+    Parameters
+    ----------
+    target : NDArray
+        A d-dimensional target to match the template coordinate set to.
     template_coordinates : NDArray
-        The coordinates of the template.
-    target_weights : NDArray
-        The weights of the target.
+        Template coordinate array with shape [d x N].
     template_weights : NDArray
-        The weights of the template.
-    sampling_rate : NDArray
-        The size of the voxel.
+        Template weight array with shape [N].
     template_mask_coordinates : NDArray, optional
-        The coordinates of the template mask. Default is None.
-    target_mask_coordinates : NDArray, optional
-        The coordinates of the target mask. Default is None.
-    **kwargs : dict, optional
-        Other keyword arguments.
+        Template mask coordinates with shape [d x N].
+    target_mask : NDArray, optional
+        A d-dimensional mask to be applied to the target.
+    negate_score : bool, optional
+        Whether the final score should be multiplied by negative one. Default is True.
+    **kwargs : Dict, optional
+        Keyword arguments propagated to downstream functions.
     """
 
     def __init__(
         self,
-        target_coordinates: NDArray,
+        target: NDArray,
         template_coordinates: NDArray,
-        target_weights: NDArray,
         template_weights: NDArray,
-        sampling_rate: NDArray,
         template_mask_coordinates: NDArray = None,
-        target_mask_coordinates: NDArray = None,
-        **kwargs,
+        target_mask: NDArray = None,
+        negate_score: bool = True,
+        **kwargs: Dict,
     ):
-        target, _, origin = FitRefinement.array_from_coordinates(
-            target_coordinates, target_weights, sampling_rate
-        )
         self.target_density = target
-        self.target_origin = origin
-        self.sampling_rate = sampling_rate
+        self.target_mask_density = target_mask
 
         self.template_weights = template_weights
         self.template_coordinates = template_coordinates
-        self.template_coordinates_rotated = np.empty(
-            self.template_coordinates.shape, dtype=np.float32
+        self.template_coordinates_rotated = np.copy(self.template_coordinates).astype(
+            np.float32
         )
 
-        self.target_mask_density = None
-        if target_mask_coordinates is not None:
-            target_mask, *_ = FitRefinement.array_from_coordinates(
-                coordinates=target_mask_coordinates.astype(np.float32),
-                weights=np.ones(target_mask_coordinates.shape[1]),
-                shape=self.target_density.shape,
-                origin=self.target_origin,
-                sampling_rate=self.sampling_rate,
-            )
-            self.target_mask_density = target_mask
-
-        self.template_mask_coordinates = None
-        self.template_mask_coordinates_rotated = None
+        self.template_mask_coordinates = template_mask_coordinates
+        self.template_mask_coordinates_rotated = template_mask_coordinates
         if template_mask_coordinates is not None:
-            self.template_mask_coordinates = template_mask_coordinates
-            self.template_mask_coordinates_rotated = np.empty(
-                self.template_mask_coordinates.shape, dtype=np.float32
-            )
+            self.template_mask_coordinates_rotated = np.copy(
+                self.template_mask_coordinates
+            ).astype(np.float32)
+
+        self.denominator = 1
+        self.score_sign = -1 if negate_score else 1
+
+        self.in_volume, self.in_volume_mask = self.map_coordinates_to_array(
+            coordinates=self.template_coordinates_rotated,
+            coordinates_mask=self.template_mask_coordinates_rotated,
+            array_origin=backend.zeros(target.ndim),
+            array_shape=self.target_density.shape,
+            sampling_rate=backend.full(target.ndim, fill_value=1),
+        )
 
-    def __call__(self, x: NDArray):
+        if hasattr(self, "_post_init"):
+            self._post_init(**kwargs)
+
+    def score(self, x: Tuple[float]):
         """
-        Return the score for a given transformation.
+        Compute the matching score for the given transformation parameters.
 
         Parameters
         ----------
-        x : NDArray
-            The input transformation parameters.
+        x : tuple of float
+            Even-length tuple where the first half represents translations and the
+            second half Euler angles in zyx convention for each dimension.
 
         Returns
         -------
         float
-            The negative score from the scoring function.
+            The matching score obtained for the transformation.
         """
-        translation, rotation = x[:3], x[3:]
-        rotation_matrix = euler_to_rotationmatrix(rotation)
+        translation, rotation_matrix = _format_rigid_transform(x)
 
         rigid_transform(
             coordinates=self.template_coordinates,
             coordinates_mask=self.template_mask_coordinates,
             rotation_matrix=rotation_matrix,
             translation=translation,
             out=self.template_coordinates_rotated,
             out_mask=self.template_mask_coordinates_rotated,
             use_geometric_center=False,
         )
 
-        mapping = FitRefinement.map_coordinates_to_array(
+        self.in_volume, self.in_volume_mask = self.map_coordinates_to_array(
             coordinates=self.template_coordinates_rotated,
             coordinates_mask=self.template_mask_coordinates_rotated,
-            array_origin=self.target_origin,
+            array_origin=backend.zeros(rotation_matrix.shape[0]),
             array_shape=self.target_density.shape,
-            sampling_rate=self.sampling_rate,
+            sampling_rate=backend.full(rotation_matrix.shape[0], fill_value=1),
         )
 
-        return -self.scoring_function(
-            transformed_coordinates=mapping[0],
-            transformed_coordinates_mask=mapping[1],
-            in_volume=mapping[2],
-            in_volume_mask=mapping[3],
-        )
+        return self()
 
-    @abstractmethod
-    def scoring_function(*args, **kwargs):
+    @staticmethod
+    def array_from_coordinates(
+        coordinates: NDArray,
+        weights: NDArray,
+        sampling_rate: NDArray,
+        origin: NDArray = None,
+        shape: NDArray = None,
+    ) -> Tuple[NDArray, NDArray, NDArray]:
         """
-        Computes a scoring metric for a given set of coordinates.
+        Create a volume from coordinates, using given weights and voxel size.
+
+        Parameters
+        ----------
+        coordinates : NDArray
+            An array representing the coordinates [d x N].
+        weights : NDArray
+            An array representing the weights for each coordinate [N].
+        sampling_rate : NDArray
+            The size of a voxel in the volume.
+        origin : NDArray, optional
+            The origin of the volume.
+        shape : NDArray, optional
+            The shape of the volume.
 
-        This function is not intended to be called directly, but should rather be
-        defined by classes inheriting from :py:class:`MatchCoordinatesToDensity`
-        to parse a given file format.
+        Returns
+        -------
+        tuple
+            Returns the generated volume, positions of coordinates, and origin.
         """
+        if origin is None:
+            origin = coordinates.min(axis=1)
 
+        positions = np.divide(coordinates - origin[:, None], sampling_rate[:, None])
+        positions = positions.astype(int)
 
-class MatchCoordinatesToCoordinates(ABC):
-    """
-    A class to template match coordinate sets.
+        if shape is None:
+            shape = positions.max(axis=1) + 1
+
+        arr = np.zeros(shape, dtype=np.float32)
+        np.add.at(arr, tuple(positions), weights)
+        return arr, positions, origin
+
+    @staticmethod
+    def map_coordinates_to_array(
+        coordinates: NDArray,
+        array_shape: NDArray,
+        array_origin: NDArray,
+        sampling_rate: NDArray,
+        coordinates_mask: NDArray = None,
+    ) -> Tuple[NDArray, NDArray]:
+        """
+        Map coordinates to a volume based on given voxel size and origin.
+
+        Parameters
+        ----------
+        coordinates : NDArray
+            An array representing the coordinates to be mapped [d x N].
+        array_shape : NDArray
+            The shape of the array to which the coordinates are mapped.
+        array_origin : NDArray
+            The origin of the array to which the coordinates are mapped.
+        sampling_rate : NDArray
+            The size of a voxel in the array.
+        coordinates_mask : NDArray, optional
+            An array representing the mask for the coordinates [d x T].
+
+        Returns
+        -------
+        tuple
+            Returns transformed coordinates, transformed coordinates mask,
+            mask for in_volume points, and mask for in_volume points in mask.
+        """
+        np.divide(
+            coordinates - array_origin[:, None], sampling_rate[:, None], out=coordinates
+        )
+
+        in_volume = np.logical_and(
+            coordinates < np.array(array_shape)[:, None],
+            coordinates >= 0,
+        ).min(axis=0)
+
+        in_volume_mask = None
+        if coordinates_mask is not None:
+            np.divide(
+                coordinates_mask - array_origin[:, None],
+                sampling_rate[:, None],
+                out=coordinates_mask,
+            )
+            in_volume_mask = np.logical_and(
+                coordinates_mask < np.array(array_shape)[:, None],
+                coordinates_mask >= 0,
+            ).min(axis=0)
 
+        return in_volume, in_volume_mask
+
+
+class _MatchCoordinatesToCoordinates(_MatchDensityToDensity):
+    """
     Parameters
     ----------
     target_coordinates : NDArray
-        The coordinates of the target.
+        The coordinates of the target with shape [d x N].
     template_coordinates : NDArray
-        The coordinates of the template.
+        The coordinates of the template with shape [d x T].
     target_weights : NDArray
-        The weights of the target.
+        The weights of the target with shape [N].
     template_weights : NDArray
-        The weights of the template.
-    sampling_rate : NDArray
-        The size of the voxel.
+        The weights of the template with shape [T].
     template_mask_coordinates : NDArray, optional
-        The coordinates of the template mask. Default is None.
+        The coordinates of the template mask with shape [d x T]. Default is None.
     target_mask_coordinates : NDArray, optional
-        The coordinates of the target mask. Default is None.
-    **kwargs : dict, optional
-        Other keyword arguments.
+        The coordinates of the target mask with shape [d X N]. Default is None.
+    negate_score : bool, optional
+        Whether the final score should be multiplied by negative one. Default is True.
+    **kwargs : Dict, optional
+        Keyword arguments propagated to downstream functions.
     """
 
     def __init__(
         self,
         target_coordinates: NDArray,
         template_coordinates: NDArray,
         target_weights: NDArray,
         template_weights: NDArray,
         template_mask_coordinates: NDArray = None,
         target_mask_coordinates: NDArray = None,
+        negate_score: bool = True,
         **kwargs,
     ):
         self.target_weights = target_weights
         self.target_coordinates = target_coordinates
 
         self.template_weights = template_weights
         self.template_coordinates = template_coordinates
@@ -189,142 +478,174 @@
         self.template_mask_coordinates = None
         self.template_mask_coordinates_rotated = None
         if template_mask_coordinates is not None:
             self.template_mask_coordinates = template_mask_coordinates
             self.template_mask_coordinates_rotated = np.empty(
                 self.template_mask_coordinates.shape, dtype=np.float32
             )
+        self.score_sign = -1 if negate_score else 1
+
+        if hasattr(self, "_post_init"):
+            self._post_init(**kwargs)
 
-    def __call__(self, x: NDArray):
+    def score(self, x: Tuple[float]) -> float:
         """
-        Return the score for a given transformation.
+        Compute the matching score for the given transformation parameters.
 
         Parameters
         ----------
-        x : NDArray
-            The input transformation parameters.
+        x : tuple of float
+            Even-length tuple where the first half represents translations and the
+            second half Euler angles in zyx convention for each dimension.
 
         Returns
         -------
         float
-            The negative score from the scoring function.
+            The matching score obtained for the transformation.
         """
-        translation, rotation = x[:3], x[3:]
-        rotation_matrix = euler_to_rotationmatrix(rotation)
+        translation, rotation_matrix = _format_rigid_transform(x)
 
         rigid_transform(
             coordinates=self.template_coordinates,
             coordinates_mask=self.template_mask_coordinates,
             rotation_matrix=rotation_matrix,
             translation=translation,
             out=self.template_coordinates_rotated,
             out_mask=self.template_mask_coordinates_rotated,
             use_geometric_center=False,
         )
 
-        return -self.scoring_function(
+        return self(
             transformed_coordinates=self.template_coordinates_rotated,
             transformed_coordinates_mask=self.template_mask_coordinates_rotated,
         )
 
-    @abstractmethod
-    def scoring_function(*args, **kwargs):
-        """
-        Computes a scoring metric for a given set of coordinates.
 
-        This function is not intended to be called directly, but should rather be
-        defined by classes inheriting from :py:class:`MatchCoordinatesToDensity`
-        to parse a given file format.
-        """
+class FLC(_MatchDensityToDensity):
+    __doc__ += _MatchDensityToDensity.__doc__
 
+    def _post_init(self, **kwargs: Dict):
+        if self.target_mask is not None:
+            backend.multiply(self.target, self.target_mask, out=self.target)
 
-class CrossCorrelation(MatchCoordinatesToDensity):
-    """
-    Class representing the Cross-Correlation matching score.
+        self.target_square = backend.square(self.target)
 
-    Cross-Correlation score formula:
+        normalize_under_mask(
+            template=self.template,
+            mask=self.template_mask,
+            mask_intensity=backend.sum(self.template_mask),
+        )
 
-    .. math::
+        self.template = backend.reverse(self.template)
+        self.template_mask = backend.reverse(self.template_mask)
 
-        \\text{score} = \\text{target_weights} \\cdot \\text{template_weights}
+    def __call__(self) -> float:
+        """Returns the score of the current configuration."""
+        n_observations = backend.sum(self.template_mask_rot)
+
+        normalize_under_mask(
+            template=self.template_rot,
+            mask=self.template_mask_rot,
+            mask_intensity=n_observations,
+        )
+
+        ex2 = backend.sum(
+            backend.divide(
+                backend.sum(
+                    backend.multiply(self.target_square, self.template_mask_rot),
+                ),
+                n_observations,
+            )
+        )
+        e2x = backend.square(
+            backend.divide(
+                backend.sum(backend.multiply(self.target, self.template_mask_rot)),
+                n_observations,
+            )
+        )
+
+        denominator = backend.maximum(backend.subtract(ex2, e2x), 0.0)
+        denominator = backend.sqrt(denominator)
+        denominator = backend.multiply(denominator, n_observations)
+
+        overlap = backend.sum(backend.multiply(self.template_rot, self.target))
 
+        score = backend.divide(overlap, denominator) * self.score_sign
+        return score
+
+
+class CrossCorrelation(_MatchCoordinatesToDensity):
     """
+    Computes the Cross-Correlation score as:
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.denominator = 1
+    .. math::
 
-    def scoring_function(
-        self,
-        transformed_coordinates: NDArray,
-        transformed_coordinates_mask: NDArray,
-        in_volume: NDArray,
-        in_volume_mask: NDArray,
-    ) -> float:
-        """
-        Compute the Cross-Correlation score.
+        \\text{score} = \\text{target_weights} \\cdot \\text{template_weights}
+    """
 
-        Parameters
-        ----------
-        transformed_coordinates : NDArray
-            Transformed coordinates.
-        transformed_coordinates_mask : NDArray
-            Mask for the transformed coordinates.
-        in_volume : NDArray
-            Binary mask indicating which ``transformed_coordinates`` are in the
-            target volume.
-        in_volume_mask : NDArray
-            Binary mask indicating which ``transformed_coordinates`` are in the
-            target mask volume.
+    __doc__ += _MatchCoordinatesToDensity.__doc__
 
-        Returns
-        -------
-        float
-            The Cross-Correlation score.
-        """
-        score = np.dot(
-            self.target_density[tuple(transformed_coordinates[:, in_volume])],
-            self.template_weights[in_volume],
-        )
+    def __call__(self) -> float:
+        """Returns the score of the current configuration."""
+        try:
+            score = np.dot(
+                self.target_density[
+                    tuple(
+                        self.template_coordinates_rotated[:, self.in_volume].astype(int)
+                    )
+                ],
+                self.template_weights[self.in_volume],
+            )
+        except:
+            print(self.template_coordinates_rotated[:, self.in_volume].astype(int))
+            print(self.target_density.shape)
+            print(self.in_volume)
+            coordinates = self.template_coordinates_rotated[:, self.in_volume].astype(
+                int
+            )
+            in_volume = np.logical_and(
+                coordinates < np.array(self.target_density.shape)[:, None],
+                coordinates >= 0,
+            ).min(axis=0)
+            print(in_volume)
+
+            raise ValueError()
         score /= self.denominator
-        return score
+        return score * self.score_sign
 
 
 class LaplaceCrossCorrelation(CrossCorrelation):
     """
-    Class representing the Laplace Cross-Correlation matching score.
-
-    The score is computed like CrossCorrelation, but with Laplace filtered
-    weights, indicated by the Laplace operator :math:`\\nabla^{2}`.
+    Uses the same formalism as :py:class:`CrossCorrelation` but with Laplace
+    filtered weights (:math:`\\nabla^{2}`):
 
     .. math::
 
         \\text{score} = \\nabla^{2} \\text{target_weights} \\cdot
                         \\nabla^{2} \\text{template_weights}
-
     """
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+    __doc__ += _MatchCoordinatesToDensity.__doc__
+
+    def _post_init(self, **kwargs):
         self.target_density = laplace(self.target_density)
 
-        arr, positions, _ = FitRefinement.array_from_coordinates(
-            self.template_coordinates, self.template_weights, self.sampling_rate
+        arr, positions, _ = self.array_from_coordinates(
+            self.template_coordinates,
+            self.template_weights,
+            np.ones(self.template_coordinates.shape[0]),
         )
         self.template_weights = laplace(arr)[tuple(positions)]
 
 
 class NormalizedCrossCorrelation(CrossCorrelation):
     """
-    Class representing the Normalized Cross-Correlation matching score.
-
-    The score is computed by normalizing the dot product of `target_weights` and
-    `template_weights` with the product of their norms. This normalization ensures
-    the score lies between -1 and 1, providing a measure of similarity that's invariant
-    to scale.
+    Computes a normalized version of the :py:class:`CrossCorrelation` score based
+    on the dot product of `target_weights` and `template_weights`, in order to
+    reduce bias to regions of high local energy.
 
     .. math::
 
         \\text{score} = \\frac{\\text{target_weights} \\cdot \\text{template_weights}}
                         {\\text{max(target_norm} \\times \\text{template_norm, eps)}}
 
     Where:
@@ -334,34 +655,28 @@
         \\text{target_norm} = ||\\text{target_weights}||
 
     .. math::
 
         \\text{template_norm} = ||\\text{template_weights}||
 
     Here, :math:`||.||` denotes the L2 (Euclidean) norm.
-
     """
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+    __doc__ += _MatchCoordinatesToDensity.__doc__
+
+    def _post_init(self, **kwargs):
         target_norm = np.linalg.norm(self.target_density[self.target_density != 0])
         template_norm = np.linalg.norm(self.template_weights)
         self.denominator = np.fmax(target_norm * template_norm, np.finfo(float).eps)
 
 
 class NormalizedCrossCorrelationMean(NormalizedCrossCorrelation):
     """
-    Class representing the Mean Normalized Cross-Correlation matching score.
-
-    This class extends the Normalized Cross-Correlation by computing the score
-    after subtracting the mean from both `target_weights` and `template_weights`.
-    This modification enhances the matching score's sensitivity to patterns
-    over flat regions in the data.
-
-    Mathematically, the Mean Normalized Cross-Correlation score is computed as:
+    Computes a similar score than :py:class:`NormalizedCrossCorrelation`, but
+    additionally factors in the mean of template and target.
 
     .. math::
 
         \\text{score} = \\frac{(\\text{target_weights} - \\text{mean(target_weights)})
                         \\cdot (\\text{template_weights} -
                         \\text{mean(template_weights)})}
                         {\\text{max(target_norm} \\times \\text{template_norm, eps)}}
@@ -377,29 +692,29 @@
         \\text{template_norm} = ||\\text{template_weights} -
         \\text{mean(template_weights)}||
 
     Here, :math:`||.||` denotes the L2 (Euclidean) norm, and :math:`\\text{mean(.)}`
     computes the mean of the respective weights.
     """
 
+    __doc__ += _MatchCoordinatesToDensity.__doc__
+
     def __init__(self, **kwargs):
-        print(kwargs["target_weights"].mean())
-        kwargs["target_weights"] -= kwargs["target_weights"].mean()
-        kwargs["template_weights"] -= kwargs["template_weights"].mean()
+        kwargs["target"] = np.subtract(kwargs["target"], kwargs["target"].mean())
+        kwargs["template_weights"] = np.subtract(
+            kwargs["template_weights"], kwargs["template_weights"].mean()
+        )
         super().__init__(**kwargs)
 
 
-class MaskedCrossCorrelation(MatchCoordinatesToDensity):
+class MaskedCrossCorrelation(_MatchCoordinatesToDensity):
     """
-    Class representing the Masked Cross-Correlation matching score.
-
     The Masked Cross-Correlation computes the similarity between `target_weights`
-    and `template_weights` under respective masks. The score is normalized and lies
-    between -1 and 1, providing a measure of similarity even in the presence of
-    missing or masked data.
+    and `template_weights` under respective masks. The score provides a measure of
+    similarity even in the presence of missing or masked data.
 
     The formula for the Masked Cross-Correlation is:
 
     .. math::
         \\text{numerator} = \\text{dot}(\\text{target_weights},
                             \\text{template_weights}) -
                             \\frac{\\text{sum}(\\text{mask_target}) \\times
@@ -433,343 +748,225 @@
         the masks.
 
     References
     ----------
     .. [1]  Masked FFT registration, Dirk Padfield, CVPR 2010 conference
     """
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-
-    def scoring_function(
-        self,
-        transformed_coordinates: NDArray,
-        transformed_coordinates_mask: NDArray,
-        in_volume: NDArray,
-        in_volume_mask: NDArray,
-    ) -> float:
-        """
-        Compute the Masked Cross-Correlation score.
-
-        Parameters
-        ----------
-        transformed_coordinates : NDArray
-            Transformed coordinates.
-        transformed_coordinates_mask : NDArray
-            Mask for the transformed coordinates.
-        in_volume : NDArray
-            Binary mask indicating which ``transformed_coordinates`` are in the
-            target volume.
-        in_volume_mask : NDArray
-            Binary mask indicating which ``transformed_coordinates`` are in the
-            target mask volume.
+    __doc__ += _MatchCoordinatesToDensity.__doc__
 
-        Returns
-        -------
-        float
-            The Masked Cross-Correlation score.
-        """
+    def __call__(self) -> float:
+        """Returns the score of the current configuration."""
         mask_overlap = np.sum(
             self.target_mask_density[
-                tuple(transformed_coordinates_mask[:, in_volume_mask])
+                tuple(
+                    self.template_mask_coordinates_rotated[
+                        :, self.in_volume_mask
+                    ].astype(int)
+                )
             ],
         )
         mask_overlap = np.fmax(mask_overlap, np.finfo(float).eps)
 
         mask_target = self.target_density[
-            tuple(transformed_coordinates_mask[:, in_volume_mask])
+            tuple(
+                self.template_mask_coordinates_rotated[:, self.in_volume_mask].astype(
+                    int
+                )
+            )
         ]
         denominator1 = np.subtract(
             np.sum(mask_target**2),
             np.divide(np.square(np.sum(mask_target)), mask_overlap),
         )
         mask_template = np.multiply(
-            self.template_weights[in_volume],
-            self.target_mask_density[tuple(transformed_coordinates[:, in_volume])],
+            self.template_weights[self.in_volume],
+            self.target_mask_density[
+                tuple(self.template_coordinates_rotated[:, self.in_volume].astype(int))
+            ],
         )
         denominator2 = np.subtract(
             np.sum(mask_template**2),
             np.divide(np.square(np.sum(mask_template)), mask_overlap),
         )
 
         denominator1 = np.fmax(denominator1, 0.0)
         denominator2 = np.fmax(denominator2, 0.0)
         denominator = np.sqrt(np.multiply(denominator1, denominator2))
 
         numerator = np.dot(
-            self.target_density[tuple(transformed_coordinates[:, in_volume])],
-            self.template_weights[in_volume],
+            self.target_density[
+                tuple(self.template_coordinates_rotated[:, self.in_volume].astype(int))
+            ],
+            self.template_weights[self.in_volume],
         )
 
         numerator -= np.divide(
             np.multiply(np.sum(mask_target), np.sum(mask_template)), mask_overlap
         )
 
         if denominator == 0:
-            return 0
+            return 0.0
 
         score = numerator / denominator
-        return score
+        return float(score * self.score_sign)
 
 
-class PartialLeastSquareDifference(MatchCoordinatesToDensity):
+class PartialLeastSquareDifference(_MatchCoordinatesToDensity):
     """
-    Class representing the Partial Least Square Difference matching score.
-
     The Partial Least Square Difference (PLSQ) between the target :math:`f` and the
     template :math:`g` is calculated as:
 
     .. math::
 
         \\text{d(f,g)} = \\sum_{i=1}^{n} \\| f(\\mathbf{p}_i) - g(\\mathbf{q}_i) \\|^2
 
     References
     ----------
     .. [1]  Daven Vasishtan and Maya Topf, "Scoring functions for cryoEM density
             fitting", Journal of Structural Biology, vol. 174, no. 2,
             pp. 333--343, 2011. DOI: https://doi.org/10.1016/j.jsb.2011.01.012
     """
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-
-    def scoring_function(
-        self,
-        transformed_coordinates: NDArray,
-        transformed_coordinates_mask: NDArray,
-        in_volume: NDArray,
-        in_volume_mask: NDArray,
-    ) -> float:
-        """
-        Compute the Partial Least Square Difference score.
-
-        Given the transformed coordinates and their associated mask, this function
-        computes the difference between target and template densities.
+    __doc__ += _MatchCoordinatesToDensity.__doc__
 
-        Parameters
-        ----------
-        transformed_coordinates : NDArray
-            Transformed coordinates.
-        transformed_coordinates_mask : NDArray
-            Mask for the transformed coordinates.
-        in_volume : NDArray
-            Binary mask indicating which ``transformed_coordinates`` are in the
-            target volume.
-        in_volume_mask : NDArray
-            Binary mask indicating which ``transformed_coordinates`` are in the
-            target mask volume.
-
-        Returns
-        -------
-        float
-            The negative of the Partial Least Square Difference score.
-        """
+    def __call__(self) -> float:
+        """Returns the score of the current configuration."""
         score = np.sum(
             np.square(
                 np.subtract(
-                    self.target_density[tuple(transformed_coordinates[:, in_volume])],
-                    self.template_weights[in_volume],
+                    self.target_density[
+                        tuple(
+                            self.template_coordinates_rotated[:, self.in_volume].astype(
+                                int
+                            )
+                        )
+                    ],
+                    self.template_weights[self.in_volume],
                 )
             )
         )
-        score += np.sum(np.square(self.template_weights[np.invert(in_volume)]))
-
-        return -score
-
-
-class Chamfer(MatchCoordinatesToCoordinates):
-    """
-    Class representing the Chamfer matching score.
-
-    The Chamfer distance is computed as:
-
-    .. math::
-
-        \\text{d(f,g)} = \\frac{1}{|X|} \\sum_{\\mathbf{f}_i \\in X}
-        \\inf_{\\mathbf{g} \\in Y} ||\\mathbf{f}_i - \\mathbf{g}||_2
-
-    References
-    ----------
-    .. [1]  Daven Vasishtan and Maya Topf, "Scoring functions for cryoEM density
-            fitting", Journal of Structural Biology, vol. 174, no. 2,
-            pp. 333--343, 2011. DOI: https://doi.org/10.1016/j.jsb.2011.01.012
-    """
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.target_tree = KDTree(self.target_coordinates.T)
-
-    def scoring_function(
-        self,
-        transformed_coordinates: NDArray,
-        transformed_coordinates_mask: NDArray,
-        **kwargs,
-    ) -> float:
-        """
-        Compute the Chamfer distance score.
-
-        Given the transformed coordinates and their associated mask, this function
-        calculates the average distance between the rotated template coordinates
-        and the nearest target coordinates.
-
-        Parameters
-        ----------
-        transformed_coordinates : NDArray
-            Transformed coordinates.
-
-        Returns
-        -------
-        float
-            The negative of the Chamfer distance score.
-
-        """
-        dist, _ = self.target_tree.query(self.template_coordinates_rotated.T)
-        score = np.mean(dist)
-        return -score
+        score += np.sum(np.square(self.template_weights[np.invert(self.in_volume)]))
+        return score * self.score_sign
 
 
-class MutualInformation(MatchCoordinatesToDensity):
+class MutualInformation(_MatchCoordinatesToDensity):
     """
-    Class representing the Mutual Information matching score.
-
-    The Mutual Information (MI) score is calculated as:
+    The Mutual Information (MI) score between the target :math:`f` and the
+    template :math:`g` is calculated as:
 
     .. math::
 
         \\text{d(f,g)} = \\sum_{f,g} p(f,g) \\log \\frac{p(f,g)}{p(f)p(g)}
 
     References
     ----------
     .. [1]  Daven Vasishtan and Maya Topf, "Scoring functions for cryoEM density
             fitting", Journal of Structural Biology, vol. 174, no. 2,
             pp. 333--343, 2011. DOI: https://doi.org/10.1016/j.jsb.2011.01.012
 
     """
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-
-    def scoring_function(
-        self,
-        transformed_coordinates: NDArray,
-        transformed_coordinates_mask: NDArray,
-        in_volume: NDArray,
-        in_volume_mask: NDArray,
-    ) -> float:
-        """
-        Compute the Mutual Information score.
-
-        Given the transformed coordinates and their associated mask, this function
-        computes the mutual information between the target and template densities.
+    __doc__ += _MatchCoordinatesToDensity.__doc__
 
-        Parameters
-        ----------
-        transformed_coordinates : NDArray
-            Transformed coordinates.
-        transformed_coordinates_mask : NDArray
-            Mask for the transformed coordinates.
-        in_volume : NDArray
-            Binary mask indicating which ``transformed_coordinates`` are in the
-            target volume.
-        in_volume_mask : NDArray
-            Binary mask indicating which ``transformed_coordinates`` are in the
-            target mask volume.
-
-        Returns
-        -------
-        float
-            The Mutual Information score.
-        """
+    def __call__(self) -> float:
+        """Returns the score of the current configuration."""
         p_xy, target, template = np.histogram2d(
-            self.target_density[tuple(transformed_coordinates[:, in_volume])],
-            self.template_weights[in_volume],
+            self.target_density[
+                tuple(self.template_coordinates_rotated[:, self.in_volume].astype(int))
+            ],
+            self.template_weights[self.in_volume],
         )
         p_x, p_y = np.sum(p_xy, axis=1), np.sum(p_xy, axis=0)
 
         p_xy /= p_xy.sum()
         p_x /= p_x.sum()
         p_y /= p_y.sum()
 
         logprob = np.divide(p_xy, p_x[:, None] * p_y[None, :] + np.finfo(float).eps)
         score = np.nansum(p_xy * logprob)
 
-        return score
+        return score * self.score_sign
 
 
-class Envelope(MatchCoordinatesToDensity):
+class Envelope(_MatchCoordinatesToDensity):
     """
-    Class representing the Envelope matching score.
-
-    The Envelope score (ENV) is calculated as:
+    The Envelope score (ENV) between the target :math:`f` and the
+    template :math:`g` is calculated as:
 
     .. math::
 
         \\text{d(f,g)} =    \\sum_{\\mathbf{p} \\in P} f'(\\mathbf{p})
                             \\cdot g'(\\mathbf{p})
 
     References
     ----------
     .. [1]  Daven Vasishtan and Maya Topf, "Scoring functions for cryoEM density
             fitting", Journal of Structural Biology, vol. 174, no. 2,
             pp. 333--343, 2011. DOI: https://doi.org/10.1016/j.jsb.2011.01.012
     """
 
-    def __init__(self, target_threshold: float, **kwargs):
+    __doc__ += _MatchCoordinatesToDensity.__doc__
+
+    def __init__(self, target_threshold: float = None, **kwargs):
         super().__init__(**kwargs)
+        if target_threshold is None:
+            target_threshold = np.mean(self.target_density)
         self.target_density = np.where(self.target_density > target_threshold, -1, 1)
         self.target_density_present = np.sum(self.target_density == -1)
         self.target_density_absent = np.sum(self.target_density == 1)
         self.template_weights = np.ones_like(self.template_weights)
 
-    def scoring_function(
-        self,
-        transformed_coordinates: NDArray,
-        transformed_coordinates_mask: NDArray,
-        in_volume: NDArray,
-        in_volume_mask: NDArray,
-    ) -> float:
-        """
-        Compute the Envelope score.
-
-        Given the transformed coordinates and their associated mask, this function
-        computes the envelope score based on target density thresholds.
-
-        Parameters
-        ----------
-        transformed_coordinates : NDArray
-            Transformed coordinates.
-        transformed_coordinates_mask : NDArray
-            Mask for the transformed coordinates.
-        in_volume : NDArray
-            Binary mask indicating which ``transformed_coordinates`` are in the
-            target volume.
-        in_volume_mask : NDArray
-            Binary mask indicating which ``transformed_coordinates`` are in the
-            target mask volume.
-
-        Returns
-        -------
-        float
-            The Envelope score.
-        """
-        score = self.target_density[tuple(transformed_coordinates[:, in_volume])]
+    def __call__(self) -> float:
+        """Returns the score of the current configuration."""
+        score = self.target_density[
+            tuple(self.template_coordinates_rotated[:, self.in_volume].astype(int))
+        ]
         unassigned_density = self.target_density_present - (score == -1).sum()
 
-        score = score.sum() - unassigned_density - 2 * np.sum(np.invert(in_volume))
+        score = score.sum() - unassigned_density - 2 * np.sum(np.invert(self.in_volume))
         min_score = -self.target_density_present - 2 * self.target_density_absent
         score = (score - 2 * min_score) / (2 * self.target_density_present - min_score)
 
-        return score
+        return score * self.score_sign
+
+
+class Chamfer(_MatchCoordinatesToCoordinates):
+    """
+    The Chamfer distance between the target :math:`f` and the template :math:`g`
+    is calculated as:
 
+    .. math::
+
+        \\text{d(f,g)} = \\frac{1}{|X|} \\sum_{\\mathbf{f}_i \\in X}
+        \\inf_{\\mathbf{g} \\in Y} ||\\mathbf{f}_i - \\mathbf{g}||_2
 
-class NormalVectorScore(MatchCoordinatesToCoordinates):
+    References
+    ----------
+    .. [1]  Daven Vasishtan and Maya Topf, "Scoring functions for cryoEM density
+            fitting", Journal of Structural Biology, vol. 174, no. 2,
+            pp. 333--343, 2011. DOI: https://doi.org/10.1016/j.jsb.2011.01.012
     """
-    Class representing the Normal Vector matching score.
 
-    The Normal Vector Score (NVS) is calculated as:
+    __doc__ += _MatchCoordinatesToDensity.__doc__
+
+    def _post_init(self, **kwargs):
+        self.target_tree = KDTree(self.target_coordinates.T)
+
+    def __call__(self) -> float:
+        """Returns the score of the current configuration."""
+        dist, _ = self.target_tree.query(self.template_coordinates_rotated.T)
+        score = np.mean(dist)
+        return score * self.score_sign
+
+
+class NormalVectorScore(_MatchCoordinatesToCoordinates):
+    """
+    The Normal Vector Score (NVS) between the target's :math:`f` and the template
+    :math:`g`'s normal vectors is calculated as:
 
     .. math::
 
         \\text{d(f,g)} = \\frac{1}{N} \\sum_{i=1}^{N}
         \\frac{
             {\\vec{f}_i} \\cdot {\\vec{g}_i}
         }{
@@ -780,43 +977,22 @@
     ----------
     .. [1]  Daven Vasishtan and Maya Topf, "Scoring functions for cryoEM density
             fitting", Journal of Structural Biology, vol. 174, no. 2,
             pp. 333--343, 2011. DOI: https://doi.org/10.1016/j.jsb.2011.01.012
 
     """
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-
-    def scoring_function(
-        self,
-        transformed_coordinates: NDArray,
-        transformed_coordinates_mask: NDArray,
-        **kwargs,
-    ) -> float:
-        """
-        Compute the Normal Vector Score.
-
-        Given the template and target vectors, this function computes the average
-        cosine similarity between the two sets of vectors.
+    __doc__ += _MatchCoordinatesToDensity.__doc__
 
-        Parameters
-        ----------
-        template_vectors : NDArray
-            Normal vectors derived from the template.
-        target_vectors : NDArray
-            Normal vectors derived from the target.
-
-        Returns
-        -------
-        float
-            The Normal Vector Score.
-        """
-        numerator = np.multiply(transformed_coordinates, self.target_coordinates)
-        denominator = np.linalg.norm(transformed_coordinates)
+    def __call__(self) -> float:
+        """Returns the score of the current configuration."""
+        numerator = np.multiply(
+            self.template_coordinates_rotated, self.target_coordinates
+        )
+        denominator = np.linalg.norm(self.template_coordinates_rotated)
         denominator *= np.linalg.norm(self.target_coordinates)
         score = np.mean(numerator / denominator)
         return score
 
 
 MATCHING_OPTIMIZATION_REGISTER = {
     "CrossCorrelation": CrossCorrelation,
@@ -825,299 +1001,200 @@
     "NormalizedCrossCorrelation": NormalizedCrossCorrelation,
     "MaskedCrossCorrelation": MaskedCrossCorrelation,
     "PartialLeastSquareDifference": PartialLeastSquareDifference,
     "Envelope": Envelope,
     "Chamfer": Chamfer,
     "MutualInformation": MutualInformation,
     "NormalVectorScore": NormalVectorScore,
+    "FLC": FLC,
 }
 
 
 def register_matching_optimization(match_name: str, match_class: type):
     """
-    Registers a class to be used by :py:class:`FitRefinement`.
+    Registers a new mtaching method.
 
     Parameters
     ----------
     match_name : str
         Name of the matching instance.
     match_class : type
         Class pointer.
 
     Raises
     ------
     ValueError
         If any of the required methods is not defined.
     """
-    methods_to_check = ["__init__", "__call__", "scoring_function"]
+    methods_to_check = ["__init__", "__call__"]
 
     for method in methods_to_check:
         if not hasattr(match_class, method):
             raise ValueError(
                 f"Method '{method}' is not defined in the provided class or object."
             )
     MATCHING_OPTIMIZATION_REGISTER[match_name] = match_class
 
 
-class FitRefinement:
-    """
-    A class to refine the fit between target and template coordinates.
-
-    Notes
-    -----
-    By default scipy.optimize.differential_evolution or scipy.optimize.basinhopping
-    are used which can be unreliable if the initial alignment is very poor. Other
-    optimizers can be implemented by subclassing :py:class:`FitRefinement` and
-    overwriting the :py:meth:`FitRefinement.refine` function.
-
+def create_score_object(score: str, **kwargs) -> object:
     """
+    Initialize score object with name ``score`` using `**kwargs``.
 
-    @staticmethod
-    def map_coordinates_to_array(
-        coordinates: NDArray,
-        array_shape: NDArray,
-        array_origin: NDArray,
-        sampling_rate: NDArray,
-        coordinates_mask: NDArray = None,
-    ) -> Tuple[NDArray, NDArray]:
-        """
-        Map coordinates to a volume based on given voxel size and origin.
-
-        Parameters
-        ----------
-        coordinates : NDArray
-            An array representing the coordinates to be mapped [d x N].
-        array_shape : NDArray
-            The shape of the array to which the coordinates are mapped.
-        array_origin : NDArray
-            The origin of the array to which the coordinates are mapped.
-        sampling_rate : NDArray
-            The size of a voxel in the array.
-        coordinates_mask : NDArray, optional
-            An array representing the mask for the coordinates [d x T].
+    Parameters
+    ----------
+    score: str
+        Name of the score.
+    **kwargs: Dict
+        Keyword arguments passed to the __init__ method of the score object.
+
+    Returns
+    -------
+    object
+        Initialized score object.
 
-        Returns
-        -------
-        tuple
-            Returns transformed coordinates, transformed coordinates mask,
-            mask for in_volume points, and mask for in_volume points in mask.
-        """
-        coordinates = coordinates.astype(sampling_rate.dtype)
-        np.divide(
-            coordinates - array_origin[:, None], sampling_rate[:, None], out=coordinates
-        )
-        transformed_coordinates = coordinates.astype(int)
-        in_volume = np.logical_and(
-            transformed_coordinates < np.array(array_shape)[:, None],
-            transformed_coordinates >= 0,
-        ).min(axis=0)
+    Raises
+    ------
+    ValueError
+        If ``score`` is not a key in MATCHING_OPTIMIZATION_REGISTER.
 
-        transformed_coordinates_mask, in_volume_mask = None, None
+    See Also
+    --------
+    :py:meth:`register_matching_optimization`
+    """
 
-        if coordinates_mask is not None:
-            coordinates_mask = coordinates_mask.astype(sampling_rate.dtype)
-            np.divide(
-                coordinates_mask - array_origin[:, None],
-                sampling_rate[:, None],
-                out=coordinates_mask,
-            )
-            transformed_coordinates_mask = coordinates_mask.astype(int)
-            in_volume_mask = np.logical_and(
-                transformed_coordinates_mask < np.array(array_shape)[:, None],
-                transformed_coordinates_mask >= 0,
-            ).min(axis=0)
+    score_object = MATCHING_OPTIMIZATION_REGISTER.get(score, None)
 
-        return (
-            transformed_coordinates,
-            transformed_coordinates_mask,
-            in_volume,
-            in_volume_mask,
+    if score_object is None:
+        raise ValueError(
+            f"{score} is not defined. Please pick from "
+            f" {', '.join(list(MATCHING_OPTIMIZATION_REGISTER.keys()))}."
         )
 
-    @staticmethod
-    def array_from_coordinates(
-        coordinates: NDArray,
-        weights: NDArray,
-        sampling_rate: NDArray,
-        origin: NDArray = None,
-        shape: NDArray = None,
-    ) -> Tuple[NDArray, NDArray, NDArray]:
-        """
-        Create a volume from coordinates, using given weights and voxel size.
-
-        Parameters
-        ----------
-        coordinates : NDArray
-            An array representing the coordinates [d x N].
-        weights : NDArray
-            An array representing the weights for each coordinate [N].
-        sampling_rate : NDArray
-            The size of a voxel in the volume.
-        origin : NDArray, optional
-            The origin of the volume.
-        shape : NDArray, optional
-            The shape of the volume.
-
-        Returns
-        -------
-        tuple
-            Returns the generated volume, positions of coordinates, and origin.
-        """
-        if origin is None:
-            origin = coordinates.min(axis=1)
-
-        positions = np.divide(coordinates - origin[:, None], sampling_rate[:, None])
-        positions = positions.astype(int)
-
-        if shape is None:
-            shape = positions.max(axis=1) + 1
-
-        arr = np.zeros(shape, dtype=np.float32)
-        np.add.at(arr, tuple(positions), weights)
-        return arr, positions, origin
-
-    def refine(
-        self,
-        target_coordinates: NDArray,
-        target_weights: NDArray,
-        template_coordinates: NDArray,
-        template_weights: NDArray,
-        sampling_rate: float = None,
-        translational_uncertainty: Tuple[float] = None,
-        rotational_uncertainty: Tuple[float] = None,
-        scoring_class: str = "CrossCorrelation",
-        scoring_class_parameters: Dict = dict(),
-        local_optimization: bool = True,
-        maxiter: int = 100,
-    ) -> (NDArray, NDArray):
-        """
-        Refines the alignment of template coordinates to target coordinates.
-
-        Parameters
-        ----------
-        target_coordinates : NDArray
-            The coordinates of the target.
-
-        target_weights : NDArray
-            The weights of the target.
-
-        template_coordinates : NDArray
-            The coordinates of the template.
-
-        template_weights : NDArray
-            The weights of the template.
-
-        sampling_rate : float, optional
-            The size of the voxel. Default is None.
-
-        translational_uncertainty : (float,), optional
-            The translational uncertainty. Default is None.
-
-        rotational_uncertainty : (float,), optional
-            The rotational uncertainty. Default is None.
-
-        scoring_class : str, optional
-            The scoring class to be used. Default is "CC".
+    score_object = score_object(**kwargs)
+    return score_object
 
-        scoring_class_parameters : dict, optional
-            The parameters for the scoring class. Default is an empty dictionary.
 
-        local_optimization : bool, optional
-            Whether to use local optimization. Default is True.
-
-        maxiter : int, optional
-            The maximum number of iterations. Default is 100.
-
-        Returns
-        -------
-        tuple
-            A tuple containing the translation and rotation matrix of the refinement,
-            as well as the score of the refinement.
+def optimize_match(
+    score_object: object,
+    bounds_translation: Tuple[Tuple[float]] = None,
+    bounds_rotation: Tuple[Tuple[float]] = None,
+    optimization_method: str = "basinhopping",
+    maxiter: int = 500,
+) -> Tuple[ArrayLike, ArrayLike, float]:
+    """
+    Find the translation and rotation optimizing the score returned by `score_object`
+    with respect to provided bounds.
 
-        Raises
-        ------
-        NotNotImplementedError
-            If scoring class is not a part of `MATCHING_OPTIMIZATION_REGISTER`.
-            Individual scores can be added via
-            :py:meth:`register_matching_optimization`.
-
-        See Also
-        --------
-        :py:meth:`register_matching_optimization`
-        """
-        if scoring_class not in MATCHING_OPTIMIZATION_REGISTER:
-            raise NotImplementedError(
-                f"Parameter score has to be one of "
-                f"{', '.join(MATCHING_OPTIMIZATION_REGISTER.keys())}."
-            )
-        scoring_class = MATCHING_OPTIMIZATION_REGISTER.get(scoring_class, None)
+    Parameters
+    ----------
+    score_object: object
+        Class object that defines a score method, which returns a floating point
+        value given a tuple of floating points where the first half describes a
+        translation and the second a rotation. The score will be minimized, i.e.
+        it has to be negated if similarity should be optimized.
+    bounds_translation : tuple of tuple float, optional
+        Bounds on the evaluated translations. Has to be specified per dimension
+        as tuple of (min, max). Default is None.
+    bounds_rotation : tuple of tuple float, optional
+        Bounds on the evaluated zyx Euler angles. Has to be specified per dimension
+        as tuple of (min, max). Default is None.
+    optimization_method : str, optional
+        Optimizer that will be used, by default basinhopping. For further
+        information refer to :doc:`scipy:reference/optimize`.
+
+        +--------------------------+-----------------------------------------+
+        | 'differential_evolution' | Highest accuracy but long runtime.      |
+        |                          | Requires bounds on translation.         |
+        +--------------------------+-----------------------------------------+
+        | 'basinhopping'           | Decent accuracy, medium runtime.        |
+        +--------------------------+-----------------------------------------+
+        | 'minimize'               | If initial values are closed to optimum |
+        |                          | decent performance, short runtime.      |
+        +--------------------------+-----------------------------------------+
+    maxiter : int, optional
+        The maximum number of iterations. Default is 500. Not considered for
+        `optimization_method` 'minimize'.
+
+    Returns
+    -------
+    Tuple[ArrayLike, ArrayLike, float]
+        Translation and rotation matrix yielding final score.
 
-        if sampling_rate is None:
-            sampling_rate = np.ones(1)
-        sampling_rate = np.repeat(
-            sampling_rate, target_coordinates.shape[0] // sampling_rate.size
-        )
-
-        score = scoring_class(
-            target_coordinates=target_coordinates,
-            template_coordinates=template_coordinates,
-            target_weights=target_weights,
-            template_weights=template_weights,
-            sampling_rate=sampling_rate,
-            **scoring_class_parameters,
-        )
-
-        initial_score = score(np.zeros(6))
-
-        mass_center_target = np.dot(target_coordinates, target_weights)
-        mass_center_target /= target_weights.sum()
-        mass_center_template = np.dot(template_coordinates, template_weights)
-        mass_center_template /= template_weights.sum()
-
-        if translational_uncertainty is None:
-            mass_center_difference = np.ceil(
-                np.subtract(mass_center_target, mass_center_template)
-            ).astype(int)
-            target_range = np.ceil(
-                np.divide(
-                    np.subtract(
-                        target_coordinates.max(axis=1), target_coordinates.min(axis=1)
-                    ),
-                    2,
-                )
-            ).astype(int)
-            translational_uncertainty = tuple(
-                (center - start, center + start)
-                for center, start in zip(mass_center_difference, target_range)
-            )
-        if rotational_uncertainty is None:
-            rotational_uncertainty = tuple(
-                (-90, 90) for _ in range(target_coordinates.shape[0])
-            )
+    Raises
+    ------
+    ValueError
+        If `optimization_method` is not supported.
 
-        uncertainty = (*translational_uncertainty, *rotational_uncertainty)
-        bounds = [bound if bound != (0, 0) else (-1e-9, 1e-9) for bound in uncertainty]
+    Notes
+    -----
+    This function currently only supports three-dimensional optimization and
+    `score_object` will be modified during this operation.
+    """
+    ndim = 3
+    _optimization_method = {
+        "differential_evolution": differential_evolution,
+        "basinhopping": basinhopping,
+        "minimize": minimize,
+    }
+    if optimization_method not in _optimization_method:
+        raise ValueError(
+            f"{optimization_method} is not supported. "
+            f"Pick from {', '.join(list(_optimization_method.keys()))}"
+        )
+
+    finfo = np.finfo(np.float32)
+
+    # DE always requires bounds
+    if optimization_method == "differential_evolution" and bounds_translation is None:
+        bounds_translation = tuple((finfo.min, finfo.max) for _ in range(ndim))
+
+    if bounds_translation is None and bounds_rotation is not None:
+        bounds_translation = tuple((finfo.min, finfo.max) for _ in range(ndim))
+
+    if bounds_rotation is None and bounds_translation is not None:
+        bounds_rotation = tuple((-180, 180) for _ in range(ndim))
+
+    bounds, linear_constraint = None, ()
+    if bounds_rotation is not None and bounds_translation is not None:
+        uncertainty = (*bounds_translation, *bounds_rotation)
+        bounds = [
+            bound if bound != (0, 0) else (-finfo.resolution, finfo.resolution)
+            for bound in uncertainty
+        ]
         linear_constraint = LinearConstraint(
             np.eye(len(bounds)), np.min(bounds, axis=1), np.max(bounds, axis=1)
         )
 
-        if local_optimization:
-            result = basinhopping(
-                x0=np.zeros(6),
-                func=score,
-                niter=maxiter,
-                minimizer_kwargs={"method": "COBYLA", "constraints": linear_constraint},
-            )
-        else:
-            result = differential_evolution(
-                func=score,
-                bounds=bounds,
-                constraints=linear_constraint,
-                maxiter=maxiter,
-            )
+    initial_score = score_object()
+    if optimization_method == "basinhopping":
+        result = basinhopping(
+            x0=np.zeros(2 * ndim),
+            func=score_object.score,
+            niter=maxiter,
+            minimizer_kwargs={"method": "COBYLA", "constraints": linear_constraint},
+        )
+    elif optimization_method == "differential_evolution":
+        result = differential_evolution(
+            func=score_object.score,
+            bounds=bounds,
+            constraints=linear_constraint,
+            maxiter=maxiter,
+        )
+    elif optimization_method == "minimize":
+        result = minimize(
+            x0=np.zeros(2 * ndim),
+            fun=score_object.score,
+            bounds=bounds,
+            constraints=linear_constraint,
+        )
+    print(f"Niter: {result.nit}, success : {result.success} ({result.message}).")
+    print(f"Initial score: {initial_score} - Refined score: {result.fun}")
+    if initial_score < result.fun:
+        print("Initial score better than refined score. Returning identity.")
+        result.x = np.zeros_like(result.x)
+    translation, rotation = result.x[:ndim], result.x[ndim:]
+    rotation_matrix = euler_to_rotationmatrix(rotation)
+    return translation, rotation_matrix, result.fun
 
-        print(f"Initial score: {-initial_score} - Refined score: {-result.fun}")
-        if initial_score < result.fun:
-            result.x = np.zeros_like(result.x)
-        translation, rotation = result.x[:3], result.x[3:]
-        rotation_matrix = euler_to_rotationmatrix(rotation)
-        return translation, rotation_matrix, -result.fun
+
+class FitRefinement:
+    pass
```

### Comparing `pytme-0.1.9/tme/matching_utils.py` & `pytme-0.2.0b0/tme/matching_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -225,14 +225,15 @@
 
 def compute_parallelization_schedule(
     shape1: NDArray,
     shape2: NDArray,
     max_cores: int,
     max_ram: int,
     matching_method: str,
+    split_axes: Tuple[int] = None,
     backend: str = None,
     split_only_outer: bool = False,
     shape1_padding: NDArray = None,
     analyzer_method: str = None,
     max_splits: int = 256,
     float_nbytes: int = 4,
     complex_nbytes: int = 8,
@@ -255,14 +256,16 @@
         The shape of the second input tensor.
     max_cores : int
         The maximum number of cores that can be used.
     max_ram : int
         The maximum amount of memory that can be used.
     matching_method : str
         The metric used for scoring the computations.
+    split_axes : tuple
+        Axes that can be used for splitting. By default all are considered.
     backend : str, optional
         Backend used for computations.
     split_only_outer : bool, optional
         Whether only outer splits sould be considered.
     analyzer_method : str
         The method used for score analysis.
     max_splits : int, optional
@@ -299,14 +302,21 @@
             core_assignments.append((i, max_cores // i))
             core_assignments.append((max_cores // i, i))
 
     if split_only_outer:
         core_assignments = [(1, max_cores)]
 
     possible_params, split_axis = [], np.argmax(shape1)
+
+    split_axis_index = split_axis
+    if split_axes is not None:
+        split_axis, split_axis_index = split_axes[0], 0
+    else:
+        split_axes = tuple(i for i in range(len(shape1)))
+
     split_factor, n_splits = [1 for _ in range(len(shape1))], 0
     while n_splits <= max_splits:
         splits = {k: split_factor[k] for k in range(len(split_factor))}
         array_slices = split_numpy_array_slices(shape=shape1, splits=splits)
         array_widths = [
             tuple(x.stop - x.start for x in split) for split in array_slices
         ]
@@ -337,17 +347,19 @@
 
             inits = n_splits // outer_cores
             if max_usage < max_ram:
                 possible_params.append(
                     (*split_factor, outer_cores, inner_cores, n_splits, inits)
                 )
         split_factor[split_axis] += 1
-        split_axis += 1
-        if split_axis == shape1.size:
-            split_axis = 0
+
+        split_axis_index += 1
+        if split_axis_index == len(split_axes):
+            split_axis_index = 0
+        split_axis = split_axes[split_axis_index]
 
     possible_params = np.array(possible_params)
     if not len(possible_params):
         print(
             "No suitable assignment found. Consider increasing "
             "max_ram or decrease max_cores."
         )
@@ -605,14 +617,99 @@
         ret, _ = np.linalg.qr(As)
         dets = np.linalg.det(ret)
         neg_dets = dets < 0
         ret[neg_dets, :, -1] *= -1
     return ret
 
 
+def get_rotations_around_vector(
+    cone_angle: float,
+    cone_sampling: float,
+    axis_angle: float = 360.0,
+    axis_sampling: float = None,
+    vector: Tuple[float] = (1, 0, 0),
+    n_symmetry: int = 1,
+    convention: str = None,
+) -> NDArray:
+    """
+    Generate rotations describing the possible placements of a vector in a cone.
+
+    Parameters
+    ----------
+    cone_angle : float
+        The half-angle of the cone in degrees.
+    cone_sampling : float
+        Angular increment used for sampling points on the cone in degrees.
+    axis_angle : float, optional
+        The total angle of rotation around the vector axis in degrees (default is 360.0).
+    axis_sampling : float, optional
+        Angular increment used for sampling points around the vector axis in degrees.
+        If None, it takes the value of `cone_sampling`.
+    vector : Tuple[float], optional
+        Cartesian coordinates in zyx convention.
+    n_symmetry : int, optional
+        Number of symmetry axis around the vector axis.
+    convention : str, optional
+        Convention for angles. By default returns rotation matrices.
+
+    Returns
+    -------
+    NDArray
+        An array of rotation angles represented as Euler angles (phi, theta, psi) in degrees.
+        The shape of the array is (n, 3), where `n` is the total number of rotation angles.
+        Each row represents a set of rotation angles.
+
+    References
+    ----------
+    .. [1] https://stackoverflow.com/questions/9600801/evenly-distributing-n-points-on-a-sphere
+
+    """
+    if axis_sampling is None:
+        axis_sampling = cone_sampling
+
+    # Heuristic to estimate necessary number of points on sphere
+    theta = np.linspace(0, cone_angle, round(cone_angle / cone_sampling) + 1)
+    number_of_points = np.ceil(
+        360 * np.divide(np.sin(np.radians(theta)), cone_sampling),
+    )
+    number_of_points = int(np.sum(number_of_points + 1) + 2)
+
+    # Golden Spiral
+    indices = np.arange(0, number_of_points, dtype=float) + 0.5
+    radius = cone_angle * np.sqrt(indices / number_of_points)
+    theta = np.pi * (1 + np.sqrt(5)) * indices
+
+    angles_vector = Rotation.from_euler(
+        angles=rotation_aligning_vectors([1, 0, 0], vector, convention="zyx"),
+        seq="zyx",
+        degrees=True,
+    )
+
+    # phi, theta, psi
+    axis_angle /= n_symmetry
+    phi_steps = np.max(np.round(axis_angle / axis_sampling), 1)
+    phi = np.linspace(0, axis_angle, phi_steps + 1)[:-1]
+    np.add(phi, angles_vector.as_euler("zyx", degrees=True)[0], out=phi)
+    angles = np.stack(
+        [radius * np.cos(theta), radius * np.sin(theta), np.zeros_like(radius)], axis=1
+    )
+    angles = np.repeat(angles, phi_steps, axis=0)
+    angles[:, 2] = np.tile(phi, radius.size)
+
+    angles = Rotation.from_euler(angles=angles, seq="zyx", degrees=True)
+    angles = angles_vector * angles
+
+    if convention is None:
+        rotation_angles = angles.as_matrix()
+    else:
+        rotation_angles = angles.as_euler(seq=convention, degrees=True)
+
+    return rotation_angles
+
+
 def minimum_enclosing_box(
     coordinates: NDArray,
     margin: NDArray = None,
     use_geometric_center: bool = False,
 ) -> Tuple[int]:
     """
     Computes the minimal enclosing box around coordinates with margin.
@@ -745,66 +842,113 @@
         f"{round(4*np.prod(convolution_shape_init)/1e6, 3)} MB "
         f"to {round(4*np.prod(convolution_shape)/1e6, 3)} MB "
         f"({'-' if saving > 0 else ''}{abs(round(saving, 2))}%)"
     )
     return reference_fit
 
 
-def euler_to_rotationmatrix(angles: Tuple[float]) -> NDArray:
+def euler_to_rotationmatrix(angles: Tuple[float], convention: str = "zyx") -> NDArray:
     """
     Convert Euler angles to a rotation matrix.
 
     Parameters
     ----------
     angles : tuple
         A tuple representing the Euler angles in degrees.
+    convention : str, optional
+        Euler angle convention.
 
     Returns
     -------
     NDArray
         The generated rotation matrix.
     """
     n_angles = len(angles)
-    angle_convention = "zyx"[:n_angles]
+    angle_convention = convention[:n_angles]
     if n_angles == 1:
         angles = (angles, 0, 0)
     rotation_matrix = (
         Rotation.from_euler(angle_convention, angles, degrees=True)
         .as_matrix()
         .astype(np.float32)
     )
     return rotation_matrix
 
 
-def euler_from_rotationmatrix(rotation_matrix: NDArray) -> Tuple:
+def euler_from_rotationmatrix(
+    rotation_matrix: NDArray, convention: str = "zyx"
+) -> Tuple:
     """
     Convert a rotation matrix to euler angles.
 
     Parameters
     ----------
     rotation_matrix : NDArray
         A 2 x 2 or 3 x 3 rotation matrix in z y x form.
-
+    convention : str, optional
+        Euler angle convention.
     Returns
     -------
     Tuple
         The generate euler angles in degrees
     """
     if rotation_matrix.shape[0] == 2:
         temp_matrix = np.eye(3)
         temp_matrix[:2, :2] = rotation_matrix
         rotation_matrix = temp_matrix
     euler_angles = (
         Rotation.from_matrix(rotation_matrix)
-        .as_euler("zyx", degrees=True)
+        .as_euler(convention, degrees=True)
         .astype(np.float32)
     )
     return euler_angles
 
 
+def rotation_aligning_vectors(
+    initial_vector: NDArray, target_vector: NDArray = [1, 0, 0], convention: str = None
+):
+    """
+    Compute the rotation matrix or Euler angles required to align an initial vector with a target vector.
+
+    Parameters
+    ----------
+    initial_vector : NDArray
+        The initial vector to be rotated.
+    target_vector : NDArray, optional
+        The target vector to align the initial vector with. Default is [1, 0, 0].
+    convention : str, optional
+        The generate euler angles in degrees. If None returns a rotation matrix instead.
+
+    Returns
+    -------
+    rotation_matrix_or_angles : NDArray or tuple
+        Rotation matrix if convention is None else tuple of euler angles.
+    """
+    initial_vector = np.asarray(initial_vector, dtype=np.float32)
+    target_vector = np.asarray(target_vector, dtype=np.float32)
+    initial_vector /= np.linalg.norm(initial_vector)
+    target_vector /= np.linalg.norm(target_vector)
+
+    rotation_matrix = np.eye(len(initial_vector))
+    if not np.allclose(initial_vector, target_vector):
+        rotation_axis = np.cross(initial_vector, target_vector)
+        rotation_angle = np.arccos(np.dot(initial_vector, target_vector))
+        k = rotation_axis / np.linalg.norm(rotation_axis)
+        K = np.array([[0, -k[2], k[1]], [k[2], 0, -k[0]], [-k[1], k[0], 0]])
+        rotation_matrix = np.eye(3)
+        rotation_matrix += np.sin(rotation_angle) * K
+        rotation_matrix += (1 - np.cos(rotation_angle)) * np.dot(K, K)
+
+    if convention is None:
+        return rotation_matrix
+
+    angles = euler_from_rotationmatrix(rotation_matrix, convention=convention)
+    return angles
+
+
 def rigid_transform(
     coordinates: NDArray,
     rotation_matrix: NDArray,
     out: NDArray,
     translation: NDArray,
     use_geometric_center: bool = False,
     coordinates_mask: NDArray = None,
```

### Comparing `pytme-0.1.9/tme/parser.py` & `pytme-0.2.0b0/tme/parser.py`

 * *Files identical despite different names*

### Comparing `pytme-0.1.9/tme/preprocessor.py` & `pytme-0.2.0b0/tme/preprocessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -650,20 +650,17 @@
         -------
         NDArray
             Simulated electron densities.
         """
         array = template.copy()
         interpolation_box = array.shape
 
-        print(array.shape)
-
         for k in range(template.ndim):
             array = decimate(array, q=level, axis=k)
 
-        print(array.shape)
         template = zoom(array, np.divide(template.shape, array.shape))
         template = self.interpolate_box(box=interpolation_box, arr=template)
 
         return template
 
     def wavelet_filter(
         self,
@@ -764,29 +761,32 @@
         positions = (coordinates - origin) / sampling_rate
         positions = positions[:, ::-1]
 
         out = np.zeros(shape, dtype=np.float32)
         sigma = sigma_factor * resolution
         sigma_grid = sigma / sampling_rate
         sigma_grid2 = sigma_grid * sigma_grid
-        for index, point in enumerate(np.rollaxis(positions, 0)):
-            starts = np.maximum(np.ceil(point - cutoff_value * sigma_grid), 0).astype(
-                int
-            )
-            stops = np.minimum(
-                np.floor(point + cutoff_value * sigma_grid), shape
-            ).astype(int)
 
-            grid_index = np.meshgrid(
-                *[range(start, stop) for start, stop in zip(starts, stops)]
-            )
-            distances = np.einsum(
-                "aijk->ijk",
-                np.array([(grid_index[i] - point[i]) ** 2 for i in range(len(point))]),
-                dtype=np.float64,
+        starts = np.maximum(np.ceil(positions - cutoff_value * sigma_grid), 0).astype(
+            int
+        )
+        stops = np.minimum(
+            np.floor(positions + cutoff_value * sigma_grid), shape
+        ).astype(int)
+        ranges = tuple(tuple(zip(start, stop)) for start, stop in zip(starts, stops))
+
+        positions = positions.reshape(
+            *positions.shape, *tuple(1 for _ in range(positions.shape[1]))
+        )
+        for index in range(positions.shape[0]):
+            grid_index = np.meshgrid(*[range(*coord) for coord in ranges[index]])
+            distances = np.sum(
+                np.square(np.subtract(grid_index, positions[index])),
+                dtype=np.float32,
+                axis=0,
             )
             np.add.at(
                 out,
                 tuple(grid_index),
                 weights[index] * np.exp(-0.5 * distances / sigma_grid2),
             )
 
@@ -1127,14 +1127,15 @@
 
     def step_wedge_mask(
         self,
         start_tilt: float,
         stop_tilt: float,
         tilt_step: float,
         shape: Tuple[int],
+        tilt_angles: Tuple[float] = None,
         opening_axis: int = 0,
         tilt_axis: int = 2,
         sigma: float = 0,
         omit_negative_frequencies: bool = True,
     ) -> NDArray:
         """
         Create a wedge mask with the same shape as template by rotating a
@@ -1180,15 +1181,17 @@
         of an N-1 dimensional hyperplane in N dimensions.
 
         See Also
         --------
         :py:meth:`Preprocessor.wedge_mask`
         :py:meth:`Preprocessor.continuous_wedge_mask`
         """
-        tilt_angles = np.arange(-start_tilt, stop_tilt + tilt_step, tilt_step)
+        if tilt_angles is None:
+            tilt_angles = np.arange(-start_tilt, stop_tilt + tilt_step, tilt_step)
+
         plane = np.zeros((shape[opening_axis], shape[tilt_axis]), dtype=np.float32)
         subset = tuple(
             slice(None) if i != 0 else slice(x // 2, x // 2 + 1)
             for i, x in enumerate(plane.shape)
         )
         plane[subset] = 1
         plane_rotated, wedge_volume = np.zeros_like(plane), np.zeros_like(plane)
```

### Comparing `pytme-0.1.9/tme/structure.py` & `pytme-0.2.0b0/tme/structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,53 +22,18 @@
 )
 from .helpers import atom_profile
 from .types import NDArray
 
 
 @dataclass(repr=False)
 class Structure:
-    """Represents atomic structures in accordance with the Protein Data Bank (PDB)
+    """
+    Represents atomic structures in accordance with the Protein Data Bank (PDB)
     format specification.
 
-    Attributes
-    ----------
-    record_type : NDArray
-        Type of the record, e.g., ATOM, HETATM. Array shape = (n,)
-    atom_serial_number : NDArray
-        Serial number assigned to each atom.  Array shape = (n,)
-    atom_name : NDArray
-        Standardized names for each atom.  Array shape = (n,)
-    atom_coordinate : NDArray
-        The 3D Cartesian coordinates of each atom in x, y, z.  Array shape = (n,3 )
-    alternate_location_indicator : NDArray
-        Indicator for alternate locations of an atom if it exists in multiple places.
-        Array shape = (n,)
-    residue_name : NDArray
-        Standard residue names where each atom belongs. Array shape = (n,)
-    chain_identifier : NDArray
-        Identifier for the chain where each atom is located. Array shape = (n,)
-    residue_sequence_number : NDArray
-        Sequence number of the residue in the protein chain for each atom.
-        Array shape = (n,)
-    code_for_residue_insertion : NDArray
-        Code to denote any residue insertion. Array shape = (n,)
-    occupancy : NDArray
-        Occupancy factor of each atom, indicating the fraction of time the atom
-        is located at its position. Array shape = (n,)
-    temperature_factor : NDArray
-        Measure of the atomic displacement or B-factor for each atom. Array shape = (n,)
-    segment_identifier : NDArray
-        Identifier for the segment where each atom belongs. Array shape = (n,)
-    element_symbol : NDArray
-        Atomic element symbol for each atom. Array shape = (n,)
-    charge : NDArray
-        Charge on the atom. Array shape = (n,)
-    details : dict
-        Any additional or auxiliary details. Array shape = (n,)
-
     References
     ----------
     .. [1]  https://www.cgl.ucsf.edu/chimera/docs/UsersGuide/tutorials/pdbintro.html
     """
 
     #: Return a numpy array with record types, e.g. ATOM, HETATM.
     record_type: NDArray
```

