# Comparing `tmp/tsa_course-0.2.0.tar.gz` & `tmp/tsa_course-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsa_course-0.2.0.tar", last modified: Fri Apr 19 20:12:30 2024, max compression
+gzip compressed data, was "tsa_course-0.2.1.tar", last modified: Fri Apr 19 20:19:03 2024, max compression
```

## Comparing `tsa_course-0.2.0.tar` & `tsa_course-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-19 20:12:30.065765 tsa_course-0.2.0/
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     1078 2024-04-12 23:36:28.000000 tsa_course-0.2.0/LICENSE
--rw-r--r--   0 filippo   (1001) filippo   (1001)     8175 2024-04-19 20:12:30.065765 tsa_course-0.2.0/PKG-INFO
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     7455 2024-04-17 00:21:56.000000 tsa_course-0.2.0/README.md
--rw-rw-r--   0 filippo   (1001) filippo   (1001)       38 2024-04-19 20:12:30.065765 tsa_course-0.2.0/setup.cfg
--rw-rw-r--   0 filippo   (1001) filippo   (1001)      917 2024-04-19 20:11:36.000000 tsa_course-0.2.0/setup.py
-drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-19 20:12:30.065765 tsa_course-0.2.0/tsa_course/
--rw-rw-r--   0 filippo   (1001) filippo   (1001)        0 2024-04-16 15:41:27.000000 tsa_course-0.2.0/tsa_course/__init__.py
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     1190 2024-04-18 13:30:31.000000 tsa_course-0.2.0/tsa_course/lecture1.py
--rw-rw-r--   0 filippo   (1001) filippo   (1001)    13644 2024-04-17 00:13:18.000000 tsa_course-0.2.0/tsa_course/lecture11.py
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     3309 2024-04-19 19:32:21.000000 tsa_course-0.2.0/tsa_course/lecture8.py
-drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-19 20:12:30.065765 tsa_course-0.2.0/tsa_course.egg-info/
--rw-r--r--   0 filippo   (1001) filippo   (1001)     8175 2024-04-19 20:12:30.000000 tsa_course-0.2.0/tsa_course.egg-info/PKG-INFO
--rw-rw-r--   0 filippo   (1001) filippo   (1001)      288 2024-04-19 20:12:30.000000 tsa_course-0.2.0/tsa_course.egg-info/SOURCES.txt
--rw-rw-r--   0 filippo   (1001) filippo   (1001)        1 2024-04-19 20:12:30.000000 tsa_course-0.2.0/tsa_course.egg-info/dependency_links.txt
--rw-rw-r--   0 filippo   (1001) filippo   (1001)       35 2024-04-19 20:12:30.000000 tsa_course-0.2.0/tsa_course.egg-info/requires.txt
--rw-rw-r--   0 filippo   (1001) filippo   (1001)       11 2024-04-19 20:12:30.000000 tsa_course-0.2.0/tsa_course.egg-info/top_level.txt
+drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-19 20:19:03.333765 tsa_course-0.2.1/
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     1078 2024-04-12 23:36:28.000000 tsa_course-0.2.1/LICENSE
+-rw-r--r--   0 filippo   (1001) filippo   (1001)     8148 2024-04-19 20:19:03.333765 tsa_course-0.2.1/PKG-INFO
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     7428 2024-04-19 20:18:33.000000 tsa_course-0.2.1/README.md
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)       38 2024-04-19 20:19:03.333765 tsa_course-0.2.1/setup.cfg
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)      917 2024-04-19 20:18:45.000000 tsa_course-0.2.1/setup.py
+drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-19 20:19:03.333765 tsa_course-0.2.1/tsa_course/
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)        0 2024-04-16 15:41:27.000000 tsa_course-0.2.1/tsa_course/__init__.py
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     1190 2024-04-18 13:30:31.000000 tsa_course-0.2.1/tsa_course/lecture1.py
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)    13644 2024-04-17 00:13:18.000000 tsa_course-0.2.1/tsa_course/lecture11.py
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     3309 2024-04-19 19:32:21.000000 tsa_course-0.2.1/tsa_course/lecture8.py
+drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-19 20:19:03.333765 tsa_course-0.2.1/tsa_course.egg-info/
+-rw-r--r--   0 filippo   (1001) filippo   (1001)     8148 2024-04-19 20:19:03.000000 tsa_course-0.2.1/tsa_course.egg-info/PKG-INFO
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)      288 2024-04-19 20:19:03.000000 tsa_course-0.2.1/tsa_course.egg-info/SOURCES.txt
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)        1 2024-04-19 20:19:03.000000 tsa_course-0.2.1/tsa_course.egg-info/dependency_links.txt
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)       35 2024-04-19 20:19:03.000000 tsa_course-0.2.1/tsa_course.egg-info/requires.txt
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)       11 2024-04-19 20:19:03.000000 tsa_course-0.2.1/tsa_course.egg-info/top_level.txt
```

### Comparing `tsa_course-0.2.0/LICENSE` & `tsa_course-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tsa_course-0.2.0/PKG-INFO` & `tsa_course-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsa_course
-Version: 0.2.0
+Version: 0.2.1
 Summary: A collection of scripts and functions used in the course 'Time Series Analysis with Python'
 Author: Filippo Maria Bianchi
 Author-email: filippombianchi@gmail.com
 Project-URL: Documentation, https://filippomb.github.io/python-time-series-handbook
 Project-URL: Source Code, https://github.com/FilippoMB/python-time-series-handbook
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,21 +15,19 @@
 Requires-Dist: numpy>1.19.5
 Requires-Dist: matplotlib
 Requires-Dist: scipy
 Requires-Dist: tqdm
 
 # Time Series Analysis with Python
 
