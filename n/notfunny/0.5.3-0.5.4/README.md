# Comparing `tmp/notfunny-0.5.3.tar.gz` & `tmp/notfunny-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notfunny-0.5.3.tar", last modified: Sat Apr 20 16:32:40 2024, max compression
+gzip compressed data, was "notfunny-0.5.4.tar", last modified: Sat Apr 20 16:37:41 2024, max compression
```

## Comparing `notfunny-0.5.3.tar` & `notfunny-0.5.4.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:32:40.084401 notfunny-0.5.3/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      217 2024-04-20 16:32:40.084283 notfunny-0.5.3/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       65 2024-04-20 16:25:03.000000 notfunny-0.5.3/README.md
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:32:40.083077 notfunny-0.5.3/notfunny/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       22 2024-04-20 16:30:36.000000 notfunny-0.5.3/notfunny/__init__.py
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      147 2024-04-20 16:32:25.000000 notfunny-0.5.3/notfunny/joke.py
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:32:40.084073 notfunny-0.5.3/notfunny.egg-info/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      217 2024-04-20 16:32:40.000000 notfunny-0.5.3/notfunny.egg-info/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      215 2024-04-20 16:32:40.000000 notfunny-0.5.3/notfunny.egg-info/SOURCES.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 16:32:40.000000 notfunny-0.5.3/notfunny.egg-info/dependency_links.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 13:31:25.000000 notfunny-0.5.3/notfunny.egg-info/not-zip-safe
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 16:32:40.000000 notfunny-0.5.3/notfunny.egg-info/top_level.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-20 16:32:40.084471 notfunny-0.5.3/setup.cfg
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      336 2024-04-20 16:32:31.000000 notfunny-0.5.3/setup.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:37:41.632752 notfunny-0.5.4/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       20 2024-04-20 16:37:33.000000 notfunny-0.5.4/MANIFEST.in
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      485 2024-04-20 16:37:41.632623 notfunny-0.5.4/PKG-INFO
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       65 2024-04-20 16:25:03.000000 notfunny-0.5.4/README.md
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       95 2024-04-20 16:37:15.000000 notfunny-0.5.4/README.rst
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:37:41.631434 notfunny-0.5.4/notfunny/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       22 2024-04-20 16:30:36.000000 notfunny-0.5.4/notfunny/__init__.py
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      147 2024-04-20 16:32:25.000000 notfunny-0.5.4/notfunny/joke.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:37:41.632439 notfunny-0.5.4/notfunny.egg-info/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      485 2024-04-20 16:37:41.000000 notfunny-0.5.4/notfunny.egg-info/PKG-INFO
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      238 2024-04-20 16:37:41.000000 notfunny-0.5.4/notfunny.egg-info/SOURCES.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 16:37:41.000000 notfunny-0.5.4/notfunny.egg-info/dependency_links.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 13:31:25.000000 notfunny-0.5.4/notfunny.egg-info/not-zip-safe
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 16:37:41.000000 notfunny-0.5.4/notfunny.egg-info/top_level.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-20 16:37:41.632803 notfunny-0.5.4/setup.cfg
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      671 2024-04-20 16:36:18.000000 notfunny-0.5.4/setup.py
```

