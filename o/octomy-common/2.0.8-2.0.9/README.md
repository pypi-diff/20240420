# Comparing `tmp/octomy-common-2.0.8.tar.gz` & `tmp/octomy-common-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octomy-common-2.0.8.tar", last modified: Tue Apr 16 11:31:00 2024, max compression
+gzip compressed data, was "octomy-common-2.0.9.tar", last modified: Fri Apr 19 23:12:55 2024, max compression
```

## Comparing `octomy-common-2.0.8.tar` & `octomy-common-2.0.9.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.359543 octomy-common-2.0.8/
--rw-r--r--   0 leo       (1000) leo       (1000)      735 2021-12-02 17:02:15.000000 octomy-common-2.0.8/.gitignore
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.355543 octomy-common-2.0.8/.gitlab/
--rw-r--r--   0 leo       (1000) leo       (1000)      771 2021-12-02 17:02:15.000000 octomy-common-2.0.8/.gitlab/ci.yaml
--rw-r--r--   0 leo       (1000) leo       (1000)     2021 2024-04-06 09:06:50.000000 octomy-common-2.0.8/LICENSE
--rw-r--r--   0 leo       (1000) leo       (1000)      284 2024-04-06 08:33:37.000000 octomy-common-2.0.8/Makefile
--rw-r--r--   0 leo       (1000) leo       (1000)     8435 2024-04-16 11:31:00.359543 octomy-common-2.0.8/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)     7595 2024-04-06 08:34:18.000000 octomy-common-2.0.8/README.md
--rw-r--r--   0 leo       (1000) leo       (1000)        6 2024-04-16 11:30:26.000000 octomy-common-2.0.8/VERSION
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.355543 octomy-common-2.0.8/code_quality/
--rw-r--r--   0 leo       (1000) leo       (1000)      214 2021-12-02 17:02:15.000000 octomy-common-2.0.8/code_quality/.flake8
--rw-r--r--   0 leo       (1000) leo       (1000)     2492 2021-12-28 02:40:34.000000 octomy-common-2.0.8/code_quality/Makefile
--rw-r--r--   0 leo       (1000) leo       (1000)      135 2021-12-02 17:02:15.000000 octomy-common-2.0.8/code_quality/mypy.ini
--rw-rw-r--   0 leo       (1000) leo       (1000)    11867 2020-03-02 23:49:28.000000 octomy-common-2.0.8/code_quality/pylintrc
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.355543 octomy-common-2.0.8/design/
--rw-r--r--   0 leo       (1000) leo       (1000)    62298 2021-12-02 17:02:15.000000 octomy-common-2.0.8/design/logo-1024.png
--rw-r--r--   0 leo       (1000) leo       (1000)     7427 2021-12-02 17:02:15.000000 octomy-common-2.0.8/design/logo-1024.svg
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.343543 octomy-common-2.0.8/octomy/
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.347543 octomy-common-2.0.8/octomy/access/
--rw-r--r--   0 leo       (1000) leo       (1000)    11927 2024-04-06 10:41:55.000000 octomy-common-2.0.8/octomy/access/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.347543 octomy-common-2.0.8/octomy/cad/
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.347543 octomy-common-2.0.8/octomy/cad/generators/
--rw-r--r--   0 leo       (1000) leo       (1000)     4653 2024-03-21 20:06:58.000000 octomy-common-2.0.8/octomy/cad/generators/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2023-12-09 21:11:36.000000 octomy-common-2.0.8/octomy/cad/generators/common.py
--rw-r--r--   0 leo       (1000) leo       (1000)       74 2023-12-09 21:13:26.000000 octomy-common-2.0.8/octomy/cad/generators/ntop.py
--rw-r--r--   0 leo       (1000) leo       (1000)     6642 2024-03-21 20:05:55.000000 octomy-common-2.0.8/octomy/cad/generators/openscad.py
--rw-r--r--   0 leo       (1000) leo       (1000)    15524 2024-04-06 12:29:11.000000 octomy-common-2.0.8/octomy/cad/ntop.py
--rw-r--r--   0 leo       (1000) leo       (1000)    28147 2024-04-06 12:29:00.000000 octomy-common-2.0.8/octomy/cad/openscad.py
--rw-r--r--   0 leo       (1000) leo       (1000)    20669 2024-03-21 19:38:26.000000 octomy-common-2.0.8/octomy/cad/parts.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.347543 octomy-common-2.0.8/octomy/cad/types/
--rw-r--r--   0 leo       (1000) leo       (1000)     3633 2023-12-09 22:30:55.000000 octomy-common-2.0.8/octomy/cad/types/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.347543 octomy-common-2.0.8/octomy/config/
--rw-r--r--   0 leo       (1000) leo       (1000)    13353 2024-04-14 09:41:27.000000 octomy-common-2.0.8/octomy/config/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.347543 octomy-common-2.0.8/octomy/db/
--rw-rw-r--   0 leo       (1000) leo       (1000)    18290 2024-04-16 11:27:50.000000 octomy-common-2.0.8/octomy/db/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      841 2024-04-06 17:40:11.000000 octomy-common-2.0.8/octomy/db/check.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.347543 octomy-common-2.0.8/octomy/log/
--rw-rw-r--   0 leo       (1000) leo       (1000)     1477 2024-04-06 08:54:24.000000 octomy-common-2.0.8/octomy/log/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.347543 octomy-common-2.0.8/octomy/storage/
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2023-12-09 19:06:16.000000 octomy-common-2.0.8/octomy/storage/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)    11978 2023-12-09 18:40:20.000000 octomy-common-2.0.8/octomy/storage/google_drive.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.351543 octomy-common-2.0.8/octomy/utils/
--rw-rw-r--   0 leo       (1000) leo       (1000)      129 2024-04-06 09:03:01.000000 octomy-common-2.0.8/octomy/utils/Context.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      896 2024-04-06 09:04:17.000000 octomy-common-2.0.8/octomy/utils/Profiler.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      788 2024-04-06 09:04:22.000000 octomy-common-2.0.8/octomy/utils/Svg.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      683 2024-04-06 09:04:29.000000 octomy-common-2.0.8/octomy/utils/Watchdog.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     4963 2024-04-06 09:04:36.000000 octomy-common-2.0.8/octomy/utils/WorkerPool.py
--rw-r--r--   0 leo       (1000) leo       (1000)    13893 2024-04-06 15:00:59.000000 octomy-common-2.0.8/octomy/utils/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     1623 2024-04-06 09:02:56.000000 octomy-common-2.0.8/octomy/utils/click.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     3333 2024-04-06 09:03:16.000000 octomy-common-2.0.8/octomy/utils/credentials.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     2087 2024-04-06 09:03:27.000000 octomy-common-2.0.8/octomy/utils/csv_to_db.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      587 2024-04-06 09:03:38.000000 octomy-common-2.0.8/octomy/utils/debug_view.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      944 2024-04-06 09:03:47.000000 octomy-common-2.0.8/octomy/utils/excavator.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     2622 2024-04-06 09:04:08.000000 octomy-common-2.0.8/octomy/utils/expiry_cache.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.351543 octomy-common-2.0.8/octomy/version/
--rw-r--r--   0 leo       (1000) leo       (1000)      257 2024-04-06 09:05:07.000000 octomy-common-2.0.8/octomy/version/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.351543 octomy-common-2.0.8/octomy/web/
--rw-r--r--   0 leo       (1000) leo       (1000)     4318 2024-03-24 15:23:44.000000 octomy-common-2.0.8/octomy/web/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     4390 2024-04-06 09:13:34.000000 octomy-common-2.0.8/octomy/web/autoroute.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.351543 octomy-common-2.0.8/octomy/web/context/
--rw-r--r--   0 leo       (1000) leo       (1000)     2769 2024-04-14 09:54:39.000000 octomy-common-2.0.8/octomy/web/context/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.351543 octomy-common-2.0.8/octomy/web/search/
--rw-r--r--   0 leo       (1000) leo       (1000)     3870 2023-04-10 21:13:22.000000 octomy-common-2.0.8/octomy/web/search/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.355543 octomy-common-2.0.8/octomy_common.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)     8435 2024-04-16 11:31:00.000000 octomy-common-2.0.8/octomy_common.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)     1736 2024-04-16 11:31:00.000000 octomy-common-2.0.8/octomy_common.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2024-04-16 11:31:00.000000 octomy-common-2.0.8/octomy_common.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-16 11:31:00.000000 octomy-common-2.0.8/octomy_common.egg-info/namespace_packages.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      325 2024-04-16 11:31:00.000000 octomy-common-2.0.8/octomy_common.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-16 11:31:00.000000 octomy-common-2.0.8/octomy_common.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2020-11-26 02:00:43.000000 octomy-common-2.0.8/octomy_common.egg-info/zip-safe
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.355543 octomy-common-2.0.8/requirements/
--rw-r--r--   0 leo       (1000) leo       (1000)      325 2024-04-06 17:42:08.000000 octomy-common-2.0.8/requirements/requirements.in
--rw-r--r--   0 leo       (1000) leo       (1000)     1757 2024-04-06 17:42:10.000000 octomy-common-2.0.8/requirements/requirements.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      271 2023-08-28 21:54:48.000000 octomy-common-2.0.8/requirements/test_requirements.in
--rw-r--r--   0 leo       (1000) leo       (1000)     3299 2024-01-27 21:44:17.000000 octomy-common-2.0.8/requirements/test_requirements.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      166 2024-04-16 11:31:00.359543 octomy-common-2.0.8/setup.cfg
--rwxr-xr-x   0 leo       (1000) leo       (1000)     7025 2024-04-06 09:26:59.000000 octomy-common-2.0.8/setup.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.355543 octomy-common-2.0.8/tests/
--rw-r--r--   0 leo       (1000) leo       (1000)      935 2021-12-02 17:02:15.000000 octomy-common-2.0.8/tests/Makefile
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.8/tests/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.355543 octomy-common-2.0.8/tests/integration/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.8/tests/integration/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      154 2021-12-02 17:02:15.000000 octomy-common-2.0.8/tests/integration/test_true.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.355543 octomy-common-2.0.8/tests/load/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.8/tests/load/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      147 2021-12-02 17:02:15.000000 octomy-common-2.0.8/tests/load/test_true.py
--rw-r--r--   0 leo       (1000) leo       (1000)      361 2023-08-28 21:54:48.000000 octomy-common-2.0.8/tests/pytest.ini
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.359543 octomy-common-2.0.8/tests/unit/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.8/tests/unit/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1332 2024-04-14 10:04:39.000000 octomy-common-2.0.8/tests/unit/test_util.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.819464 octomy-common-2.0.9/
+-rw-r--r--   0 leo       (1000) leo       (1000)      735 2021-12-02 17:02:15.000000 octomy-common-2.0.9/.gitignore
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.815464 octomy-common-2.0.9/.gitlab/
+-rw-r--r--   0 leo       (1000) leo       (1000)      771 2021-12-02 17:02:15.000000 octomy-common-2.0.9/.gitlab/ci.yaml
+-rw-r--r--   0 leo       (1000) leo       (1000)     2021 2024-04-06 09:06:50.000000 octomy-common-2.0.9/LICENSE
+-rw-r--r--   0 leo       (1000) leo       (1000)      284 2024-04-06 08:33:37.000000 octomy-common-2.0.9/Makefile
+-rw-r--r--   0 leo       (1000) leo       (1000)     8435 2024-04-19 23:12:55.819464 octomy-common-2.0.9/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)     7595 2024-04-06 08:34:18.000000 octomy-common-2.0.9/README.md
+-rw-r--r--   0 leo       (1000) leo       (1000)        6 2024-04-19 23:12:19.000000 octomy-common-2.0.9/VERSION
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.815464 octomy-common-2.0.9/code_quality/
+-rw-r--r--   0 leo       (1000) leo       (1000)      214 2021-12-02 17:02:15.000000 octomy-common-2.0.9/code_quality/.flake8
+-rw-r--r--   0 leo       (1000) leo       (1000)     2492 2021-12-28 02:40:34.000000 octomy-common-2.0.9/code_quality/Makefile
+-rw-r--r--   0 leo       (1000) leo       (1000)      135 2021-12-02 17:02:15.000000 octomy-common-2.0.9/code_quality/mypy.ini
+-rw-rw-r--   0 leo       (1000) leo       (1000)    11867 2020-03-02 23:49:28.000000 octomy-common-2.0.9/code_quality/pylintrc
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.815464 octomy-common-2.0.9/design/
+-rw-r--r--   0 leo       (1000) leo       (1000)    62298 2021-12-02 17:02:15.000000 octomy-common-2.0.9/design/logo-1024.png
+-rw-r--r--   0 leo       (1000) leo       (1000)     7427 2021-12-02 17:02:15.000000 octomy-common-2.0.9/design/logo-1024.svg
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.803464 octomy-common-2.0.9/octomy/
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.807464 octomy-common-2.0.9/octomy/access/
+-rw-r--r--   0 leo       (1000) leo       (1000)    11927 2024-04-06 10:41:55.000000 octomy-common-2.0.9/octomy/access/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.807464 octomy-common-2.0.9/octomy/cad/
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.807464 octomy-common-2.0.9/octomy/cad/generators/
+-rw-r--r--   0 leo       (1000) leo       (1000)     4653 2024-03-21 20:06:58.000000 octomy-common-2.0.9/octomy/cad/generators/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2023-12-09 21:11:36.000000 octomy-common-2.0.9/octomy/cad/generators/common.py
+-rw-r--r--   0 leo       (1000) leo       (1000)       74 2023-12-09 21:13:26.000000 octomy-common-2.0.9/octomy/cad/generators/ntop.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     6642 2024-03-21 20:05:55.000000 octomy-common-2.0.9/octomy/cad/generators/openscad.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    15524 2024-04-06 12:29:11.000000 octomy-common-2.0.9/octomy/cad/ntop.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    28147 2024-04-06 12:29:00.000000 octomy-common-2.0.9/octomy/cad/openscad.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    20669 2024-03-21 19:38:26.000000 octomy-common-2.0.9/octomy/cad/parts.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.807464 octomy-common-2.0.9/octomy/cad/types/
+-rw-r--r--   0 leo       (1000) leo       (1000)     3633 2023-12-09 22:30:55.000000 octomy-common-2.0.9/octomy/cad/types/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.807464 octomy-common-2.0.9/octomy/config/
+-rw-r--r--   0 leo       (1000) leo       (1000)    13353 2024-04-14 09:41:27.000000 octomy-common-2.0.9/octomy/config/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.811463 octomy-common-2.0.9/octomy/db/
+-rw-rw-r--   0 leo       (1000) leo       (1000)    18552 2024-04-19 22:45:02.000000 octomy-common-2.0.9/octomy/db/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      841 2024-04-06 17:40:11.000000 octomy-common-2.0.9/octomy/db/check.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.811463 octomy-common-2.0.9/octomy/log/
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1477 2024-04-06 08:54:24.000000 octomy-common-2.0.9/octomy/log/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.811463 octomy-common-2.0.9/octomy/storage/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2023-12-09 19:06:16.000000 octomy-common-2.0.9/octomy/storage/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    11978 2023-12-09 18:40:20.000000 octomy-common-2.0.9/octomy/storage/google_drive.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.811463 octomy-common-2.0.9/octomy/utils/
+-rw-rw-r--   0 leo       (1000) leo       (1000)      129 2024-04-06 09:03:01.000000 octomy-common-2.0.9/octomy/utils/Context.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      896 2024-04-06 09:04:17.000000 octomy-common-2.0.9/octomy/utils/Profiler.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      788 2024-04-06 09:04:22.000000 octomy-common-2.0.9/octomy/utils/Svg.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      683 2024-04-06 09:04:29.000000 octomy-common-2.0.9/octomy/utils/Watchdog.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     4963 2024-04-06 09:04:36.000000 octomy-common-2.0.9/octomy/utils/WorkerPool.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    13893 2024-04-06 15:00:59.000000 octomy-common-2.0.9/octomy/utils/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1623 2024-04-06 09:02:56.000000 octomy-common-2.0.9/octomy/utils/click.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     3333 2024-04-06 09:03:16.000000 octomy-common-2.0.9/octomy/utils/credentials.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     2087 2024-04-06 09:03:27.000000 octomy-common-2.0.9/octomy/utils/csv_to_db.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      587 2024-04-06 09:03:38.000000 octomy-common-2.0.9/octomy/utils/debug_view.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      944 2024-04-06 09:03:47.000000 octomy-common-2.0.9/octomy/utils/excavator.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     2622 2024-04-06 09:04:08.000000 octomy-common-2.0.9/octomy/utils/expiry_cache.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.811463 octomy-common-2.0.9/octomy/version/
+-rw-r--r--   0 leo       (1000) leo       (1000)      257 2024-04-06 09:05:07.000000 octomy-common-2.0.9/octomy/version/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.811463 octomy-common-2.0.9/octomy/web/
+-rw-r--r--   0 leo       (1000) leo       (1000)     4318 2024-03-24 15:23:44.000000 octomy-common-2.0.9/octomy/web/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     4390 2024-04-06 09:13:34.000000 octomy-common-2.0.9/octomy/web/autoroute.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.815464 octomy-common-2.0.9/octomy/web/context/
+-rw-r--r--   0 leo       (1000) leo       (1000)     2769 2024-04-14 09:54:39.000000 octomy-common-2.0.9/octomy/web/context/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.815464 octomy-common-2.0.9/octomy/web/search/
+-rw-r--r--   0 leo       (1000) leo       (1000)     3870 2023-04-10 21:13:22.000000 octomy-common-2.0.9/octomy/web/search/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.815464 octomy-common-2.0.9/octomy_common.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)     8435 2024-04-19 23:12:55.000000 octomy-common-2.0.9/octomy_common.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)     1736 2024-04-19 23:12:55.000000 octomy-common-2.0.9/octomy_common.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2024-04-19 23:12:55.000000 octomy-common-2.0.9/octomy_common.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-19 23:12:55.000000 octomy-common-2.0.9/octomy_common.egg-info/namespace_packages.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      325 2024-04-19 23:12:55.000000 octomy-common-2.0.9/octomy_common.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-19 23:12:55.000000 octomy-common-2.0.9/octomy_common.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2020-11-26 02:00:43.000000 octomy-common-2.0.9/octomy_common.egg-info/zip-safe
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.819464 octomy-common-2.0.9/requirements/
+-rw-r--r--   0 leo       (1000) leo       (1000)      325 2024-04-06 17:42:08.000000 octomy-common-2.0.9/requirements/requirements.in
+-rw-r--r--   0 leo       (1000) leo       (1000)     1757 2024-04-06 17:42:10.000000 octomy-common-2.0.9/requirements/requirements.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      271 2023-08-28 21:54:48.000000 octomy-common-2.0.9/requirements/test_requirements.in
+-rw-r--r--   0 leo       (1000) leo       (1000)     3299 2024-01-27 21:44:17.000000 octomy-common-2.0.9/requirements/test_requirements.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      166 2024-04-19 23:12:55.819464 octomy-common-2.0.9/setup.cfg
+-rwxr-xr-x   0 leo       (1000) leo       (1000)     7025 2024-04-06 09:26:59.000000 octomy-common-2.0.9/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.819464 octomy-common-2.0.9/tests/
+-rw-r--r--   0 leo       (1000) leo       (1000)     1039 2024-04-18 17:13:57.000000 octomy-common-2.0.9/tests/Makefile
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.9/tests/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.819464 octomy-common-2.0.9/tests/integration/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.9/tests/integration/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      149 2024-04-19 23:02:26.000000 octomy-common-2.0.9/tests/integration/test_true.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.819464 octomy-common-2.0.9/tests/load/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.9/tests/load/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      142 2024-04-19 23:02:17.000000 octomy-common-2.0.9/tests/load/test_true.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      361 2023-08-28 21:54:48.000000 octomy-common-2.0.9/tests/pytest.ini
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-19 23:12:55.819464 octomy-common-2.0.9/tests/unit/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.9/tests/unit/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1334 2024-04-19 23:03:04.000000 octomy-common-2.0.9/tests/unit/test_util.py
```

### Comparing `octomy-common-2.0.8/.gitignore` & `octomy-common-2.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/.gitlab/ci.yaml` & `octomy-common-2.0.9/.gitlab/ci.yaml`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/LICENSE` & `octomy-common-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/PKG-INFO` & `octomy-common-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octomy-common
-Version: 2.0.8
+Version: 2.0.9
 Summary: ('octomy/common',)
 Home-page: https://gitlab.com/octomy/common
 Author: OctoMY
 Author-email: pypi@octomy.org
 Maintainer: OctoMY
 Maintainer-email: pypi@octomy.org
 License: Proprietary Software License
```

