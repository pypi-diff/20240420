# Comparing `tmp/datapools-1.0.43.tar.gz` & `tmp/datapools-1.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapools-1.0.43.tar", last modified: Wed Apr 17 15:03:00 2024, max compression
+gzip compressed data, was "datapools-1.0.44.tar", last modified: Sat Apr 20 18:46:28 2024, max compression
```

## Comparing `datapools-1.0.43.tar` & `datapools-1.0.44.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.162591 datapools-1.0.43/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-17 15:02:48.000000 datapools-1.0.43/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:48.000000 datapools-1.0.43/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-17 15:02:48.000000 datapools-1.0.43/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-17 15:02:48.000000 datapools-1.0.43/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-17 15:03:00.162591 datapools-1.0.43/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-17 15:02:48.000000 datapools-1.0.43/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.154591 datapools-1.0.43/datapools/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.154591 datapools-1.0.43/datapools/common/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/backend_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.154591 datapools-1.0.43/datapools/common/queues/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12803 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/queues/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/queues/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/stoppable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.154591 datapools-1.0.43/datapools/common/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/storage/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/storage/file_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.154591 datapools-1.0.43/datapools/common/tasks_db/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/tasks_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/tasks_db/redis.py.bak
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/tasks_db/tasks_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.154591 datapools-1.0.43/datapools/producer/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/producer/base_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10977 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/worker/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12281 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/base_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/worker/plugins/dataphoenix_info/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/dataphoenix_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/worker/plugins/default/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9090 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/default/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/worker/plugins/deutsche_welle/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/deutsche_welle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/worker/plugins/google_drive/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/google_drive/google_drive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/worker/plugins/imageshack/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/imageshack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10983 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/imageshack/imageshack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/worker/plugins/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/s3/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/worker/plugins/theguardian/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/theguardian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/theguardian/theguardian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.158591 datapools-1.0.43/datapools/worker/plugins/washingtonpost/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/washingtonpost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6616 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/washingtonpost/washingtonpost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.162591 datapools-1.0.43/datapools/worker/plugins/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/wikipedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/wikipedia/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.162591 datapools-1.0.43/datapools/worker/plugins/youtube_channel/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/youtube_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/plugins/youtube_channel/youtube_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-04-17 15:02:48.000000 datapools-1.0.43/datapools/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.162591 datapools-1.0.43/datapools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-17 15:03:00.000000 datapools-1.0.43/datapools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-17 15:03:00.000000 datapools-1.0.43/datapools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:03:00.000000 datapools-1.0.43/datapools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 15:03:00.000000 datapools-1.0.43/datapools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-17 15:03:00.000000 datapools-1.0.43/datapools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 15:03:00.000000 datapools-1.0.43/datapools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 15:03:00.162591 datapools-1.0.43/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-17 15:02:48.000000 datapools-1.0.43/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:03:00.162591 datapools-1.0.43/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:48.000000 datapools-1.0.43/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-17 15:02:48.000000 datapools-1.0.43/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-17 15:02:48.000000 datapools-1.0.43/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.676915 datapools-1.0.44/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-20 18:46:18.000000 datapools-1.0.44/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:18.000000 datapools-1.0.44/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-20 18:46:18.000000 datapools-1.0.44/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-20 18:46:18.000000 datapools-1.0.44/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-20 18:46:28.676915 datapools-1.0.44/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-20 18:46:18.000000 datapools-1.0.44/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.664915 datapools-1.0.44/datapools/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.664915 datapools-1.0.44/datapools/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/backend_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.668915 datapools-1.0.44/datapools/common/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12803 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/queues/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/queues/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/stoppable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.668915 datapools-1.0.44/datapools/common/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/storage/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/storage/file_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.668915 datapools-1.0.44/datapools/common/tasks_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/tasks_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/tasks_db/redis.py.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/tasks_db/tasks_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.668915 datapools-1.0.44/datapools/producer/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/producer/base_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.668915 datapools-1.0.44/datapools/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10977 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.668915 datapools-1.0.44/datapools/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.672915 datapools-1.0.44/datapools/worker/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12281 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/base_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.672915 datapools-1.0.44/datapools/worker/plugins/dataphoenix_info/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/dataphoenix_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.672915 datapools-1.0.44/datapools/worker/plugins/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9090 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/default/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.672915 datapools-1.0.44/datapools/worker/plugins/deutsche_welle/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/deutsche_welle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.672915 datapools-1.0.44/datapools/worker/plugins/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/google_drive/google_drive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.672915 datapools-1.0.44/datapools/worker/plugins/imageshack/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/imageshack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10983 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/imageshack/imageshack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.672915 datapools-1.0.44/datapools/worker/plugins/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/s3/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.672915 datapools-1.0.44/datapools/worker/plugins/theguardian/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/theguardian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/theguardian/theguardian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.672915 datapools-1.0.44/datapools/worker/plugins/washingtonpost/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/washingtonpost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6616 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/washingtonpost/washingtonpost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.672915 datapools-1.0.44/datapools/worker/plugins/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/wikipedia/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.676915 datapools-1.0.44/datapools/worker/plugins/youtube_channel/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/youtube_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/youtube_channel/youtube_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.676915 datapools-1.0.44/datapools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-20 18:46:28.000000 datapools-1.0.44/datapools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-20 18:46:28.000000 datapools-1.0.44/datapools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:46:28.000000 datapools-1.0.44/datapools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-20 18:46:28.000000 datapools-1.0.44/datapools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-20 18:46:28.000000 datapools-1.0.44/datapools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 18:46:28.000000 datapools-1.0.44/datapools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:46:28.676915 datapools-1.0.44/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-20 18:46:18.000000 datapools-1.0.44/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.676915 datapools-1.0.44/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:18.000000 datapools-1.0.44/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-20 18:46:18.000000 datapools-1.0.44/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-20 18:46:18.000000 datapools-1.0.44/tests/test_base.py
```

### Comparing `datapools-1.0.43/LICENSE` & `datapools-1.0.44/LICENSE`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/PKG-INFO` & `datapools-1.0.44/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.43
+Version: 1.0.44
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.43/README.md` & `datapools-1.0.44/README.md`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/api.py` & `datapools-1.0.44/datapools/api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/cli.py` & `datapools-1.0.44/datapools/cli.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/common/backend_api.py` & `datapools-1.0.44/datapools/common/backend_api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/common/queues/__init__.py` & `datapools-1.0.44/datapools/common/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/common/queues/rabbitmq.py` & `datapools-1.0.44/datapools/common/queues/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/common/queues/types.py` & `datapools-1.0.44/datapools/common/queues/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/common/session_manager.py` & `datapools-1.0.44/datapools/common/session_manager.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/common/stoppable.py` & `datapools-1.0.44/datapools/common/stoppable.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/common/storage/base_storage.py` & `datapools-1.0.44/datapools/common/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/common/storage/file_storage.py` & `datapools-1.0.44/datapools/common/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/common/tasks_db/redis.py.bak` & `datapools-1.0.44/datapools/common/tasks_db/redis.py.bak`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/common/tasks_db/tasks_db.py` & `datapools-1.0.44/datapools/common/tasks_db/tasks_db.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/common/types.py` & `datapools-1.0.44/datapools/common/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,19 @@
     USE_ONLY_PLUGINS: Optional[List[str]] = None
     ADDITIONAL_PLUGINS: Optional[List[str]] = None
 
     plugins_config: dict = {}
 
     def load(self, config: dict):
         """fills self with json config"""
+        backend = config.get('backend', {})
+        api_url = backend.get('api_url')
+        if api_url is not None:
+            self.BACKEND_API_URL = api_url
+        
         # Queue
         queue = config.get('queue', {})
         queue_connection_url = queue.get('connection_url')
         if queue_connection_url is not None:
             self.QUEUE_CONNECTION_URL = queue_connection_url
         queue_size_limit = queue.get('size_limit')
         if queue_size_limit is not None:
```

