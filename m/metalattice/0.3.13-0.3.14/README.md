# Comparing `tmp/metalattice-0.3.13.tar.gz` & `tmp/metalattice-0.3.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalattice-0.3.13.tar", last modified: Sat Apr 20 06:03:30 2024, max compression
+gzip compressed data, was "metalattice-0.3.14.tar", last modified: Sat Apr 20 06:05:30 2024, max compression
```

## Comparing `metalattice-0.3.13.tar` & `metalattice-0.3.14.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:03:30.018387 metalattice-0.3.13/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:03:30.006387 metalattice-0.3.13/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:03:30.010387 metalattice-0.3.13/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-20 06:03:25.000000 metalattice-0.3.13/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-20 06:03:25.000000 metalattice-0.3.13/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-20 06:03:25.000000 metalattice-0.3.13/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-20 06:03:25.000000 metalattice-0.3.13/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-20 06:03:25.000000 metalattice-0.3.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-20 06:03:30.018387 metalattice-0.3.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-20 06:03:25.000000 metalattice-0.3.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:03:30.010387 metalattice-0.3.13/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-20 06:03:25.000000 metalattice-0.3.13/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-20 06:03:25.000000 metalattice-0.3.13/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-20 06:03:25.000000 metalattice-0.3.13/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:03:30.010387 metalattice-0.3.13/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:03:30.014387 metalattice-0.3.13/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   563164 2024-04-20 06:03:25.000000 metalattice-0.3.13/docs/source/_static/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)   593586 2024-04-20 06:03:25.000000 metalattice-0.3.13/docs/source/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-20 06:03:25.000000 metalattice-0.3.13/docs/source/_static/metalattice.css
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-20 06:03:25.000000 metalattice-0.3.13/docs/source/_static/switcher.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:03:30.006387 metalattice-0.3.13/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:03:30.014387 metalattice-0.3.13/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-20 06:03:25.000000 metalattice-0.3.13/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-04-20 06:03:25.000000 metalattice-0.3.13/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-20 06:03:25.000000 metalattice-0.3.13/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:03:30.014387 metalattice-0.3.13/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-20 06:03:25.000000 metalattice-0.3.13/docs/source/reference/abaqus.rst
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-20 06:03:25.000000 metalattice-0.3.13/docs/source/reference/geom.rst
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-20 06:03:25.000000 metalattice-0.3.13/docs/source/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-20 06:03:25.000000 metalattice-0.3.13/docs/source/reference/lattice.rst
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-20 06:03:25.000000 metalattice-0.3.13/docs/source/reference/main_namespace.rst
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-20 06:03:25.000000 metalattice-0.3.13/docs/source/reference/material.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:03:30.014387 metalattice-0.3.13/docs/source/release/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-20 06:03:25.000000 metalattice-0.3.13/docs/source/release/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:03:30.014387 metalattice-0.3.13/docs/source/user/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-20 06:03:25.000000 metalattice-0.3.13/docs/source/user/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-20 06:03:25.000000 metalattice-0.3.13/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 06:03:30.018387 metalattice-0.3.13/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:03:30.010387 metalattice-0.3.13/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:03:30.014387 metalattice-0.3.13/src/metalattice/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-20 06:03:25.000000 metalattice-0.3.13/src/metalattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-20 06:03:29.000000 metalattice-0.3.13/src/metalattice/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:03:30.014387 metalattice-0.3.13/src/metalattice/abaqus/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-20 06:03:25.000000 metalattice-0.3.13/src/metalattice/abaqus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:03:30.014387 metalattice-0.3.13/src/metalattice/geom/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-20 06:03:25.000000 metalattice-0.3.13/src/metalattice/geom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:03:30.014387 metalattice-0.3.13/src/metalattice/lattice/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-20 06:03:25.000000 metalattice-0.3.13/src/metalattice/lattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-20 06:03:25.000000 metalattice-0.3.13/src/metalattice/logo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:03:30.014387 metalattice-0.3.13/src/metalattice/material/
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-20 06:03:25.000000 metalattice-0.3.13/src/metalattice/material/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:03:30.014387 metalattice-0.3.13/src/metalattice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-20 06:03:29.000000 metalattice-0.3.13/src/metalattice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-20 06:03:30.000000 metalattice-0.3.13/src/metalattice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 06:03:29.000000 metalattice-0.3.13/src/metalattice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-20 06:03:29.000000 metalattice-0.3.13/src/metalattice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-20 06:03:29.000000 metalattice-0.3.13/src/metalattice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:05:29.999821 metalattice-0.3.14/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:05:29.991821 metalattice-0.3.14/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:05:29.991821 metalattice-0.3.14/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-20 06:05:25.000000 metalattice-0.3.14/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-20 06:05:25.000000 metalattice-0.3.14/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-20 06:05:25.000000 metalattice-0.3.14/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-20 06:05:25.000000 metalattice-0.3.14/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-20 06:05:25.000000 metalattice-0.3.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-20 06:05:29.999821 metalattice-0.3.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-20 06:05:25.000000 metalattice-0.3.14/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:05:29.991821 metalattice-0.3.14/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-20 06:05:25.000000 metalattice-0.3.14/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-20 06:05:25.000000 metalattice-0.3.14/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-20 06:05:25.000000 metalattice-0.3.14/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:05:29.995821 metalattice-0.3.14/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:05:29.995821 metalattice-0.3.14/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   563164 2024-04-20 06:05:25.000000 metalattice-0.3.14/docs/source/_static/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   593586 2024-04-20 06:05:25.000000 metalattice-0.3.14/docs/source/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-20 06:05:25.000000 metalattice-0.3.14/docs/source/_static/metalattice.css
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-20 06:05:25.000000 metalattice-0.3.14/docs/source/_static/switcher.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:05:29.991821 metalattice-0.3.14/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:05:29.995821 metalattice-0.3.14/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-20 06:05:25.000000 metalattice-0.3.14/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-04-20 06:05:25.000000 metalattice-0.3.14/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-20 06:05:25.000000 metalattice-0.3.14/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:05:29.995821 metalattice-0.3.14/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-20 06:05:25.000000 metalattice-0.3.14/docs/source/reference/abaqus.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-20 06:05:25.000000 metalattice-0.3.14/docs/source/reference/geom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-20 06:05:25.000000 metalattice-0.3.14/docs/source/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-20 06:05:25.000000 metalattice-0.3.14/docs/source/reference/lattice.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-20 06:05:25.000000 metalattice-0.3.14/docs/source/reference/main_namespace.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-20 06:05:25.000000 metalattice-0.3.14/docs/source/reference/material.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:05:29.995821 metalattice-0.3.14/docs/source/release/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-20 06:05:25.000000 metalattice-0.3.14/docs/source/release/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:05:29.995821 metalattice-0.3.14/docs/source/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-20 06:05:25.000000 metalattice-0.3.14/docs/source/user/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-20 06:05:25.000000 metalattice-0.3.14/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 06:05:29.999821 metalattice-0.3.14/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:05:29.991821 metalattice-0.3.14/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:05:29.999821 metalattice-0.3.14/src/metalattice/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-20 06:05:25.000000 metalattice-0.3.14/src/metalattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-20 06:05:29.000000 metalattice-0.3.14/src/metalattice/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:05:29.999821 metalattice-0.3.14/src/metalattice/abaqus/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-20 06:05:25.000000 metalattice-0.3.14/src/metalattice/abaqus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:05:29.999821 metalattice-0.3.14/src/metalattice/geom/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-20 06:05:25.000000 metalattice-0.3.14/src/metalattice/geom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:05:29.999821 metalattice-0.3.14/src/metalattice/lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-20 06:05:25.000000 metalattice-0.3.14/src/metalattice/lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-20 06:05:25.000000 metalattice-0.3.14/src/metalattice/logo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:05:29.999821 metalattice-0.3.14/src/metalattice/material/
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-20 06:05:25.000000 metalattice-0.3.14/src/metalattice/material/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:05:29.999821 metalattice-0.3.14/src/metalattice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-20 06:05:29.000000 metalattice-0.3.14/src/metalattice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-20 06:05:29.000000 metalattice-0.3.14/src/metalattice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 06:05:29.000000 metalattice-0.3.14/src/metalattice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-20 06:05:29.000000 metalattice-0.3.14/src/metalattice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-20 06:05:29.000000 metalattice-0.3.14/src/metalattice.egg-info/top_level.txt
```

### Comparing `metalattice-0.3.13/.github/workflows/python-publish.yml` & `metalattice-0.3.14/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.13/.gitignore` & `metalattice-0.3.14/.gitignore`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.13/.readthedocs.yaml` & `metalattice-0.3.14/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.13/LICENSE` & `metalattice-0.3.14/LICENSE`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.13/PKG-INFO` & `metalattice-0.3.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalattice
-Version: 0.3.13
+Version: 0.3.14
 Summary: A Python package to model lattice metamaterials, using Abaqus.
 Author-email: Huang Lihao <huang-lihao@outlook.com>
 Maintainer-email: Huang Lihao <huang-lihao@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 HUANG Lihao (黄立昊)
