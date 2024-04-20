# Comparing `tmp/exafs_neo-2.0.3.tar.gz` & `tmp/exafs_neo-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exafs_neo-2.0.3.tar", last modified: Fri Apr 19 05:23:12 2024, max compression
+gzip compressed data, was "exafs_neo-2.0.4.tar", last modified: Sat Apr 20 17:35:44 2024, max compression
```

## Comparing `exafs_neo-2.0.3.tar` & `exafs_neo-2.0.4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-19 05:23:12.679463 exafs_neo-2.0.3/
--rw-r--r--   0 andy       (501) staff       (20)    35198 2021-08-14 12:28:51.000000 exafs_neo-2.0.3/LICENSE
--rw-r--r--   0 andy       (501) staff       (20)     5897 2024-04-19 05:23:12.679390 exafs_neo-2.0.3/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)     5337 2024-04-01 06:56:32.000000 exafs_neo-2.0.3/README.md
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-19 05:23:12.667887 exafs_neo-2.0.3/exafs_neo/
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-02-03 07:16:06.000000 exafs_neo-2.0.3/exafs_neo/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)      152 2024-04-19 05:23:01.000000 exafs_neo-2.0.3/exafs_neo/_version.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-19 05:23:12.670130 exafs_neo-2.0.3/exafs_neo/analysis/
--rw-r--r--   0 andy       (501) staff       (20)    28217 2024-04-02 02:45:54.000000 exafs_neo-2.0.3/exafs_neo/analysis/EXAFS_Analysis.py
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-19 04:33:48.000000 exafs_neo-2.0.3/exafs_neo/analysis/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)    20093 2024-03-19 06:15:52.000000 exafs_neo-2.0.3/exafs_neo/analysis/larch_score.py
--rw-r--r--   0 andy       (501) staff       (20)     4189 2024-04-02 00:35:24.000000 exafs_neo-2.0.3/exafs_neo/exafs.py
--rw-r--r--   0 andy       (501) staff       (20)     5812 2024-04-02 02:57:21.000000 exafs_neo-2.0.3/exafs_neo/exafs_pop.py
--rw-r--r--   0 andy       (501) staff       (20)     5263 2024-04-02 02:59:48.000000 exafs_neo-2.0.3/exafs_neo/exafsfileobj.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-19 05:23:12.673119 exafs_neo-2.0.3/exafs_neo/gui/
--rw-r--r--   0 andy       (501) staff       (20)     3079 2024-03-19 04:34:51.000000 exafs_neo-2.0.3/exafs_neo/gui/Analysis_plot.py
--rw-r--r--   0 andy       (501) staff       (20)     5721 2024-03-18 17:12:48.000000 exafs_neo-2.0.3/exafs_neo/gui/Background_plot.py
--rw-r--r--   0 andy       (501) staff       (20)     2124 2024-03-18 17:11:48.000000 exafs_neo-2.0.3/exafs_neo/gui/Console.py
--rw-r--r--   0 andy       (501) staff       (20)     1341 2024-03-18 17:10:04.000000 exafs_neo-2.0.3/exafs_neo/gui/Misc_Function.py
--rw-r--r--   0 andy       (501) staff       (20)    55561 2024-04-02 19:11:16.000000 exafs_neo-2.0.3/exafs_neo/gui/XAFS_GUI.py
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-18 05:23:32.000000 exafs_neo-2.0.3/exafs_neo/gui/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     3268 2024-03-18 17:10:18.000000 exafs_neo-2.0.3/exafs_neo/gui/feff_folder_larch.py
--rw-r--r--   0 andy       (501) staff       (20)      265 2023-05-16 01:15:35.000000 exafs_neo-2.0.3/exafs_neo/gui/first_shell_fits.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-19 05:23:12.674782 exafs_neo-2.0.3/exafs_neo/gui/media/
--rw-r--r--   0 andy       (501) staff       (20)      539 2023-07-01 21:09:31.000000 exafs_neo-2.0.3/exafs_neo/gui/media/Citation
--rw-r--r--   0 andy       (501) staff       (20)    35198 2024-04-02 19:10:46.000000 exafs_neo-2.0.3/exafs_neo/gui/media/LICENSE
--rw-r--r--   0 andy       (501) staff       (20)     3848 2021-08-14 12:28:51.000000 exafs_neo-2.0.3/exafs_neo/gui/media/icon.png
--rw-r--r--   0 andy       (501) staff       (20)      983 2024-04-02 03:00:16.000000 exafs_neo-2.0.3/exafs_neo/helper.py
--rw-r--r--   0 andy       (501) staff       (20)     3909 2024-04-02 03:07:35.000000 exafs_neo-2.0.3/exafs_neo/individual.py
--rw-r--r--   0 andy       (501) staff       (20)     6206 2024-04-02 03:12:20.000000 exafs_neo-2.0.3/exafs_neo/ini_parser.py
--rwxr-xr-x   0 andy       (501) staff       (20)     1317 2024-04-02 03:13:29.000000 exafs_neo-2.0.3/exafs_neo/input_arg.py
--rw-r--r--   0 andy       (501) staff       (20)     9228 2024-03-23 23:40:18.000000 exafs_neo-2.0.3/exafs_neo/neoCrossOver.py
--rw-r--r--   0 andy       (501) staff       (20)     3364 2024-04-02 03:14:48.000000 exafs_neo-2.0.3/exafs_neo/neoFilePars.py
--rw-r--r--   0 andy       (501) staff       (20)     9223 2024-04-02 03:15:32.000000 exafs_neo-2.0.3/exafs_neo/neoMutator.py
--rw-r--r--   0 andy       (501) staff       (20)    13651 2024-04-17 06:16:45.000000 exafs_neo-2.0.3/exafs_neo/neoPars.py
--rw-r--r--   0 andy       (501) staff       (20)     3122 2024-04-02 03:23:54.000000 exafs_neo-2.0.3/exafs_neo/neoResult.py
--rw-r--r--   0 andy       (501) staff       (20)     3920 2024-04-02 03:27:20.000000 exafs_neo-2.0.3/exafs_neo/neoSelector.py
--rwxr-xr-x   0 andy       (501) staff       (20)     5748 2024-04-02 05:25:47.000000 exafs_neo-2.0.3/exafs_neo/parser.py
--rw-r--r--   0 andy       (501) staff       (20)     2953 2024-04-02 05:26:13.000000 exafs_neo-2.0.3/exafs_neo/pathObj.py
--rw-r--r--   0 andy       (501) staff       (20)     5121 2024-04-02 03:36:53.000000 exafs_neo-2.0.3/exafs_neo/pathrange.py
--rw-r--r--   0 andy       (501) staff       (20)     1321 2024-04-02 03:39:27.000000 exafs_neo-2.0.3/exafs_neo/pathrange_file.py
--rw-r--r--   0 andy       (501) staff       (20)    19175 2024-04-02 05:26:30.000000 exafs_neo-2.0.3/exafs_neo/utils.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-19 05:23:12.679050 exafs_neo-2.0.3/exafs_neo.egg-info/
--rw-r--r--   0 andy       (501) staff       (20)     5897 2024-04-19 05:23:12.000000 exafs_neo-2.0.3/exafs_neo.egg-info/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)     1482 2024-04-19 05:23:12.000000 exafs_neo-2.0.3/exafs_neo.egg-info/SOURCES.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2024-04-19 05:23:12.000000 exafs_neo-2.0.3/exafs_neo.egg-info/dependency_links.txt
--rw-r--r--   0 andy       (501) staff       (20)       99 2024-04-19 05:23:12.000000 exafs_neo-2.0.3/exafs_neo.egg-info/entry_points.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2024-02-18 07:51:41.000000 exafs_neo-2.0.3/exafs_neo.egg-info/not-zip-safe
--rw-r--r--   0 andy       (501) staff       (20)       40 2024-04-19 05:23:12.000000 exafs_neo-2.0.3/exafs_neo.egg-info/requires.txt
--rw-r--r--   0 andy       (501) staff       (20)       16 2024-04-19 05:23:12.000000 exafs_neo-2.0.3/exafs_neo.egg-info/top_level.txt
--rw-r--r--   0 andy       (501) staff       (20)       79 2024-04-19 05:23:12.679705 exafs_neo-2.0.3/setup.cfg
--rw-r--r--   0 andy       (501) staff       (20)     1240 2024-04-19 05:22:39.000000 exafs_neo-2.0.3/setup.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-19 05:23:12.678529 exafs_neo-2.0.3/tests/
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-17 22:01:17.000000 exafs_neo-2.0.3/tests/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     4089 2024-03-23 20:03:07.000000 exafs_neo-2.0.3/tests/test_EXAFS_analysis.py
--rw-r--r--   0 andy       (501) staff       (20)     1607 2024-03-23 19:26:46.000000 exafs_neo-2.0.3/tests/test_exafs_fileobj.py
--rw-r--r--   0 andy       (501) staff       (20)     3857 2024-03-23 20:01:49.000000 exafs_neo-2.0.3/tests/test_exafs_pars.py
--rw-r--r--   0 andy       (501) staff       (20)     2280 2024-03-20 02:02:00.000000 exafs_neo-2.0.3/tests/test_exafs_pathObj.py
--rw-r--r--   0 andy       (501) staff       (20)     1573 2024-02-03 07:05:06.000000 exafs_neo-2.0.3/tests/test_exafs_pathrange.py
--rw-r--r--   0 andy       (501) staff       (20)     1053 2024-03-20 03:41:05.000000 exafs_neo-2.0.3/tests/test_individual.py
--rw-r--r--   0 andy       (501) staff       (20)      514 2024-03-17 20:09:18.000000 exafs_neo-2.0.3/tests/test_ini_parser.py
--rw-r--r--   0 andy       (501) staff       (20)     3385 2024-03-23 20:03:36.000000 exafs_neo-2.0.3/tests/test_larchscore.py
--rw-r--r--   0 andy       (501) staff       (20)      976 2024-03-23 23:13:20.000000 exafs_neo-2.0.3/tests/test_neo_pop.py
--rw-r--r--   0 andy       (501) staff       (20)     5754 2024-03-31 00:14:43.000000 exafs_neo-2.0.3/tests/test_neocrossover.py
--rw-r--r--   0 andy       (501) staff       (20)     3771 2024-04-03 00:18:39.000000 exafs_neo-2.0.3/tests/test_neomutator.py
--rw-r--r--   0 andy       (501) staff       (20)      338 2024-02-18 20:02:49.000000 exafs_neo-2.0.3/tests/test_utils.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-20 17:35:44.953078 exafs_neo-2.0.4/
+-rw-r--r--   0 andy       (501) staff       (20)    35198 2021-08-14 12:28:51.000000 exafs_neo-2.0.4/LICENSE
+-rw-r--r--   0 andy       (501) staff       (20)     5897 2024-04-20 17:35:44.953001 exafs_neo-2.0.4/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)     5337 2024-04-20 17:35:07.000000 exafs_neo-2.0.4/README.md
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-20 17:35:44.942760 exafs_neo-2.0.4/exafs_neo/
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-02-03 07:16:06.000000 exafs_neo-2.0.4/exafs_neo/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)      152 2024-04-20 17:34:57.000000 exafs_neo-2.0.4/exafs_neo/_version.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-20 17:35:44.945072 exafs_neo-2.0.4/exafs_neo/analysis/
+-rw-r--r--   0 andy       (501) staff       (20)    28217 2024-04-02 02:45:54.000000 exafs_neo-2.0.4/exafs_neo/analysis/EXAFS_Analysis.py
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-19 04:33:48.000000 exafs_neo-2.0.4/exafs_neo/analysis/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)    20093 2024-03-19 06:15:52.000000 exafs_neo-2.0.4/exafs_neo/analysis/larch_score.py
+-rw-r--r--   0 andy       (501) staff       (20)     4189 2024-04-02 00:35:24.000000 exafs_neo-2.0.4/exafs_neo/exafs.py
+-rw-r--r--   0 andy       (501) staff       (20)     5812 2024-04-02 02:57:21.000000 exafs_neo-2.0.4/exafs_neo/exafs_pop.py
+-rw-r--r--   0 andy       (501) staff       (20)     5263 2024-04-02 02:59:48.000000 exafs_neo-2.0.4/exafs_neo/exafsfileobj.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-20 17:35:44.948035 exafs_neo-2.0.4/exafs_neo/gui/
+-rw-r--r--   0 andy       (501) staff       (20)     3079 2024-03-19 04:34:51.000000 exafs_neo-2.0.4/exafs_neo/gui/Analysis_plot.py
+-rw-r--r--   0 andy       (501) staff       (20)     5721 2024-03-18 17:12:48.000000 exafs_neo-2.0.4/exafs_neo/gui/Background_plot.py
+-rw-r--r--   0 andy       (501) staff       (20)     2124 2024-03-18 17:11:48.000000 exafs_neo-2.0.4/exafs_neo/gui/Console.py
+-rw-r--r--   0 andy       (501) staff       (20)     1575 2024-04-20 17:28:50.000000 exafs_neo-2.0.4/exafs_neo/gui/Misc_Function.py
+-rw-r--r--   0 andy       (501) staff       (20)    55561 2024-04-02 19:11:16.000000 exafs_neo-2.0.4/exafs_neo/gui/XAFS_GUI.py
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-18 05:23:32.000000 exafs_neo-2.0.4/exafs_neo/gui/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)     3268 2024-03-18 17:10:18.000000 exafs_neo-2.0.4/exafs_neo/gui/feff_folder_larch.py
+-rw-r--r--   0 andy       (501) staff       (20)      265 2023-05-16 01:15:35.000000 exafs_neo-2.0.4/exafs_neo/gui/first_shell_fits.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-20 17:35:44.949039 exafs_neo-2.0.4/exafs_neo/gui/media/
+-rw-r--r--   0 andy       (501) staff       (20)      539 2023-07-01 21:09:31.000000 exafs_neo-2.0.4/exafs_neo/gui/media/Citation
+-rw-r--r--   0 andy       (501) staff       (20)    35198 2024-04-02 19:10:46.000000 exafs_neo-2.0.4/exafs_neo/gui/media/LICENSE
+-rw-r--r--   0 andy       (501) staff       (20)     3848 2021-08-14 12:28:51.000000 exafs_neo-2.0.4/exafs_neo/gui/media/icon.png
+-rw-r--r--   0 andy       (501) staff       (20)      983 2024-04-02 03:00:16.000000 exafs_neo-2.0.4/exafs_neo/helper.py
+-rw-r--r--   0 andy       (501) staff       (20)     3909 2024-04-02 03:07:35.000000 exafs_neo-2.0.4/exafs_neo/individual.py
+-rw-r--r--   0 andy       (501) staff       (20)     6206 2024-04-02 03:12:20.000000 exafs_neo-2.0.4/exafs_neo/ini_parser.py
+-rwxr-xr-x   0 andy       (501) staff       (20)     1317 2024-04-02 03:13:29.000000 exafs_neo-2.0.4/exafs_neo/input_arg.py
+-rw-r--r--   0 andy       (501) staff       (20)     9228 2024-03-23 23:40:18.000000 exafs_neo-2.0.4/exafs_neo/neoCrossOver.py
+-rw-r--r--   0 andy       (501) staff       (20)     3364 2024-04-02 03:14:48.000000 exafs_neo-2.0.4/exafs_neo/neoFilePars.py
+-rw-r--r--   0 andy       (501) staff       (20)     9223 2024-04-02 03:15:32.000000 exafs_neo-2.0.4/exafs_neo/neoMutator.py
+-rw-r--r--   0 andy       (501) staff       (20)    13651 2024-04-17 06:16:45.000000 exafs_neo-2.0.4/exafs_neo/neoPars.py
+-rw-r--r--   0 andy       (501) staff       (20)     3122 2024-04-02 03:23:54.000000 exafs_neo-2.0.4/exafs_neo/neoResult.py
+-rw-r--r--   0 andy       (501) staff       (20)     3920 2024-04-02 03:27:20.000000 exafs_neo-2.0.4/exafs_neo/neoSelector.py
+-rwxr-xr-x   0 andy       (501) staff       (20)     5748 2024-04-02 05:25:47.000000 exafs_neo-2.0.4/exafs_neo/parser.py
+-rw-r--r--   0 andy       (501) staff       (20)     2953 2024-04-02 05:26:13.000000 exafs_neo-2.0.4/exafs_neo/pathObj.py
+-rw-r--r--   0 andy       (501) staff       (20)     5121 2024-04-02 03:36:53.000000 exafs_neo-2.0.4/exafs_neo/pathrange.py
+-rw-r--r--   0 andy       (501) staff       (20)     1321 2024-04-02 03:39:27.000000 exafs_neo-2.0.4/exafs_neo/pathrange_file.py
+-rw-r--r--   0 andy       (501) staff       (20)    19175 2024-04-02 05:26:30.000000 exafs_neo-2.0.4/exafs_neo/utils.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-20 17:35:44.952709 exafs_neo-2.0.4/exafs_neo.egg-info/
+-rw-r--r--   0 andy       (501) staff       (20)     5897 2024-04-20 17:35:44.000000 exafs_neo-2.0.4/exafs_neo.egg-info/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)     1482 2024-04-20 17:35:44.000000 exafs_neo-2.0.4/exafs_neo.egg-info/SOURCES.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2024-04-20 17:35:44.000000 exafs_neo-2.0.4/exafs_neo.egg-info/dependency_links.txt
+-rw-r--r--   0 andy       (501) staff       (20)       99 2024-04-20 17:35:44.000000 exafs_neo-2.0.4/exafs_neo.egg-info/entry_points.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2024-02-18 07:51:41.000000 exafs_neo-2.0.4/exafs_neo.egg-info/not-zip-safe
+-rw-r--r--   0 andy       (501) staff       (20)       40 2024-04-20 17:35:44.000000 exafs_neo-2.0.4/exafs_neo.egg-info/requires.txt
+-rw-r--r--   0 andy       (501) staff       (20)       16 2024-04-20 17:35:44.000000 exafs_neo-2.0.4/exafs_neo.egg-info/top_level.txt
+-rw-r--r--   0 andy       (501) staff       (20)       79 2024-04-20 17:35:44.953330 exafs_neo-2.0.4/setup.cfg
+-rw-r--r--   0 andy       (501) staff       (20)     1240 2024-04-19 05:22:39.000000 exafs_neo-2.0.4/setup.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-20 17:35:44.952399 exafs_neo-2.0.4/tests/
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-17 22:01:17.000000 exafs_neo-2.0.4/tests/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)     4089 2024-03-23 20:03:07.000000 exafs_neo-2.0.4/tests/test_EXAFS_analysis.py
+-rw-r--r--   0 andy       (501) staff       (20)     1607 2024-03-23 19:26:46.000000 exafs_neo-2.0.4/tests/test_exafs_fileobj.py
+-rw-r--r--   0 andy       (501) staff       (20)     3857 2024-03-23 20:01:49.000000 exafs_neo-2.0.4/tests/test_exafs_pars.py
+-rw-r--r--   0 andy       (501) staff       (20)     2280 2024-03-20 02:02:00.000000 exafs_neo-2.0.4/tests/test_exafs_pathObj.py
+-rw-r--r--   0 andy       (501) staff       (20)     1573 2024-02-03 07:05:06.000000 exafs_neo-2.0.4/tests/test_exafs_pathrange.py
+-rw-r--r--   0 andy       (501) staff       (20)     1053 2024-03-20 03:41:05.000000 exafs_neo-2.0.4/tests/test_individual.py
+-rw-r--r--   0 andy       (501) staff       (20)      514 2024-03-17 20:09:18.000000 exafs_neo-2.0.4/tests/test_ini_parser.py
+-rw-r--r--   0 andy       (501) staff       (20)     3385 2024-03-23 20:03:36.000000 exafs_neo-2.0.4/tests/test_larchscore.py
+-rw-r--r--   0 andy       (501) staff       (20)      976 2024-03-23 23:13:20.000000 exafs_neo-2.0.4/tests/test_neo_pop.py
+-rw-r--r--   0 andy       (501) staff       (20)     5754 2024-03-31 00:14:43.000000 exafs_neo-2.0.4/tests/test_neocrossover.py
+-rw-r--r--   0 andy       (501) staff       (20)     3771 2024-04-03 00:18:39.000000 exafs_neo-2.0.4/tests/test_neomutator.py
+-rw-r--r--   0 andy       (501) staff       (20)      338 2024-02-18 20:02:49.000000 exafs_neo-2.0.4/tests/test_utils.py
```

### Comparing `exafs_neo-2.0.3/LICENSE` & `exafs_neo-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/PKG-INFO` & `exafs_neo-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exafs_neo
-Version: 2.0.3
+Version: 2.0.4
 Summary: exafs_neo AI analysis using GA
 Home-page: https://github.com/laumiulun/EXAFS_Neo
 Download-URL: https://github.com/laumiulun/EXAFS_Neo/tarball/master
 Author: Miu Lun Lau, Jeff Terry, Min Long
 Author-email: andylau@u.boisestate.edu, jterry98@iit.edu, minlong@boisestate.edu
 License: GPLv3
 Keywords: exafs_neo,AI,analysis
