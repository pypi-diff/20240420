# Comparing `tmp/flechemano-0.6.tar.gz` & `tmp/flechemano-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flechemano-0.6.tar", last modified: Sat Apr 20 08:15:09 2024, max compression
+gzip compressed data, was "flechemano-0.8.tar", last modified: Sat Apr 20 08:20:11 2024, max compression
```

## Comparing `flechemano-0.6.tar` & `flechemano-0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 08:15:09.927552 flechemano-0.6/
--rw-r--r--   0 root         (0) root         (0)      683 2024-04-20 08:15:09.927552 flechemano-0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      387 2024-04-20 07:51:01.000000 flechemano-0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 08:15:09.927552 flechemano-0.6/flechemano.egg-info/
--rw-r--r--   0 root         (0) root         (0)      683 2024-04-20 08:15:09.000000 flechemano-0.6/flechemano.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      191 2024-04-20 08:15:09.000000 flechemano-0.6/flechemano.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 08:15:09.000000 flechemano-0.6/flechemano.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2024-04-20 08:15:09.000000 flechemano-0.6/flechemano.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 08:15:09.000000 flechemano-0.6/flechemano.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 08:15:09.927552 flechemano-0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      529 2024-04-20 08:15:08.000000 flechemano-0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 08:20:11.384731 flechemano-0.8/
+-rw-r--r--   0 root         (0) root         (0)      683 2024-04-20 08:20:11.384731 flechemano-0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      387 2024-04-20 07:51:01.000000 flechemano-0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 08:20:11.384731 flechemano-0.8/flechemano.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      683 2024-04-20 08:20:11.000000 flechemano-0.8/flechemano.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      191 2024-04-20 08:20:11.000000 flechemano-0.8/flechemano.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 08:20:11.000000 flechemano-0.8/flechemano.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2024-04-20 08:20:11.000000 flechemano-0.8/flechemano.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 08:20:11.000000 flechemano-0.8/flechemano.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 08:20:11.384731 flechemano-0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      578 2024-04-20 08:20:04.000000 flechemano-0.8/setup.py
```

### Comparing `flechemano-0.6/PKG-INFO` & `flechemano-0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flechemano
-Version: 0.6
+Version: 0.8
 Summary: A package developed for blacktea024 to integrate it with PyPI.
 Home-page: https://github.com/flechemano/flechemano
 Author: flechemano
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `flechemano-0.6/flechemano.egg-info/PKG-INFO` & `flechemano-0.8/flechemano.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flechemano
-Version: 0.6
+Version: 0.8
 Summary: A package developed for blacktea024 to integrate it with PyPI.
 Home-page: https://github.com/flechemano/flechemano
 Author: flechemano
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `flechemano-0.6/setup.py` & `flechemano-0.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='flechemano',
-    version='0.6',
+    version='0.8',
     description='A package developed for blacktea024 to integrate it with PyPI.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='flechemano',
     url='https://github.com/flechemano/flechemano',
     packages=find_packages(),
     python_requires='>=3.6',
+    package_data={'flechemano': ['install.py']},
     entry_points={
         'console_scripts': [
             'run_install = flechemano.install:main'
         ]
     }
 )
```

