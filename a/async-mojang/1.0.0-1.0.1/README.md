# Comparing `tmp/async_mojang-1.0.0.tar.gz` & `tmp/async_mojang-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_mojang-1.0.0.tar", last modified: Sat Apr 20 04:35:46 2024, max compression
+gzip compressed data, was "async_mojang-1.0.1.tar", last modified: Sat Apr 20 04:37:58 2024, max compression
```

## Comparing `async_mojang-1.0.0.tar` & `async_mojang-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jbeal      (501) staff       (20)        0 2024-04-20 04:35:46.148357 async_mojang-1.0.0/
--rw-rw-r--   0 jbeal      (501) staff       (20)     1071 2024-04-20 04:12:18.000000 async_mojang-1.0.0/LICENSE
--rw-r--r--   0 jbeal      (501) staff       (20)     1735 2024-04-20 04:35:46.148169 async_mojang-1.0.0/PKG-INFO
--rw-rw-r--   0 jbeal      (501) staff       (20)      664 2024-04-20 04:22:21.000000 async_mojang-1.0.0/README.md
-drwxr-xr-x   0 jbeal      (501) staff       (20)        0 2024-04-20 04:35:46.147173 async_mojang-1.0.0/async_mojang/
--rw-rw-r--   0 jbeal      (501) staff       (20)      263 2024-04-20 04:32:27.000000 async_mojang-1.0.0/async_mojang/__init__.py
--rw-rw-r--   0 jbeal      (501) staff       (20)     2815 2024-04-20 04:32:31.000000 async_mojang-1.0.0/async_mojang/_http_client.py
--rw-rw-r--   0 jbeal      (501) staff       (20)      737 2024-04-20 04:32:48.000000 async_mojang-1.0.0/async_mojang/_types.py
--rw-rw-r--   0 jbeal      (501) staff       (20)      398 2024-04-20 04:32:51.000000 async_mojang-1.0.0/async_mojang/_utils.py
--rw-rw-r--   0 jbeal      (501) staff       (20)     3347 2024-04-20 04:34:26.000000 async_mojang-1.0.0/async_mojang/api.py
--rw-rw-r--   0 jbeal      (501) staff       (20)     2035 2024-04-20 04:34:18.000000 async_mojang-1.0.0/async_mojang/errors.py
-drwxr-xr-x   0 jbeal      (501) staff       (20)        0 2024-04-20 04:35:46.147972 async_mojang-1.0.0/async_mojang.egg-info/
--rw-r--r--   0 jbeal      (501) staff       (20)     1735 2024-04-20 04:35:46.000000 async_mojang-1.0.0/async_mojang.egg-info/PKG-INFO
--rw-r--r--   0 jbeal      (501) staff       (20)      348 2024-04-20 04:35:46.000000 async_mojang-1.0.0/async_mojang.egg-info/SOURCES.txt
--rw-r--r--   0 jbeal      (501) staff       (20)        1 2024-04-20 04:35:46.000000 async_mojang-1.0.0/async_mojang.egg-info/dependency_links.txt
--rw-r--r--   0 jbeal      (501) staff       (20)        8 2024-04-20 04:35:46.000000 async_mojang-1.0.0/async_mojang.egg-info/requires.txt
--rw-r--r--   0 jbeal      (501) staff       (20)       13 2024-04-20 04:35:46.000000 async_mojang-1.0.0/async_mojang.egg-info/top_level.txt
--rw-r--r--   0 jbeal      (501) staff       (20)       38 2024-04-20 04:35:46.148407 async_mojang-1.0.0/setup.cfg
--rw-rw-r--   0 jbeal      (501) staff       (20)     1269 2024-04-20 04:31:19.000000 async_mojang-1.0.0/setup.py
+drwxr-xr-x   0 jbeal      (501) staff       (20)        0 2024-04-20 04:37:58.127135 async_mojang-1.0.1/
+-rw-rw-r--   0 jbeal      (501) staff       (20)     1071 2024-04-20 04:12:18.000000 async_mojang-1.0.1/LICENSE
+-rw-r--r--   0 jbeal      (501) staff       (20)     2573 2024-04-20 04:37:58.126879 async_mojang-1.0.1/PKG-INFO
+-rw-rw-r--   0 jbeal      (501) staff       (20)     1502 2024-04-20 04:37:46.000000 async_mojang-1.0.1/README.md
+drwxr-xr-x   0 jbeal      (501) staff       (20)        0 2024-04-20 04:37:58.125869 async_mojang-1.0.1/async_mojang/
+-rw-rw-r--   0 jbeal      (501) staff       (20)      263 2024-04-20 04:32:27.000000 async_mojang-1.0.1/async_mojang/__init__.py
+-rw-rw-r--   0 jbeal      (501) staff       (20)     2815 2024-04-20 04:32:31.000000 async_mojang-1.0.1/async_mojang/_http_client.py
+-rw-rw-r--   0 jbeal      (501) staff       (20)      737 2024-04-20 04:32:48.000000 async_mojang-1.0.1/async_mojang/_types.py
+-rw-rw-r--   0 jbeal      (501) staff       (20)      398 2024-04-20 04:32:51.000000 async_mojang-1.0.1/async_mojang/_utils.py
+-rw-rw-r--   0 jbeal      (501) staff       (20)     3347 2024-04-20 04:34:26.000000 async_mojang-1.0.1/async_mojang/api.py
+-rw-rw-r--   0 jbeal      (501) staff       (20)     2035 2024-04-20 04:34:18.000000 async_mojang-1.0.1/async_mojang/errors.py
+drwxr-xr-x   0 jbeal      (501) staff       (20)        0 2024-04-20 04:37:58.126672 async_mojang-1.0.1/async_mojang.egg-info/
+-rw-r--r--   0 jbeal      (501) staff       (20)     2573 2024-04-20 04:37:58.000000 async_mojang-1.0.1/async_mojang.egg-info/PKG-INFO
+-rw-r--r--   0 jbeal      (501) staff       (20)      348 2024-04-20 04:37:58.000000 async_mojang-1.0.1/async_mojang.egg-info/SOURCES.txt
+-rw-r--r--   0 jbeal      (501) staff       (20)        1 2024-04-20 04:37:58.000000 async_mojang-1.0.1/async_mojang.egg-info/dependency_links.txt
+-rw-r--r--   0 jbeal      (501) staff       (20)        8 2024-04-20 04:37:58.000000 async_mojang-1.0.1/async_mojang.egg-info/requires.txt
+-rw-r--r--   0 jbeal      (501) staff       (20)       13 2024-04-20 04:37:58.000000 async_mojang-1.0.1/async_mojang.egg-info/top_level.txt
+-rw-r--r--   0 jbeal      (501) staff       (20)       38 2024-04-20 04:37:58.127187 async_mojang-1.0.1/setup.cfg
+-rw-rw-r--   0 jbeal      (501) staff       (20)     1269 2024-04-20 04:37:27.000000 async_mojang-1.0.1/setup.py
```

### Comparing `async_mojang-1.0.0/LICENSE` & `async_mojang-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `async_mojang-1.0.0/async_mojang/_http_client.py` & `async_mojang-1.0.1/async_mojang/_http_client.py`

 * *Files identical despite different names*

### Comparing `async_mojang-1.0.0/async_mojang/_types.py` & `async_mojang-1.0.1/async_mojang/_types.py`

 * *Files identical despite different names*

### Comparing `async_mojang-1.0.0/async_mojang/api.py` & `async_mojang-1.0.1/async_mojang/api.py`

 * *Files identical despite different names*

### Comparing `async_mojang-1.0.0/async_mojang/errors.py` & `async_mojang-1.0.1/async_mojang/errors.py`

 * *Files identical despite different names*

### Comparing `async_mojang-1.0.0/setup.py` & `async_mojang-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="async-mojang",
-    version="1.0.0",
+    version="1.0.1",
     author="FroostySnoowman",
     description="An async Python wrapper for the Mojang API.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/FroostySnoowman/Async-Mojang",
     packages=find_packages(),
     classifiers=[
```

