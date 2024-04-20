# Comparing `tmp/ondilo-0.4.0.tar.gz` & `tmp/ondilo-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ondilo-0.4.0.tar", last modified: Fri Mar 22 16:48:02 2024, max compression
+gzip compressed data, was "ondilo-0.5.0.tar", last modified: Sat Apr 20 16:33:38 2024, max compression
```

## Comparing `ondilo-0.4.0.tar` & `ondilo-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:48:02.592084 ondilo-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-22 16:47:51.000000 ondilo-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-22 16:48:02.592084 ondilo-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-03-22 16:47:51.000000 ondilo-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 16:48:02.592084 ondilo-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-22 16:47:51.000000 ondilo-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:48:02.588084 ondilo-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:48:02.588084 ondilo-0.4.0/src/ondilo/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-22 16:47:51.000000 ondilo-0.4.0/src/ondilo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-03-22 16:47:51.000000 ondilo-0.4.0/src/ondilo/ondilo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:48:02.592084 ondilo-0.4.0/src/ondilo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-22 16:48:02.000000 ondilo-0.4.0/src/ondilo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-22 16:48:02.000000 ondilo-0.4.0/src/ondilo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 16:48:02.000000 ondilo-0.4.0/src/ondilo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-22 16:48:02.000000 ondilo-0.4.0/src/ondilo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-22 16:48:02.000000 ondilo-0.4.0/src/ondilo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:33:38.642005 ondilo-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-20 16:33:27.000000 ondilo-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-20 16:33:38.642005 ondilo-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-20 16:33:27.000000 ondilo-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 16:33:38.642005 ondilo-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-20 16:33:27.000000 ondilo-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:33:38.642005 ondilo-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:33:38.642005 ondilo-0.5.0/src/ondilo/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-20 16:33:27.000000 ondilo-0.5.0/src/ondilo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-20 16:33:27.000000 ondilo-0.5.0/src/ondilo/ondilo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:33:38.642005 ondilo-0.5.0/src/ondilo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-20 16:33:38.000000 ondilo-0.5.0/src/ondilo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-20 16:33:38.000000 ondilo-0.5.0/src/ondilo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 16:33:38.000000 ondilo-0.5.0/src/ondilo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-20 16:33:38.000000 ondilo-0.5.0/src/ondilo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-20 16:33:38.000000 ondilo-0.5.0/src/ondilo.egg-info/top_level.txt
```

### Comparing `ondilo-0.4.0/LICENSE.txt` & `ondilo-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ondilo-0.4.0/PKG-INFO` & `ondilo-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondilo
-Version: 0.4.0
+Version: 0.5.0
 Summary: A client to access Ondilo ICO APIs
 Home-page: https://github.com/JeromeHXP/ondilo
 Author: Jérôme Mainguet
 Author-email: dartdoka@mainguet.fr
 License: MIT
 Description: Ondilo ICO
         ==========
```

### Comparing `ondilo-0.4.0/README.md` & `ondilo-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ondilo-0.4.0/setup.py` & `ondilo-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ondilo",
-    version="0.4.0",
+    version="0.5.0",
     author="Jérôme Mainguet",
     author_email="dartdoka@mainguet.fr",
     description="A client to access Ondilo ICO APIs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JeromeHXP/ondilo",
     packages=setuptools.find_packages('src'),
```

### Comparing `ondilo-0.4.0/src/ondilo.egg-info/PKG-INFO` & `ondilo-0.5.0/src/ondilo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondilo
-Version: 0.4.0
+Version: 0.5.0
 Summary: A client to access Ondilo ICO APIs
 Home-page: https://github.com/JeromeHXP/ondilo
 Author: Jérôme Mainguet
 Author-email: dartdoka@mainguet.fr
 License: MIT
 Description: Ondilo ICO
         ==========
```

