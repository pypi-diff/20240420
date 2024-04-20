# Comparing `tmp/sponge-0.0.6.tar.gz` & `tmp/sponge-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sponge-0.0.6.tar", last modified: Fri Apr 19 05:12:46 2024, max compression
+gzip compressed data, was "sponge-0.0.7.tar", last modified: Sat Apr 20 09:39:21 2024, max compression
```

## Comparing `sponge-0.0.6.tar` & `sponge-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 william    (502) staff       (20)        0 2024-04-19 05:12:46.086076 sponge-0.0.6/
--rw-r--r--   0 william    (502) staff       (20)    35147 2024-04-19 04:29:01.000000 sponge-0.0.6/LICENSE
--rw-r--r--   0 william    (502) staff       (20)     2189 2024-04-19 05:12:46.085789 sponge-0.0.6/PKG-INFO
--rw-r--r--   0 william    (502) staff       (20)     1275 2024-04-19 04:29:01.000000 sponge-0.0.6/README.rst
--rw-r--r--   0 william    (502) staff       (20)       38 2024-04-19 05:12:46.086189 sponge-0.0.6/setup.cfg
--rw-r--r--   0 william    (502) staff       (20)     1348 2024-04-19 04:29:01.000000 sponge-0.0.6/setup.py
-drwxr-xr-x   0 william    (502) staff       (20)        0 2024-04-19 05:12:46.076770 sponge-0.0.6/sponge/
--rw-r--r--   0 william    (502) staff       (20)      324 2024-04-19 05:12:38.000000 sponge-0.0.6/sponge/__init__.py
-drwxr-xr-x   0 william    (502) staff       (20)        0 2024-04-19 05:12:46.083453 sponge-0.0.6/sponge/drivers/
--rw-r--r--   0 william    (502) staff       (20)      172 2024-04-19 04:29:01.000000 sponge-0.0.6/sponge/drivers/__init__.py
--rw-r--r--   0 william    (502) staff       (20)      624 2024-04-19 04:29:01.000000 sponge-0.0.6/sponge/drivers/driver.py
--rw-r--r--   0 william    (502) staff       (20)     1393 2024-04-19 04:29:01.000000 sponge-0.0.6/sponge/drivers/memory.py
--rw-r--r--   0 william    (502) staff       (20)     1252 2024-04-19 04:29:01.000000 sponge-0.0.6/sponge/drivers/redis.py
--rw-r--r--   0 william    (502) staff       (20)     1842 2024-04-19 04:49:21.000000 sponge-0.0.6/sponge/drivers/sqlite.py
--rw-r--r--   0 william    (502) staff       (20)     1539 2024-04-19 04:29:01.000000 sponge-0.0.6/sponge/manager.py
-drwxr-xr-x   0 william    (502) staff       (20)        0 2024-04-19 05:12:46.081742 sponge-0.0.6/sponge.egg-info/
--rw-r--r--   0 william    (502) staff       (20)     2189 2024-04-19 05:12:45.000000 sponge-0.0.6/sponge.egg-info/PKG-INFO
--rw-r--r--   0 william    (502) staff       (20)      435 2024-04-19 05:12:46.000000 sponge-0.0.6/sponge.egg-info/SOURCES.txt
--rw-r--r--   0 william    (502) staff       (20)        1 2024-04-19 05:12:45.000000 sponge-0.0.6/sponge.egg-info/dependency_links.txt
--rw-r--r--   0 william    (502) staff       (20)       14 2024-04-19 05:12:45.000000 sponge-0.0.6/sponge.egg-info/requires.txt
--rw-r--r--   0 william    (502) staff       (20)       13 2024-04-19 05:12:45.000000 sponge-0.0.6/sponge.egg-info/top_level.txt
-drwxr-xr-x   0 william    (502) staff       (20)        0 2024-04-19 05:12:46.085182 sponge-0.0.6/tests/
--rw-r--r--   0 william    (502) staff       (20)      172 2024-04-19 04:29:01.000000 sponge-0.0.6/tests/__init__.py
--rw-r--r--   0 william    (502) staff       (20)     2137 2024-04-19 04:29:01.000000 sponge-0.0.6/tests/driver.py
--rw-r--r--   0 william    (502) staff       (20)      380 2024-04-19 04:29:01.000000 sponge-0.0.6/tests/test_memory.py
--rw-r--r--   0 william    (502) staff       (20)      379 2024-04-19 04:29:01.000000 sponge-0.0.6/tests/test_redis.py
--rw-r--r--   0 william    (502) staff       (20)     2291 2024-04-19 04:51:57.000000 sponge-0.0.6/tests/test_sqlite.py
+drwxr-xr-x   0 william    (502) staff       (20)        0 2024-04-20 09:39:21.390813 sponge-0.0.7/
+-rw-r--r--   0 william    (502) staff       (20)    35147 2024-04-19 04:29:01.000000 sponge-0.0.7/LICENSE
+-rw-r--r--   0 william    (502) staff       (20)     2189 2024-04-20 09:39:21.390595 sponge-0.0.7/PKG-INFO
+-rw-r--r--   0 william    (502) staff       (20)     1275 2024-04-19 04:29:01.000000 sponge-0.0.7/README.rst
+-rw-r--r--   0 william    (502) staff       (20)       38 2024-04-20 09:39:21.390877 sponge-0.0.7/setup.cfg
+-rw-r--r--   0 william    (502) staff       (20)     1348 2024-04-19 04:29:01.000000 sponge-0.0.7/setup.py
+drwxr-xr-x   0 william    (502) staff       (20)        0 2024-04-20 09:39:21.385362 sponge-0.0.7/sponge/
+-rw-r--r--   0 william    (502) staff       (20)      324 2024-04-20 09:39:05.000000 sponge-0.0.7/sponge/__init__.py
+drwxr-xr-x   0 william    (502) staff       (20)        0 2024-04-20 09:39:21.388461 sponge-0.0.7/sponge/drivers/
+-rw-r--r--   0 william    (502) staff       (20)      172 2024-04-19 04:29:01.000000 sponge-0.0.7/sponge/drivers/__init__.py
+-rw-r--r--   0 william    (502) staff       (20)      624 2024-04-19 04:29:01.000000 sponge-0.0.7/sponge/drivers/driver.py
+-rw-r--r--   0 william    (502) staff       (20)     1393 2024-04-19 04:29:01.000000 sponge-0.0.7/sponge/drivers/memory.py
+-rw-r--r--   0 william    (502) staff       (20)     1252 2024-04-19 04:29:01.000000 sponge-0.0.7/sponge/drivers/redis.py
+-rw-r--r--   0 william    (502) staff       (20)     1842 2024-04-19 05:45:58.000000 sponge-0.0.7/sponge/drivers/sqlite.py
+-rw-r--r--   0 william    (502) staff       (20)     1549 2024-04-19 05:44:20.000000 sponge-0.0.7/sponge/manager.py
+drwxr-xr-x   0 william    (502) staff       (20)        0 2024-04-20 09:39:21.386797 sponge-0.0.7/sponge.egg-info/
+-rw-r--r--   0 william    (502) staff       (20)     2189 2024-04-20 09:39:21.000000 sponge-0.0.7/sponge.egg-info/PKG-INFO
+-rw-r--r--   0 william    (502) staff       (20)      435 2024-04-20 09:39:21.000000 sponge-0.0.7/sponge.egg-info/SOURCES.txt
+-rw-r--r--   0 william    (502) staff       (20)        1 2024-04-20 09:39:21.000000 sponge-0.0.7/sponge.egg-info/dependency_links.txt
+-rw-r--r--   0 william    (502) staff       (20)       14 2024-04-20 09:39:21.000000 sponge-0.0.7/sponge.egg-info/requires.txt
+-rw-r--r--   0 william    (502) staff       (20)       13 2024-04-20 09:39:21.000000 sponge-0.0.7/sponge.egg-info/top_level.txt
+drwxr-xr-x   0 william    (502) staff       (20)        0 2024-04-20 09:39:21.390103 sponge-0.0.7/tests/
+-rw-r--r--   0 william    (502) staff       (20)      172 2024-04-19 04:29:01.000000 sponge-0.0.7/tests/__init__.py
+-rw-r--r--   0 william    (502) staff       (20)     2137 2024-04-19 04:29:01.000000 sponge-0.0.7/tests/driver.py
+-rw-r--r--   0 william    (502) staff       (20)      380 2024-04-19 04:29:01.000000 sponge-0.0.7/tests/test_memory.py
+-rw-r--r--   0 william    (502) staff       (20)      379 2024-04-19 04:29:01.000000 sponge-0.0.7/tests/test_redis.py
+-rw-r--r--   0 william    (502) staff       (20)     2291 2024-04-19 04:51:57.000000 sponge-0.0.7/tests/test_sqlite.py
```

### Comparing `sponge-0.0.6/LICENSE` & `sponge-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sponge-0.0.6/PKG-INFO` & `sponge-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sponge
-Version: 0.0.6
+Version: 0.0.7
 Summary: An elegant cache library for python
 Home-page: https://github.com/IamBusy/sponge
 Author: William Wei
 Author-email: 1342247033@qq.com
 Maintainer: William Wei
 Maintainer-email: 1342247033@qq.com
 License: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `sponge-0.0.6/README.rst` & `sponge-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `sponge-0.0.6/setup.py` & `sponge-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `sponge-0.0.6/sponge/drivers/driver.py` & `sponge-0.0.7/sponge/drivers/driver.py`

 * *Files identical despite different names*

