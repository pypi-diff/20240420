# Comparing `tmp/octomy-batch-2.0.8.tar.gz` & `tmp/octomy-batch-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octomy-batch-2.0.8.tar", last modified: Tue Apr 16 11:50:44 2024, max compression
+gzip compressed data, was "octomy-batch-2.0.9.tar", last modified: Thu Apr 18 16:44:14 2024, max compression
```

## Comparing `octomy-batch-2.0.8.tar` & `octomy-batch-2.0.9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:50:44.559640 octomy-batch-2.0.8/
--rw-r--r--   0 leo       (1000) leo       (1000)      496 2021-12-17 22:49:10.000000 octomy-batch-2.0.8/.gitignore
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:50:44.555640 octomy-batch-2.0.8/.gitlab/
--rw-r--r--   0 leo       (1000) leo       (1000)      804 2021-11-09 04:03:42.000000 octomy-batch-2.0.8/.gitlab/ci.yaml
--rw-r--r--   0 leo       (1000) leo       (1000)     2021 2024-04-01 18:16:40.000000 octomy-batch-2.0.8/LICENSE
--rw-r--r--   0 leo       (1000) leo       (1000)      284 2024-04-01 17:02:28.000000 octomy-batch-2.0.8/Makefile
--rw-r--r--   0 leo       (1000) leo       (1000)     3129 2024-04-16 11:50:44.559640 octomy-batch-2.0.8/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)     2292 2024-04-01 18:15:51.000000 octomy-batch-2.0.8/README.md
--rw-r--r--   0 leo       (1000) leo       (1000)        6 2024-04-16 11:50:08.000000 octomy-batch-2.0.8/VERSION
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:50:44.555640 octomy-batch-2.0.8/bin/
--rwxr-xr-x   0 leo       (1000) leo       (1000)     3257 2024-04-06 21:53:07.000000 octomy-batch-2.0.8/bin/octomy-batch
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:50:44.555640 octomy-batch-2.0.8/code_quality/
--rw-rw-r--   0 leo       (1000) leo       (1000)      136 2020-03-25 22:47:14.000000 octomy-batch-2.0.8/code_quality/.flake8
--rw-r--r--   0 leo       (1000) leo       (1000)     1919 2021-11-09 04:03:42.000000 octomy-batch-2.0.8/code_quality/Makefile
--rw-rw-r--   0 leo       (1000) leo       (1000)      117 2020-03-25 22:44:52.000000 octomy-batch-2.0.8/code_quality/mypy.ini
--rw-rw-r--   0 leo       (1000) leo       (1000)    11867 2020-03-25 22:43:04.000000 octomy-batch-2.0.8/code_quality/pylintrc
--rw-r--r--   0 leo       (1000) leo       (1000)     2789 2021-11-09 04:03:47.000000 octomy-batch-2.0.8/config.json
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:50:44.547640 octomy-batch-2.0.8/octomy/
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:50:44.551640 octomy-batch-2.0.8/octomy/batch/
--rw-r--r--   0 leo       (1000) leo       (1000)    20902 2024-04-16 11:49:32.000000 octomy-batch-2.0.8/octomy/batch/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:50:44.551640 octomy-batch-2.0.8/octomy/batch/filters/
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2024-04-06 13:13:35.000000 octomy-batch-2.0.8/octomy/batch/filters/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:50:44.551640 octomy-batch-2.0.8/octomy/batch/filters/base/
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2021-11-09 04:03:42.000000 octomy-batch-2.0.8/octomy/batch/filters/base/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      302 2024-04-01 17:33:21.000000 octomy-batch-2.0.8/octomy/batch/filters/base/hello.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:50:44.555640 octomy-batch-2.0.8/octomy/batch/filters/utils/
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2021-11-09 04:03:42.000000 octomy-batch-2.0.8/octomy/batch/filters/utils/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      697 2024-04-01 20:23:49.000000 octomy-batch-2.0.8/octomy/batch/filters/utils/ping.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1285 2024-04-07 18:05:17.000000 octomy-batch-2.0.8/octomy/batch/filters/utils/test.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:50:44.555640 octomy-batch-2.0.8/octomy/batch/server/
--rw-rw-r--   0 leo       (1000) leo       (1000)     4381 2024-03-22 18:00:16.000000 octomy-batch-2.0.8/octomy/batch/server/WebsiteIO.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2254 2024-04-06 21:57:46.000000 octomy-batch-2.0.8/octomy/batch/server/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     4487 2024-04-11 00:20:42.000000 octomy-batch-2.0.8/octomy/batch/types.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:50:44.555640 octomy-batch-2.0.8/octomy_batch.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)     3129 2024-04-16 11:50:44.000000 octomy-batch-2.0.8/octomy_batch.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)     1301 2024-04-16 11:50:44.000000 octomy-batch-2.0.8/octomy_batch.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2024-04-16 11:50:44.000000 octomy-batch-2.0.8/octomy_batch.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-16 11:50:44.000000 octomy-batch-2.0.8/octomy_batch.egg-info/namespace_packages.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       21 2024-04-16 11:50:44.000000 octomy-batch-2.0.8/octomy_batch.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-16 11:50:44.000000 octomy-batch-2.0.8/octomy_batch.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2020-11-28 23:26:57.000000 octomy-batch-2.0.8/octomy_batch.egg-info/zip-safe
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:50:44.559640 octomy-batch-2.0.8/requirements/
--rw-r--r--   0 leo       (1000) leo       (1000)       21 2024-04-16 11:30:48.000000 octomy-batch-2.0.8/requirements/requirements.in
--rw-r--r--   0 leo       (1000) leo       (1000)     1743 2024-04-16 11:33:47.000000 octomy-batch-2.0.8/requirements/requirements.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      215 2021-11-09 04:03:42.000000 octomy-batch-2.0.8/requirements/test_requirements.in
--rw-r--r--   0 leo       (1000) leo       (1000)     2903 2023-08-28 22:19:16.000000 octomy-batch-2.0.8/requirements/test_requirements.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      166 2024-04-16 11:50:44.559640 octomy-batch-2.0.8/setup.cfg
--rwxr-xr-x   0 leo       (1000) leo       (1000)     7479 2024-04-11 00:17:44.000000 octomy-batch-2.0.8/setup.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:50:44.559640 octomy-batch-2.0.8/tests/
--rw-rw-r--   0 leo       (1000) leo       (1000)     1097 2020-03-19 22:34:38.000000 octomy-batch-2.0.8/tests/Makefile
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-19 20:39:36.000000 octomy-batch-2.0.8/tests/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:50:44.559640 octomy-batch-2.0.8/tests/integration/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-batch-2.0.8/tests/integration/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      125 2024-04-13 19:27:35.000000 octomy-batch-2.0.8/tests/integration/test_integration.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:50:44.559640 octomy-batch-2.0.8/tests/load/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-12-15 04:59:08.000000 octomy-batch-2.0.8/tests/load/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      118 2024-04-13 19:27:44.000000 octomy-batch-2.0.8/tests/load/test_load.py
--rw-r--r--   0 leo       (1000) leo       (1000)      339 2022-01-12 22:37:26.000000 octomy-batch-2.0.8/tests/pytest.ini
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:50:44.559640 octomy-batch-2.0.8/tests/regressions/
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2020-12-15 04:59:10.000000 octomy-batch-2.0.8/tests/regressions/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      125 2024-04-13 19:27:26.000000 octomy-batch-2.0.8/tests/regressions/test_regressions.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:50:44.559640 octomy-batch-2.0.8/tests/unit/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-batch-2.0.8/tests/unit/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1188 2024-04-13 21:48:19.000000 octomy-batch-2.0.8/tests/unit/test_batch_processor.py
--rw-r--r--   0 leo       (1000) leo       (1000)      178 2024-04-13 14:03:03.000000 octomy-batch-2.0.8/tests/unit/test_server.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2828 2024-04-13 14:24:05.000000 octomy-batch-2.0.8/tests/unit/test_unit.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-18 16:44:14.264067 octomy-batch-2.0.9/
+-rw-r--r--   0 leo       (1000) leo       (1000)      496 2021-12-17 22:49:10.000000 octomy-batch-2.0.9/.gitignore
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-18 16:44:14.260067 octomy-batch-2.0.9/.gitlab/
+-rw-r--r--   0 leo       (1000) leo       (1000)      804 2021-11-09 04:03:42.000000 octomy-batch-2.0.9/.gitlab/ci.yaml
+-rw-r--r--   0 leo       (1000) leo       (1000)     2021 2024-04-01 18:16:40.000000 octomy-batch-2.0.9/LICENSE
+-rw-r--r--   0 leo       (1000) leo       (1000)      284 2024-04-01 17:02:28.000000 octomy-batch-2.0.9/Makefile
+-rw-r--r--   0 leo       (1000) leo       (1000)     3129 2024-04-18 16:44:14.264067 octomy-batch-2.0.9/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)     2292 2024-04-01 18:15:51.000000 octomy-batch-2.0.9/README.md
+-rw-r--r--   0 leo       (1000) leo       (1000)        6 2024-04-18 16:43:32.000000 octomy-batch-2.0.9/VERSION
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-18 16:44:14.260067 octomy-batch-2.0.9/bin/
+-rwxr-xr-x   0 leo       (1000) leo       (1000)     3257 2024-04-06 21:53:07.000000 octomy-batch-2.0.9/bin/octomy-batch
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-18 16:44:14.260067 octomy-batch-2.0.9/code_quality/
+-rw-rw-r--   0 leo       (1000) leo       (1000)      136 2020-03-25 22:47:14.000000 octomy-batch-2.0.9/code_quality/.flake8
+-rw-r--r--   0 leo       (1000) leo       (1000)     1919 2021-11-09 04:03:42.000000 octomy-batch-2.0.9/code_quality/Makefile
+-rw-rw-r--   0 leo       (1000) leo       (1000)      117 2020-03-25 22:44:52.000000 octomy-batch-2.0.9/code_quality/mypy.ini
+-rw-rw-r--   0 leo       (1000) leo       (1000)    11867 2020-03-25 22:43:04.000000 octomy-batch-2.0.9/code_quality/pylintrc
+-rw-r--r--   0 leo       (1000) leo       (1000)     2789 2021-11-09 04:03:47.000000 octomy-batch-2.0.9/config.json
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-18 16:44:14.248067 octomy-batch-2.0.9/octomy/
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-18 16:44:14.256067 octomy-batch-2.0.9/octomy/batch/
+-rw-r--r--   0 leo       (1000) leo       (1000)    20895 2024-04-18 16:43:19.000000 octomy-batch-2.0.9/octomy/batch/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-18 16:44:14.256067 octomy-batch-2.0.9/octomy/batch/filters/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2024-04-06 13:13:35.000000 octomy-batch-2.0.9/octomy/batch/filters/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-18 16:44:14.256067 octomy-batch-2.0.9/octomy/batch/filters/base/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2021-11-09 04:03:42.000000 octomy-batch-2.0.9/octomy/batch/filters/base/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      302 2024-04-01 17:33:21.000000 octomy-batch-2.0.9/octomy/batch/filters/base/hello.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-18 16:44:14.256067 octomy-batch-2.0.9/octomy/batch/filters/utils/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2021-11-09 04:03:42.000000 octomy-batch-2.0.9/octomy/batch/filters/utils/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      697 2024-04-01 20:23:49.000000 octomy-batch-2.0.9/octomy/batch/filters/utils/ping.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1285 2024-04-07 18:05:17.000000 octomy-batch-2.0.9/octomy/batch/filters/utils/test.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-18 16:44:14.256067 octomy-batch-2.0.9/octomy/batch/server/
+-rw-rw-r--   0 leo       (1000) leo       (1000)     4381 2024-03-22 18:00:16.000000 octomy-batch-2.0.9/octomy/batch/server/WebsiteIO.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2254 2024-04-06 21:57:46.000000 octomy-batch-2.0.9/octomy/batch/server/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     4487 2024-04-11 00:20:42.000000 octomy-batch-2.0.9/octomy/batch/types.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-18 16:44:14.260067 octomy-batch-2.0.9/octomy_batch.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)     3129 2024-04-18 16:44:14.000000 octomy-batch-2.0.9/octomy_batch.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)     1301 2024-04-18 16:44:14.000000 octomy-batch-2.0.9/octomy_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2024-04-18 16:44:14.000000 octomy-batch-2.0.9/octomy_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-18 16:44:14.000000 octomy-batch-2.0.9/octomy_batch.egg-info/namespace_packages.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       21 2024-04-18 16:44:14.000000 octomy-batch-2.0.9/octomy_batch.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-18 16:44:14.000000 octomy-batch-2.0.9/octomy_batch.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2020-11-28 23:26:57.000000 octomy-batch-2.0.9/octomy_batch.egg-info/zip-safe
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-18 16:44:14.260067 octomy-batch-2.0.9/requirements/
+-rw-r--r--   0 leo       (1000) leo       (1000)       21 2024-04-16 11:30:48.000000 octomy-batch-2.0.9/requirements/requirements.in
+-rw-r--r--   0 leo       (1000) leo       (1000)     1743 2024-04-16 11:33:47.000000 octomy-batch-2.0.9/requirements/requirements.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      215 2021-11-09 04:03:42.000000 octomy-batch-2.0.9/requirements/test_requirements.in
+-rw-r--r--   0 leo       (1000) leo       (1000)     2903 2023-08-28 22:19:16.000000 octomy-batch-2.0.9/requirements/test_requirements.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      166 2024-04-18 16:44:14.268067 octomy-batch-2.0.9/setup.cfg
+-rwxr-xr-x   0 leo       (1000) leo       (1000)     7479 2024-04-11 00:17:44.000000 octomy-batch-2.0.9/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-18 16:44:14.264067 octomy-batch-2.0.9/tests/
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1097 2020-03-19 22:34:38.000000 octomy-batch-2.0.9/tests/Makefile
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-19 20:39:36.000000 octomy-batch-2.0.9/tests/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-18 16:44:14.264067 octomy-batch-2.0.9/tests/integration/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-batch-2.0.9/tests/integration/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      125 2024-04-13 19:27:35.000000 octomy-batch-2.0.9/tests/integration/test_integration.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-18 16:44:14.264067 octomy-batch-2.0.9/tests/load/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-12-15 04:59:08.000000 octomy-batch-2.0.9/tests/load/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      118 2024-04-13 19:27:44.000000 octomy-batch-2.0.9/tests/load/test_load.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      339 2022-01-12 22:37:26.000000 octomy-batch-2.0.9/tests/pytest.ini
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-18 16:44:14.264067 octomy-batch-2.0.9/tests/regressions/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2020-12-15 04:59:10.000000 octomy-batch-2.0.9/tests/regressions/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      125 2024-04-13 19:27:26.000000 octomy-batch-2.0.9/tests/regressions/test_regressions.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-18 16:44:14.264067 octomy-batch-2.0.9/tests/unit/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-batch-2.0.9/tests/unit/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1188 2024-04-13 21:48:19.000000 octomy-batch-2.0.9/tests/unit/test_batch_processor.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      178 2024-04-13 14:03:03.000000 octomy-batch-2.0.9/tests/unit/test_server.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2828 2024-04-13 14:24:05.000000 octomy-batch-2.0.9/tests/unit/test_unit.py
```

### Comparing `octomy-batch-2.0.8/.gitlab/ci.yaml` & `octomy-batch-2.0.9/.gitlab/ci.yaml`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.8/LICENSE` & `octomy-batch-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.8/PKG-INFO` & `octomy-batch-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octomy-batch
-Version: 2.0.8
+Version: 2.0.9
 Summary: ('octomy/batch',)
 Home-page: https://gitlab.com/octomy/batch
 Author: OctoMY
 Author-email: pypi@octomy.org
 Maintainer: OctoMY
 Maintainer-email: pypi@octomy.org
 License: Proprietary Software License
```

