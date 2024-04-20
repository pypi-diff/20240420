# Comparing `tmp/pyhasura-1.0.0.tar.gz` & `tmp/pyhasura-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhasura-1.0.0.tar", last modified: Fri Apr 19 21:26:46 2024, max compression
+gzip compressed data, was "pyhasura-1.0.2.tar", last modified: Sat Apr 20 12:43:03 2024, max compression
```

## Comparing `pyhasura-1.0.0.tar` & `pyhasura-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-19 21:26:46.444988 pyhasura-1.0.0/
--rw-r--r--   0 kennethstott   (501) staff       (20)     3438 2024-04-19 21:26:46.444836 pyhasura-1.0.0/PKG-INFO
--rw-r--r--   0 kennethstott   (501) staff       (20)     2967 2024-04-19 21:24:41.000000 pyhasura-1.0.0/README.md
-drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-19 21:26:46.442592 pyhasura-1.0.0/pyhasura/
--rw-r--r--   0 kennethstott   (501) staff       (20)      136 2024-04-19 18:25:03.000000 pyhasura-1.0.0/pyhasura/__init__.py
--rw-r--r--   0 kennethstott   (501) staff       (20)      745 2024-04-19 10:52:53.000000 pyhasura-1.0.0/pyhasura/flatten_dict.py
--rw-r--r--   0 kennethstott   (501) staff       (20)      364 2024-04-19 10:56:57.000000 pyhasura-1.0.0/pyhasura/gql_client.py
--rw-r--r--   0 kennethstott   (501) staff       (20)    13008 2024-04-19 21:13:47.000000 pyhasura-1.0.0/pyhasura/hasura_client.py
-drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-19 21:26:46.444468 pyhasura-1.0.0/pyhasura.egg-info/
--rw-r--r--   0 kennethstott   (501) staff       (20)     3438 2024-04-19 21:26:46.000000 pyhasura-1.0.0/pyhasura.egg-info/PKG-INFO
--rw-r--r--   0 kennethstott   (501) staff       (20)      287 2024-04-19 21:26:46.000000 pyhasura-1.0.0/pyhasura.egg-info/SOURCES.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)        1 2024-04-19 21:26:46.000000 pyhasura-1.0.0/pyhasura.egg-info/dependency_links.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)       74 2024-04-19 21:26:46.000000 pyhasura-1.0.0/pyhasura.egg-info/requires.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)        9 2024-04-19 21:26:46.000000 pyhasura-1.0.0/pyhasura.egg-info/top_level.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)      481 2024-04-19 20:25:27.000000 pyhasura-1.0.0/pyproject.toml
--rw-r--r--   0 kennethstott   (501) staff       (20)       38 2024-04-19 21:26:46.445048 pyhasura-1.0.0/setup.cfg
--rw-r--r--   0 kennethstott   (501) staff       (20)      346 2024-04-19 19:59:34.000000 pyhasura-1.0.0/setup.py
+drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-20 12:43:03.228135 pyhasura-1.0.2/
+-rw-r--r--   0 kennethstott   (501) staff       (20)     1065 2024-04-20 12:02:03.000000 pyhasura-1.0.2/LICENSE
+-rw-r--r--   0 kennethstott   (501) staff       (20)     3546 2024-04-20 12:43:03.227934 pyhasura-1.0.2/PKG-INFO
+-rw-r--r--   0 kennethstott   (501) staff       (20)     2967 2024-04-19 21:24:41.000000 pyhasura-1.0.2/README.md
+drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-20 12:43:03.226727 pyhasura-1.0.2/pyhasura/
+-rw-r--r--   0 kennethstott   (501) staff       (20)      136 2024-04-19 18:25:03.000000 pyhasura-1.0.2/pyhasura/__init__.py
+-rw-r--r--   0 kennethstott   (501) staff       (20)      745 2024-04-19 10:52:53.000000 pyhasura-1.0.2/pyhasura/flatten_dict.py
+-rw-r--r--   0 kennethstott   (501) staff       (20)      359 2024-04-20 12:07:08.000000 pyhasura-1.0.2/pyhasura/gql_client.py
+-rw-r--r--   0 kennethstott   (501) staff       (20)    13008 2024-04-19 21:13:47.000000 pyhasura-1.0.2/pyhasura/hasura_client.py
+drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-20 12:43:03.227572 pyhasura-1.0.2/pyhasura.egg-info/
+-rw-r--r--   0 kennethstott   (501) staff       (20)     3546 2024-04-20 12:43:03.000000 pyhasura-1.0.2/pyhasura.egg-info/PKG-INFO
+-rw-r--r--   0 kennethstott   (501) staff       (20)      295 2024-04-20 12:43:03.000000 pyhasura-1.0.2/pyhasura.egg-info/SOURCES.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)        1 2024-04-20 12:43:03.000000 pyhasura-1.0.2/pyhasura.egg-info/dependency_links.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)       82 2024-04-20 12:43:03.000000 pyhasura-1.0.2/pyhasura.egg-info/requires.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)        9 2024-04-20 12:43:03.000000 pyhasura-1.0.2/pyhasura.egg-info/top_level.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)      712 2024-04-20 12:31:56.000000 pyhasura-1.0.2/pyproject.toml
+-rw-r--r--   0 kennethstott   (501) staff       (20)       38 2024-04-20 12:43:03.228240 pyhasura-1.0.2/setup.cfg
+-rw-r--r--   0 kennethstott   (501) staff       (20)      427 2024-04-20 12:22:29.000000 pyhasura-1.0.2/setup.py
```

### Comparing `pyhasura-1.0.0/PKG-INFO` & `pyhasura-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: pyhasura
-Version: 1.0.0
+Version: 1.0.2
 Summary: A Python library to simplify Hasura, GraphQL and Machine Learning
 Author-email: Kenneth Stott <ken@kenstott.com>
+Project-URL: respository, https://github.com/kenstott/pyhasura
 Keywords: graphql,hasura,ml,ai,machine learning,arrow
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: scikit-learn
 Requires-Dist: scikit-learn-extra
 Requires-Dist: pyarrow
 Requires-Dist: pandas
 Requires-Dist: gql
 Requires-Dist: python-dotenv
 Requires-Dist: pprintpp
+Requires-Dist: aiohttp
 
 # PyHasura
 
 A library for conveniently working with Hasura, GraphQL, File Formats, and some basic Machine Learning.
 
 ## Getting Started
```

### Comparing `pyhasura-1.0.0/README.md` & `pyhasura-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.0/pyhasura/flatten_dict.py` & `pyhasura-1.0.2/pyhasura/flatten_dict.py`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.0/pyhasura/hasura_client.py` & `pyhasura-1.0.2/pyhasura/hasura_client.py`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.0/pyhasura.egg-info/PKG-INFO` & `pyhasura-1.0.2/pyhasura.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: pyhasura
-Version: 1.0.0
+Version: 1.0.2
 Summary: A Python library to simplify Hasura, GraphQL and Machine Learning
 Author-email: Kenneth Stott <ken@kenstott.com>
+Project-URL: respository, https://github.com/kenstott/pyhasura
 Keywords: graphql,hasura,ml,ai,machine learning,arrow
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: scikit-learn
 Requires-Dist: scikit-learn-extra
 Requires-Dist: pyarrow
 Requires-Dist: pandas
 Requires-Dist: gql
 Requires-Dist: python-dotenv
 Requires-Dist: pprintpp
+Requires-Dist: aiohttp
 
 # PyHasura
 
 A library for conveniently working with Hasura, GraphQL, File Formats, and some basic Machine Learning.
 
 ## Getting Started
```

