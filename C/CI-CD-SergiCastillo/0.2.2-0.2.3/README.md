# Comparing `tmp/CI-CD-SergiCastillo-0.2.2.tar.gz` & `tmp/CI-CD-SergiCastillo-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/CI-CD-SergiCastillo-0.2.2.tar", last modified: Sat Apr 20 15:32:55 2024, max compression
+gzip compressed data, was "dist/CI-CD-SergiCastillo-0.2.3.tar", last modified: Sat Apr 20 15:59:39 2024, max compression
```

## Comparing `CI-CD-SergiCastillo-0.2.2.tar` & `CI-CD-SergiCastillo-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-20 15:32:55.208944 CI-CD-SergiCastillo-0.2.2/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-20 15:32:55.208944 CI-CD-SergiCastillo-0.2.2/CI_CD_SergiCastillo.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-20 15:32:55.000000 CI-CD-SergiCastillo-0.2.2/CI_CD_SergiCastillo.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      259 2024-04-20 15:32:55.000000 CI-CD-SergiCastillo-0.2.2/CI_CD_SergiCastillo.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-04-20 15:32:55.000000 CI-CD-SergiCastillo-0.2.2/CI_CD_SergiCastillo.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2024-04-20 15:32:55.000000 CI-CD-SergiCastillo-0.2.2/CI_CD_SergiCastillo.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2024-04-20 15:32:55.000000 CI-CD-SergiCastillo-0.2.2/CI_CD_SergiCastillo.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-20 15:32:55.208944 CI-CD-SergiCastillo-0.2.2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-04-20 15:30:33.000000 CI-CD-SergiCastillo-0.2.2/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-20 15:32:55.208944 CI-CD-SergiCastillo-0.2.2/app/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-04-20 15:32:39.000000 CI-CD-SergiCastillo-0.2.2/app/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3233 2024-04-20 15:30:33.000000 CI-CD-SergiCastillo-0.2.2/app/app.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-04-20 15:32:55.208944 CI-CD-SergiCastillo-0.2.2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      704 2024-04-20 15:30:33.000000 CI-CD-SergiCastillo-0.2.2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-20 15:59:38.994642 CI-CD-SergiCastillo-0.2.3/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-20 15:59:38.994642 CI-CD-SergiCastillo-0.2.3/CI_CD_SergiCastillo.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-20 15:59:38.000000 CI-CD-SergiCastillo-0.2.3/CI_CD_SergiCastillo.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      259 2024-04-20 15:59:38.000000 CI-CD-SergiCastillo-0.2.3/CI_CD_SergiCastillo.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-04-20 15:59:38.000000 CI-CD-SergiCastillo-0.2.3/CI_CD_SergiCastillo.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2024-04-20 15:59:38.000000 CI-CD-SergiCastillo-0.2.3/CI_CD_SergiCastillo.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2024-04-20 15:59:38.000000 CI-CD-SergiCastillo-0.2.3/CI_CD_SergiCastillo.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-20 15:59:38.994642 CI-CD-SergiCastillo-0.2.3/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-04-20 15:57:37.000000 CI-CD-SergiCastillo-0.2.3/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-20 15:59:38.994642 CI-CD-SergiCastillo-0.2.3/app/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-04-20 15:59:24.000000 CI-CD-SergiCastillo-0.2.3/app/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3233 2024-04-20 15:57:37.000000 CI-CD-SergiCastillo-0.2.3/app/app.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-04-20 15:59:38.994642 CI-CD-SergiCastillo-0.2.3/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      704 2024-04-20 15:57:37.000000 CI-CD-SergiCastillo-0.2.3/setup.py
```

### Comparing `CI-CD-SergiCastillo-0.2.2/app/app.py` & `CI-CD-SergiCastillo-0.2.3/app/app.py`

 * *Files identical despite different names*

### Comparing `CI-CD-SergiCastillo-0.2.2/setup.py` & `CI-CD-SergiCastillo-0.2.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from setuptools import setup, find_packages
 
 # Obtener la versión actual del paquete
-version = '0.2.2'
+version = '0.2.3'
 
 # Eliminar el archivo .tar.gz existente si ya está presente
 if os.path.exists(f"dist/CI-CD-SergiCastillo-{version}.tar.gz"):
     os.remove(f"dist/CI-CD-SergiCastillo-{version}.tar.gz")
 
 setup(
     name='CI-CD-SergiCastillo',
```