### Comparing `sponge-0.0.6/sponge/drivers/memory.py` & `sponge-0.0.7/sponge/drivers/memory.py`

 * *Files identical despite different names*

### Comparing `sponge-0.0.6/sponge/drivers/redis.py` & `sponge-0.0.7/sponge/drivers/redis.py`

 * *Files identical despite different names*

### Comparing `sponge-0.0.6/sponge/drivers/sqlite.py` & `sponge-0.0.7/sponge/drivers/sqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # encoding: utf-8
 import time
 from sponge.drivers.driver import Driver
 
-class SQLiteDriver(Driver):
+class SqliteDriver(Driver):
 	def __init__(self, cfg=None):
 		import sqlite3
 		self._conn = sqlite3.connect(cfg['db'])
 		self._conn.execute('CREATE TABLE IF NOT EXISTS sponge (key TEXT PRIMARY KEY, value TEXT, expire INTEGER)')
 
 	def get(self, key):
 		current_time = int(time.time())
```

### Comparing `sponge-0.0.6/sponge/manager.py` & `sponge-0.0.7/sponge/manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 @file: manager.py
 @time: 22/05/2018 16:03
 """
 import importlib
 
 
 class CacheManager(object):
-    _supported_stores = ('redis', 'memory')
+    _supported_stores = ('redis', 'memory', 'sqlite')
 
     def __init__(self, cfg):
         self._cfg = cfg
         self._stores = {}
         if 'default' not in cfg:
             keys = list(self._cfg.keys())
             if len(keys) > 0:
```

### Comparing `sponge-0.0.6/sponge.egg-info/PKG-INFO` & `sponge-0.0.7/sponge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sponge
-Version: 0.0.6
+Version: 0.0.7
 Summary: An elegant cache library for python
 Home-page: https://github.com/IamBusy/sponge
 Author: William Wei
 Author-email: 1342247033@qq.com
 Maintainer: William Wei
 Maintainer-email: 1342247033@qq.com
 License: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `sponge-0.0.6/tests/driver.py` & `sponge-0.0.7/tests/driver.py`

 * *Files identical despite different names*

### Comparing `sponge-0.0.6/tests/test_sqlite.py` & `sponge-0.0.7/tests/test_sqlite.py`

 * *Files identical despite different names*

