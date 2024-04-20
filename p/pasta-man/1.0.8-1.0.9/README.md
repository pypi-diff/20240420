# Comparing `tmp/pasta_man-1.0.8.tar.gz` & `tmp/pasta_man-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasta_man-1.0.8.tar", last modified: Tue Apr 16 07:54:11 2024, max compression
+gzip compressed data, was "pasta_man-1.0.9.tar", last modified: Wed Apr 17 16:29:53 2024, max compression
```

## Comparing `pasta_man-1.0.8.tar` & `pasta_man-1.0.9.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 07:54:11.969215 pasta_man-1.0.8/
--rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-15 01:10:20.000000 pasta_man-1.0.8/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     8106 2024-04-16 07:54:11.968847 pasta_man-1.0.8/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     5603 2024-04-16 07:54:02.000000 pasta_man-1.0.8/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1501 2024-04-16 06:51:39.000000 pasta_man-1.0.8/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-16 07:54:11.969279 pasta_man-1.0.8/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 07:54:11.955011 pasta_man-1.0.8/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 07:54:11.960335 pasta_man-1.0.8/src/pasta_man/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 01:10:20.000000 pasta_man-1.0.8/src/pasta_man/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)      129 2024-04-15 01:10:20.000000 pasta_man-1.0.8/src/pasta_man/__main__.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 07:54:11.964721 pasta_man-1.0.8/src/pasta_man/architectures/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 21:32:13.000000 pasta_man-1.0.8/src/pasta_man/architectures/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)    11489 2024-04-16 04:18:44.000000 pasta_man-1.0.8/src/pasta_man/architectures/gui.py
--rw-r--r--   0 d33pster   (501) staff       (20)     9911 2024-04-15 21:32:13.000000 pasta_man-1.0.8/src/pasta_man/architectures/targets.py
--rw-r--r--   0 d33pster   (501) staff       (20)      776 2024-04-15 01:10:20.000000 pasta_man-1.0.8/src/pasta_man/encryption.py
--rw-r--r--   0 d33pster   (501) staff       (20)      237 2024-04-15 01:10:20.000000 pasta_man-1.0.8/src/pasta_man/exceptions.py
--rwxr-xr-x   0 d33pster   (501) staff       (20)     4168 2024-04-16 07:17:47.000000 pasta_man-1.0.8/src/pasta_man/pasta_man.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 07:54:11.966111 pasta_man-1.0.8/src/pasta_man/self_launch_thread/
--rw-r--r--   0 d33pster   (501) staff       (20)     2494 2024-04-16 07:44:32.000000 pasta_man-1.0.8/src/pasta_man/self_launch_thread/Launcher.py
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 21:32:13.000000 pasta_man-1.0.8/src/pasta_man/self_launch_thread/__init__.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 07:54:11.967660 pasta_man-1.0.8/src/pasta_man/utilities/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 18:18:11.000000 pasta_man-1.0.8/src/pasta_man/utilities/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)      639 2024-04-15 18:18:11.000000 pasta_man-1.0.8/src/pasta_man/utilities/helptext.py
--rw-r--r--   0 d33pster   (501) staff       (20)     7579 2024-04-16 03:54:54.000000 pasta_man-1.0.8/src/pasta_man/utilities/pasta_menu.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 07:54:11.968358 pasta_man-1.0.8/src/pasta_man.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     8106 2024-04-16 07:54:11.000000 pasta_man-1.0.8/src/pasta_man.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      705 2024-04-16 07:54:11.000000 pasta_man-1.0.8/src/pasta_man.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-16 07:54:11.000000 pasta_man-1.0.8/src/pasta_man.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)      119 2024-04-16 07:54:11.000000 pasta_man-1.0.8/src/pasta_man.egg-info/entry_points.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       81 2024-04-16 07:54:11.000000 pasta_man-1.0.8/src/pasta_man.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       10 2024-04-16 07:54:11.000000 pasta_man-1.0.8/src/pasta_man.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-17 16:29:53.152001 pasta_man-1.0.9/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-15 01:10:20.000000 pasta_man-1.0.9/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     9094 2024-04-17 16:29:53.151513 pasta_man-1.0.9/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     6591 2024-04-17 16:24:54.000000 pasta_man-1.0.9/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1501 2024-04-17 16:24:54.000000 pasta_man-1.0.9/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-17 16:29:53.152071 pasta_man-1.0.9/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-17 16:29:53.134794 pasta_man-1.0.9/src/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-17 16:29:53.140789 pasta_man-1.0.9/src/pasta_man/
+-rw-r--r--   0 d33pster   (501) staff       (20)      106 2024-04-17 16:24:54.000000 pasta_man-1.0.9/src/pasta_man/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      108 2024-04-17 16:24:54.000000 pasta_man-1.0.9/src/pasta_man/__main__.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-17 16:29:53.146683 pasta_man-1.0.9/src/pasta_man/architectures/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 21:32:13.000000 pasta_man-1.0.9/src/pasta_man/architectures/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)    11522 2024-04-17 16:29:38.000000 pasta_man-1.0.9/src/pasta_man/architectures/gui.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     9911 2024-04-15 21:32:13.000000 pasta_man-1.0.9/src/pasta_man/architectures/targets.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     4052 2024-04-17 16:24:54.000000 pasta_man-1.0.9/src/pasta_man/encryption.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     1692 2024-04-17 16:24:54.000000 pasta_man-1.0.9/src/pasta_man/exceptions.py
+-rwxr-xr-x   0 d33pster   (501) staff       (20)     8843 2024-04-17 16:24:54.000000 pasta_man-1.0.9/src/pasta_man/pasta_man.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-17 16:29:53.147839 pasta_man-1.0.9/src/pasta_man/self_launch_thread/
+-rw-r--r--   0 d33pster   (501) staff       (20)     3949 2024-04-17 16:24:54.000000 pasta_man-1.0.9/src/pasta_man/self_launch_thread/Launcher.py
+-rw-r--r--   0 d33pster   (501) staff       (20)       96 2024-04-17 16:24:54.000000 pasta_man-1.0.9/src/pasta_man/self_launch_thread/__init__.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-17 16:29:53.150085 pasta_man-1.0.9/src/pasta_man/utilities/
+-rw-r--r--   0 d33pster   (501) staff       (20)       51 2024-04-17 16:24:54.000000 pasta_man-1.0.9/src/pasta_man/utilities/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     1915 2024-04-17 16:24:54.000000 pasta_man-1.0.9/src/pasta_man/utilities/helptext.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     6713 2024-04-17 16:24:54.000000 pasta_man-1.0.9/src/pasta_man/utilities/pasta_docs.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     7810 2024-04-17 16:28:51.000000 pasta_man-1.0.9/src/pasta_man/utilities/pasta_menu.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-17 16:29:53.150812 pasta_man-1.0.9/src/pasta_man.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     9094 2024-04-17 16:29:53.000000 pasta_man-1.0.9/src/pasta_man.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      743 2024-04-17 16:29:53.000000 pasta_man-1.0.9/src/pasta_man.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-17 16:29:53.000000 pasta_man-1.0.9/src/pasta_man.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)      119 2024-04-17 16:29:53.000000 pasta_man-1.0.9/src/pasta_man.egg-info/entry_points.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       81 2024-04-17 16:29:53.000000 pasta_man-1.0.9/src/pasta_man.egg-info/requires.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       10 2024-04-17 16:29:53.000000 pasta_man-1.0.9/src/pasta_man.egg-info/top_level.txt
```

### Comparing `pasta_man-1.0.8/LICENSE` & `pasta_man-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.8/PKG-INFO` & `pasta_man-1.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta-man
-Version: 1.0.8
+Version: 1.0.9
 Summary: Password Manager
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>, Sairam Pimple <sairampimple003@gmail.com>, Shubham Narendra Singh <shubh1122000@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -47,14 +47,15 @@
 Requires-Dist: tk
 Requires-Dist: optioner>=1.5.2
 Requires-Dist: pyperclip
 Requires-Dist: ttkthemes
 Requires-Dist: pyinstaller
 
 ![PyPI - Version](https://img.shields.io/pypi/v/pasta-man)
+![PyPI - Status](https://img.shields.io/pypi/status/pasta-man)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pasta-man)
 ![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/pasta-man)
 ![PyPI - License](https://img.shields.io/pypi/l/pasta-man)
 
 
 # Overview
 Pasta-Man is a software application designed to securely store passwords and sensitive information in an encrypted format. It provides users with a convenient way to manage their passwords, ensuring they are protected from unauthorized access. 
@@ -92,19 +93,19 @@
 
 ### Faster than basic tkinter apps
 `Pasta-Man` actively uses Threads to carry out intensive tasks in order to minimize GUI lag as well as have better performance than any basic app created through python tkinter lib.
 
 ### Themes
 User can now change Theme for the app from the Menu Bar. Default is `Arc`. Whatever theme the user chooses, It will be set as default and next time `Pasta-Man` is launched, that theme will be loaded.
 
-Themes can be changed using the MenuBar.
+Themes can be changed using the MenuBar -
 
-<!-- <img src="images/MenuBar.png"> -->
+<img src="images/MenuBar.png">
 
-<!-- ###### <p align='center'>MenuBar Screenshot<p> -->
+###### <p align='center'>MenuBar Screenshot<p>
 
 #### Currently Supported Themes
 
 - Adapta
 - Arc
 - Aquativo
 - Black
@@ -117,14 +118,47 @@
 - Kroc
 - Plastik
 - Radiance (Ubuntu)
 - Smog
 - Win XP
 - Yaru
 
+## Code Description
+
+To know more about the code structure and module information like - 
+
+- Modules that are imported
+    
+    - Internal (all the modules used that already come with your python interpreter)
+
+    - External (all the modules used that were installed using pip, these are also mentioned in pyproject.toml and requirements.txt)
+
+    - Project specifiv (all the modules used that were specifically created for this project.)
+
+- Hierarchy
+    
+    The hierarchy of classes and functions.
+
+- Individial Object Descriptions
+
+    Descriptions about individual components of the code such as funtions and parameters.
+
+- Working
+
+    If there is any working rule or basic working of the module.
+
+All these can be seen by running the following commands:
+
+```console
+# pasta-man v1.0.9 and above supports docstring fetching, and can be done using:
+
+# in the terminal/CMD, run
+$ pasta-man -dwl # for docs with listing of hierarchy.
+```
+
 ## Dependencies
 - Python>=3.9
 - pandas
 - tk
 - ttkthemes
 - termcolor
 - pyperclip
@@ -133,15 +167,15 @@
 - pyinstaller
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.0.8
+pip install pasta-man==1.0.9
 ```
 
 ## README before [#Usage](#usage)
 
 After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man>=1.0.4` -> `pasta-man` and `pasta-man-launcher`.
 
 - `pasta-man` Command
```

### Comparing `pasta_man-1.0.8/README.md` & `pasta_man-1.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 ![PyPI - Version](https://img.shields.io/pypi/v/pasta-man)
+![PyPI - Status](https://img.shields.io/pypi/status/pasta-man)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pasta-man)
 ![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/pasta-man)
 ![PyPI - License](https://img.shields.io/pypi/l/pasta-man)
 
 
 # Overview
 Pasta-Man is a software application designed to securely store passwords and sensitive information in an encrypted format. It provides users with a convenient way to manage their passwords, ensuring they are protected from unauthorized access. 
@@ -40,19 +41,19 @@
 
 ### Faster than basic tkinter apps
 `Pasta-Man` actively uses Threads to carry out intensive tasks in order to minimize GUI lag as well as have better performance than any basic app created through python tkinter lib.
 
 ### Themes
 User can now change Theme for the app from the Menu Bar. Default is `Arc`. Whatever theme the user chooses, It will be set as default and next time `Pasta-Man` is launched, that theme will be loaded.
 
-Themes can be changed using the MenuBar.
+Themes can be changed using the MenuBar -
 
-<!-- <img src="images/MenuBar.png"> -->
+<img src="images/MenuBar.png">
 
-<!-- ###### <p align='center'>MenuBar Screenshot<p> -->
+###### <p align='center'>MenuBar Screenshot<p>
 
 #### Currently Supported Themes
 
 - Adapta
 - Arc
 - Aquativo
 - Black
@@ -65,14 +66,47 @@
 - Kroc
 - Plastik
 - Radiance (Ubuntu)
 - Smog
 - Win XP
 - Yaru
 
+## Code Description
+
+To know more about the code structure and module information like - 
+
+- Modules that are imported
+    
+    - Internal (all the modules used that already come with your python interpreter)
+
+    - External (all the modules used that were installed using pip, these are also mentioned in pyproject.toml and requirements.txt)
+
+    - Project specifiv (all the modules used that were specifically created for this project.)
+
+- Hierarchy
+    
+    The hierarchy of classes and functions.
+
+- Individial Object Descriptions
+
+    Descriptions about individual components of the code such as funtions and parameters.
+
+- Working
+
+    If there is any working rule or basic working of the module.
+
+All these can be seen by running the following commands:
+
+```console
+# pasta-man v1.0.9 and above supports docstring fetching, and can be done using:
+
+# in the terminal/CMD, run
+$ pasta-man -dwl # for docs with listing of hierarchy.
+```
+
 ## Dependencies
 - Python>=3.9
 - pandas
 - tk
 - ttkthemes
 - termcolor
 - pyperclip
@@ -81,15 +115,15 @@
 - pyinstaller
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.0.8
+pip install pasta-man==1.0.9
 ```
 
 ## README before [#Usage](#usage)
 
 After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man>=1.0.4` -> `pasta-man` and `pasta-man-launcher`.
 
 - `pasta-man` Command
```

### Comparing `pasta_man-1.0.8/pyproject.toml` & `pasta_man-1.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pasta-man"
-version = "1.0.8"
+version = "1.0.9"
 description = "Password Manager"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Software Development",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `pasta_man-1.0.8/src/pasta_man/architectures/gui.py` & `pasta_man-1.0.9/src/pasta_man/architectures/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         self.arch = targets(masterpassword)
         
         # set menu
         menu = Menu(self.parent)
         self.parent.config(menu=menu)
         # -> add menus
         self.pasta_menu = __menu__(menuparent=menu)
+        # self.pasta_menu.Data()
         self.pasta_menu.Themes()
         
         # create Enclosing Frame
         self.EF = ttk.Frame(self.parent)
         self.EF.pack(fill=BOTH, expand=True)
         
         self.initthread = threading.Thread(target=self.arch.init).start()
```

### Comparing `pasta_man-1.0.8/src/pasta_man/architectures/targets.py` & `pasta_man-1.0.9/src/pasta_man/architectures/targets.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.8/src/pasta_man/utilities/pasta_menu.py` & `pasta_man-1.0.9/src/pasta_man/utilities/pasta_menu.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,22 @@
         if not there(jPath(str(Path.home()), '.pastaman', '.defaulttheme')):
             self.style:ttkthemes.themed_style.ThemedStyle = ttkthemes.themed_style.ThemedStyle(theme='arc')
         else:
             with open(jPath(str(Path.home()), '.pastaman', '.defaulttheme'), 'r') as theme:
                 self.defaultTheme = theme.read().replace('\n', '')
                 self.style:ttkthemes.themed_style.ThemedStyle = ttkthemes.themed_style.ThemedStyle(theme=self.defaultTheme)
     
+    def Data(self):
+        DataMenu = Menu(self.parent)
+        
+        self.parent.add_cascade(label="Data", menu=DataMenu)
+        
+        DataMenu.add_command(label="Import")
+        DataMenu.add_command(label="Export")
+    
     def Themes(self):
         ThemeMenu = Menu(self.parent)
         
         self.parent.add_cascade(label="Themes", menu=ThemeMenu)
         
         # Themes Functions #
         def savetheme(theme:str):
```

### Comparing `pasta_man-1.0.8/src/pasta_man.egg-info/PKG-INFO` & `pasta_man-1.0.9/src/pasta_man.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta-man
-Version: 1.0.8
+Version: 1.0.9
 Summary: Password Manager
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>, Sairam Pimple <sairampimple003@gmail.com>, Shubham Narendra Singh <shubh1122000@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -47,14 +47,15 @@
 Requires-Dist: tk
 Requires-Dist: optioner>=1.5.2
 Requires-Dist: pyperclip
 Requires-Dist: ttkthemes
 Requires-Dist: pyinstaller
 
 ![PyPI - Version](https://img.shields.io/pypi/v/pasta-man)
+![PyPI - Status](https://img.shields.io/pypi/status/pasta-man)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pasta-man)
 ![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/pasta-man)
 ![PyPI - License](https://img.shields.io/pypi/l/pasta-man)
 
 
 # Overview
 Pasta-Man is a software application designed to securely store passwords and sensitive information in an encrypted format. It provides users with a convenient way to manage their passwords, ensuring they are protected from unauthorized access. 
@@ -92,19 +93,19 @@
 
 ### Faster than basic tkinter apps
 `Pasta-Man` actively uses Threads to carry out intensive tasks in order to minimize GUI lag as well as have better performance than any basic app created through python tkinter lib.
 
 ### Themes
 User can now change Theme for the app from the Menu Bar. Default is `Arc`. Whatever theme the user chooses, It will be set as default and next time `Pasta-Man` is launched, that theme will be loaded.
 
-Themes can be changed using the MenuBar.
+Themes can be changed using the MenuBar -
 
-<!-- <img src="images/MenuBar.png"> -->
+<img src="images/MenuBar.png">
 
-<!-- ###### <p align='center'>MenuBar Screenshot<p> -->
+###### <p align='center'>MenuBar Screenshot<p>
 
 #### Currently Supported Themes
 
 - Adapta
 - Arc
 - Aquativo
 - Black
@@ -117,14 +118,47 @@
 - Kroc
 - Plastik
 - Radiance (Ubuntu)
 - Smog
 - Win XP
 - Yaru
 
+## Code Description
+
+To know more about the code structure and module information like - 
+
+- Modules that are imported
+    
+    - Internal (all the modules used that already come with your python interpreter)
+
+    - External (all the modules used that were installed using pip, these are also mentioned in pyproject.toml and requirements.txt)
+
+    - Project specifiv (all the modules used that were specifically created for this project.)
+
+- Hierarchy
+    
+    The hierarchy of classes and functions.
+
+- Individial Object Descriptions
+
+    Descriptions about individual components of the code such as funtions and parameters.
+
+- Working
+
+    If there is any working rule or basic working of the module.
+
+All these can be seen by running the following commands:
+
+```console
+# pasta-man v1.0.9 and above supports docstring fetching, and can be done using:
+
+# in the terminal/CMD, run
+$ pasta-man -dwl # for docs with listing of hierarchy.
+```
+
 ## Dependencies
 - Python>=3.9
 - pandas
 - tk
 - ttkthemes
 - termcolor
 - pyperclip
@@ -133,15 +167,15 @@
 - pyinstaller
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.0.8
+pip install pasta-man==1.0.9
 ```
 
 ## README before [#Usage](#usage)
 
 After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man>=1.0.4` -> `pasta-man` and `pasta-man-launcher`.
 
 - `pasta-man` Command
```

### Comparing `pasta_man-1.0.8/src/pasta_man.egg-info/SOURCES.txt` & `pasta_man-1.0.9/src/pasta_man.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 src/pasta_man/architectures/__init__.py
 src/pasta_man/architectures/gui.py
 src/pasta_man/architectures/targets.py
 src/pasta_man/self_launch_thread/Launcher.py
 src/pasta_man/self_launch_thread/__init__.py
 src/pasta_man/utilities/__init__.py
 src/pasta_man/utilities/helptext.py
+src/pasta_man/utilities/pasta_docs.py
 src/pasta_man/utilities/pasta_menu.py
```

