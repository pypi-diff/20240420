# Comparing `tmp/notfunny-0.6.6.tar.gz` & `tmp/notfunny-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notfunny-0.6.6.tar", last modified: Sat Apr 20 19:37:42 2024, max compression
+gzip compressed data, was "notfunny-0.6.8.tar", last modified: Sat Apr 20 19:49:49 2024, max compression
```

## Comparing `notfunny-0.6.6.tar` & `notfunny-0.6.8.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:37:42.071111 notfunny-0.6.6/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       20 2024-04-20 16:37:33.000000 notfunny-0.6.6/MANIFEST.in
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      591 2024-04-20 19:37:42.070993 notfunny-0.6.6/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       65 2024-04-20 16:25:03.000000 notfunny-0.6.6/README.md
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       95 2024-04-20 16:37:15.000000 notfunny-0.6.6/README.rst
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:37:42.069815 notfunny-0.6.6/bin/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       63 2024-04-20 19:20:31.000000 notfunny-0.6.6/bin/notfunny-joke
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:37:42.070083 notfunny-0.6.6/notfunny/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       22 2024-04-20 16:30:36.000000 notfunny-0.6.6/notfunny/__init__.py
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      147 2024-04-20 16:32:25.000000 notfunny-0.6.6/notfunny/joke.py
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:37:42.070838 notfunny-0.6.6/notfunny.egg-info/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      591 2024-04-20 19:37:42.000000 notfunny-0.6.6/notfunny.egg-info/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      287 2024-04-20 19:37:42.000000 notfunny-0.6.6/notfunny.egg-info/SOURCES.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 19:37:42.000000 notfunny-0.6.6/notfunny.egg-info/dependency_links.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 13:31:25.000000 notfunny-0.6.6/notfunny.egg-info/not-zip-safe
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 19:37:42.000000 notfunny-0.6.6/notfunny.egg-info/requires.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 19:37:42.000000 notfunny-0.6.6/notfunny.egg-info/top_level.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-20 19:37:42.071168 notfunny-0.6.6/setup.cfg
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      902 2024-04-20 19:37:26.000000 notfunny-0.6.6/setup.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:49:49.420968 notfunny-0.6.8/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       20 2024-04-20 16:37:33.000000 notfunny-0.6.8/MANIFEST.in
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      591 2024-04-20 19:49:49.420855 notfunny-0.6.8/PKG-INFO
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       65 2024-04-20 16:25:03.000000 notfunny-0.6.8/README.md
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       95 2024-04-20 16:37:15.000000 notfunny-0.6.8/README.rst
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:49:49.419067 notfunny-0.6.8/bin/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       63 2024-04-20 19:20:31.000000 notfunny-0.6.8/bin/notfunny-joke
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:49:49.419768 notfunny-0.6.8/notfunny/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       22 2024-04-20 16:30:36.000000 notfunny-0.6.8/notfunny/__init__.py
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       57 2024-04-20 19:47:47.000000 notfunny-0.6.8/notfunny/command_line.py
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      147 2024-04-20 16:32:25.000000 notfunny-0.6.8/notfunny/joke.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 19:49:49.420700 notfunny-0.6.8/notfunny.egg-info/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      591 2024-04-20 19:49:49.000000 notfunny-0.6.8/notfunny.egg-info/PKG-INFO
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      312 2024-04-20 19:49:49.000000 notfunny-0.6.8/notfunny.egg-info/SOURCES.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 19:49:49.000000 notfunny-0.6.8/notfunny.egg-info/dependency_links.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 13:31:25.000000 notfunny-0.6.8/notfunny.egg-info/not-zip-safe
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 19:49:49.000000 notfunny-0.6.8/notfunny.egg-info/requires.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 19:49:49.000000 notfunny-0.6.8/notfunny.egg-info/top_level.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-20 19:49:49.421009 notfunny-0.6.8/setup.cfg
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      971 2024-04-20 19:49:37.000000 notfunny-0.6.8/setup.py
```

### Comparing `notfunny-0.6.6/PKG-INFO` & `notfunny-0.6.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notfunny
-Version: 0.6.6
+Version: 0.6.8
 Summary: Only the worst
 Home-page: http://github.com/ohthepain/notfunny
 Author: Paul Wilkinson
 Author-email: paul@thisco.co
 License: MIT
 Keywords: joke
 Platform: UNKNOWN
```

### Comparing `notfunny-0.6.6/notfunny.egg-info/PKG-INFO` & `notfunny-0.6.8/notfunny.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notfunny
-Version: 0.6.6
+Version: 0.6.8
 Summary: Only the worst
 Home-page: http://github.com/ohthepain/notfunny
 Author: Paul Wilkinson
 Author-email: paul@thisco.co
 License: MIT
 Keywords: joke
 Platform: UNKNOWN
```

### Comparing `notfunny-0.6.6/setup.py` & `notfunny-0.6.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='notfunny',
-      version='0.6.6',
+      version='0.6.8',
       description='Only the worst',
       long_description='Really, the worst jokes around. Actually just the one worst. This is really just a test project for packaging python projects. But as an added bonus it really isnt funny.',
       classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
         'Topic :: Text Processing :: Linguistic',
@@ -13,13 +13,14 @@
       keywords='joke',
       url='http://github.com/ohthepain/notfunny',
       author='Paul Wilkinson',
       author_email='paul@thisco.co',
       license='MIT',
       packages=['notfunny'],
       scripts=['bin/notfunny-joke'],
+      console_scripts= ['funniest-joke=funniest.command_line:main'],
       install_requires=[
             'unittest'
       ],
       test_suite='nose.collector',
       tests_require=['nose'],
       zip_safe=False)
```

