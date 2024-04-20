# Comparing `tmp/cerbogen-0.0.34.tar.gz` & `tmp/cerbogen-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbogen-0.0.34.tar", last modified: Sat Apr 20 15:29:45 2024, max compression
+gzip compressed data, was "cerbogen-0.0.35.tar", last modified: Sat Apr 20 16:21:53 2024, max compression
```

## Comparing `cerbogen-0.0.34.tar` & `cerbogen-0.0.35.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 15:29:45.787241 cerbogen-0.0.34/
--rw-rw-rw-   0        0        0      680 2024-04-20 15:29:45.786265 cerbogen-0.0.34/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.34/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 15:29:45.760384 cerbogen-0.0.34/cerbogen/
--rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.34/cerbogen/__init__.py
--rw-rw-rw-   0        0        0     8764 2024-04-20 13:28:49.000000 cerbogen-0.0.34/cerbogen/cerbogen.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:29:45.756480 cerbogen-0.0.34/cerbogen/data/
-drwxrwxrwx   0        0        0        0 2024-04-20 15:29:45.772601 cerbogen-0.0.34/cerbogen/data/img/
--rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.34/cerbogen/data/img/logo.ico
--rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.34/cerbogen/data/img/logo.png
--rw-rw-rw-   0        0        0    10191 2024-04-20 15:17:40.000000 cerbogen-0.0.34/cerbogen/main.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:29:45.785291 cerbogen-0.0.34/cerbogen/mod/
--rw-rw-rw-   0        0        0     2930 2024-04-20 15:29:31.000000 cerbogen-0.0.34/cerbogen/mod/after_install.py
--rw-rw-rw-   0        0        0     9107 2024-04-20 15:20:54.000000 cerbogen-0.0.34/cerbogen/mod/cerbogen.py
--rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.34/cerbogen/mod/check.py
--rw-rw-rw-   0        0        0     2928 2024-04-20 13:25:55.000000 cerbogen-0.0.34/cerbogen/mod/ffmpeg_install.py
--rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.34/cerbogen/mod/plot.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:29:45.786265 cerbogen-0.0.34/cerbogen.egg-info/
--rw-rw-rw-   0        0        0      680 2024-04-20 15:29:45.000000 cerbogen-0.0.34/cerbogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2024-04-20 15:29:45.000000 cerbogen-0.0.34/cerbogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 15:29:45.000000 cerbogen-0.0.34/cerbogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-04-20 15:29:45.000000 cerbogen-0.0.34/cerbogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-20 15:29:45.000000 cerbogen-0.0.34/cerbogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 15:29:45.787241 cerbogen-0.0.34/setup.cfg
--rw-rw-rw-   0        0        0     1372 2024-04-20 15:29:45.000000 cerbogen-0.0.34/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:21:53.259570 cerbogen-0.0.35/
+-rw-rw-rw-   0        0        0      680 2024-04-20 16:21:53.257618 cerbogen-0.0.35/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.35/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 16:21:53.221974 cerbogen-0.0.35/cerbogen/
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.35/cerbogen/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:21:53.220022 cerbogen-0.0.35/cerbogen/data/
+drwxrwxrwx   0        0        0        0 2024-04-20 16:21:53.240049 cerbogen-0.0.35/cerbogen/data/img/
+-rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.35/cerbogen/data/img/logo.ico
+-rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.35/cerbogen/data/img/logo.png
+drwxrwxrwx   0        0        0        0 2024-04-20 16:21:53.253713 cerbogen-0.0.35/cerbogen/mod/
+-rw-rw-rw-   0        0        0        0 2024-04-20 16:21:25.000000 cerbogen-0.0.35/cerbogen/mod/__init__.py
+-rw-rw-rw-   0        0        0     9107 2024-04-20 15:20:54.000000 cerbogen-0.0.35/cerbogen/mod/cerbogen.py
+-rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.35/cerbogen/mod/check.py
+-rw-rw-rw-   0        0        0     2930 2024-04-20 15:29:31.000000 cerbogen-0.0.35/cerbogen/mod/install.py
+-rw-rw-rw-   0        0        0     2928 2024-04-20 13:25:55.000000 cerbogen-0.0.35/cerbogen/mod/install_ffmpeg.py
+-rw-rw-rw-   0        0        0     2166 2024-04-20 16:20:34.000000 cerbogen-0.0.35/cerbogen/mod/install_location.py
+-rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.35/cerbogen/mod/plot.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:21:53.255669 cerbogen-0.0.35/cerbogen.egg-info/
+-rw-rw-rw-   0        0        0      680 2024-04-20 16:21:53.000000 cerbogen-0.0.35/cerbogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2024-04-20 16:21:53.000000 cerbogen-0.0.35/cerbogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 16:21:53.000000 cerbogen-0.0.35/cerbogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-20 16:21:53.000000 cerbogen-0.0.35/cerbogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-20 16:21:53.000000 cerbogen-0.0.35/cerbogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 16:21:53.259570 cerbogen-0.0.35/setup.cfg
+-rw-rw-rw-   0        0        0     1372 2024-04-20 16:21:52.000000 cerbogen-0.0.35/setup.py
```

### Comparing `cerbogen-0.0.34/PKG-INFO` & `cerbogen-0.0.35/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.34
+Version: 0.0.35
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.34/cerbogen/cerbogen.py` & `cerbogen-0.0.35/cerbogen/mod/cerbogen.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,26 @@
-import numpy as np
+import platform
+
 from pydub import AudioSegment
+import numpy as np
+
 from pydub import AudioSegment
 
-# Zero fill
+from mod.plot import Plot
+
+# # Set the path to FFmpeg based on the operating system
+# if platform.system() == "Windows":
+#     # Path to FFmpeg for Windows
+#     AudioSegment.converter = "./ffmpeg/win/bin/ffmpeg.exe"
+# else:
+#     # Path to FFmpeg for macOS or Linux
+#     AudioSegment.converter = "./ffmpeg/mac/ffmpeg"
+
+
+
 zf = lambda x,y: str(x).zfill( len( str(y) ) )
 
 class binbeats:
 
     main_buffer = [] 
     diffrence=[]
     timeline=[]
```

### Comparing `cerbogen-0.0.34/cerbogen/data/img/logo.ico` & `cerbogen-0.0.35/cerbogen/data/img/logo.ico`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.34/cerbogen/data/img/logo.png` & `cerbogen-0.0.35/cerbogen/data/img/logo.png`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.34/cerbogen/mod/after_install.py` & `cerbogen-0.0.35/cerbogen/mod/install.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.34/cerbogen/mod/check.py` & `cerbogen-0.0.35/cerbogen/mod/check.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.34/cerbogen/mod/ffmpeg_install.py` & `cerbogen-0.0.35/cerbogen/mod/install_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.34/cerbogen/mod/plot.py` & `cerbogen-0.0.35/cerbogen/mod/plot.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.34/cerbogen.egg-info/PKG-INFO` & `cerbogen-0.0.35/cerbogen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.34
+Version: 0.0.35
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.34/setup.py` & `cerbogen-0.0.35/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class PostInstallCommand(install):
     def run(self):
         install.run(self)
         subprocess.call([sys.executable, os.path.join(self.install_lib, 'cerbogen', 'setup.py')])
 
 setup(
     name='cerbogen',
-    version = '0.0.34',
+    version = '0.0.35',
     description='A Python package for CerboTech',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Clarence Parmar',
     author_email='git.clarence@gmail.com',
     url='https://github.com/clarenceparmar/cerbogen',
     packages=find_packages(),
```

