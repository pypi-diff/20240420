# Comparing `tmp/ldjcourse-0.0.2.tar.gz` & `tmp/ldjcourse-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ldjcourse-0.0.2.tar", last modified: Sat Apr 20 05:41:11 2024, max compression
+gzip compressed data, was "dist\ldjcourse-0.0.3.tar", last modified: Sat Apr 20 05:50:23 2024, max compression
```

## Comparing `ldjcourse-0.0.2.tar` & `ldjcourse-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 05:41:11.080752 ldjcourse-0.0.2/
--rw-rw-rw-   0        0        0      166 2024-04-20 05:41:11.074665 ldjcourse-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-20 05:41:10.991685 ldjcourse-0.0.2/ldjcourse/
--rw-rw-rw-   0        0        0        0 2024-04-06 11:24:13.000000 ldjcourse-0.0.2/ldjcourse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 05:41:11.015249 ldjcourse-0.0.2/ldjcourse/pandas/
--rw-rw-rw-   0        0        0        0 2024-04-20 04:41:18.000000 ldjcourse-0.0.2/ldjcourse/pandas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 05:41:11.052453 ldjcourse-0.0.2/ldjcourse/pandas/v1_1/
--rw-rw-rw-   0        0        0        0 2024-04-06 11:25:30.000000 ldjcourse-0.0.2/ldjcourse/pandas/v1_1/__init__.py
--rw-rw-rw-   0        0        0      278 2024-04-20 05:40:52.000000 ldjcourse-0.0.2/ldjcourse/pandas/v1_1/api.py
--rw-rw-rw-   0        0        0      578 2024-04-20 04:55:25.000000 ldjcourse-0.0.2/ldjcourse/pandas/v1_1/data.py
--rw-rw-rw-   0        0        0       22 2024-04-20 04:51:34.000000 ldjcourse-0.0.2/ldjcourse/pandas/v1_1/setting.py
-drwxrwxrwx   0        0        0        0 2024-04-20 05:41:11.067708 ldjcourse-0.0.2/ldjcourse.egg-info/
--rw-rw-rw-   0        0        0      166 2024-04-20 05:41:10.000000 ldjcourse-0.0.2/ldjcourse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2024-04-20 05:41:10.000000 ldjcourse-0.0.2/ldjcourse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 05:41:10.000000 ldjcourse-0.0.2/ldjcourse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-20 05:41:10.000000 ldjcourse-0.0.2/ldjcourse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 05:41:11.081526 ldjcourse-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      358 2024-04-20 05:41:08.000000 ldjcourse-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 05:50:23.389980 ldjcourse-0.0.3/
+-rw-rw-rw-   0        0        0      166 2024-04-20 05:50:23.380874 ldjcourse-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-20 05:50:23.314134 ldjcourse-0.0.3/ldjcourse/
+-rw-rw-rw-   0        0        0        0 2024-04-06 11:24:13.000000 ldjcourse-0.0.3/ldjcourse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 05:50:23.336047 ldjcourse-0.0.3/ldjcourse/pandas/
+-rw-rw-rw-   0        0        0        0 2024-04-20 04:41:18.000000 ldjcourse-0.0.3/ldjcourse/pandas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 05:50:23.365925 ldjcourse-0.0.3/ldjcourse/pandas/v1_1/
+-rw-rw-rw-   0        0        0        0 2024-04-06 11:25:30.000000 ldjcourse-0.0.3/ldjcourse/pandas/v1_1/__init__.py
+-rw-rw-rw-   0        0        0      280 2024-04-20 05:47:51.000000 ldjcourse-0.0.3/ldjcourse/pandas/v1_1/api.py
+-rw-rw-rw-   0        0        0      578 2024-04-20 04:55:25.000000 ldjcourse-0.0.3/ldjcourse/pandas/v1_1/data.py
+-rw-rw-rw-   0        0        0       22 2024-04-20 04:51:34.000000 ldjcourse-0.0.3/ldjcourse/pandas/v1_1/setting.py
+drwxrwxrwx   0        0        0        0 2024-04-20 05:50:23.374976 ldjcourse-0.0.3/ldjcourse.egg-info/
+-rw-rw-rw-   0        0        0      166 2024-04-20 05:50:23.000000 ldjcourse-0.0.3/ldjcourse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-04-20 05:50:23.000000 ldjcourse-0.0.3/ldjcourse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 05:50:23.000000 ldjcourse-0.0.3/ldjcourse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-20 05:50:23.000000 ldjcourse-0.0.3/ldjcourse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 05:50:23.390606 ldjcourse-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      358 2024-04-20 05:50:21.000000 ldjcourse-0.0.3/setup.py
```

### Comparing `ldjcourse-0.0.2/ldjcourse/pandas/v1_1/data.py` & `ldjcourse-0.0.3/ldjcourse/pandas/v1_1/data.py`

 * *Files identical despite different names*

