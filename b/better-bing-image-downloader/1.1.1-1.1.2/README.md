# Comparing `tmp/better_bing_image_downloader-1.1.1.tar.gz` & `tmp/better_bing_image_downloader-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_bing_image_downloader-1.1.1.tar", last modified: Mon Apr  1 16:25:55 2024, max compression
+gzip compressed data, was "better_bing_image_downloader-1.1.2.tar", last modified: Sat Apr 20 19:06:11 2024, max compression
```

## Comparing `better_bing_image_downloader-1.1.1.tar` & `better_bing_image_downloader-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:25:55.889739 better_bing_image_downloader-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-01 16:25:51.000000 better_bing_image_downloader-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-01 16:25:55.889739 better_bing_image_downloader-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-01 16:25:51.000000 better_bing_image_downloader-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:25:55.885739 better_bing_image_downloader-1.1.1/better_bing_image_downloader/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-01 16:25:51.000000 better_bing_image_downloader-1.1.1/better_bing_image_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8684 2024-04-01 16:25:51.000000 better_bing_image_downloader-1.1.1/better_bing_image_downloader/bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-01 16:25:51.000000 better_bing_image_downloader-1.1.1/better_bing_image_downloader/download.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:25:55.889739 better_bing_image_downloader-1.1.1/better_bing_image_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-01 16:25:55.000000 better_bing_image_downloader-1.1.1/better_bing_image_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-01 16:25:55.000000 better_bing_image_downloader-1.1.1/better_bing_image_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:25:55.000000 better_bing_image_downloader-1.1.1/better_bing_image_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-01 16:25:55.000000 better_bing_image_downloader-1.1.1/better_bing_image_downloader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 16:25:55.889739 better_bing_image_downloader-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-01 16:25:51.000000 better_bing_image_downloader-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:25:55.889739 better_bing_image_downloader-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-01 16:25:51.000000 better_bing_image_downloader-1.1.1/tests/test_bing.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:25:51.000000 better_bing_image_downloader-1.1.1/tests/test_download.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:06:11.318972 better_bing_image_downloader-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-20 19:06:07.000000 better_bing_image_downloader-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-04-20 19:06:11.318972 better_bing_image_downloader-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-20 19:06:07.000000 better_bing_image_downloader-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:06:11.314972 better_bing_image_downloader-1.1.2/better_bing_image_downloader/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-20 19:06:07.000000 better_bing_image_downloader-1.1.2/better_bing_image_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8684 2024-04-20 19:06:07.000000 better_bing_image_downloader-1.1.2/better_bing_image_downloader/bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10566 2024-04-20 19:06:07.000000 better_bing_image_downloader-1.1.2/better_bing_image_downloader/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-20 19:06:07.000000 better_bing_image_downloader-1.1.2/better_bing_image_downloader/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-20 19:06:07.000000 better_bing_image_downloader-1.1.2/better_bing_image_downloader/helperdownload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-20 19:06:07.000000 better_bing_image_downloader-1.1.2/better_bing_image_downloader/multidownloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-20 19:06:07.000000 better_bing_image_downloader-1.1.2/better_bing_image_downloader/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:06:11.318972 better_bing_image_downloader-1.1.2/better_bing_image_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-04-20 19:06:11.000000 better_bing_image_downloader-1.1.2/better_bing_image_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-20 19:06:11.000000 better_bing_image_downloader-1.1.2/better_bing_image_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 19:06:11.000000 better_bing_image_downloader-1.1.2/better_bing_image_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-20 19:06:11.000000 better_bing_image_downloader-1.1.2/better_bing_image_downloader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 19:06:11.318972 better_bing_image_downloader-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-20 19:06:07.000000 better_bing_image_downloader-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:06:11.314972 better_bing_image_downloader-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-20 19:06:07.000000 better_bing_image_downloader-1.1.2/tests/test_bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 19:06:07.000000 better_bing_image_downloader-1.1.2/tests/test_download.py
```

### Comparing `better_bing_image_downloader-1.1.1/LICENSE` & `better_bing_image_downloader-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `better_bing_image_downloader-1.1.1/better_bing_image_downloader/bing.py` & `better_bing_image_downloader-1.1.2/better_bing_image_downloader/bing.py`

 * *Files identical despite different names*

### Comparing `better_bing_image_downloader-1.1.1/better_bing_image_downloader/download.py` & `better_bing_image_downloader-1.1.2/better_bing_image_downloader/download.py`

 * *Files identical despite different names*

### Comparing `better_bing_image_downloader-1.1.1/setup.py` & `better_bing_image_downloader-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="better_bing_image_downloader",
-    version="1.1.1",
+    version="1.1.2",
     author="Krishnatejaswi S",
     author_email="shentharkrishnatejaswi@gmail.com",
     description="This package is built on top of bing-image-downloader by gaurav singh",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/KTS-o7/better_bing_image_downloader",
     keywords=['bing', 'images', 'scraping', 'image download', 'bulk image downloader',],
```

### Comparing `better_bing_image_downloader-1.1.1/tests/test_bing.py` & `better_bing_image_downloader-1.1.2/tests/test_bing.py`

 * *Files identical despite different names*