-<div align="center">
-   <img src="https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/logo.png" style="width: 5cm; display: block; margin: auto;">
-</div>
+<img src="https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/logo.png" style="width: 5cm; display: block; margin: auto;">
 
 <br>
 <div align="center">
-📚 <a href="https://filippomb.github.io/python-time-series-handbook">Read the book</a>
+📚 <a href="https://filippomb.github.io/python-time-series-handbook">Read it as a book</a>
 </div>
 <br>
 
 This is the collection of notebooks for the course *Time Series Analysis with Python*.
 For more information and for reading the content of this repository, please refer to the [book](https://filippomb.github.io/python-time-series-handbook) version.
 
 ## 📑 Content
```

#### html2text {}

```diff
@@ -1,21 +1,19 @@
-Metadata-Version: 2.1 Name: tsa_course Version: 0.2.0 Summary: A collection of
+Metadata-Version: 2.1 Name: tsa_course Version: 0.2.1 Summary: A collection of
 scripts and functions used in the course 'Time Series Analysis with Python'
 Author: Filippo Maria Bianchi Author-email: filippombianchi@gmail.com Project-
 URL: Documentation, https://filippomb.github.io/python-time-series-handbook
 Project-URL: Source Code, https://github.com/FilippoMB/python-time-series-
 handbook Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: numpy>1.19.5 Requires-Dist: matplotlib Requires-Dist:
-scipy Requires-Dist: tqdm # Time Series Analysis with Python
-[https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/
-                                   logo.png]
-
-                              ð _R_e_a_d_ _t_h_e_ _b_o_o_k
+scipy Requires-Dist: tqdm # Time Series Analysis with Python[https://
+raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/logo.png]
+                            ð _R_e_a_d_ _i_t_ _a_s_ _a_ _b_o_o_k
 
 This is the collection of notebooks for the course *Time Series Analysis with
 Python*. For more information and for reading the content of this repository,
 please refer to the [book](https://filippomb.github.io/python-time-series-
 handbook) version. ## ð Content 1. **Introduction to time series analysis**
 - Definition of time series data - Main applications of time series analysis -
 Statistical vs dynamical models perspective - Components of a time series -
```

### Comparing `tsa_course-0.2.0/README.md` & `tsa_course-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # Time Series Analysis with Python
 
-<div align="center">
-   <img src="https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/logo.png" style="width: 5cm; display: block; margin: auto;">
-</div>
+<img src="https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/logo.png" style="width: 5cm; display: block; margin: auto;">
 
 <br>
 <div align="center">
-📚 <a href="https://filippomb.github.io/python-time-series-handbook">Read the book</a>
+📚 <a href="https://filippomb.github.io/python-time-series-handbook">Read it as a book</a>
 </div>
 <br>
 
 This is the collection of notebooks for the course *Time Series Analysis with Python*.
 For more information and for reading the content of this repository, please refer to the [book](https://filippomb.github.io/python-time-series-handbook) version.
 
 ## 📑 Content
```

#### html2text {}

```diff
@@ -1,12 +1,10 @@
-# Time Series Analysis with Python
-[https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/
-                                   logo.png]
-
-                              ð _R_e_a_d_ _t_h_e_ _b_o_o_k
+# Time Series Analysis with Python[https://raw.githubusercontent.com/FilippoMB/
+python-time-series-handbook/main/logo.png]
+                            ð _R_e_a_d_ _i_t_ _a_s_ _a_ _b_o_o_k
 
 This is the collection of notebooks for the course *Time Series Analysis with
 Python*. For more information and for reading the content of this repository,
 please refer to the [book](https://filippomb.github.io/python-time-series-
 handbook) version. ## ð Content 1. **Introduction to time series analysis**
 - Definition of time series data - Main applications of time series analysis -
 Statistical vs dynamical models perspective - Components of a time series -
