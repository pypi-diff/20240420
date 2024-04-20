# Comparing `tmp/pyBSDate-0.3.0rc1.tar.gz` & `tmp/pyBSDate-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyBSDate-0.3.0rc1.tar", last modified: Mon Jun 15 10:38:40 2020, max compression
+gzip compressed data, was "dist/pyBSDate-0.3.1.tar", last modified: Sat Apr 20 05:28:35 2024, max compression
```

## Comparing `pyBSDate-0.3.0rc1.tar` & `pyBSDate-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sushilsh   (501) staff       (20)        0 2020-06-15 10:38:40.000000 pyBSDate-0.3.0rc1/
--rw-r--r--   0 sushilsh   (501) staff       (20)     1923 2020-06-15 10:38:40.000000 pyBSDate-0.3.0rc1/PKG-INFO
-drwxr-xr-x   0 sushilsh   (501) staff       (20)        0 2020-06-15 10:38:40.000000 pyBSDate-0.3.0rc1/pyBSDate/
--rw-r--r--   0 sushilsh   (501) staff       (20)     2731 2020-06-15 04:32:01.000000 pyBSDate-0.3.0rc1/pyBSDate/BaseCalendar.py
--rw-r--r--   0 sushilsh   (501) staff       (20)     1458 2020-06-15 04:32:01.000000 pyBSDate-0.3.0rc1/pyBSDate/DateConverter.py
--rw-r--r--   0 sushilsh   (501) staff       (20)      431 2020-06-15 04:32:01.000000 pyBSDate-0.3.0rc1/pyBSDate/BSCalendar.py
--rw-r--r--   0 sushilsh   (501) staff       (20)      632 2020-06-15 04:32:01.000000 pyBSDate-0.3.0rc1/pyBSDate/__init__.py
--rw-r--r--   0 sushilsh   (501) staff       (20)      621 2020-06-15 04:32:01.000000 pyBSDate-0.3.0rc1/pyBSDate/ADCalendar.py
--rw-r--r--   0 sushilsh   (501) staff       (20)     2376 2020-06-15 10:24:16.000000 pyBSDate-0.3.0rc1/pyBSDate/wrappers.py
--rw-r--r--   0 sushilsh   (501) staff       (20)      652 2020-06-15 04:33:16.000000 pyBSDate-0.3.0rc1/pyBSDate/BSDate.py
--rw-r--r--   0 sushilsh   (501) staff       (20)     4669 2020-06-13 23:40:25.000000 pyBSDate-0.3.0rc1/pyBSDate/utilities.py
--rw-r--r--   0 sushilsh   (501) staff       (20)    13111 2020-06-15 04:32:01.000000 pyBSDate-0.3.0rc1/pyBSDate/DateMap.py
--rw-r--r--   0 sushilsh   (501) staff       (20)     1221 2020-06-13 23:40:25.000000 pyBSDate-0.3.0rc1/README.md
--rw-r--r--   0 sushilsh   (501) staff       (20)      556 2020-06-15 10:36:50.000000 pyBSDate-0.3.0rc1/setup.py
--rw-r--r--   0 sushilsh   (501) staff       (20)       79 2020-06-15 10:38:40.000000 pyBSDate-0.3.0rc1/setup.cfg
-drwxr-xr-x   0 sushilsh   (501) staff       (20)        0 2020-06-15 10:38:40.000000 pyBSDate-0.3.0rc1/pyBSDate.egg-info/
--rw-r--r--   0 sushilsh   (501) staff       (20)     1923 2020-06-15 10:38:40.000000 pyBSDate-0.3.0rc1/pyBSDate.egg-info/PKG-INFO
--rw-r--r--   0 sushilsh   (501) staff       (20)      356 2020-06-15 10:38:40.000000 pyBSDate-0.3.0rc1/pyBSDate.egg-info/SOURCES.txt
--rw-r--r--   0 sushilsh   (501) staff       (20)        9 2020-06-15 10:38:40.000000 pyBSDate-0.3.0rc1/pyBSDate.egg-info/top_level.txt
--rw-r--r--   0 sushilsh   (501) staff       (20)        1 2020-06-15 10:38:40.000000 pyBSDate-0.3.0rc1/pyBSDate.egg-info/dependency_links.txt
+drwxr-xr-x   0 sushilsh   (501) staff       (20)        0 2024-04-20 05:28:34.000000 pyBSDate-0.3.1/
+-rw-r--r--   0 sushilsh   (501) staff       (20)     4715 2024-04-20 05:28:34.000000 pyBSDate-0.3.1/PKG-INFO
+drwxr-xr-x   0 sushilsh   (501) staff       (20)        0 2024-04-20 05:28:34.000000 pyBSDate-0.3.1/pyBSDate/
+-rw-r--r--   0 sushilsh   (501) staff       (20)     2731 2020-06-17 19:00:22.000000 pyBSDate-0.3.1/pyBSDate/BaseCalendar.py
+-rw-r--r--   0 sushilsh   (501) staff       (20)     1458 2020-06-17 19:00:22.000000 pyBSDate-0.3.1/pyBSDate/DateConverter.py
+-rw-r--r--   0 sushilsh   (501) staff       (20)      431 2020-06-17 19:00:22.000000 pyBSDate-0.3.1/pyBSDate/BSCalendar.py
+-rw-r--r--   0 sushilsh   (501) staff       (20)      632 2020-06-17 19:00:22.000000 pyBSDate-0.3.1/pyBSDate/__init__.py
+-rw-r--r--   0 sushilsh   (501) staff       (20)      621 2020-06-17 19:00:22.000000 pyBSDate-0.3.1/pyBSDate/ADCalendar.py
+-rw-r--r--   0 sushilsh   (501) staff       (20)     2376 2020-06-17 19:00:22.000000 pyBSDate-0.3.1/pyBSDate/wrappers.py
+-rw-r--r--   0 sushilsh   (501) staff       (20)      652 2020-06-17 19:00:22.000000 pyBSDate-0.3.1/pyBSDate/BSDate.py
+-rw-r--r--   0 sushilsh   (501) staff       (20)     4669 2020-06-13 23:40:25.000000 pyBSDate-0.3.1/pyBSDate/utilities.py
+-rw-r--r--   0 sushilsh   (501) staff       (20)    13112 2024-04-20 05:16:37.000000 pyBSDate-0.3.1/pyBSDate/DateMap.py
+-rw-r--r--   0 sushilsh   (501) staff       (20)     3232 2024-04-20 05:05:16.000000 pyBSDate-0.3.1/README.md
+-rw-r--r--   0 sushilsh   (501) staff       (20)      757 2024-04-20 05:24:03.000000 pyBSDate-0.3.1/setup.py
+-rw-r--r--   0 sushilsh   (501) staff       (20)       79 2024-04-20 05:28:34.000000 pyBSDate-0.3.1/setup.cfg
+drwxr-xr-x   0 sushilsh   (501) staff       (20)        0 2024-04-20 05:28:34.000000 pyBSDate-0.3.1/pyBSDate.egg-info/
+-rw-r--r--   0 sushilsh   (501) staff       (20)     4715 2024-04-20 05:28:34.000000 pyBSDate-0.3.1/pyBSDate.egg-info/PKG-INFO
+-rw-r--r--   0 sushilsh   (501) staff       (20)      356 2024-04-20 05:28:34.000000 pyBSDate-0.3.1/pyBSDate.egg-info/SOURCES.txt
+-rw-r--r--   0 sushilsh   (501) staff       (20)        9 2024-04-20 05:28:34.000000 pyBSDate-0.3.1/pyBSDate.egg-info/top_level.txt
+-rw-r--r--   0 sushilsh   (501) staff       (20)        1 2024-04-20 05:28:34.000000 pyBSDate-0.3.1/pyBSDate.egg-info/dependency_links.txt
```

### Comparing `pyBSDate-0.3.0rc1/pyBSDate/BaseCalendar.py` & `pyBSDate-0.3.1/pyBSDate/BaseCalendar.py`

 * *Files identical despite different names*

### Comparing `pyBSDate-0.3.0rc1/pyBSDate/DateConverter.py` & `pyBSDate-0.3.1/pyBSDate/DateConverter.py`

 * *Files identical despite different names*

### Comparing `pyBSDate-0.3.0rc1/pyBSDate/__init__.py` & `pyBSDate-0.3.1/pyBSDate/__init__.py`

 * *Files identical despite different names*

### Comparing `pyBSDate-0.3.0rc1/pyBSDate/ADCalendar.py` & `pyBSDate-0.3.1/pyBSDate/ADCalendar.py`

 * *Files identical despite different names*

### Comparing `pyBSDate-0.3.0rc1/pyBSDate/wrappers.py` & `pyBSDate-0.3.1/pyBSDate/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyBSDate-0.3.0rc1/pyBSDate/BSDate.py` & `pyBSDate-0.3.1/pyBSDate/BSDate.py`

 * *Files identical despite different names*

### Comparing `pyBSDate-0.3.0rc1/pyBSDate/utilities.py` & `pyBSDate-0.3.1/pyBSDate/utilities.py`

 * *Files identical despite different names*

### Comparing `pyBSDate-0.3.0rc1/pyBSDate/DateMap.py` & `pyBSDate-0.3.1/pyBSDate/DateMap.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 "2074":{"1stbaisakh":"2017-04-14", "daysonmonth":[31, 31, 31, 32, 31, 31, 30, 29, 30, 29, 30, 30]},
 "2075":{"1stbaisakh":"2018-04-14", "daysonmonth":[31, 31, 32, 31, 31, 31, 30, 29, 30, 29, 30, 30]},
 "2076":{"1stbaisakh":"2019-04-14", "daysonmonth":[31, 32, 31, 32, 31, 30, 30, 30, 29, 29, 30, 30]},
 "2077":{"1stbaisakh":"2020-04-13", "daysonmonth":[31, 32, 31, 32, 31, 30, 30, 30, 29, 30, 29, 31]},
 "2078":{"1stbaisakh":"2021-04-14", "daysonmonth":[31, 31, 31, 32, 31, 31, 30, 29, 30, 29, 30, 30]},
 "2079":{"1stbaisakh":"2022-04-14", "daysonmonth":[31, 31, 32, 31, 31, 31, 30, 29, 30, 29, 30, 30]},
 "2080":{"1stbaisakh":"2023-04-14", "daysonmonth":[31, 32, 31, 32, 31, 30, 30, 30, 29, 29, 30, 30]},
