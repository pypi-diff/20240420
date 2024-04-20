# Comparing `tmp/notfunny-0.3.tar.gz` & `tmp/notfunny-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notfunny-0.3.tar", last modified: Sat Apr 20 16:23:34 2024, max compression
+gzip compressed data, was "notfunny-0.4.tar", last modified: Sat Apr 20 16:25:46 2024, max compression
```

## Comparing `notfunny-0.3.tar` & `notfunny-0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:23:34.274394 notfunny-0.3/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      215 2024-04-20 16:23:34.274261 notfunny-0.3/PKG-INFO
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:23:34.272950 notfunny-0.3/notfunny/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       21 2024-04-20 16:22:12.000000 notfunny-0.3/notfunny/__init__.py
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      147 2024-04-20 16:18:24.000000 notfunny-0.3/notfunny/joke.py
-drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:23:34.274073 notfunny-0.3/notfunny.egg-info/
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      215 2024-04-20 16:23:34.000000 notfunny-0.3/notfunny.egg-info/PKG-INFO
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      205 2024-04-20 16:23:34.000000 notfunny-0.3/notfunny.egg-info/SOURCES.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 16:23:34.000000 notfunny-0.3/notfunny.egg-info/dependency_links.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 13:31:25.000000 notfunny-0.3/notfunny.egg-info/not-zip-safe
--rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 16:23:34.000000 notfunny-0.3/notfunny.egg-info/top_level.txt
--rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-20 16:23:34.274450 notfunny-0.3/setup.cfg
--rw-r--r--   0 paulwilkinson   (501) staff       (20)      300 2024-04-20 16:22:16.000000 notfunny-0.3/setup.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:25:46.240482 notfunny-0.4/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      215 2024-04-20 16:25:46.240362 notfunny-0.4/PKG-INFO
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       65 2024-04-20 16:25:03.000000 notfunny-0.4/README.md
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:25:46.239235 notfunny-0.4/notfunny/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       21 2024-04-20 16:22:12.000000 notfunny-0.4/notfunny/__init__.py
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      147 2024-04-20 16:18:24.000000 notfunny-0.4/notfunny/joke.py
+drwxr-xr-x   0 paulwilkinson   (501) staff       (20)        0 2024-04-20 16:25:46.240183 notfunny-0.4/notfunny.egg-info/
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      215 2024-04-20 16:25:46.000000 notfunny-0.4/notfunny.egg-info/PKG-INFO
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      215 2024-04-20 16:25:46.000000 notfunny-0.4/notfunny.egg-info/SOURCES.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 16:25:46.000000 notfunny-0.4/notfunny.egg-info/dependency_links.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        1 2024-04-20 13:31:25.000000 notfunny-0.4/notfunny.egg-info/not-zip-safe
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)        9 2024-04-20 16:25:46.000000 notfunny-0.4/notfunny.egg-info/top_level.txt
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)       38 2024-04-20 16:25:46.240533 notfunny-0.4/setup.cfg
+-rw-r--r--   0 paulwilkinson   (501) staff       (20)      300 2024-04-20 16:25:20.000000 notfunny-0.4/setup.py
```