```

### Comparing `tsa_course-0.2.0/setup.py` & `tsa_course-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tsa_course",
-    version="0.2.0",
+    version="0.2.1",
     packages=find_packages(),
     python_requires='>=3.10',
     install_requires=[
         'numpy>1.19.5',
         'matplotlib',
         'scipy',
         'tqdm'
```

### Comparing `tsa_course-0.2.0/tsa_course/lecture1.py` & `tsa_course-0.2.1/tsa_course/lecture1.py`

 * *Files identical despite different names*

### Comparing `tsa_course-0.2.0/tsa_course/lecture11.py` & `tsa_course-0.2.1/tsa_course/lecture11.py`

 * *Files identical despite different names*

### Comparing `tsa_course-0.2.0/tsa_course/lecture8.py` & `tsa_course-0.2.1/tsa_course/lecture8.py`

 * *Files identical despite different names*

### Comparing `tsa_course-0.2.0/tsa_course.egg-info/PKG-INFO` & `tsa_course-0.2.1/tsa_course.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsa_course
-Version: 0.2.0
+Version: 0.2.1
 Summary: A collection of scripts and functions used in the course 'Time Series Analysis with Python'
 Author: Filippo Maria Bianchi
 Author-email: filippombianchi@gmail.com
 Project-URL: Documentation, https://filippomb.github.io/python-time-series-handbook
 Project-URL: Source Code, https://github.com/FilippoMB/python-time-series-handbook
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,21 +15,19 @@
 Requires-Dist: numpy>1.19.5
 Requires-Dist: matplotlib
 Requires-Dist: scipy
 Requires-Dist: tqdm
 
 # Time Series Analysis with Python
 
-<div align="center">
-   <img src="https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/logo.png" style="width: 5cm; display: block; margin: auto;">
-</div>
+<img src="https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/logo.png" style="width: 5cm; display: block; margin: auto;">
 
 <br>
 <div align="center">
-📚 <a href="https://filippomb.github.io/python-time-series-handbook">Read the book</a>
+📚 <a href="https://filippomb.github.io/python-time-series-handbook">Read it as a book</a>
 </div>
 <br>
 
 This is the collection of notebooks for the course *Time Series Analysis with Python*.
 For more information and for reading the content of this repository, please refer to the [book](https://filippomb.github.io/python-time-series-handbook) version.
 
 ## 📑 Content
```

#### html2text {}

```diff
@@ -1,21 +1,19 @@
-Metadata-Version: 2.1 Name: tsa_course Version: 0.2.0 Summary: A collection of
+Metadata-Version: 2.1 Name: tsa_course Version: 0.2.1 Summary: A collection of
 scripts and functions used in the course 'Time Series Analysis with Python'
 Author: Filippo Maria Bianchi Author-email: filippombianchi@gmail.com Project-
 URL: Documentation, https://filippomb.github.io/python-time-series-handbook
 Project-URL: Source Code, https://github.com/FilippoMB/python-time-series-
 handbook Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: numpy>1.19.5 Requires-Dist: matplotlib Requires-Dist:
-scipy Requires-Dist: tqdm # Time Series Analysis with Python
-[https://raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/
-                                   logo.png]
-
-                              ð _R_e_a_d_ _t_h_e_ _b_o_o_k
+scipy Requires-Dist: tqdm # Time Series Analysis with Python[https://
+raw.githubusercontent.com/FilippoMB/python-time-series-handbook/main/logo.png]
+                            ð _R_e_a_d_ _i_t_ _a_s_ _a_ _b_o_o_k
 
 This is the collection of notebooks for the course *Time Series Analysis with
 Python*. For more information and for reading the content of this repository,
 please refer to the [book](https://filippomb.github.io/python-time-series-
 handbook) version. ## ð Content 1. **Introduction to time series analysis**
 - Definition of time series data - Main applications of time series analysis -
 Statistical vs dynamical models perspective - Components of a time series -
```

