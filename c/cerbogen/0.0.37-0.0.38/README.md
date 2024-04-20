# Comparing `tmp/cerbogen-0.0.37.tar.gz` & `tmp/cerbogen-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbogen-0.0.37.tar", last modified: Sat Apr 20 16:26:52 2024, max compression
+gzip compressed data, was "cerbogen-0.0.38.tar", last modified: Sat Apr 20 16:47:54 2024, max compression
```

## Comparing `cerbogen-0.0.37.tar` & `cerbogen-0.0.38.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 16:26:52.655177 cerbogen-0.0.37/
--rw-rw-rw-   0        0        0      680 2024-04-20 16:26:52.654202 cerbogen-0.0.37/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.37/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 16:26:52.623944 cerbogen-0.0.37/cerbogen/
--rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.37/cerbogen/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 16:26:52.621996 cerbogen-0.0.37/cerbogen/data/
-drwxrwxrwx   0        0        0        0 2024-04-20 16:26:52.635658 cerbogen-0.0.37/cerbogen/data/img/
--rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.37/cerbogen/data/img/logo.ico
--rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.37/cerbogen/data/img/logo.png
-drwxrwxrwx   0        0        0        0 2024-04-20 16:26:52.650298 cerbogen-0.0.37/cerbogen/mod/
--rw-rw-rw-   0        0        0        0 2024-04-20 16:21:25.000000 cerbogen-0.0.37/cerbogen/mod/__init__.py
--rw-rw-rw-   0        0        0     9107 2024-04-20 15:20:54.000000 cerbogen-0.0.37/cerbogen/mod/cerbogen.py
--rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.37/cerbogen/mod/check.py
--rw-rw-rw-   0        0        0     2928 2024-04-20 13:25:55.000000 cerbogen-0.0.37/cerbogen/mod/install_ffmpeg.py
--rw-rw-rw-   0        0        0     2166 2024-04-20 16:20:34.000000 cerbogen-0.0.37/cerbogen/mod/install_location.py
--rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.37/cerbogen/mod/plot.py
--rw-rw-rw-   0        0        0     2955 2024-04-20 16:24:36.000000 cerbogen-0.0.37/cerbogen/mod/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 16:26:52.652249 cerbogen-0.0.37/cerbogen.egg-info/
--rw-rw-rw-   0        0        0      680 2024-04-20 16:26:52.000000 cerbogen-0.0.37/cerbogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2024-04-20 16:26:52.000000 cerbogen-0.0.37/cerbogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 16:26:52.000000 cerbogen-0.0.37/cerbogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-04-20 16:26:52.000000 cerbogen-0.0.37/cerbogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-20 16:26:52.000000 cerbogen-0.0.37/cerbogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 16:26:52.656153 cerbogen-0.0.37/setup.cfg
--rw-rw-rw-   0        0        0     1510 2024-04-20 16:26:52.000000 cerbogen-0.0.37/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:47:54.030507 cerbogen-0.0.38/
+-rw-rw-rw-   0        0        0      680 2024-04-20 16:47:54.029531 cerbogen-0.0.38/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.38/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 16:47:53.994395 cerbogen-0.0.38/cerbogen/
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.38/cerbogen/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:47:53.993418 cerbogen-0.0.38/cerbogen/data/
+drwxrwxrwx   0        0        0        0 2024-04-20 16:47:54.017820 cerbogen-0.0.38/cerbogen/data/img/
+-rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.38/cerbogen/data/img/logo.ico
+-rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.38/cerbogen/data/img/logo.png
+drwxrwxrwx   0        0        0        0 2024-04-20 16:47:54.027579 cerbogen-0.0.38/cerbogen/mod/
+-rw-rw-rw-   0        0        0        0 2024-04-20 16:21:25.000000 cerbogen-0.0.38/cerbogen/mod/__init__.py
+-rw-rw-rw-   0        0        0     9107 2024-04-20 15:20:54.000000 cerbogen-0.0.38/cerbogen/mod/cerbogen.py
+-rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.38/cerbogen/mod/check.py
+-rw-rw-rw-   0        0        0     2930 2024-04-20 16:38:30.000000 cerbogen-0.0.38/cerbogen/mod/install_ffmpeg.py
+-rw-rw-rw-   0        0        0     2428 2024-04-20 16:45:37.000000 cerbogen-0.0.38/cerbogen/mod/install_location.py
+-rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.38/cerbogen/mod/plot.py
+-rw-rw-rw-   0        0        0     2051 2024-04-20 16:41:49.000000 cerbogen-0.0.38/cerbogen/mod/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:47:54.028554 cerbogen-0.0.38/cerbogen.egg-info/
+-rw-rw-rw-   0        0        0      680 2024-04-20 16:47:53.000000 cerbogen-0.0.38/cerbogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2024-04-20 16:47:53.000000 cerbogen-0.0.38/cerbogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 16:47:53.000000 cerbogen-0.0.38/cerbogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-04-20 16:47:53.000000 cerbogen-0.0.38/cerbogen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       31 2024-04-20 16:47:53.000000 cerbogen-0.0.38/cerbogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-20 16:47:53.000000 cerbogen-0.0.38/cerbogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 16:47:54.030507 cerbogen-0.0.38/setup.cfg
+-rw-rw-rw-   0        0        0     1262 2024-04-20 16:47:53.000000 cerbogen-0.0.38/setup.py
```

### Comparing `cerbogen-0.0.37/PKG-INFO` & `cerbogen-0.0.38/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.37
+Version: 0.0.38
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.37/cerbogen/data/img/logo.ico` & `cerbogen-0.0.38/cerbogen/data/img/logo.ico`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.37/cerbogen/data/img/logo.png` & `cerbogen-0.0.38/cerbogen/data/img/logo.png`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.37/cerbogen/mod/cerbogen.py` & `cerbogen-0.0.38/cerbogen/mod/cerbogen.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.37/cerbogen/mod/check.py` & `cerbogen-0.0.38/cerbogen/mod/check.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.37/cerbogen/mod/install_ffmpeg.py` & `cerbogen-0.0.38/cerbogen/mod/install_ffmpeg.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 import platform
 import requests
 import shutil
 import tarfile
 import zipfile
 from tqdm import tqdm
 
