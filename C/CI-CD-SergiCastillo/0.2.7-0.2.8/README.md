# Comparing `tmp/CI-CD-SergiCastillo-0.2.7.tar.gz` & `tmp/CI-CD-SergiCastillo-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/CI-CD-SergiCastillo-0.2.7.tar", last modified: Sat Apr 20 17:06:11 2024, max compression
+gzip compressed data, was "dist/CI-CD-SergiCastillo-0.2.8.tar", last modified: Sat Apr 20 17:14:12 2024, max compression
```

## Comparing `CI-CD-SergiCastillo-0.2.7.tar` & `CI-CD-SergiCastillo-0.2.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-20 17:06:11.778282 CI-CD-SergiCastillo-0.2.7/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-20 17:06:11.774282 CI-CD-SergiCastillo-0.2.7/CI_CD_SergiCastillo.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-20 17:06:11.000000 CI-CD-SergiCastillo-0.2.7/CI_CD_SergiCastillo.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      259 2024-04-20 17:06:11.000000 CI-CD-SergiCastillo-0.2.7/CI_CD_SergiCastillo.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-04-20 17:06:11.000000 CI-CD-SergiCastillo-0.2.7/CI_CD_SergiCastillo.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2024-04-20 17:06:11.000000 CI-CD-SergiCastillo-0.2.7/CI_CD_SergiCastillo.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2024-04-20 17:06:11.000000 CI-CD-SergiCastillo-0.2.7/CI_CD_SergiCastillo.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-20 17:06:11.778282 CI-CD-SergiCastillo-0.2.7/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-04-20 17:04:18.000000 CI-CD-SergiCastillo-0.2.7/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-20 17:06:11.778282 CI-CD-SergiCastillo-0.2.7/app/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-04-20 17:05:57.000000 CI-CD-SergiCastillo-0.2.7/app/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3233 2024-04-20 17:04:18.000000 CI-CD-SergiCastillo-0.2.7/app/app.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-04-20 17:06:11.778282 CI-CD-SergiCastillo-0.2.7/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      704 2024-04-20 17:04:18.000000 CI-CD-SergiCastillo-0.2.7/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-20 17:14:12.888198 CI-CD-SergiCastillo-0.2.8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-20 17:14:12.888198 CI-CD-SergiCastillo-0.2.8/CI_CD_SergiCastillo.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-20 17:14:12.000000 CI-CD-SergiCastillo-0.2.8/CI_CD_SergiCastillo.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      259 2024-04-20 17:14:12.000000 CI-CD-SergiCastillo-0.2.8/CI_CD_SergiCastillo.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-04-20 17:14:12.000000 CI-CD-SergiCastillo-0.2.8/CI_CD_SergiCastillo.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2024-04-20 17:14:12.000000 CI-CD-SergiCastillo-0.2.8/CI_CD_SergiCastillo.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2024-04-20 17:14:12.000000 CI-CD-SergiCastillo-0.2.8/CI_CD_SergiCastillo.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-20 17:14:12.888198 CI-CD-SergiCastillo-0.2.8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-04-20 17:12:33.000000 CI-CD-SergiCastillo-0.2.8/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-20 17:14:12.888198 CI-CD-SergiCastillo-0.2.8/app/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-04-20 17:13:58.000000 CI-CD-SergiCastillo-0.2.8/app/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3233 2024-04-20 17:12:33.000000 CI-CD-SergiCastillo-0.2.8/app/app.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-04-20 17:14:12.888198 CI-CD-SergiCastillo-0.2.8/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      704 2024-04-20 17:12:33.000000 CI-CD-SergiCastillo-0.2.8/setup.py
```

### Comparing `CI-CD-SergiCastillo-0.2.7/app/app.py` & `CI-CD-SergiCastillo-0.2.8/app/app.py`

 * *Files identical despite different names*

### Comparing `CI-CD-SergiCastillo-0.2.7/setup.py` & `CI-CD-SergiCastillo-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from setuptools import setup, find_packages
 
 # Obtener la versión actual del paquete
-version = '0.2.7'
+version = '0.2.8'
 
 # Eliminar el archivo .tar.gz existente si ya está presente
 if os.path.exists(f"dist/CI-CD-SergiCastillo-{version}.tar.gz"):
     os.remove(f"dist/CI-CD-SergiCastillo-{version}.tar.gz")
 
 setup(
     name='CI-CD-SergiCastillo',
```

