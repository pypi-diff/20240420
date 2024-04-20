# Comparing `tmp/dosview-0.1.2.tar.gz` & `tmp/dosview-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dosview-0.1.2.tar", last modified: Tue Apr 16 20:38:48 2024, max compression
+gzip compressed data, was "dosview-0.1.3.tar", last modified: Fri Apr 19 11:04:19 2024, max compression
```

## Comparing `dosview-0.1.2.tar` & `dosview-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:38:48.943755 dosview-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-16 20:38:48.943755 dosview-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-16 20:38:22.000000 dosview-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:38:48.939755 dosview-0.1.2/dosview/
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-16 20:38:22.000000 dosview-0.1.2/dosview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-16 20:38:22.000000 dosview-0.1.2/dosview.desktop
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:38:48.943755 dosview-0.1.2/dosview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-16 20:38:48.000000 dosview-0.1.2/dosview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-16 20:38:48.000000 dosview-0.1.2/dosview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:38:48.000000 dosview-0.1.2/dosview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-16 20:38:48.000000 dosview-0.1.2/dosview.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-16 20:38:48.000000 dosview-0.1.2/dosview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 20:38:48.000000 dosview-0.1.2/dosview.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:38:48.939755 dosview-0.1.2/media/
--rw-r--r--   0 runner    (1001) docker     (127)    14178 2024-04-16 20:38:22.000000 dosview-0.1.2/media/icon_ust.png
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 20:38:48.943755 dosview-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-16 20:38:22.000000 dosview-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:04:19.761426 dosview-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-19 11:04:19.761426 dosview-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-19 11:03:41.000000 dosview-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:04:19.757426 dosview-0.1.3/dosview/
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-04-19 11:03:41.000000 dosview-0.1.3/dosview/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:04:19.761426 dosview-0.1.3/dosview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-19 11:04:19.000000 dosview-0.1.3/dosview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-19 11:04:19.000000 dosview-0.1.3/dosview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 11:04:19.000000 dosview-0.1.3/dosview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 11:04:19.000000 dosview-0.1.3/dosview.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-19 11:04:19.000000 dosview-0.1.3/dosview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 11:04:19.000000 dosview-0.1.3/dosview.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 11:04:19.761426 dosview-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-19 11:03:41.000000 dosview-0.1.3/setup.py
```

### Comparing `dosview-0.1.2/PKG-INFO` & `dosview-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: dosview
-Version: 0.1.2
+Version: 0.1.3
 Summary: A .dos file viewer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyqt5
+Requires-Dist: pyqtgraph
 
 # Dosview
 
 ## Overview
 **Dosview** is a lightweight, efficient log viewer written in Python3, utilizing the Qt framework for its graphical interface. It is designed to facilitate quick viewing and analysis of log files directly from the command line.
 
+![obrazek](https://github.com/UniversalScientificTechnologies/dosview/assets/5196729/7279580d-4de3-4dfe-9a29-1a9149133691)
+
+
+
 ## Features
 - **Command Line Interface**: Start viewing logs with a simple command.
 - **Fast Performance**: Optimized for quick loading and smooth scrolling through large log files.
 - **Cross-Platform Compatibility**: Works on any platform that supports Python and Qt.
 - **Callable from gui**: Dosimeter file can be opened from graphical file browser. 
 
 ## Installation
@@ -39,15 +44,27 @@
 ### From GitHub Repository Using pip
 1. Ensure you have pip installed on your system.
 2. Run the following command to install directly from GitHub:
    ```
    sudo pip3 install git+https://github.com/UniversalScientificTechnologies/dosview.git
    ```
 
+### From local repository clone using pip
+1. solve requirements from previous instructions
+2. Clone your repository 
+```
+  git clone git://github.com:UniversalScientificTechnologies/dosview.git
+  cd dosview
+  sudo pip3 install . 
+```
+
 ### From setup.py
+
+> This way is not recomended
+
 1. Download the source code from the GitHub repository.
 2. Navigate to the directory containing `setup.py`.
 3. Run the following command:
    ```
    sudo python3 setup.py install
    ```
    This will install the necessary dependencies and the dosview tool.
```

### Comparing `dosview-0.1.2/README.md` & `dosview-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Dosview
 
 ## Overview
 **Dosview** is a lightweight, efficient log viewer written in Python3, utilizing the Qt framework for its graphical interface. It is designed to facilitate quick viewing and analysis of log files directly from the command line.
 
+![obrazek](https://github.com/UniversalScientificTechnologies/dosview/assets/5196729/7279580d-4de3-4dfe-9a29-1a9149133691)
+
+
+
 ## Features
 - **Command Line Interface**: Start viewing logs with a simple command.
 - **Fast Performance**: Optimized for quick loading and smooth scrolling through large log files.
 - **Cross-Platform Compatibility**: Works on any platform that supports Python and Qt.
 - **Callable from gui**: Dosimeter file can be opened from graphical file browser. 
 
 ## Installation
@@ -21,15 +25,27 @@
 ### From GitHub Repository Using pip
 1. Ensure you have pip installed on your system.
 2. Run the following command to install directly from GitHub:
    ```
    sudo pip3 install git+https://github.com/UniversalScientificTechnologies/dosview.git
    ```
 
+### From local repository clone using pip
+1. solve requirements from previous instructions
+2. Clone your repository 
+```
+  git clone git://github.com:UniversalScientificTechnologies/dosview.git
+  cd dosview
+  sudo pip3 install . 
+```
+
 ### From setup.py
+
+> This way is not recomended
+
 1. Download the source code from the GitHub repository.
 2. Navigate to the directory containing `setup.py`.
 3. Run the following command:
    ```
    sudo python3 setup.py install
    ```
    This will install the necessary dependencies and the dosview tool.
```

### Comparing `dosview-0.1.2/dosview.egg-info/PKG-INFO` & `dosview-0.1.3/dosview.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: dosview
-Version: 0.1.2
+Version: 0.1.3
 Summary: A .dos file viewer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyqt5
+Requires-Dist: pyqtgraph
 
 # Dosview
 
 ## Overview
 **Dosview** is a lightweight, efficient log viewer written in Python3, utilizing the Qt framework for its graphical interface. It is designed to facilitate quick viewing and analysis of log files directly from the command line.
 
+![obrazek](https://github.com/UniversalScientificTechnologies/dosview/assets/5196729/7279580d-4de3-4dfe-9a29-1a9149133691)
+
+
+
 ## Features
 - **Command Line Interface**: Start viewing logs with a simple command.
 - **Fast Performance**: Optimized for quick loading and smooth scrolling through large log files.
 - **Cross-Platform Compatibility**: Works on any platform that supports Python and Qt.
 - **Callable from gui**: Dosimeter file can be opened from graphical file browser. 
 
 ## Installation
@@ -39,15 +44,27 @@
 ### From GitHub Repository Using pip
 1. Ensure you have pip installed on your system.
 2. Run the following command to install directly from GitHub:
    ```
    sudo pip3 install git+https://github.com/UniversalScientificTechnologies/dosview.git
    ```
 
+### From local repository clone using pip
+1. solve requirements from previous instructions
+2. Clone your repository 
+```
+  git clone git://github.com:UniversalScientificTechnologies/dosview.git
+  cd dosview
+  sudo pip3 install . 
+```
+
 ### From setup.py
+
+> This way is not recomended
+
 1. Download the source code from the GitHub repository.
 2. Navigate to the directory containing `setup.py`.
 3. Run the following command:
    ```
    sudo python3 setup.py install
    ```
    This will install the necessary dependencies and the dosview tool.
```

