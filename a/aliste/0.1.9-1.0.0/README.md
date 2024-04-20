# Comparing `tmp/aliste-0.1.9.tar.gz` & `tmp/aliste-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aliste-0.1.9.tar", last modified: Fri Oct 13 12:20:08 2023, max compression
+gzip compressed data, was "aliste-1.0.0.tar", max compression
```

## Comparing `aliste-0.1.9.tar` & `aliste-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-10-13 12:20:08.423065 aliste-0.1.9/
--rw-rw-rw-   0        0        0     1089 2023-07-11 08:03:48.000000 aliste-0.1.9/LICENSE
--rw-rw-rw-   0        0        0      763 2023-10-13 12:20:08.423065 aliste-0.1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-10-13 12:20:08.417769 aliste-0.1.9/aliste/
--rw-rw-rw-   0        0        0       26 2023-07-11 13:34:58.000000 aliste-0.1.9/aliste/__init__.py
--rw-rw-rw-   0        0        0     1567 2023-10-13 12:19:21.000000 aliste-0.1.9/aliste/broker.py
--rw-rw-rw-   0        0        0      346 2023-10-13 11:08:39.000000 aliste-0.1.9/aliste/constants.py
--rw-rw-rw-   0        0        0     1952 2023-07-12 08:19:09.000000 aliste-0.1.9/aliste/device.py
--rw-rw-rw-   0        0        0      145 2023-07-11 11:16:10.000000 aliste-0.1.9/aliste/enums.py
--rw-rw-rw-   0        0        0      346 2023-07-11 13:20:17.000000 aliste-0.1.9/aliste/home.py
--rw-rw-rw-   0        0        0     2628 2023-07-11 15:18:00.000000 aliste-0.1.9/aliste/hub.py
--rw-rw-rw-   0        0        0      353 2023-07-11 11:01:22.000000 aliste-0.1.9/aliste/user.py
--rw-rw-rw-   0        0        0      230 2023-07-11 15:34:53.000000 aliste-0.1.9/aliste/utils.py
-drwxrwxrwx   0        0        0        0 2023-10-13 12:20:08.422062 aliste-0.1.9/aliste.egg-info/
--rw-rw-rw-   0        0        0      763 2023-10-13 12:20:08.000000 aliste-0.1.9/aliste.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-10-13 12:20:08.000000 aliste-0.1.9/aliste.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-13 12:20:08.000000 aliste-0.1.9/aliste.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-10-13 12:20:08.000000 aliste-0.1.9/aliste.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-13 12:20:08.423065 aliste-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      994 2023-10-13 12:19:32.000000 aliste-0.1.9/setup.py
+-rw-r--r--   0        0        0     1068 2024-04-20 16:05:43.312360 aliste-1.0.0/LICENSE
+-rw-r--r--   0        0        0      356 2024-04-20 16:05:43.312360 aliste-1.0.0/README.md
+-rw-r--r--   0        0        0       25 2024-04-20 16:05:43.312360 aliste-1.0.0/aliste/__init__.py
+-rw-r--r--   0        0        0     3642 2024-04-20 16:05:43.312360 aliste-1.0.0/aliste/broker.py
+-rw-r--r--   0        0        0      517 2024-04-20 16:05:43.312360 aliste-1.0.0/aliste/constants.py
+-rw-r--r--   0        0        0     1884 2024-04-20 16:05:43.312360 aliste-1.0.0/aliste/device.py
+-rw-r--r--   0        0        0      136 2024-04-20 16:05:43.312360 aliste-1.0.0/aliste/enums.py
+-rw-r--r--   0        0        0      333 2024-04-20 16:05:43.312360 aliste-1.0.0/aliste/home.py
+-rw-r--r--   0        0        0     4705 2024-04-20 16:05:43.312360 aliste-1.0.0/aliste/hub.py
+-rw-r--r--   0        0        0      420 2024-04-20 16:05:43.312360 aliste-1.0.0/aliste/user.py
+-rw-r--r--   0        0        0      220 2024-04-20 16:05:43.312360 aliste-1.0.0/aliste/utils.py
+-rw-r--r--   0        0        0      464 2024-04-20 16:05:43.312360 aliste-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 aliste-1.0.0/PKG-INFO
```

