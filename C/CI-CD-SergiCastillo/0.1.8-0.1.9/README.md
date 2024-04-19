# Comparing `tmp/CI-CD-SergiCastillo-0.1.8.tar.gz` & `tmp/CI-CD-SergiCastillo-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/CI-CD-SergiCastillo-0.1.8.tar", last modified: Thu Apr 18 20:22:29 2024, max compression
+gzip compressed data, was "dist/CI-CD-SergiCastillo-0.1.9.tar", last modified: Thu Apr 18 20:25:19 2024, max compression
```

## Comparing `CI-CD-SergiCastillo-0.1.8.tar` & `CI-CD-SergiCastillo-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-18 20:22:29.640025 CI-CD-SergiCastillo-0.1.8/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-18 20:22:29.640025 CI-CD-SergiCastillo-0.1.8/CI_CD_SergiCastillo.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-18 20:22:29.000000 CI-CD-SergiCastillo-0.1.8/CI_CD_SergiCastillo.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      259 2024-04-18 20:22:29.000000 CI-CD-SergiCastillo-0.1.8/CI_CD_SergiCastillo.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-04-18 20:22:29.000000 CI-CD-SergiCastillo-0.1.8/CI_CD_SergiCastillo.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2024-04-18 20:22:29.000000 CI-CD-SergiCastillo-0.1.8/CI_CD_SergiCastillo.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2024-04-18 20:22:29.000000 CI-CD-SergiCastillo-0.1.8/CI_CD_SergiCastillo.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-18 20:22:29.640025 CI-CD-SergiCastillo-0.1.8/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-04-18 20:21:22.000000 CI-CD-SergiCastillo-0.1.8/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-18 20:22:29.640025 CI-CD-SergiCastillo-0.1.8/app/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-04-18 20:22:17.000000 CI-CD-SergiCastillo-0.1.8/app/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3678 2024-04-18 20:21:22.000000 CI-CD-SergiCastillo-0.1.8/app/app.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-04-18 20:22:29.640025 CI-CD-SergiCastillo-0.1.8/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      462 2024-04-18 20:21:22.000000 CI-CD-SergiCastillo-0.1.8/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-18 20:25:19.702783 CI-CD-SergiCastillo-0.1.9/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-18 20:25:19.702783 CI-CD-SergiCastillo-0.1.9/CI_CD_SergiCastillo.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-18 20:25:19.000000 CI-CD-SergiCastillo-0.1.9/CI_CD_SergiCastillo.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      259 2024-04-18 20:25:19.000000 CI-CD-SergiCastillo-0.1.9/CI_CD_SergiCastillo.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-04-18 20:25:19.000000 CI-CD-SergiCastillo-0.1.9/CI_CD_SergiCastillo.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2024-04-18 20:25:19.000000 CI-CD-SergiCastillo-0.1.9/CI_CD_SergiCastillo.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2024-04-18 20:25:19.000000 CI-CD-SergiCastillo-0.1.9/CI_CD_SergiCastillo.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-18 20:25:19.702783 CI-CD-SergiCastillo-0.1.9/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-04-18 20:24:08.000000 CI-CD-SergiCastillo-0.1.9/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-18 20:25:19.702783 CI-CD-SergiCastillo-0.1.9/app/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-04-18 20:25:07.000000 CI-CD-SergiCastillo-0.1.9/app/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3678 2024-04-18 20:24:08.000000 CI-CD-SergiCastillo-0.1.9/app/app.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-04-18 20:25:19.702783 CI-CD-SergiCastillo-0.1.9/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      462 2024-04-18 20:24:08.000000 CI-CD-SergiCastillo-0.1.9/setup.py
```

### Comparing `CI-CD-SergiCastillo-0.1.8/app/app.py` & `CI-CD-SergiCastillo-0.1.9/app/app.py`

 * *Files identical despite different names*

