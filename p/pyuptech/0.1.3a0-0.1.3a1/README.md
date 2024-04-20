# Comparing `tmp/pyuptech-0.1.3a0.tar.gz` & `tmp/pyuptech-0.1.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuptech-0.1.3a0.tar", last modified: Sat Apr 20 12:24:31 2024, max compression
+gzip compressed data, was "pyuptech-0.1.3a1.tar", last modified: Sat Apr 20 12:42:04 2024, max compression
```

## Comparing `pyuptech-0.1.3a0.tar` & `pyuptech-0.1.3a1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7052 2024-04-20 12:24:13.162366 pyuptech-0.1.3a0/README.md
--rw-r--r--   0        0        0      461 2024-04-20 12:24:31.682448 pyuptech-0.1.3a0/pyproject.toml
--rw-r--r--   0        0        0     1095 2024-04-20 12:24:13.166365 pyuptech-0.1.3a0/src/pyuptech/__init__.py
--rw-r--r--   0        0        0       35 2024-04-20 12:24:13.166365 pyuptech-0.1.3a0/src/pyuptech/modules/constant.py
--rw-r--r--   0        0        0     1096 2024-04-20 12:24:13.166365 pyuptech-0.1.3a0/src/pyuptech/modules/loader.py
--rw-r--r--   0        0        0      577 2024-04-20 12:24:13.166365 pyuptech-0.1.3a0/src/pyuptech/modules/logger.py
--rw-r--r--   0        0        0     1659 2024-04-20 12:24:13.166365 pyuptech-0.1.3a0/src/pyuptech/modules/pins.py
--rw-r--r--   0        0        0    10454 2024-04-20 12:24:13.166365 pyuptech-0.1.3a0/src/pyuptech/modules/screen.py
--rw-r--r--   0        0        0     9833 2024-04-20 12:24:13.166365 pyuptech-0.1.3a0/src/pyuptech/modules/sensors.py
--rw-r--r--   0        0        0     4912 2024-04-20 12:24:13.166365 pyuptech-0.1.3a0/src/pyuptech/tools/display.py
--rw-r--r--   0        0        0        0 2024-04-20 12:24:13.166365 pyuptech-0.1.3a0/tests/__init__.py
--rw-r--r--   0        0        0     1105 2024-04-20 12:24:13.166365 pyuptech-0.1.3a0/tests/perf_tests.py
--rw-r--r--   0        0        0     7369 1970-01-01 00:00:00.000000 pyuptech-0.1.3a0/PKG-INFO
+-rw-r--r--   0        0        0     7052 2024-04-20 12:41:47.782210 pyuptech-0.1.3a1/README.md
+-rw-r--r--   0        0        0      462 2024-04-20 12:42:04.322245 pyuptech-0.1.3a1/pyproject.toml
+-rw-r--r--   0        0        0     1095 2024-04-20 12:41:47.782210 pyuptech-0.1.3a1/src/pyuptech/__init__.py
+-rw-r--r--   0        0        0      110 2024-04-20 12:41:47.782210 pyuptech-0.1.3a1/src/pyuptech/modules/constant.py
+-rw-r--r--   0        0        0     1096 2024-04-20 12:41:47.782210 pyuptech-0.1.3a1/src/pyuptech/modules/loader.py
+-rw-r--r--   0        0        0      577 2024-04-20 12:41:47.782210 pyuptech-0.1.3a1/src/pyuptech/modules/logger.py
+-rw-r--r--   0        0        0     1659 2024-04-20 12:41:47.782210 pyuptech-0.1.3a1/src/pyuptech/modules/pins.py
+-rw-r--r--   0        0        0    10454 2024-04-20 12:41:47.782210 pyuptech-0.1.3a1/src/pyuptech/modules/screen.py
+-rw-r--r--   0        0        0     9833 2024-04-20 12:41:47.782210 pyuptech-0.1.3a1/src/pyuptech/modules/sensors.py
+-rw-r--r--   0        0        0     4912 2024-04-20 12:41:47.782210 pyuptech-0.1.3a1/src/pyuptech/tools/display.py
+-rw-r--r--   0        0        0        0 2024-04-20 12:41:47.782210 pyuptech-0.1.3a1/tests/__init__.py
+-rw-r--r--   0        0        0     1105 2024-04-20 12:41:47.782210 pyuptech-0.1.3a1/tests/perf_tests.py
+-rw-r--r--   0        0        0     7369 1970-01-01 00:00:00.000000 pyuptech-0.1.3a1/PKG-INFO
```

### Comparing `pyuptech-0.1.3a0/README.md` & `pyuptech-0.1.3a1/README.md`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a0/src/pyuptech/__init__.py` & `pyuptech-0.1.3a1/src/pyuptech/__init__.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a0/src/pyuptech/modules/loader.py` & `pyuptech-0.1.3a1/src/pyuptech/modules/loader.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a0/src/pyuptech/modules/logger.py` & `pyuptech-0.1.3a1/src/pyuptech/modules/logger.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a0/src/pyuptech/modules/pins.py` & `pyuptech-0.1.3a1/src/pyuptech/modules/pins.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a0/src/pyuptech/modules/screen.py` & `pyuptech-0.1.3a1/src/pyuptech/modules/screen.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a0/src/pyuptech/modules/sensors.py` & `pyuptech-0.1.3a1/src/pyuptech/modules/sensors.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a0/src/pyuptech/tools/display.py` & `pyuptech-0.1.3a1/src/pyuptech/tools/display.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a0/tests/perf_tests.py` & `pyuptech-0.1.3a1/tests/perf_tests.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a0/PKG-INFO` & `pyuptech-0.1.3a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuptech
-Version: 0.1.3a0
+Version: 0.1.3a1
 Summary: A Python wrapper for the uptech binary lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: terminaltables>=3.1.10
 Description-Content-Type: text/markdown
```

