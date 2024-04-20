# Comparing `tmp/notfunny-0.6.0.tar.gz` & `tmp/notfunny-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notfunny-0.6.0.tar", last modified: Sat Apr 20 19:21:08 2024, max compression
+gzip compressed data, was "notfunny-0.6.3.tar", last modified: Sat Apr 20 19:32:31 2024, max compression
```

## Comparing `notfunny-0.6.0.tar` & `notfunny-0.6.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:21:08.783371 notfunny-0.6.0/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       20 2024-04-20 16:37:33.000000 notfunny-0.6.0/MANIFEST.in
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      591 2024-04-20 19:21:08.783251 notfunny-0.6.0/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       65 2024-04-20 16:25:03.000000 notfunny-0.6.0/README.md
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       95 2024-04-20 16:37:15.000000 notfunny-0.6.0/README.rst
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:21:08.782075 notfunny-0.6.0/notfunny/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       22 2024-04-20 16:30:36.000000 notfunny-0.6.0/notfunny/__init__.py
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      147 2024-04-20 16:32:25.000000 notfunny-0.6.0/notfunny/joke.py
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:21:08.783082 notfunny-0.6.0/notfunny.egg-info/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      591 2024-04-20 19:21:08.000000 notfunny-0.6.0/notfunny.egg-info/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      269 2024-04-20 19:21:08.000000 notfunny-0.6.0/notfunny.egg-info/SOURCES.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 19:21:08.000000 notfunny-0.6.0/notfunny.egg-info/dependency_links.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 13:31:25.000000 notfunny-0.6.0/notfunny.egg-info/not-zip-safe
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 19:21:08.000000 notfunny-0.6.0/notfunny.egg-info/requires.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 19:21:08.000000 notfunny-0.6.0/notfunny.egg-info/top_level.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-20 19:21:08.783415 notfunny-0.6.0/setup.cfg
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      902 2024-04-20 19:21:00.000000 notfunny-0.6.0/setup.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:32:31.907968 notfunny-0.6.3/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       20 2024-04-20 16:37:33.000000 notfunny-0.6.3/MANIFEST.in
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      591 2024-04-20 19:32:31.907863 notfunny-0.6.3/PKG-INFO
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       65 2024-04-20 16:25:03.000000 notfunny-0.6.3/README.md
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       95 2024-04-20 16:37:15.000000 notfunny-0.6.3/README.rst
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:32:31.906119 notfunny-0.6.3/bin/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       63 2024-04-20 19:20:31.000000 notfunny-0.6.3/bin/notfunny_joke
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:32:31.906680 notfunny-0.6.3/notfunny/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       22 2024-04-20 16:30:36.000000 notfunny-0.6.3/notfunny/__init__.py
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      147 2024-04-20 16:32:25.000000 notfunny-0.6.3/notfunny/joke.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:32:31.907721 notfunny-0.6.3/notfunny.egg-info/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      591 2024-04-20 19:32:31.000000 notfunny-0.6.3/notfunny.egg-info/PKG-INFO
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      287 2024-04-20 19:32:31.000000 notfunny-0.6.3/notfunny.egg-info/SOURCES.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 19:32:31.000000 notfunny-0.6.3/notfunny.egg-info/dependency_links.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 13:31:25.000000 notfunny-0.6.3/notfunny.egg-info/not-zip-safe
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 19:32:31.000000 notfunny-0.6.3/notfunny.egg-info/requires.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 19:32:31.000000 notfunny-0.6.3/notfunny.egg-info/top_level.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-20 19:32:31.908012 notfunny-0.6.3/setup.cfg
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      904 2024-04-20 19:31:43.000000 notfunny-0.6.3/setup.py
```

### Comparing `notfunny-0.6.0/PKG-INFO` & `notfunny-0.6.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notfunny
-Version: 0.6.0
+Version: 0.6.3
 Summary: Only the worst
 Home-page: http://github.com/ohthepain/notfunny
 Author: Paul Wilkinson
 Author-email: paul@thisco.co
 License: MIT
 Keywords: joke
 Platform: UNKNOWN
```

### Comparing `notfunny-0.6.0/notfunny.egg-info/PKG-INFO` & `notfunny-0.6.3/notfunny.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notfunny
-Version: 0.6.0
+Version: 0.6.3
 Summary: Only the worst
 Home-page: http://github.com/ohthepain/notfunny
 Author: Paul Wilkinson
 Author-email: paul@thisco.co
 License: MIT
 Keywords: joke
 Platform: UNKNOWN
```

### Comparing `notfunny-0.6.0/setup.py` & `notfunny-0.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup
 
 setup(name='notfunny',
-      version='0.6.0',
+      version='0.6.3',
       description='Only the worst',
       long_description='Really, the worst jokes around. Actually just the one worst. This is really just a test project for packaging python projects. But as an added bonus it really isnt funny.',
       classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
         'Topic :: Text Processing :: Linguistic',
       ],
       keywords='joke',
       url='http://github.com/ohthepain/notfunny',
       author='Paul Wilkinson',
       author_email='paul@thisco.co',
       license='MIT',
       packages=['notfunny'],
-      scripts=['bin/notfunny-joke'],
+      # scripts=['bin/notfunny_joke'],
       install_requires=[
             'unittest'
       ],
       test_suite='nose.collector',
       tests_require=['nose'],
       zip_safe=False)
```