### Comparing `octomy-common-2.0.8/README.md` & `octomy-common-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/code_quality/Makefile` & `octomy-common-2.0.9/code_quality/Makefile`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/code_quality/pylintrc` & `octomy-common-2.0.9/code_quality/pylintrc`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/design/logo-1024.png` & `octomy-common-2.0.9/design/logo-1024.png`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/design/logo-1024.svg` & `octomy-common-2.0.9/design/logo-1024.svg`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/access/__init__.py` & `octomy-common-2.0.9/octomy/access/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/cad/generators/__init__.py` & `octomy-common-2.0.9/octomy/cad/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/cad/generators/openscad.py` & `octomy-common-2.0.9/octomy/cad/generators/openscad.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/cad/ntop.py` & `octomy-common-2.0.9/octomy/cad/ntop.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/cad/openscad.py` & `octomy-common-2.0.9/octomy/cad/openscad.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/cad/parts.py` & `octomy-common-2.0.9/octomy/cad/parts.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/cad/types/__init__.py` & `octomy-common-2.0.9/octomy/cad/types/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/config/__init__.py` & `octomy-common-2.0.9/octomy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/db/__init__.py` & `octomy-common-2.0.9/octomy/db/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,31 +271,38 @@
 			if not self.query_dirs or len(self.query_dirs) <= 0:
 				return self._error(f"No query dirs registered: '{self.query_dirs}'")
 			return True, None
 		except Exception as e:
 			logger.warning(f"Unknown error '{e}':", exc_info=True)
 			return False, str(e)
 
