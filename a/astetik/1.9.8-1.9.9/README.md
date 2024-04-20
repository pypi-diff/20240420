# Comparing `tmp/astetik-1.9.8.tar.gz` & `tmp/astetik-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/astetik-1.9.8.tar", last modified: Thu Mar  7 12:47:40 2019, max compression
+gzip compressed data, was "dist/astetik-1.9.9.tar", last modified: Sat Sep  7 10:38:11 2019, max compression
```

## Comparing `astetik-1.9.8.tar` & `astetik-1.9.9.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-07 12:47:40.000000 astetik-1.9.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6786 2019-03-07 12:46:05.000000 astetik-1.9.8/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-07 12:47:40.000000 astetik-1.9.8/astetik.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2019-03-07 12:47:40.000000 astetik-1.9.8/astetik.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1302 2019-03-07 12:47:40.000000 astetik-1.9.8/astetik.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-07 12:47:40.000000 astetik-1.9.8/astetik.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1262 2019-03-07 12:47:40.000000 astetik-1.9.8/astetik.egg-info/SOURCES.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-07 12:47:40.000000 astetik-1.9.8/astetik/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-07 12:47:40.000000 astetik-1.9.8/astetik/style/
--rw-rw-r--   0 travis    (2000) travis    (2000)      206 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/style/random_colors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      568 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/style/formats.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/style/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      161 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/style/sizer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4466 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/style/color_picker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1218 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/style/titles.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2418 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/style/template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4182 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/style/style.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-07 12:47:40.000000 astetik-1.9.8/astetik/tables/
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/tables/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1363 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/tables/text.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2955 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/tables/table.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1049 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-07 12:47:40.000000 astetik-1.9.8/astetik/plots/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4072 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/strip.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4927 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/world.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1770 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/animate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4128 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/scat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4193 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/swarm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4514 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/compare.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3979 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/hist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5037 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/overlap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6922 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/line.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3964 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/regs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4040 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/bargrid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3482 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/kde.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3482 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/grid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3707 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/violin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3908 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/bartwo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4941 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/roc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4769 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/multikde.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4877 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/corr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3727 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/multicount.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3290 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/count.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4095 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/bar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3742 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/box.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3830 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/plots/pie.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-07 12:47:40.000000 astetik-1.9.8/astetik/extras/
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/extras/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-07 12:47:40.000000 astetik-1.9.8/astetik/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)      341 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/utils/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3167 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/utils/datetime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      164 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/utils/load_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7955 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/utils/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      467 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/utils/gui.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4630 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/utils/transform.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      550 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/utils/outliers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      528 2019-03-07 12:46:05.000000 astetik-1.9.8/astetik/utils/country_code.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3455 2019-03-07 12:46:05.000000 astetik-1.9.8/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-03-07 12:47:40.000000 astetik-1.9.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1302 2019-03-07 12:47:40.000000 astetik-1.9.8/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-07 10:38:11.000000 astetik-1.9.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6786 2019-09-07 10:36:39.000000 astetik-1.9.9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-07 10:38:11.000000 astetik-1.9.9/astetik.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2019-09-07 10:38:11.000000 astetik-1.9.9/astetik.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1302 2019-09-07 10:38:11.000000 astetik-1.9.9/astetik.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-09-07 10:38:11.000000 astetik-1.9.9/astetik.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1306 2019-09-07 10:38:11.000000 astetik-1.9.9/astetik.egg-info/SOURCES.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-07 10:38:11.000000 astetik-1.9.9/astetik/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-07 10:38:11.000000 astetik-1.9.9/astetik/style/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      206 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/style/random_colors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      847 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/style/formats.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/style/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      161 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/style/sizer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4466 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/style/color_picker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1218 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/style/titles.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2418 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/style/template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4182 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/style/style.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-07 10:38:11.000000 astetik-1.9.9/astetik/tables/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/tables/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1363 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/tables/text.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2955 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/tables/table.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1131 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-07 10:38:11.000000 astetik-1.9.9/astetik/plots/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4084 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/strip.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4954 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/world.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1770 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/animate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4086 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/scat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4204 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/swarm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4514 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/compare.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3993 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/hist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5049 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/overlap.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6924 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/line.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3977 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/regs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      410 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/oned.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4040 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/bargrid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      638 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/twod.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3494 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/kde.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3482 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/grid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3719 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/violin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3908 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/bartwo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4941 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/roc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4769 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/multikde.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4802 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/corr.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3727 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/multicount.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3292 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/count.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4095 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/bar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3754 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/box.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3830 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/plots/pie.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-07 10:38:11.000000 astetik-1.9.9/astetik/extras/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/extras/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-07 10:38:11.000000 astetik-1.9.9/astetik/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      341 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/utils/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3167 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/utils/datetime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      164 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/utils/load_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7955 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/utils/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      471 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/utils/gui.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4630 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/utils/transform.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      550 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/utils/outliers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      528 2019-09-07 10:36:39.000000 astetik-1.9.9/astetik/utils/country_code.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3451 2019-09-07 10:36:39.000000 astetik-1.9.9/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-09-07 10:38:11.000000 astetik-1.9.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1302 2019-09-07 10:38:11.000000 astetik-1.9.9/PKG-INFO
```

### Comparing `astetik-1.9.8/README.md` & `astetik-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/astetik.egg-info/PKG-INFO` & `astetik-1.9.9/astetik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: astetik
-Version: 1.9.8
+Version: 1.9.9
 Summary: Astetik data visualization and reporting library
 Home-page: http://mikkokotila.com
 Author: Mikko Kotila
 Author-email: mailme@mikkokotila.com
 Maintainer: Mikko Kotila
 Maintainer-email: mailme@mikkokotila.com
 License: MIT
