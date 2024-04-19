# Comparing `tmp/rent_counter-0.3.0.tar.gz` & `tmp/rent_counter-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rent_counter-0.3.0.tar", last modified: Fri Apr 19 14:14:37 2024, max compression
+gzip compressed data, was "rent_counter-0.4.0.tar", last modified: Fri Apr 19 16:59:49 2024, max compression
```

## Comparing `rent_counter-0.3.0.tar` & `rent_counter-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 14:14:37.543629 rent_counter-0.3.0/
--rw-rw-rw-   0        0        0     2001 2024-04-19 14:14:37.537631 rent_counter-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1465 2024-04-19 07:51:08.000000 rent_counter-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 14:14:37.534633 rent_counter-0.3.0/rent_counter.egg-info/
--rw-rw-rw-   0        0        0     2001 2024-04-19 14:14:37.000000 rent_counter-0.3.0/rent_counter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-04-19 14:14:37.000000 rent_counter-0.3.0/rent_counter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 14:14:37.000000 rent_counter-0.3.0/rent_counter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 14:14:37.000000 rent_counter-0.3.0/rent_counter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 14:14:37.544627 rent_counter-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      777 2024-04-19 14:13:35.000000 rent_counter-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:14:37.521220 rent_counter-0.3.0/tests/
--rw-rw-rw-   0        0        0     1119 2024-04-19 12:54:47.000000 rent_counter-0.3.0/tests/test_countdown.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:59:49.198145 rent_counter-0.4.0/
+-rw-rw-rw-   0        0        0     2001 2024-04-19 16:59:49.193148 rent_counter-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1465 2024-04-19 07:51:08.000000 rent_counter-0.4.0/README.md
+-rw-rw-rw-   0        0        0      451 2024-04-19 07:51:08.000000 rent_counter-0.4.0/countdown.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:59:49.191150 rent_counter-0.4.0/rent_counter.egg-info/
+-rw-rw-rw-   0        0        0     2001 2024-04-19 16:59:48.000000 rent_counter-0.4.0/rent_counter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2024-04-19 16:59:49.000000 rent_counter-0.4.0/rent_counter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 16:59:49.000000 rent_counter-0.4.0/rent_counter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-19 16:59:49.000000 rent_counter-0.4.0/rent_counter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 16:59:49.199145 rent_counter-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      813 2024-04-19 16:56:47.000000 rent_counter-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:59:49.186153 rent_counter-0.4.0/tests/
+-rw-rw-rw-   0        0        0     1119 2024-04-19 12:54:47.000000 rent_counter-0.4.0/tests/test_countdown.py
```

### Comparing `rent_counter-0.3.0/PKG-INFO` & `rent_counter-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rent_counter
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python library for managing rent expiration countdowns
 Home-page: https://github.com/Erickadikah/count
 Author: Erick Adikah
 Author-email: your.email@example.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rent_counter-0.3.0/README.md` & `rent_counter-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `rent_counter-0.3.0/rent_counter.egg-info/PKG-INFO` & `rent_counter-0.4.0/rent_counter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rent_counter
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python library for managing rent expiration countdowns
 Home-page: https://github.com/Erickadikah/count
 Author: Erick Adikah
 Author-email: your.email@example.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rent_counter-0.3.0/tests/test_countdown.py` & `rent_counter-0.4.0/tests/test_countdown.py`

 * *Files identical despite different names*

