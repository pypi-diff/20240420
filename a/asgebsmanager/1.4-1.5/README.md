# Comparing `tmp/asgebsmanager-1.4.tar.gz` & `tmp/asgebsmanager-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgebsmanager-1.4.tar", last modified: Sat Apr 20 12:37:05 2024, max compression
+gzip compressed data, was "asgebsmanager-1.5.tar", last modified: Sat Apr 20 12:41:50 2024, max compression
```

## Comparing `asgebsmanager-1.4.tar` & `asgebsmanager-1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-20 12:37:05.625118 asgebsmanager-1.4/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-20 12:37:05.624597 asgebsmanager-1.4/PKG-INFO
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-20 12:37:05.623998 asgebsmanager-1.4/asgebsmanager.egg-info/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-20 12:37:05.000000 asgebsmanager-1.4/asgebsmanager.egg-info/PKG-INFO
--rw-r--r--   0 raghavgupta   (501) staff       (20)      388 2024-04-20 12:37:05.000000 asgebsmanager-1.4/asgebsmanager.egg-info/SOURCES.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-20 12:37:05.000000 asgebsmanager-1.4/asgebsmanager.egg-info/dependency_links.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       62 2024-04-20 12:37:05.000000 asgebsmanager-1.4/asgebsmanager.egg-info/entry_points.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)      188 2024-04-20 12:37:05.000000 asgebsmanager-1.4/asgebsmanager.egg-info/requires.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       14 2024-04-20 12:37:05.000000 asgebsmanager-1.4/asgebsmanager.egg-info/top_level.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-20 12:37:05.625221 asgebsmanager-1.4/setup.cfg
--rw-r--r--   0 raghavgupta   (501) staff       (20)      807 2024-04-20 08:28:52.000000 asgebsmanager-1.4/setup.py
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-20 12:37:05.615452 asgebsmanager-1.4/src/
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-20 12:37:05.622754 asgebsmanager-1.4/src/asgebsmanager/
--rw-r--r--   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:26:40.000000 asgebsmanager-1.4/src/asgebsmanager/__init__.py
--rw-r--r--   0 raghavgupta   (501) staff       (20)     1530 2024-04-20 09:16:10.000000 asgebsmanager-1.4/src/asgebsmanager/__main__.py
--rw-r--r--   0 raghavgupta   (501) staff       (20)     9846 2024-04-20 09:14:58.000000 asgebsmanager-1.4/src/asgebsmanager/ebs_manager.py
--rw-r--r--   0 raghavgupta   (501) staff       (20)     1508 2024-04-20 09:22:56.000000 asgebsmanager-1.4/src/asgebsmanager/file_utils.py
--rw-r--r--   0 raghavgupta   (501) staff       (20)     1620 2024-04-14 10:40:38.000000 asgebsmanager-1.4/src/asgebsmanager/mds_utils.py
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-20 12:41:50.825027 asgebsmanager-1.5/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      153 2024-04-20 12:41:50.824676 asgebsmanager-1.5/PKG-INFO
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-20 12:41:50.819892 asgebsmanager-1.5/asgebsmanager.egg-info/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      153 2024-04-20 12:41:50.000000 asgebsmanager-1.5/asgebsmanager.egg-info/PKG-INFO
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      388 2024-04-20 12:41:50.000000 asgebsmanager-1.5/asgebsmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-20 12:41:50.000000 asgebsmanager-1.5/asgebsmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       62 2024-04-20 12:41:50.000000 asgebsmanager-1.5/asgebsmanager.egg-info/entry_points.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      104 2024-04-20 12:41:50.000000 asgebsmanager-1.5/asgebsmanager.egg-info/requires.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       14 2024-04-20 12:41:50.000000 asgebsmanager-1.5/asgebsmanager.egg-info/top_level.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-20 12:41:50.825147 asgebsmanager-1.5/setup.cfg
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      723 2024-04-20 12:39:49.000000 asgebsmanager-1.5/setup.py
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-20 12:41:50.816627 asgebsmanager-1.5/src/
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-20 12:41:50.823806 asgebsmanager-1.5/src/asgebsmanager/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:26:40.000000 asgebsmanager-1.5/src/asgebsmanager/__init__.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     1530 2024-04-20 09:16:10.000000 asgebsmanager-1.5/src/asgebsmanager/__main__.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     9846 2024-04-20 09:14:58.000000 asgebsmanager-1.5/src/asgebsmanager/ebs_manager.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     1508 2024-04-20 09:22:56.000000 asgebsmanager-1.5/src/asgebsmanager/file_utils.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     1620 2024-04-14 10:40:38.000000 asgebsmanager-1.5/src/asgebsmanager/mds_utils.py
```

### Comparing `asgebsmanager-1.4/setup.py` & `asgebsmanager-1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import setup, find_packages
 import os 
 
 setup(
     name = 'asgebsmanager',
-    version = "1.4",
+    version = "1.5",
     author = 'Raghav Gupta',
     description = 'AWS Asg ebs manager',
     packages = find_packages("src"),
     package_dir= {
         "asgebsmanager": os.path.join("src","asgebsmanager")
     },
     install_requires = [
-        "boto3==1.34.84",
-        "botocore==1.34.84",
-        "certifi==2024.2.2",
-        "charset-normalizer==3.3.2",
-        "idna==3.7",
-        "jmespath==1.0.1",
-        "python-dateutil==2.9.0.post0",
-        "requests==2.31.0",
-        "s3transfer==0.10.1",
-        "six==1.16.0",
+        "boto3",
+        "botocore",
+        "certifi",
+        "charset-normalizer",
+        "idna",
+        "jmespath",
+        "python-dateutil",
+        "requests",
+        "s3transfer",
+        "six",
         "urllib3"
     ],
     classifiers=[
         "Programming Language :: Python :: 3"
     ],
     entry_points = {'console_scripts': ['asgebsmanager = asgebsmanager.__main__:main'],}
 )
```

### Comparing `asgebsmanager-1.4/src/asgebsmanager/__main__.py` & `asgebsmanager-1.5/src/asgebsmanager/__main__.py`

 * *Files identical despite different names*

### Comparing `asgebsmanager-1.4/src/asgebsmanager/ebs_manager.py` & `asgebsmanager-1.5/src/asgebsmanager/ebs_manager.py`

 * *Files identical despite different names*

### Comparing `asgebsmanager-1.4/src/asgebsmanager/file_utils.py` & `asgebsmanager-1.5/src/asgebsmanager/file_utils.py`

 * *Files identical despite different names*

### Comparing `asgebsmanager-1.4/src/asgebsmanager/mds_utils.py` & `asgebsmanager-1.5/src/asgebsmanager/mds_utils.py`

 * *Files identical despite different names*

