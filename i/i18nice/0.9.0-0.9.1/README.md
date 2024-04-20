# Comparing `tmp/i18nice-0.9.0.tar.gz` & `tmp/i18nice-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i18nice-0.9.0.tar", last modified: Tue Aug 15 16:35:46 2023, max compression
+gzip compressed data, was "i18nice-0.9.1.tar", last modified: Tue Aug 15 16:50:59 2023, max compression
```

## Comparing `i18nice-0.9.0.tar` & `i18nice-0.9.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-15 16:35:46.920683 i18nice-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (122)     2040 2023-08-15 16:35:38.000000 i18nice-0.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-08-15 16:35:38.000000 i18nice-0.9.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-08-15 16:35:38.000000 i18nice-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-08-15 16:35:38.000000 i18nice-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8783 2023-08-15 16:35:46.920683 i18nice-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7908 2023-08-15 16:35:38.000000 i18nice-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-15 16:35:46.916683 i18nice-0.9.0/i18n/
--rw-r--r--   0 runner    (1001) docker     (122)      920 2023-08-15 16:35:38.000000 i18nice-0.9.0/i18n/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-08-15 16:35:38.000000 i18nice-0.9.0/i18n/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     1183 2023-08-15 16:35:38.000000 i18nice-0.9.0/i18n/custom_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)      599 2023-08-15 16:35:38.000000 i18nice-0.9.0/i18n/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     8292 2023-08-15 16:35:38.000000 i18nice-0.9.0/i18n/formatters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-15 16:35:46.920683 i18nice-0.9.0/i18n/loaders/
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-08-15 16:35:38.000000 i18nice-0.9.0/i18n/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      418 2023-08-15 16:35:38.000000 i18nice-0.9.0/i18n/loaders/json_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     3442 2023-08-15 16:35:38.000000 i18nice-0.9.0/i18n/loaders/loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-08-15 16:35:38.000000 i18nice-0.9.0/i18n/loaders/python_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)      675 2023-08-15 16:35:38.000000 i18nice-0.9.0/i18n/loaders/yaml_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     8486 2023-08-15 16:35:38.000000 i18nice-0.9.0/i18n/resource_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-08-15 16:35:38.000000 i18nice-0.9.0/i18n/translations.py
--rw-r--r--   0 runner    (1001) docker     (122)     4238 2023-08-15 16:35:38.000000 i18nice-0.9.0/i18n/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-15 16:35:46.920683 i18nice-0.9.0/i18nice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8783 2023-08-15 16:35:46.000000 i18nice-0.9.0/i18nice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      536 2023-08-15 16:35:46.000000 i18nice-0.9.0/i18nice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-15 16:35:46.000000 i18nice-0.9.0/i18nice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-08-15 16:35:46.000000 i18nice-0.9.0/i18nice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-08-15 16:35:46.000000 i18nice-0.9.0/i18nice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-15 16:35:46.000000 i18nice-0.9.0/i18nice.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-15 16:35:46.920683 i18nice-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1366 2023-08-15 16:35:38.000000 i18nice-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-15 16:50:59.847791 i18nice-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     2040 2023-08-15 16:50:51.000000 i18nice-0.9.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-08-15 16:50:51.000000 i18nice-0.9.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-08-15 16:50:51.000000 i18nice-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-08-15 16:50:51.000000 i18nice-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8807 2023-08-15 16:50:59.847791 i18nice-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7908 2023-08-15 16:50:51.000000 i18nice-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-15 16:50:59.843791 i18nice-0.9.1/i18n/
+-rw-r--r--   0 runner    (1001) docker     (122)      920 2023-08-15 16:50:51.000000 i18nice-0.9.1/i18n/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-08-15 16:50:51.000000 i18nice-0.9.1/i18n/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1183 2023-08-15 16:50:51.000000 i18nice-0.9.1/i18n/custom_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      599 2023-08-15 16:50:51.000000 i18nice-0.9.1/i18n/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8292 2023-08-15 16:50:51.000000 i18nice-0.9.1/i18n/formatters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-15 16:50:59.843791 i18nice-0.9.1/i18n/loaders/
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-08-15 16:50:51.000000 i18nice-0.9.1/i18n/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      418 2023-08-15 16:50:51.000000 i18nice-0.9.1/i18n/loaders/json_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3442 2023-08-15 16:50:51.000000 i18nice-0.9.1/i18n/loaders/loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-08-15 16:50:51.000000 i18nice-0.9.1/i18n/loaders/python_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2023-08-15 16:50:51.000000 i18nice-0.9.1/i18n/loaders/yaml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8486 2023-08-15 16:50:51.000000 i18nice-0.9.1/i18n/resource_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-08-15 16:50:51.000000 i18nice-0.9.1/i18n/translations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4238 2023-08-15 16:50:51.000000 i18nice-0.9.1/i18n/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-15 16:50:59.847791 i18nice-0.9.1/i18nice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8807 2023-08-15 16:50:59.000000 i18nice-0.9.1/i18nice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-08-15 16:50:59.000000 i18nice-0.9.1/i18nice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-15 16:50:59.000000 i18nice-0.9.1/i18nice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-08-15 16:50:59.000000 i18nice-0.9.1/i18nice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-08-15 16:50:59.000000 i18nice-0.9.1/i18nice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-15 16:50:59.000000 i18nice-0.9.1/i18nice.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-15 16:50:59.847791 i18nice-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1319 2023-08-15 16:50:51.000000 i18nice-0.9.1/setup.py
```

### Comparing `i18nice-0.9.0/CHANGELOG.md` & `i18nice-0.9.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `i18nice-0.9.0/CONTRIBUTING.md` & `i18nice-0.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `i18nice-0.9.0/LICENSE` & `i18nice-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `i18nice-0.9.0/PKG-INFO` & `i18nice-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: i18nice
-Version: 0.9.0
+Version: 0.9.1
 Summary: Translation library for Python
 Home-page: https://github.com/Krutyi-4el/i18nice
-Download-URL: https://github.com/Krutyi-4el/archive/master.zip
+Download-URL: https://github.com/Krutyi-4el/i18nice/archive/master.zip
 Author: Daniel Perez
 Author-email: tuvistavie@gmail.com
 Maintainer: Krutyi 4el
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
@@ -21,17 +21,17 @@
 License-File: LICENSE
 
 # i18nice [![tests](https://github.com/Krutyi-4el/i18nice/actions/workflows/ci.yml/badge.svg)](https://github.com/Krutyi-4el/i18nice/actions/workflows/ci.yml) [![Coverage Status](https://coveralls.io/repos/github/Krutyi-4el/i18nice/badge.svg)](https://coveralls.io/github/Krutyi-4el/i18nice)
 
 
 This library provides i18n functionality for Python 3 out of the box. The usage is mostly based on Rails i18n library.
 
-[CHANGELOG](https://github.com/Krutyi-4el/blob/master/CHANGELOG.md)
+[CHANGELOG](https://github.com/Krutyi-4el/i18nice/blob/master/CHANGELOG.md)
 
-[CONTRIBUTING](https://github.com/Krutyi-4el/blob/master/CONTRIBUTING.md)
+[CONTRIBUTING](https://github.com/Krutyi-4el/i18nice/blob/master/CONTRIBUTING.md)
 
 ## Installation
 
 Just run
 
     pip install i18nice
```