### Comparing `octomy-batch-2.0.8/README.md` & `octomy-batch-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.8/bin/octomy-batch` & `octomy-batch-2.0.9/bin/octomy-batch`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.8/code_quality/Makefile` & `octomy-batch-2.0.9/code_quality/Makefile`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.8/code_quality/pylintrc` & `octomy-batch-2.0.9/code_quality/pylintrc`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.8/config.json` & `octomy-batch-2.0.9/config.json`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.8/octomy/batch/__init__.py` & `octomy-batch-2.0.9/octomy/batch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 	alphabet = string.ascii_letters + string.digits
 	return "".join(random.choice(alphabet) for i in range(length))
 
 
 def get_package_relative_dir():
 	path = pathlib.Path(__file__).resolve()
 	logger.info(f"get_package_relative_dir file: '{path}' is file: {path.is_file()}")
-	path = path.parent.parent.parent
+	path = path.parent.parent
 	logger.info(f"get_package_relative_dir path: '{path}' is dir: {path.is_dir()}")
 	return path
 
 
 class Processor:
 	batch_sql_base:str = "octomy.batch"
```

### Comparing `octomy-batch-2.0.8/octomy/batch/filters/utils/ping.py` & `octomy-batch-2.0.9/octomy/batch/filters/utils/ping.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.8/octomy/batch/filters/utils/test.py` & `octomy-batch-2.0.9/octomy/batch/filters/utils/test.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.8/octomy/batch/server/WebsiteIO.py` & `octomy-batch-2.0.9/octomy/batch/server/WebsiteIO.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.8/octomy/batch/server/__init__.py` & `octomy-batch-2.0.9/octomy/batch/server/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.8/octomy/batch/types.py` & `octomy-batch-2.0.9/octomy/batch/types.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.8/octomy_batch.egg-info/PKG-INFO` & `octomy-batch-2.0.9/octomy_batch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octomy-batch
-Version: 2.0.8
+Version: 2.0.9
 Summary: ('octomy/batch',)
 Home-page: https://gitlab.com/octomy/batch
 Author: OctoMY
 Author-email: pypi@octomy.org
 Maintainer: OctoMY
 Maintainer-email: pypi@octomy.org
 License: Proprietary Software License
```

### Comparing `octomy-batch-2.0.8/octomy_batch.egg-info/SOURCES.txt` & `octomy-batch-2.0.9/octomy_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.8/requirements/requirements.txt` & `octomy-batch-2.0.9/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.8/requirements/test_requirements.txt` & `octomy-batch-2.0.9/requirements/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.8/setup.py` & `octomy-batch-2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.8/tests/Makefile` & `octomy-batch-2.0.9/tests/Makefile`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.8/tests/unit/test_batch_processor.py` & `octomy-batch-2.0.9/tests/unit/test_batch_processor.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.8/tests/unit/test_unit.py` & `octomy-batch-2.0.9/tests/unit/test_unit.py`

 * *Files identical despite different names*