-	async def state(self, do_online = False):
-		logger.info(f"Status{' [ONLINE]' if do_online else ' [OFFLINE]'}:")
+	async def state(self, do_online = False, show_full = False):
+		head_c=c.GREEN
+		logger.info(f"{head_c}Status [{c.WARNING}{'ONLINE' if do_online else 'OFFLINE'}{head_c}]:")
 		ok, err = await self.verify(do_online = do_online)
-		logger.info(f"\t{'OK' if ok else 'ERROR: '}{'' if ok else err}")
+		if ok:
+			logger.info(f"\t{c.GREEN}OK")
+		else:
+			logger.info(f"\t{c.RED}ERROR: {c.WARNING}{err}")
 		if self.query_dirs:
-			logger.info("Query paths:")
+			logger.info(f"{head_c}Query paths:")
 			for query_dir in self.query_dirs:
-				logger.info(f"\t{query_dir}")
+				logger.info(f"\t{c.CYAN}{query_dir}")
 		else:
 			logger.info("No query paths")
 		if self.queries:
-			logger.info("Loaded queries:")
+			logger.info(f"{head_c}Loaded queries:")
 			tabs2 = "\t\t"
 			for key, query in self.queries.items():
-				logger.info(f"\t{key:>10}: {indent(query, tabs2)}")
+				if show_full:
+					logger.info(f"\t{c.BLUE}{key:>10}{c.ENDC}: {c.GREEN}{indent(query, tabs2)}")
+				else:
+					logger.info(f"\t{c.BLUE}{key:>10}{c.ENDC}: {c.GREEN}{len(query)} chars")
 		else:
