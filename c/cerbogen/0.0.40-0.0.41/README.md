# Comparing `tmp/cerbogen-0.0.40.tar.gz` & `tmp/cerbogen-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbogen-0.0.40.tar", last modified: Sat Apr 20 16:51:20 2024, max compression
+gzip compressed data, was "cerbogen-0.0.41.tar", last modified: Sat Apr 20 16:53:34 2024, max compression
```

## Comparing `cerbogen-0.0.40.tar` & `cerbogen-0.0.41.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 16:51:20.012924 cerbogen-0.0.40/
--rw-rw-rw-   0        0        0      680 2024-04-20 16:51:20.010973 cerbogen-0.0.40/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.40/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 16:51:19.927034 cerbogen-0.0.40/cerbogen/
--rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.40/cerbogen/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 16:51:19.926057 cerbogen-0.0.40/cerbogen/data/
-drwxrwxrwx   0        0        0        0 2024-04-20 16:51:19.944601 cerbogen-0.0.40/cerbogen/data/img/
--rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.40/cerbogen/data/img/logo.ico
--rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.40/cerbogen/data/img/logo.png
-drwxrwxrwx   0        0        0        0 2024-04-20 16:51:20.006091 cerbogen-0.0.40/cerbogen/mod/
--rw-rw-rw-   0        0        0        0 2024-04-20 16:21:25.000000 cerbogen-0.0.40/cerbogen/mod/__init__.py
--rw-rw-rw-   0        0        0     9107 2024-04-20 15:20:54.000000 cerbogen-0.0.40/cerbogen/mod/cerbogen.py
--rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.40/cerbogen/mod/check.py
--rw-rw-rw-   0        0        0     2930 2024-04-20 16:38:30.000000 cerbogen-0.0.40/cerbogen/mod/install_ffmpeg.py
--rw-rw-rw-   0        0        0     2428 2024-04-20 16:45:37.000000 cerbogen-0.0.40/cerbogen/mod/install_location.py
--rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.40/cerbogen/mod/plot.py
--rw-rw-rw-   0        0        0     2051 2024-04-20 16:41:49.000000 cerbogen-0.0.40/cerbogen/mod/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 16:51:20.009019 cerbogen-0.0.40/cerbogen.egg-info/
--rw-rw-rw-   0        0        0      680 2024-04-20 16:51:19.000000 cerbogen-0.0.40/cerbogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2024-04-20 16:51:19.000000 cerbogen-0.0.40/cerbogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 16:51:19.000000 cerbogen-0.0.40/cerbogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-04-20 16:51:19.000000 cerbogen-0.0.40/cerbogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-20 16:51:19.000000 cerbogen-0.0.40/cerbogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 16:51:20.013900 cerbogen-0.0.40/setup.cfg
--rw-rw-rw-   0        0        0     1062 2024-04-20 16:51:19.000000 cerbogen-0.0.40/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:53:34.141728 cerbogen-0.0.41/
+-rw-rw-rw-   0        0        0      680 2024-04-20 16:53:34.140751 cerbogen-0.0.41/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.41/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 16:53:34.109519 cerbogen-0.0.41/cerbogen/
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.41/cerbogen/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:53:34.107568 cerbogen-0.0.41/cerbogen/data/
+drwxrwxrwx   0        0        0        0 2024-04-20 16:53:34.125136 cerbogen-0.0.41/cerbogen/data/img/
+-rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.41/cerbogen/data/img/logo.ico
+-rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.41/cerbogen/data/img/logo.png
+drwxrwxrwx   0        0        0        0 2024-04-20 16:53:34.139777 cerbogen-0.0.41/cerbogen/mod/
+-rw-rw-rw-   0        0        0        0 2024-04-20 16:21:25.000000 cerbogen-0.0.41/cerbogen/mod/__init__.py
+-rw-rw-rw-   0        0        0     9107 2024-04-20 15:20:54.000000 cerbogen-0.0.41/cerbogen/mod/cerbogen.py
+-rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.41/cerbogen/mod/check.py
+-rw-rw-rw-   0        0        0     2930 2024-04-20 16:38:30.000000 cerbogen-0.0.41/cerbogen/mod/install_ffmpeg.py
+-rw-rw-rw-   0        0        0     2213 2024-04-20 16:53:16.000000 cerbogen-0.0.41/cerbogen/mod/install_location.py
+-rw-rw-rw-   0        0        0     2335 2024-04-20 14:14:22.000000 cerbogen-0.0.41/cerbogen/mod/plot.py
+-rw-rw-rw-   0        0        0     2051 2024-04-20 16:41:49.000000 cerbogen-0.0.41/cerbogen/mod/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:53:34.140751 cerbogen-0.0.41/cerbogen.egg-info/
+-rw-rw-rw-   0        0        0      680 2024-04-20 16:53:33.000000 cerbogen-0.0.41/cerbogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2024-04-20 16:53:34.000000 cerbogen-0.0.41/cerbogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 16:53:33.000000 cerbogen-0.0.41/cerbogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-20 16:53:33.000000 cerbogen-0.0.41/cerbogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-20 16:53:33.000000 cerbogen-0.0.41/cerbogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 16:53:34.141728 cerbogen-0.0.41/setup.cfg
+-rw-rw-rw-   0        0        0     1062 2024-04-20 16:53:33.000000 cerbogen-0.0.41/setup.py
```

### Comparing `cerbogen-0.0.40/PKG-INFO` & `cerbogen-0.0.41/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.40
+Version: 0.0.41
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.40/cerbogen/data/img/logo.ico` & `cerbogen-0.0.41/cerbogen/data/img/logo.ico`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.40/cerbogen/data/img/logo.png` & `cerbogen-0.0.41/cerbogen/data/img/logo.png`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.40/cerbogen/mod/cerbogen.py` & `cerbogen-0.0.41/cerbogen/mod/cerbogen.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.40/cerbogen/mod/check.py` & `cerbogen-0.0.41/cerbogen/mod/check.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.40/cerbogen/mod/install_ffmpeg.py` & `cerbogen-0.0.41/cerbogen/mod/install_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.40/cerbogen/mod/install_location.py` & `cerbogen-0.0.41/cerbogen/mod/install_location.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,66 @@
 import tkinter as tk
 from tkinter import filedialog
 import shutil
 import os
 
