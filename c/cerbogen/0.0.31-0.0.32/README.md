# Comparing `tmp/cerbogen-0.0.31.tar.gz` & `tmp/cerbogen-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbogen-0.0.31.tar", last modified: Sat Apr 20 15:08:22 2024, max compression
+gzip compressed data, was "cerbogen-0.0.32.tar", last modified: Sat Apr 20 15:17:47 2024, max compression
```

## Comparing `cerbogen-0.0.31.tar` & `cerbogen-0.0.32.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 15:08:22.125955 cerbogen-0.0.31/
--rw-rw-rw-   0        0        0      680 2024-04-20 15:08:22.124980 cerbogen-0.0.31/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.31/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 15:08:22.106435 cerbogen-0.0.31/cerbogen/
--rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.31/cerbogen/__init__.py
--rw-rw-rw-   0        0        0     8764 2024-04-20 13:28:49.000000 cerbogen-0.0.31/cerbogen/cerbogen.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:08:22.097651 cerbogen-0.0.31/cerbogen/data/
-drwxrwxrwx   0        0        0        0 2024-04-20 15:08:22.118147 cerbogen-0.0.31/cerbogen/data/img/
--rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.31/cerbogen/data/img/logo.ico
--rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.31/cerbogen/data/img/logo.png
--rw-rw-rw-   0        0        0    10291 2024-04-20 15:08:11.000000 cerbogen-0.0.31/cerbogen/main.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:08:22.123027 cerbogen-0.0.31/cerbogen/mod/
--rw-rw-rw-   0        0        0     2772 2024-04-20 14:15:38.000000 cerbogen-0.0.31/cerbogen/mod/after_install.py
--rw-rw-rw-   0        0        0     9190 2024-04-20 12:45:58.000000 cerbogen-0.0.31/cerbogen/mod/cerbogen.py
--rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.31/cerbogen/mod/check.py
--rw-rw-rw-   0        0        0     2928 2024-04-20 13:25:55.000000 cerbogen-0.0.31/cerbogen/mod/ffmpeg_install.py
--rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.31/cerbogen/mod/plot.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:08:22.124003 cerbogen-0.0.31/cerbogen.egg-info/
--rw-rw-rw-   0        0        0      680 2024-04-20 15:08:21.000000 cerbogen-0.0.31/cerbogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2024-04-20 15:08:22.000000 cerbogen-0.0.31/cerbogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 15:08:21.000000 cerbogen-0.0.31/cerbogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-04-20 15:08:21.000000 cerbogen-0.0.31/cerbogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-20 15:08:21.000000 cerbogen-0.0.31/cerbogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 15:08:22.125955 cerbogen-0.0.31/setup.cfg
--rw-rw-rw-   0        0        0     1372 2024-04-20 15:08:21.000000 cerbogen-0.0.31/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:17:47.700655 cerbogen-0.0.32/
+-rw-rw-rw-   0        0        0      680 2024-04-20 15:17:47.699678 cerbogen-0.0.32/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.32/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 15:17:47.679182 cerbogen-0.0.32/cerbogen/
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.32/cerbogen/__init__.py
+-rw-rw-rw-   0        0        0     8764 2024-04-20 13:28:49.000000 cerbogen-0.0.32/cerbogen/cerbogen.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:17:47.676254 cerbogen-0.0.32/cerbogen/data/
+drwxrwxrwx   0        0        0        0 2024-04-20 15:17:47.692846 cerbogen-0.0.32/cerbogen/data/img/
+-rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.32/cerbogen/data/img/logo.ico
+-rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.32/cerbogen/data/img/logo.png
+-rw-rw-rw-   0        0        0    10191 2024-04-20 15:17:40.000000 cerbogen-0.0.32/cerbogen/main.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:17:47.697727 cerbogen-0.0.32/cerbogen/mod/
+-rw-rw-rw-   0        0        0     2902 2024-04-20 15:17:36.000000 cerbogen-0.0.32/cerbogen/mod/after_install.py
+-rw-rw-rw-   0        0        0     9196 2024-04-20 15:11:37.000000 cerbogen-0.0.32/cerbogen/mod/cerbogen.py
+-rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.32/cerbogen/mod/check.py
+-rw-rw-rw-   0        0        0     2928 2024-04-20 13:25:55.000000 cerbogen-0.0.32/cerbogen/mod/ffmpeg_install.py
+-rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.32/cerbogen/mod/plot.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:17:47.698702 cerbogen-0.0.32/cerbogen.egg-info/
+-rw-rw-rw-   0        0        0      680 2024-04-20 15:17:47.000000 cerbogen-0.0.32/cerbogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2024-04-20 15:17:47.000000 cerbogen-0.0.32/cerbogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 15:17:47.000000 cerbogen-0.0.32/cerbogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-20 15:17:47.000000 cerbogen-0.0.32/cerbogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-20 15:17:47.000000 cerbogen-0.0.32/cerbogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 15:17:47.700655 cerbogen-0.0.32/setup.cfg
+-rw-rw-rw-   0        0        0     1372 2024-04-20 15:17:47.000000 cerbogen-0.0.32/setup.py
```

### Comparing `cerbogen-0.0.31/PKG-INFO` & `cerbogen-0.0.32/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.31
+Version: 0.0.32
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.31/cerbogen/cerbogen.py` & `cerbogen-0.0.32/cerbogen/cerbogen.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.31/cerbogen/data/img/logo.ico` & `cerbogen-0.0.32/cerbogen/data/img/logo.ico`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.31/cerbogen/data/img/logo.png` & `cerbogen-0.0.32/cerbogen/data/img/logo.png`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.31/cerbogen/main.py` & `cerbogen-0.0.32/cerbogen/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import subprocess
-
 import tkinter as tk
 from tkinter import ttk
 from tkinter import messagebox