-"2081":{"1stbaisakh":"2024-04-13", "daysonmonth":[31, 31, 32, 32, 31, 30, 30, 30, 29, 30, 30, 30]},
+"2081":{"1stbaisakh":"2024-04-13", "daysonmonth":[31, 32, 31, 32, 31, 30, 30, 30, 29, 30, 29, 31]},
 "2082":{"1stbaisakh":"2025-04-14", "daysonmonth":[31, 32, 31, 32, 31, 30, 30, 30, 29, 30, 30, 30]},
 "2083":{"1stbaisakh":"2026-04-14", "daysonmonth":[31, 31, 32, 31, 31, 30, 30, 30, 29, 30, 30, 30]},
 "2084":{"1stbaisakh":"2027-04-14", "daysonmonth":[31, 31, 32, 31, 31, 30, 30, 30, 29, 30, 30, 30]},
 "2085":{"1stbaisakh":"2028-04-13", "daysonmonth":[31, 32, 31, 32, 31, 31, 30, 30, 29, 30, 30, 30]},
 "2086":{"1stbaisakh":"2029-04-14", "daysonmonth":[31, 32, 31, 32, 31, 30, 30, 30, 29, 30, 30, 30]},
 "2087":{"1stbaisakh":"2030-04-14", "daysonmonth":[31, 31, 32, 31, 31, 31, 30, 30, 29, 30, 30, 30]},
 "2088":{"1stbaisakh":"2031-04-15", "daysonmonth":[30, 31, 32, 32, 30, 31, 30, 30, 29, 30, 30, 30]},
