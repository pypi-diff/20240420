# Comparing `tmp/pynysiis-1.0.1.tar.gz` & `tmp/pynysiis-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynysiis-1.0.1.tar", last modified: Sat Apr 20 20:24:17 2024, max compression
+gzip compressed data, was "pynysiis-1.0.2.tar", last modified: Sat Apr 20 20:38:11 2024, max compression
```

## Comparing `pynysiis-1.0.1.tar` & `pynysiis-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2024-04-20 20:24:17.157450 pynysiis-1.0.1/
--rw-r--r--   0 finn       (501) staff       (20)     1099 2024-04-20 18:17:07.000000 pynysiis-1.0.1/LICENSE
--rw-r--r--   0 finn       (501) staff       (20)     3488 2024-04-20 20:24:17.157620 pynysiis-1.0.1/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     1585 2024-04-20 20:22:51.000000 pynysiis-1.0.1/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2024-04-20 20:24:17.155102 pynysiis-1.0.1/nysiis/
--rw-r--r--   0 finn       (501) staff       (20)       68 2024-04-20 19:18:47.000000 pynysiis-1.0.1/nysiis/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     8805 2024-04-20 19:18:55.000000 pynysiis-1.0.1/nysiis/nysiis.py
--rw-r--r--   0 finn       (501) staff       (20)    34581 2024-04-20 18:21:02.000000 pynysiis-1.0.1/nysiis/six.py
--rw-r--r--   0 finn       (501) staff       (20)       18 2024-04-20 20:22:55.000000 pynysiis-1.0.1/nysiis/version.py
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2024-04-20 20:24:17.157148 pynysiis-1.0.1/pynysiis.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     3488 2024-04-20 20:24:17.000000 pynysiis-1.0.1/pynysiis.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      294 2024-04-20 20:24:17.000000 pynysiis-1.0.1/pynysiis.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2024-04-20 20:24:17.000000 pynysiis-1.0.1/pynysiis.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2024-04-20 20:19:34.000000 pynysiis-1.0.1/pynysiis.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)        9 2024-04-20 20:24:17.000000 pynysiis-1.0.1/pynysiis.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)        7 2024-04-20 20:24:17.000000 pynysiis-1.0.1/pynysiis.egg-info/top_level.txt
--rw-r--r--   0 finn       (501) staff       (20)       38 2024-04-20 20:24:17.158249 pynysiis-1.0.1/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2147 2024-04-20 20:22:55.000000 pynysiis-1.0.1/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2024-04-20 20:38:11.300495 pynysiis-1.0.2/
+-rw-r--r--   0 finn       (501) staff       (20)     1099 2024-04-20 18:17:07.000000 pynysiis-1.0.2/LICENSE
+-rw-r--r--   0 finn       (501) staff       (20)     3621 2024-04-20 20:38:11.300774 pynysiis-1.0.2/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     1802 2024-04-20 20:35:50.000000 pynysiis-1.0.2/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2024-04-20 20:38:11.296335 pynysiis-1.0.2/nysiis/
+-rw-r--r--   0 finn       (501) staff       (20)       93 2024-04-20 20:36:02.000000 pynysiis-1.0.2/nysiis/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     8805 2024-04-20 20:36:04.000000 pynysiis-1.0.2/nysiis/nysiis.py
+-rw-r--r--   0 finn       (501) staff       (20)    34581 2024-04-20 18:21:02.000000 pynysiis-1.0.2/nysiis/six.py
+-rw-r--r--   0 finn       (501) staff       (20)       18 2024-04-20 20:37:39.000000 pynysiis-1.0.2/nysiis/version.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2024-04-20 20:38:11.300024 pynysiis-1.0.2/pynysiis.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     3621 2024-04-20 20:38:11.000000 pynysiis-1.0.2/pynysiis.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      294 2024-04-20 20:38:11.000000 pynysiis-1.0.2/pynysiis.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2024-04-20 20:38:11.000000 pynysiis-1.0.2/pynysiis.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2024-04-20 20:19:34.000000 pynysiis-1.0.2/pynysiis.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)        9 2024-04-20 20:38:11.000000 pynysiis-1.0.2/pynysiis.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)        7 2024-04-20 20:38:11.000000 pynysiis-1.0.2/pynysiis.egg-info/top_level.txt
+-rw-r--r--   0 finn       (501) staff       (20)       38 2024-04-20 20:38:11.301798 pynysiis-1.0.2/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2147 2024-04-20 20:37:39.000000 pynysiis-1.0.2/setup.py
```

### Comparing `pynysiis-1.0.1/LICENSE` & `pynysiis-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynysiis-1.0.1/PKG-INFO` & `pynysiis-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynysiis
-Version: 1.0.1
+Version: 1.0.2
 Summary: NYSIIS phonetic encoding algorithm.
 Home-page: https://finbarrs.eu/
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/nysiis/issues
 Project-URL: Changes, https://github.com/0xnu/nysiis/blob/main/CHANGELOG.md
