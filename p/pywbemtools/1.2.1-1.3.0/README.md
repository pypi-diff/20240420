# Comparing `tmp/pywbemtools-1.2.1.tar.gz` & `tmp/pywbemtools-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywbemtools-1.2.1.tar", last modified: Fri Mar 29 12:04:22 2024, max compression
+gzip compressed data, was "pywbemtools-1.3.0.tar", last modified: Sat Apr 20 11:03:34 2024, max compression
```

## Comparing `pywbemtools-1.2.1.tar` & `pywbemtools-1.3.0.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-03-29 12:04:22.409908 pywbemtools-1.2.1/
--rw-r--r--   0 maiera     (501) staff       (20)      205 2021-05-11 05:03:28.000000 pywbemtools-1.2.1/AUTHORS
--rw-r--r--   0 maiera     (501) staff       (20)    10173 2021-02-20 08:31:47.000000 pywbemtools-1.2.1/LICENSE.txt
--rw-r--r--   0 maiera     (501) staff       (20)      224 2024-03-29 12:03:22.000000 pywbemtools-1.2.1/MANIFEST.in
--rw-r--r--   0 maiera     (501) staff       (20)    13782 2024-03-29 12:04:22.409358 pywbemtools-1.2.1/PKG-INFO
--rw-r--r--   0 maiera     (501) staff       (20)    17745 2024-03-29 12:02:05.000000 pywbemtools-1.2.1/README.rst
--rw-r--r--   0 maiera     (501) staff       (20)    10381 2021-02-20 08:31:47.000000 pywbemtools-1.2.1/README_PYPI.rst
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-03-29 12:04:22.364606 pywbemtools-1.2.1/pywbemtools/
--rw-r--r--   0 maiera     (501) staff       (20)     1122 2021-02-20 08:31:47.000000 pywbemtools-1.2.1/pywbemtools/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)    12192 2023-03-13 16:54:53.000000 pywbemtools-1.2.1/pywbemtools/_click_extensions.py
--rw-r--r--   0 maiera     (501) staff       (20)     4917 2023-03-20 14:25:46.000000 pywbemtools-1.2.1/pywbemtools/_common_cmd_actions.py
--rw-r--r--   0 maiera     (501) staff       (20)     2089 2022-10-09 14:29:33.000000 pywbemtools-1.2.1/pywbemtools/_options.py
--rw-r--r--   0 maiera     (501) staff       (20)    19417 2022-10-16 19:08:08.000000 pywbemtools-1.2.1/pywbemtools/_output_formatting.py
--rw-r--r--   0 maiera     (501) staff       (20)     5744 2023-11-05 15:31:40.000000 pywbemtools-1.2.1/pywbemtools/_utils.py
--rw-r--r--   0 maiera     (501) staff       (20)      973 2024-03-29 12:02:08.000000 pywbemtools-1.2.1/pywbemtools/_version.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-03-29 12:04:22.400313 pywbemtools-1.2.1/pywbemtools/pywbemcli/
--rw-r--r--   0 maiera     (501) staff       (20)     2448 2024-03-29 12:02:05.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)    35899 2022-10-16 19:08:08.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_association_shrub.py
--rw-r--r--   0 maiera     (501) staff       (20)    20125 2022-10-09 14:29:33.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_cimvalueformatter.py
--rw-r--r--   0 maiera     (501) staff       (20)    36241 2022-10-16 19:08:08.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_class.py
--rw-r--r--   0 maiera     (501) staff       (20)    36773 2023-03-05 18:05:43.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_connection.py
--rw-r--r--   0 maiera     (501) staff       (20)     1442 2023-03-13 16:54:53.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_docs.py
--rw-r--r--   0 maiera     (501) staff       (20)    11053 2023-03-20 14:25:46.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_help.py
--rw-r--r--   0 maiera     (501) staff       (20)    66534 2023-03-05 18:05:43.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_instance.py
--rw-r--r--   0 maiera     (501) staff       (20)    13443 2022-10-09 14:29:33.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_namespace.py
--rw-r--r--   0 maiera     (501) staff       (20)    12074 2022-10-16 19:08:08.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_profile.py
--rw-r--r--   0 maiera     (501) staff       (20)     7316 2022-10-16 19:08:08.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_qualifier.py
--rw-r--r--   0 maiera     (501) staff       (20)    21798 2024-03-17 13:09:45.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_server.py
--rw-r--r--   0 maiera     (501) staff       (20)    22301 2022-10-09 14:29:33.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_statistics.py
--rw-r--r--   0 maiera     (501) staff       (20)    87470 2022-10-16 19:08:08.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_subscription.py
--rw-r--r--   0 maiera     (501) staff       (20)    52401 2023-03-05 18:05:39.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_common.py
--rw-r--r--   0 maiera     (501) staff       (20)    25686 2022-10-16 19:08:08.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_common_cmd_functions.py
--rw-r--r--   0 maiera     (501) staff       (20)     7447 2022-10-16 19:08:08.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_common_options.py
--rw-r--r--   0 maiera     (501) staff       (20)    24010 2022-10-09 14:29:33.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_connection_repository.py
--rw-r--r--   0 maiera     (501) staff       (20)    14883 2023-03-05 18:05:43.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_context_obj.py
--rw-r--r--   0 maiera     (501) staff       (20)    45120 2022-10-16 19:08:08.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_display_cimobjects.py
--rw-r--r--   0 maiera     (501) staff       (20)     9456 2022-10-09 14:29:33.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_displaytree.py
--rw-r--r--   0 maiera     (501) staff       (20)    26615 2022-10-09 14:29:33.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_pywbem_server.py
--rw-r--r--   0 maiera     (501) staff       (20)    31447 2023-03-13 16:55:24.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/_pywbemcli_operations.py
--rw-r--r--   0 maiera     (501) staff       (20)     4661 2022-10-09 14:29:33.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/config.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-03-29 12:04:22.400868 pywbemtools-1.2.1/pywbemtools/pywbemcli/mockscripts/
--rw-r--r--   0 maiera     (501) staff       (20)     7754 2024-03-29 12:02:05.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/mockscripts/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)    51083 2024-03-29 12:02:05.000000 pywbemtools-1.2.1/pywbemtools/pywbemcli/pywbemcli.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-03-29 12:04:22.407216 pywbemtools-1.2.1/pywbemtools/pywbemlistener/
--rw-r--r--   0 maiera     (501) staff       (20)     1323 2023-03-20 14:25:46.000000 pywbemtools-1.2.1/pywbemtools/pywbemlistener/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)     1447 2023-03-13 16:54:53.000000 pywbemtools-1.2.1/pywbemtools/pywbemlistener/_cmd_docs.py
--rw-r--r--   0 maiera     (501) staff       (20)     8396 2023-03-20 14:25:46.000000 pywbemtools-1.2.1/pywbemtools/pywbemlistener/_cmd_help.py
--rw-r--r--   0 maiera     (501) staff       (20)    46882 2024-03-29 12:02:05.000000 pywbemtools-1.2.1/pywbemtools/pywbemlistener/_cmd_listener.py
--rw-r--r--   0 maiera     (501) staff       (20)     1409 2022-10-09 14:29:33.000000 pywbemtools-1.2.1/pywbemtools/pywbemlistener/_config.py
--rw-r--r--   0 maiera     (501) staff       (20)     5578 2022-10-09 14:29:33.000000 pywbemtools-1.2.1/pywbemtools/pywbemlistener/_context_obj.py
--rw-r--r--   0 maiera     (501) staff       (20)     5846 2023-03-13 16:55:24.000000 pywbemtools-1.2.1/pywbemtools/pywbemlistener/pywbemlistener.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-03-29 12:04:22.408406 pywbemtools-1.2.1/pywbemtools.egg-info/
--rw-r--r--   0 maiera     (501) staff       (20)    13782 2024-03-29 12:04:22.000000 pywbemtools-1.2.1/pywbemtools.egg-info/PKG-INFO
--rw-r--r--   0 maiera     (501) staff       (20)     1848 2024-03-29 12:04:22.000000 pywbemtools-1.2.1/pywbemtools.egg-info/SOURCES.txt
--rw-r--r--   0 maiera     (501) staff       (20)        1 2024-03-29 12:04:22.000000 pywbemtools-1.2.1/pywbemtools.egg-info/dependency_links.txt
--rw-r--r--   0 maiera     (501) staff       (20)      129 2024-03-29 12:04:22.000000 pywbemtools-1.2.1/pywbemtools.egg-info/entry_points.txt
--rw-r--r--   0 maiera     (501) staff       (20)      996 2024-03-29 12:04:22.000000 pywbemtools-1.2.1/pywbemtools.egg-info/requires.txt
--rw-r--r--   0 maiera     (501) staff       (20)       12 2024-03-29 12:04:22.000000 pywbemtools-1.2.1/pywbemtools.egg-info/top_level.txt
--rw-r--r--   0 maiera     (501) staff       (20)        1 2024-03-29 12:03:40.000000 pywbemtools-1.2.1/pywbemtools.egg-info/zip-safe
--rw-r--r--   0 maiera     (501) staff       (20)     3900 2024-03-29 12:02:05.000000 pywbemtools-1.2.1/requirements.txt
--rw-r--r--   0 maiera     (501) staff       (20)       38 2024-03-29 12:04:22.410005 pywbemtools-1.2.1/setup.cfg
--rw-r--r--   0 maiera     (501) staff       (20)     4984 2024-03-29 12:02:05.000000 pywbemtools-1.2.1/setup.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-20 11:03:34.765302 pywbemtools-1.3.0/
+-rw-r--r--   0 maiera     (501) staff       (20)      205 2021-05-11 05:03:28.000000 pywbemtools-1.3.0/AUTHORS
+-rw-r--r--   0 maiera     (501) staff       (20)    10173 2021-02-20 08:31:47.000000 pywbemtools-1.3.0/LICENSE.txt
+-rw-r--r--   0 maiera     (501) staff       (20)      222 2024-04-20 04:10:39.000000 pywbemtools-1.3.0/MANIFEST.in
+-rw-r--r--   0 maiera     (501) staff       (20)    13254 2024-04-20 11:03:34.764213 pywbemtools-1.3.0/PKG-INFO
+-rw-r--r--   0 maiera     (501) staff       (20)    16544 2024-04-20 04:20:16.000000 pywbemtools-1.3.0/README.md
+-rw-r--r--   0 maiera     (501) staff       (20)     9684 2024-04-20 04:10:39.000000 pywbemtools-1.3.0/README_PYPI.md
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-20 11:03:34.704606 pywbemtools-1.3.0/pywbemtools/
+-rw-r--r--   0 maiera     (501) staff       (20)     1122 2021-02-20 08:31:47.000000 pywbemtools-1.3.0/pywbemtools/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)    12192 2023-03-13 16:54:53.000000 pywbemtools-1.3.0/pywbemtools/_click_extensions.py
+-rw-r--r--   0 maiera     (501) staff       (20)     4917 2023-03-20 14:25:46.000000 pywbemtools-1.3.0/pywbemtools/_common_cmd_actions.py
+-rw-r--r--   0 maiera     (501) staff       (20)     2089 2022-10-09 14:29:33.000000 pywbemtools-1.3.0/pywbemtools/_options.py
+-rw-r--r--   0 maiera     (501) staff       (20)    19417 2022-10-16 19:08:08.000000 pywbemtools-1.3.0/pywbemtools/_output_formatting.py
+-rw-r--r--   0 maiera     (501) staff       (20)     5744 2023-11-05 15:31:40.000000 pywbemtools-1.3.0/pywbemtools/_utils.py
+-rw-r--r--   0 maiera     (501) staff       (20)      973 2024-04-20 11:02:53.000000 pywbemtools-1.3.0/pywbemtools/_version.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-20 11:03:34.749076 pywbemtools-1.3.0/pywbemtools/pywbemcli/
+-rw-r--r--   0 maiera     (501) staff       (20)     2505 2024-04-20 04:10:39.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)    35899 2022-10-16 19:08:08.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_association_shrub.py
+-rw-r--r--   0 maiera     (501) staff       (20)    20125 2022-10-09 14:29:33.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_cimvalueformatter.py
+-rw-r--r--   0 maiera     (501) staff       (20)    36241 2022-10-16 19:08:08.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_class.py
+-rw-r--r--   0 maiera     (501) staff       (20)    36773 2023-03-05 18:05:43.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_connection.py
+-rw-r--r--   0 maiera     (501) staff       (20)     1442 2023-03-13 16:54:53.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_docs.py
+-rw-r--r--   0 maiera     (501) staff       (20)    11053 2023-03-20 14:25:46.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_help.py
+-rw-r--r--   0 maiera     (501) staff       (20)    66534 2023-03-05 18:05:43.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_instance.py
+-rw-r--r--   0 maiera     (501) staff       (20)    13443 2022-10-09 14:29:33.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_namespace.py
+-rw-r--r--   0 maiera     (501) staff       (20)    12074 2022-10-16 19:08:08.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_profile.py
+-rw-r--r--   0 maiera     (501) staff       (20)     7316 2022-10-16 19:08:08.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_qualifier.py
+-rw-r--r--   0 maiera     (501) staff       (20)    21798 2024-03-17 13:09:45.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_server.py
+-rw-r--r--   0 maiera     (501) staff       (20)    22301 2022-10-09 14:29:33.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_statistics.py
+-rw-r--r--   0 maiera     (501) staff       (20)    87470 2022-10-16 19:08:08.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_subscription.py
+-rw-r--r--   0 maiera     (501) staff       (20)    52401 2023-03-05 18:05:39.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_common.py
+-rw-r--r--   0 maiera     (501) staff       (20)    25686 2022-10-16 19:08:08.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_common_cmd_functions.py
+-rw-r--r--   0 maiera     (501) staff       (20)     7447 2022-10-16 19:08:08.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_common_options.py
+-rw-r--r--   0 maiera     (501) staff       (20)    24010 2022-10-09 14:29:33.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_connection_repository.py
+-rw-r--r--   0 maiera     (501) staff       (20)    14883 2023-03-05 18:05:43.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_context_obj.py
+-rw-r--r--   0 maiera     (501) staff       (20)    45120 2022-10-16 19:08:08.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_display_cimobjects.py
+-rw-r--r--   0 maiera     (501) staff       (20)     9456 2022-10-09 14:29:33.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_displaytree.py
+-rw-r--r--   0 maiera     (501) staff       (20)    26615 2022-10-09 14:29:33.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_pywbem_server.py
+-rw-r--r--   0 maiera     (501) staff       (20)    31447 2023-03-13 16:55:24.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_pywbemcli_operations.py
+-rw-r--r--   0 maiera     (501) staff       (20)     1396 2024-04-20 04:10:39.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/_warnings.py
+-rw-r--r--   0 maiera     (501) staff       (20)     4661 2022-10-09 14:29:33.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/config.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-20 11:03:34.750928 pywbemtools-1.3.0/pywbemtools/pywbemcli/mockscripts/
+-rw-r--r--   0 maiera     (501) staff       (20)     7754 2024-04-20 04:10:39.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/mockscripts/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)    50783 2024-04-20 04:10:39.000000 pywbemtools-1.3.0/pywbemtools/pywbemcli/pywbemcli.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-20 11:03:34.760383 pywbemtools-1.3.0/pywbemtools/pywbemlistener/
+-rw-r--r--   0 maiera     (501) staff       (20)     1323 2023-03-20 14:25:46.000000 pywbemtools-1.3.0/pywbemtools/pywbemlistener/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)     1447 2023-03-13 16:54:53.000000 pywbemtools-1.3.0/pywbemtools/pywbemlistener/_cmd_docs.py
+-rw-r--r--   0 maiera     (501) staff       (20)     8396 2023-03-20 14:25:46.000000 pywbemtools-1.3.0/pywbemtools/pywbemlistener/_cmd_help.py
+-rw-r--r--   0 maiera     (501) staff       (20)    48711 2024-04-20 04:10:39.000000 pywbemtools-1.3.0/pywbemtools/pywbemlistener/_cmd_listener.py
+-rw-r--r--   0 maiera     (501) staff       (20)     1409 2022-10-09 14:29:33.000000 pywbemtools-1.3.0/pywbemtools/pywbemlistener/_config.py
+-rw-r--r--   0 maiera     (501) staff       (20)     5578 2022-10-09 14:29:33.000000 pywbemtools-1.3.0/pywbemtools/pywbemlistener/_context_obj.py
+-rw-r--r--   0 maiera     (501) staff       (20)     5846 2023-03-13 16:55:24.000000 pywbemtools-1.3.0/pywbemtools/pywbemlistener/pywbemlistener.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-04-20 11:03:34.762055 pywbemtools-1.3.0/pywbemtools.egg-info/
+-rw-r--r--   0 maiera     (501) staff       (20)    13254 2024-04-20 11:03:34.000000 pywbemtools-1.3.0/pywbemtools.egg-info/PKG-INFO
+-rw-r--r--   0 maiera     (501) staff       (20)     1881 2024-04-20 11:03:34.000000 pywbemtools-1.3.0/pywbemtools.egg-info/SOURCES.txt
+-rw-r--r--   0 maiera     (501) staff       (20)        1 2024-04-20 11:03:34.000000 pywbemtools-1.3.0/pywbemtools.egg-info/dependency_links.txt
+-rw-r--r--   0 maiera     (501) staff       (20)      129 2024-04-20 11:03:34.000000 pywbemtools-1.3.0/pywbemtools.egg-info/entry_points.txt
+-rw-r--r--   0 maiera     (501) staff       (20)     1046 2024-04-20 11:03:34.000000 pywbemtools-1.3.0/pywbemtools.egg-info/requires.txt
+-rw-r--r--   0 maiera     (501) staff       (20)       12 2024-04-20 11:03:34.000000 pywbemtools-1.3.0/pywbemtools.egg-info/top_level.txt
+-rw-r--r--   0 maiera     (501) staff       (20)        1 2024-04-20 04:22:12.000000 pywbemtools-1.3.0/pywbemtools.egg-info/zip-safe
+-rw-r--r--   0 maiera     (501) staff       (20)     4347 2024-04-20 04:10:39.000000 pywbemtools-1.3.0/requirements.txt
+-rw-r--r--   0 maiera     (501) staff       (20)       38 2024-04-20 11:03:34.765714 pywbemtools-1.3.0/setup.cfg
+-rw-r--r--   0 maiera     (501) staff       (20)     5005 2024-04-20 04:10:39.000000 pywbemtools-1.3.0/setup.py
```

### Comparing `pywbemtools-1.2.1/LICENSE.txt` & `pywbemtools-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/PKG-INFO` & `pywbemtools-1.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywbemtools
-Version: 1.2.1
+Version: 1.3.0
 Summary: Python client tools to work with WBEM Servers using the PyWBEM API.
 Home-page: https://github.com/pywbem/pywbemtools
 Author: Karl Schopmeyer, Andreas Maier
 Author-email: k.schopmeyer@swbell.net, maiera@de.ibm.com
 Maintainer: Karl Schopmeyer, Andreas Maier
 Maintainer-email: k.schopmeyer@swbell.net, maiera@de.ibm.com
 License: Apache License, Version 2.0
@@ -18,345 +18,330 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
-Description-Content-Type: text/x-rst
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: AUTHORS
-Requires-Dist: pywbem>=1.6.3
+Requires-Dist: pywbem>=1.7.2
 Requires-Dist: nocaselist>=1.0.3
 Requires-Dist: nocasedict>=1.0.1
 Requires-Dist: six>=1.14.0; python_version <= "3.9"
 Requires-Dist: six>=1.16.0; python_version >= "3.10"