@@ -124,8 +124,8 @@
 "2093":{"1stbaisakh":"2036-04-14", "daysonmonth":[31, 32, 31, 32, 31, 30, 30, 30, 29, 30, 30, 30]},
 "2094":{"1stbaisakh":"2037-04-14", "daysonmonth":[31, 31, 32, 31, 31, 30, 30, 30, 29, 30, 30, 30]},
 "2095":{"1stbaisakh":"2038-04-14", "daysonmonth":[31, 31, 32, 31, 31, 31, 30, 29, 30, 30, 30, 30]},
 "2096":{"1stbaisakh":"2039-04-15", "daysonmonth":[30, 31, 32, 32, 31, 30, 30, 29, 30, 29, 30, 30]},
 "2097":{"1stbaisakh":"2040-04-13", "daysonmonth":[31, 32, 31, 32, 31, 30, 30, 30, 29, 30, 30, 30]},
 "2098":{"1stbaisakh":"2041-04-14", "daysonmonth":[31, 31, 32, 31, 31, 31, 29, 30, 29, 30, 30, 31]},
 "2099":{"1stbaisakh":"2042-04-14", "daysonmonth":[31, 31, 32, 31, 31, 31, 30, 29, 29, 30, 30, 30]},
-"2100":{"1stbaisakh":"2043-04-14", "daysonmonth":[31, 32, 31, 32, 30, 31, 30, 29, 30, 29, 30, 30]}}
+"2100":{"1stbaisakh":"2043-04-14", "daysonmonth":[31, 32, 31, 32, 30, 31, 30, 29, 30, 29, 30, 30]}}
```

