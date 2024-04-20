# Comparing `tmp/skbu-2nd-sem-1.0.0.tar.gz` & `tmp/skbu_2nd_sem-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skbu-2nd-sem-1.0.0.tar", last modified: Sat Apr 20 10:44:23 2024, max compression
+gzip compressed data, was "skbu_2nd_sem-1.0.1.tar", last modified: Sat Apr 20 10:57:57 2024, max compression
```

## Comparing `skbu-2nd-sem-1.0.0.tar` & `skbu_2nd_sem-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 10:44:23.639841 skbu-2nd-sem-1.0.0/
--rw-rw-rw-   0        0        0     2208 2024-04-20 10:44:23.639841 skbu-2nd-sem-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1722 2024-04-20 04:58:31.000000 skbu-2nd-sem-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 10:44:23.541576 skbu-2nd-sem-1.0.0/data_structures/
--rw-rw-rw-   0        0        0        0 2024-04-20 06:36:35.000000 skbu-2nd-sem-1.0.0/data_structures/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-20 10:44:23.639841 skbu-2nd-sem-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      752 2024-04-20 04:52:23.000000 skbu-2nd-sem-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 10:44:23.627195 skbu-2nd-sem-1.0.0/skbu_2nd_sem.egg-info/
--rw-rw-rw-   0        0        0     2208 2024-04-20 10:44:23.000000 skbu-2nd-sem-1.0.0/skbu_2nd_sem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-04-20 10:44:23.000000 skbu-2nd-sem-1.0.0/skbu_2nd_sem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 10:44:23.000000 skbu-2nd-sem-1.0.0/skbu_2nd_sem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-04-20 10:44:23.000000 skbu-2nd-sem-1.0.0/skbu_2nd_sem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-20 10:44:23.000000 skbu-2nd-sem-1.0.0/skbu_2nd_sem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 10:57:57.042068 skbu_2nd_sem-1.0.1/
+-rw-rw-rw-   0        0        0     2208 2024-04-20 10:57:57.031623 skbu_2nd_sem-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1722 2024-04-20 10:55:24.000000 skbu_2nd_sem-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 10:57:57.007518 skbu_2nd_sem-1.0.1/data_structures/
+-rw-rw-rw-   0        0        0        0 2024-04-20 06:36:35.000000 skbu_2nd_sem-1.0.1/data_structures/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-20 10:57:57.042068 skbu_2nd_sem-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      663 2024-04-20 10:57:30.000000 skbu_2nd_sem-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:57:57.031623 skbu_2nd_sem-1.0.1/skbu_2nd_sem.egg-info/
+-rw-rw-rw-   0        0        0     2208 2024-04-20 10:57:56.000000 skbu_2nd_sem-1.0.1/skbu_2nd_sem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-04-20 10:57:56.000000 skbu_2nd_sem-1.0.1/skbu_2nd_sem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 10:57:56.000000 skbu_2nd_sem-1.0.1/skbu_2nd_sem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-20 10:57:56.000000 skbu_2nd_sem-1.0.1/skbu_2nd_sem.egg-info/top_level.txt
```

### Comparing `skbu-2nd-sem-1.0.0/PKG-INFO` & `skbu_2nd_sem-1.0.1/skbu_2nd_sem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skbu-2nd-sem
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package for implementing data structures and algorithms for SKBU 2nd semester syllabus.
 Home-page: https://github.com/PB2204/SKBU-2nd-Sem
 Author: Pabitra Banerjee
 Author-email: pabitra.banerjee@explorecode.live
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 This Python package provides implementations of various data structures and algorithms as per the syllabus of the 2nd semester of Sidho Kanho Birsha University (SKBU). It covers topics such as arrays, linked lists, stacks, queues, recursion, trees, graphs, searching, sorting, and hashing.
 
 ## Installation
 
 You can install the package using pip:
 
 ```bash
-pip install skbu-2nd-sem
+pip install skbu_2nd_sem
 ```
 
 ## Usage
 
 To use the package, simply import the desired modules:
 
 ```python
```

