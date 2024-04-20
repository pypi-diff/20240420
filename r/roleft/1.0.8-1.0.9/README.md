# Comparing `tmp/roleft-1.0.8.tar.gz` & `tmp/roleft-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roleft-1.0.8.tar", last modified: Wed Aug  9 07:45:24 2023, max compression
+gzip compressed data, was "roleft-1.0.9.tar", last modified: Wed Aug  9 07:52:50 2023, max compression
```

## Comparing `roleft-1.0.8.tar` & `roleft-1.0.9.tar`

### file list

```diff
@@ -1,34 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-09 07:45:24.112946 roleft-1.0.8/
--rw-rw-rw-   0        0        0      311 2023-08-09 07:45:24.111946 roleft-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      484 2023-08-09 07:45:06.000000 roleft-1.0.8/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-08-09 07:45:24.066965 roleft-1.0.8/roleft/
-drwxrwxrwx   0        0        0        0 2023-08-09 07:45:24.075958 roleft-1.0.8/roleft/Entities/
--rw-rw-rw-   0        0        0      244 2023-08-09 06:14:27.000000 roleft-1.0.8/roleft/Entities/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-09 07:45:24.084955 roleft-1.0.8/roleft/Enumerable/
--rw-rw-rw-   0        0        0      664 2023-08-09 06:41:16.000000 roleft-1.0.8/roleft/Enumerable/RoleftDateTime.py
--rw-rw-rw-   0        0        0     1280 2023-08-09 06:31:11.000000 roleft-1.0.8/roleft/Enumerable/RoleftDict.py
--rw-rw-rw-   0        0        0     3597 2023-08-09 06:27:32.000000 roleft-1.0.8/roleft/Enumerable/RoleftList.py
--rw-rw-rw-   0        0        0       60 2023-08-09 06:30:52.000000 roleft-1.0.8/roleft/Enumerable/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-09 07:45:24.092952 roleft-1.0.8/roleft/Utilities/
--rw-rw-rw-   0        0        0     1434 2023-07-21 15:48:29.000000 roleft-1.0.8/roleft/Utilities/AU.py
--rw-rw-rw-   0        0        0     1576 2023-08-09 07:12:28.000000 roleft-1.0.8/roleft/Utilities/CU.py
--rw-rw-rw-   0        0        0      134 2023-07-21 15:48:42.000000 roleft-1.0.8/roleft/Utilities/HU.py
--rw-rw-rw-   0        0        0     2516 2023-08-09 06:18:33.000000 roleft-1.0.8/roleft/Utilities/ListU.py
--rw-rw-rw-   0        0        0        0 2023-07-21 15:51:50.000000 roleft-1.0.8/roleft/Utilities/__init__.py
--rw-rw-rw-   0        0        0      192 2023-08-09 07:23:48.000000 roleft-1.0.8/roleft/__init__.py
--rw-rw-rw-   0        0        0      118 2023-08-09 06:20:37.000000 roleft-1.0.8/roleft/entry.py
-drwxrwxrwx   0        0        0        0 2023-08-09 07:45:24.071961 roleft-1.0.8/roleft.egg-info/
--rw-rw-rw-   0        0        0      311 2023-08-09 07:45:24.000000 roleft-1.0.8/roleft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      583 2023-08-09 07:45:24.000000 roleft-1.0.8/roleft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-09 07:45:24.000000 roleft-1.0.8/roleft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-08-09 07:45:24.000000 roleft-1.0.8/roleft.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-09 07:45:24.112946 roleft-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-09 07:45:24.108947 roleft-1.0.8/tests/
--rw-rw-rw-   0        0        0      624 2023-07-28 10:38:35.000000 roleft-1.0.8/tests/test_1.py
--rw-rw-rw-   0        0        0     1290 2023-08-09 06:31:34.000000 roleft-1.0.8/tests/test_2.py
--rw-rw-rw-   0        0        0      843 2023-07-26 16:08:39.000000 roleft-1.0.8/tests/test_2copy.py
--rw-rw-rw-   0        0        0      879 2023-08-09 06:31:44.000000 roleft-1.0.8/tests/test_3.py
--rw-rw-rw-   0        0        0      898 2023-08-09 06:17:43.000000 roleft-1.0.8/tests/test_4.py
--rw-rw-rw-   0        0        0      937 2023-08-09 06:17:47.000000 roleft-1.0.8/tests/test_5.py
--rw-rw-rw-   0        0        0     1162 2023-07-28 10:17:06.000000 roleft-1.0.8/tests/test_6.py
--rw-rw-rw-   0        0        0      854 2023-07-28 10:06:55.000000 roleft-1.0.8/tests/test_7.py
+-rw-r--r--   0        0        0      423 2023-08-09 07:52:50.514332 roleft-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      244 2023-08-09 06:14:27.029672 roleft-1.0.9/roleft/Entities/__init__.py
+-rw-r--r--   0        0        0      664 2023-08-09 06:41:16.530379 roleft-1.0.9/roleft/Enumerable/RoleftDateTime.py
+-rw-r--r--   0        0        0     1280 2023-08-09 06:31:11.254798 roleft-1.0.9/roleft/Enumerable/RoleftDict.py
+-rw-r--r--   0        0        0     3597 2023-08-09 06:27:32.270724 roleft-1.0.9/roleft/Enumerable/RoleftList.py
+-rw-r--r--   0        0        0       60 2023-08-09 06:30:52.354087 roleft-1.0.9/roleft/Enumerable/__init__.py
+-rw-r--r--   0        0        0     1434 2023-07-21 15:48:29.156603 roleft-1.0.9/roleft/Utilities/AU.py
+-rw-r--r--   0        0        0     1576 2023-08-09 07:12:28.231683 roleft-1.0.9/roleft/Utilities/CU.py
+-rw-r--r--   0        0        0      134 2023-07-21 15:48:42.676876 roleft-1.0.9/roleft/Utilities/HU.py
+-rw-r--r--   0        0        0     2516 2023-08-09 06:18:33.109476 roleft-1.0.9/roleft/Utilities/ListU.py
+-rw-r--r--   0        0        0        0 2023-07-21 15:51:50.240498 roleft-1.0.9/roleft/Utilities/__init__.py
+-rw-r--r--   0        0        0      192 2023-08-09 07:23:48.571242 roleft-1.0.9/roleft/__init__.py
+-rw-r--r--   0        0        0      118 2023-08-09 06:20:37.751616 roleft-1.0.9/roleft/entry.py
+-rw-r--r--   0        0        0      624 2023-07-28 10:38:35.541060 roleft-1.0.9/tests/test_1.py
+-rw-r--r--   0        0        0     1290 2023-08-09 06:31:34.738900 roleft-1.0.9/tests/test_2.py
+-rw-r--r--   0        0        0      843 2023-07-26 16:08:39.520041 roleft-1.0.9/tests/test_2copy.py
+-rw-r--r--   0        0        0      879 2023-08-09 06:31:44.629728 roleft-1.0.9/tests/test_3.py
+-rw-r--r--   0        0        0      898 2023-08-09 06:17:43.995520 roleft-1.0.9/tests/test_4.py
+-rw-r--r--   0        0        0      937 2023-08-09 06:17:47.130296 roleft-1.0.9/tests/test_5.py
+-rw-r--r--   0        0        0     1162 2023-07-28 10:17:06.342522 roleft-1.0.9/tests/test_6.py
+-rw-r--r--   0        0        0      854 2023-07-28 10:06:55.112561 roleft-1.0.9/tests/test_7.py
+-rw-r--r--   0        0        0      302 1970-01-01 00:00:00.000000 roleft-1.0.9/PKG-INFO
```

### Comparing `roleft-1.0.8/roleft/Enumerable/RoleftDateTime.py` & `roleft-1.0.9/roleft/Enumerable/RoleftDateTime.py`

 * *Files identical despite different names*

### Comparing `roleft-1.0.8/roleft/Enumerable/RoleftDict.py` & `roleft-1.0.9/roleft/Enumerable/RoleftDict.py`

 * *Files identical despite different names*

### Comparing `roleft-1.0.8/roleft/Enumerable/RoleftList.py` & `roleft-1.0.9/roleft/Enumerable/RoleftList.py`

 * *Files identical despite different names*

### Comparing `roleft-1.0.8/roleft/Utilities/AU.py` & `roleft-1.0.9/roleft/Utilities/AU.py`

 * *Files identical despite different names*

### Comparing `roleft-1.0.8/roleft/Utilities/CU.py` & `roleft-1.0.9/roleft/Utilities/CU.py`

 * *Files identical despite different names*

### Comparing `roleft-1.0.8/roleft/Utilities/ListU.py` & `roleft-1.0.9/roleft/Utilities/ListU.py`

 * *Files identical despite different names*

### Comparing `roleft-1.0.8/tests/test_1.py` & `roleft-1.0.9/tests/test_1.py`

 * *Files identical despite different names*

### Comparing `roleft-1.0.8/tests/test_2.py` & `roleft-1.0.9/tests/test_2.py`

 * *Files identical despite different names*

### Comparing `roleft-1.0.8/tests/test_2copy.py` & `roleft-1.0.9/tests/test_2copy.py`

 * *Files identical despite different names*

### Comparing `roleft-1.0.8/tests/test_3.py` & `roleft-1.0.9/tests/test_3.py`

 * *Files identical despite different names*

### Comparing `roleft-1.0.8/tests/test_4.py` & `roleft-1.0.9/tests/test_4.py`

 * *Files identical despite different names*

### Comparing `roleft-1.0.8/tests/test_5.py` & `roleft-1.0.9/tests/test_5.py`

 * *Files identical despite different names*

### Comparing `roleft-1.0.8/tests/test_6.py` & `roleft-1.0.9/tests/test_6.py`

 * *Files identical despite different names*

### Comparing `roleft-1.0.8/tests/test_7.py` & `roleft-1.0.9/tests/test_7.py`

 * *Files identical despite different names*

