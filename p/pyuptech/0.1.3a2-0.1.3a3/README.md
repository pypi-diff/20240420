# Comparing `tmp/pyuptech-0.1.3a2.tar.gz` & `tmp/pyuptech-0.1.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuptech-0.1.3a2.tar", last modified: Sat Apr 20 15:50:07 2024, max compression
+gzip compressed data, was "pyuptech-0.1.3a3.tar", last modified: Sat Apr 20 15:56:01 2024, max compression
```

## Comparing `pyuptech-0.1.3a2.tar` & `pyuptech-0.1.3a3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     7052 2024-04-20 15:49:51.254282 pyuptech-0.1.3a2/README.md
--rw-r--r--   0        0        0      462 2024-04-20 15:50:07.550658 pyuptech-0.1.3a2/pyproject.toml
--rw-r--r--   0        0        0     1095 2024-04-20 15:49:51.254282 pyuptech-0.1.3a2/src/pyuptech/__init__.py
--rw-r--r--   0        0        0      110 2024-04-20 15:49:51.254282 pyuptech-0.1.3a2/src/pyuptech/modules/constant.py
--rw-r--r--   0        0        0     1096 2024-04-20 15:49:51.254282 pyuptech-0.1.3a2/src/pyuptech/modules/loader.py
--rw-r--r--   0        0        0      577 2024-04-20 15:49:51.254282 pyuptech-0.1.3a2/src/pyuptech/modules/logger.py
--rw-r--r--   0        0        0     1725 2024-04-20 15:49:51.254282 pyuptech-0.1.3a2/src/pyuptech/modules/pins.py
--rw-r--r--   0        0        0    10454 2024-04-20 15:49:51.254282 pyuptech-0.1.3a2/src/pyuptech/modules/screen.py
--rw-r--r--   0        0        0     9833 2024-04-20 15:49:51.254282 pyuptech-0.1.3a2/src/pyuptech/modules/sensors.py
--rw-r--r--   0        0        0     4912 2024-04-20 15:49:51.254282 pyuptech-0.1.3a2/src/pyuptech/tools/display.py
--rw-r--r--   0        0        0        0 2024-04-20 15:49:51.254282 pyuptech-0.1.3a2/tests/__init__.py
--rw-r--r--   0        0        0     1105 2024-04-20 15:49:51.254282 pyuptech-0.1.3a2/tests/perf_tests.py
--rw-r--r--   0        0        0     7369 1970-01-01 00:00:00.000000 pyuptech-0.1.3a2/PKG-INFO
+-rw-r--r--   0        0        0     7052 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/README.md
+-rw-r--r--   0        0        0      462 2024-04-20 15:56:01.263247 pyuptech-0.1.3a3/pyproject.toml
+-rw-r--r--   0        0        0     1095 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/src/pyuptech/__init__.py
+-rw-r--r--   0        0        0   219512 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/src/pyuptech/lib/libuptech.so
+-rw-r--r--   0        0        0      110 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/src/pyuptech/modules/constant.py
+-rw-r--r--   0        0        0     1096 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/src/pyuptech/modules/loader.py
+-rw-r--r--   0        0        0      577 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/src/pyuptech/modules/logger.py
+-rw-r--r--   0        0        0     1725 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/src/pyuptech/modules/pins.py
+-rw-r--r--   0        0        0    10454 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/src/pyuptech/modules/screen.py
+-rw-r--r--   0        0        0     9833 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/src/pyuptech/modules/sensors.py
+-rw-r--r--   0        0        0     4912 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/src/pyuptech/tools/display.py
+-rw-r--r--   0        0        0        0 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/tests/__init__.py
+-rw-r--r--   0        0        0     1105 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/tests/perf_tests.py
+-rw-r--r--   0        0        0     7369 1970-01-01 00:00:00.000000 pyuptech-0.1.3a3/PKG-INFO
```

### Comparing `pyuptech-0.1.3a2/README.md` & `pyuptech-0.1.3a3/README.md`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a2/src/pyuptech/__init__.py` & `pyuptech-0.1.3a3/src/pyuptech/__init__.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a2/src/pyuptech/modules/loader.py` & `pyuptech-0.1.3a3/src/pyuptech/modules/loader.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a2/src/pyuptech/modules/logger.py` & `pyuptech-0.1.3a3/src/pyuptech/modules/logger.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a2/src/pyuptech/modules/pins.py` & `pyuptech-0.1.3a3/src/pyuptech/modules/pins.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a2/src/pyuptech/modules/screen.py` & `pyuptech-0.1.3a3/src/pyuptech/modules/screen.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a2/src/pyuptech/modules/sensors.py` & `pyuptech-0.1.3a3/src/pyuptech/modules/sensors.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a2/src/pyuptech/tools/display.py` & `pyuptech-0.1.3a3/src/pyuptech/tools/display.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a2/tests/perf_tests.py` & `pyuptech-0.1.3a3/tests/perf_tests.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a2/PKG-INFO` & `pyuptech-0.1.3a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuptech
-Version: 0.1.3a2
+Version: 0.1.3a3
 Summary: A Python wrapper for the uptech binary lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: terminaltables>=3.1.10
 Description-Content-Type: text/markdown
```

