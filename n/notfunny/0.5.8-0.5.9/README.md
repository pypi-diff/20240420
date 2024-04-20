# Comparing `tmp/notfunny-0.5.8.tar.gz` & `tmp/notfunny-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notfunny-0.5.8.tar", last modified: Sat Apr 20 16:58:41 2024, max compression
+gzip compressed data, was "notfunny-0.5.9.tar", last modified: Sat Apr 20 17:00:29 2024, max compression
```

## Comparing `notfunny-0.5.8.tar` & `notfunny-0.5.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:58:41.203106 notfunny-0.5.8/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       20 2024-04-20 16:37:33.000000 notfunny-0.5.8/MANIFEST.in
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      591 2024-04-20 16:58:41.202992 notfunny-0.5.8/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       65 2024-04-20 16:25:03.000000 notfunny-0.5.8/README.md
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       95 2024-04-20 16:37:15.000000 notfunny-0.5.8/README.rst
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:58:41.201860 notfunny-0.5.8/notfunny/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       22 2024-04-20 16:30:36.000000 notfunny-0.5.8/notfunny/__init__.py
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      147 2024-04-20 16:32:25.000000 notfunny-0.5.8/notfunny/joke.py
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:58:41.202840 notfunny-0.5.8/notfunny.egg-info/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      591 2024-04-20 16:58:41.000000 notfunny-0.5.8/notfunny.egg-info/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      269 2024-04-20 16:58:41.000000 notfunny-0.5.8/notfunny.egg-info/SOURCES.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 16:58:41.000000 notfunny-0.5.8/notfunny.egg-info/dependency_links.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 13:31:25.000000 notfunny-0.5.8/notfunny.egg-info/not-zip-safe
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 16:58:41.000000 notfunny-0.5.8/notfunny.egg-info/requires.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 16:58:41.000000 notfunny-0.5.8/notfunny.egg-info/top_level.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-20 16:58:41.203147 notfunny-0.5.8/setup.cfg
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      800 2024-04-20 16:58:30.000000 notfunny-0.5.8/setup.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 17:00:29.011907 notfunny-0.5.9/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       20 2024-04-20 16:37:33.000000 notfunny-0.5.9/MANIFEST.in
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      591 2024-04-20 17:00:29.011799 notfunny-0.5.9/PKG-INFO
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       65 2024-04-20 16:25:03.000000 notfunny-0.5.9/README.md
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       95 2024-04-20 16:37:15.000000 notfunny-0.5.9/README.rst
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 17:00:29.010706 notfunny-0.5.9/notfunny/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       22 2024-04-20 16:30:36.000000 notfunny-0.5.9/notfunny/__init__.py
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      147 2024-04-20 16:32:25.000000 notfunny-0.5.9/notfunny/joke.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 17:00:29.011635 notfunny-0.5.9/notfunny.egg-info/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      591 2024-04-20 17:00:29.000000 notfunny-0.5.9/notfunny.egg-info/PKG-INFO
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      269 2024-04-20 17:00:29.000000 notfunny-0.5.9/notfunny.egg-info/SOURCES.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 17:00:29.000000 notfunny-0.5.9/notfunny.egg-info/dependency_links.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 13:31:25.000000 notfunny-0.5.9/notfunny.egg-info/not-zip-safe
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 17:00:29.000000 notfunny-0.5.9/notfunny.egg-info/requires.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 17:00:29.000000 notfunny-0.5.9/notfunny.egg-info/top_level.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-20 17:00:29.011949 notfunny-0.5.9/setup.cfg
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      865 2024-04-20 17:00:25.000000 notfunny-0.5.9/setup.py
```

### Comparing `notfunny-0.5.8/PKG-INFO` & `notfunny-0.5.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notfunny
-Version: 0.5.8
+Version: 0.5.9
 Summary: Only the worst
 Home-page: http://github.com/ohthepain/notfunny
 Author: Paul Wilkinson
 Author-email: paul@thisco.co
 License: MIT
 Keywords: joke
 Platform: UNKNOWN
```

### Comparing `notfunny-0.5.8/notfunny.egg-info/PKG-INFO` & `notfunny-0.5.9/notfunny.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notfunny
-Version: 0.5.8
+Version: 0.5.9
 Summary: Only the worst
 Home-page: http://github.com/ohthepain/notfunny
 Author: Paul Wilkinson
 Author-email: paul@thisco.co
 License: MIT
 Keywords: joke
 Platform: UNKNOWN
```

