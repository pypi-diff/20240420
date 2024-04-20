# Comparing `tmp/tukey-0.0.2.tar.gz` & `tmp/tukey-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tukey-0.0.2.tar", last modified: Wed Apr 17 22:09:28 2024, max compression
+gzip compressed data, was "tukey-0.1.0.tar", last modified: Sat Apr 20 21:42:22 2024, max compression
```

## Comparing `tukey-0.0.2.tar` & `tukey-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 22:09:28.390659 tukey-0.0.2/
--rw-rw-rw-   0        0        0    35821 2024-04-17 16:42:19.000000 tukey-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0    44214 2024-04-17 22:09:28.388374 tukey-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1812 2024-04-17 21:54:19.000000 tukey-0.0.2/README.md
--rw-rw-rw-   0        0        0     1379 2024-04-17 22:07:39.000000 tukey-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 22:09:28.390659 tukey-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 22:09:28.324175 tukey-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 22:09:28.343287 tukey-0.0.2/src/tukey/
--rw-rw-rw-   0        0        0       25 2024-04-17 16:40:37.000000 tukey-0.0.2/src/tukey/__init__.py
--rw-rw-rw-   0        0        0      302 2024-04-17 21:55:15.000000 tukey-0.0.2/src/tukey/tukey.py
-drwxrwxrwx   0        0        0        0 2024-04-17 22:09:28.380409 tukey-0.0.2/src/tukey.egg-info/
--rw-rw-rw-   0        0        0    44214 2024-04-17 22:09:28.000000 tukey-0.0.2/src/tukey.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-04-17 22:09:28.000000 tukey-0.0.2/src/tukey.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 22:09:28.000000 tukey-0.0.2/src/tukey.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-17 22:09:28.000000 tukey-0.0.2/src/tukey.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2024-04-17 22:09:28.000000 tukey-0.0.2/src/tukey.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 21:42:22.091904 tukey-0.1.0/
+-rw-rw-rw-   0        0        0    35821 2024-04-17 16:42:19.000000 tukey-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0    44258 2024-04-20 21:42:22.089489 tukey-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1856 2024-04-20 21:40:07.000000 tukey-0.1.0/README.md
+-rw-rw-rw-   0        0        0     1379 2024-04-20 21:35:38.000000 tukey-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-20 21:42:22.091904 tukey-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-20 21:42:22.020094 tukey-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-20 21:42:22.038183 tukey-0.1.0/src/tukey/
+-rw-rw-rw-   0        0        0       25 2024-04-17 16:40:37.000000 tukey-0.1.0/src/tukey/__init__.py
+-rw-rw-rw-   0        0        0      406 2024-04-20 21:36:45.000000 tukey-0.1.0/src/tukey/tukey.py
+drwxrwxrwx   0        0        0        0 2024-04-20 21:42:22.085408 tukey-0.1.0/src/tukey.egg-info/
+-rw-rw-rw-   0        0        0    44258 2024-04-20 21:42:21.000000 tukey-0.1.0/src/tukey.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-04-20 21:42:22.000000 tukey-0.1.0/src/tukey.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 21:42:21.000000 tukey-0.1.0/src/tukey.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-20 21:42:21.000000 tukey-0.1.0/src/tukey.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2024-04-20 21:42:21.000000 tukey-0.1.0/src/tukey.egg-info/top_level.txt
```

### Comparing `tukey-0.0.2/LICENSE.txt` & `tukey-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tukey-0.0.2/PKG-INFO` & `tukey-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tukey
-Version: 0.0.2
+Version: 0.1.0
 Summary: A python based math module
 Author-email: Shubhranil Basak <Shubhranil.Basak@iiitb.ac.in>
 Maintainer-email: Shubhranil Basak <Shubhranil.Basak@iiitb.ac.in>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -694,15 +694,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# tukey (v 0.0.2)
