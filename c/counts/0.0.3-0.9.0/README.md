# Comparing `tmp/counts-0.0.3.tar.gz` & `tmp/counts-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "counts-0.0.3.tar", last modified: Sat Apr 20 01:19:08 2024, max compression
+gzip compressed data, was "counts-0.9.0.tar", last modified: Sat Apr 20 00:24:15 2024, max compression
```

## Comparing `counts-0.0.3.tar` & `counts-0.9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 01:19:08.645135 counts-0.0.3/
--rw-rw-rw-   0        0        0     1995 2024-04-20 01:19:08.643131 counts-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1465 2024-04-19 07:51:08.000000 counts-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 01:19:08.587901 counts-0.0.3/counts/
--rw-rw-rw-   0        0        0        2 2024-04-19 14:08:38.000000 counts-0.0.3/counts/__init__.py
--rw-rw-rw-   0        0        0      491 2024-04-20 01:15:42.000000 counts-0.0.3/counts/countdown.py
-drwxrwxrwx   0        0        0        0 2024-04-20 01:19:08.640147 counts-0.0.3/counts.egg-info/
--rw-rw-rw-   0        0        0     1995 2024-04-20 01:19:08.000000 counts-0.0.3/counts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2024-04-20 01:19:08.000000 counts-0.0.3/counts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 01:19:08.000000 counts-0.0.3/counts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-20 01:19:08.000000 counts-0.0.3/counts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 01:19:08.649133 counts-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      790 2024-04-20 01:18:24.000000 counts-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 00:24:15.580448 counts-0.9.0/
+-rw-rw-rw-   0        0        0     1995 2024-04-20 00:24:15.578431 counts-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1465 2024-04-19 07:51:08.000000 counts-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 00:24:15.550969 counts-0.9.0/countf/
+-rw-rw-rw-   0        0        0        2 2024-04-19 14:08:38.000000 counts-0.9.0/countf/__init__.py
+-rw-rw-rw-   0        0        0      451 2024-04-19 07:51:08.000000 counts-0.9.0/countf/countdown.py
+drwxrwxrwx   0        0        0        0 2024-04-20 00:24:15.574419 counts-0.9.0/counts.egg-info/
+-rw-rw-rw-   0        0        0     1995 2024-04-20 00:24:15.000000 counts-0.9.0/counts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2024-04-20 00:24:15.000000 counts-0.9.0/counts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 00:24:15.000000 counts-0.9.0/counts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-20 00:24:15.000000 counts-0.9.0/counts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 00:24:15.580448 counts-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      785 2024-04-20 00:22:35.000000 counts-0.9.0/setup.py
```

### Comparing `counts-0.0.3/PKG-INFO` & `counts-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: counts
-Version: 0.0.3
+Version: 0.9.0
 Summary: A Python library for managing rent expiration countdowns
 Home-page: https://github.com/Erickadikah/count
 Author: Erick Adikah
 Author-email: your.email@example.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `counts-0.0.3/README.md` & `counts-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `counts-0.0.3/counts.egg-info/PKG-INFO` & `counts-0.9.0/counts.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: counts
-Version: 0.0.3
+Version: 0.9.0
 Summary: A Python library for managing rent expiration countdowns
 Home-page: https://github.com/Erickadikah/count
 Author: Erick Adikah
 Author-email: your.email@example.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `counts-0.0.3/setup.py` & `counts-0.9.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 from setuptools import setup, find_packages
 
 setup(
     name='counts',
-    version='0.0.3',
-    packages=find_packages(),
+    version='0.9.0',
+    packages=['countf'],
     include_package_data=True,
     description='A Python library for managing rent expiration countdowns',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Erick Adikah',
     author_email='your.email@example.com',
     license='MIT',
```