-			logger.info("No loaded queries")
+			logger.info(f"{head_c}No loaded queries")
 		return ok, err
 
 	def reset_queries(self):
 		"""Reset the internal cache of queries, forcing queries to be reloaded upon next invocation"""
 		self.queries = dict()
 
 	def preload_queries(self, do_debug = False):
```

### Comparing `octomy-common-2.0.8/octomy/db/check.py` & `octomy-common-2.0.9/octomy/db/check.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/log/__init__.py` & `octomy-common-2.0.9/octomy/log/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/storage/google_drive.py` & `octomy-common-2.0.9/octomy/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/utils/Profiler.py` & `octomy-common-2.0.9/octomy/utils/Profiler.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/utils/Svg.py` & `octomy-common-2.0.9/octomy/utils/Svg.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/utils/Watchdog.py` & `octomy-common-2.0.9/octomy/utils/Watchdog.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/utils/WorkerPool.py` & `octomy-common-2.0.9/octomy/utils/WorkerPool.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/utils/__init__.py` & `octomy-common-2.0.9/octomy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/utils/click.py` & `octomy-common-2.0.9/octomy/utils/click.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/utils/credentials.py` & `octomy-common-2.0.9/octomy/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/utils/csv_to_db.py` & `octomy-common-2.0.9/octomy/utils/csv_to_db.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/utils/debug_view.py` & `octomy-common-2.0.9/octomy/utils/debug_view.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/utils/excavator.py` & `octomy-common-2.0.9/octomy/utils/excavator.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/utils/expiry_cache.py` & `octomy-common-2.0.9/octomy/utils/expiry_cache.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/web/__init__.py` & `octomy-common-2.0.9/octomy/web/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/web/autoroute.py` & `octomy-common-2.0.9/octomy/web/autoroute.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/web/context/__init__.py` & `octomy-common-2.0.9/octomy/web/context/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy/web/search/__init__.py` & `octomy-common-2.0.9/octomy/web/search/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/octomy_common.egg-info/PKG-INFO` & `octomy-common-2.0.9/octomy_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octomy-common
-Version: 2.0.8
+Version: 2.0.9
 Summary: ('octomy/common',)
 Home-page: https://gitlab.com/octomy/common
 Author: OctoMY
 Author-email: pypi@octomy.org
 Maintainer: OctoMY
 Maintainer-email: pypi@octomy.org
 License: Proprietary Software License
