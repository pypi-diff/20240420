# Comparing `tmp/hjnwtx-0.1.4.tar.gz` & `tmp/hjnwtx-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hjnwtx-0.1.4.tar", last modified: Tue Mar  5 02:11:16 2024, max compression
+gzip compressed data, was "hjnwtx-0.1.5.tar", last modified: Sat Apr 20 04:49:44 2024, max compression
```

## Comparing `hjnwtx-0.1.4.tar` & `hjnwtx-0.1.5.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 hjn       (1003) hjn       (1003)        0 2024-03-05 02:11:16.714022 hjnwtx-0.1.4/
--rw-r--r--   0 hjn       (1003) hjn       (1003)      140 2024-03-05 02:11:16.714022 hjnwtx-0.1.4/PKG-INFO
--rw-rw-r--   0 hjn       (1003) hjn       (1003)       16 2024-01-03 00:18:24.000000 hjnwtx-0.1.4/README.md
-drwxrwxr-x   0 hjn       (1003) hjn       (1003)        0 2024-03-05 02:11:16.710022 hjnwtx-0.1.4/hjnwtx/
--rw-rw-r--   0 hjn       (1003) hjn       (1003)    17426 2024-01-23 02:42:51.000000 hjnwtx-0.1.4/hjnwtx/H8mess.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)      171 2024-01-03 00:18:24.000000 hjnwtx-0.1.4/hjnwtx/__init__.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)    23455 2024-01-03 00:18:24.000000 hjnwtx-0.1.4/hjnwtx/cinradHJN.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     1163 2024-01-06 12:54:45.000000 hjnwtx-0.1.4/hjnwtx/colormap.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)    11590 2024-01-03 00:18:24.000000 hjnwtx-0.1.4/hjnwtx/examMeso.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)      800 2024-01-03 00:18:24.000000 hjnwtx-0.1.4/hjnwtx/hjnDAAS.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     2927 2024-01-03 00:18:24.000000 hjnwtx-0.1.4/hjnwtx/hjnFTP.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)    12118 2024-03-05 02:10:16.000000 hjnwtx-0.1.4/hjnwtx/hjnGIS.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)      516 2024-01-03 00:18:24.000000 hjnwtx-0.1.4/hjnwtx/hjnGPU.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     2362 2024-01-03 00:18:24.000000 hjnwtx-0.1.4/hjnwtx/hjnIDW.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     2395 2024-01-03 00:18:24.000000 hjnwtx-0.1.4/hjnwtx/hjnKDTree.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     1975 2024-01-03 00:18:24.000000 hjnwtx-0.1.4/hjnwtx/hjnLAPSTransform.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     6580 2024-01-23 02:47:03.000000 hjnwtx-0.1.4/hjnwtx/hjnMiscellaneous.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     5753 2024-01-23 02:42:52.000000 hjnwtx-0.1.4/hjnwtx/hjnProj.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     1290 2024-01-03 00:18:24.000000 hjnwtx-0.1.4/hjnwtx/inotify.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     3343 2024-01-03 00:18:24.000000 hjnwtx-0.1.4/hjnwtx/matplotlibMess.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)    24653 2024-01-24 03:29:07.000000 hjnwtx-0.1.4/hjnwtx/mkNCHJN.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)    23449 2024-01-03 00:18:24.000000 hjnwtx-0.1.4/hjnwtx/newTypeRadar.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)       80 2024-01-03 00:18:24.000000 hjnwtx-0.1.4/hjnwtx/test.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     5119 2024-01-03 00:18:24.000000 hjnwtx-0.1.4/hjnwtx/tlogP.py
-drwxrwxr-x   0 hjn       (1003) hjn       (1003)        0 2024-03-05 02:11:16.714022 hjnwtx-0.1.4/hjnwtx.egg-info/
--rw-r--r--   0 hjn       (1003) hjn       (1003)      140 2024-03-05 02:11:16.000000 hjnwtx-0.1.4/hjnwtx.egg-info/PKG-INFO
--rw-rw-r--   0 hjn       (1003) hjn       (1003)      564 2024-03-05 02:11:16.000000 hjnwtx-0.1.4/hjnwtx.egg-info/SOURCES.txt
--rw-rw-r--   0 hjn       (1003) hjn       (1003)        1 2024-03-05 02:11:16.000000 hjnwtx-0.1.4/hjnwtx.egg-info/dependency_links.txt
--rw-rw-r--   0 hjn       (1003) hjn       (1003)        1 2024-01-03 00:19:56.000000 hjnwtx-0.1.4/hjnwtx.egg-info/not-zip-safe
--rw-rw-r--   0 hjn       (1003) hjn       (1003)        7 2024-03-05 02:11:16.000000 hjnwtx-0.1.4/hjnwtx.egg-info/top_level.txt
--rw-rw-r--   0 hjn       (1003) hjn       (1003)       38 2024-03-05 02:11:16.714022 hjnwtx-0.1.4/setup.cfg
--rw-rw-r--   0 hjn       (1003) hjn       (1003)      250 2024-03-05 02:11:15.000000 hjnwtx-0.1.4/setup.py
+drwxrwxr-x   0 hjn       (1003) hjn       (1003)        0 2024-04-20 04:49:44.217986 hjnwtx-0.1.5/
+-rw-r--r--   0 hjn       (1003) hjn       (1003)      140 2024-04-20 04:49:44.217986 hjnwtx-0.1.5/PKG-INFO
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)       16 2024-01-03 00:18:24.000000 hjnwtx-0.1.5/README.md
+drwxrwxr-x   0 hjn       (1003) hjn       (1003)        0 2024-04-20 04:49:44.217986 hjnwtx-0.1.5/hjnwtx/
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)    17426 2024-01-23 02:42:51.000000 hjnwtx-0.1.5/hjnwtx/H8mess.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)      171 2024-01-03 00:18:24.000000 hjnwtx-0.1.5/hjnwtx/__init__.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)    23455 2024-01-03 00:18:24.000000 hjnwtx-0.1.5/hjnwtx/cinradHJN.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     1163 2024-01-06 12:54:45.000000 hjnwtx-0.1.5/hjnwtx/colormap.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)    11590 2024-01-03 00:18:24.000000 hjnwtx-0.1.5/hjnwtx/examMeso.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)      800 2024-01-03 00:18:24.000000 hjnwtx-0.1.5/hjnwtx/hjnDAAS.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     2927 2024-01-03 00:18:24.000000 hjnwtx-0.1.5/hjnwtx/hjnFTP.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)    12118 2024-03-05 02:10:16.000000 hjnwtx-0.1.5/hjnwtx/hjnGIS.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)      516 2024-01-03 00:18:24.000000 hjnwtx-0.1.5/hjnwtx/hjnGPU.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     2362 2024-01-03 00:18:24.000000 hjnwtx-0.1.5/hjnwtx/hjnIDW.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     2395 2024-01-03 00:18:24.000000 hjnwtx-0.1.5/hjnwtx/hjnKDTree.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     1975 2024-01-03 00:18:24.000000 hjnwtx-0.1.5/hjnwtx/hjnLAPSTransform.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     2240 2024-04-20 04:49:09.000000 hjnwtx-0.1.5/hjnwtx/hjnLog.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     6580 2024-01-23 02:47:03.000000 hjnwtx-0.1.5/hjnwtx/hjnMiscellaneous.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     5753 2024-01-23 02:42:52.000000 hjnwtx-0.1.5/hjnwtx/hjnProj.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     1290 2024-01-03 00:18:24.000000 hjnwtx-0.1.5/hjnwtx/inotify.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     3343 2024-01-03 00:18:24.000000 hjnwtx-0.1.5/hjnwtx/matplotlibMess.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)    24653 2024-01-24 03:29:07.000000 hjnwtx-0.1.5/hjnwtx/mkNCHJN.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)    23449 2024-01-03 00:18:24.000000 hjnwtx-0.1.5/hjnwtx/newTypeRadar.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)       80 2024-01-03 00:18:24.000000 hjnwtx-0.1.5/hjnwtx/test.py
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)     5119 2024-01-03 00:18:24.000000 hjnwtx-0.1.5/hjnwtx/tlogP.py
+drwxrwxr-x   0 hjn       (1003) hjn       (1003)        0 2024-04-20 04:49:44.217986 hjnwtx-0.1.5/hjnwtx.egg-info/
+-rw-r--r--   0 hjn       (1003) hjn       (1003)      140 2024-04-20 04:49:44.000000 hjnwtx-0.1.5/hjnwtx.egg-info/PKG-INFO
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)      581 2024-04-20 04:49:44.000000 hjnwtx-0.1.5/hjnwtx.egg-info/SOURCES.txt
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)        1 2024-04-20 04:49:44.000000 hjnwtx-0.1.5/hjnwtx.egg-info/dependency_links.txt
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)        1 2024-01-03 00:19:56.000000 hjnwtx-0.1.5/hjnwtx.egg-info/not-zip-safe
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)        7 2024-04-20 04:49:44.000000 hjnwtx-0.1.5/hjnwtx.egg-info/top_level.txt
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)       38 2024-04-20 04:49:44.217986 hjnwtx-0.1.5/setup.cfg
+-rw-rw-r--   0 hjn       (1003) hjn       (1003)      250 2024-04-20 04:49:36.000000 hjnwtx-0.1.5/setup.py
```

### Comparing `hjnwtx-0.1.4/hjnwtx/H8mess.py` & `hjnwtx-0.1.5/hjnwtx/H8mess.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.4/hjnwtx/cinradHJN.py` & `hjnwtx-0.1.5/hjnwtx/cinradHJN.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.4/hjnwtx/colormap.py` & `hjnwtx-0.1.5/hjnwtx/colormap.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.4/hjnwtx/examMeso.py` & `hjnwtx-0.1.5/hjnwtx/examMeso.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.4/hjnwtx/hjnDAAS.py` & `hjnwtx-0.1.5/hjnwtx/hjnDAAS.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.4/hjnwtx/hjnFTP.py` & `hjnwtx-0.1.5/hjnwtx/hjnFTP.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.4/hjnwtx/hjnGIS.py` & `hjnwtx-0.1.5/hjnwtx/hjnGIS.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.4/hjnwtx/hjnGPU.py` & `hjnwtx-0.1.5/hjnwtx/hjnGPU.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.4/hjnwtx/hjnIDW.py` & `hjnwtx-0.1.5/hjnwtx/hjnIDW.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.4/hjnwtx/hjnKDTree.py` & `hjnwtx-0.1.5/hjnwtx/hjnKDTree.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.4/hjnwtx/hjnLAPSTransform.py` & `hjnwtx-0.1.5/hjnwtx/hjnLAPSTransform.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.4/hjnwtx/hjnMiscellaneous.py` & `hjnwtx-0.1.5/hjnwtx/hjnMiscellaneous.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.4/hjnwtx/hjnProj.py` & `hjnwtx-0.1.5/hjnwtx/hjnProj.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.4/hjnwtx/inotify.py` & `hjnwtx-0.1.5/hjnwtx/inotify.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.4/hjnwtx/matplotlibMess.py` & `hjnwtx-0.1.5/hjnwtx/matplotlibMess.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.4/hjnwtx/mkNCHJN.py` & `hjnwtx-0.1.5/hjnwtx/mkNCHJN.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.4/hjnwtx/newTypeRadar.py` & `hjnwtx-0.1.5/hjnwtx/newTypeRadar.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.4/hjnwtx/tlogP.py` & `hjnwtx-0.1.5/hjnwtx/tlogP.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.4/hjnwtx.egg-info/SOURCES.txt` & `hjnwtx-0.1.5/hjnwtx.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 hjnwtx/hjnDAAS.py
 hjnwtx/hjnFTP.py
 hjnwtx/hjnGIS.py
 hjnwtx/hjnGPU.py
 hjnwtx/hjnIDW.py
 hjnwtx/hjnKDTree.py
 hjnwtx/hjnLAPSTransform.py
+hjnwtx/hjnLog.py
 hjnwtx/hjnMiscellaneous.py
 hjnwtx/hjnProj.py
 hjnwtx/inotify.py
 hjnwtx/matplotlibMess.py
 hjnwtx/mkNCHJN.py
 hjnwtx/newTypeRadar.py
 hjnwtx/test.py
```

