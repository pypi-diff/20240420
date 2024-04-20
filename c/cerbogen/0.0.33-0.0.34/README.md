# Comparing `tmp/cerbogen-0.0.33.tar.gz` & `tmp/cerbogen-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbogen-0.0.33.tar", last modified: Sat Apr 20 15:19:27 2024, max compression
+gzip compressed data, was "cerbogen-0.0.34.tar", last modified: Sat Apr 20 15:29:45 2024, max compression
```

## Comparing `cerbogen-0.0.33.tar` & `cerbogen-0.0.34.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 15:19:27.162532 cerbogen-0.0.33/
--rw-rw-rw-   0        0        0      680 2024-04-20 15:19:27.161556 cerbogen-0.0.33/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.33/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 15:19:27.134228 cerbogen-0.0.33/cerbogen/
--rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.33/cerbogen/__init__.py
--rw-rw-rw-   0        0        0     8764 2024-04-20 13:28:49.000000 cerbogen-0.0.33/cerbogen/cerbogen.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:19:27.130324 cerbogen-0.0.33/cerbogen/data/
-drwxrwxrwx   0        0        0        0 2024-04-20 15:19:27.146916 cerbogen-0.0.33/cerbogen/data/img/
--rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.33/cerbogen/data/img/logo.ico
--rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.33/cerbogen/data/img/logo.png
--rw-rw-rw-   0        0        0    10191 2024-04-20 15:17:40.000000 cerbogen-0.0.33/cerbogen/main.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:19:27.158628 cerbogen-0.0.33/cerbogen/mod/
--rw-rw-rw-   0        0        0     2902 2024-04-20 15:17:36.000000 cerbogen-0.0.33/cerbogen/mod/after_install.py
--rw-rw-rw-   0        0        0     9200 2024-04-20 15:19:10.000000 cerbogen-0.0.33/cerbogen/mod/cerbogen.py
--rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.33/cerbogen/mod/check.py
--rw-rw-rw-   0        0        0     2928 2024-04-20 13:25:55.000000 cerbogen-0.0.33/cerbogen/mod/ffmpeg_install.py
--rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.33/cerbogen/mod/plot.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:19:27.160580 cerbogen-0.0.33/cerbogen.egg-info/
--rw-rw-rw-   0        0        0      680 2024-04-20 15:19:27.000000 cerbogen-0.0.33/cerbogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2024-04-20 15:19:27.000000 cerbogen-0.0.33/cerbogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 15:19:27.000000 cerbogen-0.0.33/cerbogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-04-20 15:19:27.000000 cerbogen-0.0.33/cerbogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-20 15:19:27.000000 cerbogen-0.0.33/cerbogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 15:19:27.162532 cerbogen-0.0.33/setup.cfg
--rw-rw-rw-   0        0        0     1372 2024-04-20 15:19:26.000000 cerbogen-0.0.33/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:29:45.787241 cerbogen-0.0.34/
+-rw-rw-rw-   0        0        0      680 2024-04-20 15:29:45.786265 cerbogen-0.0.34/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.34/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 15:29:45.760384 cerbogen-0.0.34/cerbogen/
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.34/cerbogen/__init__.py
+-rw-rw-rw-   0        0        0     8764 2024-04-20 13:28:49.000000 cerbogen-0.0.34/cerbogen/cerbogen.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:29:45.756480 cerbogen-0.0.34/cerbogen/data/
+drwxrwxrwx   0        0        0        0 2024-04-20 15:29:45.772601 cerbogen-0.0.34/cerbogen/data/img/
+-rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.34/cerbogen/data/img/logo.ico
+-rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.34/cerbogen/data/img/logo.png
+-rw-rw-rw-   0        0        0    10191 2024-04-20 15:17:40.000000 cerbogen-0.0.34/cerbogen/main.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:29:45.785291 cerbogen-0.0.34/cerbogen/mod/
+-rw-rw-rw-   0        0        0     2930 2024-04-20 15:29:31.000000 cerbogen-0.0.34/cerbogen/mod/after_install.py
+-rw-rw-rw-   0        0        0     9107 2024-04-20 15:20:54.000000 cerbogen-0.0.34/cerbogen/mod/cerbogen.py
+-rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.34/cerbogen/mod/check.py
+-rw-rw-rw-   0        0        0     2928 2024-04-20 13:25:55.000000 cerbogen-0.0.34/cerbogen/mod/ffmpeg_install.py
+-rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.34/cerbogen/mod/plot.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:29:45.786265 cerbogen-0.0.34/cerbogen.egg-info/
+-rw-rw-rw-   0        0        0      680 2024-04-20 15:29:45.000000 cerbogen-0.0.34/cerbogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2024-04-20 15:29:45.000000 cerbogen-0.0.34/cerbogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 15:29:45.000000 cerbogen-0.0.34/cerbogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-20 15:29:45.000000 cerbogen-0.0.34/cerbogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-20 15:29:45.000000 cerbogen-0.0.34/cerbogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 15:29:45.787241 cerbogen-0.0.34/setup.cfg
+-rw-rw-rw-   0        0        0     1372 2024-04-20 15:29:45.000000 cerbogen-0.0.34/setup.py
```

### Comparing `cerbogen-0.0.33/PKG-INFO` & `cerbogen-0.0.34/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.33
+Version: 0.0.34
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.33/cerbogen/cerbogen.py` & `cerbogen-0.0.34/cerbogen/cerbogen.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.33/cerbogen/data/img/logo.ico` & `cerbogen-0.0.34/cerbogen/data/img/logo.ico`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.33/cerbogen/data/img/logo.png` & `cerbogen-0.0.34/cerbogen/data/img/logo.png`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.33/cerbogen/main.py` & `cerbogen-0.0.34/cerbogen/main.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.33/cerbogen/mod/after_install.py` & `cerbogen-0.0.34/cerbogen/mod/after_install.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 import os
 import platform
