# Comparing `tmp/flechemano-0.1.tar.gz` & `tmp/flechemano-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flechemano-0.1.tar", last modified: Sat Apr 20 07:14:32 2024, max compression
+gzip compressed data, was "flechemano-0.2.tar", last modified: Sat Apr 20 07:41:15 2024, max compression
```

## Comparing `flechemano-0.1.tar` & `flechemano-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 07:14:32.989907 flechemano-0.1/
--rw-r--r--   0 root         (0) root         (0)      709 2024-04-20 07:14:32.989907 flechemano-0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      413 2024-04-20 07:12:43.000000 flechemano-0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 07:14:32.989907 flechemano-0.1/flechemano.egg-info/
--rw-r--r--   0 root         (0) root         (0)      709 2024-04-20 07:14:32.000000 flechemano-0.1/flechemano.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      187 2024-04-20 07:14:32.000000 flechemano-0.1/flechemano.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 07:14:32.000000 flechemano-0.1/flechemano.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-20 07:14:32.000000 flechemano-0.1/flechemano.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 07:14:32.000000 flechemano-0.1/flechemano.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 07:14:32.989907 flechemano-0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      466 2024-04-20 07:14:25.000000 flechemano-0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 07:41:15.100909 flechemano-0.2/
+-rw-r--r--   0 root         (0) root         (0)      709 2024-04-20 07:41:15.100909 flechemano-0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      413 2024-04-20 07:12:43.000000 flechemano-0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 07:41:15.096908 flechemano-0.2/flechemano.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      709 2024-04-20 07:41:15.000000 flechemano-0.2/flechemano.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      187 2024-04-20 07:41:15.000000 flechemano-0.2/flechemano.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 07:41:15.000000 flechemano-0.2/flechemano.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-20 07:41:15.000000 flechemano-0.2/flechemano.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 07:41:15.000000 flechemano-0.2/flechemano.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 07:41:15.100909 flechemano-0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      466 2024-04-20 07:40:54.000000 flechemano-0.2/setup.py
```

### Comparing `flechemano-0.1/PKG-INFO` & `flechemano-0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flechemano
-Version: 0.1
+Version: 0.2
 Summary: A package developed for blacktea024 to integrate it with PyPI.
 Home-page: https://github.com/flechemano/flechemano
 Author: flechemano
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `flechemano-0.1/flechemano.egg-info/PKG-INFO` & `flechemano-0.2/flechemano.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flechemano
-Version: 0.1
+Version: 0.2
 Summary: A package developed for blacktea024 to integrate it with PyPI.
 Home-page: https://github.com/flechemano/flechemano
 Author: flechemano
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