```

### Comparing `astetik-1.9.8/astetik.egg-info/SOURCES.txt` & `astetik-1.9.9/astetik.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 astetik/plots/count.py
 astetik/plots/grid.py
 astetik/plots/hist.py
 astetik/plots/kde.py
 astetik/plots/line.py
 astetik/plots/multicount.py
 astetik/plots/multikde.py
+astetik/plots/oned.py
 astetik/plots/overlap.py
 astetik/plots/pie.py
 astetik/plots/regs.py
 astetik/plots/roc.py
 astetik/plots/scat.py
 astetik/plots/strip.py
 astetik/plots/swarm.py
+astetik/plots/twod.py
 astetik/plots/violin.py
 astetik/plots/world.py
 astetik/style/__init__.py
 astetik/style/color_picker.py
 astetik/style/formats.py
 astetik/style/random_colors.py
 astetik/style/sizer.py
```

### Comparing `astetik-1.9.8/astetik/style/color_picker.py` & `astetik-1.9.9/astetik/style/color_picker.py`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/astetik/style/titles.py` & `astetik-1.9.9/astetik/style/titles.py`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/astetik/style/template.py` & `astetik-1.9.9/astetik/style/template.py`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/astetik/style/style.py` & `astetik-1.9.9/astetik/style/style.py`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/astetik/tables/text.py` & `astetik-1.9.9/astetik/tables/text.py`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/astetik/tables/table.py` & `astetik-1.9.9/astetik/tables/table.py`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/astetik/__init__.py` & `astetik-1.9.9/astetik/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 from .plots.bartwo import bartwo
 from .plots.animate import Animation
 from .plots.world import world
 from .plots.regs import regs
 from .plots.roc import roc
 # from .plots.words import words
 
+from .utils.gui import toggle as toggle
+from .utils.gui import warning as warning
 
 # TABLES
 from .tables.table import table
 from .tables.text import text
 # from .tables.timeseries import timeseries
 
 try:
@@ -46,8 +48,8 @@
     pass
 
 try:
     del utils
 except:
     pass
 
-__version__ = "1.9.8"
+__version__ = "1.9.9"
```

### Comparing `astetik-1.9.8/astetik/plots/strip.py` & `astetik-1.9.9/astetik/plots/strip.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,13 +138,13 @@
     if x_scale != 'linear' or y_scale != 'linear':
         _scaler(p, x_scale, y_scale)
 
     if x_limit != None or y_limit != None:
         _limiter(data=data, x=x, y=y, x_limit=None, y_limit=y_limit)
 
     # FOOTER STARTS >>>
