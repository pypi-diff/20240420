# Comparing `tmp/FoxDotEditor-0.9.8.tar.gz` & `tmp/foxdoteditor-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FoxDotEditor-0.9.8.tar", last modified: Tue Feb 13 02:10:56 2024, max compression
+gzip compressed data, was "foxdoteditor-0.9.9.tar", last modified: Sat Apr 20 17:39:00 2024, max compression
```

## Comparing `FoxDotEditor-0.9.8.tar` & `foxdoteditor-0.9.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 02:10:56.909720 FoxDotEditor-0.9.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 02:10:56.905720 FoxDotEditor-0.9.8/FoxDotEditor/
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-02-13 02:10:43.000000 FoxDotEditor-0.9.8/FoxDotEditor/AppFunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-02-13 02:10:43.000000 FoxDotEditor-0.9.8/FoxDotEditor/BracketHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-02-13 02:10:43.000000 FoxDotEditor-0.9.8/FoxDotEditor/ConfigFile.py
--rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-02-13 02:10:43.000000 FoxDotEditor-0.9.8/FoxDotEditor/Console.py
--rw-r--r--   0 runner    (1001) docker     (127)    50918 2024-02-13 02:10:43.000000 FoxDotEditor-0.9.8/FoxDotEditor/Editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-02-13 02:10:43.000000 FoxDotEditor-0.9.8/FoxDotEditor/Format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-02-13 02:10:43.000000 FoxDotEditor-0.9.8/FoxDotEditor/LineNumbers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10178 2024-02-13 02:10:43.000000 FoxDotEditor-0.9.8/FoxDotEditor/MenuBar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-02-13 02:10:43.000000 FoxDotEditor-0.9.8/FoxDotEditor/Prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)    15759 2024-02-13 02:10:43.000000 FoxDotEditor-0.9.8/FoxDotEditor/SampleChart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 02:10:56.909720 FoxDotEditor-0.9.8/FoxDotEditor/Settings/
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-02-13 02:10:43.000000 FoxDotEditor-0.9.8/FoxDotEditor/Settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-02-13 02:10:43.000000 FoxDotEditor-0.9.8/FoxDotEditor/Settings/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-02-13 02:10:43.000000 FoxDotEditor-0.9.8/FoxDotEditor/TextBox.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-02-13 02:10:43.000000 FoxDotEditor-0.9.8/FoxDotEditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-02-13 02:10:43.000000 FoxDotEditor-0.9.8/FoxDotEditor/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 02:10:56.909720 FoxDotEditor-0.9.8/FoxDotEditor/img/
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-02-13 02:10:43.000000 FoxDotEditor-0.9.8/FoxDotEditor/img/foxdot.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-02-13 02:10:43.000000 FoxDotEditor-0.9.8/FoxDotEditor/img/icon.gif
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-02-13 02:10:43.000000 FoxDotEditor-0.9.8/FoxDotEditor/img/icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-13 02:10:43.000000 FoxDotEditor-0.9.8/FoxDotEditor/tkimport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 02:10:56.909720 FoxDotEditor-0.9.8/FoxDotEditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-02-13 02:10:56.000000 FoxDotEditor-0.9.8/FoxDotEditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-02-13 02:10:56.000000 FoxDotEditor-0.9.8/FoxDotEditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 02:10:56.000000 FoxDotEditor-0.9.8/FoxDotEditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-13 02:10:56.000000 FoxDotEditor-0.9.8/FoxDotEditor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-13 02:10:56.000000 FoxDotEditor-0.9.8/FoxDotEditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-13 02:10:56.000000 FoxDotEditor-0.9.8/FoxDotEditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-02-13 02:10:56.909720 FoxDotEditor-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-02-13 02:10:43.000000 FoxDotEditor-0.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 02:10:56.909720 FoxDotEditor-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-02-13 02:10:43.000000 FoxDotEditor-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:39:00.666886 foxdoteditor-0.9.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:39:00.662886 foxdoteditor-0.9.9/FoxDotEditor/
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/AppFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/BracketHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/ConfigFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/Console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50918 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/Editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/Format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/LineNumbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10178 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/MenuBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/Prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15759 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/SampleChart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:39:00.666886 foxdoteditor-0.9.9/FoxDotEditor/Settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/Settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/Settings/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/TextBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:39:00.666886 foxdoteditor-0.9.9/FoxDotEditor/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/img/foxdot.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/img/icon.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/img/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/FoxDotEditor/tkimport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:39:00.666886 foxdoteditor-0.9.9/FoxDotEditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-20 17:39:00.000000 foxdoteditor-0.9.9/FoxDotEditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-20 17:39:00.000000 foxdoteditor-0.9.9/FoxDotEditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 17:39:00.000000 foxdoteditor-0.9.9/FoxDotEditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-20 17:39:00.000000 foxdoteditor-0.9.9/FoxDotEditor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-20 17:39:00.000000 foxdoteditor-0.9.9/FoxDotEditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-20 17:39:00.000000 foxdoteditor-0.9.9/FoxDotEditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-20 17:39:00.666886 foxdoteditor-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 17:39:00.666886 foxdoteditor-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-20 17:38:56.000000 foxdoteditor-0.9.9/setup.py
```

### Comparing `FoxDotEditor-0.9.8/FoxDotEditor/AppFunctions.py` & `foxdoteditor-0.9.9/FoxDotEditor/AppFunctions.py`

 * *Files identical despite different names*

### Comparing `FoxDotEditor-0.9.8/FoxDotEditor/BracketHandler.py` & `foxdoteditor-0.9.9/FoxDotEditor/BracketHandler.py`

 * *Files identical despite different names*

### Comparing `FoxDotEditor-0.9.8/FoxDotEditor/ConfigFile.py` & `foxdoteditor-0.9.9/FoxDotEditor/ConfigFile.py`

 * *Files identical despite different names*

### Comparing `FoxDotEditor-0.9.8/FoxDotEditor/Console.py` & `foxdoteditor-0.9.9/FoxDotEditor/Console.py`

 * *Files identical despite different names*

### Comparing `FoxDotEditor-0.9.8/FoxDotEditor/Editor.py` & `foxdoteditor-0.9.9/FoxDotEditor/Editor.py`

 * *Files identical despite different names*

### Comparing `FoxDotEditor-0.9.8/FoxDotEditor/Format.py` & `foxdoteditor-0.9.9/FoxDotEditor/Format.py`

 * *Files identical despite different names*

### Comparing `FoxDotEditor-0.9.8/FoxDotEditor/LineNumbers.py` & `foxdoteditor-0.9.9/FoxDotEditor/LineNumbers.py`

 * *Files identical despite different names*

### Comparing `FoxDotEditor-0.9.8/FoxDotEditor/MenuBar.py` & `foxdoteditor-0.9.9/FoxDotEditor/MenuBar.py`

 * *Files identical despite different names*

### Comparing `FoxDotEditor-0.9.8/FoxDotEditor/Prompt.py` & `foxdoteditor-0.9.9/FoxDotEditor/Prompt.py`

 * *Files identical despite different names*

### Comparing `FoxDotEditor-0.9.8/FoxDotEditor/SampleChart.py` & `foxdoteditor-0.9.9/FoxDotEditor/SampleChart.py`

 * *Files identical despite different names*

### Comparing `FoxDotEditor-0.9.8/FoxDotEditor/Settings/__init__.py` & `foxdoteditor-0.9.9/FoxDotEditor/Settings/__init__.py`

 * *Files identical despite different names*

### Comparing `FoxDotEditor-0.9.8/FoxDotEditor/Settings/conf.py` & `foxdoteditor-0.9.9/FoxDotEditor/Settings/conf.py`

 * *Files identical despite different names*

### Comparing `FoxDotEditor-0.9.8/FoxDotEditor/TextBox.py` & `foxdoteditor-0.9.9/FoxDotEditor/TextBox.py`

 * *Files identical despite different names*

### Comparing `FoxDotEditor-0.9.8/FoxDotEditor/__init__.py` & `foxdoteditor-0.9.9/FoxDotEditor/__init__.py`

 * *Files identical despite different names*

### Comparing `FoxDotEditor-0.9.8/FoxDotEditor/__main__.py` & `foxdoteditor-0.9.9/FoxDotEditor/__main__.py`

 * *Files identical despite different names*

### Comparing `FoxDotEditor-0.9.8/FoxDotEditor/img/foxdot.ico` & `foxdoteditor-0.9.9/FoxDotEditor/img/foxdot.ico`

 * *Files identical despite different names*

### Comparing `FoxDotEditor-0.9.8/FoxDotEditor/img/icon.gif` & `foxdoteditor-0.9.9/FoxDotEditor/img/icon.gif`

 * *Files identical despite different names*

### Comparing `FoxDotEditor-0.9.8/FoxDotEditor/img/icon.ico` & `foxdoteditor-0.9.9/FoxDotEditor/img/icon.ico`

 * *Files identical despite different names*

### Comparing `FoxDotEditor-0.9.8/FoxDotEditor.egg-info/PKG-INFO` & `foxdoteditor-0.9.9/FoxDotEditor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: FoxDotEditor
-Version: 0.9.8
+Version: 0.9.9
 Summary: Original FoxDot editor extracted from FoxDot Project - Live coding music with SuperCollider
 Home-page: http://foxdot.org/
 Author: Elie Gavoty
 Author-email: eliegavoty@free.fr
 License: cc-by-sa-4.0
 Description-Content-Type: text/markdown