@@ -14,17 +14,17 @@
 Requires-Dist: xraylarch
 Requires-Dist: attrs
 Requires-Dist: matplotlib
 Requires-Dist: psutil
 
 # EXAFS Neo
 
-#### Versions: 2.0.2
+#### Versions: 2.0.4
 
-#### Last update: Mar 23, 2024
+#### Last update: Apr 20, 2024
 
 <!-- ![example workflow](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/<WORKFLOW_FILE>/badge.svg) -->
 
 [![Test with Ubuntu, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml)[![Test with Windows, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml)
 
 
 EXAFS Neo utilize Genetic algorithm in fitting Extended X-ray absorption fine structure(EXAFS).
```

### Comparing `exafs_neo-2.0.3/README.md` & `exafs_neo-2.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # EXAFS Neo
 
-#### Versions: 2.0.2
+#### Versions: 2.0.4
 
-#### Last update: Mar 23, 2024
+#### Last update: Apr 20, 2024
 
 <!-- ![example workflow](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/<WORKFLOW_FILE>/badge.svg) -->
 
 [![Test with Ubuntu, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml)[![Test with Windows, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml)
 
 
 EXAFS Neo utilize Genetic algorithm in fitting Extended X-ray absorption fine structure(EXAFS).
```

### Comparing `exafs_neo-2.0.3/exafs_neo/analysis/EXAFS_Analysis.py` & `exafs_neo-2.0.4/exafs_neo/analysis/EXAFS_Analysis.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/analysis/larch_score.py` & `exafs_neo-2.0.4/exafs_neo/analysis/larch_score.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/exafs.py` & `exafs_neo-2.0.4/exafs_neo/exafs.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/exafs_pop.py` & `exafs_neo-2.0.4/exafs_neo/exafs_pop.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/exafsfileobj.py` & `exafs_neo-2.0.4/exafs_neo/exafsfileobj.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/gui/Analysis_plot.py` & `exafs_neo-2.0.4/exafs_neo/gui/Analysis_plot.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/gui/Background_plot.py` & `exafs_neo-2.0.4/exafs_neo/gui/Background_plot.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/gui/Console.py` & `exafs_neo-2.0.4/exafs_neo/gui/Console.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/gui/Misc_Function.py` & `exafs_neo-2.0.4/exafs_neo/gui/Misc_Function.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,27 +25,31 @@
     (See Toothy's implementation in the comments)
     '''
     return [atoi(c) for c in re.split(r'(\d+)', text)]
 
 
 def check_sabcor_folder(ostype):
     # check sabcor folder if it initializes
-
+    default_sabcor = False
     if ostype == "Windows":
         print("Window doesn't have sabcor capabilites, continue without sabcor")
     else:
-        if not os.listdir('./contrib/sabcor'):
-            print("Please Initialize \"Sabcor\" as submodules")
-            exit()
-        else:
-
-            if os.path.exists('../contrib/sabcor/sabcor'):
-                print("Please make the sabcor executable first in './contrib/sabcor' directory")
+        if os.path.exists('./contrib/sabcor'):
+            if not os.listdir('./contrib/sabcor'):
+                print("Please Initialize \"Sabcor\" as submodules")
+                exit()
             else:
-                sys.path.insert(1, './contrib/sabcor')
-                from sabcor import check_executable
+                if os.path.exists('../contrib/sabcor/sabcor'):
+                    print("Please make the sabcor executable first in './contrib/sabcor' directory")
+                else:
+                    sys.path.insert(1, './contrib/sabcor')
+                    from sabcor import check_executable
+                    default_sabcor = True
+        else:
+            print("Sabcor is not found...")
 
+    return default_sabcor
 
 
 if __name__ == "__main__":
     os_name = get_platform()
     print(os_name)
```

### Comparing `exafs_neo-2.0.3/exafs_neo/gui/XAFS_GUI.py` & `exafs_neo-2.0.4/exafs_neo/gui/XAFS_GUI.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/gui/feff_folder_larch.py` & `exafs_neo-2.0.4/exafs_neo/gui/feff_folder_larch.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/gui/media/Citation` & `exafs_neo-2.0.4/exafs_neo/gui/media/Citation`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/gui/media/LICENSE` & `exafs_neo-2.0.4/exafs_neo/gui/media/LICENSE`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/gui/media/icon.png` & `exafs_neo-2.0.4/exafs_neo/gui/media/icon.png`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/helper.py` & `exafs_neo-2.0.4/exafs_neo/helper.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/individual.py` & `exafs_neo-2.0.4/exafs_neo/individual.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/ini_parser.py` & `exafs_neo-2.0.4/exafs_neo/ini_parser.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/input_arg.py` & `exafs_neo-2.0.4/exafs_neo/input_arg.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/neoCrossOver.py` & `exafs_neo-2.0.4/exafs_neo/neoCrossOver.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/neoFilePars.py` & `exafs_neo-2.0.4/exafs_neo/neoFilePars.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/neoMutator.py` & `exafs_neo-2.0.4/exafs_neo/neoMutator.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/neoPars.py` & `exafs_neo-2.0.4/exafs_neo/neoPars.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/neoResult.py` & `exafs_neo-2.0.4/exafs_neo/neoResult.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/neoSelector.py` & `exafs_neo-2.0.4/exafs_neo/neoSelector.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/parser.py` & `exafs_neo-2.0.4/exafs_neo/parser.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/pathObj.py` & `exafs_neo-2.0.4/exafs_neo/pathObj.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/pathrange.py` & `exafs_neo-2.0.4/exafs_neo/pathrange.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/pathrange_file.py` & `exafs_neo-2.0.4/exafs_neo/pathrange_file.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo/utils.py` & `exafs_neo-2.0.4/exafs_neo/utils.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/exafs_neo.egg-info/PKG-INFO` & `exafs_neo-2.0.4/exafs_neo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exafs_neo
-Version: 2.0.3
+Version: 2.0.4
 Summary: exafs_neo AI analysis using GA
 Home-page: https://github.com/laumiulun/EXAFS_Neo
 Download-URL: https://github.com/laumiulun/EXAFS_Neo/tarball/master
 Author: Miu Lun Lau, Jeff Terry, Min Long
 Author-email: andylau@u.boisestate.edu, jterry98@iit.edu, minlong@boisestate.edu
 License: GPLv3
 Keywords: exafs_neo,AI,analysis
@@ -14,17 +14,17 @@
 Requires-Dist: xraylarch
 Requires-Dist: attrs
 Requires-Dist: matplotlib
 Requires-Dist: psutil
 
 # EXAFS Neo
 
-#### Versions: 2.0.2
+#### Versions: 2.0.4
 
-#### Last update: Mar 23, 2024
+#### Last update: Apr 20, 2024
 
 <!-- ![example workflow](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/<WORKFLOW_FILE>/badge.svg) -->
 
 [![Test with Ubuntu, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml)[![Test with Windows, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml)
 
 
 EXAFS Neo utilize Genetic algorithm in fitting Extended X-ray absorption fine structure(EXAFS).
```

### Comparing `exafs_neo-2.0.3/exafs_neo.egg-info/SOURCES.txt` & `exafs_neo-2.0.4/exafs_neo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/setup.py` & `exafs_neo-2.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/tests/test_EXAFS_analysis.py` & `exafs_neo-2.0.4/tests/test_EXAFS_analysis.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/tests/test_exafs_fileobj.py` & `exafs_neo-2.0.4/tests/test_exafs_fileobj.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/tests/test_exafs_pars.py` & `exafs_neo-2.0.4/tests/test_exafs_pars.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/tests/test_exafs_pathObj.py` & `exafs_neo-2.0.4/tests/test_exafs_pathObj.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/tests/test_exafs_pathrange.py` & `exafs_neo-2.0.4/tests/test_exafs_pathrange.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/tests/test_individual.py` & `exafs_neo-2.0.4/tests/test_individual.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/tests/test_ini_parser.py` & `exafs_neo-2.0.4/tests/test_ini_parser.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/tests/test_larchscore.py` & `exafs_neo-2.0.4/tests/test_larchscore.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/tests/test_neo_pop.py` & `exafs_neo-2.0.4/tests/test_neo_pop.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/tests/test_neocrossover.py` & `exafs_neo-2.0.4/tests/test_neocrossover.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.3/tests/test_neomutator.py` & `exafs_neo-2.0.4/tests/test_neomutator.py`

 * *Files identical despite different names*