-    _thousand_sep(p, ax)
+    _thousand_sep(p, ax, data, x, y)
     _titles(title, sub_title=sub_title)
     _footer(p, x_label, y_label, legend, n, save)
 
     p.spines['bottom'].set_color('black')
     p.set_xticklabels(order, rotation=90)
```

### Comparing `astetik-1.9.8/astetik/plots/world.py` & `astetik-1.9.9/astetik/plots/world.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,8 +152,8 @@
                                    boundaries=bins,
                                    orientation='horizontal')
 
     cb.ax.set_xticklabels([str(round(i, 1)) for i in bins], rotation=45, ha='right')
 
     plt.annotate(descripton, xy=(-.8, -3.2), size=14, xycoords='axes fraction')
 
-    _thousand_sep(p, ax)
+    _thousand_sep(p, ax, data, area_col, value_col)
```

### Comparing `astetik-1.9.8/astetik/plots/animate.py` & `astetik-1.9.9/astetik/plots/animate.py`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/astetik/plots/scat.py` & `astetik-1.9.9/astetik/plots/scat.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,11 +147,9 @@
         _scaler(p, x_scale, y_scale)
 
     if x_limit != None or y_limit != None:
         _limiter(data=data, x=x, y=y, x_limit=x_limit, y_limit=y_limit)
 
     # START OF TITLES >>>
     _titles(title, sub_title=sub_title)
-    #_thousand_sep(p, ax)
+    _thousand_sep(p, ax, data, x, y)
     _footer(p, x_label, y_label, legend, n, save)
-
-    #ax.xaxis.set_major_locator(plt.MaxNLocator(5))
```

### Comparing `astetik-1.9.8/astetik/plots/swarm.py` & `astetik-1.9.9/astetik/plots/swarm.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     '''SWARM PLOT
     This is similar to scatter plot, in the sense that overlapping observations
     are avoided (each sample will be seen as a dot), but observations are
     grouped based on 'x'.
 
     NOTE: this plot takes time to draw, so if your sample is tens or hundreds
           of thousands of observations, be patient. Or if it's not that important