-Requires-Dist: renardo-lib==0.9.8
+Requires-Dist: renardo-lib==0.9.9
 Requires-Dist: psutil
 Requires-Dist: playsound
 
 FoxDot - Editor
 =====================================
 
 Original FoxDot editor extract from original project for use with separated FoxDot library or renardo fork.
```

### Comparing `FoxDotEditor-0.9.8/FoxDotEditor.egg-info/SOURCES.txt` & `foxdoteditor-0.9.9/FoxDotEditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FoxDotEditor-0.9.8/PKG-INFO` & `foxdoteditor-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: FoxDotEditor
-Version: 0.9.8
+Version: 0.9.9
 Summary: Original FoxDot editor extracted from FoxDot Project - Live coding music with SuperCollider
 Home-page: http://foxdot.org/
 Author: Elie Gavoty
 Author-email: eliegavoty@free.fr
 License: cc-by-sa-4.0
 Description-Content-Type: text/markdown
-Requires-Dist: renardo-lib==0.9.8
+Requires-Dist: renardo-lib==0.9.9
 Requires-Dist: psutil
 Requires-Dist: playsound
 
 FoxDot - Editor
 =====================================
 
 Original FoxDot editor extract from original project for use with separated FoxDot library or renardo fork.
```

### Comparing `FoxDotEditor-0.9.8/README.md` & `foxdoteditor-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `FoxDotEditor-0.9.8/setup.py` & `foxdoteditor-0.9.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description=f.read()
 
 setup(
     name='FoxDotEditor',
-    version="0.9.8",
+    version="0.9.9",
     description='Original FoxDot editor extracted from FoxDot Project - Live coding music with SuperCollider',
     author='Elie Gavoty',
     author_email='eliegavoty@free.fr',
     license='cc-by-sa-4.0',
     url='http://foxdot.org/',
     packages=['FoxDotEditor', 'FoxDotEditor.Settings'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={'gui_scripts' : ['FoxDotEditor = FoxDotEditor.__init__:main']},
     # data_files=[('', 'LICENSE')],
     package_data = {'FoxDotEditor': ['README.md','img/*','tmp/*'],},
     install_requires=[
-        'renardo-lib==0.9.8',
+        'renardo-lib==0.9.9',
         'psutil',
         'playsound',
     ],
 )
```

