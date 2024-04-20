# Comparing `tmp/notfunny-0.5.0.tar.gz` & `tmp/notfunny-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notfunny-0.5.0.tar", last modified: Sat Apr 20 16:28:47 2024, max compression
+gzip compressed data, was "notfunny-0.5.1.tar", last modified: Sat Apr 20 16:30:51 2024, max compression
```

## Comparing `notfunny-0.5.0.tar` & `notfunny-0.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:28:47.229933 notfunny-0.5.0/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      217 2024-04-20 16:28:47.229813 notfunny-0.5.0/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       65 2024-04-20 16:25:03.000000 notfunny-0.5.0/README.md
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:28:47.228731 notfunny-0.5.0/notfunny/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       21 2024-04-20 16:22:12.000000 notfunny-0.5.0/notfunny/__init__.py
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      221 2024-04-20 16:27:35.000000 notfunny-0.5.0/notfunny/joke.py
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:28:47.229657 notfunny-0.5.0/notfunny.egg-info/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      217 2024-04-20 16:28:47.000000 notfunny-0.5.0/notfunny.egg-info/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      246 2024-04-20 16:28:47.000000 notfunny-0.5.0/notfunny.egg-info/SOURCES.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 16:28:47.000000 notfunny-0.5.0/notfunny.egg-info/dependency_links.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 13:31:25.000000 notfunny-0.5.0/notfunny.egg-info/not-zip-safe
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 16:28:47.000000 notfunny-0.5.0/notfunny.egg-info/requires.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 16:28:47.000000 notfunny-0.5.0/notfunny.egg-info/top_level.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-20 16:28:47.229982 notfunny-0.5.0/setup.cfg
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      359 2024-04-20 16:28:42.000000 notfunny-0.5.0/setup.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:30:51.851955 notfunny-0.5.1/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      217 2024-04-20 16:30:51.851852 notfunny-0.5.1/PKG-INFO
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       65 2024-04-20 16:25:03.000000 notfunny-0.5.1/README.md
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:30:51.850884 notfunny-0.5.1/notfunny/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       22 2024-04-20 16:30:36.000000 notfunny-0.5.1/notfunny/__init__.py
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      221 2024-04-20 16:27:35.000000 notfunny-0.5.1/notfunny/joke.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:30:51.851706 notfunny-0.5.1/notfunny.egg-info/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      217 2024-04-20 16:30:51.000000 notfunny-0.5.1/notfunny.egg-info/PKG-INFO
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      246 2024-04-20 16:30:51.000000 notfunny-0.5.1/notfunny.egg-info/SOURCES.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 16:30:51.000000 notfunny-0.5.1/notfunny.egg-info/dependency_links.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 13:31:25.000000 notfunny-0.5.1/notfunny.egg-info/not-zip-safe
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 16:30:51.000000 notfunny-0.5.1/notfunny.egg-info/requires.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 16:30:51.000000 notfunny-0.5.1/notfunny.egg-info/top_level.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-20 16:30:51.851996 notfunny-0.5.1/setup.cfg
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      359 2024-04-20 16:30:41.000000 notfunny-0.5.1/setup.py
```

