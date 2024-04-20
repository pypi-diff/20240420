# Comparing `tmp/notfunny-0.1.tar.gz` & `tmp/notfunny-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notfunny-0.1.tar", last modified: Sat Apr 20 16:07:19 2024, max compression
+gzip compressed data, was "notfunny-0.2.tar", last modified: Sat Apr 20 16:19:47 2024, max compression
```

## Comparing `notfunny-0.1.tar` & `notfunny-0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:07:19.185789 notfunny-0.1/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      215 2024-04-20 16:07:19.185678 notfunny-0.1/PKG-INFO
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:07:19.184535 notfunny-0.1/notfunny/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      147 2024-04-20 13:23:17.000000 notfunny-0.1/notfunny/__init__.py
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:07:19.185533 notfunny-0.1/notfunny.egg-info/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      215 2024-04-20 16:07:19.000000 notfunny-0.1/notfunny.egg-info/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      188 2024-04-20 16:07:19.000000 notfunny-0.1/notfunny.egg-info/SOURCES.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 16:07:19.000000 notfunny-0.1/notfunny.egg-info/dependency_links.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 13:31:25.000000 notfunny-0.1/notfunny.egg-info/not-zip-safe
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 16:07:19.000000 notfunny-0.1/notfunny.egg-info/top_level.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-20 16:07:19.185831 notfunny-0.1/setup.cfg
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      300 2024-04-20 13:30:09.000000 notfunny-0.1/setup.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:19:47.317747 notfunny-0.2/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      215 2024-04-20 16:19:47.317639 notfunny-0.2/PKG-INFO
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:19:47.316698 notfunny-0.2/notfunny/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:18:39.000000 notfunny-0.2/notfunny/__init__.py
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      147 2024-04-20 16:18:24.000000 notfunny-0.2/notfunny/joke.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:19:47.317497 notfunny-0.2/notfunny.egg-info/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      215 2024-04-20 16:19:47.000000 notfunny-0.2/notfunny.egg-info/PKG-INFO
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      205 2024-04-20 16:19:47.000000 notfunny-0.2/notfunny.egg-info/SOURCES.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 16:19:47.000000 notfunny-0.2/notfunny.egg-info/dependency_links.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 13:31:25.000000 notfunny-0.2/notfunny.egg-info/not-zip-safe
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 16:19:47.000000 notfunny-0.2/notfunny.egg-info/top_level.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-20 16:19:47.317792 notfunny-0.2/setup.cfg
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      300 2024-04-20 16:18:49.000000 notfunny-0.2/setup.py
```

