# Comparing `tmp/structifyai-0.8.0.tar.gz` & `tmp/structifyai-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structifyai-0.8.0.tar", last modified: Wed Mar 27 03:48:22 2024, max compression
+gzip compressed data, was "structifyai-0.9.0.tar", last modified: Wed Mar 27 03:52:26 2024, max compression
```

## Comparing `structifyai-0.8.0.tar` & `structifyai-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 dev       (1004) dev       (1000)        0 2024-03-27 03:48:22.256003 structifyai-0.8.0/
--rw-r--r--   0 dev       (1004) dev       (1000)       62 2024-03-27 03:48:03.000000 structifyai-0.8.0/CHANGELOG.md
--rw-r--r--   0 dev       (1004) dev       (1000)     1073 2024-03-27 03:48:03.000000 structifyai-0.8.0/LICENSE
--rw-r--r--   0 dev       (1004) dev       (1000)      120 2024-03-27 03:48:03.000000 structifyai-0.8.0/MANIFEST.in
--rw-r--r--   0 dev       (1004) dev       (1000)     1706 2024-03-27 03:48:22.256003 structifyai-0.8.0/PKG-INFO
--rw-r--r--   0 dev       (1004) dev       (1000)      729 2024-03-27 03:48:03.000000 structifyai-0.8.0/README.md
--rw-r--r--   0 dev       (1004) dev       (1000)       38 2024-03-27 03:48:22.256003 structifyai-0.8.0/setup.cfg
--rw-r--r--   0 dev       (1004) dev       (1000)     2007 2024-03-27 03:48:06.000000 structifyai-0.8.0/setup.py
-drwxr-xr-x   0 dev       (1004) dev       (1000)        0 2024-03-27 03:48:22.256003 structifyai-0.8.0/structify/
--rw-r--r--   0 dev       (1004) dev       (1000)      761 2024-03-27 03:48:06.000000 structifyai-0.8.0/structify/__init__.py
--rw-r--r--   0 dev       (1004) dev       (1000)     4751 2024-03-27 03:48:06.000000 structifyai-0.8.0/structify/_client.py
--rw-r--r--   0 dev       (1004) dev       (1000)     1826 2024-03-27 03:48:06.000000 structifyai-0.8.0/structify/_configuration.py
--rw-r--r--   0 dev       (1004) dev       (1000)      674 2024-03-27 03:48:06.000000 structifyai-0.8.0/structify/_patch.py
--rw-r--r--   0 dev       (1004) dev       (1000)    78873 2024-03-27 03:48:06.000000 structifyai-0.8.0/structify/_serialization.py
--rw-r--r--   0 dev       (1004) dev       (1000)      385 2024-03-27 03:48:22.000000 structifyai-0.8.0/structify/_version.py
-drwxr-xr-x   0 dev       (1004) dev       (1000)        0 2024-03-27 03:48:22.256003 structifyai-0.8.0/structify/aio/
--rw-r--r--   0 dev       (1004) dev       (1000)      708 2024-03-27 03:48:06.000000 structifyai-0.8.0/structify/aio/__init__.py
--rw-r--r--   0 dev       (1004) dev       (1000)     4885 2024-03-27 03:48:06.000000 structifyai-0.8.0/structify/aio/_client.py
--rw-r--r--   0 dev       (1004) dev       (1000)     1837 2024-03-27 03:48:06.000000 structifyai-0.8.0/structify/aio/_configuration.py
--rw-r--r--   0 dev       (1004) dev       (1000)      674 2024-03-27 03:48:06.000000 structifyai-0.8.0/structify/aio/_patch.py
-drwxr-xr-x   0 dev       (1004) dev       (1000)        0 2024-03-27 03:48:22.256003 structifyai-0.8.0/structify/aio/operations/
--rw-r--r--   0 dev       (1004) dev       (1000)      884 2024-03-27 03:48:06.000000 structifyai-0.8.0/structify/aio/operations/__init__.py
--rw-r--r--   0 dev       (1004) dev       (1000)    35291 2024-03-27 03:48:06.000000 structifyai-0.8.0/structify/aio/operations/_operations.py
--rw-r--r--   0 dev       (1004) dev       (1000)      674 2024-03-27 03:48:06.000000 structifyai-0.8.0/structify/aio/operations/_patch.py
-drwxr-xr-x   0 dev       (1004) dev       (1000)        0 2024-03-27 03:48:22.256003 structifyai-0.8.0/structify/operations/
--rw-r--r--   0 dev       (1004) dev       (1000)      884 2024-03-27 03:48:06.000000 structifyai-0.8.0/structify/operations/__init__.py
--rw-r--r--   0 dev       (1004) dev       (1000)    40831 2024-03-27 03:48:06.000000 structifyai-0.8.0/structify/operations/_operations.py
--rw-r--r--   0 dev       (1004) dev       (1000)      674 2024-03-27 03:48:06.000000 structifyai-0.8.0/structify/operations/_patch.py
--rw-r--r--   0 dev       (1004) dev       (1000)       26 2024-03-27 03:48:03.000000 structifyai-0.8.0/structify/py.typed
-drwxr-xr-x   0 dev       (1004) dev       (1000)        0 2024-03-27 03:48:22.256003 structifyai-0.8.0/structifyai.egg-info/
--rw-r--r--   0 dev       (1004) dev       (1000)     1706 2024-03-27 03:48:22.000000 structifyai-0.8.0/structifyai.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1004) dev       (1000)      738 2024-03-27 03:48:22.000000 structifyai-0.8.0/structifyai.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1004) dev       (1000)        1 2024-03-27 03:48:22.000000 structifyai-0.8.0/structifyai.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1004) dev       (1000)        1 2024-03-27 03:48:22.000000 structifyai-0.8.0/structifyai.egg-info/not-zip-safe
--rw-r--r--   0 dev       (1004) dev       (1000)       41 2024-03-27 03:48:22.000000 structifyai-0.8.0/structifyai.egg-info/requires.txt
--rw-r--r--   0 dev       (1004) dev       (1000)       10 2024-03-27 03:48:22.000000 structifyai-0.8.0/structifyai.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1004) dev       (1000)        0 2024-03-27 03:52:26.955476 structifyai-0.9.0/
+-rw-r--r--   0 dev       (1004) dev       (1000)       62 2024-03-27 03:52:09.000000 structifyai-0.9.0/CHANGELOG.md
+-rw-r--r--   0 dev       (1004) dev       (1000)     1073 2024-03-27 03:52:09.000000 structifyai-0.9.0/LICENSE
+-rw-r--r--   0 dev       (1004) dev       (1000)      120 2024-03-27 03:52:09.000000 structifyai-0.9.0/MANIFEST.in
+-rw-r--r--   0 dev       (1004) dev       (1000)     1706 2024-03-27 03:52:26.955476 structifyai-0.9.0/PKG-INFO
+-rw-r--r--   0 dev       (1004) dev       (1000)      729 2024-03-27 03:52:09.000000 structifyai-0.9.0/README.md
+-rw-r--r--   0 dev       (1004) dev       (1000)       38 2024-03-27 03:52:26.955476 structifyai-0.9.0/setup.cfg
+-rw-r--r--   0 dev       (1004) dev       (1000)     2007 2024-03-27 03:52:11.000000 structifyai-0.9.0/setup.py
+drwxr-xr-x   0 dev       (1004) dev       (1000)        0 2024-03-27 03:52:26.955476 structifyai-0.9.0/structify/
+-rw-r--r--   0 dev       (1004) dev       (1000)      761 2024-03-27 03:52:11.000000 structifyai-0.9.0/structify/__init__.py
+-rw-r--r--   0 dev       (1004) dev       (1000)     4751 2024-03-27 03:52:11.000000 structifyai-0.9.0/structify/_client.py
+-rw-r--r--   0 dev       (1004) dev       (1000)     1826 2024-03-27 03:52:11.000000 structifyai-0.9.0/structify/_configuration.py
+-rw-r--r--   0 dev       (1004) dev       (1000)      674 2024-03-27 03:52:11.000000 structifyai-0.9.0/structify/_patch.py
+-rw-r--r--   0 dev       (1004) dev       (1000)    78873 2024-03-27 03:52:11.000000 structifyai-0.9.0/structify/_serialization.py
+-rw-r--r--   0 dev       (1004) dev       (1000)      385 2024-03-27 03:52:26.000000 structifyai-0.9.0/structify/_version.py
+drwxr-xr-x   0 dev       (1004) dev       (1000)        0 2024-03-27 03:52:26.955476 structifyai-0.9.0/structify/aio/
+-rw-r--r--   0 dev       (1004) dev       (1000)      708 2024-03-27 03:52:11.000000 structifyai-0.9.0/structify/aio/__init__.py
+-rw-r--r--   0 dev       (1004) dev       (1000)     4885 2024-03-27 03:52:11.000000 structifyai-0.9.0/structify/aio/_client.py
+-rw-r--r--   0 dev       (1004) dev       (1000)     1837 2024-03-27 03:52:11.000000 structifyai-0.9.0/structify/aio/_configuration.py
+-rw-r--r--   0 dev       (1004) dev       (1000)      674 2024-03-27 03:52:11.000000 structifyai-0.9.0/structify/aio/_patch.py
+drwxr-xr-x   0 dev       (1004) dev       (1000)        0 2024-03-27 03:52:26.955476 structifyai-0.9.0/structify/aio/operations/
+-rw-r--r--   0 dev       (1004) dev       (1000)      884 2024-03-27 03:52:11.000000 structifyai-0.9.0/structify/aio/operations/__init__.py
+-rw-r--r--   0 dev       (1004) dev       (1000)    35291 2024-03-27 03:52:11.000000 structifyai-0.9.0/structify/aio/operations/_operations.py
+-rw-r--r--   0 dev       (1004) dev       (1000)      674 2024-03-27 03:52:11.000000 structifyai-0.9.0/structify/aio/operations/_patch.py
+drwxr-xr-x   0 dev       (1004) dev       (1000)        0 2024-03-27 03:52:26.955476 structifyai-0.9.0/structify/operations/
+-rw-r--r--   0 dev       (1004) dev       (1000)      884 2024-03-27 03:52:11.000000 structifyai-0.9.0/structify/operations/__init__.py
+-rw-r--r--   0 dev       (1004) dev       (1000)    40831 2024-03-27 03:52:11.000000 structifyai-0.9.0/structify/operations/_operations.py
+-rw-r--r--   0 dev       (1004) dev       (1000)      674 2024-03-27 03:52:11.000000 structifyai-0.9.0/structify/operations/_patch.py
+-rw-r--r--   0 dev       (1004) dev       (1000)       26 2024-03-27 03:52:09.000000 structifyai-0.9.0/structify/py.typed
+drwxr-xr-x   0 dev       (1004) dev       (1000)        0 2024-03-27 03:52:26.955476 structifyai-0.9.0/structifyai.egg-info/
+-rw-r--r--   0 dev       (1004) dev       (1000)     1706 2024-03-27 03:52:26.000000 structifyai-0.9.0/structifyai.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1004) dev       (1000)      738 2024-03-27 03:52:26.000000 structifyai-0.9.0/structifyai.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1004) dev       (1000)        1 2024-03-27 03:52:26.000000 structifyai-0.9.0/structifyai.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1004) dev       (1000)        1 2024-03-27 03:52:26.000000 structifyai-0.9.0/structifyai.egg-info/not-zip-safe
+-rw-r--r--   0 dev       (1004) dev       (1000)       41 2024-03-27 03:52:26.000000 structifyai-0.9.0/structifyai.egg-info/requires.txt
+-rw-r--r--   0 dev       (1004) dev       (1000)       10 2024-03-27 03:52:26.000000 structifyai-0.9.0/structifyai.egg-info/top_level.txt
```

### Comparing `structifyai-0.8.0/LICENSE` & `structifyai-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `structifyai-0.8.0/PKG-INFO` & `structifyai-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structifyai
-Version: 0.8.0
+Version: 0.9.0
 Summary: Microsoft Structify Client Library for Python
 Home-page: UNKNOWN
 Author: Microsoft Corporation
 License: MIT License
 Description: # Structify
         [Screenshot](assets/logo.png)
```

