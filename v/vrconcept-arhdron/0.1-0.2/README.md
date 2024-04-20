# Comparing `tmp/vrconcept_arhdron-0.1.tar.gz` & `tmp/vrconcept_arhdron-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vrconcept_arhdron-0.1.tar", last modified: Mon Apr  1 15:58:07 2024, max compression
+gzip compressed data, was "vrconcept_arhdron-0.2.tar", last modified: Sat Apr 20 13:52:57 2024, max compression
```

## Comparing `vrconcept_arhdron-0.1.tar` & `vrconcept_arhdron-0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 15:58:07.866861 vrconcept_arhdron-0.1/
--rw-rw-rw-   0        0        0      139 2024-04-01 15:58:07.866861 vrconcept_arhdron-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      316 2024-04-01 15:54:25.000000 vrconcept_arhdron-0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-01 15:58:07.867945 vrconcept_arhdron-0.1/setup.cfg
--rw-rw-rw-   0        0        0      238 2024-04-01 15:55:45.000000 vrconcept_arhdron-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 15:58:07.857715 vrconcept_arhdron-0.1/vrconcept_arhdron/
--rw-rw-rw-   0        0        0      827 2024-04-01 15:47:51.000000 vrconcept_arhdron-0.1/vrconcept_arhdron/Client.py
--rw-rw-rw-   0        0        0     8917 2024-04-01 14:44:18.000000 vrconcept_arhdron-0.1/vrconcept_arhdron/Data.py
--rw-rw-rw-   0        0        0      114 2024-04-01 14:44:59.000000 vrconcept_arhdron-0.1/vrconcept_arhdron/Game.py
--rw-rw-rw-   0        0        0       74 2024-04-01 14:48:09.000000 vrconcept_arhdron-0.1/vrconcept_arhdron/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 15:58:07.865745 vrconcept_arhdron-0.1/vrconcept_arhdron.egg-info/
--rw-rw-rw-   0        0        0      139 2024-04-01 15:58:07.000000 vrconcept_arhdron-0.1/vrconcept_arhdron.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-04-01 15:58:07.000000 vrconcept_arhdron-0.1/vrconcept_arhdron.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 15:58:07.000000 vrconcept_arhdron-0.1/vrconcept_arhdron.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-01 15:14:33.000000 vrconcept_arhdron-0.1/vrconcept_arhdron.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2024-04-01 15:58:07.000000 vrconcept_arhdron-0.1/vrconcept_arhdron.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 13:52:57.790580 vrconcept_arhdron-0.2/
+-rw-rw-rw-   0        0        0      139 2024-04-20 13:52:57.790580 vrconcept_arhdron-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2024-04-01 15:54:25.000000 vrconcept_arhdron-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-20 13:52:57.792734 vrconcept_arhdron-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      238 2024-04-20 13:47:03.000000 vrconcept_arhdron-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:52:57.768114 vrconcept_arhdron-0.2/vrconcept_arhdron/
+-rw-rw-rw-   0        0        0     1871 2024-04-20 13:47:03.000000 vrconcept_arhdron-0.2/vrconcept_arhdron/Capture.py
+-rw-rw-rw-   0        0        0      827 2024-04-01 15:47:51.000000 vrconcept_arhdron-0.2/vrconcept_arhdron/Client.py
+-rw-rw-rw-   0        0        0     8917 2024-04-01 14:44:18.000000 vrconcept_arhdron-0.2/vrconcept_arhdron/Data.py
+-rw-rw-rw-   0        0        0      114 2024-04-01 14:44:59.000000 vrconcept_arhdron-0.2/vrconcept_arhdron/Game.py
+-rw-rw-rw-   0        0        0      104 2024-04-20 13:47:03.000000 vrconcept_arhdron-0.2/vrconcept_arhdron/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:52:57.788073 vrconcept_arhdron-0.2/vrconcept_arhdron.egg-info/
+-rw-rw-rw-   0        0        0      139 2024-04-20 13:52:57.000000 vrconcept_arhdron-0.2/vrconcept_arhdron.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2024-04-20 13:52:57.000000 vrconcept_arhdron-0.2/vrconcept_arhdron.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 13:52:57.000000 vrconcept_arhdron-0.2/vrconcept_arhdron.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-01 15:14:33.000000 vrconcept_arhdron-0.2/vrconcept_arhdron.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2024-04-20 13:52:57.000000 vrconcept_arhdron-0.2/vrconcept_arhdron.egg-info/top_level.txt
```

### Comparing `vrconcept_arhdron-0.1/vrconcept_arhdron/Client.py` & `vrconcept_arhdron-0.2/vrconcept_arhdron/Client.py`

 * *Files identical despite different names*

### Comparing `vrconcept_arhdron-0.1/vrconcept_arhdron/Data.py` & `vrconcept_arhdron-0.2/vrconcept_arhdron/Data.py`

 * *Files identical despite different names*