-import matplotlib.pyplot as plt
-from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 
 from mod.cerbogen import binbeats
 from mod.plot import Plot
 
 def generate_binaural_beats():
     base_f = float(base_entry.get())
     diff = float(diff_entry.get())
```

### Comparing `cerbogen-0.0.31/cerbogen/mod/after_install.py` & `cerbogen-0.0.32/cerbogen/mod/after_install.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,21 +37,25 @@
         # Create Windows shortcut
         try:
             from win32com.client import Dispatch
         except ImportError:
             print("pywin32 not found. Install it to create shortcuts on Windows.")
             sys.exit(1)
         
+        script_dir = os.path.dirname(os.path.abspath(__file__))
+        icon_path = os.path.join(script_dir, "data", "img", "logo.ico")
+
         shell = Dispatch('WScript.Shell')
         shortcut = shell.CreateShortCut(shortcut_path)
         shortcut.TargetPath = python_exe
         shortcut.Arguments = ui_py_path
         shortcut.WorkingDirectory = os.path.dirname(ui_py_path)
-        shortcut.IconLocation = "./data/img/logo.ico"
+        shortcut.IconLocation = icon_path
         shortcut.save()
+
     else:
         # Create shortcut for Linux and macOS
         with open(shortcut_path, 'w') as shortcut_file:
             shortcut_file.write("[Desktop Entry]\n")
             shortcut_file.write("Name=Cerbogen UI\n")
             shortcut_file.write("Exec={} {}\n".format(python_exe, ui_py_path))
             shortcut_file.write("Type=Application\n")
```

### Comparing `cerbogen-0.0.31/cerbogen/mod/cerbogen.py` & `cerbogen-0.0.32/cerbogen/mod/cerbogen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import platform
+
 from pydub import AudioSegment
 import numpy as np
-from plot import Plot
-import platform
+
 from pydub import AudioSegment
 
+from plot import Plot
+
 # # Set the path to FFmpeg based on the operating system
 # if platform.system() == "Windows":
 #     # Path to FFmpeg for Windows
 #     AudioSegment.converter = "./ffmpeg/win/bin/ffmpeg.exe"
 # else:
 #     # Path to FFmpeg for macOS or Linux
 #     AudioSegment.converter = "./ffmpeg/mac/ffmpeg"
```

### Comparing `cerbogen-0.0.31/cerbogen/mod/check.py` & `cerbogen-0.0.32/cerbogen/mod/check.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.31/cerbogen/mod/ffmpeg_install.py` & `cerbogen-0.0.32/cerbogen/mod/ffmpeg_install.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.31/cerbogen/mod/plot.py` & `cerbogen-0.0.32/cerbogen/mod/plot.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.31/cerbogen.egg-info/PKG-INFO` & `cerbogen-0.0.32/cerbogen.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.31
+Version: 0.0.32
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.31/setup.py` & `cerbogen-0.0.32/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class PostInstallCommand(install):
     def run(self):
         install.run(self)
         subprocess.call([sys.executable, os.path.join(self.install_lib, 'cerbogen', 'setup.py')])
 
 setup(
     name='cerbogen',
-    version = '0.0.31',
+    version = '0.0.32',
     description='A Python package for CerboTech',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Clarence Parmar',
     author_email='git.clarence@gmail.com',
     url='https://github.com/clarenceparmar/cerbogen',
     packages=find_packages(),
```

