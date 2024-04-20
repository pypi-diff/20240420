# Comparing `tmp/pbix_chinese-23.7.8.tar.gz` & `tmp/pbix_chinese-24.4.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbix_chinese-23.7.8.tar", last modified: Sat Jul 29 10:06:53 2023, max compression
+gzip compressed data, was "pbix_chinese-24.4.20.tar", last modified: Sat Apr 20 02:37:55 2024, max compression
```

## Comparing `pbix_chinese-23.7.8.tar` & `pbix_chinese-24.4.20.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 10:06:53.582476 pbix_chinese-23.7.8/
--rw-rw-rw-   0        0        0       99 2023-07-29 10:06:53.581475 pbix_chinese-23.7.8/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-07-17 07:47:27.000000 pbix_chinese-23.7.8/README.txt
--rw-rw-rw-   0        0        0       52 2023-07-15 07:22:48.000000 pbix_chinese-23.7.8/license.txt
-drwxrwxrwx   0        0        0        0 2023-07-29 10:06:53.567484 pbix_chinese-23.7.8/pbix_chinese/
--rw-rw-rw-   0        0        0       51 2023-07-17 07:53:45.000000 pbix_chinese-23.7.8/pbix_chinese/__init__.py
--rw-rw-rw-   0        0        0     2053 2023-07-29 10:06:20.000000 pbix_chinese-23.7.8/pbix_chinese/pbix_refresher.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:06:53.577478 pbix_chinese-23.7.8/pbix_chinese.egg-info/
--rw-rw-rw-   0        0        0       99 2023-07-29 10:06:53.000000 pbix_chinese-23.7.8/pbix_chinese.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-07-29 10:06:53.000000 pbix_chinese-23.7.8/pbix_chinese.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 10:06:53.000000 pbix_chinese-23.7.8/pbix_chinese.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-29 10:06:53.000000 pbix_chinese-23.7.8/pbix_chinese.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 10:06:53.582476 pbix_chinese-23.7.8/setup.cfg
--rw-rw-rw-   0        0        0      221 2023-07-29 09:51:52.000000 pbix_chinese-23.7.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 02:37:55.376219 pbix_chinese-24.4.20/
+-rw-rw-rw-   0        0        0      160 2024-04-20 02:37:55.374232 pbix_chinese-24.4.20/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2024-04-06 07:18:35.000000 pbix_chinese-24.4.20/README.txt
+-rw-rw-rw-   0        0        0       52 2024-04-06 07:14:29.000000 pbix_chinese-24.4.20/license.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 02:37:55.369505 pbix_chinese-24.4.20/pbix_chinese/
+-rw-rw-rw-   0        0        0     1376 2024-04-06 06:51:19.000000 pbix_chinese-24.4.20/pbix_chinese/pbix_refresher.py
+drwxrwxrwx   0        0        0        0 2024-04-20 02:37:55.372218 pbix_chinese-24.4.20/pbix_chinese.egg-info/
+-rw-rw-rw-   0        0        0      160 2024-04-20 02:37:55.000000 pbix_chinese-24.4.20/pbix_chinese.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2024-04-20 02:37:55.000000 pbix_chinese-24.4.20/pbix_chinese.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 02:37:55.000000 pbix_chinese-24.4.20/pbix_chinese.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-20 02:37:55.000000 pbix_chinese-24.4.20/pbix_chinese.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 02:37:55.377222 pbix_chinese-24.4.20/setup.cfg
+-rw-rw-rw-   0        0        0      282 2024-04-20 02:36:37.000000 pbix_chinese-24.4.20/setup.py
```

