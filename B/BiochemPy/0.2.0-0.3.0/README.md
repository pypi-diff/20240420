# Comparing `tmp/BiochemPy-0.2.0.tar.gz` & `tmp/BiochemPy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BiochemPy-0.2.0.tar", last modified: Sun Apr 14 09:54:56 2024, max compression
+gzip compressed data, was "BiochemPy-0.3.0.tar", last modified: Sat Apr 20 21:44:24 2024, max compression
```

## Comparing `BiochemPy-0.2.0.tar` & `BiochemPy-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:54:56.043964 BiochemPy-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:54:56.043964 BiochemPy-0.2.0/BiochemPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-14 09:54:56.000000 BiochemPy-0.2.0/BiochemPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-14 09:54:56.000000 BiochemPy-0.2.0/BiochemPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 09:54:56.000000 BiochemPy-0.2.0/BiochemPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 09:54:56.000000 BiochemPy-0.2.0/BiochemPy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-14 09:54:45.000000 BiochemPy-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-14 09:54:56.043964 BiochemPy-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 09:54:56.043964 BiochemPy-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-14 09:54:45.000000 BiochemPy-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:44:24.006759 BiochemPy-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:44:24.006759 BiochemPy-0.3.0/BiochemPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-20 21:44:23.000000 BiochemPy-0.3.0/BiochemPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-20 21:44:23.000000 BiochemPy-0.3.0/BiochemPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 21:44:23.000000 BiochemPy-0.3.0/BiochemPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 21:44:23.000000 BiochemPy-0.3.0/BiochemPy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-20 21:44:18.000000 BiochemPy-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-20 21:44:24.006759 BiochemPy-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 21:44:24.006759 BiochemPy-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-20 21:44:18.000000 BiochemPy-0.3.0/setup.py
```

### Comparing `BiochemPy-0.2.0/LICENSE` & `BiochemPy-0.3.0/LICENSE`

 * *Files identical despite different names*