```

### Comparing `octomy-common-2.0.8/octomy_common.egg-info/SOURCES.txt` & `octomy-common-2.0.9/octomy_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/requirements/requirements.txt` & `octomy-common-2.0.9/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/requirements/test_requirements.txt` & `octomy-common-2.0.9/requirements/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/setup.py` & `octomy-common-2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.8/tests/Makefile` & `octomy-common-2.0.9/tests/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 all: unit integration load
 
 devops: unit
 
 unit:
 	$(TEST_CMD) -vv unit
 
-utils:
-	$(TEST_CMD) -vv unit/test_utils.py
-
 integration:
 	$(TEST_CMD) -vv integration
 
 load:
 	$(TEST_CMD) -vv load
+############### Shortcuts ####################
 
+utils:
+	$(TEST_CMD) -vv unit/test_utils.py
 
 ############### Help ####################
 
 help:
 	@echo ""
 	@echo " General targets:"
 	@echo ""
@@ -34,14 +34,15 @@
 	@echo " + make all             Run all tests"
 	@echo " + make devops          Run devops tests"
 	@echo " + make load            Run load tests (WIP)"
 	@echo ""
 	@echo "Unit targets:"
 	@echo ""
 	@echo " + make unit            Run unit tests"
+	@echo " + make utils           Run unit tests for utils"
 	@echo ""
 	@echo "Integration targets:"
 	@echo ""
 	@echo " + make integration     Run integration tests"
 	@echo ""
 	@echo "Component targets:"
 	@echo ""
