# Comparing `tmp/cerbogen-0.0.16.tar.gz` & `tmp/cerbogen-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbogen-0.0.16.tar", last modified: Sat Apr 20 10:13:02 2024, max compression
+gzip compressed data, was "cerbogen-0.0.17.tar", last modified: Sat Apr 20 11:15:14 2024, max compression
```

## Comparing `cerbogen-0.0.16.tar` & `cerbogen-0.0.17.tar`

### file list

```diff
@@ -1,25 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 10:13:02.440092 cerbogen-0.0.16/
--rw-rw-rw-   0        0        0      701 2024-04-20 10:13:02.439117 cerbogen-0.0.16/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.16/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 10:13:02.386042 cerbogen-0.0.16/cerbogen/
--rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.16/cerbogen/__init__.py
--rw-rw-rw-   0        0        0     8856 2024-04-19 07:05:53.000000 cerbogen-0.0.16/cerbogen/cerbogen.py
--rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.16/cerbogen/check.py
-drwxrwxrwx   0        0        0        0 2024-04-20 10:13:02.380401 cerbogen-0.0.16/cerbogen/data/
-drwxrwxrwx   0        0        0        0 2024-04-20 10:13:02.423499 cerbogen-0.0.16/cerbogen/data/img/
--rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.16/cerbogen/data/img/logo.ico
--rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.16/cerbogen/data/img/logo.png
-drwxrwxrwx   0        0        0        0 2024-04-20 10:13:02.437164 cerbogen-0.0.16/cerbogen/ffmpeg/
--rw-rw-rw-   0        0        0    35147 2023-12-31 08:04:26.000000 cerbogen-0.0.16/cerbogen/ffmpeg/LICENSE
--rw-rw-rw-   0        0        0    42234 2023-12-31 08:04:27.000000 cerbogen-0.0.16/cerbogen/ffmpeg/README.txt
--rw-rw-rw-   0        0        0     2348 2024-04-10 13:05:15.000000 cerbogen-0.0.16/cerbogen/plot.py
--rw-rw-rw-   0        0        0     2748 2024-04-20 10:12:35.000000 cerbogen-0.0.16/cerbogen/setup.py
--rw-rw-rw-   0        0        0     9327 2024-04-19 13:45:49.000000 cerbogen-0.0.16/cerbogen/ui.py
-drwxrwxrwx   0        0        0        0 2024-04-20 10:13:02.438139 cerbogen-0.0.16/cerbogen.egg-info/
--rw-rw-rw-   0        0        0      701 2024-04-20 10:13:02.000000 cerbogen-0.0.16/cerbogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2024-04-20 10:13:02.000000 cerbogen-0.0.16/cerbogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 10:13:02.000000 cerbogen-0.0.16/cerbogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-20 10:13:02.000000 cerbogen-0.0.16/cerbogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-20 10:13:02.000000 cerbogen-0.0.16/cerbogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 10:13:02.440092 cerbogen-0.0.16/setup.cfg
--rw-rw-rw-   0        0        0     1355 2024-04-20 10:13:01.000000 cerbogen-0.0.16/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 11:15:14.601837 cerbogen-0.0.17/
+-rw-rw-rw-   0        0        0      701 2024-04-20 11:15:14.600861 cerbogen-0.0.17/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.17/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 11:15:14.573614 cerbogen-0.0.17/cerbogen/
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.17/cerbogen/__init__.py
+-rw-rw-rw-   0        0        0     9081 2024-04-20 11:14:39.000000 cerbogen-0.0.17/cerbogen/cerbogen.py
+-rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.17/cerbogen/check.py
+drwxrwxrwx   0        0        0        0 2024-04-20 11:15:14.554500 cerbogen-0.0.17/cerbogen/data/
+drwxrwxrwx   0        0        0        0 2024-04-20 11:15:14.598908 cerbogen-0.0.17/cerbogen/data/img/
+-rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.17/cerbogen/data/img/logo.ico
+-rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.17/cerbogen/data/img/logo.png
+-rw-rw-rw-   0        0        0     2348 2024-04-10 13:05:15.000000 cerbogen-0.0.17/cerbogen/plot.py
+-rw-rw-rw-   0        0        0     2748 2024-04-20 11:14:51.000000 cerbogen-0.0.17/cerbogen/setup.py
+-rw-rw-rw-   0        0        0     9327 2024-04-19 13:45:49.000000 cerbogen-0.0.17/cerbogen/ui.py
+drwxrwxrwx   0        0        0        0 2024-04-20 11:15:14.599884 cerbogen-0.0.17/cerbogen.egg-info/
+-rw-rw-rw-   0        0        0      701 2024-04-20 11:15:14.000000 cerbogen-0.0.17/cerbogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2024-04-20 11:15:14.000000 cerbogen-0.0.17/cerbogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 11:15:14.000000 cerbogen-0.0.17/cerbogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-20 11:15:14.000000 cerbogen-0.0.17/cerbogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-20 11:15:14.000000 cerbogen-0.0.17/cerbogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 11:15:14.601837 cerbogen-0.0.17/setup.cfg
+-rw-rw-rw-   0        0        0     1355 2024-04-20 11:15:13.000000 cerbogen-0.0.17/setup.py
```

### Comparing `cerbogen-0.0.16/PKG-INFO` & `cerbogen-0.0.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.16
+Version: 0.0.17
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.16/cerbogen/cerbogen.py` & `cerbogen-0.0.17/cerbogen/cerbogen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from pydub import AudioSegment
 import numpy as np
 from plot import Plot
-
+import platform
 from pydub import AudioSegment
 
-# Set the path to FFmpeg
-AudioSegment.converter = "./ffmpeg/bin/ffmpeg.exe"
+# Set the path to FFmpeg based on the operating system
+if platform.system() == "Windows":
+    # Path to FFmpeg for Windows
+    AudioSegment.converter = "./ffmpeg/win/bin/ffmpeg.exe"
+else:
+    # Path to FFmpeg for macOS or Linux
+    AudioSegment.converter = "./ffmpeg/mac/ffmpeg"
+
 
 
 zf = lambda x,y: str(x).zfill( len( str(y) ) )
 
 class binbeats:
 
     main_buffer = []
```

### Comparing `cerbogen-0.0.16/cerbogen/check.py` & `cerbogen-0.0.17/cerbogen/check.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.16/cerbogen/data/img/logo.ico` & `cerbogen-0.0.17/cerbogen/data/img/logo.ico`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.16/cerbogen/data/img/logo.png` & `cerbogen-0.0.17/cerbogen/data/img/logo.png`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.16/cerbogen/plot.py` & `cerbogen-0.0.17/cerbogen/plot.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.16/cerbogen/setup.py` & `cerbogen-0.0.17/cerbogen/setup.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.16/cerbogen/ui.py` & `cerbogen-0.0.17/cerbogen/ui.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.16/cerbogen.egg-info/PKG-INFO` & `cerbogen-0.0.17/cerbogen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.16
+Version: 0.0.17
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.16/setup.py` & `cerbogen-0.0.17/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class PostInstallCommand(install):
     def run(self):
         install.run(self)
         subprocess.call([sys.executable, os.path.join(self.install_lib, 'cerbogen', 'setup.py')])
 
 setup(
     name='cerbogen',
-    version = '0.0.16',
+    version = '0.0.17',
     description='A Python package for CerboTech',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Clarence Parmar',
     author_email='git.clarence@gmail.com',
     url='https://github.com/clarenceparmar/cerbogen',
     packages=find_packages(),
```

