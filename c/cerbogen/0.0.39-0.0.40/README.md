# Comparing `tmp/cerbogen-0.0.39.tar.gz` & `tmp/cerbogen-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbogen-0.0.39.tar", last modified: Sat Apr 20 16:50:04 2024, max compression
+gzip compressed data, was "cerbogen-0.0.40.tar", last modified: Sat Apr 20 16:51:20 2024, max compression
```

## Comparing `cerbogen-0.0.39.tar` & `cerbogen-0.0.40.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 16:50:04.060896 cerbogen-0.0.39/
--rw-rw-rw-   0        0        0      680 2024-04-20 16:50:04.059921 cerbogen-0.0.39/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.39/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 16:50:04.021856 cerbogen-0.0.39/cerbogen/
--rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.39/cerbogen/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 16:50:04.019904 cerbogen-0.0.39/cerbogen/data/
-drwxrwxrwx   0        0        0        0 2024-04-20 16:50:04.046257 cerbogen-0.0.39/cerbogen/data/img/
--rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.39/cerbogen/data/img/logo.ico
--rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.39/cerbogen/data/img/logo.png
-drwxrwxrwx   0        0        0        0 2024-04-20 16:50:04.057968 cerbogen-0.0.39/cerbogen/mod/
--rw-rw-rw-   0        0        0        0 2024-04-20 16:21:25.000000 cerbogen-0.0.39/cerbogen/mod/__init__.py
--rw-rw-rw-   0        0        0     9107 2024-04-20 15:20:54.000000 cerbogen-0.0.39/cerbogen/mod/cerbogen.py
--rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.39/cerbogen/mod/check.py
--rw-rw-rw-   0        0        0     2930 2024-04-20 16:38:30.000000 cerbogen-0.0.39/cerbogen/mod/install_ffmpeg.py
--rw-rw-rw-   0        0        0     2428 2024-04-20 16:45:37.000000 cerbogen-0.0.39/cerbogen/mod/install_location.py
--rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.39/cerbogen/mod/plot.py
--rw-rw-rw-   0        0        0     2051 2024-04-20 16:41:49.000000 cerbogen-0.0.39/cerbogen/mod/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 16:50:04.058944 cerbogen-0.0.39/cerbogen.egg-info/
--rw-rw-rw-   0        0        0      680 2024-04-20 16:50:03.000000 cerbogen-0.0.39/cerbogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      466 2024-04-20 16:50:03.000000 cerbogen-0.0.39/cerbogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 16:50:03.000000 cerbogen-0.0.39/cerbogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2024-04-20 16:50:03.000000 cerbogen-0.0.39/cerbogen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       31 2024-04-20 16:50:03.000000 cerbogen-0.0.39/cerbogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-20 16:50:03.000000 cerbogen-0.0.39/cerbogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 16:50:04.060896 cerbogen-0.0.39/setup.cfg
--rw-rw-rw-   0        0        0     1172 2024-04-20 16:50:03.000000 cerbogen-0.0.39/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:51:20.012924 cerbogen-0.0.40/
+-rw-rw-rw-   0        0        0      680 2024-04-20 16:51:20.010973 cerbogen-0.0.40/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.40/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 16:51:19.927034 cerbogen-0.0.40/cerbogen/
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.40/cerbogen/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:51:19.926057 cerbogen-0.0.40/cerbogen/data/
+drwxrwxrwx   0        0        0        0 2024-04-20 16:51:19.944601 cerbogen-0.0.40/cerbogen/data/img/
+-rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.40/cerbogen/data/img/logo.ico
+-rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.40/cerbogen/data/img/logo.png
+drwxrwxrwx   0        0        0        0 2024-04-20 16:51:20.006091 cerbogen-0.0.40/cerbogen/mod/
+-rw-rw-rw-   0        0        0        0 2024-04-20 16:21:25.000000 cerbogen-0.0.40/cerbogen/mod/__init__.py
+-rw-rw-rw-   0        0        0     9107 2024-04-20 15:20:54.000000 cerbogen-0.0.40/cerbogen/mod/cerbogen.py
+-rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.40/cerbogen/mod/check.py
+-rw-rw-rw-   0        0        0     2930 2024-04-20 16:38:30.000000 cerbogen-0.0.40/cerbogen/mod/install_ffmpeg.py
+-rw-rw-rw-   0        0        0     2428 2024-04-20 16:45:37.000000 cerbogen-0.0.40/cerbogen/mod/install_location.py
+-rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.40/cerbogen/mod/plot.py
+-rw-rw-rw-   0        0        0     2051 2024-04-20 16:41:49.000000 cerbogen-0.0.40/cerbogen/mod/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:51:20.009019 cerbogen-0.0.40/cerbogen.egg-info/
+-rw-rw-rw-   0        0        0      680 2024-04-20 16:51:19.000000 cerbogen-0.0.40/cerbogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2024-04-20 16:51:19.000000 cerbogen-0.0.40/cerbogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 16:51:19.000000 cerbogen-0.0.40/cerbogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-20 16:51:19.000000 cerbogen-0.0.40/cerbogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-20 16:51:19.000000 cerbogen-0.0.40/cerbogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 16:51:20.013900 cerbogen-0.0.40/setup.cfg
+-rw-rw-rw-   0        0        0     1062 2024-04-20 16:51:19.000000 cerbogen-0.0.40/setup.py
```

### Comparing `cerbogen-0.0.39/PKG-INFO` & `cerbogen-0.0.40/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.39
+Version: 0.0.40
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.39/cerbogen/data/img/logo.ico` & `cerbogen-0.0.40/cerbogen/data/img/logo.ico`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.39/cerbogen/data/img/logo.png` & `cerbogen-0.0.40/cerbogen/data/img/logo.png`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.39/cerbogen/mod/cerbogen.py` & `cerbogen-0.0.40/cerbogen/mod/cerbogen.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.39/cerbogen/mod/check.py` & `cerbogen-0.0.40/cerbogen/mod/check.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.39/cerbogen/mod/install_ffmpeg.py` & `cerbogen-0.0.40/cerbogen/mod/install_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.39/cerbogen/mod/install_location.py` & `cerbogen-0.0.40/cerbogen/mod/install_location.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.39/cerbogen/mod/plot.py` & `cerbogen-0.0.40/cerbogen/mod/plot.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.39/cerbogen/mod/setup.py` & `cerbogen-0.0.40/cerbogen/mod/setup.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.39/cerbogen.egg-info/PKG-INFO` & `cerbogen-0.0.40/cerbogen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.39
+Version: 0.0.40
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.39/setup.py` & `cerbogen-0.0.40/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cerbogen',
-    version = '0.0.39',
+    version = '0.0.40',
     description='A Python package for CerboTech',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Clarence Parmar',
     author_email='git.clarence@gmail.com',
     url='https://github.com/clarenceparmar/cerbogen',
     packages=find_packages(),
@@ -25,14 +25,10 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
 
-    # Specify the entry point to execute the install_location function
-    entry_points={
-        'console_scripts': [
-            'install_cerbogen=cerbogen.mod.install_location:install_location',
-        ],
-    }
+    # Specify the script to be executed during installation
+    scripts=['cerbogen/mod/install_location.py']
 )
```

