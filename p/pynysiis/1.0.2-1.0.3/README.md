# Comparing `tmp/pynysiis-1.0.2.tar.gz` & `tmp/pynysiis-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynysiis-1.0.2.tar", last modified: Sat Apr 20 20:38:11 2024, max compression
+gzip compressed data, was "pynysiis-1.0.3.tar", last modified: Sat Apr 20 20:49:11 2024, max compression
```

## Comparing `pynysiis-1.0.2.tar` & `pynysiis-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2024-04-20 20:38:11.300495 pynysiis-1.0.2/
--rw-r--r--   0 finn       (501) staff       (20)     1099 2024-04-20 18:17:07.000000 pynysiis-1.0.2/LICENSE
--rw-r--r--   0 finn       (501) staff       (20)     3621 2024-04-20 20:38:11.300774 pynysiis-1.0.2/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     1802 2024-04-20 20:35:50.000000 pynysiis-1.0.2/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2024-04-20 20:38:11.296335 pynysiis-1.0.2/nysiis/
--rw-r--r--   0 finn       (501) staff       (20)       93 2024-04-20 20:36:02.000000 pynysiis-1.0.2/nysiis/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     8805 2024-04-20 20:36:04.000000 pynysiis-1.0.2/nysiis/nysiis.py
--rw-r--r--   0 finn       (501) staff       (20)    34581 2024-04-20 18:21:02.000000 pynysiis-1.0.2/nysiis/six.py
--rw-r--r--   0 finn       (501) staff       (20)       18 2024-04-20 20:37:39.000000 pynysiis-1.0.2/nysiis/version.py
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2024-04-20 20:38:11.300024 pynysiis-1.0.2/pynysiis.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     3621 2024-04-20 20:38:11.000000 pynysiis-1.0.2/pynysiis.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      294 2024-04-20 20:38:11.000000 pynysiis-1.0.2/pynysiis.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2024-04-20 20:38:11.000000 pynysiis-1.0.2/pynysiis.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2024-04-20 20:19:34.000000 pynysiis-1.0.2/pynysiis.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)        9 2024-04-20 20:38:11.000000 pynysiis-1.0.2/pynysiis.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)        7 2024-04-20 20:38:11.000000 pynysiis-1.0.2/pynysiis.egg-info/top_level.txt
--rw-r--r--   0 finn       (501) staff       (20)       38 2024-04-20 20:38:11.301798 pynysiis-1.0.2/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2147 2024-04-20 20:37:39.000000 pynysiis-1.0.2/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2024-04-20 20:49:11.605473 pynysiis-1.0.3/
+-rw-r--r--   0 finn       (501) staff       (20)     1099 2024-04-20 18:17:07.000000 pynysiis-1.0.3/LICENSE
+-rw-r--r--   0 finn       (501) staff       (20)     4881 2024-04-20 20:49:11.605757 pynysiis-1.0.3/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     2996 2024-04-20 20:47:54.000000 pynysiis-1.0.3/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2024-04-20 20:49:11.601666 pynysiis-1.0.3/nysiis/
+-rw-r--r--   0 finn       (501) staff       (20)       93 2024-04-20 20:36:02.000000 pynysiis-1.0.3/nysiis/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     8805 2024-04-20 20:36:04.000000 pynysiis-1.0.3/nysiis/nysiis.py
+-rw-r--r--   0 finn       (501) staff       (20)    34581 2024-04-20 18:21:02.000000 pynysiis-1.0.3/nysiis/six.py
+-rw-r--r--   0 finn       (501) staff       (20)       18 2024-04-20 20:48:56.000000 pynysiis-1.0.3/nysiis/version.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2024-04-20 20:49:11.605012 pynysiis-1.0.3/pynysiis.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     4881 2024-04-20 20:49:11.000000 pynysiis-1.0.3/pynysiis.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      294 2024-04-20 20:49:11.000000 pynysiis-1.0.3/pynysiis.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2024-04-20 20:49:11.000000 pynysiis-1.0.3/pynysiis.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2024-04-20 20:19:34.000000 pynysiis-1.0.3/pynysiis.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)        9 2024-04-20 20:49:11.000000 pynysiis-1.0.3/pynysiis.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)        7 2024-04-20 20:49:11.000000 pynysiis-1.0.3/pynysiis.egg-info/top_level.txt
+-rw-r--r--   0 finn       (501) staff       (20)       38 2024-04-20 20:49:11.606573 pynysiis-1.0.3/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2147 2024-04-20 20:48:56.000000 pynysiis-1.0.3/setup.py
```

### Comparing `pynysiis-1.0.2/LICENSE` & `pynysiis-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pynysiis-1.0.2/nysiis/nysiis.py` & `pynysiis-1.0.3/nysiis/nysiis.py`

 * *Files identical despite different names*

### Comparing `pynysiis-1.0.2/nysiis/six.py` & `pynysiis-1.0.3/nysiis/six.py`

 * *Files identical despite different names*

### Comparing `pynysiis-1.0.2/setup.py` & `pynysiis-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "pynysiis"
-VERSION = "1.0.2"
+VERSION = "1.0.3"
 REQUIRES = ["pydantic"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

