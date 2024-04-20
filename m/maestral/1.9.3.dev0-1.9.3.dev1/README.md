# Comparing `tmp/maestral-1.9.3.dev0.tar.gz` & `tmp/maestral-1.9.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestral-1.9.3.dev0.tar", last modified: Wed Mar 27 22:44:19 2024, max compression
+gzip compressed data, was "maestral-1.9.3.dev1.tar", last modified: Sat Apr 13 13:48:17 2024, max compression
```

## Comparing `maestral-1.9.3.dev0.tar` & `maestral-1.9.3.dev1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:44:19.906506 maestral-1.9.3.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9886 2024-03-27 22:44:19.906506 maestral-1.9.3.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 22:44:19.906506 maestral-1.9.3.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:44:19.890506 maestral-1.9.3.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:44:19.894506 maestral-1.9.3.dev0/src/maestral/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/autostart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:44:19.898506 maestral-1.9.3.dev0/src/maestral/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14787 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/cli/cli_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10518 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/cli/cli_info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1867 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/cli/cli_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    15396 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/cli/cli_maintenance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/cli/cli_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/cli/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/cli/output.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    69560 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:44:19.898506 maestral-1.9.3.dev0/src/maestral/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/config/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    17864 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/config/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    21902 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/daemon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:44:19.902506 maestral-1.9.3.dev0/src/maestral/database/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/database/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    17305 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/database/orm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/database/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/database/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    33651 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/errorhandling.py
--rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:44:19.902506 maestral-1.9.3.dev0/src/maestral/fsevents/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/fsevents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/fsevents/polling.py
--rw-r--r--   0 runner    (1001) docker     (127)     9847 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/keyring.py
--rw-r--r--   0 runner    (1001) docker     (127)     8819 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    63409 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    28369 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    18363 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/notify.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:44:19.902506 maestral-1.9.3.dev0/src/maestral/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   137001 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/resources/maestral.png
--rw-r--r--   0 runner    (1001) docker     (127)   150595 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:44:19.902506 maestral-1.9.3.dev0/src/maestral/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/utils/appdirs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/utils/caches.py
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/utils/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/utils/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    19722 2024-03-27 22:44:15.000000 maestral-1.9.3.dev0/src/maestral/utils/path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:44:19.902506 maestral-1.9.3.dev0/src/maestral.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9886 2024-03-27 22:44:19.000000 maestral-1.9.3.dev0/src/maestral.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-03-27 22:44:19.000000 maestral-1.9.3.dev0/src/maestral.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 22:44:19.000000 maestral-1.9.3.dev0/src/maestral.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-27 22:44:19.000000 maestral-1.9.3.dev0/src/maestral.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-27 22:44:19.000000 maestral-1.9.3.dev0/src/maestral.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-27 22:44:19.000000 maestral-1.9.3.dev0/src/maestral.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:48:17.229197 maestral-1.9.3.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9886 2024-04-13 13:48:17.229197 maestral-1.9.3.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:48:17.229197 maestral-1.9.3.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:48:17.217197 maestral-1.9.3.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:48:17.221197 maestral-1.9.3.dev1/src/maestral/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/autostart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:48:17.225197 maestral-1.9.3.dev1/src/maestral/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14787 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/cli/cli_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10518 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/cli/cli_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1867 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/cli/cli_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15396 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/cli/cli_maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/cli/cli_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/cli/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/cli/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69560 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:48:17.225197 maestral-1.9.3.dev1/src/maestral/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/config/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17864 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/config/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21902 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/daemon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:48:17.225197 maestral-1.9.3.dev1/src/maestral/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/database/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17305 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/database/orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/database/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/database/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33651 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/errorhandling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:48:17.225197 maestral-1.9.3.dev1/src/maestral/fsevents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/fsevents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/fsevents/polling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9847 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8819 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63409 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28369 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18363 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:48:17.225197 maestral-1.9.3.dev1/src/maestral/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137001 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/resources/maestral.png
+-rw-r--r--   0 runner    (1001) docker     (127)   150595 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:48:17.229197 maestral-1.9.3.dev1/src/maestral/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/utils/appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/utils/caches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/utils/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/utils/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19722 2024-04-13 13:48:12.000000 maestral-1.9.3.dev1/src/maestral/utils/path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:48:17.229197 maestral-1.9.3.dev1/src/maestral.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9886 2024-04-13 13:48:17.000000 maestral-1.9.3.dev1/src/maestral.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-13 13:48:17.000000 maestral-1.9.3.dev1/src/maestral.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:48:17.000000 maestral-1.9.3.dev1/src/maestral.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-13 13:48:17.000000 maestral-1.9.3.dev1/src/maestral.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-13 13:48:17.000000 maestral-1.9.3.dev1/src/maestral.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 13:48:17.000000 maestral-1.9.3.dev1/src/maestral.egg-info/top_level.txt
```

### Comparing `maestral-1.9.3.dev0/LICENSE.txt` & `maestral-1.9.3.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/PKG-INFO` & `maestral-1.9.3.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestral
-Version: 1.9.3.dev0
+Version: 1.9.3.dev1
 Summary: Open-source Dropbox client for macOS and Linux.
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://maestral.app
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
@@ -34,16 +34,16 @@
 Requires-Dist: rubicon-objc>=0.4.1; sys_platform == "darwin"
 Requires-Dist: setuptools
 Requires-Dist: survey<6.0,>=4.0
 Requires-Dist: typing_extensions
 Requires-Dist: watchdog>=2.0.1
 Requires-Dist: xattr
 Provides-Extra: gui
