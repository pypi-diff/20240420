# Comparing `tmp/ovinc_client-0.1.9.tar.gz` & `tmp/ovinc_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovinc_client-0.1.9.tar", last modified: Sun Mar 24 06:52:29 2024, max compression
+gzip compressed data, was "ovinc_client-0.2.0.tar", last modified: Sat Apr 20 09:51:54 2024, max compression
```

## Comparing `ovinc_client-0.1.9.tar` & `ovinc_client-0.2.0.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 06:52:29.423990 ovinc_client-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-24 06:52:29.423990 ovinc_client-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 06:52:29.415990 ovinc_client-0.1.9/ovinc_client/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 06:52:29.419990 ovinc_client-0.1.9/ovinc_client/account/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/account/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/account/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/account/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/account/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 06:52:29.419990 ovinc_client-0.1.9/ovinc_client/account/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/account/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/account/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/account/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/account/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/account/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/account/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 06:52:29.419990 ovinc_client-0.1.9/ovinc_client/components/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/components/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/components/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/components/notice.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 06:52:29.423990 ovinc_client-0.1.9/ovinc_client/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/core/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/core/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/core/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/core/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/core/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/core/paginations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/core/renderers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/core/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 06:52:29.423990 ovinc_client-0.1.9/ovinc_client/trace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/trace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/trace/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/trace/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/trace/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/trace/instrumentors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/trace/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/trace/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/trace/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/ovinc_client/trace/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 06:52:29.423990 ovinc_client-0.1.9/ovinc_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-24 06:52:29.000000 ovinc_client-0.1.9/ovinc_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-03-24 06:52:29.000000 ovinc_client-0.1.9/ovinc_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 06:52:29.000000 ovinc_client-0.1.9/ovinc_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-24 06:52:29.000000 ovinc_client-0.1.9/ovinc_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-24 06:52:29.000000 ovinc_client-0.1.9/ovinc_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 06:52:29.423990 ovinc_client-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-24 06:52:25.000000 ovinc_client-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:51:54.647715 ovinc_client-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-20 09:51:54.647715 ovinc_client-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:51:54.639715 ovinc_client-0.2.0/ovinc_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:51:54.643715 ovinc_client-0.2.0/ovinc_client/account/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/account/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/account/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/account/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/account/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:51:54.643715 ovinc_client-0.2.0/ovinc_client/account/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/account/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/account/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/account/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/account/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/account/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/account/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:51:54.643715 ovinc_client-0.2.0/ovinc_client/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/components/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/components/notice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/components/tcaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:51:54.647715 ovinc_client-0.2.0/ovinc_client/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/core/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/core/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/core/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/core/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/core/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/core/paginations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/core/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/core/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:51:54.647715 ovinc_client-0.2.0/ovinc_client/trace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/trace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/trace/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/trace/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/trace/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/trace/instrumentors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/trace/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/trace/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/trace/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/ovinc_client/trace/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:51:54.647715 ovinc_client-0.2.0/ovinc_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-20 09:51:54.000000 ovinc_client-0.2.0/ovinc_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-20 09:51:54.000000 ovinc_client-0.2.0/ovinc_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 09:51:54.000000 ovinc_client-0.2.0/ovinc_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-20 09:51:54.000000 ovinc_client-0.2.0/ovinc_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-20 09:51:54.000000 ovinc_client-0.2.0/ovinc_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 09:51:54.647715 ovinc_client-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-20 09:51:50.000000 ovinc_client-0.2.0/setup.py
```

### Comparing `ovinc_client-0.1.9/LICENSE` & `ovinc_client-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/PKG-INFO` & `ovinc_client-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovinc_client
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Tool for OVINC Union API
 Home-page: https://www.ovinc.cn/
 Author: OVINC
 Author-email: contact@ovinc.cn
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django<5,>=4
@@ -42,7 +42,11 @@
 ### Auth
 
 Available: `verify_code`
 
 ### Notice
 
 Available: `mail` `sms` `robot`
+
+### TCaptcha
+
+Available: `tcaptcha`
```

### Comparing `ovinc_client-0.1.9/ovinc_client/account/constants.py` & `ovinc_client-0.2.0/ovinc_client/account/constants.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/account/migrations/0001_initial.py` & `ovinc_client-0.2.0/ovinc_client/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/account/models.py` & `ovinc_client-0.2.0/ovinc_client/account/models.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/account/serializers.py` & `ovinc_client-0.2.0/ovinc_client/account/serializers.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/account/views.py` & `ovinc_client-0.2.0/ovinc_client/account/views.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/client.py` & `ovinc_client-0.2.0/ovinc_client/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import json
 import os
 from json import JSONDecodeError
 
 import requests
 from requests import HTTPError, Response
 
-from ovinc_client.components import Notice
 from ovinc_client.components.auth import Auth
