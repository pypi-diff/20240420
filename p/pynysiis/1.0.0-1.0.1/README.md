# Comparing `tmp/pynysiis-1.0.0.tar.gz` & `tmp/pynysiis-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynysiis-1.0.0.tar", last modified: Sat Apr 20 20:19:44 2024, max compression
+gzip compressed data, was "pynysiis-1.0.1.tar", last modified: Sat Apr 20 20:24:17 2024, max compression
```

## Comparing `pynysiis-1.0.0.tar` & `pynysiis-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2024-04-20 20:19:44.110936 pynysiis-1.0.0/
--rw-r--r--   0 finn       (501) staff       (20)     1099 2024-04-20 18:17:07.000000 pynysiis-1.0.0/LICENSE
--rw-r--r--   0 finn       (501) staff       (20)     3478 2024-04-20 20:19:44.111093 pynysiis-1.0.0/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     1579 2024-04-20 19:22:22.000000 pynysiis-1.0.0/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2024-04-20 20:19:44.108422 pynysiis-1.0.0/nysiis/
--rw-r--r--   0 finn       (501) staff       (20)       68 2024-04-20 19:18:47.000000 pynysiis-1.0.0/nysiis/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     8805 2024-04-20 19:18:55.000000 pynysiis-1.0.0/nysiis/nysiis.py
--rw-r--r--   0 finn       (501) staff       (20)    34581 2024-04-20 18:21:02.000000 pynysiis-1.0.0/nysiis/six.py
--rw-r--r--   0 finn       (501) staff       (20)       18 2024-04-20 19:30:50.000000 pynysiis-1.0.0/nysiis/version.py
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2024-04-20 20:19:44.110626 pynysiis-1.0.0/pynysiis.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     3478 2024-04-20 20:19:43.000000 pynysiis-1.0.0/pynysiis.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      294 2024-04-20 20:19:44.000000 pynysiis-1.0.0/pynysiis.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2024-04-20 20:19:43.000000 pynysiis-1.0.0/pynysiis.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2024-04-20 20:19:34.000000 pynysiis-1.0.0/pynysiis.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)        9 2024-04-20 20:19:43.000000 pynysiis-1.0.0/pynysiis.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)        7 2024-04-20 20:19:43.000000 pynysiis-1.0.0/pynysiis.egg-info/top_level.txt
--rw-r--r--   0 finn       (501) staff       (20)       38 2024-04-20 20:19:44.111576 pynysiis-1.0.0/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2147 2024-04-20 20:18:31.000000 pynysiis-1.0.0/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2024-04-20 20:24:17.157450 pynysiis-1.0.1/
+-rw-r--r--   0 finn       (501) staff       (20)     1099 2024-04-20 18:17:07.000000 pynysiis-1.0.1/LICENSE
+-rw-r--r--   0 finn       (501) staff       (20)     3488 2024-04-20 20:24:17.157620 pynysiis-1.0.1/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     1585 2024-04-20 20:22:51.000000 pynysiis-1.0.1/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2024-04-20 20:24:17.155102 pynysiis-1.0.1/nysiis/
+-rw-r--r--   0 finn       (501) staff       (20)       68 2024-04-20 19:18:47.000000 pynysiis-1.0.1/nysiis/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     8805 2024-04-20 19:18:55.000000 pynysiis-1.0.1/nysiis/nysiis.py
+-rw-r--r--   0 finn       (501) staff       (20)    34581 2024-04-20 18:21:02.000000 pynysiis-1.0.1/nysiis/six.py
+-rw-r--r--   0 finn       (501) staff       (20)       18 2024-04-20 20:22:55.000000 pynysiis-1.0.1/nysiis/version.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2024-04-20 20:24:17.157148 pynysiis-1.0.1/pynysiis.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     3488 2024-04-20 20:24:17.000000 pynysiis-1.0.1/pynysiis.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      294 2024-04-20 20:24:17.000000 pynysiis-1.0.1/pynysiis.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2024-04-20 20:24:17.000000 pynysiis-1.0.1/pynysiis.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2024-04-20 20:19:34.000000 pynysiis-1.0.1/pynysiis.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)        9 2024-04-20 20:24:17.000000 pynysiis-1.0.1/pynysiis.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)        7 2024-04-20 20:24:17.000000 pynysiis-1.0.1/pynysiis.egg-info/top_level.txt
+-rw-r--r--   0 finn       (501) staff       (20)       38 2024-04-20 20:24:17.158249 pynysiis-1.0.1/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2147 2024-04-20 20:22:55.000000 pynysiis-1.0.1/setup.py
```

### Comparing `pynysiis-1.0.0/LICENSE` & `pynysiis-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynysiis-1.0.0/PKG-INFO` & `pynysiis-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynysiis
-Version: 1.0.0
+Version: 1.0.1
 Summary: NYSIIS phonetic encoding algorithm.
 Home-page: https://finbarrs.eu/
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/nysiis/issues
 Project-URL: Changes, https://github.com/0xnu/nysiis/blob/main/CHANGELOG.md
