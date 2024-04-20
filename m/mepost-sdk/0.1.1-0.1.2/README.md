# Comparing `tmp/mepost-sdk-0.1.1.tar.gz` & `tmp/mepost-sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mepost-sdk-0.1.1.tar", last modified: Sat Apr 20 16:49:53 2024, max compression
+gzip compressed data, was "mepost-sdk-0.1.2.tar", last modified: Sat Apr 20 16:54:07 2024, max compression
```

## Comparing `mepost-sdk-0.1.1.tar` & `mepost-sdk-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ertugrulkutluer   (501) staff       (20)        0 2024-04-20 16:49:53.614270 mepost-sdk-0.1.1/
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)        0 2024-04-20 15:50:15.000000 mepost-sdk-0.1.1/LICENSE
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)     1281 2024-04-20 16:49:53.614042 mepost-sdk-0.1.1/PKG-INFO
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)      437 2024-04-20 16:37:26.000000 mepost-sdk-0.1.1/README.md
-drwxr-xr-x   0 ertugrulkutluer   (501) staff       (20)        0 2024-04-20 16:49:53.612937 mepost-sdk-0.1.1/mepost/
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)        0 2024-04-20 15:49:17.000000 mepost-sdk-0.1.1/mepost/__init__.py
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)     1703 2024-04-20 16:48:20.000000 mepost-sdk-0.1.1/mepost/client.py
-drwxr-xr-x   0 ertugrulkutluer   (501) staff       (20)        0 2024-04-20 16:49:53.613827 mepost-sdk-0.1.1/mepost_sdk.egg-info/
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)     1281 2024-04-20 16:49:53.000000 mepost-sdk-0.1.1/mepost_sdk.egg-info/PKG-INFO
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)      231 2024-04-20 16:49:53.000000 mepost-sdk-0.1.1/mepost_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)        1 2024-04-20 16:49:53.000000 mepost-sdk-0.1.1/mepost_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)        9 2024-04-20 16:49:53.000000 mepost-sdk-0.1.1/mepost_sdk.egg-info/requires.txt
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)        7 2024-04-20 16:49:53.000000 mepost-sdk-0.1.1/mepost_sdk.egg-info/top_level.txt
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)       38 2024-04-20 16:49:53.614317 mepost-sdk-0.1.1/setup.cfg
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)     1037 2024-04-20 16:48:48.000000 mepost-sdk-0.1.1/setup.py
+drwxr-xr-x   0 ertugrulkutluer   (501) staff       (20)        0 2024-04-20 16:54:07.810652 mepost-sdk-0.1.2/
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)        0 2024-04-20 15:50:15.000000 mepost-sdk-0.1.2/LICENSE
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)     1256 2024-04-20 16:54:07.810390 mepost-sdk-0.1.2/PKG-INFO
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)      437 2024-04-20 16:37:26.000000 mepost-sdk-0.1.2/README.md
+drwxr-xr-x   0 ertugrulkutluer   (501) staff       (20)        0 2024-04-20 16:54:07.809078 mepost-sdk-0.1.2/mepost/
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)        0 2024-04-20 15:49:17.000000 mepost-sdk-0.1.2/mepost/__init__.py
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)     1703 2024-04-20 16:48:20.000000 mepost-sdk-0.1.2/mepost/client.py
+drwxr-xr-x   0 ertugrulkutluer   (501) staff       (20)        0 2024-04-20 16:54:07.810137 mepost-sdk-0.1.2/mepost_sdk.egg-info/
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)     1256 2024-04-20 16:54:07.000000 mepost-sdk-0.1.2/mepost_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)      231 2024-04-20 16:54:07.000000 mepost-sdk-0.1.2/mepost_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)        1 2024-04-20 16:54:07.000000 mepost-sdk-0.1.2/mepost_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)        9 2024-04-20 16:54:07.000000 mepost-sdk-0.1.2/mepost_sdk.egg-info/requires.txt
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)        7 2024-04-20 16:54:07.000000 mepost-sdk-0.1.2/mepost_sdk.egg-info/top_level.txt
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)       38 2024-04-20 16:54:07.810702 mepost-sdk-0.1.2/setup.cfg
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)     1012 2024-04-20 16:53:59.000000 mepost-sdk-0.1.2/setup.py
```

### Comparing `mepost-sdk-0.1.1/PKG-INFO` & `mepost-sdk-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mepost-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python SDK for interacting with the Mepost API.
-Home-page: https://github.com/yourusername/mepost-sdk
-Author: https://github.com/mepost-io
+Home-page: https://github.com/mepost-io/mepost-sdk
+Author: mepost
 Author-email: info@mepost.io
 License: MIT
 Keywords: mepost,email,sdk,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mepost-sdk-0.1.1/mepost/client.py` & `mepost-sdk-0.1.2/mepost/client.py`

 * *Files identical despite different names*

### Comparing `mepost-sdk-0.1.1/mepost_sdk.egg-info/PKG-INFO` & `mepost-sdk-0.1.2/mepost_sdk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mepost-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python SDK for interacting with the Mepost API.
-Home-page: https://github.com/yourusername/mepost-sdk
-Author: https://github.com/mepost-io
+Home-page: https://github.com/mepost-io/mepost-sdk
+Author: mepost
 Author-email: info@mepost.io
 License: MIT
 Keywords: mepost,email,sdk,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mepost-sdk-0.1.1/setup.py` & `mepost-sdk-0.1.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mepost-sdk',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     description='A Python SDK for interacting with the Mepost API.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    author='https://github.com/mepost-io',
+    author='mepost',
     author_email='info@mepost.io',
     license='MIT',
     install_requires=[
         'requests'
     ],
-    url='https://github.com/yourusername/mepost-sdk',
+    url='https://github.com/mepost-io/mepost-sdk',
     keywords='mepost, email, sdk, api',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

