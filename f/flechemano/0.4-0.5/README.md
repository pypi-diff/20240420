# Comparing `tmp/flechemano-0.4.tar.gz` & `tmp/flechemano-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flechemano-0.4.tar", last modified: Sat Apr 20 07:51:30 2024, max compression
+gzip compressed data, was "flechemano-0.5.tar", last modified: Sat Apr 20 08:02:03 2024, max compression
```

## Comparing `flechemano-0.4.tar` & `flechemano-0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 07:51:30.215316 flechemano-0.4/
--rw-r--r--   0 root         (0) root         (0)      683 2024-04-20 07:51:30.215316 flechemano-0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      387 2024-04-20 07:51:01.000000 flechemano-0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 07:51:30.215316 flechemano-0.4/flechemano.egg-info/
--rw-r--r--   0 root         (0) root         (0)      683 2024-04-20 07:51:30.000000 flechemano-0.4/flechemano.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      187 2024-04-20 07:51:30.000000 flechemano-0.4/flechemano.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 07:51:30.000000 flechemano-0.4/flechemano.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-20 07:51:30.000000 flechemano-0.4/flechemano.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 07:51:30.000000 flechemano-0.4/flechemano.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 07:51:30.215316 flechemano-0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      466 2024-04-20 07:51:16.000000 flechemano-0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 08:02:03.486008 flechemano-0.5/
+-rw-r--r--   0 root         (0) root         (0)      683 2024-04-20 08:02:03.486008 flechemano-0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      387 2024-04-20 07:51:01.000000 flechemano-0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 08:02:03.486008 flechemano-0.5/flechemano.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      683 2024-04-20 08:02:03.000000 flechemano-0.5/flechemano.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      187 2024-04-20 08:02:03.000000 flechemano-0.5/flechemano.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 08:02:03.000000 flechemano-0.5/flechemano.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-04-20 08:02:03.000000 flechemano-0.5/flechemano.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 08:02:03.000000 flechemano-0.5/flechemano.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 08:02:03.486008 flechemano-0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      458 2024-04-20 08:01:33.000000 flechemano-0.5/setup.py
```

### Comparing `flechemano-0.4/PKG-INFO` & `flechemano-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flechemano
-Version: 0.4
+Version: 0.5
 Summary: A package developed for blacktea024 to integrate it with PyPI.
 Home-page: https://github.com/flechemano/flechemano
 Author: flechemano
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `flechemano-0.4/flechemano.egg-info/PKG-INFO` & `flechemano-0.5/flechemano.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flechemano
-Version: 0.4
+Version: 0.5
 Summary: A package developed for blacktea024 to integrate it with PyPI.
 Home-page: https://github.com/flechemano/flechemano
 Author: flechemano
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

