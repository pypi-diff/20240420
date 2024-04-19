# Comparing `tmp/superdupper-0.0.5.tar.gz` & `tmp/superdupper-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superdupper-0.0.5.tar", last modified: Fri Apr 19 23:40:12 2024, max compression
+gzip compressed data, was "superdupper-0.0.6.tar", last modified: Fri Apr 19 23:45:23 2024, max compression
```

## Comparing `superdupper-0.0.5.tar` & `superdupper-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:40:12.076523 superdupper-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-19 23:40:12.076523 superdupper-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 23:40:07.000000 superdupper-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-19 23:40:07.000000 superdupper-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 23:40:12.076523 superdupper-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:40:12.072523 superdupper-0.0.5/superdupper/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:40:12.072523 superdupper-0.0.5/superdupper/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 23:40:07.000000 superdupper-0.0.5/superdupper/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 23:40:07.000000 superdupper-0.0.5/superdupper/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:40:12.072523 superdupper-0.0.5/superdupper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-19 23:40:12.000000 superdupper-0.0.5/superdupper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-19 23:40:12.000000 superdupper-0.0.5/superdupper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 23:40:12.000000 superdupper-0.0.5/superdupper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-19 23:40:12.000000 superdupper-0.0.5/superdupper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 23:40:12.000000 superdupper-0.0.5/superdupper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:45:23.677912 superdupper-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-19 23:45:23.677912 superdupper-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 23:45:19.000000 superdupper-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-19 23:45:19.000000 superdupper-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 23:45:23.677912 superdupper-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:45:23.673912 superdupper-0.0.6/superdupper/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:45:23.677912 superdupper-0.0.6/superdupper/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 23:45:19.000000 superdupper-0.0.6/superdupper/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 23:45:19.000000 superdupper-0.0.6/superdupper/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:45:23.677912 superdupper-0.0.6/superdupper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-19 23:45:23.000000 superdupper-0.0.6/superdupper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-19 23:45:23.000000 superdupper-0.0.6/superdupper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 23:45:23.000000 superdupper-0.0.6/superdupper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-19 23:45:23.000000 superdupper-0.0.6/superdupper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 23:45:23.000000 superdupper-0.0.6/superdupper.egg-info/top_level.txt
```