+# tukey (v 0.1.0)
 The tukey package provides basic mathematical operations like addition, subtraction, multiplication and division.
 
 * **Code and Documentation:** [https://github.com/Shubhranil-Basak/tukey](https://github.com/Shubhranil-Basak/tukey)
 *  **PyPi:** [https://pypi.org/project/tukey/](https://pypi.org/project/tukey/)
 *  **Bug Reports:** [https://github.com/Shubhranil-Basak/tukey/issues](https://github.com/Shubhranil-Basak/tukey/issues)
 
 Installation
@@ -717,14 +717,15 @@
 ```python
 from tukey import tukey
 
 # Basic arithmatic operations
 print(tukey.add(1, 2))         # Output: 3
 print(tukey.subtract(5, 3))    # Output: 2
 print(tukey.multiply(4, 6))    # Output: 24
+print(tukey.modulo(5, 2))      # Output: 1
 print(tukey.divide(8, 2))      # Output: 4.0
 print(tukey.divide(10, 0))     # Output: Cannot divide by zero
 ```
 
 
 Inspiration
 ----------------------
```

### Comparing `tukey-0.0.2/README.md` & `tukey-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# tukey (v 0.0.2)
+# tukey (v 0.1.0)
 The tukey package provides basic mathematical operations like addition, subtraction, multiplication and division.
 
 * **Code and Documentation:** [https://github.com/Shubhranil-Basak/tukey](https://github.com/Shubhranil-Basak/tukey)
 *  **PyPi:** [https://pypi.org/project/tukey/](https://pypi.org/project/tukey/)
 *  **Bug Reports:** [https://github.com/Shubhranil-Basak/tukey/issues](https://github.com/Shubhranil-Basak/tukey/issues)
 
 Installation
@@ -17,14 +17,15 @@
 ```python
 from tukey import tukey
 
 # Basic arithmatic operations
 print(tukey.add(1, 2))         # Output: 3
 print(tukey.subtract(5, 3))    # Output: 2
 print(tukey.multiply(4, 6))    # Output: 24
+print(tukey.modulo(5, 2))      # Output: 1
 print(tukey.divide(8, 2))      # Output: 4.0
 print(tukey.divide(10, 0))     # Output: Cannot divide by zero
 ```
 
 
 Inspiration
 ----------------------
```

### Comparing `tukey-0.0.2/pyproject.toml` & `tukey-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 
 [project]
 
 name = "tukey"
 
-version = "0.0.2"
+version = "0.1.0"
 
 description = "A python based math module"
 
 readme = "README.md"
 
 requires-python = ">=3.8"
```

### Comparing `tukey-0.0.2/src/tukey.egg-info/PKG-INFO` & `tukey-0.1.0/src/tukey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tukey
-Version: 0.0.2
+Version: 0.1.0
 Summary: A python based math module
 Author-email: Shubhranil Basak <Shubhranil.Basak@iiitb.ac.in>
 Maintainer-email: Shubhranil Basak <Shubhranil.Basak@iiitb.ac.in>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -694,15 +694,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# tukey (v 0.0.2)
+# tukey (v 0.1.0)
 The tukey package provides basic mathematical operations like addition, subtraction, multiplication and division.
 
 * **Code and Documentation:** [https://github.com/Shubhranil-Basak/tukey](https://github.com/Shubhranil-Basak/tukey)
 *  **PyPi:** [https://pypi.org/project/tukey/](https://pypi.org/project/tukey/)
 *  **Bug Reports:** [https://github.com/Shubhranil-Basak/tukey/issues](https://github.com/Shubhranil-Basak/tukey/issues)
 
 Installation
@@ -717,14 +717,15 @@
 ```python
 from tukey import tukey
 
 # Basic arithmatic operations
 print(tukey.add(1, 2))         # Output: 3
 print(tukey.subtract(5, 3))    # Output: 2
 print(tukey.multiply(4, 6))    # Output: 24
+print(tukey.modulo(5, 2))      # Output: 1
 print(tukey.divide(8, 2))      # Output: 4.0
 print(tukey.divide(10, 0))     # Output: Cannot divide by zero
 ```
 
 
 Inspiration
 ----------------------
```