-import ffmpeg_install
+# import ffmpeg_install
 
 def install_pywin32():
     if platform.system() == "Windows":
         try:
             import win32com.client
         except ImportError:
             print("pywin32 not found. Installing...")
@@ -26,17 +26,20 @@
     cerbogen_path = os.path.join(site_packages, 'cerbogen')
     if os.path.exists(cerbogen_path):
         return cerbogen_path
     else:
         return None
 
 def create_desktop_shortcut(ui_py_path):
+    
     desktop_dir = os.path.join(os.path.expanduser("~"), "Desktop")
     shortcut_path = os.path.join(desktop_dir, "cerbogen_ui.lnk" if platform.system() == "Windows" else "cerbogen_ui.desktop")
     python_exe = sys.executable
+
+
     if platform.system() == "Windows":
         # Create Windows shortcut
         try:
             from win32com.client import Dispatch
         except ImportError:
             print("pywin32 not found. Install it to create shortcuts on Windows.")
             sys.exit(1)
@@ -59,18 +62,21 @@
             shortcut_file.write("Name=Cerbogen UI\n")
             shortcut_file.write("Exec={} {}\n".format(python_exe, ui_py_path))
             shortcut_file.write("Type=Application\n")
             shortcut_file.write("Terminal=false\n")
         os.chmod(shortcut_path, 0o755)  # Add execute permission for Linux/macOS
 
 if __name__ == "__main__":
+
     install_pywin32()
+    
     cerbogen_path = find_cerbogen_package()
+    
     if cerbogen_path:
-        ui_py_path = os.path.join(cerbogen_path, 'ui.py')
+        ui_py_path = os.path.join(cerbogen_path, 'main.py')
         if os.path.exists(ui_py_path):
             create_desktop_shortcut(ui_py_path)
             print("Desktop shortcut for Cerbogen UI created successfully!")
         else:
             print("ui.py not found in Cerbogen package.")
     else:
         print("Cerbogen package not found.")
```

### Comparing `cerbogen-0.0.33/cerbogen/mod/cerbogen.py` & `cerbogen-0.0.34/cerbogen/mod/cerbogen.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,13 +257,7 @@
                                                              sample_rate , left_level , 
                                                              right_level ) )
                 
                 right = round(right - 0.1, 1)
 
 
             num = round( num + update_per_sec , 1 )
-
-
-
-binbeats.down_xx( 100 , 100 , 50 , 5 , d_r=True )
-binbeats.save("binbeats", "mp3")
-
```

### Comparing `cerbogen-0.0.33/cerbogen/mod/check.py` & `cerbogen-0.0.34/cerbogen/mod/check.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.33/cerbogen/mod/ffmpeg_install.py` & `cerbogen-0.0.34/cerbogen/mod/ffmpeg_install.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.33/cerbogen/mod/plot.py` & `cerbogen-0.0.34/cerbogen/mod/plot.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.33/cerbogen.egg-info/PKG-INFO` & `cerbogen-0.0.34/cerbogen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.33
+Version: 0.0.34
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.33/setup.py` & `cerbogen-0.0.34/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class PostInstallCommand(install):
     def run(self):
         install.run(self)
         subprocess.call([sys.executable, os.path.join(self.install_lib, 'cerbogen', 'setup.py')])
 
 setup(
     name='cerbogen',
-    version = '0.0.33',
+    version = '0.0.34',
     description='A Python package for CerboTech',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Clarence Parmar',
     author_email='git.clarence@gmail.com',
     url='https://github.com/clarenceparmar/cerbogen',
     packages=find_packages(),
```