-Requires-Dist: maestral-qt>=1.9.3.dev0; sys_platform == "linux" and extra == "gui"
-Requires-Dist: maestral-cocoa>=1.9.3.dev0; sys_platform == "darwin" and extra == "gui"
+Requires-Dist: maestral-qt>=1.9.3.dev1; sys_platform == "linux" and extra == "gui"
+Requires-Dist: maestral-cocoa>=1.9.3.dev1; sys_platform == "darwin" and extra == "gui"
 Provides-Extra: syslog
 Requires-Dist: systemd-python; extra == "syslog"
 Provides-Extra: lint
 Requires-Dist: black; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
 Requires-Dist: flake8-pyproject; extra == "lint"
 Requires-Dist: mypy; extra == "lint"
```

### Comparing `maestral-1.9.3.dev0/README.md` & `maestral-1.9.3.dev1/README.md`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/pyproject.toml` & `maestral-1.9.3.dev1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "maestral"
-version = "1.9.3.dev0"
+version = "1.9.3.dev1"
 authors = [{name = "Sam Schott", email = "sam.schott@outlook.com"}]
 license = {text = "MIT"}
 description = "Open-source Dropbox client for macOS and Linux."
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: Unix",
     "Programming Language :: Python",
@@ -46,16 +46,16 @@
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.optional-dependencies]
 gui = [
-    "maestral-qt>=1.9.3.dev0;sys_platform=='linux'",
-    "maestral-cocoa>=1.9.3.dev0;sys_platform=='darwin'",
+    "maestral-qt>=1.9.3.dev1;sys_platform=='linux'",
+    "maestral-cocoa>=1.9.3.dev1;sys_platform=='darwin'",
 ]
 syslog = ["systemd-python"]
 lint = [
     "black",
     "flake8",
     "flake8-pyproject",
     "mypy",
```

