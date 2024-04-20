# Comparing `tmp/mepost-sdk-0.1.0.tar.gz` & `tmp/mepost-sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mepost-sdk-0.1.0.tar", last modified: Sat Apr 20 16:38:52 2024, max compression
+gzip compressed data, was "mepost-sdk-0.1.1.tar", last modified: Sat Apr 20 16:49:53 2024, max compression
```

## Comparing `mepost-sdk-0.1.0.tar` & `mepost-sdk-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ertugrulkutluer   (501) staff       (20)        0 2024-04-20 16:38:52.813985 mepost-sdk-0.1.0/
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)        0 2024-04-20 15:50:15.000000 mepost-sdk-0.1.0/LICENSE
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)     1281 2024-04-20 16:38:52.813774 mepost-sdk-0.1.0/PKG-INFO
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)      437 2024-04-20 16:37:26.000000 mepost-sdk-0.1.0/README.md
-drwxr-xr-x   0 ertugrulkutluer   (501) staff       (20)        0 2024-04-20 16:38:52.812446 mepost-sdk-0.1.0/mepost/
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)        0 2024-04-20 15:49:17.000000 mepost-sdk-0.1.0/mepost/__init__.py
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)     1710 2024-04-20 15:55:24.000000 mepost-sdk-0.1.0/mepost/client.py
-drwxr-xr-x   0 ertugrulkutluer   (501) staff       (20)        0 2024-04-20 16:38:52.813495 mepost-sdk-0.1.0/mepost_sdk.egg-info/
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)     1281 2024-04-20 16:38:52.000000 mepost-sdk-0.1.0/mepost_sdk.egg-info/PKG-INFO
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)      231 2024-04-20 16:38:52.000000 mepost-sdk-0.1.0/mepost_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)        1 2024-04-20 16:38:52.000000 mepost-sdk-0.1.0/mepost_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)        9 2024-04-20 16:38:52.000000 mepost-sdk-0.1.0/mepost_sdk.egg-info/requires.txt
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)        7 2024-04-20 16:38:52.000000 mepost-sdk-0.1.0/mepost_sdk.egg-info/top_level.txt
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)       38 2024-04-20 16:38:52.814031 mepost-sdk-0.1.0/setup.cfg
--rw-r--r--   0 ertugrulkutluer   (501) staff       (20)     1037 2024-04-20 15:50:49.000000 mepost-sdk-0.1.0/setup.py
+drwxr-xr-x   0 ertugrulkutluer   (501) staff       (20)        0 2024-04-20 16:49:53.614270 mepost-sdk-0.1.1/
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)        0 2024-04-20 15:50:15.000000 mepost-sdk-0.1.1/LICENSE
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)     1281 2024-04-20 16:49:53.614042 mepost-sdk-0.1.1/PKG-INFO
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)      437 2024-04-20 16:37:26.000000 mepost-sdk-0.1.1/README.md
+drwxr-xr-x   0 ertugrulkutluer   (501) staff       (20)        0 2024-04-20 16:49:53.612937 mepost-sdk-0.1.1/mepost/
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)        0 2024-04-20 15:49:17.000000 mepost-sdk-0.1.1/mepost/__init__.py
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)     1703 2024-04-20 16:48:20.000000 mepost-sdk-0.1.1/mepost/client.py
+drwxr-xr-x   0 ertugrulkutluer   (501) staff       (20)        0 2024-04-20 16:49:53.613827 mepost-sdk-0.1.1/mepost_sdk.egg-info/
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)     1281 2024-04-20 16:49:53.000000 mepost-sdk-0.1.1/mepost_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)      231 2024-04-20 16:49:53.000000 mepost-sdk-0.1.1/mepost_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)        1 2024-04-20 16:49:53.000000 mepost-sdk-0.1.1/mepost_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)        9 2024-04-20 16:49:53.000000 mepost-sdk-0.1.1/mepost_sdk.egg-info/requires.txt
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)        7 2024-04-20 16:49:53.000000 mepost-sdk-0.1.1/mepost_sdk.egg-info/top_level.txt
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)       38 2024-04-20 16:49:53.614317 mepost-sdk-0.1.1/setup.cfg
+-rw-r--r--   0 ertugrulkutluer   (501) staff       (20)     1037 2024-04-20 16:48:48.000000 mepost-sdk-0.1.1/setup.py
```

### Comparing `mepost-sdk-0.1.0/PKG-INFO` & `mepost-sdk-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mepost-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python SDK for interacting with the Mepost API.
 Home-page: https://github.com/yourusername/mepost-sdk
 Author: https://github.com/mepost-io
 Author-email: info@mepost.io
 License: MIT
 Keywords: mepost,email,sdk,api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mepost-sdk-0.1.0/mepost/client.py` & `mepost-sdk-0.1.1/mepost/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import requests
 
 class MepostClient:
     def __init__(self, api_key):
         self.api_key = api_key
         self.base_url = 'https://api.mepost.io/v1'
         self.headers = {
-            'Authorization': f'Bearer {self.api_key}',
+            'Authorization': f'{self.api_key}',
             'Accept': 'application/json'
         }
 
     def send_email(self, email_data):
         """Send an email using the Mepost API."""
         url = f"{self.base_url}/messages/send"
         response = requests.post(url, json=email_data, headers=self.headers)
```

### Comparing `mepost-sdk-0.1.0/mepost_sdk.egg-info/PKG-INFO` & `mepost-sdk-0.1.1/mepost_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mepost-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python SDK for interacting with the Mepost API.
 Home-page: https://github.com/yourusername/mepost-sdk
 Author: https://github.com/mepost-io
 Author-email: info@mepost.io
 License: MIT
 Keywords: mepost,email,sdk,api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mepost-sdk-0.1.0/setup.py` & `mepost-sdk-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mepost-sdk',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     description='A Python SDK for interacting with the Mepost API.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='https://github.com/mepost-io',
     author_email='info@mepost.io',
     license='MIT',
```