### Comparing `i18nice-0.9.0/README.md` & `i18nice-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `i18nice-0.9.0/i18n/__init__.py` & `i18nice-0.9.1/i18n/__init__.py`

 * *Files identical despite different names*

### Comparing `i18nice-0.9.0/i18n/config.py` & `i18nice-0.9.1/i18n/config.py`

 * *Files identical despite different names*

### Comparing `i18nice-0.9.0/i18n/custom_functions.py` & `i18nice-0.9.1/i18n/custom_functions.py`

 * *Files identical despite different names*

### Comparing `i18nice-0.9.0/i18n/errors.py` & `i18nice-0.9.1/i18n/errors.py`

 * *Files identical despite different names*

### Comparing `i18nice-0.9.0/i18n/formatters.py` & `i18nice-0.9.1/i18n/formatters.py`

 * *Files identical despite different names*

### Comparing `i18nice-0.9.0/i18n/loaders/loader.py` & `i18nice-0.9.1/i18n/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `i18nice-0.9.0/i18n/loaders/python_loader.py` & `i18nice-0.9.1/i18n/loaders/python_loader.py`

 * *Files identical despite different names*

### Comparing `i18nice-0.9.0/i18n/loaders/yaml_loader.py` & `i18nice-0.9.1/i18n/loaders/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `i18nice-0.9.0/i18n/resource_loader.py` & `i18nice-0.9.1/i18n/resource_loader.py`

 * *Files identical despite different names*