```

### Comparing `metalattice-0.3.13/README.md` & `metalattice-0.3.14/README.md`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.13/docs/Makefile` & `metalattice-0.3.14/docs/Makefile`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.13/docs/make.bat` & `metalattice-0.3.14/docs/make.bat`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.13/docs/source/_static/favicon.svg` & `metalattice-0.3.14/docs/source/_static/favicon.svg`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.13/docs/source/_static/logo.svg` & `metalattice-0.3.14/docs/source/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.13/docs/source/_static/metalattice.css` & `metalattice-0.3.14/docs/source/_static/metalattice.css`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.13/docs/source/_templates/autosummary/class.rst` & `metalattice-0.3.14/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.13/docs/source/conf.py` & `metalattice-0.3.14/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,20 +154,21 @@
         lineno = None
 
     if lineno:
         linespec = "#L%d-L%d" % (lineno, lineno + len(source) - 1)
     else:
         linespec = ""
 
-    startdir = os.path.abspath(os.path.join(dirname(metalattice.__file__), '../..'))
+    startdir = os.path.abspath(os.path.join(dirname(metalattice.__file__), '..'))
     fn = relpath(fn, start=startdir).replace(os.path.sep, '/')
 
     print("**********************************************************", fn, linespec)
 
-    if fn.startswith('src/metalattice/'):
+    if fn.startswith('metalattice/'):
+        fn = "src/" + fn
         m = re.match(r'^.*dev0\+([a-f0-9]+)$', metalattice.__version__)
         base_url = "https://github.com/huang-lihao/metalattice/blob"
         if m:
             return f"{base_url}/{m.group(1)}/{fn}{linespec}"
         elif 'dev' in metalattice.__version__:
             return f"{base_url}/main/{fn}{linespec}"
         else:
```

### Comparing `metalattice-0.3.13/docs/source/reference/index.rst` & `metalattice-0.3.14/docs/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.13/docs/source/reference/main_namespace.rst` & `metalattice-0.3.14/docs/source/reference/main_namespace.rst`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.13/pyproject.toml` & `metalattice-0.3.14/pyproject.toml`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.13/src/metalattice/logo.py` & `metalattice-0.3.14/src/metalattice/logo.py`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.13/src/metalattice/material/__init__.py` & `metalattice-0.3.14/src/metalattice/material/__init__.py`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.13/src/metalattice.egg-info/PKG-INFO` & `metalattice-0.3.14/src/metalattice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalattice
-Version: 0.3.13
+Version: 0.3.14
 Summary: A Python package to model lattice metamaterials, using Abaqus.
 Author-email: Huang Lihao <huang-lihao@outlook.com>
 Maintainer-email: Huang Lihao <huang-lihao@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 HUANG Lihao (黄立昊)
```

### Comparing `metalattice-0.3.13/src/metalattice.egg-info/SOURCES.txt` & `metalattice-0.3.14/src/metalattice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