+# URLs of the archives
+windows_url = "https://github.com/BtbN/FFmpeg-Builds/releases/download/autobuild-2024-04-20-12-56/ffmpeg-N-114897-gbba996d6cd-win64-gpl-shared.zip"
+mac_url = "https://evermeet.cx/ffmpeg/ffmpeg-114896-gf18de5bc4a.7z"
+linux_url = "https://example.com/ffmpeg_linux.tar.xz"  # Provide the actual Linux archive URL
+
+
 # Function to download a file
 def download_file(url, filename):
     response = requests.get(url, stream=True)
     total_size = int(response.headers.get('content-length', 0))
     block_size = 1024
     progress_bar = tqdm(total=total_size, unit='B', unit_scale=True)
     with open(filename, 'wb') as file:
@@ -31,19 +37,14 @@
     os.system(f'7z x "{archive_path}" -o"{extract_dir}"')
     print(f"Extraction of {archive_path} complete.")
 
 # Function to remove a file
 def remove_file(file_path):
     os.remove(file_path)
 
-# URLs of the archives
-windows_url = "https://github.com/BtbN/FFmpeg-Builds/releases/download/autobuild-2024-04-20-12-56/ffmpeg-N-114897-gbba996d6cd-win64-gpl-shared.zip"
-mac_url = "https://evermeet.cx/ffmpeg/ffmpeg-114896-gf18de5bc4a.7z"
-linux_url = "https://example.com/ffmpeg_linux.tar.xz"  # Provide the actual Linux archive URL
-
 # Download and extract archives based on the system
 if platform.system() == "Windows":
     # Download the Windows archive
     download_file(windows_url, "win_ffmpeg.zip")
     # Extract the Windows archive
     with zipfile.ZipFile("win_ffmpeg.zip", 'r') as zip_ref:
         zip_ref.extractall("win_ffmpeg")
```

### Comparing `cerbogen-0.0.37/cerbogen/mod/plot.py` & `cerbogen-0.0.38/cerbogen/mod/plot.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.37/cerbogen.egg-info/PKG-INFO` & `cerbogen-0.0.38/cerbogen.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.37
+Version: 0.0.38
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.37/setup.py` & `cerbogen-0.0.38/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,47 @@
+# setup.py
 
-import sys
 from setuptools import setup, find_packages
-from setuptools.command.install import install
-import subprocess
 import os
-
-# Custom installation class to run setup.py after installation
-class PostInstallCommand(install):
-   def run(self):
-        install.run(self)
-        # Get the path to cerbogen/mod/setup.py
-        setup_script = os.path.join(os.path.dirname(__file__), 'cerbogen', 'mod', 'setup.py')
-        # Run the setup.py script
-        subprocess.call([sys.executable, setup_script])
+from cerbogen.mod.install_location import install_location
 
 
 setup(
     name='cerbogen',
-    version = '0.0.37',
+    version = '0.0.38',
     description='A Python package for CerboTech',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Clarence Parmar',
     author_email='git.clarence@gmail.com',
     url='https://github.com/clarenceparmar/cerbogen',
     packages=find_packages(),
     
     package_data={
-
-        '': ['ffmpeg/mac/*', 'data/img/*' , "mod/*" ]
+        '': ['ffmpeg/mac/*', 'data/img/*', 'mod/*']
     },
 
     install_requires=[
-
-        "matplotlib", "pydub", "numpy" , "librosa" 
-
+        "matplotlib", "pydub", "numpy", "librosa"
     ],
     
     python_requires='>=3.6',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
-    cmdclass={
-        'install': PostInstallCommand,
-    }
 
-    
+    # Specify the entry point to execute install.py during installation
+    entry_points={
+        'console_scripts': [
+            'install_cerbogen=cerbogen.mod.install:install_location',
+        ],
+    },
+
+
 )
+
+
```

