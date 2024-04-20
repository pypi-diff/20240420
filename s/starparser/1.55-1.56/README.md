# Comparing `tmp/starparser-1.55.tar.gz` & `tmp/starparser-1.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starparser-1.55.tar", last modified: Mon Apr  8 19:13:22 2024, max compression
+gzip compressed data, was "starparser-1.56.tar", last modified: Sat Apr 20 08:52:32 2024, max compression
```

## Comparing `starparser-1.55.tar` & `starparser-1.56.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-08 19:13:22.984596 starparser-1.55/
--rw-r--r--   0 chaaban    (501) staff       (20)     1069 2023-06-05 21:07:33.000000 starparser-1.55/LICENSE.txt
--rw-r--r--   0 chaaban    (501) staff       (20)    36955 2024-04-08 19:13:22.984473 starparser-1.55/PKG-INFO
--rw-r--r--   0 chaaban    (501) staff       (20)    36652 2024-04-07 12:48:53.000000 starparser-1.55/README.md
--rw-r--r--   0 chaaban    (501) staff       (20)       38 2024-04-08 19:13:22.984649 starparser-1.55/setup.cfg
--rw-r--r--   0 chaaban    (501) staff       (20)      880 2023-08-26 16:02:58.000000 starparser-1.55/setup.py
-drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-08 19:13:22.983426 starparser-1.55/starparser/
--rw-r--r--   0 chaaban    (501) staff       (20)       82 2024-04-08 19:02:33.000000 starparser-1.55/starparser/__init__.py
--rw-r--r--   0 chaaban    (501) staff       (20)      119 2023-08-11 15:52:04.000000 starparser-1.55/starparser/__main__.py
--rw-r--r--   0 chaaban    (501) staff       (20)    20433 2024-04-07 12:48:12.000000 starparser-1.55/starparser/argparser.py
--rw-r--r--   0 chaaban    (501) staff       (20)     9351 2024-01-27 11:30:44.000000 starparser-1.55/starparser/columnplay.py
--rw-r--r--   0 chaaban    (501) staff       (20)    52470 2024-04-07 12:48:26.000000 starparser-1.55/starparser/decisiontree.py
--rw-r--r--   0 chaaban    (501) staff       (20)    10501 2024-04-08 15:16:19.000000 starparser-1.55/starparser/fileparser.py
--rw-r--r--   0 chaaban    (501) staff       (20)    22901 2024-04-08 19:02:22.000000 starparser-1.55/starparser/particleplay.py
--rw-r--r--   0 chaaban    (501) staff       (20)    26805 2023-09-02 00:09:18.000000 starparser-1.55/starparser/plots.py
--rw-r--r--   0 chaaban    (501) staff       (20)    13056 2023-08-26 18:27:37.000000 starparser-1.55/starparser/specialparticles.py
--rw-r--r--   0 chaaban    (501) staff       (20)     1890 2023-08-11 15:52:04.000000 starparser-1.55/starparser/splits.py
-drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-08 19:13:22.984276 starparser-1.55/starparser.egg-info/
--rw-r--r--   0 chaaban    (501) staff       (20)    36955 2024-04-08 19:13:22.000000 starparser-1.55/starparser.egg-info/PKG-INFO
--rw-r--r--   0 chaaban    (501) staff       (20)      482 2024-04-08 19:13:22.000000 starparser-1.55/starparser.egg-info/SOURCES.txt
--rw-r--r--   0 chaaban    (501) staff       (20)        1 2024-04-08 19:13:22.000000 starparser-1.55/starparser.egg-info/dependency_links.txt
--rw-r--r--   0 chaaban    (501) staff       (20)       56 2024-04-08 19:13:22.000000 starparser-1.55/starparser.egg-info/entry_points.txt
--rw-r--r--   0 chaaban    (501) staff       (20)       30 2024-04-08 19:13:22.000000 starparser-1.55/starparser.egg-info/requires.txt
--rw-r--r--   0 chaaban    (501) staff       (20)       11 2024-04-08 19:13:22.000000 starparser-1.55/starparser.egg-info/top_level.txt
+drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-20 08:52:32.201653 starparser-1.56/
+-rw-r--r--   0 chaaban    (501) staff       (20)     1069 2023-06-05 21:07:33.000000 starparser-1.56/LICENSE.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)    36912 2024-04-20 08:52:32.201526 starparser-1.56/PKG-INFO
+-rw-r--r--   0 chaaban    (501) staff       (20)    36609 2024-04-08 21:18:39.000000 starparser-1.56/README.md
+-rw-r--r--   0 chaaban    (501) staff       (20)       38 2024-04-20 08:52:32.201712 starparser-1.56/setup.cfg
+-rw-r--r--   0 chaaban    (501) staff       (20)      880 2023-08-26 16:02:58.000000 starparser-1.56/setup.py
+drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-20 08:52:32.200545 starparser-1.56/starparser/
+-rw-r--r--   0 chaaban    (501) staff       (20)       82 2024-04-20 08:51:20.000000 starparser-1.56/starparser/__init__.py
+-rw-r--r--   0 chaaban    (501) staff       (20)      119 2023-08-11 15:52:04.000000 starparser-1.56/starparser/__main__.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    20433 2024-04-07 12:48:12.000000 starparser-1.56/starparser/argparser.py
+-rw-r--r--   0 chaaban    (501) staff       (20)     9351 2024-01-27 11:30:44.000000 starparser-1.56/starparser/columnplay.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    52470 2024-04-07 12:48:26.000000 starparser-1.56/starparser/decisiontree.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    10501 2024-04-08 15:16:19.000000 starparser-1.56/starparser/fileparser.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    22907 2024-04-20 08:37:29.000000 starparser-1.56/starparser/particleplay.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    26805 2023-09-02 00:09:18.000000 starparser-1.56/starparser/plots.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    13056 2023-08-26 18:27:37.000000 starparser-1.56/starparser/specialparticles.py
+-rw-r--r--   0 chaaban    (501) staff       (20)     1890 2023-08-11 15:52:04.000000 starparser-1.56/starparser/splits.py
+drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-20 08:52:32.201329 starparser-1.56/starparser.egg-info/
+-rw-r--r--   0 chaaban    (501) staff       (20)    36912 2024-04-20 08:52:32.000000 starparser-1.56/starparser.egg-info/PKG-INFO
+-rw-r--r--   0 chaaban    (501) staff       (20)      482 2024-04-20 08:52:32.000000 starparser-1.56/starparser.egg-info/SOURCES.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)        1 2024-04-20 08:52:32.000000 starparser-1.56/starparser.egg-info/dependency_links.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)       56 2024-04-20 08:52:32.000000 starparser-1.56/starparser.egg-info/entry_points.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)       30 2024-04-20 08:52:32.000000 starparser-1.56/starparser.egg-info/requires.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)       11 2024-04-20 08:52:32.000000 starparser-1.56/starparser.egg-info/top_level.txt
```

### Comparing `starparser-1.55/LICENSE.txt` & `starparser-1.56/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starparser-1.55/PKG-INFO` & `starparser-1.56/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starparser
-Version: 1.55
+Version: 1.56
 Summary: Manipulate and mine Relion star files.
 Home-page: http://pypi.python.org/pypi/starparser/
 Author: Sami Chaaban
 Author-email: chaaban@mrc-lmb.cam.ac.uk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -264,15 +264,15 @@
 
 Pass this if you want an exact match of the values to the query(ies) provided by ```--q```. For example, you must pass this if you want just to look for "1" and ignore "15" (which has a "1" in it).
 
 ### Other
 
 **```--opticsless```**
 
