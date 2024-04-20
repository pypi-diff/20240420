# Comparing `tmp/metalattice-0.3.11.tar.gz` & `tmp/metalattice-0.3.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalattice-0.3.11.tar", last modified: Tue Sep 19 03:06:05 2023, max compression
+gzip compressed data, was "metalattice-0.3.12.tar", last modified: Sat Apr 20 05:52:14 2024, max compression
```

## Comparing `metalattice-0.3.11.tar` & `metalattice-0.3.12.tar`

### file list

```diff
@@ -1,34 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 03:06:05.075506 metalattice-0.3.11/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 03:06:05.071506 metalattice-0.3.11/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 03:06:05.071506 metalattice-0.3.11/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2023-09-19 03:05:55.000000 metalattice-0.3.11/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2023-09-19 03:05:55.000000 metalattice-0.3.11/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-09-19 03:05:55.000000 metalattice-0.3.11/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-09-19 03:05:55.000000 metalattice-0.3.11/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2023-09-19 03:05:55.000000 metalattice-0.3.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2023-09-19 03:06:05.075506 metalattice-0.3.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-09-19 03:05:55.000000 metalattice-0.3.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 03:06:05.071506 metalattice-0.3.11/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-09-19 03:05:55.000000 metalattice-0.3.11/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2023-09-19 03:05:55.000000 metalattice-0.3.11/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-09-19 03:05:55.000000 metalattice-0.3.11/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 03:06:05.071506 metalattice-0.3.11/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 03:06:05.071506 metalattice-0.3.11/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   563164 2023-09-19 03:05:55.000000 metalattice-0.3.11/docs/source/_static/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)   593586 2023-09-19 03:05:55.000000 metalattice-0.3.11/docs/source/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-09-19 03:05:55.000000 metalattice-0.3.11/docs/source/_static/switcher.json
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2023-09-19 03:05:55.000000 metalattice-0.3.11/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2023-09-19 03:05:55.000000 metalattice-0.3.11/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      922 2023-09-19 03:05:55.000000 metalattice-0.3.11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-19 03:06:05.075506 metalattice-0.3.11/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 03:06:05.071506 metalattice-0.3.11/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 03:06:05.071506 metalattice-0.3.11/src/metalattice/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-09-19 03:05:55.000000 metalattice-0.3.11/src/metalattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2023-09-19 03:06:04.000000 metalattice-0.3.11/src/metalattice/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2023-09-19 03:05:55.000000 metalattice-0.3.11/src/metalattice/logo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 03:06:05.071506 metalattice-0.3.11/src/metalattice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2023-09-19 03:06:05.000000 metalattice-0.3.11/src/metalattice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      570 2023-09-19 03:06:05.000000 metalattice-0.3.11/src/metalattice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-19 03:06:05.000000 metalattice-0.3.11/src/metalattice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-09-19 03:06:05.000000 metalattice-0.3.11/src/metalattice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-09-19 03:06:05.000000 metalattice-0.3.11/src/metalattice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:52:14.096677 metalattice-0.3.12/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:52:14.088677 metalattice-0.3.12/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:52:14.092677 metalattice-0.3.12/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-20 05:52:09.000000 metalattice-0.3.12/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-20 05:52:09.000000 metalattice-0.3.12/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-20 05:52:09.000000 metalattice-0.3.12/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-20 05:52:09.000000 metalattice-0.3.12/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-20 05:52:09.000000 metalattice-0.3.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-20 05:52:14.096677 metalattice-0.3.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-20 05:52:09.000000 metalattice-0.3.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:52:14.092677 metalattice-0.3.12/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-20 05:52:09.000000 metalattice-0.3.12/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-20 05:52:09.000000 metalattice-0.3.12/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-20 05:52:09.000000 metalattice-0.3.12/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:52:14.092677 metalattice-0.3.12/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:52:14.092677 metalattice-0.3.12/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   563164 2024-04-20 05:52:09.000000 metalattice-0.3.12/docs/source/_static/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   593586 2024-04-20 05:52:09.000000 metalattice-0.3.12/docs/source/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-20 05:52:09.000000 metalattice-0.3.12/docs/source/_static/metalattice.css
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-20 05:52:09.000000 metalattice-0.3.12/docs/source/_static/switcher.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:52:14.088677 metalattice-0.3.12/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:52:14.092677 metalattice-0.3.12/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-20 05:52:09.000000 metalattice-0.3.12/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-04-20 05:52:09.000000 metalattice-0.3.12/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-20 05:52:09.000000 metalattice-0.3.12/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:52:14.096677 metalattice-0.3.12/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-20 05:52:09.000000 metalattice-0.3.12/docs/source/reference/abaqus.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-20 05:52:09.000000 metalattice-0.3.12/docs/source/reference/geom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-20 05:52:09.000000 metalattice-0.3.12/docs/source/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-20 05:52:09.000000 metalattice-0.3.12/docs/source/reference/lattice.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-20 05:52:09.000000 metalattice-0.3.12/docs/source/reference/main_namespace.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-20 05:52:09.000000 metalattice-0.3.12/docs/source/reference/material.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:52:14.096677 metalattice-0.3.12/docs/source/release/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-20 05:52:09.000000 metalattice-0.3.12/docs/source/release/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:52:14.096677 metalattice-0.3.12/docs/source/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-20 05:52:09.000000 metalattice-0.3.12/docs/source/user/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-20 05:52:09.000000 metalattice-0.3.12/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 05:52:14.096677 metalattice-0.3.12/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:52:14.088677 metalattice-0.3.12/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:52:14.096677 metalattice-0.3.12/src/metalattice/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-20 05:52:09.000000 metalattice-0.3.12/src/metalattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-20 05:52:14.000000 metalattice-0.3.12/src/metalattice/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:52:14.096677 metalattice-0.3.12/src/metalattice/abaqus/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-20 05:52:09.000000 metalattice-0.3.12/src/metalattice/abaqus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:52:14.096677 metalattice-0.3.12/src/metalattice/geom/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-20 05:52:09.000000 metalattice-0.3.12/src/metalattice/geom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:52:14.096677 metalattice-0.3.12/src/metalattice/lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-20 05:52:09.000000 metalattice-0.3.12/src/metalattice/lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-20 05:52:09.000000 metalattice-0.3.12/src/metalattice/logo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:52:14.096677 metalattice-0.3.12/src/metalattice/material/
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-20 05:52:09.000000 metalattice-0.3.12/src/metalattice/material/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:52:14.096677 metalattice-0.3.12/src/metalattice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-20 05:52:14.000000 metalattice-0.3.12/src/metalattice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-20 05:52:14.000000 metalattice-0.3.12/src/metalattice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 05:52:14.000000 metalattice-0.3.12/src/metalattice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-20 05:52:14.000000 metalattice-0.3.12/src/metalattice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-20 05:52:14.000000 metalattice-0.3.12/src/metalattice.egg-info/top_level.txt
```

### Comparing `metalattice-0.3.11/.github/workflows/python-publish.yml` & `metalattice-0.3.12/.github/workflows/python-publish.yml`

 * *Files 0% similar despite different names*

```diff
@@ -15,19 +15,18 @@
 permissions:
   contents: read
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
-
     # Specifying a GitHub environment is optional, but strongly encouraged
     environment: release
     permissions:
