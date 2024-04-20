# Comparing `tmp/superdupper_core-0.0.12.tar.gz` & `tmp/superdupper_core-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superdupper_core-0.0.12.tar", last modified: Sat Apr 20 00:13:29 2024, max compression
+gzip compressed data, was "superdupper_core-0.0.13.tar", last modified: Sat Apr 20 00:21:40 2024, max compression
```

## Comparing `superdupper_core-0.0.12.tar` & `superdupper_core-0.0.13.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:13:29.424910 superdupper_core-0.0.12/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-20 00:13:29.424910 superdupper_core-0.0.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-20 00:13:15.000000 superdupper_core-0.0.12/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-20 00:13:15.000000 superdupper_core-0.0.12/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 00:13:29.424910 superdupper_core-0.0.12/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:13:29.424910 superdupper_core-0.0.12/superdupper/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:13:29.424910 superdupper_core-0.0.12/superdupper/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:13:15.000000 superdupper_core-0.0.12/superdupper/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-20 00:13:15.000000 superdupper_core-0.0.12/superdupper/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:13:29.424910 superdupper_core-0.0.12/superdupper_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-20 00:13:29.000000 superdupper_core-0.0.12/superdupper_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-20 00:13:29.000000 superdupper_core-0.0.12/superdupper_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 00:13:29.000000 superdupper_core-0.0.12/superdupper_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-20 00:13:29.000000 superdupper_core-0.0.12/superdupper_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:21:40.631491 superdupper_core-0.0.13/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-20 00:21:40.631491 superdupper_core-0.0.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-20 00:21:19.000000 superdupper_core-0.0.13/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-20 00:21:19.000000 superdupper_core-0.0.13/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 00:21:40.631491 superdupper_core-0.0.13/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:21:40.627491 superdupper_core-0.0.13/superdupper/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:21:40.631491 superdupper_core-0.0.13/superdupper/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:21:19.000000 superdupper_core-0.0.13/superdupper/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-20 00:21:19.000000 superdupper_core-0.0.13/superdupper/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:21:40.631491 superdupper_core-0.0.13/superdupper/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:21:19.000000 superdupper_core-0.0.13/superdupper/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-20 00:21:19.000000 superdupper_core-0.0.13/superdupper/services/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:21:40.631491 superdupper_core-0.0.13/superdupper_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-20 00:21:40.000000 superdupper_core-0.0.13/superdupper_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-20 00:21:40.000000 superdupper_core-0.0.13/superdupper_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 00:21:40.000000 superdupper_core-0.0.13/superdupper_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-20 00:21:40.000000 superdupper_core-0.0.13/superdupper_core.egg-info/top_level.txt
```