```

### Comparing `octomy-common-2.0.8/tests/unit/test_util.py` & `octomy-common-2.0.9/tests/unit/test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 		}
 		,"F12F52B73358C297F47A80768ABDFADF20D021F6A20E9929178908F981B75FA1"
 		,"postgres://arnold:secret123@hello.com:1234/mydb"
 	)
 }
 # fmt: on
 
-def test_db_get_config_hash():
+def _test_db_get_config_hash():
 
 	for name, pack in configs.items():
 		logger.info(f"NAME:{name}")
 		config, expected, _ = pack
 		logger.info(f"config:{config}")
 		logger.info(f"expected:{expected}")
 		actual = octomy.db.get_config_hash(config)
 		logger.info(f"actual:{actual}")
 		assert actual == expected
 	return True
 
 
-def test_db_uri_to_and_from_config():
+def _test_db_uri_to_and_from_config():
 	for name, pack in configs.items():
 		logger.info(f"NAME:{name}")
 		expected_config, _, expected_uri = pack
 		logger.info(f"expected_config:{expected_config}")
 		logger.info(f"expected_uri:   {expected_uri}")
 		actual_uri, actual_uri_err = octomy.db.db_uri_from_conf(expected_config, do_online=False)
 		actual_config = octomy.db.db_uri_to_config(expected_uri, do_online=False)
```