-def install_location():
+# Function to select an installation location
+def select_installation_location():
+    # Prompt user to select an installation location
+    install_location = filedialog.askdirectory()
+    if install_location:
+        install_location_entry.delete(0, tk.END)
+        install_location_entry.insert(0, install_location)
+
+def install_cerbogen():
+    # Get the installation location
+    install_location = install_location_entry.get()
+
+    # Check if the installation location is provided
+    if install_location:
+        try:
+            # Get the absolute path of the current directory
+            current_dir = os.path.abspath(os.path.dirname(__file__))
+            
+            # Construct the destination file path
+            code_file = os.path.join(current_dir, "..", "cerbogen.pyw")
+            
+            print( code_file )
+
+            # Copy the file
+            shutil.copy(code_file, install_location)
+
+
+            # Show success message
+            tk.messagebox.showinfo("Success", f" Run Cerbogen.pyw file to use the generator ")
+            exit(0)
+
+        except Exception as e:
+            # Show error message if copying fails
+            tk.messagebox.showerror("Error", f"Failed to copy file: {str(e)}")
+    else:
+        # Show error message if the installation location is not provided
+        tk.messagebox.showerror("Error", "Please select an installation location.")
+
+
+# Create main window
+root = tk.Tk()
+root.title("Cerbogen Installation")
+
+# Installation location frame
+install_frame = tk.Frame(root, padx=10, pady=10)
+install_frame.pack()
+
+install_label = tk.Label(install_frame, text="Select Installation Location:")
+install_label.grid(row=0, column=0)
+
+install_location_entry = tk.Entry(install_frame, width=50)
+install_location_entry.grid(row=0, column=1)
+
+install_button = tk.Button(install_frame, text="Browse", command=select_installation_location)
+install_button.grid(row=0, column=2)
+
+# Install button
+install_button = tk.Button(root, text="Install Cerbogen", command=install_cerbogen)
+install_button.pack(pady=10)
 
-    # Function to select an installation location
-    def select_installation_location():
-        # Prompt user to select an installation location
-        install_location = filedialog.askdirectory()
-        if install_location:
-            install_location_entry.delete(0, tk.END)
-            install_location_entry.insert(0, install_location)
-
-    def install_cerbogen():
-        # Get the installation location
-        install_location = install_location_entry.get()
-
-        # Check if the installation location is provided
-        if install_location:
-            try:
-                # Get the absolute path of the current directory
-                current_dir = os.path.abspath(os.path.dirname(__file__))
-                
-                # Construct the destination file path
-                code_file = os.path.join(current_dir, "..", "cerbogen.pyw")
-                
-                print( code_file )
-
-                # Copy the file
-                shutil.copy(code_file, install_location)
-
-
-                # Show success message
-                tk.messagebox.showinfo("Success", f" Run Cerbogen.pyw file to use the generator ")
-                exit(0)
-
-            except Exception as e:
-                # Show error message if copying fails
-                tk.messagebox.showerror("Error", f"Failed to copy file: {str(e)}")
-        else:
-            # Show error message if the installation location is not provided
-            tk.messagebox.showerror("Error", "Please select an installation location.")
-
-
-    # Create main window
-    root = tk.Tk()
-    root.title("Cerbogen Installation")
-
-    # Installation location frame
-    install_frame = tk.Frame(root, padx=10, pady=10)
-    install_frame.pack()
-
-    install_label = tk.Label(install_frame, text="Select Installation Location:")
-    install_label.grid(row=0, column=0)
-
-    install_location_entry = tk.Entry(install_frame, width=50)
-    install_location_entry.grid(row=0, column=1)
-
-    install_button = tk.Button(install_frame, text="Browse", command=select_installation_location)
-    install_button.grid(row=0, column=2)
-
-    # Install button
-    install_button = tk.Button(root, text="Install Cerbogen", command=install_cerbogen)
-    install_button.pack(pady=10)
-
-    root.mainloop()
+root.mainloop()
```

### Comparing `cerbogen-0.0.40/cerbogen/mod/plot.py` & `cerbogen-0.0.41/cerbogen/mod/plot.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.40/cerbogen/mod/setup.py` & `cerbogen-0.0.41/cerbogen/mod/setup.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.40/cerbogen.egg-info/PKG-INFO` & `cerbogen-0.0.41/cerbogen.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.40
+Version: 0.0.41
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cerbogen-0.0.40/setup.py` & `cerbogen-0.0.41/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cerbogen',
-    version = '0.0.40',
+    version = '0.0.41',
     description='A Python package for CerboTech',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Clarence Parmar',
     author_email='git.clarence@gmail.com',
     url='https://github.com/clarenceparmar/cerbogen',
     packages=find_packages(),
```