### Comparing `skbu-2nd-sem-1.0.0/README.md` & `skbu_2nd_sem-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,31 @@
+Metadata-Version: 2.1
+Name: skbu_2nd_sem
+Version: 1.0.1
+Summary: A Python package for implementing data structures and algorithms for SKBU 2nd semester syllabus.
+Home-page: https://github.com/PB2204/SKBU-2nd-Sem
+Author: Pabitra Banerjee
+Author-email: pabitra.banerjee@explorecode.live
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+
 # SKBU 2nd Semester Python Package
 
 ## Overview
 
 This Python package provides implementations of various data structures and algorithms as per the syllabus of the 2nd semester of Sidho Kanho Birsha University (SKBU). It covers topics such as arrays, linked lists, stacks, queues, recursion, trees, graphs, searching, sorting, and hashing.
 
 ## Installation
 
 You can install the package using pip:
 
 ```bash
-pip install skbu-2nd-sem
+pip install skbu_2nd_sem
 ```
 
 ## Usage
 
 To use the package, simply import the desired modules:
 
 ```python
@@ -42,8 +54,8 @@
 - **Email:** pabitra.banerjee@explorecode.live
 - **LinkedIn:** [Pabitra Banerjee](https://www.linkedin.com/in/pabitra-banerjee)
 - **Twitter:** [@FossilianBhed](https://twitter.com/FossilianBhed)
 - **Website:** [Code Explorer](https://explorecode.live/)
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE](https://github.com/PB2204/SKBU-2nd-Sem/blob/main/LICENSE) file for details.
+This project is licensed under the MIT License - see the [LICENSE](https://github.com/PB2204/SKBU-2nd-Sem/blob/main/LICENSE) file for details.
```

### Comparing `skbu-2nd-sem-1.0.0/setup.py` & `skbu_2nd_sem-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='skbu-2nd-sem',
-    version='1.0.0',
+    name='skbu_2nd_sem',
+    version='1.0.1',
     packages=find_packages(),
-    install_requires=[
-        'pytest==6.2.4',
-        'pytest-cov==2.12.1',
-    ],
     author='Pabitra Banerjee',
     author_email='pabitra.banerjee@explorecode.live',
     description='A Python package for implementing data structures and algorithms for SKBU 2nd semester syllabus.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/PB2204/SKBU-2nd-Sem',
     classifiers=[
```

### Comparing `skbu-2nd-sem-1.0.0/skbu_2nd_sem.egg-info/PKG-INFO` & `skbu_2nd_sem-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,19 @@
-Metadata-Version: 2.1
-Name: skbu-2nd-sem
-Version: 1.0.0
-Summary: A Python package for implementing data structures and algorithms for SKBU 2nd semester syllabus.
-Home-page: https://github.com/PB2204/SKBU-2nd-Sem
-Author: Pabitra Banerjee
-Author-email: pabitra.banerjee@explorecode.live
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 # SKBU 2nd Semester Python Package
 
 ## Overview
 
 This Python package provides implementations of various data structures and algorithms as per the syllabus of the 2nd semester of Sidho Kanho Birsha University (SKBU). It covers topics such as arrays, linked lists, stacks, queues, recursion, trees, graphs, searching, sorting, and hashing.
 
 ## Installation
 
 You can install the package using pip:
 
 ```bash
-pip install skbu-2nd-sem
+pip install skbu_2nd_sem
 ```
 
 ## Usage
 
 To use the package, simply import the desired modules:
 
 ```python
@@ -54,8 +42,8 @@
 - **Email:** pabitra.banerjee@explorecode.live
 - **LinkedIn:** [Pabitra Banerjee](https://www.linkedin.com/in/pabitra-banerjee)
 - **Twitter:** [@FossilianBhed](https://twitter.com/FossilianBhed)
 - **Website:** [Code Explorer](https://explorecode.live/)
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE](https://github.com/PB2204/SKBU-2nd-Sem/blob/main/LICENSE) file for details.
+This project is licensed under the MIT License - see the [LICENSE](https://github.com/PB2204/SKBU-2nd-Sem/blob/main/LICENSE) file for details.
```