-    # IMPORTANT: this permission is mandatory for trusted publishing
+      # IMPORTANT: this permission is mandatory for trusted publishing
       id-token: write
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v3
       with:
```

### Comparing `metalattice-0.3.11/.gitignore` & `metalattice-0.3.12/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 _version.py
+generated
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `metalattice-0.3.11/.readthedocs.yaml` & `metalattice-0.3.12/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.11/LICENSE` & `metalattice-0.3.12/LICENSE`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.11/PKG-INFO` & `metalattice-0.3.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalattice
-Version: 0.3.11
+Version: 0.3.12
 Summary: A Python package to model lattice metamaterials, using Abaqus.
 Author-email: Huang Lihao <huang-lihao@outlook.com>
 Maintainer-email: Huang Lihao <huang-lihao@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 HUANG Lihao (黄立昊)
         
@@ -39,17 +39,17 @@
 Requires-Dist: gfort2py
 Requires-Dist: matplotlib
 Requires-Dist: meshio
 Requires-Dist: numpy
 Requires-Dist: sympy
 
 # MetaLattice
+[![GitHub](https://img.shields.io/github/license/huang-lihao/metalattice)](LICENSE)
 [![PyPI - Version](https://img.shields.io/pypi/v/metalattice?logo=pypi)](https://pypi.org/project/metalattice/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/metalattice?logo=pypi)](https://pypi.org/project/metalattice/)
-[![GitHub](https://img.shields.io/github/license/huang-lihao/metalattice)](LICENSE)
 [![IJMS Paper](https://img.shields.io/badge/DOI-10.1016/j.ijmecsci.2022.107836-blue)](https://doi.org/10.1016/j.ijmecsci.2022.107836)\
 [![Upload Python Package](https://github.com/huang-lihao/MetaLattice/actions/workflows/python-publish.yml/badge.svg)](https://github.com/huang-lihao/MetaLattice/actions/workflows/python-publish.yml)
 [![Documentation Status](https://readthedocs.org/projects/metalattice/badge/?version=latest)](https://metalattice.readthedocs.io/en/latest/?badge=latest)
 
 Install
 ----------------------
 Use PyPI to install [metalattice](https://pypi.org/project/metalattice/):
```

### Comparing `metalattice-0.3.11/README.md` & `metalattice-0.3.12/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # MetaLattice
+[![GitHub](https://img.shields.io/github/license/huang-lihao/metalattice)](LICENSE)
 [![PyPI - Version](https://img.shields.io/pypi/v/metalattice?logo=pypi)](https://pypi.org/project/metalattice/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/metalattice?logo=pypi)](https://pypi.org/project/metalattice/)
-[![GitHub](https://img.shields.io/github/license/huang-lihao/metalattice)](LICENSE)
 [![IJMS Paper](https://img.shields.io/badge/DOI-10.1016/j.ijmecsci.2022.107836-blue)](https://doi.org/10.1016/j.ijmecsci.2022.107836)\
 [![Upload Python Package](https://github.com/huang-lihao/MetaLattice/actions/workflows/python-publish.yml/badge.svg)](https://github.com/huang-lihao/MetaLattice/actions/workflows/python-publish.yml)
 [![Documentation Status](https://readthedocs.org/projects/metalattice/badge/?version=latest)](https://metalattice.readthedocs.io/en/latest/?badge=latest)
 
 Install
 ----------------------
 Use PyPI to install [metalattice](https://pypi.org/project/metalattice/):
```

### Comparing `metalattice-0.3.11/docs/Makefile` & `metalattice-0.3.12/docs/Makefile`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.11/docs/make.bat` & `metalattice-0.3.12/docs/make.bat`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.11/docs/source/_static/favicon.svg` & `metalattice-0.3.12/docs/source/_static/favicon.svg`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.11/docs/source/_static/logo.svg` & `metalattice-0.3.12/docs/source/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.11/pyproject.toml` & `metalattice-0.3.12/pyproject.toml`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.11/src/metalattice/logo.py` & `metalattice-0.3.12/src/metalattice/logo.py`

 * *Files identical despite different names*

### Comparing `metalattice-0.3.11/src/metalattice.egg-info/PKG-INFO` & `metalattice-0.3.12/src/metalattice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalattice
-Version: 0.3.11
+Version: 0.3.12
 Summary: A Python package to model lattice metamaterials, using Abaqus.
 Author-email: Huang Lihao <huang-lihao@outlook.com>
 Maintainer-email: Huang Lihao <huang-lihao@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 HUANG Lihao (黄立昊)
         
@@ -39,17 +39,17 @@
 Requires-Dist: gfort2py
 Requires-Dist: matplotlib
 Requires-Dist: meshio
 Requires-Dist: numpy
 Requires-Dist: sympy
 
 # MetaLattice
+[![GitHub](https://img.shields.io/github/license/huang-lihao/metalattice)](LICENSE)
 [![PyPI - Version](https://img.shields.io/pypi/v/metalattice?logo=pypi)](https://pypi.org/project/metalattice/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/metalattice?logo=pypi)](https://pypi.org/project/metalattice/)
-[![GitHub](https://img.shields.io/github/license/huang-lihao/metalattice)](LICENSE)
 [![IJMS Paper](https://img.shields.io/badge/DOI-10.1016/j.ijmecsci.2022.107836-blue)](https://doi.org/10.1016/j.ijmecsci.2022.107836)\
 [![Upload Python Package](https://github.com/huang-lihao/MetaLattice/actions/workflows/python-publish.yml/badge.svg)](https://github.com/huang-lihao/MetaLattice/actions/workflows/python-publish.yml)
 [![Documentation Status](https://readthedocs.org/projects/metalattice/badge/?version=latest)](https://metalattice.readthedocs.io/en/latest/?badge=latest)
 
 Install
 ----------------------
 Use PyPI to install [metalattice](https://pypi.org/project/metalattice/):
```