### Comparing `structifyai-0.8.0/README.md` & `structifyai-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `structifyai-0.8.0/setup.py` & `structifyai-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.8.0/structify/__init__.py` & `structifyai-0.9.0/structify/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.8.0/structify/_client.py` & `structifyai-0.9.0/structify/_client.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.8.0/structify/_configuration.py` & `structifyai-0.9.0/structify/_configuration.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.8.0/structify/_patch.py` & `structifyai-0.9.0/structify/_patch.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.8.0/structify/_serialization.py` & `structifyai-0.9.0/structify/_serialization.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.8.0/structify/aio/__init__.py` & `structifyai-0.9.0/structify/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.8.0/structify/aio/_client.py` & `structifyai-0.9.0/structify/aio/_client.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.8.0/structify/aio/_configuration.py` & `structifyai-0.9.0/structify/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.8.0/structify/aio/_patch.py` & `structifyai-0.9.0/structify/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.8.0/structify/aio/operations/__init__.py` & `structifyai-0.9.0/structify/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.8.0/structify/aio/operations/_operations.py` & `structifyai-0.9.0/structify/aio/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.8.0/structify/aio/operations/_patch.py` & `structifyai-0.9.0/structify/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.8.0/structify/operations/__init__.py` & `structifyai-0.9.0/structify/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.8.0/structify/operations/_operations.py` & `structifyai-0.9.0/structify/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.8.0/structify/operations/_patch.py` & `structifyai-0.9.0/structify/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `structifyai-0.8.0/structifyai.egg-info/PKG-INFO` & `structifyai-0.9.0/structifyai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structifyai
-Version: 0.8.0
+Version: 0.9.0
 Summary: Microsoft Structify Client Library for Python
 Home-page: UNKNOWN
 Author: Microsoft Corporation
 License: MIT License
 Description: # Structify
         [Screenshot](assets/logo.png)
```

### Comparing `structifyai-0.8.0/structifyai.egg-info/SOURCES.txt` & `structifyai-0.9.0/structifyai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

