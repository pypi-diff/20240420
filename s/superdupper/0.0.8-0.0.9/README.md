# Comparing `tmp/superdupper-0.0.8.tar.gz` & `tmp/superdupper-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superdupper-0.0.8.tar", last modified: Fri Apr 19 23:53:28 2024, max compression
+gzip compressed data, was "superdupper-0.0.9.tar", last modified: Fri Apr 19 23:59:33 2024, max compression
```

## Comparing `superdupper-0.0.8.tar` & `superdupper-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:53:28.212518 superdupper-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-19 23:53:28.208518 superdupper-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 23:53:23.000000 superdupper-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-19 23:53:23.000000 superdupper-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 23:53:28.212518 superdupper-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:53:28.208518 superdupper-0.0.8/superdupper/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:53:28.208518 superdupper-0.0.8/superdupper/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 23:53:23.000000 superdupper-0.0.8/superdupper/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 23:53:23.000000 superdupper-0.0.8/superdupper/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:53:28.208518 superdupper-0.0.8/superdupper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-19 23:53:28.000000 superdupper-0.0.8/superdupper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-19 23:53:28.000000 superdupper-0.0.8/superdupper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 23:53:28.000000 superdupper-0.0.8/superdupper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-19 23:53:28.000000 superdupper-0.0.8/superdupper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 23:53:28.000000 superdupper-0.0.8/superdupper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:59:33.734222 superdupper-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-19 23:59:33.734222 superdupper-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 23:59:29.000000 superdupper-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-19 23:59:29.000000 superdupper-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 23:59:33.734222 superdupper-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:59:33.730222 superdupper-0.0.9/superdupper/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:59:33.730222 superdupper-0.0.9/superdupper/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 23:59:29.000000 superdupper-0.0.9/superdupper/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 23:59:29.000000 superdupper-0.0.9/superdupper/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:59:33.730222 superdupper-0.0.9/superdupper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-19 23:59:33.000000 superdupper-0.0.9/superdupper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-19 23:59:33.000000 superdupper-0.0.9/superdupper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 23:59:33.000000 superdupper-0.0.9/superdupper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-19 23:59:33.000000 superdupper-0.0.9/superdupper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 23:59:33.000000 superdupper-0.0.9/superdupper.egg-info/top_level.txt
```

