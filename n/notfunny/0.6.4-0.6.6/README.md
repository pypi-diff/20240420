# Comparing `tmp/notfunny-0.6.4.tar.gz` & `tmp/notfunny-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notfunny-0.6.4.tar", last modified: Sat Apr 20 19:33:23 2024, max compression
+gzip compressed data, was "notfunny-0.6.6.tar", last modified: Sat Apr 20 19:37:42 2024, max compression
```

## Comparing `notfunny-0.6.4.tar` & `notfunny-0.6.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:33:23.434754 notfunny-0.6.4/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       20 2024-04-20 16:37:33.000000 notfunny-0.6.4/MANIFEST.in
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      591 2024-04-20 19:33:23.434634 notfunny-0.6.4/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       65 2024-04-20 16:25:03.000000 notfunny-0.6.4/README.md
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       95 2024-04-20 16:37:15.000000 notfunny-0.6.4/README.rst
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:33:23.432790 notfunny-0.6.4/bin/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       63 2024-04-20 19:20:31.000000 notfunny-0.6.4/bin/notfunny_joke
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:33:23.433341 notfunny-0.6.4/notfunny/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       22 2024-04-20 16:30:36.000000 notfunny-0.6.4/notfunny/__init__.py
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      147 2024-04-20 16:32:25.000000 notfunny-0.6.4/notfunny/joke.py
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:33:23.434463 notfunny-0.6.4/notfunny.egg-info/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      591 2024-04-20 19:33:23.000000 notfunny-0.6.4/notfunny.egg-info/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      287 2024-04-20 19:33:23.000000 notfunny-0.6.4/notfunny.egg-info/SOURCES.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 19:33:23.000000 notfunny-0.6.4/notfunny.egg-info/dependency_links.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 13:31:25.000000 notfunny-0.6.4/notfunny.egg-info/not-zip-safe
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 19:33:23.000000 notfunny-0.6.4/notfunny.egg-info/requires.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 19:33:23.000000 notfunny-0.6.4/notfunny.egg-info/top_level.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-20 19:33:23.434813 notfunny-0.6.4/setup.cfg
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      902 2024-04-20 19:33:14.000000 notfunny-0.6.4/setup.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:37:42.071111 notfunny-0.6.6/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       20 2024-04-20 16:37:33.000000 notfunny-0.6.6/MANIFEST.in
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      591 2024-04-20 19:37:42.070993 notfunny-0.6.6/PKG-INFO
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       65 2024-04-20 16:25:03.000000 notfunny-0.6.6/README.md
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       95 2024-04-20 16:37:15.000000 notfunny-0.6.6/README.rst
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:37:42.069815 notfunny-0.6.6/bin/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       63 2024-04-20 19:20:31.000000 notfunny-0.6.6/bin/notfunny-joke
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:37:42.070083 notfunny-0.6.6/notfunny/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       22 2024-04-20 16:30:36.000000 notfunny-0.6.6/notfunny/__init__.py
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      147 2024-04-20 16:32:25.000000 notfunny-0.6.6/notfunny/joke.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:37:42.070838 notfunny-0.6.6/notfunny.egg-info/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      591 2024-04-20 19:37:42.000000 notfunny-0.6.6/notfunny.egg-info/PKG-INFO
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      287 2024-04-20 19:37:42.000000 notfunny-0.6.6/notfunny.egg-info/SOURCES.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 19:37:42.000000 notfunny-0.6.6/notfunny.egg-info/dependency_links.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 13:31:25.000000 notfunny-0.6.6/notfunny.egg-info/not-zip-safe
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 19:37:42.000000 notfunny-0.6.6/notfunny.egg-info/requires.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 19:37:42.000000 notfunny-0.6.6/notfunny.egg-info/top_level.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-20 19:37:42.071168 notfunny-0.6.6/setup.cfg
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      902 2024-04-20 19:37:26.000000 notfunny-0.6.6/setup.py
```

### Comparing `notfunny-0.6.4/PKG-INFO` & `notfunny-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notfunny
-Version: 0.6.4
+Version: 0.6.6
 Summary: Only the worst
 Home-page: http://github.com/ohthepain/notfunny
 Author: Paul Wilkinson
 Author-email: paul@thisco.co
 License: MIT
 Keywords: joke
 Platform: UNKNOWN
```

### Comparing `notfunny-0.6.4/notfunny.egg-info/PKG-INFO` & `notfunny-0.6.6/notfunny.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notfunny
-Version: 0.6.4
+Version: 0.6.6
 Summary: Only the worst
 Home-page: http://github.com/ohthepain/notfunny
 Author: Paul Wilkinson
 Author-email: paul@thisco.co
 License: MIT
 Keywords: joke
 Platform: UNKNOWN
```

### Comparing `notfunny-0.6.4/setup.py` & `notfunny-0.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup
 
 setup(name='notfunny',
-      version='0.6.4',
+      version='0.6.6',
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
-      scripts=['bin/notfunny_joke'],
+      scripts=['bin/notfunny-joke'],
       install_requires=[
             'unittest'
       ],
       test_suite='nose.collector',
       tests_require=['nose'],
       zip_safe=False)
```