### Comparing `i18nice-0.9.0/i18n/translations.py` & `i18nice-0.9.1/i18n/translations.py`

 * *Files identical despite different names*

### Comparing `i18nice-0.9.0/i18n/translator.py` & `i18nice-0.9.1/i18n/translator.py`

 * *Files identical despite different names*

### Comparing `i18nice-0.9.0/i18nice.egg-info/PKG-INFO` & `i18nice-0.9.1/i18nice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: i18nice
-Version: 0.9.0
+Version: 0.9.1
 Summary: Translation library for Python
 Home-page: https://github.com/Krutyi-4el/i18nice
-Download-URL: https://github.com/Krutyi-4el/archive/master.zip
+Download-URL: https://github.com/Krutyi-4el/i18nice/archive/master.zip
 Author: Daniel Perez
 Author-email: tuvistavie@gmail.com
 Maintainer: Krutyi 4el
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
@@ -21,17 +21,17 @@
 License-File: LICENSE
 
 # i18nice [![tests](https://github.com/Krutyi-4el/i18nice/actions/workflows/ci.yml/badge.svg)](https://github.com/Krutyi-4el/i18nice/actions/workflows/ci.yml) [![Coverage Status](https://coveralls.io/repos/github/Krutyi-4el/i18nice/badge.svg)](https://coveralls.io/github/Krutyi-4el/i18nice)
 
 
 This library provides i18n functionality for Python 3 out of the box. The usage is mostly based on Rails i18n library.
 
-[CHANGELOG](https://github.com/Krutyi-4el/blob/master/CHANGELOG.md)
+[CHANGELOG](https://github.com/Krutyi-4el/i18nice/blob/master/CHANGELOG.md)
 
-[CONTRIBUTING](https://github.com/Krutyi-4el/blob/master/CONTRIBUTING.md)
+[CONTRIBUTING](https://github.com/Krutyi-4el/i18nice/blob/master/CONTRIBUTING.md)
 
 ## Installation
 
 Just run
 
     pip install i18nice
```

### Comparing `i18nice-0.9.0/i18nice.egg-info/SOURCES.txt` & `i18nice-0.9.1/i18nice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `i18nice-0.9.0/setup.py` & `i18nice-0.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import re
-from urllib.parse import urljoin
 
 from setuptools import setup
 
 
 GITHUB_URL = "https://github.com/Krutyi-4el/i18nice"
 long_description = open("README.md").read()
 # links on PyPI should have absolute URLs
 long_description = re.sub(
     r"(\[[^\]]+\]\()((?!https?:)[^\)]+)(\))",
-    lambda m: m.group(1) + urljoin(GITHUB_URL, "blob/master/" + m.group(2)) + m.group(3),
+    lambda m: m.group(1) + GITHUB_URL + "/blob/master/" + m.group(2) + m.group(3),
     long_description,
 )
 
 setup(
     name='i18nice',
-    version='0.9.0',
+    version='0.9.1',
     description='Translation library for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Daniel Perez',
     author_email='tuvistavie@gmail.com',
     maintainer="Krutyi 4el",
     url=GITHUB_URL,
-    download_url=urljoin(GITHUB_URL, "archive/master.zip"),
+    download_url=GITHUB_URL + "/archive/master.zip",
     license='MIT',
     packages=['i18n', 'i18n.loaders'],
     zip_safe=True,
     test_suite='i18n.tests',
     extras_require={
         'YAML': ["pyyaml>=3.10"],
     },
```

