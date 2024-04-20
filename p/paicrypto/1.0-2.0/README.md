# Comparing `tmp/paicrypto-1.0.tar.gz` & `tmp/paicrypto-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/paicrypto-1.0.tar", last modified: Sat Apr 20 08:27:28 2024, max compression
+gzip compressed data, was "paicrypto-2.0.tar", last modified: Sat Apr 20 08:51:39 2024, max compression
```

## Comparing `paicrypto-1.0.tar` & `paicrypto-2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 adithya   (1000) adithya   (1000)        0 2024-04-20 08:27:28.000000 paicrypto-1.0/
--rw-rw-r--   0 adithya   (1000) adithya   (1000)      221 2024-04-20 08:27:28.000000 paicrypto-1.0/PKG-INFO
--rw-rw-r--   0 adithya   (1000) adithya   (1000)      369 2024-04-20 08:24:56.000000 paicrypto-1.0/setup.py
-drwxrwxr-x   0 adithya   (1000) adithya   (1000)        0 2024-04-20 08:27:28.000000 paicrypto-1.0/paicrypto/
--rw-rw-r--   0 adithya   (1000) adithya   (1000)    13274 2024-04-20 08:27:20.000000 paicrypto-1.0/paicrypto/main.py
--rw-rw-r--   0 adithya   (1000) adithya   (1000)       28 2024-04-20 08:19:28.000000 paicrypto-1.0/paicrypto/__init__.py
--rw-rw-r--   0 adithya   (1000) adithya   (1000)       38 2024-04-20 08:27:28.000000 paicrypto-1.0/setup.cfg
-drwxrwxr-x   0 adithya   (1000) adithya   (1000)        0 2024-04-20 08:27:28.000000 paicrypto-1.0/paicrypto.egg-info/
--rw-rw-r--   0 adithya   (1000) adithya   (1000)       10 2024-04-20 08:27:27.000000 paicrypto-1.0/paicrypto.egg-info/top_level.txt
--rw-rw-r--   0 adithya   (1000) adithya   (1000)      221 2024-04-20 08:27:27.000000 paicrypto-1.0/paicrypto.egg-info/PKG-INFO
--rw-rw-r--   0 adithya   (1000) adithya   (1000)       22 2024-04-20 08:27:27.000000 paicrypto-1.0/paicrypto.egg-info/requires.txt
--rw-rw-r--   0 adithya   (1000) adithya   (1000)      222 2024-04-20 08:27:27.000000 paicrypto-1.0/paicrypto.egg-info/SOURCES.txt
--rw-rw-r--   0 adithya   (1000) adithya   (1000)        1 2024-04-20 08:27:27.000000 paicrypto-1.0/paicrypto.egg-info/dependency_links.txt
--rw-rw-r--   0 adithya   (1000) adithya   (1000)      174 2024-04-20 08:15:36.000000 paicrypto-1.0/README.md
+drwxrwxr-x   0 adithya   (1000) adithya   (1000)        0 2024-04-20 08:51:39.727837 paicrypto-2.0/
+-rw-rw-r--   0 adithya   (1000) adithya   (1000)      468 2024-04-20 08:51:39.723837 paicrypto-2.0/PKG-INFO
+-rw-rw-r--   0 adithya   (1000) adithya   (1000)      174 2024-04-20 08:15:36.000000 paicrypto-2.0/README.md
+drwxrwxr-x   0 adithya   (1000) adithya   (1000)        0 2024-04-20 08:51:39.723837 paicrypto-2.0/paicrypto/
+-rw-rw-r--   0 adithya   (1000) adithya   (1000)       28 2024-04-20 08:19:28.000000 paicrypto-2.0/paicrypto/__init__.py
+-rw-rw-r--   0 adithya   (1000) adithya   (1000)    13274 2024-04-20 08:27:20.000000 paicrypto-2.0/paicrypto/main.py
+drwxrwxr-x   0 adithya   (1000) adithya   (1000)        0 2024-04-20 08:51:39.723837 paicrypto-2.0/paicrypto.egg-info/
+-rw-rw-r--   0 adithya   (1000) adithya   (1000)      468 2024-04-20 08:51:39.000000 paicrypto-2.0/paicrypto.egg-info/PKG-INFO
+-rw-rw-r--   0 adithya   (1000) adithya   (1000)      222 2024-04-20 08:51:39.000000 paicrypto-2.0/paicrypto.egg-info/SOURCES.txt
+-rw-rw-r--   0 adithya   (1000) adithya   (1000)        1 2024-04-20 08:51:39.000000 paicrypto-2.0/paicrypto.egg-info/dependency_links.txt
+-rw-rw-r--   0 adithya   (1000) adithya   (1000)       22 2024-04-20 08:51:39.000000 paicrypto-2.0/paicrypto.egg-info/requires.txt
+-rw-rw-r--   0 adithya   (1000) adithya   (1000)       10 2024-04-20 08:51:39.000000 paicrypto-2.0/paicrypto.egg-info/top_level.txt
+-rw-rw-r--   0 adithya   (1000) adithya   (1000)       38 2024-04-20 08:51:39.727837 paicrypto-2.0/setup.cfg
+-rw-rw-r--   0 adithya   (1000) adithya   (1000)      467 2024-04-20 08:48:58.000000 paicrypto-2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `paicrypto-1.0/paicrypto/main.py` & `paicrypto-2.0/paicrypto/main.py`

 * *Files identical despite different names*

