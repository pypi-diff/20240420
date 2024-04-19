# Comparing `tmp/rent_counter-0.4.0.tar.gz` & `tmp/rent_counter-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rent_counter-0.4.0.tar", last modified: Fri Apr 19 16:59:49 2024, max compression
+gzip compressed data, was "rent_counter-0.5.0.tar", last modified: Fri Apr 19 23:05:31 2024, max compression
```

## Comparing `rent_counter-0.4.0.tar` & `rent_counter-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 16:59:49.198145 rent_counter-0.4.0/
--rw-rw-rw-   0        0        0     2001 2024-04-19 16:59:49.193148 rent_counter-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1465 2024-04-19 07:51:08.000000 rent_counter-0.4.0/README.md
--rw-rw-rw-   0        0        0      451 2024-04-19 07:51:08.000000 rent_counter-0.4.0/countdown.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:59:49.191150 rent_counter-0.4.0/rent_counter.egg-info/
--rw-rw-rw-   0        0        0     2001 2024-04-19 16:59:48.000000 rent_counter-0.4.0/rent_counter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2024-04-19 16:59:49.000000 rent_counter-0.4.0/rent_counter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 16:59:49.000000 rent_counter-0.4.0/rent_counter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-19 16:59:49.000000 rent_counter-0.4.0/rent_counter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 16:59:49.199145 rent_counter-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-04-19 16:56:47.000000 rent_counter-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:59:49.186153 rent_counter-0.4.0/tests/
--rw-rw-rw-   0        0        0     1119 2024-04-19 12:54:47.000000 rent_counter-0.4.0/tests/test_countdown.py
+drwxrwxrwx   0        0        0        0 2024-04-19 23:05:31.598233 rent_counter-0.5.0/
+-rw-rw-rw-   0        0        0     2001 2024-04-19 23:05:31.593233 rent_counter-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1465 2024-04-19 07:51:08.000000 rent_counter-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 23:05:31.502540 rent_counter-0.5.0/countf/
+-rw-rw-rw-   0        0        0        2 2024-04-19 14:08:38.000000 rent_counter-0.5.0/countf/__init__.py
+-rw-rw-rw-   0        0        0      451 2024-04-19 07:51:08.000000 rent_counter-0.5.0/countf/countdown.py
+drwxrwxrwx   0        0        0        0 2024-04-19 23:05:31.589999 rent_counter-0.5.0/rent_counter.egg-info/
+-rw-rw-rw-   0        0        0     2001 2024-04-19 23:05:31.000000 rent_counter-0.5.0/rent_counter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-04-19 23:05:31.000000 rent_counter-0.5.0/rent_counter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 23:05:31.000000 rent_counter-0.5.0/rent_counter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-19 23:05:31.000000 rent_counter-0.5.0/rent_counter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 23:05:31.599230 rent_counter-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      845 2024-04-19 23:01:45.000000 rent_counter-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 23:05:31.586001 rent_counter-0.5.0/tests/
+-rw-rw-rw-   0        0        0     1126 2024-04-19 22:54:29.000000 rent_counter-0.5.0/tests/test_countdown.py
```

### Comparing `rent_counter-0.4.0/PKG-INFO` & `rent_counter-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rent_counter
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python library for managing rent expiration countdowns
 Home-page: https://github.com/Erickadikah/count
 Author: Erick Adikah
 Author-email: your.email@example.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rent_counter-0.4.0/README.md` & `rent_counter-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `rent_counter-0.4.0/rent_counter.egg-info/PKG-INFO` & `rent_counter-0.5.0/rent_counter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rent_counter
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python library for managing rent expiration countdowns
 Home-page: https://github.com/Erickadikah/count
 Author: Erick Adikah
 Author-email: your.email@example.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rent_counter-0.4.0/setup.py` & `rent_counter-0.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rent_counter',
-    version='0.4.0',
-    py_modules=['countdown'],  # Include countdown.py as a module
+    version='0.5.0',
+    py_modules=['countf.countdown'],  # Include countdown.py as a module inside the countf folder
     include_package_data=True,
     description='A Python library for managing rent expiration countdowns',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Erick Adikah',
     author_email='your.email@example.com',
     license='MIT',
```

### Comparing `rent_counter-0.4.0/tests/test_countdown.py` & `rent_counter-0.5.0/tests/test_countdown.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 from datetime import datetime, timedelta
-from countdown import calculate_remaining_time
+from countf.countdown import calculate_remaining_time
 
 class TestCountdown(unittest.TestCase):
     def test_remaining_time_future(self):
         end_date = datetime.now() + timedelta(days=7)  # End date 7 days from now
         remaining_time = calculate_remaining_time(end_date)
         self.assertIsInstance(remaining_time, timedelta)
         self.assertGreaterEqual(remaining_time.total_seconds(), 0)
```

