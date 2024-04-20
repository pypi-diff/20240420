# Comparing `tmp/HimDonHaiDraws-0.1.tar.gz` & `tmp/HimDonHaiDraws-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HimDonHaiDraws-0.1.tar", last modified: Sat Apr 20 18:29:33 2024, max compression
+gzip compressed data, was "HimDonHaiDraws-0.2.tar", last modified: Sat Apr 20 18:33:27 2024, max compression
```

## Comparing `HimDonHaiDraws-0.1.tar` & `HimDonHaiDraws-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 18:29:33.673506 HimDonHaiDraws-0.1/
-drwxrwxrwx   0        0        0        0 2024-04-20 18:29:33.635804 HimDonHaiDraws-0.1/HimDonHaiDraws/
--rw-rw-rw-   0        0        0       23 2024-04-20 16:34:18.000000 HimDonHaiDraws-0.1/HimDonHaiDraws/__init__.py
--rw-rw-rw-   0        0        0     2294 2024-04-20 18:28:36.000000 HimDonHaiDraws-0.1/HimDonHaiDraws/main.py
-drwxrwxrwx   0        0        0        0 2024-04-20 18:29:33.671519 HimDonHaiDraws-0.1/HimDonHaiDraws.egg-info/
--rw-rw-rw-   0        0        0       59 2024-04-20 18:29:33.000000 HimDonHaiDraws-0.1/HimDonHaiDraws.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-04-20 18:29:33.000000 HimDonHaiDraws-0.1/HimDonHaiDraws.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 18:29:33.000000 HimDonHaiDraws-0.1/HimDonHaiDraws.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-20 18:29:33.000000 HimDonHaiDraws-0.1/HimDonHaiDraws.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-20 18:29:33.000000 HimDonHaiDraws-0.1/HimDonHaiDraws.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       59 2024-04-20 18:29:33.672515 HimDonHaiDraws-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-20 16:16:22.000000 HimDonHaiDraws-0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-20 18:29:33.673506 HimDonHaiDraws-0.1/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-04-20 18:28:40.000000 HimDonHaiDraws-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 18:33:27.630860 HimDonHaiDraws-0.2/
+drwxrwxrwx   0        0        0        0 2024-04-20 18:33:27.612794 HimDonHaiDraws-0.2/HimDonHaiDraws/
+-rw-rw-rw-   0        0        0       22 2024-04-20 18:32:50.000000 HimDonHaiDraws-0.2/HimDonHaiDraws/__init__.py
+-rw-rw-rw-   0        0        0     2294 2024-04-20 18:28:36.000000 HimDonHaiDraws-0.2/HimDonHaiDraws/main.py
+drwxrwxrwx   0        0        0        0 2024-04-20 18:33:27.628854 HimDonHaiDraws-0.2/HimDonHaiDraws.egg-info/
+-rw-rw-rw-   0        0        0       59 2024-04-20 18:33:27.000000 HimDonHaiDraws-0.2/HimDonHaiDraws.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2024-04-20 18:33:27.000000 HimDonHaiDraws-0.2/HimDonHaiDraws.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 18:33:27.000000 HimDonHaiDraws-0.2/HimDonHaiDraws.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-20 18:33:27.000000 HimDonHaiDraws-0.2/HimDonHaiDraws.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-20 18:33:27.000000 HimDonHaiDraws-0.2/HimDonHaiDraws.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       59 2024-04-20 18:33:27.629853 HimDonHaiDraws-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-20 16:16:22.000000 HimDonHaiDraws-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-20 18:33:27.630860 HimDonHaiDraws-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-04-20 18:32:39.000000 HimDonHaiDraws-0.2/setup.py
```

### Comparing `HimDonHaiDraws-0.1/HimDonHaiDraws/main.py` & `HimDonHaiDraws-0.2/HimDonHaiDraws/main.py`

 * *Files identical despite different names*

