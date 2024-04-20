# Comparing `tmp/churchtools-0.1.7.tar.gz` & `tmp/churchtools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "churchtools-0.1.7.tar", last modified: Fri Jul 14 08:42:29 2023, max compression
+gzip compressed data, was "churchtools-0.1.8.tar", last modified: Fri Jul 14 08:46:00 2023, max compression
```

## Comparing `churchtools-0.1.7.tar` & `churchtools-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:42:29.161047 churchtools-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-14 08:42:20.000000 churchtools-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-14 08:42:29.161047 churchtools-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-14 08:42:20.000000 churchtools-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:42:29.157047 churchtools-0.1.7/churchtools/
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/calendars.py
--rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/ct_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/departments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/general.py
--rw-r--r--   0 runner    (1001) docker     (123)    11764 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/persons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/songs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/wiki.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:42:29.157047 churchtools-0.1.7/churchtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-14 08:42:29.000000 churchtools-0.1.7/churchtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-14 08:42:29.000000 churchtools-0.1.7/churchtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:42:29.000000 churchtools-0.1.7/churchtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 08:42:29.000000 churchtools-0.1.7/churchtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 08:42:29.000000 churchtools-0.1.7/churchtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 08:42:29.161047 churchtools-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-14 08:42:20.000000 churchtools-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:46:00.543709 churchtools-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-14 08:45:52.000000 churchtools-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-14 08:46:00.543709 churchtools-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-14 08:45:52.000000 churchtools-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:46:00.543709 churchtools-0.1.8/churchtools/
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-07-14 08:45:52.000000 churchtools-0.1.8/churchtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-14 08:45:52.000000 churchtools-0.1.8/churchtools/calendars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-07-14 08:45:52.000000 churchtools-0.1.8/churchtools/ct_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-14 08:45:52.000000 churchtools-0.1.8/churchtools/departments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-14 08:45:52.000000 churchtools-0.1.8/churchtools/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-14 08:45:52.000000 churchtools-0.1.8/churchtools/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11764 2023-07-14 08:45:52.000000 churchtools-0.1.8/churchtools/persons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-14 08:45:52.000000 churchtools-0.1.8/churchtools/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-14 08:45:52.000000 churchtools-0.1.8/churchtools/songs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-14 08:45:52.000000 churchtools-0.1.8/churchtools/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-14 08:45:52.000000 churchtools-0.1.8/churchtools/wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:46:00.543709 churchtools-0.1.8/churchtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-14 08:46:00.000000 churchtools-0.1.8/churchtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-14 08:46:00.000000 churchtools-0.1.8/churchtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:46:00.000000 churchtools-0.1.8/churchtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-14 08:46:00.000000 churchtools-0.1.8/churchtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 08:46:00.000000 churchtools-0.1.8/churchtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 08:46:00.543709 churchtools-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-14 08:45:52.000000 churchtools-0.1.8/setup.py
```

### Comparing `churchtools-0.1.7/LICENSE` & `churchtools-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.7/PKG-INFO` & `churchtools-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: churchtools
-Version: 0.1.7
+Version: 0.1.8
 Summary: A library for the ChurchTools API
 Home-page: https://git.sr.ht/~pglaum/pychurchtools
 Author: Philipp Glaum
 Author-email: p@pglaum.de
 License: GPLv3
 Keywords: api churchtools
 Classifier: Programming Language :: Python :: 3
```

### Comparing `churchtools-0.1.7/README.md` & `churchtools-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.7/churchtools/__init__.py` & `churchtools-0.1.8/churchtools/__init__.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.7/churchtools/calendars.py` & `churchtools-0.1.8/churchtools/calendars.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.7/churchtools/ct_types.py` & `churchtools-0.1.8/churchtools/ct_types.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.7/churchtools/departments.py` & `churchtools-0.1.8/churchtools/departments.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.7/churchtools/events.py` & `churchtools-0.1.8/churchtools/events.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.7/churchtools/general.py` & `churchtools-0.1.8/churchtools/general.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.7/churchtools/persons.py` & `churchtools-0.1.8/churchtools/persons.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.7/churchtools/services.py` & `churchtools-0.1.8/churchtools/services.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.7/churchtools/songs.py` & `churchtools-0.1.8/churchtools/songs.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.7/churchtools/status.py` & `churchtools-0.1.8/churchtools/status.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.7/churchtools/wiki.py` & `churchtools-0.1.8/churchtools/wiki.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.7/churchtools.egg-info/PKG-INFO` & `churchtools-0.1.8/churchtools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: churchtools
-Version: 0.1.7
+Version: 0.1.8
 Summary: A library for the ChurchTools API
 Home-page: https://git.sr.ht/~pglaum/pychurchtools
 Author: Philipp Glaum
 Author-email: p@pglaum.de
 License: GPLv3
 Keywords: api churchtools
 Classifier: Programming Language :: Python :: 3
```

### Comparing `churchtools-0.1.7/setup.py` & `churchtools-0.1.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="churchtools",
-    version="0.1.7",
+    version="0.1.8",
     author="Philipp Glaum",
     author_email="p@pglaum.de",
     description=("A library for the ChurchTools API"),
     license="GPLv3",
     keywords="api churchtools",
     url="https://git.sr.ht/~pglaum/pychurchtools",
     packages=["churchtools"],
-    install_requires=["pydantic", "requests"],
+    install_requires=["pydantic==1.10.10", "requests"],
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     ],
```