### Comparing `datapools-1.0.43/datapools/producer/base_producer.py` & `datapools-1.0.44/datapools/producer/base_producer.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/scheduler/scheduler.py` & `datapools-1.0.44/datapools/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/worker/plugins/base_plugin.py` & `datapools-1.0.44/datapools/worker/plugins/base_plugin.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py` & `datapools-1.0.44/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/worker/plugins/default/default.py` & `datapools-1.0.44/datapools/worker/plugins/default/default.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/worker/plugins/deutsche_welle/deutsche_welle.py` & `datapools-1.0.44/datapools/worker/plugins/deutsche_welle/deutsche_welle.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/worker/plugins/google_drive/google_drive.py` & `datapools-1.0.44/datapools/worker/plugins/google_drive/google_drive.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/worker/plugins/imageshack/imageshack.py` & `datapools-1.0.44/datapools/worker/plugins/imageshack/imageshack.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/worker/plugins/s3/s3.py` & `datapools-1.0.44/datapools/worker/plugins/s3/s3.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/worker/plugins/theguardian/theguardian.py` & `datapools-1.0.44/datapools/worker/plugins/theguardian/theguardian.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/worker/plugins/washingtonpost/washingtonpost.py` & `datapools-1.0.44/datapools/worker/plugins/washingtonpost/washingtonpost.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/worker/plugins/wikipedia/wikipedia.py` & `datapools-1.0.44/datapools/worker/plugins/wikipedia/wikipedia.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/worker/plugins/youtube_channel/youtube_channel.py` & `datapools-1.0.44/datapools/worker/plugins/youtube_channel/youtube_channel.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools/worker/worker.py` & `datapools-1.0.44/datapools/worker/worker.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/datapools.egg-info/PKG-INFO` & `datapools-1.0.44/datapools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.43
+Version: 1.0.44
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.43/datapools.egg-info/SOURCES.txt` & `datapools-1.0.44/datapools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datapools-1.0.43/setup.py` & `datapools-1.0.44/setup.py`

 * *Files identical despite different names*