-          that observations do not overlap, try strip() instead. 
+          that observations do not overlap, try strip() instead.
 
     Inputs: 2 to 3
     Features: 1 continuous and 1 or 2 categoricals
 
     1. USE
     ======
     ast.violin(data=patients,
@@ -143,11 +143,11 @@
         _limiter(data=data, x=x, y=y, x_limit=None, y_limit=y_limit)
     # <<< SCALING AND LIMITS ENDS
 
     # START OF TITLES >>>
     _titles(title, sub_title=sub_title)
     # <<< END OF TITLES
 
-    _thousand_sep(p, ax)
+    _thousand_sep(p, ax, data, x, y)
     _footer(p, x_label, y_label, legend, n, save)
     # <<< FOOTER ENDS
     p.set_xticklabels(order, rotation=90)
```

### Comparing `astetik-1.9.8/astetik/plots/compare.py` & `astetik-1.9.9/astetik/plots/compare.py`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/astetik/plots/hist.py` & `astetik-1.9.9/astetik/plots/hist.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     y_limit :: int or list with two ints
 
     outliers :: Remove outliers using either 'zscore' or 'iqr'
 
     '''
     warnings.simplefilter("ignore")
 
-    
+
     if bins == True:
         if isinstance(x, list) is False:
             bins = int(len(data[x].unique()) / 10) + 5
         else:
             bins = 10
 
     if dropna is True:
@@ -148,10 +148,10 @@
     if x_scale != 'linear' or y_scale != 'linear':
         _scaler(p, x_scale, y_scale)
 
     if x_limit != None or y_limit != None:
         _limiter(data=data, x=x, y=x, x_limit=x_limit, y_limit=y_limit)
 
     # HEADER
-    _thousand_sep(p, ax)
+    _thousand_sep(p, ax, data, x[0], None)
     _titles(title, sub_title)
     _footer(p, x_label, y_label, save=save)
```

### Comparing `astetik-1.9.8/astetik/plots/overlap.py` & `astetik-1.9.9/astetik/plots/overlap.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,10 +170,10 @@
         y_patch = mpatches.Patch(color=palette[1], label=y)
         ax.legend(handles=[x_patch, y_patch], ncol=1, loc="upper right", frameon=True)
 
     ax.set(ylabel=y_label, xlabel=x_label)
     sns.despine(bottom=True)
     ax.xaxis.set_major_locator(plt.MaxNLocator(5))
 
-    _thousand_sep(p, ax)
+    _thousand_sep(p, ax, data, x, y)
     if len(title) + len(sub_title) < 0:
         _titles(title, sub_title=sub_title)
```

### Comparing `astetik-1.9.8/astetik/plots/line.py` & `astetik-1.9.9/astetik/plots/line.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,15 @@
         date_handler(data[y], ax, time_frame)
 
     # LIMITS
     if x_limit != None or y_limit != None:
         _limiter(data=data, x=x, y='_R_E_S_', x_limit=None, y_limit=y_limit)
 
     # HEADER
-    _thousand_sep(p, ax, x_sep=False)
+    _thousand_sep(p, ax, data, x[0], y)
     _titles(title, sub_title=sub_title)
     _footer(p, x_label, y_label, save=save)
 
     if legend != False:
         if legend_labels != None:
             x = legend_labels
         plt.legend(x, loc=1, ncol=1, bbox_to_anchor=(1.35, 1.0))
```

### Comparing `astetik-1.9.8/astetik/plots/regs.py` & `astetik-1.9.9/astetik/plots/regs.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,11 +136,12 @@
         _scaler(p, x_scale, y_scale)
 
     if x_limit != None or y_limit != None:
         _limiter(data=data, x=x, y=y, x_limit=x_limit, y_limit=y_limit)
 
     # START OF TITLES >>>
     _titles(title, sub_title=sub_title)
-    _thousand_sep(p, ax)
+
+    _thousand_sep(p, ax, data, x, y)
     _footer(p=p, xlabel=x_label, ylabel=y_label, legend=False, n=1, save=save)
 
     ax.xaxis.set_major_locator(plt.MaxNLocator(5))
```

### Comparing `astetik-1.9.8/astetik/plots/bargrid.py` & `astetik-1.9.9/astetik/plots/bargrid.py`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/astetik/plots/kde.py` & `astetik-1.9.9/astetik/plots/kde.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,10 +130,10 @@
     if x_scale != 'linear' or y_scale != 'linear':
         _scaler(p, x_scale, y_scale)
 
     if x_limit != None or y_limit != None:
         _limiter(data=data, x=x, y=y, x_limit=x_limit, y_limit=y_limit)
 
     # FOOTER
-    _thousand_sep(p, ax)
+    _thousand_sep(p, ax, data, x, y)
     _titles(title, sub_title=sub_title)
     _footer(p, x_label, y_label, save=save)
```

### Comparing `astetik-1.9.8/astetik/plots/grid.py` & `astetik-1.9.9/astetik/plots/grid.py`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/astetik/plots/violin.py` & `astetik-1.9.9/astetik/plots/violin.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,13 +128,13 @@
     if x_scale != 'linear' or y_scale != 'linear':
         _scaler(p, x_scale, y_scale)
     if x_limit != None or y_limit != None:
         _limiter(data=data, x=x, y=y, x_limit=None, y_limit=y_limit)
     # <<< SCALING AND LIMITS ENDS
 
     # FOOTER STARTS >>>
-    _thousand_sep(p, ax)
+    _thousand_sep(p, ax, data, x, y)
     _titles(title, sub_title=sub_title)
     _footer(p, x_label, y_label, legend, 2, save)
 
     p.spines['bottom'].set_color('black')
     # <<< FOOTER ENDS
```

### Comparing `astetik-1.9.8/astetik/plots/bartwo.py` & `astetik-1.9.9/astetik/plots/bartwo.py`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/astetik/plots/roc.py` & `astetik-1.9.9/astetik/plots/roc.py`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/astetik/plots/multikde.py` & `astetik-1.9.9/astetik/plots/multikde.py`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/astetik/plots/corr.py` & `astetik-1.9.9/astetik/plots/corr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import warnings
 warnings.filterwarnings("ignore")
 
 import numpy as np
-import matplotlib
-matplotlib.use('Agg')
-# ENDS #
+
 import matplotlib.pyplot as plt
 import seaborn as sns
 
-
-
 from ..style.formats import _thousand_sep
 from ..style.titles import _titles
 from ..style.template import _header, _footer
 
 
 def corr(data,
          corr_method='spearman',
@@ -164,13 +160,12 @@
                     mask=mask,
                     linewidths=line_width,
                     linecolor=line_color,
                     cmap=palette,
                     annot=annot)
 
     # HEADER
-    _thousand_sep(p, ax)
     _titles(title, sub_title=sub_title)
     _footer(p, x_label, y_label, save=save, tight=False, despine=False)
 
     p.set_xticklabels(data, rotation=90)
     p.set_yticklabels(data, rotation=0)
```

### Comparing `astetik-1.9.8/astetik/plots/multicount.py` & `astetik-1.9.9/astetik/plots/multicount.py`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/astetik/plots/count.py` & `astetik-1.9.9/astetik/plots/count.py`

 * *Files 10% similar despite different names*

```diff
@@ -116,11 +116,11 @@
                        kind='count',
                        legend=legend,
                        legend_out=False,
                        order=sort)
 
     # FOOTER
     _titles(title, sub_title)
-    _thousand_sep(p, p.ax, y_sep=False)
+    _thousand_sep(p, p.ax, data, x, None)
     _footer(p, x_label, y_label, save=save)
 
     p.set_xticklabels(None, rotation=90)
```

### Comparing `astetik-1.9.8/astetik/plots/bar.py` & `astetik-1.9.9/astetik/plots/bar.py`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/astetik/plots/box.py` & `astetik-1.9.9/astetik/plots/box.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,11 +136,11 @@
     # <<< SCALING AND LIMITS ENDS
 
     if hue == None:
         legend = False
 
     # FOOTER
     _titles(title, sub_title)
-    _thousand_sep(p, ax)
+    _thousand_sep(p, ax, data, x, y)
     _footer(p, x_label, y_label, legend, n, save=save)
 
     p.spines['bottom'].set_color('black')
```

### Comparing `astetik-1.9.8/astetik/plots/pie.py` & `astetik-1.9.9/astetik/plots/pie.py`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/astetik/utils/datetime.py` & `astetik-1.9.9/astetik/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/astetik/utils/utils.py` & `astetik-1.9.9/astetik/utils/utils.py`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/astetik/utils/transform.py` & `astetik-1.9.9/astetik/utils/transform.py`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/astetik/utils/outliers.py` & `astetik-1.9.9/astetik/utils/outliers.py`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/astetik/utils/country_code.py` & `astetik-1.9.9/astetik/utils/country_code.py`

 * *Files identical despite different names*

### Comparing `astetik-1.9.8/setup.py` & `astetik-1.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 DISTNAME = 'astetik'
 MAINTAINER = 'Mikko Kotila'
 MAINTAINER_EMAIL = 'mailme@mikkokotila.com'
 URL = 'http://mikkokotila.com'
 LICENSE = 'MIT'
 DOWNLOAD_URL = 'https://github.com/mikkokotila/pretty'
-VERSION = '1.9.8'
+VERSION = '1.9.9'
 
 try:
     from setuptools import setup
     _has_setuptools = True
 except ImportError:
     from distutils.core import setup
 
@@ -67,15 +67,15 @@
         import statsmodels
     except ImportError:
         install_requires.append('statsmodels')
     try:
         import sklearn
     except ImportError:
         install_requires.append('sklearn')
-    
+
     return install_requires
 
 if __name__ == "__main__":
 
     install_requires = check_dependencies()
 
     setup(name=DISTNAME,
```

### Comparing `astetik-1.9.8/PKG-INFO` & `astetik-1.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: astetik
-Version: 1.9.8
+Version: 1.9.9
 Summary: Astetik data visualization and reporting library
 Home-page: http://mikkokotila.com
 Author: Mikko Kotila
 Author-email: mailme@mikkokotila.com
 Maintainer: Mikko Kotila
 Maintainer-email: mailme@mikkokotila.com
 License: MIT
```

