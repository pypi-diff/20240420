# Comparing `tmp/mingzi-1.2.0.tar.gz` & `tmp/mingzi-1.2.1.tar.gz`

## Comparing `mingzi-1.2.0.tar` & `mingzi-1.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 mingzi-1.2.0/src/mingzi/__init__.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 mingzi-1.2.0/src/mingzi/_mingzi.py
--rw-r--r--   0        0        0    27035 2020-02-02 00:00:00.000000 mingzi-1.2.0/src/mingzi/data.json
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 mingzi-1.2.0/LICENSE
--rw-r--r--   0        0        0     9622 2020-02-02 00:00:00.000000 mingzi-1.2.0/README.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 mingzi-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     9937 2020-02-02 00:00:00.000000 mingzi-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 mingzi-1.2.1/src/mingzi/__init__.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 mingzi-1.2.1/src/mingzi/_mingzi.py
+-rw-r--r--   0        0        0    27035 2020-02-02 00:00:00.000000 mingzi-1.2.1/src/mingzi/data.json
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 mingzi-1.2.1/LICENSE
+-rw-r--r--   0        0        0     9615 2020-02-02 00:00:00.000000 mingzi-1.2.1/README.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 mingzi-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     9930 2020-02-02 00:00:00.000000 mingzi-1.2.1/PKG-INFO
```

### Comparing `mingzi-1.2.0/src/mingzi/_mingzi.py` & `mingzi-1.2.1/src/mingzi/_mingzi.py`

 * *Files identical despite different names*

### Comparing `mingzi-1.2.0/src/mingzi/data.json` & `mingzi-1.2.1/src/mingzi/data.json`

 * *Files identical despite different names*

### Comparing `mingzi-1.2.0/LICENSE` & `mingzi-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mingzi-1.2.0/README.md` & `mingzi-1.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 pip install mingzi
 ```
 
 
 ## Quick Start
 
 ```{python}
-from mingzi.mingzi import *
+from mingzi import *
 mingzi()
 >>> ['崔依梅']
 mingzi()
 >>> ['崔曦']
 ```
```

### Comparing `mingzi-1.2.0/pyproject.toml` & `mingzi-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mingzi"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Aliyacs Souna", email="17818403529@139.com" },
 ]
 description = "这是一个用来生成随机中文姓名的包。This is a library for developers to use to generate random Chinese names."
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
```

### Comparing `mingzi-1.2.0/PKG-INFO` & `mingzi-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mingzi
-Version: 1.2.0
+Version: 1.2.1
 Summary: 这是一个用来生成随机中文姓名的包。This is a library for developers to use to generate random Chinese names.
 Author-email: Aliyacs Souna <17818403529@139.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
@@ -32,15 +32,15 @@
 pip install mingzi
 ```
 
 
 ## Quick Start
 
 ```{python}
-from mingzi.mingzi import *
+from mingzi import *
 mingzi()
 >>> ['崔依梅']
 mingzi()
 >>> ['崔曦']
 ```
```