-Pass this if the input star file lacks an optics group (more specifically: the star file has exactly one table), such as with Relion 3.0 files. It will create a dummy optics table before moving on. This option does not work with ```--plot_class_proportions``` or commands that require parsing a second file.
+Pass this if the input star file lacks an optics group (more specifically: the star file has exactly one table), such as with Relion 3.0 files. This option does not work with ```--plot_class_proportions``` and most commands that also require parsing a second file.
 
 ### Output<a name="output"></a>
 
 **```--o```** *```filename```*
 
 Output file name. Default is output.star.
```

### Comparing `starparser-1.55/README.md` & `starparser-1.56/starparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: starparser
+Version: 1.56
+Summary: Manipulate and mine Relion star files.
+Home-page: http://pypi.python.org/pypi/starparser/
+Author: Sami Chaaban
+Author-email: chaaban@mrc-lmb.cam.ac.uk
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # starparser
 
 Use this package to manipulate Relion star files, including counting, modifying, plotting, and sifting the data. At the very least, this is a useful alternative to *awk* commands, which can get *awk*ward. Below is a description of the command-line options with some examples. Alternatively, use starparser within Relion or load the modules in your own Python scripts.
 
 Some of the options below are already available in Relion with "relion_star_handler".
 
 1. [Installation](#installation)
@@ -253,15 +264,15 @@
 
 Pass this if you want an exact match of the values to the query(ies) provided by ```--q```. For example, you must pass this if you want just to look for "1" and ignore "15" (which has a "1" in it).
 
 ### Other
 
 **```--opticsless```**
 
-Pass this if the input star file lacks an optics group (more specifically: the star file has exactly one table), such as with Relion 3.0 files. It will create a dummy optics table before moving on. This option does not work with ```--plot_class_proportions``` or commands that require parsing a second file.
+Pass this if the input star file lacks an optics group (more specifically: the star file has exactly one table), such as with Relion 3.0 files. This option does not work with ```--plot_class_proportions``` and most commands that also require parsing a second file.
 
 ### Output<a name="output"></a>
 
 **```--o```** *```filename```*
 
 Output file name. Default is output.star.
```

### Comparing `starparser-1.55/setup.py` & `starparser-1.56/setup.py`

 * *Files identical despite different names*

### Comparing `starparser-1.55/starparser/argparser.py` & `starparser-1.56/starparser/argparser.py`

 * *Files identical despite different names*

### Comparing `starparser-1.55/starparser/columnplay.py` & `starparser-1.56/starparser/columnplay.py`

 * *Files identical despite different names*

### Comparing `starparser-1.55/starparser/decisiontree.py` & `starparser-1.56/starparser/decisiontree.py`

 * *Files identical despite different names*

### Comparing `starparser-1.55/starparser/fileparser.py` & `starparser-1.56/starparser/fileparser.py`

 * *Files identical despite different names*

### Comparing `starparser-1.55/starparser/particleplay.py` & `starparser-1.56/starparser/particleplay.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 import matplotlib.pyplot as plt
 from matplotlib.widgets import LassoSelector
 from matplotlib.path import Path
 import matplotlib.patches as patches
 
 import warnings
-from matplotlib.cbook import MatplotlibDeprecationWarning
-warnings.filterwarnings("ignore", category=MatplotlibDeprecationWarning)
+#from matplotlib.cbook import MatplotlibDeprecationWarning
+#warnings.filterwarnings("ignore", category=MatplotlibDeprecationWarning)
 
 """
 These functions still require explanations.
 """
 
 """
 --limit
@@ -239,21 +239,21 @@
 """
 --new_optics (also see setparticeoptics())
 """
 def makeopticsgroup(particles,metadata,newgroup):
     
     optics = metadata[2]
     
-    newoptics = optics.append(optics.loc[len(optics.index)-1], ignore_index = True)
+    newoptics = pd.concat([optics, optics.iloc[[len(optics.index)-1]]], ignore_index = True)
     
-    newoptics.loc[len(newoptics.index)-1]["_rlnOpticsGroupName"] = newgroup
+    newoptics.loc[newoptics.index[-1], "_rlnOpticsGroupName"] = newgroup
     
     opticsnumber = int(newoptics.loc[len(newoptics.index)-1]["_rlnOpticsGroup"]) + 1
     
-    newoptics.loc[len(newoptics.index)-1]["_rlnOpticsGroup"] = opticsnumber
+    newoptics.loc[newoptics.index[-1], "_rlnOpticsGroup"] = opticsnumber
     
     return(newoptics, opticsnumber)
 
 """
 --new_optics (also see makeopticsgroup())
 """
 def setparticleoptics(particles,column,query,queryexact,opticsnumber):
@@ -620,8 +620,8 @@
     elif col.startswith("_rn") or col.startswith("rn"):
         print(f"\n>> Error: check the column name {col}.\n")
         sys.exit()
     elif col.startswith("rn") and not col.startswith("rln"):
         print(f"\n>> Error: check the column name {col}.\n")
         sys.exit()
     else:
-        return("_rln"+col)
+        return("_rln"+col)
```

### Comparing `starparser-1.55/starparser/plots.py` & `starparser-1.56/starparser/plots.py`

 * *Files identical despite different names*

### Comparing `starparser-1.55/starparser/specialparticles.py` & `starparser-1.56/starparser/specialparticles.py`

 * *Files identical despite different names*

### Comparing `starparser-1.55/starparser/splits.py` & `starparser-1.56/starparser/splits.py`

 * *Files identical despite different names*

### Comparing `starparser-1.55/starparser.egg-info/PKG-INFO` & `starparser-1.56/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: starparser
-Version: 1.55
-Summary: Manipulate and mine Relion star files.
-Home-page: http://pypi.python.org/pypi/starparser/
-Author: Sami Chaaban
-Author-email: chaaban@mrc-lmb.cam.ac.uk
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # starparser
 
 Use this package to manipulate Relion star files, including counting, modifying, plotting, and sifting the data. At the very least, this is a useful alternative to *awk* commands, which can get *awk*ward. Below is a description of the command-line options with some examples. Alternatively, use starparser within Relion or load the modules in your own Python scripts.
 
 Some of the options below are already available in Relion with "relion_star_handler".
 
 1. [Installation](#installation)
@@ -264,15 +253,15 @@
 
 Pass this if you want an exact match of the values to the query(ies) provided by ```--q```. For example, you must pass this if you want just to look for "1" and ignore "15" (which has a "1" in it).
 
 ### Other
 
 **```--opticsless```**
 
-Pass this if the input star file lacks an optics group (more specifically: the star file has exactly one table), such as with Relion 3.0 files. It will create a dummy optics table before moving on. This option does not work with ```--plot_class_proportions``` or commands that require parsing a second file.
+Pass this if the input star file lacks an optics group (more specifically: the star file has exactly one table), such as with Relion 3.0 files. This option does not work with ```--plot_class_proportions``` and most commands that also require parsing a second file.
 
 ### Output<a name="output"></a>
 
 **```--o```** *```filename```*
 
 Output file name. Default is output.star.
```

