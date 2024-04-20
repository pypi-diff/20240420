# Comparing `tmp/FrustrationDynamiX-0.1.0.tar.gz` & `tmp/FrustrationDynamiX-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FrustrationDynamiX-0.1.0.tar", last modified: Sat Apr 20 20:31:08 2024, max compression
+gzip compressed data, was "FrustrationDynamiX-0.2.0.tar", last modified: Sat Apr 20 20:36:51 2024, max compression
```

## Comparing `FrustrationDynamiX-0.1.0.tar` & `FrustrationDynamiX-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 20:31:08.627771 FrustrationDynamiX-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-04-20 20:31:08.597604 FrustrationDynamiX-0.1.0/FrustrationDynamiX/
--rw-rw-rw-   0        0        0       36 2024-04-19 23:23:05.000000 FrustrationDynamiX-0.1.0/FrustrationDynamiX/__init__.py
--rw-rw-rw-   0        0        0    25409 2024-04-19 23:18:01.000000 FrustrationDynamiX-0.1.0/FrustrationDynamiX/core.py
-drwxrwxrwx   0        0        0        0 2024-04-20 20:31:08.627771 FrustrationDynamiX-0.1.0/FrustrationDynamiX.egg-info/
--rw-rw-rw-   0        0        0     1370 2024-04-20 20:31:08.000000 FrustrationDynamiX-0.1.0/FrustrationDynamiX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2024-04-20 20:31:08.000000 FrustrationDynamiX-0.1.0/FrustrationDynamiX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 20:31:08.000000 FrustrationDynamiX-0.1.0/FrustrationDynamiX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2024-04-20 20:31:08.000000 FrustrationDynamiX-0.1.0/FrustrationDynamiX.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-20 20:31:08.000000 FrustrationDynamiX-0.1.0/FrustrationDynamiX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1094 2024-04-20 20:30:54.000000 FrustrationDynamiX-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1370 2024-04-20 20:31:08.627771 FrustrationDynamiX-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      600 2024-04-20 20:05:17.000000 FrustrationDynamiX-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-20 20:31:08.627771 FrustrationDynamiX-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1317 2024-04-20 20:31:00.000000 FrustrationDynamiX-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 20:36:51.751260 FrustrationDynamiX-0.2.0/
+drwxrwxrwx   0        0        0        0 2024-04-20 20:36:51.714828 FrustrationDynamiX-0.2.0/FrustrationDynamiX/
+-rw-rw-rw-   0        0        0       36 2024-04-19 23:23:05.000000 FrustrationDynamiX-0.2.0/FrustrationDynamiX/__init__.py
+-rw-rw-rw-   0        0        0    25409 2024-04-19 23:18:01.000000 FrustrationDynamiX-0.2.0/FrustrationDynamiX/core.py
+drwxrwxrwx   0        0        0        0 2024-04-20 20:36:51.747575 FrustrationDynamiX-0.2.0/FrustrationDynamiX.egg-info/
+-rw-rw-rw-   0        0        0     1370 2024-04-20 20:36:51.000000 FrustrationDynamiX-0.2.0/FrustrationDynamiX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-04-20 20:36:51.000000 FrustrationDynamiX-0.2.0/FrustrationDynamiX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 20:36:51.000000 FrustrationDynamiX-0.2.0/FrustrationDynamiX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2024-04-20 20:36:51.000000 FrustrationDynamiX-0.2.0/FrustrationDynamiX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-20 20:36:51.000000 FrustrationDynamiX-0.2.0/FrustrationDynamiX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1094 2024-04-20 20:30:54.000000 FrustrationDynamiX-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1370 2024-04-20 20:36:51.751260 FrustrationDynamiX-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2024-04-20 20:05:17.000000 FrustrationDynamiX-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-20 20:36:51.754769 FrustrationDynamiX-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1310 2024-04-20 20:36:33.000000 FrustrationDynamiX-0.2.0/setup.py
```

### Comparing `FrustrationDynamiX-0.1.0/FrustrationDynamiX/core.py` & `FrustrationDynamiX-0.2.0/FrustrationDynamiX/core.py`

 * *Files identical despite different names*

### Comparing `FrustrationDynamiX-0.1.0/FrustrationDynamiX.egg-info/PKG-INFO` & `FrustrationDynamiX-0.2.0/FrustrationDynamiX.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FrustrationDynamiX
-Version: 0.1.0
+Version: 0.2.0
 Summary: A package for handling computing frustration in dynamical systems
 Home-page: https://github.com/asb24repo/FrustrationDynamiX
 Author: Ali S. Badereddine
 Author-email: asb24@mail.aub.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FrustrationDynamiX-0.1.0/LICENSE` & `FrustrationDynamiX-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FrustrationDynamiX-0.1.0/PKG-INFO` & `FrustrationDynamiX-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FrustrationDynamiX
-Version: 0.1.0
+Version: 0.2.0
 Summary: A package for handling computing frustration in dynamical systems
 Home-page: https://github.com/asb24repo/FrustrationDynamiX
 Author: Ali S. Badereddine
 Author-email: asb24@mail.aub.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FrustrationDynamiX-0.1.0/README.md` & `FrustrationDynamiX-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `FrustrationDynamiX-0.1.0/setup.py` & `FrustrationDynamiX-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FrustrationDynamiX',
-    version='0.1.0',
+    version='0.2.0',
     packages=find_packages(),
     description='A package for handling computing frustration in dynamical systems',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Ali S. Badereddine',
     author_email='asb24@mail.aub.edu',
     license='MIT',
     install_requires=[
         'numpy',
         'pandas',
         'matplotlib',
         'networkx',
         'scipy',
-        'python-ortools',
+        'ortools',
         'tqdm',
         'pyEDM==1.14.3',
         'shutilwhich', # if shutil is required, it's part of the standard library and doesn't need to be installed
         'warnings' # warnings is also part of the standard library
     ],
     python_requires='>=3.6',
     url='https://github.com/asb24repo/FrustrationDynamiX',
```

