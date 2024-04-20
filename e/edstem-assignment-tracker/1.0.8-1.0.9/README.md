# Comparing `tmp/edstem_assignment_tracker-1.0.8.tar.gz` & `tmp/edstem_assignment_tracker-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edstem_assignment_tracker-1.0.8.tar", last modified: Fri Apr 19 15:31:36 2024, max compression
+gzip compressed data, was "edstem_assignment_tracker-1.0.9.tar", last modified: Fri Apr 19 16:07:55 2024, max compression
```

## Comparing `edstem_assignment_tracker-1.0.8.tar` & `edstem_assignment_tracker-1.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 15:31:36.094706 edstem_assignment_tracker-1.0.8/
--rw-r--r--   0 trevormoy   (501) staff       (20)       48 2024-04-19 04:25:47.000000 edstem_assignment_tracker-1.0.8/MANIFEST.in
--rw-r--r--   0 trevormoy   (501) staff       (20)      533 2024-04-19 15:31:36.094490 edstem_assignment_tracker-1.0.8/PKG-INFO
--rw-r--r--   0 trevormoy   (501) staff       (20)      610 2024-04-18 13:05:16.000000 edstem_assignment_tracker-1.0.8/README.md
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 15:31:36.090327 edstem_assignment_tracker-1.0.8/edstem/
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 15:31:36.091489 edstem_assignment_tracker-1.0.8/edstem/integration/
--rw-r--r--   0 trevormoy   (501) staff       (20)       13 2024-04-19 01:31:10.000000 edstem_assignment_tracker-1.0.8/edstem/integration/__init__.py
--rw-r--r--   0 trevormoy   (501) staff       (20)     8869 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.8/edstem/integration/get_data.py
--rw-r--r--   0 trevormoy   (501) staff       (20)     1229 2024-04-19 15:31:05.000000 edstem_assignment_tracker-1.0.8/edstem/integration/run_eat.py
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 15:31:36.093465 edstem_assignment_tracker-1.0.8/edstem/integration/storage/
--rw-r--r--   0 trevormoy   (501) staff       (20)    16961 2024-04-19 14:58:57.000000 edstem_assignment_tracker-1.0.8/edstem/integration/storage/avl.cpp
--rw-r--r--   0 trevormoy   (501) staff       (20)     2982 2024-04-19 12:28:10.000000 edstem_assignment_tracker-1.0.8/edstem/integration/storage/avl.h
--rw-r--r--   0 trevormoy   (501) staff       (20)    12157 2024-04-19 14:56:45.000000 edstem_assignment_tracker-1.0.8/edstem/integration/storage/bh.cpp
--rw-r--r--   0 trevormoy   (501) staff       (20)     1738 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.8/edstem/integration/storage/bh.h
--rw-r--r--   0 trevormoy   (501) staff       (20)    12183 2024-04-19 13:48:06.000000 edstem_assignment_tracker-1.0.8/edstem/integration/storage/main.cpp
--rw-r--r--   0 trevormoy   (501) staff       (20)      309 2024-04-19 12:27:38.000000 edstem_assignment_tracker-1.0.8/edstem/integration/storage/node.cpp
--rw-r--r--   0 trevormoy   (501) staff       (20)     1286 2024-04-18 23:34:50.000000 edstem_assignment_tracker-1.0.8/edstem/integration/storage/node.h
--rw-r--r--   0 trevormoy   (501) staff       (20)     5586 2024-04-19 12:27:37.000000 edstem_assignment_tracker-1.0.8/edstem/integration/storage/st.cpp
--rw-r--r--   0 trevormoy   (501) staff       (20)     1549 2024-04-18 23:34:50.000000 edstem_assignment_tracker-1.0.8/edstem/integration/storage/st.h
-drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 15:31:36.094307 edstem_assignment_tracker-1.0.8/edstem_assignment_tracker.egg-info/
--rw-r--r--   0 trevormoy   (501) staff       (20)      533 2024-04-19 15:31:36.000000 edstem_assignment_tracker-1.0.8/edstem_assignment_tracker.egg-info/PKG-INFO
--rw-r--r--   0 trevormoy   (501) staff       (20)      724 2024-04-19 15:31:36.000000 edstem_assignment_tracker-1.0.8/edstem_assignment_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 trevormoy   (501) staff       (20)        1 2024-04-19 15:31:36.000000 edstem_assignment_tracker-1.0.8/edstem_assignment_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 trevormoy   (501) staff       (20)       58 2024-04-19 15:31:36.000000 edstem_assignment_tracker-1.0.8/edstem_assignment_tracker.egg-info/entry_points.txt
--rw-r--r--   0 trevormoy   (501) staff       (20)       24 2024-04-19 15:31:36.000000 edstem_assignment_tracker-1.0.8/edstem_assignment_tracker.egg-info/requires.txt
--rw-r--r--   0 trevormoy   (501) staff       (20)        7 2024-04-19 15:31:36.000000 edstem_assignment_tracker-1.0.8/edstem_assignment_tracker.egg-info/top_level.txt
--rw-r--r--   0 trevormoy   (501) staff       (20)       38 2024-04-19 15:31:36.094756 edstem_assignment_tracker-1.0.8/setup.cfg
--rw-r--r--   0 trevormoy   (501) staff       (20)     1371 2024-04-19 15:31:14.000000 edstem_assignment_tracker-1.0.8/setup.py
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 16:07:55.541589 edstem_assignment_tracker-1.0.9/
+-rw-r--r--   0 trevormoy   (501) staff       (20)       48 2024-04-19 04:25:47.000000 edstem_assignment_tracker-1.0.9/MANIFEST.in
+-rw-r--r--   0 trevormoy   (501) staff       (20)      533 2024-04-19 16:07:55.541398 edstem_assignment_tracker-1.0.9/PKG-INFO
+-rw-r--r--   0 trevormoy   (501) staff       (20)      610 2024-04-18 13:05:16.000000 edstem_assignment_tracker-1.0.9/README.md
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 16:07:55.537004 edstem_assignment_tracker-1.0.9/edstem/
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 16:07:55.538200 edstem_assignment_tracker-1.0.9/edstem/integration/
+-rw-r--r--   0 trevormoy   (501) staff       (20)       13 2024-04-19 01:31:10.000000 edstem_assignment_tracker-1.0.9/edstem/integration/__init__.py
+-rw-r--r--   0 trevormoy   (501) staff       (20)     8869 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.9/edstem/integration/get_data.py
+-rw-r--r--   0 trevormoy   (501) staff       (20)     1229 2024-04-19 15:31:05.000000 edstem_assignment_tracker-1.0.9/edstem/integration/run_eat.py
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 16:07:55.540342 edstem_assignment_tracker-1.0.9/edstem/integration/storage/
+-rw-r--r--   0 trevormoy   (501) staff       (20)    16961 2024-04-19 14:58:57.000000 edstem_assignment_tracker-1.0.9/edstem/integration/storage/avl.cpp
+-rw-r--r--   0 trevormoy   (501) staff       (20)     2982 2024-04-19 12:28:10.000000 edstem_assignment_tracker-1.0.9/edstem/integration/storage/avl.h
+-rw-r--r--   0 trevormoy   (501) staff       (20)    12157 2024-04-19 14:56:45.000000 edstem_assignment_tracker-1.0.9/edstem/integration/storage/bh.cpp
+-rw-r--r--   0 trevormoy   (501) staff       (20)     1738 2024-04-18 23:34:54.000000 edstem_assignment_tracker-1.0.9/edstem/integration/storage/bh.h
+-rw-r--r--   0 trevormoy   (501) staff       (20)    12183 2024-04-19 13:48:06.000000 edstem_assignment_tracker-1.0.9/edstem/integration/storage/main.cpp
+-rw-r--r--   0 trevormoy   (501) staff       (20)      309 2024-04-19 12:27:38.000000 edstem_assignment_tracker-1.0.9/edstem/integration/storage/node.cpp
+-rw-r--r--   0 trevormoy   (501) staff       (20)     1286 2024-04-18 23:34:50.000000 edstem_assignment_tracker-1.0.9/edstem/integration/storage/node.h
+-rw-r--r--   0 trevormoy   (501) staff       (20)     5586 2024-04-19 12:27:37.000000 edstem_assignment_tracker-1.0.9/edstem/integration/storage/st.cpp
+-rw-r--r--   0 trevormoy   (501) staff       (20)     1549 2024-04-18 23:34:50.000000 edstem_assignment_tracker-1.0.9/edstem/integration/storage/st.h
+drwxr-xr-x   0 trevormoy   (501) staff       (20)        0 2024-04-19 16:07:55.541224 edstem_assignment_tracker-1.0.9/edstem_assignment_tracker.egg-info/
+-rw-r--r--   0 trevormoy   (501) staff       (20)      533 2024-04-19 16:07:55.000000 edstem_assignment_tracker-1.0.9/edstem_assignment_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 trevormoy   (501) staff       (20)      724 2024-04-19 16:07:55.000000 edstem_assignment_tracker-1.0.9/edstem_assignment_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)        1 2024-04-19 16:07:55.000000 edstem_assignment_tracker-1.0.9/edstem_assignment_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)       63 2024-04-19 16:07:55.000000 edstem_assignment_tracker-1.0.9/edstem_assignment_tracker.egg-info/entry_points.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)       24 2024-04-19 16:07:55.000000 edstem_assignment_tracker-1.0.9/edstem_assignment_tracker.egg-info/requires.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)        7 2024-04-19 16:07:55.000000 edstem_assignment_tracker-1.0.9/edstem_assignment_tracker.egg-info/top_level.txt
+-rw-r--r--   0 trevormoy   (501) staff       (20)       38 2024-04-19 16:07:55.541634 edstem_assignment_tracker-1.0.9/setup.cfg
+-rw-r--r--   0 trevormoy   (501) staff       (20)     1376 2024-04-19 16:07:09.000000 edstem_assignment_tracker-1.0.9/setup.py
```

### Comparing `edstem_assignment_tracker-1.0.8/PKG-INFO` & `edstem_assignment_tracker-1.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edstem-assignment-tracker
-Version: 1.0.8
+Version: 1.0.9
 Summary: Edstem Assignment Tracker.
 Home-page: https://github.com/SP24-212/Edstem-Tracker
 Author: Trevor Moy
 Author-email: trevormoy14@uri.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `edstem_assignment_tracker-1.0.8/README.md` & `edstem_assignment_tracker-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.8/edstem/integration/get_data.py` & `edstem_assignment_tracker-1.0.9/edstem/integration/get_data.py`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.8/edstem/integration/run_eat.py` & `edstem_assignment_tracker-1.0.9/edstem/integration/run_eat.py`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.8/edstem/integration/storage/avl.cpp` & `edstem_assignment_tracker-1.0.9/edstem/integration/storage/avl.cpp`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.8/edstem/integration/storage/avl.h` & `edstem_assignment_tracker-1.0.9/edstem/integration/storage/avl.h`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.8/edstem/integration/storage/bh.cpp` & `edstem_assignment_tracker-1.0.9/edstem/integration/storage/bh.cpp`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.8/edstem/integration/storage/bh.h` & `edstem_assignment_tracker-1.0.9/edstem/integration/storage/bh.h`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.8/edstem/integration/storage/main.cpp` & `edstem_assignment_tracker-1.0.9/edstem/integration/storage/main.cpp`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.8/edstem/integration/storage/node.h` & `edstem_assignment_tracker-1.0.9/edstem/integration/storage/node.h`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.8/edstem/integration/storage/st.cpp` & `edstem_assignment_tracker-1.0.9/edstem/integration/storage/st.cpp`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.8/edstem/integration/storage/st.h` & `edstem_assignment_tracker-1.0.9/edstem/integration/storage/st.h`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.8/edstem_assignment_tracker.egg-info/PKG-INFO` & `edstem_assignment_tracker-1.0.9/edstem_assignment_tracker.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edstem-assignment-tracker
-Version: 1.0.8
+Version: 1.0.9
 Summary: Edstem Assignment Tracker.
 Home-page: https://github.com/SP24-212/Edstem-Tracker
 Author: Trevor Moy
 Author-email: trevormoy14@uri.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `edstem_assignment_tracker-1.0.8/edstem_assignment_tracker.egg-info/SOURCES.txt` & `edstem_assignment_tracker-1.0.9/edstem_assignment_tracker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edstem_assignment_tracker-1.0.8/setup.py` & `edstem_assignment_tracker-1.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
                         include_dirs=['edstem/integration/storage/'],
                         language='c++',
                         extra_compile_args=['-std=c++11']
                           )
 
 setup(
     name='edstem-assignment-tracker',
-    version='1.0.8',
+    version='1.0.9',
     description='Edstem Assignment Tracker.',
     long_description='Edstem Assignment Tracker is a python package that allows you to easily track your assignments for the Edstem platform.',
     author='Trevor Moy',
     author_email='trevormoy14@uri.edu',
     url='https://github.com/SP24-212/Edstem-Tracker',
     packages=['edstem.integration'],
     package_data={'edstem.integration.storage': ['*.h']},
@@ -25,11 +25,11 @@
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     entry_points={
         'console_scripts': [
-            'ed-tracker = edstem.integration:run_eat'
+            'ed-tracker = edstem.integration.run_eat:main'
         ]
     }
 )
```

