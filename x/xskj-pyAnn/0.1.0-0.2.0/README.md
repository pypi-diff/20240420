# Comparing `tmp/xskj-pyAnn-0.1.0.tar.gz` & `tmp/xskj-pyAnn-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xskj-pyAnn-0.1.0.tar", last modified: Thu Apr 18 06:23:41 2024, max compression
+gzip compressed data, was "xskj-pyAnn-0.2.0.tar", last modified: Sat Apr 20 14:28:36 2024, max compression
```

## Comparing `xskj-pyAnn-0.1.0.tar` & `xskj-pyAnn-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 06:23:41.283590 xskj-pyAnn-0.1.0/
--rw-rw-rw-   0        0        0     1060 2024-04-12 15:20:56.000000 xskj-pyAnn-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       26 2024-04-12 15:20:56.000000 xskj-pyAnn-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      711 2024-04-18 06:23:41.282590 xskj-pyAnn-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       23 2024-04-18 06:16:00.000000 xskj-pyAnn-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 06:23:41.251589 xskj-pyAnn-0.1.0/pyANN/
--rw-rw-rw-   0        0        0       20 2024-04-12 15:20:56.000000 xskj-pyAnn-0.1.0/pyANN/__init__.py
--rw-rw-rw-   0        0        0      352 2024-04-12 15:20:56.000000 xskj-pyAnn-0.1.0/pyANN/__version__.py
--rw-rw-rw-   0        0        0       42 2024-04-18 06:11:13.000000 xskj-pyAnn-0.1.0/pyANN/core.py
--rw-rw-rw-   0        0        0       42 2024-04-14 20:55:51.000000 xskj-pyAnn-0.1.0/pyANN/test.py
--rw-rw-rw-   0        0        0       42 2024-04-18 06:23:41.283590 xskj-pyAnn-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     3785 2024-04-18 06:22:21.000000 xskj-pyAnn-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 06:23:41.277591 xskj-pyAnn-0.1.0/xskj_pyAnn.egg-info/
--rw-rw-rw-   0        0        0      711 2024-04-18 06:23:41.000000 xskj-pyAnn-0.1.0/xskj_pyAnn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2024-04-18 06:23:41.000000 xskj-pyAnn-0.1.0/xskj_pyAnn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 06:23:41.000000 xskj-pyAnn-0.1.0/xskj_pyAnn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-18 06:23:41.000000 xskj-pyAnn-0.1.0/xskj_pyAnn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 14:28:36.034370 xskj-pyAnn-0.2.0/
+-rw-rw-rw-   0        0        0     1060 2024-04-12 15:20:56.000000 xskj-pyAnn-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       26 2024-04-12 15:20:56.000000 xskj-pyAnn-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      759 2024-04-20 14:28:36.034370 xskj-pyAnn-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-20 14:25:51.000000 xskj-pyAnn-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 14:28:36.024169 xskj-pyAnn-0.2.0/pyANN/
+-rw-rw-rw-   0        0        0       20 2024-04-12 15:20:56.000000 xskj-pyAnn-0.2.0/pyANN/__init__.py
+-rw-rw-rw-   0        0        0      352 2024-04-12 15:20:56.000000 xskj-pyAnn-0.2.0/pyANN/__version__.py
+-rw-rw-rw-   0        0        0       42 2024-04-18 06:11:13.000000 xskj-pyAnn-0.2.0/pyANN/core.py
+-rw-rw-rw-   0        0        0       42 2024-04-14 20:55:51.000000 xskj-pyAnn-0.2.0/pyANN/test.py
+-rw-rw-rw-   0        0        0       42 2024-04-20 14:28:36.034370 xskj-pyAnn-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     3785 2024-04-20 14:25:25.000000 xskj-pyAnn-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:28:36.034370 xskj-pyAnn-0.2.0/xskj_pyAnn.egg-info/
+-rw-rw-rw-   0        0        0      759 2024-04-20 14:28:35.000000 xskj-pyAnn-0.2.0/xskj_pyAnn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2024-04-20 14:28:35.000000 xskj-pyAnn-0.2.0/xskj_pyAnn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 14:28:35.000000 xskj-pyAnn-0.2.0/xskj_pyAnn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-20 14:28:35.000000 xskj-pyAnn-0.2.0/xskj_pyAnn.egg-info/top_level.txt
```

### Comparing `xskj-pyAnn-0.1.0/LICENSE` & `xskj-pyAnn-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xskj-pyAnn-0.1.0/PKG-INFO` & `xskj-pyAnn-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: xskj-pyAnn
-Version: 0.1.0
+Version: 0.2.0
 Summary: 不依赖于框架的神经网络实现代码
 Home-page: https://github.com/gnu-xiaosong/ANN
 Author: xskj
 Author-email: 1829134124@qq.com
 License: MIT
 Description: 
         ## "# ANN" 
-        "# ANN" 
+        
+        
+        
+        v0.2.0  增加了多分类
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `xskj-pyAnn-0.1.0/setup.py` & `xskj-pyAnn-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'xskj-pyAnn'
 DESCRIPTION = '不依赖于框架的神经网络实现代码'
 URL = 'https://github.com/gnu-xiaosong/ANN'
 EMAIL = '1829134124@qq.com'
 AUTHOR = 'xskj'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.0'
+VERSION = '0.2.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

### Comparing `xskj-pyAnn-0.1.0/xskj_pyAnn.egg-info/PKG-INFO` & `xskj-pyAnn-0.2.0/xskj_pyAnn.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: xskj-pyAnn
-Version: 0.1.0
+Version: 0.2.0
 Summary: 不依赖于框架的神经网络实现代码
 Home-page: https://github.com/gnu-xiaosong/ANN
 Author: xskj
 Author-email: 1829134124@qq.com
 License: MIT
 Description: 
         ## "# ANN" 
-        "# ANN" 
+        
+        
+        
+        v0.2.0  增加了多分类
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

