# Comparing `tmp/yctmodel-5.3.19.tar.gz` & `tmp/yctmodel-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yctmodel-5.3.19.tar", last modified: Tue Nov 28 13:57:30 2023, max compression
+gzip compressed data, was "yctmodel-5.4.0.tar", last modified: Sat Apr 20 12:57:31 2024, max compression
```

## Comparing `yctmodel-5.3.19.tar` & `yctmodel-5.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 yc4923    (1000) yc4923    (1000)        0 2023-11-28 13:57:30.506916 yctmodel-5.3.19/
--rw-r--r--   0 yc4923    (1000) yc4923    (1000)     1064 2023-11-21 10:42:36.000000 yctmodel-5.3.19/LICENSE
--rw-r--r--   0 yc4923    (1000) yc4923    (1000)       33 2023-11-21 17:42:56.000000 yctmodel-5.3.19/MANIFEST.in
--rw-r--r--   0 yc4923    (1000) yc4923    (1000)     3413 2023-11-28 13:57:30.506916 yctmodel-5.3.19/PKG-INFO
--rw-r--r--   0 yc4923    (1000) yc4923    (1000)     3147 2023-11-28 13:57:22.000000 yctmodel-5.3.19/README.md
--rw-r--r--   0 yc4923    (1000) yc4923    (1000)       38 2023-11-28 13:57:30.506916 yctmodel-5.3.19/setup.cfg
--rw-r--r--   0 yc4923    (1000) yc4923    (1000)      515 2023-11-28 13:57:27.000000 yctmodel-5.3.19/setup.py
-drwxr-xr-x   0 yc4923    (1000) yc4923    (1000)        0 2023-11-28 13:57:30.506916 yctmodel-5.3.19/yctmodel/
--rw-r--r--   0 yc4923    (1000) yc4923    (1000)      108 2023-11-22 16:00:47.000000 yctmodel-5.3.19/yctmodel/__init__.py
--rw-r--r--   0 yc4923    (1000) yc4923    (1000)    21952 2023-11-28 13:47:14.000000 yctmodel-5.3.19/yctmodel/yctmodel.py
-drwxr-xr-x   0 yc4923    (1000) yc4923    (1000)        0 2023-11-28 13:57:30.506916 yctmodel-5.3.19/yctmodel.egg-info/
--rw-r--r--   0 yc4923    (1000) yc4923    (1000)     3413 2023-11-28 13:57:30.000000 yctmodel-5.3.19/yctmodel.egg-info/PKG-INFO
--rw-r--r--   0 yc4923    (1000) yc4923    (1000)      239 2023-11-28 13:57:30.000000 yctmodel-5.3.19/yctmodel.egg-info/SOURCES.txt
--rw-r--r--   0 yc4923    (1000) yc4923    (1000)        1 2023-11-28 13:57:30.000000 yctmodel-5.3.19/yctmodel.egg-info/dependency_links.txt
--rw-r--r--   0 yc4923    (1000) yc4923    (1000)       59 2023-11-28 13:57:30.000000 yctmodel-5.3.19/yctmodel.egg-info/requires.txt
--rw-r--r--   0 yc4923    (1000) yc4923    (1000)        9 2023-11-28 13:57:30.000000 yctmodel-5.3.19/yctmodel.egg-info/top_level.txt
+drwxr-xr-x   0 yc4923    (1000) yc4923    (1000)        0 2024-04-20 12:57:31.626521 yctmodel-5.4.0/
+-rw-r--r--   0 yc4923    (1000) yc4923    (1000)     1064 2023-11-21 10:42:36.000000 yctmodel-5.4.0/LICENSE
+-rw-r--r--   0 yc4923    (1000) yc4923    (1000)       33 2023-11-21 17:42:56.000000 yctmodel-5.4.0/MANIFEST.in
+-rw-r--r--   0 yc4923    (1000) yc4923    (1000)     3412 2024-04-20 12:57:31.626521 yctmodel-5.4.0/PKG-INFO
+-rw-r--r--   0 yc4923    (1000) yc4923    (1000)     3147 2023-11-28 13:57:22.000000 yctmodel-5.4.0/README.md
+-rw-r--r--   0 yc4923    (1000) yc4923    (1000)       38 2024-04-20 12:57:31.626521 yctmodel-5.4.0/setup.cfg
+-rw-r--r--   0 yc4923    (1000) yc4923    (1000)      514 2024-04-20 12:55:40.000000 yctmodel-5.4.0/setup.py
+drwxr-xr-x   0 yc4923    (1000) yc4923    (1000)        0 2024-04-20 12:57:31.626521 yctmodel-5.4.0/yctmodel/
+-rw-r--r--   0 yc4923    (1000) yc4923    (1000)      108 2023-11-22 16:00:47.000000 yctmodel-5.4.0/yctmodel/__init__.py
+-rw-r--r--   0 yc4923    (1000) yc4923    (1000)    21952 2023-11-28 13:47:14.000000 yctmodel-5.4.0/yctmodel/yctmodel.py
+drwxr-xr-x   0 yc4923    (1000) yc4923    (1000)        0 2024-04-20 12:57:31.626521 yctmodel-5.4.0/yctmodel.egg-info/
+-rw-r--r--   0 yc4923    (1000) yc4923    (1000)     3412 2024-04-20 12:57:31.000000 yctmodel-5.4.0/yctmodel.egg-info/PKG-INFO
+-rw-r--r--   0 yc4923    (1000) yc4923    (1000)      239 2024-04-20 12:57:31.000000 yctmodel-5.4.0/yctmodel.egg-info/SOURCES.txt
+-rw-r--r--   0 yc4923    (1000) yc4923    (1000)        1 2024-04-20 12:57:31.000000 yctmodel-5.4.0/yctmodel.egg-info/dependency_links.txt
+-rw-r--r--   0 yc4923    (1000) yc4923    (1000)       59 2024-04-20 12:57:31.000000 yctmodel-5.4.0/yctmodel.egg-info/requires.txt
+-rw-r--r--   0 yc4923    (1000) yc4923    (1000)        9 2024-04-20 12:57:31.000000 yctmodel-5.4.0/yctmodel.egg-info/top_level.txt
```

### Comparing `yctmodel-5.3.19/LICENSE` & `yctmodel-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yctmodel-5.3.19/PKG-INFO` & `yctmodel-5.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yctmodel
-Version: 5.3.19
+Version: 5.4.0
 Summary: ModelSelector automates ensemble creation, added AutoTuner.
 Home-page: https://github.com/gems-yc4923/thames.git
 Author: yc4923
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `yctmodel-5.3.19/README.md` & `yctmodel-5.4.0/README.md`

 * *Files identical despite different names*

### Comparing `yctmodel-5.3.19/setup.py` & `yctmodel-5.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='yctmodel',
-    version='5.3.19',
+    version='5.4.0',
     packages=['yctmodel'],
     description="ModelSelector automates ensemble creation, added AutoTuner.",
     long_description_content_type="text/markdown",
     long_description=open("README.md").read(),
     install_requires=['scikit-learn','pandas','matplotlib',
                         'numpy','scipy','seaborn','xgboost',],
     url='https://github.com/gems-yc4923/thames.git',
```

### Comparing `yctmodel-5.3.19/yctmodel/yctmodel.py` & `yctmodel-5.4.0/yctmodel/yctmodel.py`

 * *Files identical despite different names*

### Comparing `yctmodel-5.3.19/yctmodel.egg-info/PKG-INFO` & `yctmodel-5.4.0/yctmodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yctmodel
-Version: 5.3.19
+Version: 5.4.0
 Summary: ModelSelector automates ensemble creation, added AutoTuner.
 Home-page: https://github.com/gems-yc4923/thames.git
 Author: yc4923
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