@@ -24,23 +24,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=2.7, !=3.8.*, !=3.9.*, !=3.10.*
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-nysiis
-=======
+pynysiis
+=========
 
-.. image:: https://badge.fury.io/py/nysiis.svg
-    :target: https://badge.fury.io/py/nysiis
+.. image:: https://badge.fury.io/py/pynysiis.svg
+    :target: https://badge.fury.io/py/pynysiis
     :alt: NYSIIS Python Package Version
 
 
-The `nysiis` package provides a Golang implementation of the `New York State Identification and Intelligence System`_ (NYSIIS) phonetic encoding algorithm. NYSIIS encodes names based on pronunciation, which is helpful in name-matching and searching applications.
+The `pynysiis` package provides a Golang implementation of the `New York State Identification and Intelligence System`_ (NYSIIS) phonetic encoding algorithm. NYSIIS encodes names based on pronunciation, which is helpful in name-matching and searching applications.
 
 .. _New York State Identification and Intelligence System: https://en.wikipedia.org/wiki/New_York_State_Identification_and_Intelligence_System
 
 
 Requirements
 -------------
```

### Comparing `pynysiis-1.0.0/README.md` & `pynysiis-1.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-## nysiis
+## pynysiis
 
 The `nysiis` package provides a Golang implementation of the [New York State Identification and Intelligence System](https://en.wikipedia.org/wiki/New_York_State_Identification_and_Intelligence_System) (NYSIIS) phonetic encoding algorithm. NYSIIS encodes names based on pronunciation, which is helpful in name-matching and searching applications.
 
 ### Requirements
 
 Python 2.7 and later.
 
 ### Setup
 
 You can install this package by using the pip tool and installing:
 
 ```python
-pip install nysiis
+pip install pynysiis
 ## OR
-easy_install nysiis
+easy_install pynysiis
 ```
 
 Install from source with:
 
 ```python
 python setup.py install --user
```

### Comparing `pynysiis-1.0.0/nysiis/nysiis.py` & `pynysiis-1.0.1/nysiis/nysiis.py`

 * *Files identical despite different names*

### Comparing `pynysiis-1.0.0/nysiis/six.py` & `pynysiis-1.0.1/nysiis/six.py`

 * *Files identical despite different names*

### Comparing `pynysiis-1.0.0/pynysiis.egg-info/PKG-INFO` & `pynysiis-1.0.1/pynysiis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynysiis
-Version: 1.0.0
+Version: 1.0.1
 Summary: NYSIIS phonetic encoding algorithm.
 Home-page: https://finbarrs.eu/
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/nysiis/issues
 Project-URL: Changes, https://github.com/0xnu/nysiis/blob/main/CHANGELOG.md
@@ -24,23 +24,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=2.7, !=3.8.*, !=3.9.*, !=3.10.*
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-nysiis
-=======
+pynysiis
+=========
 
-.. image:: https://badge.fury.io/py/nysiis.svg
-    :target: https://badge.fury.io/py/nysiis
+.. image:: https://badge.fury.io/py/pynysiis.svg
+    :target: https://badge.fury.io/py/pynysiis
     :alt: NYSIIS Python Package Version
 
 
-The `nysiis` package provides a Golang implementation of the `New York State Identification and Intelligence System`_ (NYSIIS) phonetic encoding algorithm. NYSIIS encodes names based on pronunciation, which is helpful in name-matching and searching applications.
+The `pynysiis` package provides a Golang implementation of the `New York State Identification and Intelligence System`_ (NYSIIS) phonetic encoding algorithm. NYSIIS encodes names based on pronunciation, which is helpful in name-matching and searching applications.
 
 .. _New York State Identification and Intelligence System: https://en.wikipedia.org/wiki/New_York_State_Identification_and_Intelligence_System
 
 
 Requirements
 -------------
```

### Comparing `pynysiis-1.0.0/setup.py` & `pynysiis-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "pynysiis"
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 REQUIRES = ["pydantic"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

