# Comparing `tmp/numpyneuron-0.1.tar.gz` & `tmp/numpyneuron-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpyneuron-0.1.tar", last modified: Fri Apr 19 21:51:42 2024, max compression
+gzip compressed data, was "numpyneuron-0.2.tar", last modified: Fri Apr 19 21:56:31 2024, max compression
```

## Comparing `numpyneuron-0.1.tar` & `numpyneuron-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 21:51:42.914491 numpyneuron-0.1/
--rw-r--r--   0 jensen     (501) staff       (20)     2605 2024-04-19 21:51:42.914311 numpyneuron-0.1/PKG-INFO
--rw-r--r--   0 jensen     (501) staff       (20)     2469 2024-04-19 21:12:37.000000 numpyneuron-0.1/README.md
-drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 21:51:42.913356 numpyneuron-0.1/nn/
-drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 21:51:42.914159 numpyneuron-0.1/nn/numpyneuron.egg-info/
--rw-r--r--   0 jensen     (501) staff       (20)     2605 2024-04-19 21:51:42.000000 numpyneuron-0.1/nn/numpyneuron.egg-info/PKG-INFO
--rw-r--r--   0 jensen     (501) staff       (20)      170 2024-04-19 21:51:42.000000 numpyneuron-0.1/nn/numpyneuron.egg-info/SOURCES.txt
--rw-r--r--   0 jensen     (501) staff       (20)        1 2024-04-19 21:51:42.000000 numpyneuron-0.1/nn/numpyneuron.egg-info/dependency_links.txt
--rw-r--r--   0 jensen     (501) staff       (20)        1 2024-04-19 21:51:42.000000 numpyneuron-0.1/nn/numpyneuron.egg-info/top_level.txt
--rw-r--r--   0 jensen     (501) staff       (20)       38 2024-04-19 21:51:42.914528 numpyneuron-0.1/setup.cfg
--rw-r--r--   0 jensen     (501) staff       (20)      759 2024-04-19 21:51:28.000000 numpyneuron-0.1/setup.py
+drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 21:56:31.033201 numpyneuron-0.2/
+-rw-r--r--   0 jensen     (501) staff       (20)     2605 2024-04-19 21:56:31.033038 numpyneuron-0.2/PKG-INFO
+-rw-r--r--   0 jensen     (501) staff       (20)     2469 2024-04-19 21:12:37.000000 numpyneuron-0.2/README.md
+drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 21:56:31.032097 numpyneuron-0.2/numpyneuron/
+drwxr-xr-x   0 jensen     (501) staff       (20)        0 2024-04-19 21:56:31.032883 numpyneuron-0.2/numpyneuron/numpyneuron.egg-info/
+-rw-r--r--   0 jensen     (501) staff       (20)     2605 2024-04-19 21:56:31.000000 numpyneuron-0.2/numpyneuron/numpyneuron.egg-info/PKG-INFO
+-rw-r--r--   0 jensen     (501) staff       (20)      206 2024-04-19 21:56:31.000000 numpyneuron-0.2/numpyneuron/numpyneuron.egg-info/SOURCES.txt
+-rw-r--r--   0 jensen     (501) staff       (20)        1 2024-04-19 21:56:31.000000 numpyneuron-0.2/numpyneuron/numpyneuron.egg-info/dependency_links.txt
+-rw-r--r--   0 jensen     (501) staff       (20)        1 2024-04-19 21:56:31.000000 numpyneuron-0.2/numpyneuron/numpyneuron.egg-info/top_level.txt
+-rw-r--r--   0 jensen     (501) staff       (20)       38 2024-04-19 21:56:31.033233 numpyneuron-0.2/setup.cfg
+-rw-r--r--   0 jensen     (501) staff       (20)      777 2024-04-19 21:56:21.000000 numpyneuron-0.2/setup.py
```

### Comparing `numpyneuron-0.1/PKG-INFO` & `numpyneuron-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numpyneuron
-Version: 0.1
+Version: 0.2
 Summary: Simple, lightweight neural network framework built in numpy
 Home-page: https://github.com/Jensen-holm/Numpy-Neuron
 Author: Jensen Holm
 Author-email: jensen.dev.01@gmail.com
 Project-URL: Bug Tracker, https://github.com/Jensen-holm/Numpy-Neuron/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `numpyneuron-0.1/README.md` & `numpyneuron-0.2/README.md`

 * *Files identical despite different names*

### Comparing `numpyneuron-0.1/nn/numpyneuron.egg-info/PKG-INFO` & `numpyneuron-0.2/numpyneuron/numpyneuron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numpyneuron
-Version: 0.1
+Version: 0.2
 Summary: Simple, lightweight neural network framework built in numpy
 Home-page: https://github.com/Jensen-holm/Numpy-Neuron
 Author: Jensen Holm
 Author-email: jensen.dev.01@gmail.com
 Project-URL: Bug Tracker, https://github.com/Jensen-holm/Numpy-Neuron/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `numpyneuron-0.1/setup.py` & `numpyneuron-0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name="numpyneuron",
-    version="0.1",
+    version="0.2",
     author="Jensen Holm",
     author_email="jensen.dev.01@gmail.com",
     description="Simple, lightweight neural network framework built in numpy",
     long_description=open("about_package.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Jensen-holm/Numpy-Neuron",
     project_urls={"Bug Tracker": "https://github.com/Jensen-holm/Numpy-Neuron/issues"},
-    package_dir={"": "nn"},
-    packages=find_packages(where="nn"),
+    package_dir={"": "numpyneuron"},
+    packages=find_packages(where="numpyneuron"),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
 )
```

