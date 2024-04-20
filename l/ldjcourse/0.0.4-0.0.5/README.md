# Comparing `tmp/ldjcourse-0.0.4.tar.gz` & `tmp/ldjcourse-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ldjcourse-0.0.4.tar", last modified: Sat Apr 20 05:53:01 2024, max compression
+gzip compressed data, was "dist\ldjcourse-0.0.5.tar", last modified: Sat Apr 20 07:05:03 2024, max compression
```

## Comparing `ldjcourse-0.0.4.tar` & `ldjcourse-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 05:53:01.236365 ldjcourse-0.0.4/
--rw-rw-rw-   0        0        0      166 2024-04-20 05:53:01.228826 ldjcourse-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-20 05:53:01.158324 ldjcourse-0.0.4/ldjcourse/
--rw-rw-rw-   0        0        0        0 2024-04-06 11:24:13.000000 ldjcourse-0.0.4/ldjcourse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 05:53:01.181924 ldjcourse-0.0.4/ldjcourse/pandas/
--rw-rw-rw-   0        0        0        0 2024-04-20 04:41:18.000000 ldjcourse-0.0.4/ldjcourse/pandas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 05:53:01.216234 ldjcourse-0.0.4/ldjcourse/pandas/v1_1/
--rw-rw-rw-   0        0        0        0 2024-04-06 11:25:30.000000 ldjcourse-0.0.4/ldjcourse/pandas/v1_1/__init__.py
--rw-rw-rw-   0        0        0      295 2024-04-20 05:52:58.000000 ldjcourse-0.0.4/ldjcourse/pandas/v1_1/api.py
--rw-rw-rw-   0        0        0      578 2024-04-20 04:55:25.000000 ldjcourse-0.0.4/ldjcourse/pandas/v1_1/data.py
--rw-rw-rw-   0        0        0       22 2024-04-20 04:51:34.000000 ldjcourse-0.0.4/ldjcourse/pandas/v1_1/setting.py
-drwxrwxrwx   0        0        0        0 2024-04-20 05:53:01.224924 ldjcourse-0.0.4/ldjcourse.egg-info/
--rw-rw-rw-   0        0        0      166 2024-04-20 05:53:00.000000 ldjcourse-0.0.4/ldjcourse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2024-04-20 05:53:01.000000 ldjcourse-0.0.4/ldjcourse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 05:53:00.000000 ldjcourse-0.0.4/ldjcourse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-20 05:53:00.000000 ldjcourse-0.0.4/ldjcourse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 05:53:01.237299 ldjcourse-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      358 2024-04-20 05:52:58.000000 ldjcourse-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:05:03.326025 ldjcourse-0.0.5/
+-rw-rw-rw-   0        0        0      166 2024-04-20 07:05:03.318678 ldjcourse-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-20 07:05:03.229498 ldjcourse-0.0.5/ldjcourse/
+-rw-rw-rw-   0        0        0        0 2024-04-06 11:24:13.000000 ldjcourse-0.0.5/ldjcourse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:05:03.267456 ldjcourse-0.0.5/ldjcourse/pandas/
+-rw-rw-rw-   0        0        0        0 2024-04-20 04:41:18.000000 ldjcourse-0.0.5/ldjcourse/pandas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:05:03.300222 ldjcourse-0.0.5/ldjcourse/pandas/v1_1/
+-rw-rw-rw-   0        0        0        0 2024-04-06 11:25:30.000000 ldjcourse-0.0.5/ldjcourse/pandas/v1_1/__init__.py
+-rw-rw-rw-   0        0        0      295 2024-04-20 05:52:58.000000 ldjcourse-0.0.5/ldjcourse/pandas/v1_1/api.py
+-rw-rw-rw-   0        0        0     1330 2024-04-20 07:04:45.000000 ldjcourse-0.0.5/ldjcourse/pandas/v1_1/data.py
+-rw-rw-rw-   0        0        0       22 2024-04-20 04:51:34.000000 ldjcourse-0.0.5/ldjcourse/pandas/v1_1/setting.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:05:03.311364 ldjcourse-0.0.5/ldjcourse.egg-info/
+-rw-rw-rw-   0        0        0      166 2024-04-20 07:05:03.000000 ldjcourse-0.0.5/ldjcourse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-04-20 07:05:03.000000 ldjcourse-0.0.5/ldjcourse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 07:05:03.000000 ldjcourse-0.0.5/ldjcourse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-20 07:05:03.000000 ldjcourse-0.0.5/ldjcourse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 07:05:03.326669 ldjcourse-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      358 2024-04-20 07:05:00.000000 ldjcourse-0.0.5/setup.py
```

