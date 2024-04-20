# Comparing `tmp/motorcalc-0.1.2.tar.gz` & `tmp/motorcalc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motorcalc-0.1.2.tar", max compression
+gzip compressed data, was "motorcalc-0.2.0.tar", max compression
```

## Comparing `motorcalc-0.1.2.tar` & `motorcalc-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    15021 2023-03-20 10:17:29.400470 motorcalc-0.1.2/Berechnung von Gleichstrommotoren.ipynb
--rw-r--r--   0        0        0     1073 2023-03-25 20:05:52.770057 motorcalc-0.1.2/LICENSE.md
--rw-r--r--   0        0        0     5255 2023-03-26 15:06:27.999734 motorcalc-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-03-20 10:17:29.401919 motorcalc-0.1.2/motorcalc/__init__.py
--rw-r--r--   0        0        0    15276 2023-03-26 14:46:11.800388 motorcalc-0.1.2/motorcalc/dcmotor.py
--rw-r--r--   0        0        0     5396 2023-03-25 18:16:15.729909 motorcalc-0.1.2/motorcalc/dcmotorexport.py
--rw-r--r--   0        0        0     5367 2023-03-26 14:59:58.112458 motorcalc-0.1.2/motorcalc/dcmotorplot.py
--rw-r--r--   0        0        0     4072 2023-03-20 10:17:29.402490 motorcalc-0.1.2/motorcalc/load_dynamics.py
--rw-r--r--   0        0        0      562 2023-03-26 15:07:12.062988 motorcalc-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5972 1970-01-01 00:00:00.000000 motorcalc-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    15021 2023-03-20 10:17:29.400470 motorcalc-0.2.0/Berechnung von Gleichstrommotoren.ipynb
+-rw-r--r--   0        0        0     1073 2024-04-20 07:25:42.897224 motorcalc-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     5372 2024-04-20 07:25:42.897658 motorcalc-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-20 10:17:29.401919 motorcalc-0.2.0/motorcalc/__init__.py
+-rw-r--r--   0        0        0    15276 2024-04-20 07:25:42.898870 motorcalc-0.2.0/motorcalc/dcmotor.py
+-rw-r--r--   0        0        0     5396 2024-04-20 07:25:42.899076 motorcalc-0.2.0/motorcalc/dcmotorexport.py
+-rw-r--r--   0        0        0     5367 2024-04-20 07:25:42.899281 motorcalc-0.2.0/motorcalc/dcmotorplot.py
+-rw-r--r--   0        0        0     4072 2023-03-20 10:17:29.402490 motorcalc-0.2.0/motorcalc/load_dynamics.py
+-rw-r--r--   0        0        0      562 2024-04-20 08:12:31.117253 motorcalc-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6140 1970-01-01 00:00:00.000000 motorcalc-0.2.0/PKG-INFO
```

### Comparing `motorcalc-0.1.2/Berechnung von Gleichstrommotoren.ipynb` & `motorcalc-0.2.0/Berechnung von Gleichstrommotoren.ipynb`

 * *Files identical despite different names*

### Comparing `motorcalc-0.1.2/LICENSE.md` & `motorcalc-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `motorcalc-0.1.2/README.md` & `motorcalc-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -127,8 +127,12 @@
 To plot performance curves the ```CDCMotorPlot```-class from the dcmotorplot-module is needed. 
 ```python
 import motorcalc.dcmotorplot as dcmplt
 dcmplt.CDCMotorPlot(m).plot_curves()
 ```
 With this command the following Matplotlib-graph is generated:
 
+<<<<<<< HEAD
 ![Test graph](https://github.com/KOCOMOTION/motorcalc/blob/master/doc/img/performance_curve.png?raw=true)
+=======
+![Test graph](./doc/img/performance_curve.png)
+>>>>>>> c898b55a7e5d24c754d9b0873b94e9de915303a5
```

### Comparing `motorcalc-0.1.2/motorcalc/dcmotor.py` & `motorcalc-0.2.0/motorcalc/dcmotor.py`

 * *Files identical despite different names*

### Comparing `motorcalc-0.1.2/motorcalc/dcmotorexport.py` & `motorcalc-0.2.0/motorcalc/dcmotorexport.py`

 * *Files identical despite different names*

### Comparing `motorcalc-0.1.2/motorcalc/dcmotorplot.py` & `motorcalc-0.2.0/motorcalc/dcmotorplot.py`

 * *Files identical despite different names*

### Comparing `motorcalc-0.1.2/motorcalc/load_dynamics.py` & `motorcalc-0.2.0/motorcalc/load_dynamics.py`

 * *Files identical despite different names*

### Comparing `motorcalc-0.1.2/pyproject.toml` & `motorcalc-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motorcalc"
-version = "0.1.2"
+version = "0.2.0"
 description = "Calculation and plotting of DC motors"
 authors = ["Gerrit Kocherscheidt <kochersg@koco-group.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/KOCOMOTION/motorcalc.git"
 keywords = ["DC motor","gearbox"]
 include = ["Berechnung von Gleichstrommotoren.ipynb"]
```

### Comparing `motorcalc-0.1.2/PKG-INFO` & `motorcalc-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: motorcalc
-Version: 0.1.2
+Version: 0.2.0
 Summary: Calculation and plotting of DC motors
 Home-page: https://github.com/KOCOMOTION/motorcalc.git
 License: MIT
 Keywords: DC motor,gearbox
 Author: Gerrit Kocherscheidt
 Author-email: kochersg@koco-group.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: texttable (>=1.6.7,<2.0.0)
 Project-URL: Repository, https://github.com/KOCOMOTION/motorcalc.git
 Description-Content-Type: text/markdown
 
@@ -147,9 +148,13 @@
 To plot performance curves the ```CDCMotorPlot```-class from the dcmotorplot-module is needed. 
 ```python
 import motorcalc.dcmotorplot as dcmplt
 dcmplt.CDCMotorPlot(m).plot_curves()
 ```
 With this command the following Matplotlib-graph is generated:
 
+<<<<<<< HEAD
 ![Test graph](https://github.com/KOCOMOTION/motorcalc/blob/master/doc/img/performance_curve.png?raw=true)
+=======
+![Test graph](./doc/img/performance_curve.png)
+>>>>>>> c898b55a7e5d24c754d9b0873b94e9de915303a5
```