### Comparing `maestral-1.9.3.dev0/src/maestral/autostart.py` & `maestral-1.9.3.dev1/src/maestral/autostart.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/cli/cli_core.py` & `maestral-1.9.3.dev1/src/maestral/cli/cli_core.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/cli/cli_info.py` & `maestral-1.9.3.dev1/src/maestral/cli/cli_info.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/cli/cli_main.py` & `maestral-1.9.3.dev1/src/maestral/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/cli/cli_maintenance.py` & `maestral-1.9.3.dev1/src/maestral/cli/cli_maintenance.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/cli/cli_settings.py` & `maestral-1.9.3.dev1/src/maestral/cli/cli_settings.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/cli/common.py` & `maestral-1.9.3.dev1/src/maestral/cli/common.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/cli/core.py` & `maestral-1.9.3.dev1/src/maestral/cli/core.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/cli/dialogs.py` & `maestral-1.9.3.dev1/src/maestral/cli/dialogs.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/cli/output.py` & `maestral-1.9.3.dev1/src/maestral/cli/output.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/client.py` & `maestral-1.9.3.dev1/src/maestral/client.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/config/__init__.py` & `maestral-1.9.3.dev1/src/maestral/config/__init__.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/config/main.py` & `maestral-1.9.3.dev1/src/maestral/config/main.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/config/user.py` & `maestral-1.9.3.dev1/src/maestral/config/user.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/constants.py` & `maestral-1.9.3.dev1/src/maestral/constants.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/core.py` & `maestral-1.9.3.dev1/src/maestral/core.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/daemon.py` & `maestral-1.9.3.dev1/src/maestral/daemon.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/database/core.py` & `maestral-1.9.3.dev1/src/maestral/database/core.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/database/orm.py` & `maestral-1.9.3.dev1/src/maestral/database/orm.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/database/query.py` & `maestral-1.9.3.dev1/src/maestral/database/query.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/database/types.py` & `maestral-1.9.3.dev1/src/maestral/database/types.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/errorhandling.py` & `maestral-1.9.3.dev1/src/maestral/errorhandling.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/exceptions.py` & `maestral-1.9.3.dev1/src/maestral/exceptions.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/fsevents/__init__.py` & `maestral-1.9.3.dev1/src/maestral/fsevents/__init__.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/fsevents/polling.py` & `maestral-1.9.3.dev1/src/maestral/fsevents/polling.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/keyring.py` & `maestral-1.9.3.dev1/src/maestral/keyring.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/logging.py` & `maestral-1.9.3.dev1/src/maestral/logging.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/main.py` & `maestral-1.9.3.dev1/src/maestral/main.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/manager.py` & `maestral-1.9.3.dev1/src/maestral/manager.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/models.py` & `maestral-1.9.3.dev1/src/maestral/models.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/notify.py` & `maestral-1.9.3.dev1/src/maestral/notify.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/resources/maestral.png` & `maestral-1.9.3.dev1/src/maestral/resources/maestral.png`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/sync.py` & `maestral-1.9.3.dev1/src/maestral/sync.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/utils/__init__.py` & `maestral-1.9.3.dev1/src/maestral/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/utils/appdirs.py` & `maestral-1.9.3.dev1/src/maestral/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/utils/caches.py` & `maestral-1.9.3.dev1/src/maestral/utils/caches.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/utils/hashing.py` & `maestral-1.9.3.dev1/src/maestral/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/utils/integration.py` & `maestral-1.9.3.dev1/src/maestral/utils/integration.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral/utils/path.py` & `maestral-1.9.3.dev1/src/maestral/utils/path.py`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral.egg-info/PKG-INFO` & `maestral-1.9.3.dev1/src/maestral.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestral
-Version: 1.9.3.dev0
+Version: 1.9.3.dev1
 Summary: Open-source Dropbox client for macOS and Linux.
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://maestral.app
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
@@ -34,16 +34,16 @@
 Requires-Dist: rubicon-objc>=0.4.1; sys_platform == "darwin"
 Requires-Dist: setuptools
 Requires-Dist: survey<6.0,>=4.0
 Requires-Dist: typing_extensions
 Requires-Dist: watchdog>=2.0.1
 Requires-Dist: xattr
 Provides-Extra: gui
-Requires-Dist: maestral-qt>=1.9.3.dev0; sys_platform == "linux" and extra == "gui"
-Requires-Dist: maestral-cocoa>=1.9.3.dev0; sys_platform == "darwin" and extra == "gui"
+Requires-Dist: maestral-qt>=1.9.3.dev1; sys_platform == "linux" and extra == "gui"
+Requires-Dist: maestral-cocoa>=1.9.3.dev1; sys_platform == "darwin" and extra == "gui"
 Provides-Extra: syslog
 Requires-Dist: systemd-python; extra == "syslog"
 Provides-Extra: lint
 Requires-Dist: black; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
 Requires-Dist: flake8-pyproject; extra == "lint"
 Requires-Dist: mypy; extra == "lint"
```

### Comparing `maestral-1.9.3.dev0/src/maestral.egg-info/SOURCES.txt` & `maestral-1.9.3.dev1/src/maestral.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maestral-1.9.3.dev0/src/maestral.egg-info/requires.txt` & `maestral-1.9.3.dev1/src/maestral.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 sphinxext-opengraph==0.9.1
 sphinx-autoapi==3.0.0
 sphinx-mdinclude==0.5.3
 
 [gui]
 
 [gui:sys_platform == "darwin"]
-maestral-cocoa>=1.9.3.dev0
+maestral-cocoa>=1.9.3.dev1
 
 [gui:sys_platform == "linux"]
-maestral-qt>=1.9.3.dev0
+maestral-qt>=1.9.3.dev1
 
 [lint]
 black
 flake8
 flake8-pyproject
 mypy
 pyupgrade
```