-Requires-Dist: Click<8.0,>=7.1.1; python_version <= "3.5"
+Requires-Dist: Click<8.0,>=7.1.1; python_version == "2.7"
 Requires-Dist: Click>=8.0.2; python_version >= "3.6"
-Requires-Dist: click-spinner>=0.1.8
-Requires-Dist: click-repl<0.3.0,>=0.1.6; python_version <= "3.5"
+Requires-Dist: click-spinner>=0.1.8; python_version <= "3.11"
+Requires-Dist: click-spinner>=0.1.10; python_version >= "3.12"
+Requires-Dist: click-repl<0.3.0,>=0.1.6; python_version == "2.7"
 Requires-Dist: click-repl<0.3.0,>=0.2; python_version >= "3.6"
 Requires-Dist: asciitree>=0.3.3
 Requires-Dist: tabulate>=0.8.2; python_version <= "3.9"
 Requires-Dist: tabulate>=0.8.8; python_version >= "3.10"
 Requires-Dist: toposort<=1.7,>=1.6; python_version <= "3.7"
 Requires-Dist: toposort>=1.6; python_version >= "3.8"
 Requires-Dist: psutil>=5.5.0; python_version <= "3.9"
 Requires-Dist: psutil>=5.8.0; python_version >= "3.10"
 Requires-Dist: prompt-toolkit<3.0.0,>=1.0.15; python_version == "2.7"
-Requires-Dist: prompt-toolkit<3.0.0,>=2.0.1; python_version == "3.5"
 Requires-Dist: prompt-toolkit>=3.0.13; python_version >= "3.6"
 Requires-Dist: PyYAML>=5.3.1; python_version <= "3.5"
 Requires-Dist: PyYAML!=5.4.0,!=5.4.1,>=5.3.1; python_version >= "3.6" and python_version <= "3.11"
 Requires-Dist: PyYAML!=5.4.0,!=5.4.1,!=6.0.0,>=5.3.1; python_version >= "3.12"
 Requires-Dist: yamlloader>=0.5.5
 Requires-Dist: packaging>=17.0; python_version == "2.7"
-Requires-Dist: packaging>=17.0; python_version == "3.5"
-Requires-Dist: packaging>=21.0; python_version >= "3.6"
+Requires-Dist: packaging<22.0,>=21.0; python_version >= "3.6"
 Requires-Dist: mock<4.0.0,>=3.0.0; python_version < "3.6"
 Requires-Dist: mock>=3.0.0; python_version >= "3.6"
 Requires-Dist: funcsigs>=1.0.2; python_version == "2.7"
-Requires-Dist: pyparsing<3.0.0,>=2.3.1; python_version < "3.5"
-Requires-Dist: pyparsing>=2.3.1; python_version >= "3.5"
-
-.. # README file for Pypi
-
-Pywbemtools is a collection of command line tools that communicate with WBEM
-servers. The tools are written in pure Python and support Python 2 and Python
-3.
+Requires-Dist: pyparsing<3.0.0,>=2.3.1; python_version == "2.7"
+Requires-Dist: pyparsing>=2.3.1; python_version >= "3.6"
+Requires-Dist: urllib3<2.0.0,>=1.26.18; python_version == "2.7"
+Requires-Dist: urllib3<2.0.0,>=1.26.18; python_version == "3.6"
+Requires-Dist: urllib3>=1.26.18; python_version >= "3.7"
+
+Pywbemtools is a collection of command line tools that communicate with
+WBEM servers. The tools are written in pure Python and support Python 2
+and Python 3.
 
 At this point, pywbemtools includes a single command line tool named
