# Comparing `tmp/notfunny-0.5.4.tar.gz` & `tmp/notfunny-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notfunny-0.5.4.tar", last modified: Sat Apr 20 16:37:41 2024, max compression
+gzip compressed data, was "notfunny-0.5.6.tar", last modified: Sat Apr 20 16:55:03 2024, max compression
```

## Comparing `notfunny-0.5.4.tar` & `notfunny-0.5.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:37:41.632752 notfunny-0.5.4/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       20 2024-04-20 16:37:33.000000 notfunny-0.5.4/MANIFEST.in
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      485 2024-04-20 16:37:41.632623 notfunny-0.5.4/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       65 2024-04-20 16:25:03.000000 notfunny-0.5.4/README.md
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       95 2024-04-20 16:37:15.000000 notfunny-0.5.4/README.rst
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:37:41.631434 notfunny-0.5.4/notfunny/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       22 2024-04-20 16:30:36.000000 notfunny-0.5.4/notfunny/__init__.py
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      147 2024-04-20 16:32:25.000000 notfunny-0.5.4/notfunny/joke.py
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:37:41.632439 notfunny-0.5.4/notfunny.egg-info/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      485 2024-04-20 16:37:41.000000 notfunny-0.5.4/notfunny.egg-info/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      238 2024-04-20 16:37:41.000000 notfunny-0.5.4/notfunny.egg-info/SOURCES.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 16:37:41.000000 notfunny-0.5.4/notfunny.egg-info/dependency_links.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 13:31:25.000000 notfunny-0.5.4/notfunny.egg-info/not-zip-safe
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 16:37:41.000000 notfunny-0.5.4/notfunny.egg-info/top_level.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-20 16:37:41.632803 notfunny-0.5.4/setup.cfg
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      671 2024-04-20 16:36:18.000000 notfunny-0.5.4/setup.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:55:03.857010 notfunny-0.5.6/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       20 2024-04-20 16:37:33.000000 notfunny-0.5.6/MANIFEST.in
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      591 2024-04-20 16:55:03.856901 notfunny-0.5.6/PKG-INFO
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       65 2024-04-20 16:25:03.000000 notfunny-0.5.6/README.md
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       95 2024-04-20 16:37:15.000000 notfunny-0.5.6/README.rst
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:55:03.855980 notfunny-0.5.6/notfunny/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       22 2024-04-20 16:30:36.000000 notfunny-0.5.6/notfunny/__init__.py
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      147 2024-04-20 16:32:25.000000 notfunny-0.5.6/notfunny/joke.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:55:03.856746 notfunny-0.5.6/notfunny.egg-info/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      591 2024-04-20 16:55:03.000000 notfunny-0.5.6/notfunny.egg-info/PKG-INFO
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      238 2024-04-20 16:55:03.000000 notfunny-0.5.6/notfunny.egg-info/SOURCES.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 16:55:03.000000 notfunny-0.5.6/notfunny.egg-info/dependency_links.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 13:31:25.000000 notfunny-0.5.6/notfunny.egg-info/not-zip-safe
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 16:55:03.000000 notfunny-0.5.6/notfunny.egg-info/top_level.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-20 16:55:03.857057 notfunny-0.5.6/setup.cfg
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      777 2024-04-20 16:54:53.000000 notfunny-0.5.6/setup.py
```

### Comparing `notfunny-0.5.4/setup.py` & `notfunny-0.5.6/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(name='notfunny',
-      version='0.5.4',
+      version='0.5.6',
       description='Only the worst',
-      long_description='Really, the worst jokes around. Actually the just the one worst.',
+      long_description='Really, the worst jokes around. Actually just the one worst. This is really just a test project for packaging python projects. But as an added bonus it really isnt funny.',
       classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
         'Topic :: Text Processing :: Linguistic',
       ],
       keywords='joke',
```

