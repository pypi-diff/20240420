# Comparing `tmp/rent_counter-0.6.0.tar.gz` & `tmp/rent_counter-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rent_counter-0.6.0.tar", last modified: Fri Apr 19 23:21:37 2024, max compression
+gzip compressed data, was "rent_counter-0.7.0.tar", last modified: Fri Apr 19 23:50:46 2024, max compression
```

## Comparing `rent_counter-0.6.0.tar` & `rent_counter-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 23:21:37.326405 rent_counter-0.6.0/
--rw-rw-rw-   0        0        0     2001 2024-04-19 23:21:37.322408 rent_counter-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     1465 2024-04-19 07:51:08.000000 rent_counter-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 23:21:37.290859 rent_counter-0.6.0/countf/
--rw-rw-rw-   0        0        0        2 2024-04-19 14:08:38.000000 rent_counter-0.6.0/countf/__init__.py
--rw-rw-rw-   0        0        0      451 2024-04-19 07:51:08.000000 rent_counter-0.6.0/countf/countdown.py
-drwxrwxrwx   0        0        0        0 2024-04-19 23:21:37.319019 rent_counter-0.6.0/rent_counter.egg-info/
--rw-rw-rw-   0        0        0     2001 2024-04-19 23:21:37.000000 rent_counter-0.6.0/rent_counter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-04-19 23:21:37.000000 rent_counter-0.6.0/rent_counter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 23:21:37.000000 rent_counter-0.6.0/rent_counter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-19 23:21:37.000000 rent_counter-0.6.0/rent_counter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 23:21:37.327405 rent_counter-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0      777 2024-04-19 23:20:19.000000 rent_counter-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 23:21:37.314020 rent_counter-0.6.0/tests/
--rw-rw-rw-   0        0        0     1126 2024-04-19 22:54:29.000000 rent_counter-0.6.0/tests/test_countdown.py
+drwxrwxrwx   0        0        0        0 2024-04-19 23:50:46.398552 rent_counter-0.7.0/
+-rw-rw-rw-   0        0        0     2001 2024-04-19 23:50:46.395554 rent_counter-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1465 2024-04-19 07:51:08.000000 rent_counter-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 23:50:46.341721 rent_counter-0.7.0/countf/
+-rw-rw-rw-   0        0        0        2 2024-04-19 14:08:38.000000 rent_counter-0.7.0/countf/__init__.py
+-rw-rw-rw-   0        0        0      451 2024-04-19 07:51:08.000000 rent_counter-0.7.0/countf/countdown.py
+drwxrwxrwx   0        0        0        0 2024-04-19 23:50:46.392555 rent_counter-0.7.0/rent_counter.egg-info/
+-rw-rw-rw-   0        0        0     2001 2024-04-19 23:50:46.000000 rent_counter-0.7.0/rent_counter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-04-19 23:50:46.000000 rent_counter-0.7.0/rent_counter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 23:50:46.000000 rent_counter-0.7.0/rent_counter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-19 23:50:46.000000 rent_counter-0.7.0/rent_counter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 23:50:46.398552 rent_counter-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      807 2024-04-19 23:50:07.000000 rent_counter-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 23:50:46.365886 rent_counter-0.7.0/tests/
+-rw-rw-rw-   0        0        0     1126 2024-04-19 22:54:29.000000 rent_counter-0.7.0/tests/test_countdown.py
```

### Comparing `rent_counter-0.6.0/PKG-INFO` & `rent_counter-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rent_counter
-Version: 0.6.0
+Version: 0.7.0
 Summary: A Python library for managing rent expiration countdowns
 Home-page: https://github.com/Erickadikah/count
 Author: Erick Adikah
 Author-email: your.email@example.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rent_counter-0.6.0/README.md` & `rent_counter-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `rent_counter-0.6.0/rent_counter.egg-info/PKG-INFO` & `rent_counter-0.7.0/rent_counter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rent_counter
-Version: 0.6.0
+Version: 0.7.0
 Summary: A Python library for managing rent expiration countdowns
 Home-page: https://github.com/Erickadikah/count
 Author: Erick Adikah
 Author-email: your.email@example.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rent_counter-0.6.0/setup.py` & `rent_counter-0.7.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import setuptools
 from setuptools import setup, find_packages
 
 setup(
     name='rent_counter',
-    version='0.6.0',
-    packages=find_packages(),
+    version='0.7.0',
+    packages=setuptools.find_packages(),
     include_package_data=True,
     description='A Python library for managing rent expiration countdowns',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Erick Adikah',
     author_email='your.email@example.com',
     license='MIT',
```

### Comparing `rent_counter-0.6.0/tests/test_countdown.py` & `rent_counter-0.7.0/tests/test_countdown.py`

 * *Files identical despite different names*