-``pywbemcli`` that uses the `pywbem package on Pypi`_ to issue operations to a
-WBEM server using the `CIM/WBEM standards`_ defined by the `DMTF`_ to perform
-system management tasks.
-
-CIM/WBEM standards are used for a wide variety of systems management tasks
-in the industry including DMTF management standards and the `SNIA`_
-Storage Management Initiative Specification (`SMI-S`_).
-
-Pywbemcli provides access to WBEM servers from the command line.
-It provides functionality to:
-
-* Explore the CIM data of WBEM servers. It can manage/inspect the CIM model
-  components including CIM classes, CIM instances, and CIM qualifiers and
-  execute CIM methods and queries on the WBEM server.
-
-* Execute specific CIM-XML operations on the WBEM server as defined in `DMTF`_
-  standard `DSP0200 (CIM Operations over HTTP)`_.
-
-* Inspect and manage WBEM server functionality including:
+`pywbemcli` that uses the
+[pywbem package on Pypi](https://pypi.org/project/pywbem/) to issue operations
+to a WBEM server using the
+[CIM/WBEM standards](https://www.dmtf.org/standards/wbem/) defined by the
+[DMTF](https://www.dmtf.org/) to perform system management tasks.
+
+CIM/WBEM standards are used for a wide variety of systems management
+tasks in the industry including DMTF management standards and the
+[SNIA](https://www.snia.org/) Storage Management Initiative Specification
+([SMI-S](https://www.snia.org/forums/smi/tech_programs/smis_home)).
+
+Pywbemcli provides access to WBEM servers from the command line. It
+provides functionality to:
+
+- Explore the CIM data of WBEM servers. It can manage/inspect the CIM
+  model components including CIM classes, CIM instances, and CIM
+  qualifiers and execute CIM methods and queries on the WBEM server.
+- Execute specific CIM-XML operations on the WBEM server as defined in
+  [DMTF](https://www.dmtf.org/) standard
+  [DSP0200 (CIM Operations over HTTP)](https://www.dmtf.org/sites/default/files/standards/documents/DSP0200_1.4.0.pdf).
+- Inspect and manage WBEM server functionality including:
+  - CIM namespaces
+  - Advertised WBEM management profiles
+  - WBEM server brand and version information
+- Capture detailed information on CIM-XML interactions with the WBEM
+  server including time statistics and details of data flow.
+- Maintain a file with persisted WBEM connection definitions so that
+  pywbemcli can access multiple WBEM servers by name.
+- Provide both a command line mode and an interactive mode where
+  multiple pywbemcli commands can be executed within the context of a
+  WBEM server.
+- Use an integrated mock WBEM server to try out commands. The mock
+  server can be loaded with CIM objects defined in MOF files or via
+  Python scripts.
 
-  * CIM namespaces
-  * Advertised WBEM management profiles
-  * WBEM server brand and version information
-
-* Capture detailed information on CIM-XML interactions with the WBEM server
-  including time statistics and details of data flow.
-
-* Maintain a file with persisted WBEM connection definitions so that pywbemcli
-  can access multiple WBEM servers by name.
-
-* Provide both a command line mode and an interactive mode where multiple
-  pywbemcli commands can be executed within the context of a WBEM server.
-
-* Use an integrated mock WBEM server to try out commands. The mock server
-  can be loaded with CIM objects defined in MOF files or via Python scripts.
-
-Documentation
--------------
+# Documentation
 
 For the latest version of pywbemtools released on Pypi:
 
-* `Documentation`_
-* `Installation`_
-* `Change history`_
-
-Quickstart
-----------
-
-All commands within pywbemcli show help with the ``-help`` or ``-h`` options:
-
-.. code-block:: text
-
-    $ pywbemcli --help
-    . . .
-    $ pywbemcli connection --help
-    . . .
-    $ pywbemcli connection save --help
-    . . .
-
-The following examples build on each other and show a typical sequence of
-exploration of a WBEM server. For simplicity, they all operate against the
-default namespace of the server, and use a persistent connection definition for
-the server:
-
-* Add a persistent connection definition named ``conn1`` for the WBEM server to
-  be used, so that the subsequent commands can refer to it:
-
-  .. code-block:: text
-
-      $ pywbemcli -s https://localhost --no-verify -u user -p password connection save conn1
-
-* pywbemcli also supports mocked WBEM servers in memory, that are preloaded
-  with CIM objects defined in MOF files. Add a persistent connection definition
-  named ``assoc1`` to a mock server using one of the MOF files provided in
-  the repo:
-
-  .. code-block:: text
-
-      $ pywbemcli -m tests/unit/simple_assoc_mock_model.mof connection save assoc1
-
-* List the persistent connection definitions:
-
-  .. code-block:: text
-
-      $ pywbemcli connection list
-      WBEM server connections(brief): (#: default, *: current)
-      name    server             mock-server
-      ------  -----------------  --------------------------------------
-      assoc1                     tests/unit/simple_assoc_mock_model.mof
-      conn1   https://localhost
-
-* List the persistent connection definitions with full information:
-
-  .. code-block:: text
-
-      $ pywbemcli connection list --full
-      WBEM server connections(full): (#: default, *: current)
-      name    server             namespace    user      timeout  use_pull    verify    certfile    keyfile    mock-server
-      ------  -----------------  -----------  ------  ---------  ----------  --------  ----------  ---------  --------------------------------------
-      assoc1                     root/cimv2                  30              True                             tests/unit/simple_assoc_mock_model.mof
-      conn1   https://localhost  root/cimv2   user           30  True        False
-
-* Show the class tree, using the previously added connection definition ``assoc1``:
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 class tree
-      root
-       +-- TST_FamilyCollection
-       +-- TST_Lineage
-       +-- TST_MemberOfFamilyCollection
-       +-- TST_Person
-           +-- TST_Personsub
-
-* Retrieve a single class from that class tree:
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 class get TST_Person
-      class TST_Person {
-
-            [Key ( true ),
-             Description ( "This is key prop" )]
-         string name;
-
-         string extraProperty = "defaultvalue";
-
-      };
-
-* Enumerate the instances of that class, returning only their instance names
-  by use of the ``--no`` option:
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 instance enumerate TST_Person --no
-      root/cimv2:TST_Person.name="Gabi"
-      root/cimv2:TST_Person.name="Mike"
-      root/cimv2:TST_Person.name="Saara"
-      root/cimv2:TST_Person.name="Sofi"
-      root/cimv2:TST_PersonSub.name="Gabisub"
-      root/cimv2:TST_PersonSub.name="Mikesub"
-      root/cimv2:TST_PersonSub.name="Saarasub"
-      root/cimv2:TST_PersonSub.name="Sofisub"
-
-* Retrieve a single instance using one of these instance names:
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 instance get 'root/cimv2:TST_Person.name="Sofi"'
-      instance of TST_Person {
-         name = "Sofi";
-      };
-
-* The instance to be retrieved can also be selected interactively by use of
-  the wildcard instance key ("CLASSNAME.?"):
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 instance get TST_Person.?
-      Pick Instance name to process
-      0: root/cimv2:TST_Person.name="Saara"
-      1: root/cimv2:TST_Person.name="Mike"
-      2: root/cimv2:TST_Person.name="Sofi"
-      3: root/cimv2:TST_Person.name="Gabi"
-      4: root/cimv2:TST_PersonSub.name="Gabisub"
-      5: root/cimv2:TST_PersonSub.name="Sofisub"
-      6: root/cimv2:TST_PersonSub.name="Mikesub"
-      7: root/cimv2:TST_PersonSub.name="Saarasub"
-      Input integer between 0 and 7 or Ctrl-C to exit selection: 3
-      instance of TST_Person {
-         name = "Gabi";
-      };
-
-* There are multiple output formats supported. The enumerated instances can for
-  example be formatted as a table of properties by use of the ``-o table``
-  general option (these instances have only one property 'name'):
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 -o table instance enumerate TST_Person
-      Instances: TST_Person
-      +------------+
-      | name       |
-      |------------|
-      | "Gabi"     |
-      | "Mike"     |
-      | "Saara"    |
-      | "Sofi"     |
-      | "Gabisub"  |
-      | "Mikesub"  |
-      | "Saarasub" |
-      | "Sofisub"  |
-      +------------+
-
-* Traverse all associations starting from a specific instance that is selected
-  interactively:
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 -o table instance associators TST_Person.?
-      Pick Instance name to process
-      0: root/cimv2:TST_Person.name="Saara"
-      1: root/cimv2:TST_Person.name="Mike"
-      2: root/cimv2:TST_Person.name="Sofi"
-      3: root/cimv2:TST_Person.name="Gabi"
-      4: root/cimv2:TST_PersonSub.name="Gabisub"
-      5: root/cimv2:TST_PersonSub.name="Sofisub"
-      6: root/cimv2:TST_PersonSub.name="Mikesub"
-      7: root/cimv2:TST_PersonSub.name="Saarasub"
-      Input integer between 0 and 7 or Ctrl-C to exit selection: 1
-      Instances: TST_FamilyCollection
-      +-----------+
-      | name      |
-      |-----------|
-      | "Family2" |
-      | "Gabi"    |
-      | "Sofi"    |
-      +-----------+
-
-Other operations against WBEM servers include getting information on namespaces,
-the Interop namespace, WBEM server brand information, or the advertised
-management profiles:
-
-* Show the Interop namespace of the server:
-
-  .. code-block:: text
-
-      $ pywbemcli -n conn1 server interop
-      Server Interop Namespace:
-      Namespace Name
-      ----------------
-      root/PG_InterOp
-
-* List the advertised management profiles:
-
-  .. code-block:: text
-
-      $ pywbemcli -n conn1 server profiles --organization DMTF
-      Advertised management profiles:
-      +----------------+----------------------+-----------+
-      | Organization   | Registered Name      | Version   |
-      |----------------+----------------------+-----------|
-      | DMTF           | CPU                  | 1.0.0     |
-      | DMTF           | Computer System      | 1.0.0     |
-      | DMTF           | Ethernet Port        | 1.0.0     |
-      | DMTF           | Fan                  | 1.0.0     |
-      | DMTF           | Indications          | 1.1.0     |
-      | DMTF           | Profile Registration | 1.0.0     |
-      +----------------+----------------------+-----------+
-
-Pywbemcli can also be executed in the interactive (REPL) mode by executing it
-without entering a command or by using the command ``repl``. In this mode
-the command line prompt is ``pywbemcli>``, the WBEM server connection is
-maintained between commands and the general options apply to all commands
-executed:
-
-.. code-block:: text
-
-    $ pywbemcli -n conn1
-    Enter 'help' for help, <CTRL-D> or ':q' to exit pywbemcli.
-    pywbemcli> server brand
-
-    Server Brand:
-    WBEM Server Brand
-    -------------------
-    OpenPegasus
-    pywbemcli> server interop
+- [Documentation](https://pywbemtools.readthedocs.io/en/stable/)
+- [Installation](https://pywbemtools.readthedocs.io/en/stable/introduction.html#installation)
+- [Change history](https://pywbemtools.readthedocs.io/en/stable/changes.html)
+
+# Quickstart
+
+All commands within pywbemcli show help with the `-help` or `-h` options:
+
+``` text
+$ pywbemcli --help
+. . .
+$ pywbemcli connection --help
+. . .
+$ pywbemcli connection save --help
+. . .
+```
+
+The following examples build on each other and show a typical sequence
+of exploration of a WBEM server. For simplicity, they all operate
+against the default namespace of the server, and use a persistent
+connection definition for the WBEM server:
+
+-   Add a persistent connection definition named `conn1` for the WBEM
+    server to be used, so that the subsequent commands can refer to it:
+
+    ``` text
+    $ pywbemcli -s https://localhost --no-verify -u user -p password connection save conn1
+    ```
+
+-   pywbemcli also supports mocked WBEM servers in memory, that are
+    preloaded with CIM objects defined in MOF files. Add a persistent
+    connection definition named `assoc1` to a mock server using one of
+    the MOF files provided in the repo:
+
+    ``` text
+    $ pywbemcli -m tests/unit/simple_assoc_mock_model.mof connection save assoc1
+    ```
+
+-   List the persistent WBEM server connection definitions:
+
+    ``` text
+    $ pywbemcli connection list
+    WBEM server connections(brief): (#: default, *: current)
+    name    server             mock-server
+    ------  -----------------  --------------------------------------
+    assoc1                     tests/unit/simple_assoc_mock_model.mof
+    conn1   https://localhost
+    ```
+
+-   List the persistent WBEM server connection definitions with full information:
+
+    ``` text
+    $ pywbemcli connection list --full
+    WBEM server connections(full): (#: default, *: current)
+    name    server             namespace    user      timeout  use_pull    verify    certfile    keyfile    mock-server
+    ------  -----------------  -----------  ------  ---------  ----------  --------  ----------  ---------  --------------------------------------
+    assoc1                     root/cimv2                  30              True                             tests/unit/simple_assoc_mock_model.mof
+    conn1   https://localhost  root/cimv2   user           30  True        False
+    ```
+
+-   Show the class tree, using the previously added WBEM server connection
+    definition `assoc1` (specified with the `-n` option):
+
+    ``` text
+    $ pywbemcli -n assoc1 class tree
+    root
+     +-- TST_FamilyCollection
+     +-- TST_Lineage
+     +-- TST_MemberOfFamilyCollection
+     +-- TST_Person
+         +-- TST_Personsub
+    ```
+
+-   Retrieve a single class from that class tree:
+
+    ``` text
+    $ pywbemcli -n assoc1 class get TST_Person
+    class TST_Person {
+
+          [Key ( true ),
+           Description ( "This is key prop" )]
+       string name;
+
+       string extraProperty = "defaultvalue";
+
+    };
+    ```
+
+-   Enumerate the instances of that class, returning only their instance
+    names by use of the `--no` option:
+
+    ``` text
+    $ pywbemcli -n assoc1 instance enumerate TST_Person --no
+    root/cimv2:TST_Person.name="Gabi"
+    root/cimv2:TST_Person.name="Mike"
+    root/cimv2:TST_Person.name="Saara"
+    root/cimv2:TST_Person.name="Sofi"
+    root/cimv2:TST_PersonSub.name="Gabisub"
+    root/cimv2:TST_PersonSub.name="Mikesub"
+    root/cimv2:TST_PersonSub.name="Saarasub"
+    root/cimv2:TST_PersonSub.name="Sofisub"
+    ```
+
+-   Retrieve a single instance using one of these instance names:
+
+    ``` text
+    $ pywbemcli -n assoc1 instance get 'root/cimv2:TST_Person.name="Sofi"'
+    instance of TST_Person {
+       name = "Sofi";
+    };
+    ```
+
+-   The instance to be retrieved can also be selected interactively by
+    use of the wildcard instance key (\"CLASSNAME.?\"):
+
+    ``` text
+    $ pywbemcli -n assoc1 instance get TST_Person.?
+    Pick Instance name to process
+    0: root/cimv2:TST_Person.name="Saara"
+    1: root/cimv2:TST_Person.name="Mike"
+    2: root/cimv2:TST_Person.name="Sofi"
+    3: root/cimv2:TST_Person.name="Gabi"
+    4: root/cimv2:TST_PersonSub.name="Gabisub"
+    5: root/cimv2:TST_PersonSub.name="Sofisub"
+    6: root/cimv2:TST_PersonSub.name="Mikesub"
+    7: root/cimv2:TST_PersonSub.name="Saarasub"
+    Input integer between 0 and 7 or Ctrl-C to exit selection: 3
+    instance of TST_Person {
+       name = "Gabi";
+    };
+    ```
+
+-   There are multiple output formats supported. The enumerated
+    instances can for example be formatted as a table of properties by
+    use of the `-o table` general option (these instances have only one
+    property \'name\'):
+
+    ``` text
+    $ pywbemcli -n assoc1 -o table instance enumerate TST_Person
+    Instances: TST_Person
+    +------------+
+    | name       |
+    |------------|
+    | "Gabi"     |
+    | "Mike"     |
+    | "Saara"    |
+    | "Sofi"     |
+    | "Gabisub"  |
+    | "Mikesub"  |
+    | "Saarasub" |
+    | "Sofisub"  |
+    +------------+
+    ```
+
+-   Traverse all associations starting from a specific instance that is
+    selected interactively:
+
+    ``` text
+    $ pywbemcli -n assoc1 -o table instance associators TST_Person.?
+    Pick Instance name to process
+    0: root/cimv2:TST_Person.name="Saara"
+    1: root/cimv2:TST_Person.name="Mike"
+    2: root/cimv2:TST_Person.name="Sofi"
+    3: root/cimv2:TST_Person.name="Gabi"
+    4: root/cimv2:TST_PersonSub.name="Gabisub"
+    5: root/cimv2:TST_PersonSub.name="Sofisub"
+    6: root/cimv2:TST_PersonSub.name="Mikesub"
+    7: root/cimv2:TST_PersonSub.name="Saarasub"
+    Input integer between 0 and 7 or Ctrl-C to exit selection: 1
+    Instances: TST_FamilyCollection
+    +-----------+
+    | name      |
+    |-----------|
+    | "Family2" |
+    | "Gabi"    |
+    | "Sofi"    |
+    +-----------+
+    ```
+
+Other operations against WBEM servers include getting information on
+namespaces, the Interop namespace, WBEM server brand information, or the
+advertised management profiles:
+
+-   Show the Interop namespace of the server:
 
+    ``` text
+    $ pywbemcli -n conn1 server interop
     Server Interop Namespace:
     Namespace Name
     ----------------
     root/PG_InterOp
-    pywbemcli> :q
+    ```
 
+-   List the advertised management profiles:
 
-.. _Documentation: https://pywbemtools.readthedocs.io/en/stable/
-.. _Installation: https://pywbemtools.readthedocs.io/en/stable/introduction.html#installation
-.. _Contributing: https://pywbemtools.readthedocs.io/en/stable/development.html#contributing
-.. _Change history: https://pywbemtools.readthedocs.io/en/stable/changes.html
-.. _pywbemtools issue tracker: https://github.com/pywbem/pywbemtools/issues
-.. _pywbem package on Pypi: https://pypi.org/project/pywbem/
-.. _DMTF: https://www.dmtf.org/
-.. _CIM/WBEM standards: https://www.dmtf.org/standards/wbem/
-.. _DSP0200 (CIM Operations over HTTP): https://www.dmtf.org/sites/default/files/standards/documents/DSP0200_1.4.0.pdf
-.. _SNIA: https://www.snia.org/
-.. _SMI-S: https://www.snia.org/forums/smi/tech_programs/smis_home
-.. _Apache 2.0 License: https://github.com/pywbem/pywbemtools/tree/master/LICENSE.txt
+    ``` text
+    $ pywbemcli -n conn1 server profiles --organization DMTF
+    Advertised management profiles:
+    +----------------+----------------------+-----------+
+    | Organization   | Registered Name      | Version   |
+    |----------------+----------------------+-----------|
+    | DMTF           | CPU                  | 1.0.0     |
+    | DMTF           | Computer System      | 1.0.0     |
+    | DMTF           | Ethernet Port        | 1.0.0     |
+    | DMTF           | Fan                  | 1.0.0     |
+    | DMTF           | Indications          | 1.1.0     |
+    | DMTF           | Profile Registration | 1.0.0     |
+    +----------------+----------------------+-----------+
+    ```
+
+Pywbemcli can also be executed in the interactive (REPL) mode by
+executing it without entering a command or by using the command `repl`.
+In this mode the command line prompt is `pywbemcli>`, the WBEM server
+connection is maintained between commands and the general options apply
+to all commands executed:
+
+``` text
+$ pywbemcli -n conn1
+Enter 'help' for help, <CTRL-D> or ':q' to exit pywbemcli.
+pywbemcli> server brand
+
+Server Brand:
+WBEM Server Brand
+-------------------
+OpenPegasus
+pywbemcli> server interop
+
+Server Interop Namespace:
+Namespace Name
+----------------
+root/PG_InterOp
+pywbemcli> :q
+```
```

### Comparing `pywbemtools-1.2.1/README.rst` & `pywbemtools-1.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,480 +1,439 @@
-pywbemtools: Python tools for communicating with WBEM servers
-=============================================================
+# pywbemtools: Python tools for communicating with WBEM servers
 
-.. image:: https://badge.fury.io/py/pywbemtools.svg
-    :target: https://pypi.python.org/pypi/pywbemtools/
-    :alt: PyPI version
-
-.. image:: https://github.com/pywbem/pywbemtools/workflows/test/badge.svg?branch=master
-    :target: https://github.com/pywbem/pywbemtools/actions/
-    :alt: Actions status
-
-.. image:: https://readthedocs.org/projects/pywbemtools/badge/?version=latest
-    :target: https://readthedocs.org/projects/pywbemtools/builds/
-    :alt: ReadTheDocs status
-
-.. image:: https://coveralls.io/repos/github/pywbem/pywbemtools/badge.svg?branch=master
-    :target: https://coveralls.io/github/pywbem/pywbemtools?branch=master
-    :alt: Coveralls result
-
-.. image:: https://img.shields.io/pypi/pyversions/pywbemtools.svg?color=brightgreen
-    :target: https://pypi.python.org/pypi/pywbemtools/
-    :alt: Supported Python
-
-
-Overview
---------
-
-Pywbemtools is a collection of command line tools that communicate with WBEM
-servers. The tools are written in pure Python and support Python 2 and Python
-3.
+[![Version on Pypi](https://img.shields.io/pypi/v/pywbemtools.svg)](https://pypi.python.org/pypi/pywbemtools/)
+[![Test status (master)](https://github.com/pywbem/pywbemtools/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/pywbem/pywbemtools/actions/workflows/test.yml?query=branch%3Amaster)
+[![Docs status (master)](https://readthedocs.org/projects/pywbemtools/badge/?version=latest)](https://readthedocs.org/projects/pywbemtools/builds/)
+[![Test coverage (master)](https://coveralls.io/repos/github/pywbem/pywbemtools/badge.svg?branch=master)](https://coveralls.io/github/pywbem/pywbemtools?branch=master)
+[![Supported Python](https://img.shields.io/pypi/pyversions/pywbemtools.svg?color=brightgreen)](https://pypi.python.org/pypi/pywbemtools/)
+
+# Overview
+
+Pywbemtools is a collection of command line tools that communicate with
+WBEM servers. The tools are written in pure Python and support Python 2
+and Python 3.
 
 Pywbemtools includes the following tools:
 
-* ``pywbemcli`` - A command line utility that uses the `pywbem package on Pypi`_
-  to issue operations to a WBEM server using the `CIM/WBEM standards`_ defined
-  by the `DMTF`_ to perform system management tasks.
-
-* ``pywbemlistener`` - A command line utility that manages WBEM indication
-  listeners running as background processes on the local system. These listeners
-  use the `pywbem package on Pypi`_ to receive indications sent by a WBEM
-  server using the `CIM/WBEM standards`_ defined by the `DMTF`_.
-
-CIM/WBEM standards are used for a wide variety of systems management tasks
-in the industry including DMTF management standards and the `SNIA`_
-Storage Management Initiative Specification (`SMI-S`_).
-
-Pywbemcli provides access to WBEM servers from the command line.
-It provides functionality to:
-
-* Explore the CIM data of WBEM servers. It can manage/inspect the CIM model
-  components including CIM classes, CIM instances, and CIM qualifiers and
-  execute CIM methods and queries on the WBEM server.
-
-* Execute specific CIM-XML operations on the WBEM server as defined in `DMTF`_
-  standard `DSP0200 (CIM Operations over HTTP)`_.
-
-* Inspect and manage WBEM server functionality including:
-
-  * CIM namespaces
-  * Advertised WBEM management profiles
-  * WBEM server brand and version information
-
-* Capture detailed information on CIM-XML interactions with the WBEM server
-  including time statistics and details of data flow.
-
-* Maintain a file with persisted WBEM connection definitions so that pywbemcli
-  can access multiple WBEM servers by name.
-
-* Provide both a command line mode and an interactive mode where multiple
-  pywbemcli commands can be executed within the context of a WBEM server.
-
-* Use an integrated mock WBEM server to try out commands. The mock server
-  can be loaded with CIM objects defined in MOF files or via Python scripts.
-
-Pywbemlistener manages WBEM indication listeners that run on the local system as
-background processes.
-It provides functionality to:
-
-* Start and stop listeners.
-
-* List and show details of listeners.
-
-* Send test indications to listeners.
+- `pywbemcli` - A command line utility that uses the
+  [pywbem package on Pypi](https://pypi.org/project/pywbem/) to issue operations
+  to a WBEM server using the
+  [CIM/WBEM standards](https://www.dmtf.org/standards/wbem/) defined by the
+  [DMTF](https://www.dmtf.org/) to perform system management tasks.
+- `pywbemlistener` - A command line utility that manages WBEM
+  indication listeners running as background processes on the local
+  system. These listeners use the
+  [pywbem package on Pypi](https://pypi.org/project/pywbem/) to receive
+  indications sent by a WBEM server using the
+  [CIM/WBEM standards](https://www.dmtf.org/standards/wbem/) defined by the
+  [DMTF](https://www.dmtf.org/).
+
+CIM/WBEM standards are used for a wide variety of systems management
+tasks in the industry including DMTF management standards and the
+[SNIA](https://www.snia.org/) Storage Management Initiative
+Specification
+([SMI-S](https://www.snia.org/forums/smi/tech_programs/smis_home)).
+
+Pywbemcli provides access to WBEM servers from the command line. It
+provides functionality to:
+
+- Explore the CIM data of WBEM servers. It can manage/inspect the CIM
+  model components including CIM classes, CIM instances, and CIM
+  qualifiers and execute CIM methods and queries on the WBEM server.
+- Execute specific CIM-XML operations on the WBEM server as defined in
+  [DMTF](https://www.dmtf.org/) standard
+  [DSP0200 (CIM Operations over HTTP)](https://www.dmtf.org/sites/default/files/standards/documents/DSP0200_1.4.0.pdf).
+- Inspect and manage WBEM server functionality including:
+  - CIM namespaces
+  - Advertised WBEM management profiles
+  - WBEM server brand and version information
+- Capture detailed information on CIM-XML interactions with the WBEM
+  server including time statistics and details of data flow.
+- Maintain a file with persisted WBEM connection definitions so that
+  pywbemcli can access multiple WBEM servers by name.
+- Provide both a command line mode and an interactive mode where
+  multiple pywbemcli commands can be executed within the context of a
+  WBEM server.
+- Use an integrated mock WBEM server to try out commands. The mock
+  server can be loaded with CIM objects defined in MOF files or via
+  Python scripts.
+
+Pywbemlistener manages WBEM indication listeners that run on the local
+system as background processes. It provides functionality to:
+
+-   Start and stop listeners.
+-   List and show details of listeners.
+-   Send test indications to listeners.
 
-Installation
-------------
+# Installation
 
 Requirements:
 
-1. Python 2.7, 3.4 and higher
-
-2. Operating Systems: Linux, OS-X, native Windows, UNIX-like environments on
-   Windows (e.g. Cygwin)
-
-3. On Python 2, the following OS-level packages are needed:
-
-   * On native Windows:
-
-     - ``choco`` - Chocolatey package manager. The pywbemtools package installation
-       uses Chocolatey to install OS-level software. See https://chocolatey.org/
-       for the installation instructions for Chocolatey.
-
-     - ``wget`` - Download tool. Can be installed with: ``choco install wget``.
-
-   * On Linux, OS-X, UNIX-like environments on Windows (e.g. Cygwin):
-
-     - ``wget`` - Download tool. Can be installed using the OS-level package
-       manager for the platform.
+1.  Python 2.7, 3.6 and higher
+2.  Operating Systems: Linux, OS-X, native Windows, UNIX-like
+    environments on Windows (e.g. Cygwin)
+3.  On Python 2, the following OS-level packages are needed:
+    - On native Windows:
+      - `choco` - Chocolatey package manager. The pywbemtools
+        package installation uses Chocolatey to install OS-level
+        software. See <https://chocolatey.org/> for the installation
+        instructions for Chocolatey.
+      - `wget` - Download tool. Can be installed with:
+        `choco install wget`.
+    - On Linux, OS-X, UNIX-like environments on Windows (e.g. Cygwin):
+      - `wget` - Download tool. Can be installed using the OS-level
+        package manager for the platform.
 
 Installation:
 
-* On Python 2, install OS-level packages needed by the pywbem package:
+- On Python 2, install OS-level packages needed by the pywbem package:
 
   - On native Windows:
 
-    .. code-block:: bash
-
-        > wget -q https://raw.githubusercontent.com/pywbem/pywbem/master/pywbem_os_setup.bat
-        > pywbem_os_setup.bat
+    ``` bash
+    > wget -q https://raw.githubusercontent.com/pywbem/pywbem/master/pywbem_os_setup.bat
+    > pywbem_os_setup.bat
+    ```
 
   - On Linux, OS-X, UNIX-like environments on Windows (e.g. Cygwin):
 
-    .. code-block:: bash
-
-        $ wget -q https://raw.githubusercontent.com/pywbem/pywbem/master/pywbem_os_setup.sh
-        $ chmod 755 pywbem_os_setup.sh
-        $ ./pywbem_os_setup.sh
-
-    The ``pywbem_os_setup.sh`` script uses sudo internally, so your userid
-    needs to have sudo permission.
-
-* Install the pywbemtools Python package:
-
-  .. code-block:: bash
-
-      $ pip install pywbemtools
+    ``` bash
+    $ wget -q https://raw.githubusercontent.com/pywbem/pywbem/master/pywbem_os_setup.sh
+    $ chmod 755 pywbem_os_setup.sh
+    $ ./pywbem_os_setup.sh
+    ```
+
+    The `pywbem_os_setup.sh` script uses sudo internally, so your
+    userid needs to have sudo permission.
+
+- Install the pywbemtools Python package:
+
+  ``` bash
+  $ pip install pywbemtools
+  ```
 
 For more details, including how to install the needed OS-level packages
-manually, see `Installation`_.
-
+manually, see
+[Installation](https://pywbemtools.readthedocs.io/en/stable/introduction.html#installation).
 
-Documentation and change history
---------------------------------
+# Documentation and change history
 
 For the latest version of pywbemtools released on Pypi:
 
-* `Documentation`_
-* `Change history`_
-
-
-Quickstart
-----------
+- [Documentation](https://pywbemtools.readthedocs.io/en/stable/)
+- [Change
+  history](https://pywbemtools.readthedocs.io/en/stable/changes.html)
+
+# Quickstart
+
+All commands within any of the pywbemtools commands show help with the
+`-help` or `-h` options. For example, for the pywbemcli command:
+
+``` text
+$ pywbemcli --help
+. . .
+$ pywbemcli connection --help
+. . .
+$ pywbemcli connection save --help
+. . .
+```
+
+The following examples build on each other and show a typical sequence
+of exploration of a WBEM server. For simplicity, they all operate
+against the default namespace of the server, and use a persistent
+connection definition for the server:
+
+- Add a persistent connection definition named `conn1` for the WBEM
+  server to be used, so that the subsequent commands can refer to it:
+
+  ``` text
+  $ pywbemcli -s https://localhost --no-verify -u user -p password connection save conn1
+  ```
+
+- pywbemcli also supports mocked WBEM servers in memory, that are
+  preloaded with CIM objects defined in MOF files. Add a persistent
+  connection definition named `assoc1` to a mock server using one of
+  the MOF files provided in the repo:
+
+  ``` text
+  $ pywbemcli -m tests/unit/simple_assoc_mock_model.mof connection save assoc1
+  ```
+
+- List the persistent connection definitions:
+
+  ``` text
+  $ pywbemcli connection list
+  WBEM server connections(brief): (#: default, *: current)
+  name    server             mock-server
+  ------  -----------------  --------------------------------------
+  assoc1                     tests/unit/simple_assoc_mock_model.mof
+  conn1   https://localhost
+  ```
+
+- List the persistent connection definitions with full information:
+
+  ``` text
+  $ pywbemcli connection list --full
+  WBEM server connections(full): (#: default, *: current)
+  name    server             namespace    user      timeout  use_pull    verify    certfile    keyfile    mock-server
+  ------  -----------------  -----------  ------  ---------  ----------  --------  ----------  ---------  --------------------------------------
+  assoc1                     root/cimv2                  30              True                             tests/unit/simple_assoc_mock_model.mof
+  conn1   https://localhost  root/cimv2   user           30  True        False
+  ```
+
+- Show the class tree, using the previously added connection
+  definition `assoc1`:
+
+  ``` text
+  $ pywbemcli -n assoc1 class tree
+  root
+   +-- TST_FamilyCollection
+   +-- TST_Lineage
+   +-- TST_MemberOfFamilyCollection
+   +-- TST_Person
+       +-- TST_Personsub
+  ```
+
+- Retrieve a single class from that class tree:
+
+  ``` text
+  $ pywbemcli -n assoc1 class get TST_Person
+  class TST_Person {
+
+        [Key ( true ),
+         Description ( "This is key prop" )]
+     string name;
+
+     string extraProperty = "defaultvalue";
+
+  };
+  ```
+
+- Enumerate the instances of that class, returning only their instance
+  names by use of the `--no` option:
+
+  ``` text
+  $ pywbemcli -n assoc1 instance enumerate TST_Person --no
+  root/cimv2:TST_Person.name="Gabi"
+  root/cimv2:TST_Person.name="Mike"
+  root/cimv2:TST_Person.name="Saara"
+  root/cimv2:TST_Person.name="Sofi"
+  root/cimv2:TST_PersonSub.name="Gabisub"
+  root/cimv2:TST_PersonSub.name="Mikesub"
+  root/cimv2:TST_PersonSub.name="Saarasub"
+  root/cimv2:TST_PersonSub.name="Sofisub"
+  ```
+
+- Retrieve a single instance using one of these instance names:
+
+  ``` text
+  $ pywbemcli -n assoc1 instance get 'root/cimv2:TST_Person.name="Sofi"'
+  instance of TST_Person {
+     name = "Sofi";
+  };
+  ```
+
+- The instance to be retrieved can also be selected interactively by
+  use of the wildcard instance key (\"CLASSNAME.?\"):
+
+  ``` text
+  $ pywbemcli -n assoc1 instance get TST_Person.?
+  Pick Instance name to process
+  0: root/cimv2:TST_Person.name="Saara"
+  1: root/cimv2:TST_Person.name="Mike"
+  2: root/cimv2:TST_Person.name="Sofi"
+  3: root/cimv2:TST_Person.name="Gabi"
+  4: root/cimv2:TST_PersonSub.name="Gabisub"
+  5: root/cimv2:TST_PersonSub.name="Sofisub"
+  6: root/cimv2:TST_PersonSub.name="Mikesub"
+  7: root/cimv2:TST_PersonSub.name="Saarasub"
+  Input integer between 0 and 7 or Ctrl-C to exit selection: 3
+  instance of TST_Person {
+     name = "Gabi";
+  };
+  ```
+
+- There are multiple output formats supported. The enumerated
+  instances can for example be formatted as a table of properties by
+  use of the `-o table` general option (these instances have only one
+  property \'name\'):
+
+  ``` text
+  $ pywbemcli -n assoc1 -o table instance enumerate TST_Person
+  Instances: TST_Person
+  +------------+
+  | name       |
+  |------------|
+  | "Gabi"     |
+  | "Mike"     |
+  | "Saara"    |
+  | "Sofi"     |
+  | "Gabisub"  |
+  | "Mikesub"  |
+  | "Saarasub" |
+  | "Sofisub"  |
+  +------------+
+  ```
+
+- Traverse all associations starting from a specific instance that is
+  selected interactively:
+
+  ``` text
+  $ pywbemcli -n assoc1 -o table instance associators TST_Person.?
+  Pick Instance name to process
+  0: root/cimv2:TST_Person.name="Saara"
+  1: root/cimv2:TST_Person.name="Mike"
+  2: root/cimv2:TST_Person.name="Sofi"
+  3: root/cimv2:TST_Person.name="Gabi"
+  4: root/cimv2:TST_PersonSub.name="Gabisub"
+  5: root/cimv2:TST_PersonSub.name="Sofisub"
+  6: root/cimv2:TST_PersonSub.name="Mikesub"
+  7: root/cimv2:TST_PersonSub.name="Saarasub"
+  Input integer between 0 and 7 or Ctrl-C to exit selection: 1
+  Instances: TST_FamilyCollection
+  +-----------+
+  | name      |
+  |-----------|
+  | "Family2" |
+  | "Gabi"    |
+  | "Sofi"    |
+  +-----------+
+  ```
+
+Other operations against WBEM servers include getting information on
+namespaces, the Interop namespace, WBEM server brand information, or the
+advertised management profiles:
+
+- Show the Interop namespace of the server:
+
+  ``` text
+  $ pywbemcli -n conn1 server interop
+  Server Interop Namespace:
+  Namespace Name
+  ----------------
+  root/PG_InterOp
+  ```
+
+- List the advertised management profiles:
+
+  ``` text
+  $ pywbemcli -n conn1 server profiles --organization DMTF
+  Advertised management profiles:
+  +----------------+----------------------+-----------+
+  | Organization   | Registered Name      | Version   |
+  |----------------+----------------------+-----------|
+  | DMTF           | CPU                  | 1.0.0     |
+  | DMTF           | Computer System      | 1.0.0     |
+  | DMTF           | Ethernet Port        | 1.0.0     |
+  | DMTF           | Fan                  | 1.0.0     |
+  | DMTF           | Indications          | 1.1.0     |
+  | DMTF           | Profile Registration | 1.0.0     |
+  +----------------+----------------------+-----------+
+  ```
+
+Pywbemcli can also be executed in the interactive (REPL) mode by
+executing it without entering a command or by using the command `repl`.
+In this mode the command line prompt is `pywbemcli>`, the WBEM server
+connection is maintained between commands and the general options apply
+to all commands executed:
+
+``` text
+$ pywbemcli -n conn1
+Enter 'help' for help, <CTRL-D> or ':q' to exit pywbemcli.
+pywbemcli> server brand
+
+Server Brand:
+WBEM Server Brand
+-------------------
+OpenPegasus
+pywbemcli> server interop
 
-All commands within any of the pywbemtools commands show help with the ``-help``
-or ``-h`` options. For example, for the pywbemcli command:
-
-.. code-block:: text
-
-    $ pywbemcli --help
-    . . .
-    $ pywbemcli connection --help
-    . . .
-    $ pywbemcli connection save --help
-    . . .
-
-The following examples build on each other and show a typical sequence of
-exploration of a WBEM server. For simplicity, they all operate against the
-default namespace of the server, and use a persistent connection definition for
-the server:
-
-* Add a persistent connection definition named ``conn1`` for the WBEM server to
-  be used, so that the subsequent commands can refer to it:
-
-  .. code-block:: text
-
-      $ pywbemcli -s https://localhost --no-verify -u user -p password connection save conn1
-
-* pywbemcli also supports mocked WBEM servers in memory, that are preloaded
-  with CIM objects defined in MOF files. Add a persistent connection definition
-  named ``assoc1`` to a mock server using one of the MOF files provided in
-  the repo:
-
-  .. code-block:: text
-
-      $ pywbemcli -m tests/unit/simple_assoc_mock_model.mof connection save assoc1
-
-* List the persistent connection definitions:
-
-  .. code-block:: text
-
-      $ pywbemcli connection list
-      WBEM server connections(brief): (#: default, *: current)
-      name    server             mock-server
-      ------  -----------------  --------------------------------------
-      assoc1                     tests/unit/simple_assoc_mock_model.mof
-      conn1   https://localhost
-
-* List the persistent connection definitions with full information:
-
-  .. code-block:: text
-
-      $ pywbemcli connection list --full
-      WBEM server connections(full): (#: default, *: current)
-      name    server             namespace    user      timeout  use_pull    verify    certfile    keyfile    mock-server
-      ------  -----------------  -----------  ------  ---------  ----------  --------  ----------  ---------  --------------------------------------
-      assoc1                     root/cimv2                  30              True                             tests/unit/simple_assoc_mock_model.mof
-      conn1   https://localhost  root/cimv2   user           30  True        False
-
-* Show the class tree, using the previously added connection definition ``assoc1``:
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 class tree
-      root
-       +-- TST_FamilyCollection
-       +-- TST_Lineage
-       +-- TST_MemberOfFamilyCollection
-       +-- TST_Person
-           +-- TST_Personsub
-
-* Retrieve a single class from that class tree:
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 class get TST_Person
-      class TST_Person {
-
-            [Key ( true ),
-             Description ( "This is key prop" )]
-         string name;
-
-         string extraProperty = "defaultvalue";
-
-      };
-
-* Enumerate the instances of that class, returning only their instance names
-  by use of the ``--no`` option:
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 instance enumerate TST_Person --no
-      root/cimv2:TST_Person.name="Gabi"
-      root/cimv2:TST_Person.name="Mike"
-      root/cimv2:TST_Person.name="Saara"
-      root/cimv2:TST_Person.name="Sofi"
-      root/cimv2:TST_PersonSub.name="Gabisub"
-      root/cimv2:TST_PersonSub.name="Mikesub"
-      root/cimv2:TST_PersonSub.name="Saarasub"
-      root/cimv2:TST_PersonSub.name="Sofisub"
-
-* Retrieve a single instance using one of these instance names:
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 instance get 'root/cimv2:TST_Person.name="Sofi"'
-      instance of TST_Person {
-         name = "Sofi";
-      };
-
-* The instance to be retrieved can also be selected interactively by use of
-  the wildcard instance key ("CLASSNAME.?"):
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 instance get TST_Person.?
-      Pick Instance name to process
-      0: root/cimv2:TST_Person.name="Saara"
-      1: root/cimv2:TST_Person.name="Mike"
-      2: root/cimv2:TST_Person.name="Sofi"
-      3: root/cimv2:TST_Person.name="Gabi"
-      4: root/cimv2:TST_PersonSub.name="Gabisub"
-      5: root/cimv2:TST_PersonSub.name="Sofisub"
-      6: root/cimv2:TST_PersonSub.name="Mikesub"
-      7: root/cimv2:TST_PersonSub.name="Saarasub"
-      Input integer between 0 and 7 or Ctrl-C to exit selection: 3
-      instance of TST_Person {
-         name = "Gabi";
-      };
-
-* There are multiple output formats supported. The enumerated instances can for
-  example be formatted as a table of properties by use of the ``-o table``
-  general option (these instances have only one property 'name'):
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 -o table instance enumerate TST_Person
-      Instances: TST_Person
-      +------------+
-      | name       |
-      |------------|
-      | "Gabi"     |
-      | "Mike"     |
-      | "Saara"    |
-      | "Sofi"     |
-      | "Gabisub"  |
-      | "Mikesub"  |
-      | "Saarasub" |
-      | "Sofisub"  |
-      +------------+
-
-* Traverse all associations starting from a specific instance that is selected
-  interactively:
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 -o table instance associators TST_Person.?
-      Pick Instance name to process
-      0: root/cimv2:TST_Person.name="Saara"
-      1: root/cimv2:TST_Person.name="Mike"
-      2: root/cimv2:TST_Person.name="Sofi"
-      3: root/cimv2:TST_Person.name="Gabi"
-      4: root/cimv2:TST_PersonSub.name="Gabisub"
-      5: root/cimv2:TST_PersonSub.name="Sofisub"
-      6: root/cimv2:TST_PersonSub.name="Mikesub"
-      7: root/cimv2:TST_PersonSub.name="Saarasub"
-      Input integer between 0 and 7 or Ctrl-C to exit selection: 1
-      Instances: TST_FamilyCollection
-      +-----------+
-      | name      |
-      |-----------|
-      | "Family2" |
-      | "Gabi"    |
-      | "Sofi"    |
-      +-----------+
-
-Other operations against WBEM servers include getting information on namespaces,
-the Interop namespace, WBEM server brand information, or the advertised
-management profiles:
-
-* Show the Interop namespace of the server:
-
-  .. code-block:: text
-
-      $ pywbemcli -n conn1 server interop
-      Server Interop Namespace:
-      Namespace Name
-      ----------------
-      root/PG_InterOp
-
-* List the advertised management profiles:
-
-  .. code-block:: text
-
-      $ pywbemcli -n conn1 server profiles --organization DMTF
-      Advertised management profiles:
-      +----------------+----------------------+-----------+
-      | Organization   | Registered Name      | Version   |
-      |----------------+----------------------+-----------|
-      | DMTF           | CPU                  | 1.0.0     |
-      | DMTF           | Computer System      | 1.0.0     |
-      | DMTF           | Ethernet Port        | 1.0.0     |
-      | DMTF           | Fan                  | 1.0.0     |
-      | DMTF           | Indications          | 1.1.0     |
-      | DMTF           | Profile Registration | 1.0.0     |
-      +----------------+----------------------+-----------+
-
-Pywbemcli can also be executed in the interactive (REPL) mode by executing it
-without entering a command or by using the command ``repl``. In this mode
-the command line prompt is ``pywbemcli>``, the WBEM server connection is
-maintained between commands and the general options apply to all commands
-executed:
-
-.. code-block:: text
-
-    $ pywbemcli -n conn1
-    Enter 'help' for help, <CTRL-D> or ':q' to exit pywbemcli.
-    pywbemcli> server brand
-
-    Server Brand:
-    WBEM Server Brand
-    -------------------
-    OpenPegasus
-    pywbemcli> server interop
-
-    Server Interop Namespace:
-    Namespace Name
-    ----------------
-    root/PG_InterOp
-    pywbemcli> :q
-
-
-The pywbemlistener command allows setting up WBEM indication listeners on the
-local system. The following example starts a listener for HTTP on port 25000 and
-uses pywbemcli to set that server up for sending indications to the listener:
-
-.. code-block:: text
-
-    # Start OpenPegasus as a Docker container
-    $ docker create keyporttech/smi-server:0.1.2 --name pegasus
-    $ docker start pegasus
-
-    # Define a pywbemcli named connection for that OpenPegasus
-    $ pywbemcli -s https://localhost:5989 --no-verify connection save pegasus
-
-    # Start a pywbem listener that appends any received indications to a file
-    $ pywbemlistener start lis1 -s http -p 25000 --indi-file lis1.out
-    $ pywbemlistener list
-    +--------+--------+----------+-------+---------------------+
-    | Name   |   Port | Scheme   |   PID | Created             |
-    |--------+--------+----------+-------+---------------------|
-    | lis1   |  25000 | http     |  6662 | 2022-01-02 13:28:04 |
-    +--------+--------+----------+-------+---------------------+
-
-    # Add our pywbem listener as a listener destination to the OpenPegasus server
-    $ pywbemcli -n pegasus subscription add-destination lis1 -l http://localhost:25000
-    Added owned destination: Name=pywbemdestination:defaultpywbemcliSubMgr:lis1
-
-    $ pywbemcli -n pegasus subscription list-destinations
-    Indication Destinations: submgr-id=defaultpywbemcliSubMgr, svr-id=https://localhost:5989, type=all
-    +-------------+------------+--------------------------------+------------------------+---------------+------------+----------------+
-    | Ownership   | Identity   | Name                           | Destination            |   Persistence |   Protocol |   Subscription |
-    |             |            | Property                       |                        |          Type |            |          Count |
-    |-------------+------------+--------------------------------+------------------------+---------------+------------+----------------|
-    | owned       | lis1       | pywbemdestination:defaultpywbe | http://localhost:25000 |             3 |          2 |              0 |
-    |             |            | mcliSubMgr:lis1                |                        |               |            |                |
-    +-------------+------------+--------------------------------+------------------------+---------------+------------+----------------+
-
-    # Use pywbemlistener to send a test indication
-    # Note: This does not utilize the OpenPegasus server but sends it directly to the listener
-    $ pywbemlistener test lis1
-    Sending the following test indication:
-    instance of CIM_AlertIndication {
-       IndicationIdentifier = NULL;
-       AlertingElementFormat = 2;
-       AlertingManagedElement = NULL;
-       AlertType = 2;
-       Message = "Test message";
-       OwningEntity = "TEST";
-       PerceivedSeverity = 2;
-       ProbableCause = 0;
-       SystemName = NULL;
-       MessageArguments = { };
-       IndicationTime = "20220102134842.761734+000";
-       MessageID = "TESTnnnn";
-    };
-
-    Sent test indication #1 to listener lis1 at http://localhost:25000
-
-    $ cat lis1.out
-    2022-01-02 13:48:43.010994+01:00 127.0.0.1 instance of CIM_AlertIndication {    IndicationIdentifier = NULL;    AlertingElementFormat = 2;
-      AlertingManagedElement = NULL;    AlertType = 2;    Message = "Test message";    OwningEntity = "TEST";    PerceivedSeverity = 2;
-      ProbableCause = 0;    SystemName = NULL;    MessageArguments = { };    IndicationTime = "20220102134842.761734+000";
-      MessageID = "TEST0001"; };
-
-
-Project Planning
+Server Interop Namespace:
+Namespace Name
 ----------------
-
-For each upcoming release, the bugs and feature requests that are planned to
-be addressed in that release are listed in the `pywbemtools issue tracker`_
-with an according milestone set that identifies the target release.
-The due date on the milestone definition is the planned release date.
-There is usually also an issue that sets out the major goals for an upcoming
+root/PG_InterOp
+pywbemcli> :q
+```
+
+The pywbemlistener command allows setting up WBEM indication listeners
+on the local system. The following example starts a listener for HTTP on
+port 25000 and uses pywbemcli to set that server up for sending
+indications to the listener:
+
+``` text
+# Start OpenPegasus as a Docker container
+$ docker create keyporttech/smi-server:0.1.2 --name pegasus
+$ docker start pegasus
+
+# Define a pywbemcli named connection for that OpenPegasus
+$ pywbemcli -s https://localhost:5989 --no-verify connection save pegasus
+
+# Start a pywbem listener that appends any received indications to a file
+$ pywbemlistener start lis1 -s http -p 25000 --indi-file lis1.out
+$ pywbemlistener list
++--------+--------+----------+-------+---------------------+
+| Name   |   Port | Scheme   |   PID | Created             |
+|--------+--------+----------+-------+---------------------|
+| lis1   |  25000 | http     |  6662 | 2022-01-02 13:28:04 |
++--------+--------+----------+-------+---------------------+
+
+# Add our pywbem listener as a listener destination to the OpenPegasus server
+$ pywbemcli -n pegasus subscription add-destination lis1 -l http://localhost:25000
+Added owned destination: Name=pywbemdestination:defaultpywbemcliSubMgr:lis1
+
+$ pywbemcli -n pegasus subscription list-destinations
+Indication Destinations: submgr-id=defaultpywbemcliSubMgr, svr-id=https://localhost:5989, type=all
++-------------+------------+--------------------------------+------------------------+---------------+------------+----------------+
+| Ownership   | Identity   | Name                           | Destination            |   Persistence |   Protocol |   Subscription |
+|             |            | Property                       |                        |          Type |            |          Count |
+|-------------+------------+--------------------------------+------------------------+---------------+------------+----------------|
+| owned       | lis1       | pywbemdestination:defaultpywbe | http://localhost:25000 |             3 |          2 |              0 |
+|             |            | mcliSubMgr:lis1                |                        |               |            |                |
++-------------+------------+--------------------------------+------------------------+---------------+------------+----------------+
+
+# Use pywbemlistener to send a test indication
+# Note: This does not utilize the OpenPegasus server but sends it directly to the listener
+$ pywbemlistener test lis1
+Sending the following test indication:
+instance of CIM_AlertIndication {
+   IndicationIdentifier = NULL;
+   AlertingElementFormat = 2;
+   AlertingManagedElement = NULL;
+   AlertType = 2;
+   Message = "Test message";
+   OwningEntity = "TEST";
+   PerceivedSeverity = 2;
+   ProbableCause = 0;
+   SystemName = NULL;
+   MessageArguments = { };
+   IndicationTime = "20220102134842.761734+000";
+   MessageID = "TESTnnnn";
+};
+
+Sent test indication #1 to listener lis1 at http://localhost:25000
+
+$ cat lis1.out
+2022-01-02 13:48:43.010994+01:00 127.0.0.1 instance of CIM_AlertIndication {    IndicationIdentifier = NULL;    AlertingElementFormat = 2;
+  AlertingManagedElement = NULL;    AlertType = 2;    Message = "Test message";    OwningEntity = "TEST";    PerceivedSeverity = 2;
+  ProbableCause = 0;    SystemName = NULL;    MessageArguments = { };    IndicationTime = "20220102134842.761734+000";
+  MessageID = "TEST0001"; };
+```
+
+# Project Planning
+
+For each upcoming release, the bugs and feature requests that are
+planned to be addressed in that release are listed in the
+[pywbemtools issue tracker](https://github.com/pywbem/pywbemtools/issues) with
+an according milestone set that identifies the target release. The due date
+on the milestone definition is the planned release date. There is
+usually also an issue that sets out the major goals for an upcoming
 release.
 
+# Contributing
 
-Contributing
-------------
-
-For information on how to contribute to this project, see `Contributing`_.
-
+For information on how to contribute to this project, see
+[Contributing](https://pywbemtools.readthedocs.io/en/stable/development.html#contributing).
 
-License
--------
+# License
 
-The pywbemtools package is licensed under the `Apache 2.0 License`_.
-
-
-.. _Documentation: https://pywbemtools.readthedocs.io/en/stable/
-.. _Installation: https://pywbemtools.readthedocs.io/en/stable/introduction.html#installation
-.. _Contributing: https://pywbemtools.readthedocs.io/en/stable/development.html#contributing
-.. _Change history: https://pywbemtools.readthedocs.io/en/stable/changes.html
-.. _pywbemtools issue tracker: https://github.com/pywbem/pywbemtools/issues
-.. _pywbem package on Pypi: https://pypi.org/project/pywbem/
-.. _DMTF: https://www.dmtf.org/
-.. _CIM/WBEM standards: https://www.dmtf.org/standards/wbem/
-.. _DSP0200 (CIM Operations over HTTP): https://www.dmtf.org/sites/default/files/standards/documents/DSP0200_1.4.0.pdf
-.. _SNIA: https://www.snia.org/
-.. _SMI-S: https://www.snia.org/forums/smi/tech_programs/smis_home
-.. _Apache 2.0 License: https://github.com/pywbem/pywbemtools/tree/master/LICENSE.txt
+The pywbemtools package is licensed under the [Apache 2.0
+License](https://github.com/pywbem/pywbemtools/tree/master/LICENSE.txt).
```

### Comparing `pywbemtools-1.2.1/README_PYPI.rst` & `pywbemtools-1.3.0/README_PYPI.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,294 +1,277 @@
-.. # README file for Pypi
-
-Pywbemtools is a collection of command line tools that communicate with WBEM
-servers. The tools are written in pure Python and support Python 2 and Python
-3.
+Pywbemtools is a collection of command line tools that communicate with
+WBEM servers. The tools are written in pure Python and support Python 2
+and Python 3.
 
 At this point, pywbemtools includes a single command line tool named
-``pywbemcli`` that uses the `pywbem package on Pypi`_ to issue operations to a
-WBEM server using the `CIM/WBEM standards`_ defined by the `DMTF`_ to perform
-system management tasks.
-
-CIM/WBEM standards are used for a wide variety of systems management tasks
-in the industry including DMTF management standards and the `SNIA`_
-Storage Management Initiative Specification (`SMI-S`_).
-
-Pywbemcli provides access to WBEM servers from the command line.
-It provides functionality to:
-
-* Explore the CIM data of WBEM servers. It can manage/inspect the CIM model
-  components including CIM classes, CIM instances, and CIM qualifiers and
-  execute CIM methods and queries on the WBEM server.
-
-* Execute specific CIM-XML operations on the WBEM server as defined in `DMTF`_
-  standard `DSP0200 (CIM Operations over HTTP)`_.
-
-* Inspect and manage WBEM server functionality including:
+`pywbemcli` that uses the
+[pywbem package on Pypi](https://pypi.org/project/pywbem/) to issue operations
+to a WBEM server using the
+[CIM/WBEM standards](https://www.dmtf.org/standards/wbem/) defined by the
+[DMTF](https://www.dmtf.org/) to perform system management tasks.
+
+CIM/WBEM standards are used for a wide variety of systems management
+tasks in the industry including DMTF management standards and the
+[SNIA](https://www.snia.org/) Storage Management Initiative Specification
+([SMI-S](https://www.snia.org/forums/smi/tech_programs/smis_home)).
+
+Pywbemcli provides access to WBEM servers from the command line. It
+provides functionality to:
+
+- Explore the CIM data of WBEM servers. It can manage/inspect the CIM
+  model components including CIM classes, CIM instances, and CIM
+  qualifiers and execute CIM methods and queries on the WBEM server.
+- Execute specific CIM-XML operations on the WBEM server as defined in
+  [DMTF](https://www.dmtf.org/) standard
+  [DSP0200 (CIM Operations over HTTP)](https://www.dmtf.org/sites/default/files/standards/documents/DSP0200_1.4.0.pdf).
+- Inspect and manage WBEM server functionality including:
+  - CIM namespaces
+  - Advertised WBEM management profiles
+  - WBEM server brand and version information
+- Capture detailed information on CIM-XML interactions with the WBEM
+  server including time statistics and details of data flow.
+- Maintain a file with persisted WBEM connection definitions so that
+  pywbemcli can access multiple WBEM servers by name.
+- Provide both a command line mode and an interactive mode where
+  multiple pywbemcli commands can be executed within the context of a
+  WBEM server.
+- Use an integrated mock WBEM server to try out commands. The mock
+  server can be loaded with CIM objects defined in MOF files or via
+  Python scripts.
 
-  * CIM namespaces
-  * Advertised WBEM management profiles
-  * WBEM server brand and version information
-
-* Capture detailed information on CIM-XML interactions with the WBEM server
-  including time statistics and details of data flow.
-
-* Maintain a file with persisted WBEM connection definitions so that pywbemcli
-  can access multiple WBEM servers by name.
-
-* Provide both a command line mode and an interactive mode where multiple
-  pywbemcli commands can be executed within the context of a WBEM server.
-
-* Use an integrated mock WBEM server to try out commands. The mock server
-  can be loaded with CIM objects defined in MOF files or via Python scripts.
-
-Documentation
--------------
+# Documentation
 
 For the latest version of pywbemtools released on Pypi:
 
-* `Documentation`_
-* `Installation`_
-* `Change history`_
-
-Quickstart
-----------
-
-All commands within pywbemcli show help with the ``-help`` or ``-h`` options:
-
-.. code-block:: text
-
-    $ pywbemcli --help
-    . . .
-    $ pywbemcli connection --help
-    . . .
-    $ pywbemcli connection save --help
-    . . .
-
-The following examples build on each other and show a typical sequence of
-exploration of a WBEM server. For simplicity, they all operate against the
-default namespace of the server, and use a persistent connection definition for
-the server:
-
-* Add a persistent connection definition named ``conn1`` for the WBEM server to
-  be used, so that the subsequent commands can refer to it:
-
-  .. code-block:: text
-
-      $ pywbemcli -s https://localhost --no-verify -u user -p password connection save conn1
-
-* pywbemcli also supports mocked WBEM servers in memory, that are preloaded
-  with CIM objects defined in MOF files. Add a persistent connection definition
-  named ``assoc1`` to a mock server using one of the MOF files provided in
-  the repo:
-
-  .. code-block:: text
-
-      $ pywbemcli -m tests/unit/simple_assoc_mock_model.mof connection save assoc1
-
-* List the persistent connection definitions:
-
-  .. code-block:: text
-
-      $ pywbemcli connection list
-      WBEM server connections(brief): (#: default, *: current)
-      name    server             mock-server
-      ------  -----------------  --------------------------------------
-      assoc1                     tests/unit/simple_assoc_mock_model.mof
-      conn1   https://localhost
-
-* List the persistent connection definitions with full information:
-
-  .. code-block:: text
-
-      $ pywbemcli connection list --full
-      WBEM server connections(full): (#: default, *: current)
-      name    server             namespace    user      timeout  use_pull    verify    certfile    keyfile    mock-server
-      ------  -----------------  -----------  ------  ---------  ----------  --------  ----------  ---------  --------------------------------------
-      assoc1                     root/cimv2                  30              True                             tests/unit/simple_assoc_mock_model.mof
-      conn1   https://localhost  root/cimv2   user           30  True        False
-
-* Show the class tree, using the previously added connection definition ``assoc1``:
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 class tree
-      root
-       +-- TST_FamilyCollection
-       +-- TST_Lineage
-       +-- TST_MemberOfFamilyCollection
-       +-- TST_Person
-           +-- TST_Personsub
-
-* Retrieve a single class from that class tree:
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 class get TST_Person
-      class TST_Person {
-
-            [Key ( true ),
-             Description ( "This is key prop" )]
-         string name;
-
-         string extraProperty = "defaultvalue";
-
-      };
-
-* Enumerate the instances of that class, returning only their instance names
-  by use of the ``--no`` option:
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 instance enumerate TST_Person --no
-      root/cimv2:TST_Person.name="Gabi"
-      root/cimv2:TST_Person.name="Mike"
-      root/cimv2:TST_Person.name="Saara"
-      root/cimv2:TST_Person.name="Sofi"
-      root/cimv2:TST_PersonSub.name="Gabisub"
-      root/cimv2:TST_PersonSub.name="Mikesub"
-      root/cimv2:TST_PersonSub.name="Saarasub"
-      root/cimv2:TST_PersonSub.name="Sofisub"
-
-* Retrieve a single instance using one of these instance names:
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 instance get 'root/cimv2:TST_Person.name="Sofi"'
-      instance of TST_Person {
-         name = "Sofi";
-      };
-
-* The instance to be retrieved can also be selected interactively by use of
-  the wildcard instance key ("CLASSNAME.?"):
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 instance get TST_Person.?
-      Pick Instance name to process
-      0: root/cimv2:TST_Person.name="Saara"
-      1: root/cimv2:TST_Person.name="Mike"
-      2: root/cimv2:TST_Person.name="Sofi"
-      3: root/cimv2:TST_Person.name="Gabi"
-      4: root/cimv2:TST_PersonSub.name="Gabisub"
-      5: root/cimv2:TST_PersonSub.name="Sofisub"
-      6: root/cimv2:TST_PersonSub.name="Mikesub"
-      7: root/cimv2:TST_PersonSub.name="Saarasub"
-      Input integer between 0 and 7 or Ctrl-C to exit selection: 3
-      instance of TST_Person {
-         name = "Gabi";
-      };
-
-* There are multiple output formats supported. The enumerated instances can for
-  example be formatted as a table of properties by use of the ``-o table``
-  general option (these instances have only one property 'name'):
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 -o table instance enumerate TST_Person
-      Instances: TST_Person
-      +------------+
-      | name       |
-      |------------|
-      | "Gabi"     |
-      | "Mike"     |
-      | "Saara"    |
-      | "Sofi"     |
-      | "Gabisub"  |
-      | "Mikesub"  |
-      | "Saarasub" |
-      | "Sofisub"  |
-      +------------+
-
-* Traverse all associations starting from a specific instance that is selected
-  interactively:
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 -o table instance associators TST_Person.?
-      Pick Instance name to process
-      0: root/cimv2:TST_Person.name="Saara"
-      1: root/cimv2:TST_Person.name="Mike"
-      2: root/cimv2:TST_Person.name="Sofi"
-      3: root/cimv2:TST_Person.name="Gabi"
-      4: root/cimv2:TST_PersonSub.name="Gabisub"
-      5: root/cimv2:TST_PersonSub.name="Sofisub"
-      6: root/cimv2:TST_PersonSub.name="Mikesub"
-      7: root/cimv2:TST_PersonSub.name="Saarasub"
-      Input integer between 0 and 7 or Ctrl-C to exit selection: 1
-      Instances: TST_FamilyCollection
-      +-----------+
-      | name      |
-      |-----------|
-      | "Family2" |
-      | "Gabi"    |
-      | "Sofi"    |
-      +-----------+
-
-Other operations against WBEM servers include getting information on namespaces,
-the Interop namespace, WBEM server brand information, or the advertised
-management profiles:
-
-* Show the Interop namespace of the server:
-
-  .. code-block:: text
-
-      $ pywbemcli -n conn1 server interop
-      Server Interop Namespace:
-      Namespace Name
-      ----------------
-      root/PG_InterOp
-
-* List the advertised management profiles:
-
-  .. code-block:: text
-
-      $ pywbemcli -n conn1 server profiles --organization DMTF
-      Advertised management profiles:
-      +----------------+----------------------+-----------+
-      | Organization   | Registered Name      | Version   |
-      |----------------+----------------------+-----------|
-      | DMTF           | CPU                  | 1.0.0     |
-      | DMTF           | Computer System      | 1.0.0     |
-      | DMTF           | Ethernet Port        | 1.0.0     |
-      | DMTF           | Fan                  | 1.0.0     |
-      | DMTF           | Indications          | 1.1.0     |
-      | DMTF           | Profile Registration | 1.0.0     |
-      +----------------+----------------------+-----------+
-
-Pywbemcli can also be executed in the interactive (REPL) mode by executing it
-without entering a command or by using the command ``repl``. In this mode
-the command line prompt is ``pywbemcli>``, the WBEM server connection is
-maintained between commands and the general options apply to all commands
-executed:
-
-.. code-block:: text
-
-    $ pywbemcli -n conn1
-    Enter 'help' for help, <CTRL-D> or ':q' to exit pywbemcli.
-    pywbemcli> server brand
-
-    Server Brand:
-    WBEM Server Brand
-    -------------------
-    OpenPegasus
-    pywbemcli> server interop
+- [Documentation](https://pywbemtools.readthedocs.io/en/stable/)
+- [Installation](https://pywbemtools.readthedocs.io/en/stable/introduction.html#installation)
+- [Change history](https://pywbemtools.readthedocs.io/en/stable/changes.html)
+
+# Quickstart
+
+All commands within pywbemcli show help with the `-help` or `-h` options:
+
+``` text
+$ pywbemcli --help
+. . .
+$ pywbemcli connection --help
+. . .
+$ pywbemcli connection save --help
+. . .
+```
+
+The following examples build on each other and show a typical sequence
+of exploration of a WBEM server. For simplicity, they all operate
+against the default namespace of the server, and use a persistent
+connection definition for the WBEM server:
+
+-   Add a persistent connection definition named `conn1` for the WBEM
+    server to be used, so that the subsequent commands can refer to it:
+
+    ``` text
+    $ pywbemcli -s https://localhost --no-verify -u user -p password connection save conn1
+    ```
+
+-   pywbemcli also supports mocked WBEM servers in memory, that are
+    preloaded with CIM objects defined in MOF files. Add a persistent
+    connection definition named `assoc1` to a mock server using one of
+    the MOF files provided in the repo:
+
+    ``` text
+    $ pywbemcli -m tests/unit/simple_assoc_mock_model.mof connection save assoc1
+    ```
+
+-   List the persistent WBEM server connection definitions:
+
+    ``` text
+    $ pywbemcli connection list
+    WBEM server connections(brief): (#: default, *: current)
+    name    server             mock-server
+    ------  -----------------  --------------------------------------
+    assoc1                     tests/unit/simple_assoc_mock_model.mof
+    conn1   https://localhost
+    ```
+
+-   List the persistent WBEM server connection definitions with full information:
+
+    ``` text
+    $ pywbemcli connection list --full
+    WBEM server connections(full): (#: default, *: current)
+    name    server             namespace    user      timeout  use_pull    verify    certfile    keyfile    mock-server
+    ------  -----------------  -----------  ------  ---------  ----------  --------  ----------  ---------  --------------------------------------
+    assoc1                     root/cimv2                  30              True                             tests/unit/simple_assoc_mock_model.mof
+    conn1   https://localhost  root/cimv2   user           30  True        False
+    ```
+
+-   Show the class tree, using the previously added WBEM server connection
+    definition `assoc1` (specified with the `-n` option):
+
+    ``` text
+    $ pywbemcli -n assoc1 class tree
+    root
+     +-- TST_FamilyCollection
+     +-- TST_Lineage
+     +-- TST_MemberOfFamilyCollection
+     +-- TST_Person
+         +-- TST_Personsub
+    ```
+
+-   Retrieve a single class from that class tree:
+
+    ``` text
+    $ pywbemcli -n assoc1 class get TST_Person
+    class TST_Person {
+
+          [Key ( true ),
+           Description ( "This is key prop" )]
+       string name;
+
+       string extraProperty = "defaultvalue";
+
+    };
+    ```
+
+-   Enumerate the instances of that class, returning only their instance
+    names by use of the `--no` option:
+
+    ``` text
+    $ pywbemcli -n assoc1 instance enumerate TST_Person --no
+    root/cimv2:TST_Person.name="Gabi"
+    root/cimv2:TST_Person.name="Mike"
+    root/cimv2:TST_Person.name="Saara"
+    root/cimv2:TST_Person.name="Sofi"
+    root/cimv2:TST_PersonSub.name="Gabisub"
+    root/cimv2:TST_PersonSub.name="Mikesub"
+    root/cimv2:TST_PersonSub.name="Saarasub"
+    root/cimv2:TST_PersonSub.name="Sofisub"
+    ```
+
+-   Retrieve a single instance using one of these instance names:
+
+    ``` text
+    $ pywbemcli -n assoc1 instance get 'root/cimv2:TST_Person.name="Sofi"'
+    instance of TST_Person {
+       name = "Sofi";
+    };
+    ```
+
+-   The instance to be retrieved can also be selected interactively by
+    use of the wildcard instance key (\"CLASSNAME.?\"):
+
+    ``` text
+    $ pywbemcli -n assoc1 instance get TST_Person.?
+    Pick Instance name to process
+    0: root/cimv2:TST_Person.name="Saara"
+    1: root/cimv2:TST_Person.name="Mike"
+    2: root/cimv2:TST_Person.name="Sofi"
+    3: root/cimv2:TST_Person.name="Gabi"
+    4: root/cimv2:TST_PersonSub.name="Gabisub"
+    5: root/cimv2:TST_PersonSub.name="Sofisub"
+    6: root/cimv2:TST_PersonSub.name="Mikesub"
+    7: root/cimv2:TST_PersonSub.name="Saarasub"
+    Input integer between 0 and 7 or Ctrl-C to exit selection: 3
+    instance of TST_Person {
+       name = "Gabi";
+    };
+    ```
+
+-   There are multiple output formats supported. The enumerated
+    instances can for example be formatted as a table of properties by
+    use of the `-o table` general option (these instances have only one
+    property \'name\'):
+
+    ``` text
+    $ pywbemcli -n assoc1 -o table instance enumerate TST_Person
+    Instances: TST_Person
+    +------------+
+    | name       |
+    |------------|
+    | "Gabi"     |
+    | "Mike"     |
+    | "Saara"    |
+    | "Sofi"     |
+    | "Gabisub"  |
+    | "Mikesub"  |
+    | "Saarasub" |
+    | "Sofisub"  |
+    +------------+
+    ```
+
+-   Traverse all associations starting from a specific instance that is
+    selected interactively:
+
+    ``` text
+    $ pywbemcli -n assoc1 -o table instance associators TST_Person.?
+    Pick Instance name to process
+    0: root/cimv2:TST_Person.name="Saara"
+    1: root/cimv2:TST_Person.name="Mike"
+    2: root/cimv2:TST_Person.name="Sofi"
+    3: root/cimv2:TST_Person.name="Gabi"
+    4: root/cimv2:TST_PersonSub.name="Gabisub"
+    5: root/cimv2:TST_PersonSub.name="Sofisub"
+    6: root/cimv2:TST_PersonSub.name="Mikesub"
+    7: root/cimv2:TST_PersonSub.name="Saarasub"
+    Input integer between 0 and 7 or Ctrl-C to exit selection: 1
+    Instances: TST_FamilyCollection
+    +-----------+
+    | name      |
+    |-----------|
+    | "Family2" |
+    | "Gabi"    |
+    | "Sofi"    |
+    +-----------+
+    ```
+
+Other operations against WBEM servers include getting information on
+namespaces, the Interop namespace, WBEM server brand information, or the
+advertised management profiles:
+
+-   Show the Interop namespace of the server:
 
+    ``` text
+    $ pywbemcli -n conn1 server interop
     Server Interop Namespace:
     Namespace Name
     ----------------
     root/PG_InterOp
-    pywbemcli> :q
+    ```
 
+-   List the advertised management profiles:
 
-.. _Documentation: https://pywbemtools.readthedocs.io/en/stable/
-.. _Installation: https://pywbemtools.readthedocs.io/en/stable/introduction.html#installation
-.. _Contributing: https://pywbemtools.readthedocs.io/en/stable/development.html#contributing
-.. _Change history: https://pywbemtools.readthedocs.io/en/stable/changes.html
-.. _pywbemtools issue tracker: https://github.com/pywbem/pywbemtools/issues
-.. _pywbem package on Pypi: https://pypi.org/project/pywbem/
-.. _DMTF: https://www.dmtf.org/
-.. _CIM/WBEM standards: https://www.dmtf.org/standards/wbem/
-.. _DSP0200 (CIM Operations over HTTP): https://www.dmtf.org/sites/default/files/standards/documents/DSP0200_1.4.0.pdf
-.. _SNIA: https://www.snia.org/
-.. _SMI-S: https://www.snia.org/forums/smi/tech_programs/smis_home
-.. _Apache 2.0 License: https://github.com/pywbem/pywbemtools/tree/master/LICENSE.txt
+    ``` text
+    $ pywbemcli -n conn1 server profiles --organization DMTF
+    Advertised management profiles:
+    +----------------+----------------------+-----------+
+    | Organization   | Registered Name      | Version   |
+    |----------------+----------------------+-----------|
+    | DMTF           | CPU                  | 1.0.0     |
+    | DMTF           | Computer System      | 1.0.0     |
+    | DMTF           | Ethernet Port        | 1.0.0     |
+    | DMTF           | Fan                  | 1.0.0     |
+    | DMTF           | Indications          | 1.1.0     |
+    | DMTF           | Profile Registration | 1.0.0     |
+    +----------------+----------------------+-----------+
+    ```
+
+Pywbemcli can also be executed in the interactive (REPL) mode by
+executing it without entering a command or by using the command `repl`.
+In this mode the command line prompt is `pywbemcli>`, the WBEM server
+connection is maintained between commands and the general options apply
+to all commands executed:
+
+``` text
+$ pywbemcli -n conn1
+Enter 'help' for help, <CTRL-D> or ':q' to exit pywbemcli.
+pywbemcli> server brand
+
+Server Brand:
+WBEM Server Brand
+-------------------
+OpenPegasus
+pywbemcli> server interop
+
+Server Interop Namespace:
+Namespace Name
+----------------
+root/PG_InterOp
+pywbemcli> :q
+```
```

### Comparing `pywbemtools-1.2.1/pywbemtools/__init__.py` & `pywbemtools-1.3.0/pywbemtools/__init__.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/_click_extensions.py` & `pywbemtools-1.3.0/pywbemtools/_click_extensions.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/_common_cmd_actions.py` & `pywbemtools-1.3.0/pywbemtools/_common_cmd_actions.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/_options.py` & `pywbemtools-1.3.0/pywbemtools/_options.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/_output_formatting.py` & `pywbemtools-1.3.0/pywbemtools/_output_formatting.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/_utils.py` & `pywbemtools-1.3.0/pywbemtools/_utils.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/_version.py` & `pywbemtools-1.3.0/pywbemtools/_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 #: The full version of this package including any development levels, as a
 #: :term:`string`.
 #:
 #: Possible formats for this version string are:
 #:
 #: * "M.N.P.devD": Development level D of a not yet released version M.N.P
 #: * "M.N.P": A released version M.N.P
-__version__ = '1.2.1'
+__version__ = '1.3.0'
```

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/__init__.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,19 @@
 from __future__ import absolute_import, print_function
 
 from .._utils import *                # noqa: F403,F401
 from .._click_extensions import *     # noqa: F403,F401
 from .._options import *              # noqa: F403,F401
 from .._output_formatting import *    # noqa: F403,F401
 from .._common_cmd_actions import *   # noqa: F403,F401
+
 from ._cmd_namespace import *         # noqa: F403,F401
 from ._common import *                # noqa: F403,F401
 from ._pywbem_server import *         # noqa: F403,F401
+from ._warnings import *              # noqa: F403,F401
 
 from ._cmd_class import *             # noqa: F403,F401
 from ._cmd_instance import *          # noqa: F403,F401
 from ._cmd_qualifier import *         # noqa: F403,F401
 from ._cmd_server import *            # noqa: F403,F401
 from ._cmd_connection import *        # noqa: F403,F401
 from ._cmd_profile import *           # noqa: F403,F401
```

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_association_shrub.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_association_shrub.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_cimvalueformatter.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_cimvalueformatter.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_class.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_class.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_connection.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_connection.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_docs.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_docs.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_help.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_help.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_instance.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_instance.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_namespace.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_namespace.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_profile.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_profile.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_qualifier.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_qualifier.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_server.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_server.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_statistics.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_statistics.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_cmd_subscription.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_cmd_subscription.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_common.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_common.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_common_cmd_functions.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_common_cmd_functions.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_common_options.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_common_options.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_connection_repository.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_connection_repository.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_context_obj.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_context_obj.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_display_cimobjects.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_display_cimobjects.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_displaytree.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_displaytree.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_pywbem_server.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_pywbem_server.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/_pywbemcli_operations.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/_pywbemcli_operations.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/config.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/config.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/mockscripts/__init__.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/mockscripts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     Raises:
       MockScriptError:
       SetupNotSupportedError (py<3.5): New-style setup in mock script not
         supported.
       NotCacheable (py<3.5): Mock environment is not cacheable.
     """
     modpath = get_modpath(file_path)
-    if sys.version_info[0:2] >= (3, 5):
+    if sys.version_info[0:2] >= (3, 6):
         spec = importlib.util.spec_from_file_location(modpath, file_path)
         module = importlib.util.module_from_spec(spec)
 
         # We cannot find out whether the script has a setup() function before
         # executing it, so we have to set the global variables for the old
         # setup approach in any case.
         module.CONN = conn
@@ -175,17 +175,17 @@
     that happens, the logic of the caller is to perform a complete build
     of the mock environment. During that build, script errors or the
     deprecation of the old setup approach will surface.
 
     Raises:
       NotCacheable
     """
-    if sys.version_info[0:2] < (3, 5):
+    if sys.version_info[0:2] == (2, 7):
         raise NotCacheable(
-            "On Python <3.5, mock scripts cannot be cached")
+            "On Python 2.7, mock scripts cannot be cached")
 
     modpath = get_modpath(file_path)
     spec = importlib.util.spec_from_file_location(modpath, file_path)
     module = importlib.util.module_from_spec(spec)
     sys.modules[modpath] = module
     try:
         spec.loader.exec_module(module)
```

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemcli/pywbemcli.py` & `pywbemtools-1.3.0/pywbemtools/pywbemcli/pywbemcli.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from __future__ import absolute_import, print_function
 
 import os
 import io
 import sys
 import warnings
 import traceback
-import six
 import packaging.version
 
 import click
 import click_repl
 from prompt_toolkit.history import FileHistory
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 
@@ -55,28 +54,22 @@
     PYWBEMCLI_HISTORY_FILE, DEFAULT_MAXPULLCNT, DEFAULT_CONNECTION_TIMEOUT, \
     MAX_TIMEOUT, USE_AUTOSUGGEST
 from ._connection_repository import ConnectionRepository, \
     ConnectionsFileError
 from .._click_extensions import PywbemtoolsTopGroup, GENERAL_OPTS_TXT, \
     SUBCMD_HELP_TXT, MutuallyExclusiveOption, click_completion_item
 from .._utils import pywbemtools_warn, get_terminal_width, \
-    CONNECTIONS_FILENAME, DEFAULT_CONNECTIONS_FILE
+    CONNECTIONS_FILENAME, DEFAULT_CONNECTIONS_FILE, debug_log
 from .._options import add_options, help_option
 from .._output_formatting import OUTPUT_FORMAT_GROUPS, OUTPUT_FORMATS
 
+from ._warnings import InvalidConnectionFile, TabCompletionError
 
-__all__ = ['cli']
-
-
-class InvalidConnectionFile(Warning):
-    """
-    Indicates that invalid connection file in startup of interactive mode.
-    """
-    pass
 
+__all__ = ['cli']
 
 # Click version as a tuple. Used to control tab-completion features
 CLICK_VERSION = packaging.version.parse(click.__version__).release
 
 PYWBEMCLI_STARTUP_ENVVAR = "PYWBEMCLI_STARTUP_SCRIPT"
 
 DEFAULT_DEFINITION_NAME = "not-saved"
@@ -120,30 +113,16 @@
 # functions like print cannot easily be used.
 
 def disp_ctx_params(ctx, param, incomplete, verbose=False):
     """
     Display parameters used in the call to a completion function
     """
     if verbose:
-        shell_debug_str("ctx attrs:{0}\nparam:  {1}\n incomplete:  {2}".
-                        format(get_ctx_attrs(ctx), param, incomplete))
-
-
-def shell_debug_str(strng):
-    """
-    Print the string in strng to the file debug.txt. Used in debugging
-    click completion functionality
-    """
-    if six.PY2:
-        # pylint: disable=unspecified-encoding
-        with open('debug.txt', 'a') as f:
-            print("{}".format(strng), file=f)
-    else:
-        with open('debug.txt', 'a', encoding='utf-8') as f:
-            print("{}".format(strng), file=f, flush=True)
+        debug_log("ctx attrs:{0}\nparam:  {1}\n incomplete:  {2}".
+                  format(get_ctx_attrs(ctx), param, incomplete))
 
 
 def get_ctx_attrs(ctx):
     """
     Write to the file debug.txt the ctx, param, and incomplete if verbose
     is True. This is used to debug the completion functions since the terminal
     is already in use as a result of the tab.
@@ -167,38 +146,44 @@
 def connection_name_completer(ctx, param, incomplete):
     # pylint: disable=unused-argument
     """
     Shell complete function for the general option --name.  This function is
     called if <TAB> is entered from terminal as part of the value of the
     --name general option.  It returns all entries in connection table that
     start with the string in incomplete.
-    """
-    connections_file = \
-        ctx.params['connections_file'] or DEFAULT_CONNECTIONS_FILE
-    # Output to stderr since terminal is not available because this only
-    # occurs when shell <TAB> entered to start tab-completion
+
+    If there is an issue with the connections file, a warning is issued and
+    an empty string returned.  This method must not generate an exception
+    because it could pass that back to the shell.
+    """
+    if 'connections_file' in ctx.params:
+        connections_file = \
+            ctx.params['connections_file'] or DEFAULT_CONNECTIONS_FILE
+    else:
+        connections_file = DEFAULT_CONNECTIONS_FILE
     try:
         connections_repo = ConnectionRepository(connections_file)
+        # Test for file exists because defining repo or iteration ignore
+        # not-existent file.
         if not connections_repo.file_exists():
-            # Abort does not allow a message and FileError does not abort.
-            raise click.ClickException("Connection file: {} does not exist.".
-                                       format(connections_file))
+            raise ConnectionsFileError(
+                "Connections file: '{}' does not exist.".
+                format(connections_file))
 
         # Returns list of click CompletionItems from list of keys in
         # the repository.
-        returns = [click_completion_item(name) for name in connections_repo
-                   if name.startswith(incomplete)]
-
-        return returns
+        return [click_completion_item(name) for name in connections_repo
+                if name.startswith(incomplete)]
 
     except ConnectionsFileError as cfe:
-        click.echo('Fatal error: {0}: {1}'.
-                   format(cfe.__class__.__name__, cfe),
-                   err=True)
-        raise click.Abort()
+        pywbemtools_warn(
+            "Connection file: {0},  Fatal Error: {1}: {2}.".
+            format(connections_file, cfe.__class__.__name__, cfe),
+            TabCompletionError)
+        return ""
 
 
 ###########################################################################
 #
 # cli option support functions
 #
 ###########################################################################
```

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemlistener/__init__.py` & `pywbemtools-1.3.0/pywbemtools/pywbemlistener/__init__.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemlistener/_cmd_docs.py` & `pywbemtools-1.3.0/pywbemtools/pywbemlistener/_cmd_docs.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemlistener/_cmd_help.py` & `pywbemtools-1.3.0/pywbemtools/pywbemlistener/_cmd_help.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemlistener/_cmd_listener.py` & `pywbemtools-1.3.0/pywbemtools/pywbemlistener/_cmd_listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,25 @@
                  'Default: {}'.format(DEFAULT_LISTENER_PORT)),
     click.option('-s', '--scheme',
                  type=click.Choice(['http', 'https']),
                  metavar='SCHEME',
                  required=False, default=DEFAULT_LISTENER_SCHEME,
                  help=u'The scheme used by the listener (http, https). '
                  'Default: {}'.format(DEFAULT_LISTENER_SCHEME)),
+    click.option('-b', '--bind-addr',
+                 type=str,
+                 metavar='HOST',
+                 required=False,
+                 default=None,
+                 help=u'A host name or IP address to which this listener '
+                      'will be bound. Binding the listener defines the '
+                      'indication destination host name or IP address for '
+                      'which this listener will accept indications. The '
+                      'default accepts indications addressed to any '
+                      'network interfaces on the listener system.'),
     click.option('-c', '--certfile',
                  type=click.Path(exists=False, dir_okay=False),
                  metavar='FILE',
                  required=False, default=None,
                  envvar=_config.PYWBEMLISTENER_CERTFILE_ENVVAR,
                  help=u'Path name of a PEM file containing the certificate '
                  'that will be presented as a server certificate during '
@@ -181,20 +192,21 @@
 
 
 class ListenerProperties(object):
     """
     The properties of a running named listener.
     """
 
-    def __init__(self, name, port, scheme, certfile, keyfile,
+    def __init__(self, name, port, bind_addr, scheme, certfile, keyfile,
                  indi_call, indi_file, indi_format,
                  logfile, pid, start_pid, created):
         self._name = name
         self._port = port
         self._scheme = scheme
+        self._bind_addr = bind_addr
         self._certfile = certfile
         self._keyfile = keyfile
         self._indi_call = indi_call
         self._indi_file = indi_file
         self._indi_format = indi_format
         self._logfile = logfile
         self._pid = pid
@@ -203,14 +215,15 @@
 
     def show_row(self):
         """Return a tuple of the properties for 'show' command"""
         return (
             self.name,
             str(self.port),
             self.scheme,
+            self.bind_addr or 'none',
             self.certfile,
             self.keyfile,
             self.indi_call,
             self.indi_file,
             self.logfile,
             str(self.pid),
             str(self.start_pid),
@@ -220,14 +233,15 @@
     @staticmethod
     def show_headers():
         """Return a tuple of the header labels for 'show' command"""
         return (
             'Name',
             'Port',
             'Scheme',
+            'Bind addr',
             'Certificate file',
             'Key file',
             'Indication call',
             'Indication file',
             'Log file',
             'PID',
             'Start PID',
@@ -236,25 +250,27 @@
 
     def list_row(self):
         """Return a tuple of the properties for 'list' command"""
         return (
             self.name,
             str(self.port),
             self.scheme,
+            self.bind_addr or 'none',
             str(self.pid),
             self.created.strftime("%Y-%m-%d %H:%M:%S"),
         )
 
     @staticmethod
     def list_headers():
         """Return a tuple of the header labels for 'list' command"""
         return (
             'Name',
             'Port',
             'Scheme',
+            'Bind addr',
             'PID',
             'Created',
         )
 
     @property
     def name(self):
         """string: Name of the listener"""
@@ -262,14 +278,19 @@
 
     @property
     def port(self):
         """int: Port number of the listener"""
         return self._port
 
     @property
+    def bind_addr(self):
+        """int: bind address of the listener"""
+        return self._bind_addr
+
+    @property
     def scheme(self):
         """string: Scheme of the listener"""
         return self._scheme
 
     @property
     def certfile(self):
         """string: Path name of certificate file of the listener"""
@@ -445,14 +466,19 @@
                 cls=TabCompleteArgument,
                 shell_complete=listener_name_completer,
                 required=False)
 @click.option('-c', '--count', type=int, metavar='INT',
               required=False, default=1,
               help=u'Count of test indications to send. '
               'Default: 1')
+@click.option('-l', '--listener', type=str, metavar='HOST',
+              required=False, default='localhost',
+              help=u'Listener host name or IP address. The indications '
+                   'are sent to this host name or IP address. '
+              'Default: localhost')
 @add_options(help_option)
 @click.pass_obj
 def listener_test(context, name, **options):
     """
     Send a test indication to a named WBEM indication listener.
 
     The indication is an alert indication with fixed properties. This allows
@@ -523,15 +549,16 @@
         if args:
             if name is None or args.name == name:
                 # pylint: disable=no-member
                 # Note: This is a workaround for Pylint raising no-member on
                 # Python 3.9 (see issue #1001)
                 logfile = get_logfile(args.logdir, args.name)
                 lis = ListenerProperties(
-                    name=args.name, port=args.port, scheme=args.scheme,
+                    name=args.name, port=args.port, bind_addr=args.bind_addr,
+                    scheme=args.scheme,
                     certfile=args.certfile, keyfile=args.keyfile,
                     indi_call=args.indi_call, indi_file=args.indi_file,
                     indi_format=args.indi_format,
                     logfile=logfile, pid=p.pid, start_pid=args.start_pid,
                     created=datetime.fromtimestamp(p.create_time()))
                 # pylint: enable=no-member
                 # Note: End of workaround
@@ -848,28 +875,30 @@
     Parse the command line arguments of a process. If it is a listener process
     return its parsed arguments (after the 'pywbemlistener' command); otherwise
     return None.
     """
 
     parser = SilentArgumentParser()
 
-    # Note: The following options must ne in sync with the Click general options
+    # Note: The following options must be in sync with the Click general options
     parser.add_argument('--output-format', '-o', type=str, default=None)
     parser.add_argument('--logdir', '-l', type=str, default=None)
     parser.add_argument('--verbose', '-v', action='count', default=0)
     parser.add_argument('--pdb', action='store_true', default=False)
     parser.add_argument('--warn', default=False, action='store_true')
 
     parser.add_argument('run', type=str, default=None)
     parser.add_argument('name', type=str, default=None)
 
     # Note: The following options must ne in sync with the Click command options
     parser.add_argument('--start-pid', type=int, default=None)
     parser.add_argument('--port', '-p', type=int,
                         default=DEFAULT_LISTENER_PORT)
+    parser.add_argument('--bind-addr', '-b', type=str,
+                        default=None)
     parser.add_argument('--scheme', '-s', type=str,
                         default=DEFAULT_LISTENER_SCHEME)
     parser.add_argument('--certfile', type=str, default=None)
     parser.add_argument('--keyfile', type=str, default=None)
     parser.add_argument('--indi-call', type=str, default=None)
     parser.add_argument('--indi-file', type=str, default=None)
     parser.add_argument('--indi-format', type=str, default=None)
@@ -955,15 +984,15 @@
 
 def cmd_listener_run(context, name, options):
     """
     Run as a listener.
     """
     port = options['port']
     scheme = options['scheme']
-    host = 'localhost'
+    bind_addr = options['bind_addr']
 
     start_pid = options['start_pid']
     if start_pid is not None:
         start_pid = int(start_pid)
 
     # If the stdout of the run process is a pipe (e.g. when capturing
     # the output of the run command or its parent start command during
@@ -1031,57 +1060,65 @@
     # process.
     if start_pid:
         atexit.register(run_exit_handler, start_pid, log_fp)
 
     listeners = get_listeners(name)
     if len(listeners) > 1:  # This upcoming listener and a previous one
         lis = listeners[0]
-        url = '{}://{}:{}'.format(lis.scheme, host, lis.port)
+        url = '{}://{}:{}'.format(lis.scheme, bind_addr, lis.port)
         raise click.ClickException(
             "Listener {} already running at {}".format(name, url))
 
     if scheme == 'http':
         http_port = port
         https_port = None
         certfile = None
         keyfile = None
     else:
         assert scheme == 'https'
         https_port = port
         http_port = None
         certfile = options['certfile']
         keyfile = options['keyfile'] or certfile
-    url = '{}://{}:{}'.format(scheme, host, port)
+
+    # If there is no defined bind address, set it to the default value
+    # for a listener that receives indications on any network address.
+    # This allows using None as the default bind_addr elsewhere in the code
+    if not bind_addr:
+        bind_addr = ''
+
+    url = '{}://{}:{}'.format(scheme, bind_addr, port)
 
     context.spinner_stop()
 
     try:
         listener = WBEMListener(
-            host=host, http_port=http_port, https_port=https_port,
+            host=bind_addr, http_port=http_port, https_port=https_port,
             certfile=certfile, keyfile=keyfile)
     except ValueError as exc:
         raise click.ClickException(
             "Cannot create listener {}: {}".format(name, exc))
     try:
         listener.start()
     except (IOError, OSError, ListenerError) as exc:
         raise click.ClickException(
             "Cannot start listener {}: {}".format(name, exc))
 
     indi_call = options['indi_call']
     indi_file = options['indi_file']
     indi_format = options['indi_format'] or DEFAULT_INDI_FORMAT
 
-    def file_func(indication, host):
+    def file_func(indication, indication_host):
         """
         Indication callback function that appends the indication to a file
         using the specified format.
         """
         try:
-            display_str = format_indication(indication, host, indi_format)
+            display_str = format_indication(indication, indication_host,
+                                            indi_format)
         except Exception as exc:  # pylint: disable=broad-except
             display_str = ("Error: Cannot format indication using format "
                            "\"{}\": {}: {}".
                            format(indi_format, exc.__class__.__name__, exc))
         with io.open(indi_file, 'a', encoding='utf-8') as fp:
             fp.write(display_str)
             fp.write(u'\n')
@@ -1160,20 +1197,20 @@
     port = options['port']
     scheme = options['scheme']
     certfile = options['certfile']
     keyfile = options['keyfile']
     indi_call = options['indi_call']
     indi_file = options['indi_file']
     indi_format = options['indi_format']
-    host = 'localhost'
+    bind_addr = options['bind_addr']
 
     listeners = get_listeners(name)
     if listeners:
         lis = listeners[0]
-        url = '{}://{}:{}'.format(lis.scheme, host, lis.port)
+        url = '{}://{}:{}'.format(lis.scheme, bind_addr, lis.port)
         raise click.ClickException(
             "Listener {} already running at {}".format(name, url))
 
     pid = os.getpid()
 
     run_args = [
         'pywbemlistener',
@@ -1184,14 +1221,17 @@
         run_args.extend(['--logdir', context.logdir])
     run_args.extend([
         'run', name,
         '--port', str(port),
         '--scheme', scheme,
         '--start-pid', str(pid),
     ])
+
+    if bind_addr:
+        run_args.extend(['--bind-addr', bind_addr])
     if certfile:
         run_args.extend(['--certfile', certfile])
     if keyfile:
         run_args.extend(['--keyfile', keyfile])
     if indi_call:
         run_args.extend(['--indi-call', indi_call])
     if indi_file:
@@ -1321,22 +1361,24 @@
     click.echo("Sending the following test indication:\n{}".
                format(indication.tomof()))
 
     for i in range(1, count + 1):
 
         indication['MessageID'] = 'TEST{:04d}'.format(i)
 
+        listener_host = options['listener']
+
         conn_kwargs = {}
         conn_kwargs['creds'] = None
         if listener.scheme == 'https':
-            url = 'https://localhost:{}'.format(listener.port)
+            url = 'https://{0}:{1}'.format(listener_host, listener.port)
             conn_kwargs['x509'] = None
             conn_kwargs['no_verification'] = True
         else:  # http
-            url = 'http://localhost:{}'.format(listener.port)
+            url = 'http://{0}:{1}'.format(listener_host, listener.port)
 
         conn = WBEMConnection(url, **conn_kwargs)
 
         try:
             conn.ExportIndication(indication)
         except Error as exc:
             raise click.ClickException(str(exc))
```

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemlistener/_config.py` & `pywbemtools-1.3.0/pywbemtools/pywbemlistener/_config.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemlistener/_context_obj.py` & `pywbemtools-1.3.0/pywbemtools/pywbemlistener/_context_obj.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools/pywbemlistener/pywbemlistener.py` & `pywbemtools-1.3.0/pywbemtools/pywbemlistener/pywbemlistener.py`

 * *Files identical despite different names*

### Comparing `pywbemtools-1.2.1/pywbemtools.egg-info/PKG-INFO` & `pywbemtools-1.3.0/pywbemtools.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywbemtools
-Version: 1.2.1
+Version: 1.3.0
 Summary: Python client tools to work with WBEM Servers using the PyWBEM API.
 Home-page: https://github.com/pywbem/pywbemtools
 Author: Karl Schopmeyer, Andreas Maier
 Author-email: k.schopmeyer@swbell.net, maiera@de.ibm.com
 Maintainer: Karl Schopmeyer, Andreas Maier
 Maintainer-email: k.schopmeyer@swbell.net, maiera@de.ibm.com
 License: Apache License, Version 2.0
@@ -18,345 +18,330 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
-Description-Content-Type: text/x-rst
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: AUTHORS
-Requires-Dist: pywbem>=1.6.3
+Requires-Dist: pywbem>=1.7.2
 Requires-Dist: nocaselist>=1.0.3
 Requires-Dist: nocasedict>=1.0.1
 Requires-Dist: six>=1.14.0; python_version <= "3.9"
 Requires-Dist: six>=1.16.0; python_version >= "3.10"
-Requires-Dist: Click<8.0,>=7.1.1; python_version <= "3.5"
+Requires-Dist: Click<8.0,>=7.1.1; python_version == "2.7"
 Requires-Dist: Click>=8.0.2; python_version >= "3.6"
-Requires-Dist: click-spinner>=0.1.8
-Requires-Dist: click-repl<0.3.0,>=0.1.6; python_version <= "3.5"
+Requires-Dist: click-spinner>=0.1.8; python_version <= "3.11"
+Requires-Dist: click-spinner>=0.1.10; python_version >= "3.12"
+Requires-Dist: click-repl<0.3.0,>=0.1.6; python_version == "2.7"
 Requires-Dist: click-repl<0.3.0,>=0.2; python_version >= "3.6"
 Requires-Dist: asciitree>=0.3.3
 Requires-Dist: tabulate>=0.8.2; python_version <= "3.9"
 Requires-Dist: tabulate>=0.8.8; python_version >= "3.10"
 Requires-Dist: toposort<=1.7,>=1.6; python_version <= "3.7"
 Requires-Dist: toposort>=1.6; python_version >= "3.8"
 Requires-Dist: psutil>=5.5.0; python_version <= "3.9"
 Requires-Dist: psutil>=5.8.0; python_version >= "3.10"
 Requires-Dist: prompt-toolkit<3.0.0,>=1.0.15; python_version == "2.7"
-Requires-Dist: prompt-toolkit<3.0.0,>=2.0.1; python_version == "3.5"
 Requires-Dist: prompt-toolkit>=3.0.13; python_version >= "3.6"
 Requires-Dist: PyYAML>=5.3.1; python_version <= "3.5"
 Requires-Dist: PyYAML!=5.4.0,!=5.4.1,>=5.3.1; python_version >= "3.6" and python_version <= "3.11"
 Requires-Dist: PyYAML!=5.4.0,!=5.4.1,!=6.0.0,>=5.3.1; python_version >= "3.12"
 Requires-Dist: yamlloader>=0.5.5
 Requires-Dist: packaging>=17.0; python_version == "2.7"
-Requires-Dist: packaging>=17.0; python_version == "3.5"
-Requires-Dist: packaging>=21.0; python_version >= "3.6"
+Requires-Dist: packaging<22.0,>=21.0; python_version >= "3.6"
 Requires-Dist: mock<4.0.0,>=3.0.0; python_version < "3.6"
 Requires-Dist: mock>=3.0.0; python_version >= "3.6"
 Requires-Dist: funcsigs>=1.0.2; python_version == "2.7"
-Requires-Dist: pyparsing<3.0.0,>=2.3.1; python_version < "3.5"
-Requires-Dist: pyparsing>=2.3.1; python_version >= "3.5"
-
-.. # README file for Pypi
-
-Pywbemtools is a collection of command line tools that communicate with WBEM
-servers. The tools are written in pure Python and support Python 2 and Python
-3.
+Requires-Dist: pyparsing<3.0.0,>=2.3.1; python_version == "2.7"
+Requires-Dist: pyparsing>=2.3.1; python_version >= "3.6"
+Requires-Dist: urllib3<2.0.0,>=1.26.18; python_version == "2.7"
+Requires-Dist: urllib3<2.0.0,>=1.26.18; python_version == "3.6"
+Requires-Dist: urllib3>=1.26.18; python_version >= "3.7"
+
+Pywbemtools is a collection of command line tools that communicate with
+WBEM servers. The tools are written in pure Python and support Python 2
+and Python 3.
 
 At this point, pywbemtools includes a single command line tool named
-``pywbemcli`` that uses the `pywbem package on Pypi`_ to issue operations to a
-WBEM server using the `CIM/WBEM standards`_ defined by the `DMTF`_ to perform
-system management tasks.
-
-CIM/WBEM standards are used for a wide variety of systems management tasks
-in the industry including DMTF management standards and the `SNIA`_
-Storage Management Initiative Specification (`SMI-S`_).
-
-Pywbemcli provides access to WBEM servers from the command line.
-It provides functionality to:
-
-* Explore the CIM data of WBEM servers. It can manage/inspect the CIM model
-  components including CIM classes, CIM instances, and CIM qualifiers and
-  execute CIM methods and queries on the WBEM server.
-
-* Execute specific CIM-XML operations on the WBEM server as defined in `DMTF`_
-  standard `DSP0200 (CIM Operations over HTTP)`_.
-
-* Inspect and manage WBEM server functionality including:
+`pywbemcli` that uses the
+[pywbem package on Pypi](https://pypi.org/project/pywbem/) to issue operations
+to a WBEM server using the
+[CIM/WBEM standards](https://www.dmtf.org/standards/wbem/) defined by the
+[DMTF](https://www.dmtf.org/) to perform system management tasks.
+
+CIM/WBEM standards are used for a wide variety of systems management
+tasks in the industry including DMTF management standards and the
+[SNIA](https://www.snia.org/) Storage Management Initiative Specification
+([SMI-S](https://www.snia.org/forums/smi/tech_programs/smis_home)).
+
+Pywbemcli provides access to WBEM servers from the command line. It
+provides functionality to:
+
+- Explore the CIM data of WBEM servers. It can manage/inspect the CIM
+  model components including CIM classes, CIM instances, and CIM
+  qualifiers and execute CIM methods and queries on the WBEM server.
+- Execute specific CIM-XML operations on the WBEM server as defined in
+  [DMTF](https://www.dmtf.org/) standard
+  [DSP0200 (CIM Operations over HTTP)](https://www.dmtf.org/sites/default/files/standards/documents/DSP0200_1.4.0.pdf).
+- Inspect and manage WBEM server functionality including:
+  - CIM namespaces
+  - Advertised WBEM management profiles
+  - WBEM server brand and version information
+- Capture detailed information on CIM-XML interactions with the WBEM
+  server including time statistics and details of data flow.
+- Maintain a file with persisted WBEM connection definitions so that
+  pywbemcli can access multiple WBEM servers by name.
+- Provide both a command line mode and an interactive mode where
+  multiple pywbemcli commands can be executed within the context of a
+  WBEM server.
+- Use an integrated mock WBEM server to try out commands. The mock
+  server can be loaded with CIM objects defined in MOF files or via
+  Python scripts.
 
-  * CIM namespaces
-  * Advertised WBEM management profiles
-  * WBEM server brand and version information
-
-* Capture detailed information on CIM-XML interactions with the WBEM server
-  including time statistics and details of data flow.
-
-* Maintain a file with persisted WBEM connection definitions so that pywbemcli
-  can access multiple WBEM servers by name.
-
-* Provide both a command line mode and an interactive mode where multiple
-  pywbemcli commands can be executed within the context of a WBEM server.
-
-* Use an integrated mock WBEM server to try out commands. The mock server
-  can be loaded with CIM objects defined in MOF files or via Python scripts.
-
-Documentation
--------------
+# Documentation
 
 For the latest version of pywbemtools released on Pypi:
 
-* `Documentation`_
-* `Installation`_
-* `Change history`_
-
-Quickstart
-----------
-
-All commands within pywbemcli show help with the ``-help`` or ``-h`` options:
-
-.. code-block:: text
-
-    $ pywbemcli --help
-    . . .
-    $ pywbemcli connection --help
-    . . .
-    $ pywbemcli connection save --help
-    . . .
-
-The following examples build on each other and show a typical sequence of
-exploration of a WBEM server. For simplicity, they all operate against the
-default namespace of the server, and use a persistent connection definition for
-the server:
-
-* Add a persistent connection definition named ``conn1`` for the WBEM server to
-  be used, so that the subsequent commands can refer to it:
-
-  .. code-block:: text
-
-      $ pywbemcli -s https://localhost --no-verify -u user -p password connection save conn1
-
-* pywbemcli also supports mocked WBEM servers in memory, that are preloaded
-  with CIM objects defined in MOF files. Add a persistent connection definition
-  named ``assoc1`` to a mock server using one of the MOF files provided in
-  the repo:
-
-  .. code-block:: text
-
-      $ pywbemcli -m tests/unit/simple_assoc_mock_model.mof connection save assoc1
-
-* List the persistent connection definitions:
-
-  .. code-block:: text
-
-      $ pywbemcli connection list
-      WBEM server connections(brief): (#: default, *: current)
-      name    server             mock-server
-      ------  -----------------  --------------------------------------
-      assoc1                     tests/unit/simple_assoc_mock_model.mof
-      conn1   https://localhost
-
-* List the persistent connection definitions with full information:
-
-  .. code-block:: text
-
-      $ pywbemcli connection list --full
-      WBEM server connections(full): (#: default, *: current)
-      name    server             namespace    user      timeout  use_pull    verify    certfile    keyfile    mock-server
-      ------  -----------------  -----------  ------  ---------  ----------  --------  ----------  ---------  --------------------------------------
-      assoc1                     root/cimv2                  30              True                             tests/unit/simple_assoc_mock_model.mof
-      conn1   https://localhost  root/cimv2   user           30  True        False
-
-* Show the class tree, using the previously added connection definition ``assoc1``:
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 class tree
-      root
-       +-- TST_FamilyCollection
-       +-- TST_Lineage
-       +-- TST_MemberOfFamilyCollection
-       +-- TST_Person
-           +-- TST_Personsub
-
-* Retrieve a single class from that class tree:
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 class get TST_Person
-      class TST_Person {
-
-            [Key ( true ),
-             Description ( "This is key prop" )]
-         string name;
-
-         string extraProperty = "defaultvalue";
-
-      };
-
-* Enumerate the instances of that class, returning only their instance names
-  by use of the ``--no`` option:
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 instance enumerate TST_Person --no
-      root/cimv2:TST_Person.name="Gabi"
-      root/cimv2:TST_Person.name="Mike"
-      root/cimv2:TST_Person.name="Saara"
-      root/cimv2:TST_Person.name="Sofi"
-      root/cimv2:TST_PersonSub.name="Gabisub"
-      root/cimv2:TST_PersonSub.name="Mikesub"
-      root/cimv2:TST_PersonSub.name="Saarasub"
-      root/cimv2:TST_PersonSub.name="Sofisub"
-
-* Retrieve a single instance using one of these instance names:
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 instance get 'root/cimv2:TST_Person.name="Sofi"'
-      instance of TST_Person {
-         name = "Sofi";
-      };
-
-* The instance to be retrieved can also be selected interactively by use of
-  the wildcard instance key ("CLASSNAME.?"):
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 instance get TST_Person.?
-      Pick Instance name to process
-      0: root/cimv2:TST_Person.name="Saara"
-      1: root/cimv2:TST_Person.name="Mike"
-      2: root/cimv2:TST_Person.name="Sofi"
-      3: root/cimv2:TST_Person.name="Gabi"
-      4: root/cimv2:TST_PersonSub.name="Gabisub"
-      5: root/cimv2:TST_PersonSub.name="Sofisub"
-      6: root/cimv2:TST_PersonSub.name="Mikesub"
-      7: root/cimv2:TST_PersonSub.name="Saarasub"
-      Input integer between 0 and 7 or Ctrl-C to exit selection: 3
-      instance of TST_Person {
-         name = "Gabi";
-      };
-
-* There are multiple output formats supported. The enumerated instances can for
-  example be formatted as a table of properties by use of the ``-o table``
-  general option (these instances have only one property 'name'):
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 -o table instance enumerate TST_Person
-      Instances: TST_Person
-      +------------+
-      | name       |
-      |------------|
-      | "Gabi"     |
-      | "Mike"     |
-      | "Saara"    |
-      | "Sofi"     |
-      | "Gabisub"  |
-      | "Mikesub"  |
-      | "Saarasub" |
-      | "Sofisub"  |
-      +------------+
-
-* Traverse all associations starting from a specific instance that is selected
-  interactively:
-
-  .. code-block:: text
-
-      $ pywbemcli -n assoc1 -o table instance associators TST_Person.?
-      Pick Instance name to process
-      0: root/cimv2:TST_Person.name="Saara"
-      1: root/cimv2:TST_Person.name="Mike"
-      2: root/cimv2:TST_Person.name="Sofi"
-      3: root/cimv2:TST_Person.name="Gabi"
-      4: root/cimv2:TST_PersonSub.name="Gabisub"
-      5: root/cimv2:TST_PersonSub.name="Sofisub"
-      6: root/cimv2:TST_PersonSub.name="Mikesub"
-      7: root/cimv2:TST_PersonSub.name="Saarasub"
-      Input integer between 0 and 7 or Ctrl-C to exit selection: 1
-      Instances: TST_FamilyCollection
-      +-----------+
-      | name      |
-      |-----------|
-      | "Family2" |
-      | "Gabi"    |
-      | "Sofi"    |
-      +-----------+
-
-Other operations against WBEM servers include getting information on namespaces,
-the Interop namespace, WBEM server brand information, or the advertised
-management profiles:
-
-* Show the Interop namespace of the server:
-
-  .. code-block:: text
-
-      $ pywbemcli -n conn1 server interop
-      Server Interop Namespace:
-      Namespace Name
-      ----------------
-      root/PG_InterOp
-
-* List the advertised management profiles:
-
-  .. code-block:: text
-
-      $ pywbemcli -n conn1 server profiles --organization DMTF
-      Advertised management profiles:
-      +----------------+----------------------+-----------+
-      | Organization   | Registered Name      | Version   |
-      |----------------+----------------------+-----------|
-      | DMTF           | CPU                  | 1.0.0     |
-      | DMTF           | Computer System      | 1.0.0     |
-      | DMTF           | Ethernet Port        | 1.0.0     |
-      | DMTF           | Fan                  | 1.0.0     |
-      | DMTF           | Indications          | 1.1.0     |
-      | DMTF           | Profile Registration | 1.0.0     |
-      +----------------+----------------------+-----------+
-
-Pywbemcli can also be executed in the interactive (REPL) mode by executing it
-without entering a command or by using the command ``repl``. In this mode
-the command line prompt is ``pywbemcli>``, the WBEM server connection is
-maintained between commands and the general options apply to all commands
-executed:
-
-.. code-block:: text
-
-    $ pywbemcli -n conn1
-    Enter 'help' for help, <CTRL-D> or ':q' to exit pywbemcli.
-    pywbemcli> server brand
-
-    Server Brand:
-    WBEM Server Brand
-    -------------------
-    OpenPegasus
-    pywbemcli> server interop
+- [Documentation](https://pywbemtools.readthedocs.io/en/stable/)
+- [Installation](https://pywbemtools.readthedocs.io/en/stable/introduction.html#installation)
+- [Change history](https://pywbemtools.readthedocs.io/en/stable/changes.html)
+
+# Quickstart
+
+All commands within pywbemcli show help with the `-help` or `-h` options:
+
+``` text
+$ pywbemcli --help
+. . .
+$ pywbemcli connection --help
+. . .
+$ pywbemcli connection save --help
+. . .
+```
+
+The following examples build on each other and show a typical sequence
+of exploration of a WBEM server. For simplicity, they all operate
+against the default namespace of the server, and use a persistent
+connection definition for the WBEM server:
+
+-   Add a persistent connection definition named `conn1` for the WBEM
+    server to be used, so that the subsequent commands can refer to it:
+
+    ``` text
+    $ pywbemcli -s https://localhost --no-verify -u user -p password connection save conn1
+    ```
+
+-   pywbemcli also supports mocked WBEM servers in memory, that are
+    preloaded with CIM objects defined in MOF files. Add a persistent
+    connection definition named `assoc1` to a mock server using one of
+    the MOF files provided in the repo:
+
+    ``` text
+    $ pywbemcli -m tests/unit/simple_assoc_mock_model.mof connection save assoc1
+    ```
+
+-   List the persistent WBEM server connection definitions:
+
+    ``` text
+    $ pywbemcli connection list
+    WBEM server connections(brief): (#: default, *: current)
+    name    server             mock-server
+    ------  -----------------  --------------------------------------
+    assoc1                     tests/unit/simple_assoc_mock_model.mof
+    conn1   https://localhost
+    ```
+
+-   List the persistent WBEM server connection definitions with full information:
+
+    ``` text
+    $ pywbemcli connection list --full
+    WBEM server connections(full): (#: default, *: current)
+    name    server             namespace    user      timeout  use_pull    verify    certfile    keyfile    mock-server
+    ------  -----------------  -----------  ------  ---------  ----------  --------  ----------  ---------  --------------------------------------
+    assoc1                     root/cimv2                  30              True                             tests/unit/simple_assoc_mock_model.mof
+    conn1   https://localhost  root/cimv2   user           30  True        False
+    ```
+
+-   Show the class tree, using the previously added WBEM server connection
+    definition `assoc1` (specified with the `-n` option):
+
+    ``` text
+    $ pywbemcli -n assoc1 class tree
+    root
+     +-- TST_FamilyCollection
+     +-- TST_Lineage
+     +-- TST_MemberOfFamilyCollection
+     +-- TST_Person
+         +-- TST_Personsub
+    ```
+
+-   Retrieve a single class from that class tree:
+
+    ``` text
+    $ pywbemcli -n assoc1 class get TST_Person
+    class TST_Person {
+
+          [Key ( true ),
+           Description ( "This is key prop" )]
+       string name;
+
+       string extraProperty = "defaultvalue";
+
+    };
+    ```
+
+-   Enumerate the instances of that class, returning only their instance
+    names by use of the `--no` option:
+
+    ``` text
+    $ pywbemcli -n assoc1 instance enumerate TST_Person --no
+    root/cimv2:TST_Person.name="Gabi"
+    root/cimv2:TST_Person.name="Mike"
+    root/cimv2:TST_Person.name="Saara"
+    root/cimv2:TST_Person.name="Sofi"
+    root/cimv2:TST_PersonSub.name="Gabisub"
+    root/cimv2:TST_PersonSub.name="Mikesub"
+    root/cimv2:TST_PersonSub.name="Saarasub"
+    root/cimv2:TST_PersonSub.name="Sofisub"
+    ```
+
+-   Retrieve a single instance using one of these instance names:
+
+    ``` text
+    $ pywbemcli -n assoc1 instance get 'root/cimv2:TST_Person.name="Sofi"'
+    instance of TST_Person {
+       name = "Sofi";
+    };
+    ```
+
+-   The instance to be retrieved can also be selected interactively by
+    use of the wildcard instance key (\"CLASSNAME.?\"):
+
+    ``` text
+    $ pywbemcli -n assoc1 instance get TST_Person.?
+    Pick Instance name to process
+    0: root/cimv2:TST_Person.name="Saara"
+    1: root/cimv2:TST_Person.name="Mike"
+    2: root/cimv2:TST_Person.name="Sofi"
+    3: root/cimv2:TST_Person.name="Gabi"
+    4: root/cimv2:TST_PersonSub.name="Gabisub"
+    5: root/cimv2:TST_PersonSub.name="Sofisub"
+    6: root/cimv2:TST_PersonSub.name="Mikesub"
+    7: root/cimv2:TST_PersonSub.name="Saarasub"
+    Input integer between 0 and 7 or Ctrl-C to exit selection: 3
+    instance of TST_Person {
+       name = "Gabi";
+    };
+    ```
+
+-   There are multiple output formats supported. The enumerated
+    instances can for example be formatted as a table of properties by
+    use of the `-o table` general option (these instances have only one
+    property \'name\'):
+
+    ``` text
+    $ pywbemcli -n assoc1 -o table instance enumerate TST_Person
+    Instances: TST_Person
+    +------------+
+    | name       |
+    |------------|
+    | "Gabi"     |
+    | "Mike"     |
+    | "Saara"    |
+    | "Sofi"     |
+    | "Gabisub"  |
+    | "Mikesub"  |
+    | "Saarasub" |
+    | "Sofisub"  |
+    +------------+
+    ```
+
+-   Traverse all associations starting from a specific instance that is
+    selected interactively:
+
+    ``` text
+    $ pywbemcli -n assoc1 -o table instance associators TST_Person.?
+    Pick Instance name to process
+    0: root/cimv2:TST_Person.name="Saara"
+    1: root/cimv2:TST_Person.name="Mike"
+    2: root/cimv2:TST_Person.name="Sofi"
+    3: root/cimv2:TST_Person.name="Gabi"
+    4: root/cimv2:TST_PersonSub.name="Gabisub"
+    5: root/cimv2:TST_PersonSub.name="Sofisub"
+    6: root/cimv2:TST_PersonSub.name="Mikesub"
+    7: root/cimv2:TST_PersonSub.name="Saarasub"
+    Input integer between 0 and 7 or Ctrl-C to exit selection: 1
+    Instances: TST_FamilyCollection
+    +-----------+
+    | name      |
+    |-----------|
+    | "Family2" |
+    | "Gabi"    |
+    | "Sofi"    |
+    +-----------+
+    ```
+
+Other operations against WBEM servers include getting information on
+namespaces, the Interop namespace, WBEM server brand information, or the
+advertised management profiles:
+
+-   Show the Interop namespace of the server:
 
+    ``` text
+    $ pywbemcli -n conn1 server interop
     Server Interop Namespace:
     Namespace Name
     ----------------
     root/PG_InterOp
-    pywbemcli> :q
+    ```
 
+-   List the advertised management profiles:
 
-.. _Documentation: https://pywbemtools.readthedocs.io/en/stable/
-.. _Installation: https://pywbemtools.readthedocs.io/en/stable/introduction.html#installation
-.. _Contributing: https://pywbemtools.readthedocs.io/en/stable/development.html#contributing
-.. _Change history: https://pywbemtools.readthedocs.io/en/stable/changes.html
-.. _pywbemtools issue tracker: https://github.com/pywbem/pywbemtools/issues
-.. _pywbem package on Pypi: https://pypi.org/project/pywbem/
-.. _DMTF: https://www.dmtf.org/
-.. _CIM/WBEM standards: https://www.dmtf.org/standards/wbem/
-.. _DSP0200 (CIM Operations over HTTP): https://www.dmtf.org/sites/default/files/standards/documents/DSP0200_1.4.0.pdf
-.. _SNIA: https://www.snia.org/
-.. _SMI-S: https://www.snia.org/forums/smi/tech_programs/smis_home
-.. _Apache 2.0 License: https://github.com/pywbem/pywbemtools/tree/master/LICENSE.txt
+    ``` text
+    $ pywbemcli -n conn1 server profiles --organization DMTF
+    Advertised management profiles:
+    +----------------+----------------------+-----------+
+    | Organization   | Registered Name      | Version   |
+    |----------------+----------------------+-----------|
+    | DMTF           | CPU                  | 1.0.0     |
+    | DMTF           | Computer System      | 1.0.0     |
+    | DMTF           | Ethernet Port        | 1.0.0     |
+    | DMTF           | Fan                  | 1.0.0     |
+    | DMTF           | Indications          | 1.1.0     |
+    | DMTF           | Profile Registration | 1.0.0     |
+    +----------------+----------------------+-----------+
+    ```
+
+Pywbemcli can also be executed in the interactive (REPL) mode by
+executing it without entering a command or by using the command `repl`.
+In this mode the command line prompt is `pywbemcli>`, the WBEM server
+connection is maintained between commands and the general options apply
+to all commands executed:
+
+``` text
+$ pywbemcli -n conn1
+Enter 'help' for help, <CTRL-D> or ':q' to exit pywbemcli.
+pywbemcli> server brand
+
+Server Brand:
+WBEM Server Brand
+-------------------
+OpenPegasus
+pywbemcli> server interop
+
+Server Interop Namespace:
+Namespace Name
+----------------
+root/PG_InterOp
+pywbemcli> :q
+```
```

### Comparing `pywbemtools-1.2.1/pywbemtools.egg-info/SOURCES.txt` & `pywbemtools-1.3.0/pywbemtools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTHORS
 LICENSE.txt
 MANIFEST.in
-README.rst
-README_PYPI.rst
+README.md
+README_PYPI.md
 requirements.txt
 setup.py
 pywbemtools/__init__.py
 pywbemtools/_click_extensions.py
 pywbemtools/_common_cmd_actions.py
 pywbemtools/_options.py
 pywbemtools/_output_formatting.py
@@ -38,14 +38,15 @@
 pywbemtools/pywbemcli/_common_options.py
 pywbemtools/pywbemcli/_connection_repository.py
 pywbemtools/pywbemcli/_context_obj.py
 pywbemtools/pywbemcli/_display_cimobjects.py
 pywbemtools/pywbemcli/_displaytree.py
 pywbemtools/pywbemcli/_pywbem_server.py
 pywbemtools/pywbemcli/_pywbemcli_operations.py
+pywbemtools/pywbemcli/_warnings.py
 pywbemtools/pywbemcli/config.py
 pywbemtools/pywbemcli/pywbemcli.py
 pywbemtools/pywbemcli/mockscripts/__init__.py
 pywbemtools/pywbemlistener/__init__.py
 pywbemtools/pywbemlistener/_cmd_docs.py
 pywbemtools/pywbemlistener/_cmd_help.py
 pywbemtools/pywbemlistener/_cmd_listener.py
```

### Comparing `pywbemtools-1.2.1/pywbemtools.egg-info/requires.txt` & `pywbemtools-1.3.0/pywbemtools.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,60 @@
-pywbem>=1.6.3
+pywbem>=1.7.2
 nocaselist>=1.0.3
 nocasedict>=1.0.1
-click-spinner>=0.1.8
 asciitree>=0.3.3
 yamlloader>=0.5.5
 
-[:python_version < "3.5"]
-pyparsing<3.0.0,>=2.3.1
-
 [:python_version < "3.6"]
 mock<4.0.0,>=3.0.0
 
+[:python_version <= "3.11"]
+click-spinner>=0.1.8
+
 [:python_version <= "3.5"]
-Click<8.0,>=7.1.1
-click-repl<0.3.0,>=0.1.6
 PyYAML>=5.3.1
 
 [:python_version <= "3.7"]
 toposort<=1.7,>=1.6
 
 [:python_version <= "3.9"]
 six>=1.14.0
 tabulate>=0.8.2
 psutil>=5.5.0
 
 [:python_version == "2.7"]
+Click<8.0,>=7.1.1
+click-repl<0.3.0,>=0.1.6
 prompt-toolkit<3.0.0,>=1.0.15
 packaging>=17.0
 funcsigs>=1.0.2
+pyparsing<3.0.0,>=2.3.1
+urllib3<2.0.0,>=1.26.18
 
-[:python_version == "3.5"]
-prompt-toolkit<3.0.0,>=2.0.1
-packaging>=17.0
+[:python_version == "3.6"]
+urllib3<2.0.0,>=1.26.18
 
 [:python_version >= "3.10"]
 six>=1.16.0
 tabulate>=0.8.8
 psutil>=5.8.0
 
 [:python_version >= "3.12"]
+click-spinner>=0.1.10
 PyYAML!=5.4.0,!=5.4.1,!=6.0.0,>=5.3.1
 
-[:python_version >= "3.5"]
-pyparsing>=2.3.1
-
 [:python_version >= "3.6"]
 Click>=8.0.2
 click-repl<0.3.0,>=0.2
 prompt-toolkit>=3.0.13
-packaging>=21.0
+packaging<22.0,>=21.0
 mock>=3.0.0
+pyparsing>=2.3.1
 
 [:python_version >= "3.6" and python_version <= "3.11"]
 PyYAML!=5.4.0,!=5.4.1,>=5.3.1
 
+[:python_version >= "3.7"]
+urllib3>=1.26.18
+
 [:python_version >= "3.8"]
 toposort>=1.6
```

### Comparing `pywbemtools-1.2.1/requirements.txt` & `pywbemtools-1.3.0/requirements.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-# Pip requirements file for pywbemtools runtime dependencies.
-#
-# The order of packages is significant, because pip processes them in the order
-# of appearance.
+# Pip requirements file for install dependencies.
 
-# Make sure that the package versions in minimum-constraints.txt are also
-# the minimum versions required in requirements.txt and dev-requirements.txt.
+# Note: The dependencies in this file will become the dependencies stated
+# in the Pypi package metadata.
 
-# Direct dependencies (except pip, setuptools, wheel):
 
-pywbem>=1.6.3
+# Direct dependencies for install (must be consistent with minimum-constraints-install.txt)
+
+pywbem>=1.7.2
 # When using the GitHub master branch of pywbem, comment out the line above,
 # activate the GitHub link based dependency below.
 # In that case, some of the install tests need to be disabled by setting
 # the 'PYWBEM_FROM_REPO' variable in in tests/install/test_install.sh.
 # git+https://github.com/pywbem/pywbem.git@master#egg=pywbem
 
 nocaselist>=1.0.3
@@ -22,21 +20,22 @@
 six>=1.16.0; python_version >= '3.10'
 # Click 7.0 has issue #1231 on Windows which we circumvent in the test code
 # Click 7.1 has a bug with output capturing
 # Click 8.0 is incompatible with python <3.0. See issues #816 (python 2.7 not
 #     supported) and #819 (click-repl incompatible)
 # The Click requirements were copied into dev-requirements.txt in order not to
 # have the safety package upgrade it. Keep them in sync.
-Click>=7.1.1,<8.0; python_version <= '3.5'
+Click>=7.1.1,<8.0; python_version == '2.7'
 # Safety package requires click 8.0.2 minimum
 Click>=8.0.2; python_version >= '3.6'
-click-spinner>=0.1.8
+click-spinner>=0.1.8; python_version <= '3.11'
+click-spinner>=0.1.10; python_version >= '3.12'
 # click-repl 0.2 is needed for compatibility with Click 8.0.
 # click-repl version 3.0 causes test failures. See issue #1312
-click-repl>=0.1.6,<0.3.0; python_version <= '3.5'
+click-repl>=0.1.6,<0.3.0; python_version == '2.7'
 click-repl>=0.2,<0.3.0; python_version >= '3.6'
 asciitree>=0.3.3
 # tabulate 0.8.8 fixes ImportError on Python 3.10.
 tabulate>=0.8.2; python_version <= '3.9'
 tabulate>=0.8.8; python_version >= '3.10'
 
 # Toposort version < 1.7 Fail with python <= 3.7
@@ -47,15 +46,14 @@
 psutil>=5.8.0; python_version >= '3.10'
 
 # prompt-toolkit>=2.0 failed on py27 (issue #192), so it was pinned to <2.0.
 #   Later, the fix for issue #224 allowed to lift that pinning.
 # prompt-toolkit>=3.0 does not support py<36.
 # prompt-toolkit>=3.0 may cause WinError 995 on py38 on Windows (issue #690).
 prompt-toolkit>=1.0.15,<3.0.0; python_version == '2.7'
-prompt-toolkit>=2.0.1,<3.0.0; python_version == '3.5'
 prompt-toolkit>=3.0.13; python_version >= '3.6'
 
 # PyYAML is also pulled in by dparse and python-coveralls
 # PyYAML 5.3 fixed narrow build error on Python 2.7
 # PyYAML 5.3.1 addressed issue 38100 reported by safety
 # PyYAML 5.2 addressed issue 38639 reported by safety
 # PyYAML 5.3 has wheel archives for Python 2.7, 3.5 - 3.9
@@ -64,23 +62,36 @@
 # PyYAML 5.4 and 6.0.0 fails install since Cython 3 was released, see issue
 #   https://github.com/yaml/pyyaml/issues/724.
 PyYAML>=5.3.1; python_version <= '3.5'
 PyYAML>=5.3.1,!=5.4.0,!=5.4.1; python_version >= '3.6' and python_version <= '3.11'
 PyYAML>=5.3.1,!=5.4.0,!=5.4.1,!=6.0.0; python_version >= '3.12'
 
 yamlloader>=0.5.5
+
+# safety 2.3.5 started pinning packaging to <22.0 and requires >=21.0
 packaging>=17.0; python_version == '2.7'
-packaging>=17.0; python_version == '3.5'
-packaging>=21.0; python_version >= '3.6'
+packaging>=21.0,<22.0; python_version >= '3.6'
 
 # See issue #822 about issue in mock 4.0.3.
 mock>=3.0.0,<4.0.0; python_version < '3.6'
 mock>=3.0.0; python_version >= '3.6'
 
+
+# Indirect dependencies for install that are needed for some reason (must be
+# consistent with minimum-constraints-install.txt)
+
 # Mock requires funcsigs>1;python_version<"3.3" but for unknown reasons
 # Pip 9.0.1 (with minimum package levels) does not install it on MacOs on Python
 # 2.7.17. The same version of Pip does install it on Linux on python 2.7.15.
 funcsigs>=1.0.2; python_version == '2.7'
 
 # Address issue that pyparsing 3.0.0b2 gets installed on py27 (used by packaging)
-pyparsing>=2.3.1,<3.0.0; python_version < '3.5'
-pyparsing>=2.3.1; python_version >= '3.5'
+pyparsing>=2.3.1,<3.0.0; python_version == '2.7'
+pyparsing>=2.3.1; python_version >= '3.6'
+
+# urllib3 < 2.0.0 required for python < 3.7
+# TODO: Following limits use of urllib3 <= 2.0  for python < 3.7 until issues
+# about upgrade resolved. Issue #1302 updates urllib3 to version 2.0.
+# Python <= 3.7 required for urllib3 <= 2.0.0
+urllib3>=1.26.18,<2.0.0; python_version == '2.7'
+urllib3>=1.26.18,<2.0.0; python_version == '3.6'
+urllib3>=1.26.18; python_version >= '3.7'
```

### Comparing `pywbemtools-1.2.1/setup.py` & `pywbemtools-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,16 +94,16 @@
     },
     include_package_data=True,  # as specified in MANIFEST.in
     install_requires=install_requires,
     dependency_links=dependency_links,
 
     description='Python client tools to work with WBEM Servers using the '
     'PyWBEM API.',
-    long_description=read_file('README_PYPI.rst'),
-    long_description_content_type='text/x-rst',
+    long_description=read_file('README_PYPI.md'),
+    long_description_content_type='text/markdown',
     license='Apache License, Version 2.0',
     author='Karl Schopmeyer, Andreas Maier',
     author_email='k.schopmeyer@swbell.net, maiera@de.ibm.com',
     maintainer='Karl Schopmeyer, Andreas Maier',
     maintainer_email='k.schopmeyer@swbell.net, maiera@de.ibm.com',
     url='https://github.com/pywbem/pywbemtools',
     project_urls={
@@ -113,28 +113,29 @@
     },
 
     options={'bdist_wheel': {'universal': True}},
     zip_safe=True,  # This package can safely be installed from a zip file
     platforms='any',
 
     # Keep these Python versions in sync with pywbemtools/__init__.py
-    python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*',
+    python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, ' \
+    '!=3.5.*',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ]
 )
```

