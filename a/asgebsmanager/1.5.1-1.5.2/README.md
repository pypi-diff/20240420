# Comparing `tmp/asgebsmanager-1.5.1.tar.gz` & `tmp/asgebsmanager-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgebsmanager-1.5.1.tar", last modified: Sat Apr 20 13:15:02 2024, max compression
+gzip compressed data, was "asgebsmanager-1.5.2.tar", last modified: Sat Apr 20 13:21:04 2024, max compression
```

## Comparing `asgebsmanager-1.5.1.tar` & `asgebsmanager-1.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-20 13:15:02.066556 asgebsmanager-1.5.1/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      424 2024-04-20 13:15:02.065734 asgebsmanager-1.5.1/PKG-INFO
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-20 13:15:02.065085 asgebsmanager-1.5.1/asgebsmanager.egg-info/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      424 2024-04-20 13:15:01.000000 asgebsmanager-1.5.1/asgebsmanager.egg-info/PKG-INFO
--rw-r--r--   0 raghavgupta   (501) staff       (20)      388 2024-04-20 13:15:01.000000 asgebsmanager-1.5.1/asgebsmanager.egg-info/SOURCES.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-20 13:15:01.000000 asgebsmanager-1.5.1/asgebsmanager.egg-info/dependency_links.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       62 2024-04-20 13:15:01.000000 asgebsmanager-1.5.1/asgebsmanager.egg-info/entry_points.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)      104 2024-04-20 13:15:01.000000 asgebsmanager-1.5.1/asgebsmanager.egg-info/requires.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       14 2024-04-20 13:15:01.000000 asgebsmanager-1.5.1/asgebsmanager.egg-info/top_level.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-20 13:15:02.066728 asgebsmanager-1.5.1/setup.cfg
--rw-r--r--   0 raghavgupta   (501) staff       (20)      725 2024-04-20 13:14:45.000000 asgebsmanager-1.5.1/setup.py
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-20 13:15:02.058096 asgebsmanager-1.5.1/src/
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-20 13:15:02.064139 asgebsmanager-1.5.1/src/asgebsmanager/
--rw-r--r--   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:26:40.000000 asgebsmanager-1.5.1/src/asgebsmanager/__init__.py
--rw-r--r--   0 raghavgupta   (501) staff       (20)     1530 2024-04-20 09:16:10.000000 asgebsmanager-1.5.1/src/asgebsmanager/__main__.py
--rw-r--r--   0 raghavgupta   (501) staff       (20)     9912 2024-04-20 13:13:37.000000 asgebsmanager-1.5.1/src/asgebsmanager/ebs_manager.py
--rw-r--r--   0 raghavgupta   (501) staff       (20)     1468 2024-04-20 13:14:41.000000 asgebsmanager-1.5.1/src/asgebsmanager/file_utils.py
--rw-r--r--   0 raghavgupta   (501) staff       (20)     1620 2024-04-14 10:40:38.000000 asgebsmanager-1.5.1/src/asgebsmanager/mds_utils.py
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-20 13:21:04.706062 asgebsmanager-1.5.2/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      424 2024-04-20 13:21:04.705426 asgebsmanager-1.5.2/PKG-INFO
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-20 13:21:04.704570 asgebsmanager-1.5.2/asgebsmanager.egg-info/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      424 2024-04-20 13:21:04.000000 asgebsmanager-1.5.2/asgebsmanager.egg-info/PKG-INFO
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      388 2024-04-20 13:21:04.000000 asgebsmanager-1.5.2/asgebsmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-20 13:21:04.000000 asgebsmanager-1.5.2/asgebsmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       62 2024-04-20 13:21:04.000000 asgebsmanager-1.5.2/asgebsmanager.egg-info/entry_points.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      104 2024-04-20 13:21:04.000000 asgebsmanager-1.5.2/asgebsmanager.egg-info/requires.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       14 2024-04-20 13:21:04.000000 asgebsmanager-1.5.2/asgebsmanager.egg-info/top_level.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-20 13:21:04.706408 asgebsmanager-1.5.2/setup.cfg
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      725 2024-04-20 13:20:29.000000 asgebsmanager-1.5.2/setup.py
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-20 13:21:04.697242 asgebsmanager-1.5.2/src/
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-20 13:21:04.703493 asgebsmanager-1.5.2/src/asgebsmanager/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:26:40.000000 asgebsmanager-1.5.2/src/asgebsmanager/__init__.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     1530 2024-04-20 09:16:10.000000 asgebsmanager-1.5.2/src/asgebsmanager/__main__.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     9912 2024-04-20 13:20:37.000000 asgebsmanager-1.5.2/src/asgebsmanager/ebs_manager.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     1468 2024-04-20 13:14:41.000000 asgebsmanager-1.5.2/src/asgebsmanager/file_utils.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     1620 2024-04-14 10:40:38.000000 asgebsmanager-1.5.2/src/asgebsmanager/mds_utils.py
```

### Comparing `asgebsmanager-1.5.1/setup.py` & `asgebsmanager-1.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os 
 
 setup(
     name = 'asgebsmanager',
-    version = "1.5.1",
+    version = "1.5.2",
     author = 'Raghav Gupta',
     description = 'AWS Asg ebs manager',
     packages = find_packages("src"),
     package_dir= {
         "asgebsmanager": os.path.join("src","asgebsmanager")
     },
     install_requires = [
```

### Comparing `asgebsmanager-1.5.1/src/asgebsmanager/__main__.py` & `asgebsmanager-1.5.2/src/asgebsmanager/__main__.py`

 * *Files identical despite different names*

### Comparing `asgebsmanager-1.5.1/src/asgebsmanager/ebs_manager.py` & `asgebsmanager-1.5.2/src/asgebsmanager/ebs_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         # only if 'force' is enabled
         # check the difference in the volume configuration and if there is a diff, 
         # create a new volume from the snapshot of the existing volume and
         # delete the older volume 
         if volume_id and args.force:
             volume = asg_ebs_manager.describe_volume(volume_id)
             snapshot_id = None
-            if volume['Size'] > args.size or volume['Iops'] != args.iops or volume['Throughput'] != args.throughput or az_diff:
+            if volume['Size'] < args.size or volume['Iops'] != args.iops or volume['Throughput'] != args.throughput or az_diff:
                 snapshot_id = asg_ebs_manager.create_snapshot(volume_id)
                 snapshot = asg_ebs_manager.describe_snapshot(snapshot_id)
                 max_retries = args.check_timeout
                 while snapshot['State'] != 'completed' and max_retries > 0:
                     sleep(60)
                     max_retries -= 1
                     snapshot = asg_ebs_manager.describe_snapshot(snapshot_id)
```

### Comparing `asgebsmanager-1.5.1/src/asgebsmanager/file_utils.py` & `asgebsmanager-1.5.2/src/asgebsmanager/file_utils.py`

 * *Files identical despite different names*

### Comparing `asgebsmanager-1.5.1/src/asgebsmanager/mds_utils.py` & `asgebsmanager-1.5.2/src/asgebsmanager/mds_utils.py`

 * *Files identical despite different names*