+from ovinc_client.components.notice import Notice
+from ovinc_client.components.tcaptcha import TCaptcha
 from ovinc_client.constants import (
     APP_AUTH_HEADER_KEY,
     APP_AUTH_ID_KEY,
     APP_AUTH_SECRET_KEY,
     OVINC_CLIENT_SIGNATURE,
     OVINC_CLIENT_TIMEOUT,
     RequestMethodEnum,
@@ -27,14 +28,15 @@
 
     def __init__(self, app_code: str, app_secret: str, union_api_url: str):
         self._app_code = app_code
         self._app_secret = app_secret
         self._union_api_url = union_api_url
         self.notice = Notice(self, self._union_api_url)
         self.auth = Auth(self, self._union_api_url)
+        self.tcaptcha = TCaptcha(self, self._union_api_url)
 
     def call_api(self, method: str, url: str, params: dict, timeout: float = OVINC_CLIENT_TIMEOUT) -> ResponseData:
         """
         call union api
         """
 
         # init kwargs
```

### Comparing `ovinc_client-0.1.9/ovinc_client/components/base.py` & `ovinc_client-0.2.0/ovinc_client/components/base.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/components/notice.py` & `ovinc_client-0.2.0/ovinc_client/components/notice.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/core/auth.py` & `ovinc_client-0.2.0/ovinc_client/core/auth.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/core/cache.py` & `ovinc_client-0.2.0/ovinc_client/core/cache.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/core/constants.py` & `ovinc_client-0.2.0/ovinc_client/core/constants.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/core/exceptions.py` & `ovinc_client-0.2.0/ovinc_client/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/core/lock.py` & `ovinc_client-0.2.0/ovinc_client/core/lock.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/core/logger.py` & `ovinc_client-0.2.0/ovinc_client/core/logger.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/core/middlewares.py` & `ovinc_client-0.2.0/ovinc_client/core/middlewares.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/core/models.py` & `ovinc_client-0.2.0/ovinc_client/core/models.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/core/paginations.py` & `ovinc_client-0.2.0/ovinc_client/core/paginations.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/core/renderers.py` & `ovinc_client-0.2.0/ovinc_client/core/renderers.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/core/utils.py` & `ovinc_client-0.2.0/ovinc_client/core/utils.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/core/viewsets.py` & `ovinc_client-0.2.0/ovinc_client/core/viewsets.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/trace/constants.py` & `ovinc_client-0.2.0/ovinc_client/trace/constants.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/trace/exporters.py` & `ovinc_client-0.2.0/ovinc_client/trace/exporters.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/trace/instrumentors.py` & `ovinc_client-0.2.0/ovinc_client/trace/instrumentors.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/trace/setup.py` & `ovinc_client-0.2.0/ovinc_client/trace/setup.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/trace/utils.py` & `ovinc_client-0.2.0/ovinc_client/trace/utils.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client/trace/views.py` & `ovinc_client-0.2.0/ovinc_client/trace/views.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/ovinc_client.egg-info/PKG-INFO` & `ovinc_client-0.2.0/ovinc_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovinc_client
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Tool for OVINC Union API
 Home-page: https://www.ovinc.cn/
 Author: OVINC
 Author-email: contact@ovinc.cn
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django<5,>=4
@@ -42,7 +42,11 @@
 ### Auth
 
 Available: `verify_code`
 
 ### Notice
 
 Available: `mail` `sms` `robot`
+
+### TCaptcha
+
+Available: `tcaptcha`
```

### Comparing `ovinc_client-0.1.9/ovinc_client.egg-info/SOURCES.txt` & `ovinc_client-0.2.0/ovinc_client.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 ovinc_client/account/views.py
 ovinc_client/account/migrations/0001_initial.py
 ovinc_client/account/migrations/__init__.py
 ovinc_client/components/__init__.py
 ovinc_client/components/auth.py
 ovinc_client/components/base.py
 ovinc_client/components/notice.py
+ovinc_client/components/tcaptcha.py
 ovinc_client/core/__init__.py
 ovinc_client/core/auth.py
 ovinc_client/core/cache.py
 ovinc_client/core/constants.py
 ovinc_client/core/exceptions.py
 ovinc_client/core/lock.py
 ovinc_client/core/logger.py
```

### Comparing `ovinc_client-0.1.9/ovinc_client.egg-info/requires.txt` & `ovinc_client-0.2.0/ovinc_client.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.1.9/setup.py` & `ovinc_client-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="ovinc_client",
-    version="0.1.9",
+    version="0.2.0",
     author="OVINC",
     url="https://www.ovinc.cn/",
     author_email="contact@ovinc.cn",
     description="A Tool for OVINC Union API",
     packages=[
         "ovinc_client",
         "ovinc_client.account",
```