@@ -64,19 +64,23 @@
 
 
 Usage Example
 -------------
 
 .. code-block:: python
 
-  from nysiis import nysiis
+  from nysiis import NYSIIS
 
-  name = "John Smith"
-  coded_name = nysiis(name)
-  print(coded_name)
+  # Create an instance of the NYSIIS class
+  nysiis = NYSIIS()
+
+  # Encode a string using the NYSIIS instance
+  name = "Watkins"
+  coded_name = nysiis.encode(name)
+  print(coded_name) # Output: "WATCAN"
 
 
 Reference
 ----------
 
 .. code-block:: bibtex
```

### Comparing `pynysiis-1.0.1/README.md` & `pynysiis-1.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -23,15 +23,23 @@
 
 ## or `sudo python setup.py install` to install the package for all users
 ```
 
 ### Usage
 
 ```python
+from nysiis import NYSIIS
 
+# Create an instance of the NYSIIS class
+nysiis = NYSIIS()
+
+# Encode a string using the NYSIIS instance
+name = "Watkins"
+coded_name = nysiis.encode(name)
+print(coded_name) # Output: "WATCAN"
 ```
 
 ### Reference
 
 ```tex
 @inproceedings{Rajkovic2007,
   author    = {Petar Rajkovic and Dragan Jankovic},
```

### Comparing `pynysiis-1.0.1/nysiis/nysiis.py` & `pynysiis-1.0.2/nysiis/nysiis.py`

 * *Files identical despite different names*

### Comparing `pynysiis-1.0.1/nysiis/six.py` & `pynysiis-1.0.2/nysiis/six.py`

 * *Files identical despite different names*

### Comparing `pynysiis-1.0.1/pynysiis.egg-info/PKG-INFO` & `pynysiis-1.0.2/pynysiis.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynysiis
-Version: 1.0.1
+Version: 1.0.2
 Summary: NYSIIS phonetic encoding algorithm.
 Home-page: https://finbarrs.eu/
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/nysiis/issues
 Project-URL: Changes, https://github.com/0xnu/nysiis/blob/main/CHANGELOG.md
@@ -64,19 +64,23 @@
 
 
 Usage Example
 -------------
 
 .. code-block:: python
 
-  from nysiis import nysiis
+  from nysiis import NYSIIS
 
-  name = "John Smith"
-  coded_name = nysiis(name)
-  print(coded_name)
+  # Create an instance of the NYSIIS class
+  nysiis = NYSIIS()
+
+  # Encode a string using the NYSIIS instance
+  name = "Watkins"
+  coded_name = nysiis.encode(name)
+  print(coded_name) # Output: "WATCAN"
 
 
 Reference
 ----------
 
 .. code-block:: bibtex
```

### Comparing `pynysiis-1.0.1/setup.py` & `pynysiis-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "pynysiis"
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 REQUIRES = ["pydantic"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

