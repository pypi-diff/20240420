# Comparing `tmp/cerbogen-0.0.30.tar.gz` & `tmp/cerbogen-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbogen-0.0.30.tar", last modified: Sat Apr 20 15:05:48 2024, max compression
+gzip compressed data, was "cerbogen-0.0.31.tar", last modified: Sat Apr 20 15:08:22 2024, max compression
```

## Comparing `cerbogen-0.0.30.tar` & `cerbogen-0.0.31.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 15:05:48.003806 cerbogen-0.0.30/
--rw-rw-rw-   0        0        0      680 2024-04-20 15:05:48.002830 cerbogen-0.0.30/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.30/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 15:05:47.984286 cerbogen-0.0.30/cerbogen/
--rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.30/cerbogen/__init__.py
--rw-rw-rw-   0        0        0     8764 2024-04-20 13:28:49.000000 cerbogen-0.0.30/cerbogen/cerbogen.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:05:47.981358 cerbogen-0.0.30/cerbogen/data/
-drwxrwxrwx   0        0        0        0 2024-04-20 15:05:47.996974 cerbogen-0.0.30/cerbogen/data/img/
--rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.30/cerbogen/data/img/logo.ico
--rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.30/cerbogen/data/img/logo.png
--rw-rw-rw-   0        0        0    10309 2024-04-20 15:03:10.000000 cerbogen-0.0.30/cerbogen/main.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:05:48.001856 cerbogen-0.0.30/cerbogen/mod/
--rw-rw-rw-   0        0        0     2772 2024-04-20 14:15:38.000000 cerbogen-0.0.30/cerbogen/mod/after_install.py
--rw-rw-rw-   0        0        0     9190 2024-04-20 12:45:58.000000 cerbogen-0.0.30/cerbogen/mod/cerbogen.py
--rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.30/cerbogen/mod/check.py
--rw-rw-rw-   0        0        0     2928 2024-04-20 13:25:55.000000 cerbogen-0.0.30/cerbogen/mod/ffmpeg_install.py
--rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.30/cerbogen/mod/plot.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:05:48.002830 cerbogen-0.0.30/cerbogen.egg-info/
--rw-rw-rw-   0        0        0      680 2024-04-20 15:05:47.000000 cerbogen-0.0.30/cerbogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2024-04-20 15:05:47.000000 cerbogen-0.0.30/cerbogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 15:05:47.000000 cerbogen-0.0.30/cerbogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-04-20 15:05:47.000000 cerbogen-0.0.30/cerbogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-20 15:05:47.000000 cerbogen-0.0.30/cerbogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 15:05:48.003806 cerbogen-0.0.30/setup.cfg
--rw-rw-rw-   0        0        0     1372 2024-04-20 15:05:47.000000 cerbogen-0.0.30/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:08:22.125955 cerbogen-0.0.31/
+-rw-rw-rw-   0        0        0      680 2024-04-20 15:08:22.124980 cerbogen-0.0.31/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.31/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 15:08:22.106435 cerbogen-0.0.31/cerbogen/
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.31/cerbogen/__init__.py
+-rw-rw-rw-   0        0        0     8764 2024-04-20 13:28:49.000000 cerbogen-0.0.31/cerbogen/cerbogen.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:08:22.097651 cerbogen-0.0.31/cerbogen/data/
+drwxrwxrwx   0        0        0        0 2024-04-20 15:08:22.118147 cerbogen-0.0.31/cerbogen/data/img/
+-rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.31/cerbogen/data/img/logo.ico
+-rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.31/cerbogen/data/img/logo.png
+-rw-rw-rw-   0        0        0    10291 2024-04-20 15:08:11.000000 cerbogen-0.0.31/cerbogen/main.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:08:22.123027 cerbogen-0.0.31/cerbogen/mod/
+-rw-rw-rw-   0        0        0     2772 2024-04-20 14:15:38.000000 cerbogen-0.0.31/cerbogen/mod/after_install.py
+-rw-rw-rw-   0        0        0     9190 2024-04-20 12:45:58.000000 cerbogen-0.0.31/cerbogen/mod/cerbogen.py
+-rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.31/cerbogen/mod/check.py
+-rw-rw-rw-   0        0        0     2928 2024-04-20 13:25:55.000000 cerbogen-0.0.31/cerbogen/mod/ffmpeg_install.py
+-rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.31/cerbogen/mod/plot.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:08:22.124003 cerbogen-0.0.31/cerbogen.egg-info/
+-rw-rw-rw-   0        0        0      680 2024-04-20 15:08:21.000000 cerbogen-0.0.31/cerbogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2024-04-20 15:08:22.000000 cerbogen-0.0.31/cerbogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 15:08:21.000000 cerbogen-0.0.31/cerbogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-20 15:08:21.000000 cerbogen-0.0.31/cerbogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-20 15:08:21.000000 cerbogen-0.0.31/cerbogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 15:08:22.125955 cerbogen-0.0.31/setup.cfg
+-rw-rw-rw-   0        0        0     1372 2024-04-20 15:08:21.000000 cerbogen-0.0.31/setup.py
```

### Comparing `cerbogen-0.0.30/PKG-INFO` & `cerbogen-0.0.31/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.30
+Version: 0.0.31
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.30/cerbogen/cerbogen.py` & `cerbogen-0.0.31/cerbogen/cerbogen.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.30/cerbogen/data/img/logo.ico` & `cerbogen-0.0.31/cerbogen/data/img/logo.ico`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.30/cerbogen/data/img/logo.png` & `cerbogen-0.0.31/cerbogen/data/img/logo.png`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.30/cerbogen/main.py` & `cerbogen-0.0.31/cerbogen/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import tkinter as tk
 from tkinter import ttk
 from tkinter import messagebox
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 
-from cerbogen.mod.cerbogen import binbeats
-from cerbogen.mod.plot import Plot
+from mod.cerbogen import binbeats
+from mod.plot import Plot
 
 def generate_binaural_beats():
     base_f = float(base_entry.get())
     diff = float(diff_entry.get())
     duration = int(duration_entry.get())
     output_file = output_bin_entry.get()
     selected_format = format_combobox.get()
```

### Comparing `cerbogen-0.0.30/cerbogen/mod/after_install.py` & `cerbogen-0.0.31/cerbogen/mod/after_install.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.30/cerbogen/mod/cerbogen.py` & `cerbogen-0.0.31/cerbogen/mod/cerbogen.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.30/cerbogen/mod/check.py` & `cerbogen-0.0.31/cerbogen/mod/check.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.30/cerbogen/mod/ffmpeg_install.py` & `cerbogen-0.0.31/cerbogen/mod/ffmpeg_install.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.30/cerbogen/mod/plot.py` & `cerbogen-0.0.31/cerbogen/mod/plot.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.30/cerbogen.egg-info/PKG-INFO` & `cerbogen-0.0.31/cerbogen.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.30
+Version: 0.0.31
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.30/setup.py` & `cerbogen-0.0.31/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class PostInstallCommand(install):
     def run(self):
         install.run(self)
         subprocess.call([sys.executable, os.path.join(self.install_lib, 'cerbogen', 'setup.py')])
 
 setup(
     name='cerbogen',
-    version = '0.0.30',
+    version = '0.0.31',
     description='A Python package for CerboTech',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Clarence Parmar',
     author_email='git.clarence@gmail.com',
     url='https://github.com/clarenceparmar/cerbogen',
     packages=find_packages(),
```

