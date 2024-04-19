# Comparing `tmp/superdupper-0.0.4.tar.gz` & `tmp/superdupper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superdupper-0.0.4.tar", last modified: Fri Apr 19 23:32:15 2024, max compression
+gzip compressed data, was "superdupper-0.0.5.tar", last modified: Fri Apr 19 23:40:12 2024, max compression
```

## Comparing `superdupper-0.0.4.tar` & `superdupper-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:32:15.872754 superdupper-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-19 23:32:15.872754 superdupper-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 23:32:11.000000 superdupper-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-19 23:32:11.000000 superdupper-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 23:32:15.872754 superdupper-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:32:15.872754 superdupper-0.0.4/superdupper/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:32:15.872754 superdupper-0.0.4/superdupper/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 23:32:11.000000 superdupper-0.0.4/superdupper/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 23:32:11.000000 superdupper-0.0.4/superdupper/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:32:15.872754 superdupper-0.0.4/superdupper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-19 23:32:15.000000 superdupper-0.0.4/superdupper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-19 23:32:15.000000 superdupper-0.0.4/superdupper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 23:32:15.000000 superdupper-0.0.4/superdupper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-19 23:32:15.000000 superdupper-0.0.4/superdupper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 23:32:15.000000 superdupper-0.0.4/superdupper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:40:12.076523 superdupper-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-19 23:40:12.076523 superdupper-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 23:40:07.000000 superdupper-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-19 23:40:07.000000 superdupper-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 23:40:12.076523 superdupper-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:40:12.072523 superdupper-0.0.5/superdupper/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:40:12.072523 superdupper-0.0.5/superdupper/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 23:40:07.000000 superdupper-0.0.5/superdupper/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 23:40:07.000000 superdupper-0.0.5/superdupper/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:40:12.072523 superdupper-0.0.5/superdupper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-19 23:40:12.000000 superdupper-0.0.5/superdupper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-19 23:40:12.000000 superdupper-0.0.5/superdupper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 23:40:12.000000 superdupper-0.0.5/superdupper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-19 23:40:12.000000 superdupper-0.0.5/superdupper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 23:40:12.000000 superdupper-0.0.5/superdupper.egg-info/top_level.txt
```

