# Comparing `tmp/FrustrationDynamiX-0.2.1.tar.gz` & `tmp/FrustrationDynamiX-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FrustrationDynamiX-0.2.1.tar", last modified: Sat Apr 20 20:39:51 2024, max compression
+gzip compressed data, was "FrustrationDynamiX-0.2.2.tar", last modified: Sat Apr 20 21:37:48 2024, max compression
```

## Comparing `FrustrationDynamiX-0.2.1.tar` & `FrustrationDynamiX-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 20:39:51.479250 FrustrationDynamiX-0.2.1/
-drwxrwxrwx   0        0        0        0 2024-04-20 20:39:51.449598 FrustrationDynamiX-0.2.1/FrustrationDynamiX/
--rw-rw-rw-   0        0        0       36 2024-04-19 23:23:05.000000 FrustrationDynamiX-0.2.1/FrustrationDynamiX/__init__.py
--rw-rw-rw-   0        0        0    25409 2024-04-19 23:18:01.000000 FrustrationDynamiX-0.2.1/FrustrationDynamiX/core.py
-drwxrwxrwx   0        0        0        0 2024-04-20 20:39:51.479250 FrustrationDynamiX-0.2.1/FrustrationDynamiX.egg-info/
--rw-rw-rw-   0        0        0     1370 2024-04-20 20:39:51.000000 FrustrationDynamiX-0.2.1/FrustrationDynamiX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2024-04-20 20:39:51.000000 FrustrationDynamiX-0.2.1/FrustrationDynamiX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 20:39:51.000000 FrustrationDynamiX-0.2.1/FrustrationDynamiX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-04-20 20:39:51.000000 FrustrationDynamiX-0.2.1/FrustrationDynamiX.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-20 20:39:51.000000 FrustrationDynamiX-0.2.1/FrustrationDynamiX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1094 2024-04-20 20:30:54.000000 FrustrationDynamiX-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     1370 2024-04-20 20:39:51.479250 FrustrationDynamiX-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      600 2024-04-20 20:05:17.000000 FrustrationDynamiX-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-20 20:39:51.482036 FrustrationDynamiX-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1125 2024-04-20 20:39:45.000000 FrustrationDynamiX-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 21:37:48.023747 FrustrationDynamiX-0.2.2/
+drwxrwxrwx   0        0        0        0 2024-04-20 21:37:47.978192 FrustrationDynamiX-0.2.2/FrustrationDynamiX/
+-rw-rw-rw-   0        0        0       36 2024-04-19 23:23:05.000000 FrustrationDynamiX-0.2.2/FrustrationDynamiX/__init__.py
+-rw-rw-rw-   0        0        0    25473 2024-04-20 21:37:34.000000 FrustrationDynamiX-0.2.2/FrustrationDynamiX/core.py
+drwxrwxrwx   0        0        0        0 2024-04-20 21:37:48.017748 FrustrationDynamiX-0.2.2/FrustrationDynamiX.egg-info/
+-rw-rw-rw-   0        0        0     1370 2024-04-20 21:37:47.000000 FrustrationDynamiX-0.2.2/FrustrationDynamiX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-04-20 21:37:47.000000 FrustrationDynamiX-0.2.2/FrustrationDynamiX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 21:37:47.000000 FrustrationDynamiX-0.2.2/FrustrationDynamiX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-04-20 21:37:47.000000 FrustrationDynamiX-0.2.2/FrustrationDynamiX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-20 21:37:47.000000 FrustrationDynamiX-0.2.2/FrustrationDynamiX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1094 2024-04-20 20:30:54.000000 FrustrationDynamiX-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     1370 2024-04-20 21:37:48.022747 FrustrationDynamiX-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2024-04-20 20:05:17.000000 FrustrationDynamiX-0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-20 21:37:48.024747 FrustrationDynamiX-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1125 2024-04-20 21:37:39.000000 FrustrationDynamiX-0.2.2/setup.py
```

### Comparing `FrustrationDynamiX-0.2.1/FrustrationDynamiX/core.py` & `FrustrationDynamiX-0.2.2/FrustrationDynamiX/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -589,11 +589,12 @@
             #assert self.frustration != None, "Missing call: compute_frustration_evolution method should be called first"
             plt.plot(self.time_vector, self.cohesiveness, marker = "x")
             plt.plot(self.time_vector, self.divisiveness, marker = "x")
         
         plt.xlabel(xlabel)
         plt.ylabel(ylabel)
         plt.title(title)
+        plt.legend(loc='center left', bbox_to_anchor=(1, 0.5))
         if save_plot != None:
             assert type(save_plot) == str, "save_plot variable should have type string, type " + str(type(save_plot)) + " was given instead"
             plt.savefig(save_plot)
         plt.show()
```

### Comparing `FrustrationDynamiX-0.2.1/FrustrationDynamiX.egg-info/PKG-INFO` & `FrustrationDynamiX-0.2.2/FrustrationDynamiX.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FrustrationDynamiX
-Version: 0.2.1
+Version: 0.2.2
 Summary: A package for handling computing frustration in dynamical systems
 Home-page: https://github.com/asb24repo/FrustrationDynamiX
 Author: Ali S. Badereddine
 Author-email: asb24@mail.aub.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FrustrationDynamiX-0.2.1/LICENSE` & `FrustrationDynamiX-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FrustrationDynamiX-0.2.1/PKG-INFO` & `FrustrationDynamiX-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FrustrationDynamiX
-Version: 0.2.1
+Version: 0.2.2
 Summary: A package for handling computing frustration in dynamical systems
 Home-page: https://github.com/asb24repo/FrustrationDynamiX
 Author: Ali S. Badereddine
 Author-email: asb24@mail.aub.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `FrustrationDynamiX-0.2.1/README.md` & `FrustrationDynamiX-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `FrustrationDynamiX-0.2.1/setup.py` & `FrustrationDynamiX-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FrustrationDynamiX',
-    version='0.2.1',
+    version='0.2.2',
     packages=find_packages(),
     description='A package for handling computing frustration in dynamical systems',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Ali S. Badereddine',
     author_email='asb24@mail.aub.edu',
     license='MIT',
```

