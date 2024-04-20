# Comparing `tmp/streamlit-chip-filter-0.0.4.tar.gz` & `tmp/streamlit-chip-filter-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-chip-filter-0.0.4.tar", last modified: Sat Apr 20 17:22:28 2024, max compression
+gzip compressed data, was "streamlit-chip-filter-0.0.5.tar", last modified: Sat Apr 20 17:42:25 2024, max compression
```

## Comparing `streamlit-chip-filter-0.0.4.tar` & `streamlit-chip-filter-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 17:22:28.806005 streamlit-chip-filter-0.0.4/
--rw-rw-rw-   0        0        0     1082 2024-04-20 10:03:36.000000 streamlit-chip-filter-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       51 2024-04-20 13:23:30.000000 streamlit-chip-filter-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      177 2024-04-20 17:22:28.798436 streamlit-chip-filter-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-04-20 10:03:36.000000 streamlit-chip-filter-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 17:22:27.866816 streamlit-chip-filter-0.0.4/chip_component/
--rw-rw-rw-   0        0        0     1020 2024-04-20 16:58:49.000000 streamlit-chip-filter-0.0.4/chip_component/__init__.py
--rw-rw-rw-   0        0        0      677 2024-04-20 16:58:58.000000 streamlit-chip-filter-0.0.4/chip_component/example.py
-drwxrwxrwx   0        0        0        0 2024-04-20 17:22:27.636065 streamlit-chip-filter-0.0.4/chip_component/frontend/
-drwxrwxrwx   0        0        0        0 2024-04-20 17:22:28.137736 streamlit-chip-filter-0.0.4/chip_component/frontend/build/
--rw-rw-rw-   0        0        0      374 2024-04-20 17:06:50.000000 streamlit-chip-filter-0.0.4/chip_component/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2024-04-20 10:03:36.000000 streamlit-chip-filter-0.0.4/chip_component/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0   589892 2024-03-23 11:30:35.000000 streamlit-chip-filter-0.0.4/chip_component/frontend/build/bootstrap.min.css.map
--rw-rw-rw-   0        0        0      682 2024-04-20 17:06:50.000000 streamlit-chip-filter-0.0.4/chip_component/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2024-04-20 17:22:27.737039 streamlit-chip-filter-0.0.4/chip_component/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2024-04-20 17:22:28.199141 streamlit-chip-filter-0.0.4/chip_component/frontend/build/static/css/
--rw-rw-rw-   0        0        0      684 2024-04-20 17:06:50.000000 streamlit-chip-filter-0.0.4/chip_component/frontend/build/static/css/main.c5d93354.css
--rw-rw-rw-   0        0        0     1610 2024-04-20 17:06:50.000000 streamlit-chip-filter-0.0.4/chip_component/frontend/build/static/css/main.c5d93354.css.map
-drwxrwxrwx   0        0        0        0 2024-04-20 17:22:28.596665 streamlit-chip-filter-0.0.4/chip_component/frontend/build/static/js/
--rw-rw-rw-   0        0        0   342662 2024-04-20 17:06:50.000000 streamlit-chip-filter-0.0.4/chip_component/frontend/build/static/js/main.301d0b88.js
--rw-rw-rw-   0        0        0     1293 2024-04-20 17:06:50.000000 streamlit-chip-filter-0.0.4/chip_component/frontend/build/static/js/main.301d0b88.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1370254 2024-04-20 17:06:50.000000 streamlit-chip-filter-0.0.4/chip_component/frontend/build/static/js/main.301d0b88.js.map
--rw-rw-rw-   0        0        0     1801 2024-04-20 13:35:47.000000 streamlit-chip-filter-0.0.4/chip_component/streamlit_callback.py
--rw-rw-rw-   0        0        0       42 2024-04-20 17:22:28.806005 streamlit-chip-filter-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1058 2024-04-20 17:04:17.000000 streamlit-chip-filter-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 17:22:28.795822 streamlit-chip-filter-0.0.4/streamlit_chip_filter.egg-info/
--rw-rw-rw-   0        0        0      177 2024-04-20 17:22:26.000000 streamlit-chip-filter-0.0.4/streamlit_chip_filter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      852 2024-04-20 17:22:27.000000 streamlit-chip-filter-0.0.4/streamlit_chip_filter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 17:22:26.000000 streamlit-chip-filter-0.0.4/streamlit_chip_filter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-04-20 17:22:26.000000 streamlit-chip-filter-0.0.4/streamlit_chip_filter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-20 17:22:26.000000 streamlit-chip-filter-0.0.4/streamlit_chip_filter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 17:42:25.054345 streamlit-chip-filter-0.0.5/
+-rw-rw-rw-   0        0        0     1082 2024-04-20 10:03:36.000000 streamlit-chip-filter-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       51 2024-04-20 13:23:30.000000 streamlit-chip-filter-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      177 2024-04-20 17:42:24.934350 streamlit-chip-filter-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-04-20 10:03:36.000000 streamlit-chip-filter-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 17:42:24.054042 streamlit-chip-filter-0.0.5/chip_component/
+-rw-rw-rw-   0        0        0     1019 2024-04-20 17:41:52.000000 streamlit-chip-filter-0.0.5/chip_component/__init__.py
+-rw-rw-rw-   0        0        0      677 2024-04-20 16:58:58.000000 streamlit-chip-filter-0.0.5/chip_component/example.py
+drwxrwxrwx   0        0        0        0 2024-04-20 17:42:23.799908 streamlit-chip-filter-0.0.5/chip_component/frontend/
+drwxrwxrwx   0        0        0        0 2024-04-20 17:42:24.287047 streamlit-chip-filter-0.0.5/chip_component/frontend/build/
+-rw-rw-rw-   0        0        0      374 2024-04-20 17:06:50.000000 streamlit-chip-filter-0.0.5/chip_component/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2024-04-20 10:03:36.000000 streamlit-chip-filter-0.0.5/chip_component/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0   589892 2024-03-23 11:30:35.000000 streamlit-chip-filter-0.0.5/chip_component/frontend/build/bootstrap.min.css.map
+-rw-rw-rw-   0        0        0      682 2024-04-20 17:06:50.000000 streamlit-chip-filter-0.0.5/chip_component/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2024-04-20 17:42:23.879905 streamlit-chip-filter-0.0.5/chip_component/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2024-04-20 17:42:24.400049 streamlit-chip-filter-0.0.5/chip_component/frontend/build/static/css/
+-rw-rw-rw-   0        0        0      684 2024-04-20 17:06:50.000000 streamlit-chip-filter-0.0.5/chip_component/frontend/build/static/css/main.c5d93354.css
+-rw-rw-rw-   0        0        0     1610 2024-04-20 17:06:50.000000 streamlit-chip-filter-0.0.5/chip_component/frontend/build/static/css/main.c5d93354.css.map
+drwxrwxrwx   0        0        0        0 2024-04-20 17:42:24.619050 streamlit-chip-filter-0.0.5/chip_component/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   342662 2024-04-20 17:06:50.000000 streamlit-chip-filter-0.0.5/chip_component/frontend/build/static/js/main.301d0b88.js
+-rw-rw-rw-   0        0        0     1293 2024-04-20 17:06:50.000000 streamlit-chip-filter-0.0.5/chip_component/frontend/build/static/js/main.301d0b88.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1370254 2024-04-20 17:06:50.000000 streamlit-chip-filter-0.0.5/chip_component/frontend/build/static/js/main.301d0b88.js.map
+-rw-rw-rw-   0        0        0     1801 2024-04-20 13:35:47.000000 streamlit-chip-filter-0.0.5/chip_component/streamlit_callback.py
+-rw-rw-rw-   0        0        0       42 2024-04-20 17:42:25.068358 streamlit-chip-filter-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1058 2024-04-20 17:42:07.000000 streamlit-chip-filter-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 17:42:24.922348 streamlit-chip-filter-0.0.5/streamlit_chip_filter.egg-info/
+-rw-rw-rw-   0        0        0      177 2024-04-20 17:42:22.000000 streamlit-chip-filter-0.0.5/streamlit_chip_filter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      852 2024-04-20 17:42:23.000000 streamlit-chip-filter-0.0.5/streamlit_chip_filter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 17:42:22.000000 streamlit-chip-filter-0.0.5/streamlit_chip_filter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-04-20 17:42:22.000000 streamlit-chip-filter-0.0.5/streamlit_chip_filter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-20 17:42:22.000000 streamlit-chip-filter-0.0.5/streamlit_chip_filter.egg-info/top_level.txt
```

### Comparing `streamlit-chip-filter-0.0.4/LICENSE` & `streamlit-chip-filter-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.4/chip_component/__init__.py` & `streamlit-chip-filter-0.0.5/chip_component/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import streamlit as st
 import streamlit.components.v1 as components
 from chip_component.streamlit_callback import register 
 
-_RELEASE = False 
+_RELEASE = True 
 
 if not _RELEASE:
     _chip_filter= components.declare_component(
         
         "chip_filter",
 
         url="http://localhost:3001",
```

### Comparing `streamlit-chip-filter-0.0.4/chip_component/example.py` & `streamlit-chip-filter-0.0.5/chip_component/example.py`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.4/chip_component/frontend/build/bootstrap.min.css` & `streamlit-chip-filter-0.0.5/chip_component/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.4/chip_component/frontend/build/bootstrap.min.css.map` & `streamlit-chip-filter-0.0.5/chip_component/frontend/build/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.4/chip_component/frontend/build/index.html` & `streamlit-chip-filter-0.0.5/chip_component/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.4/chip_component/frontend/build/static/css/main.c5d93354.css` & `streamlit-chip-filter-0.0.5/chip_component/frontend/build/static/css/main.c5d93354.css`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.4/chip_component/frontend/build/static/css/main.c5d93354.css.map` & `streamlit-chip-filter-0.0.5/chip_component/frontend/build/static/css/main.c5d93354.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.4/chip_component/frontend/build/static/js/main.301d0b88.js` & `streamlit-chip-filter-0.0.5/chip_component/frontend/build/static/js/main.301d0b88.js`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.4/chip_component/frontend/build/static/js/main.301d0b88.js.LICENSE.txt` & `streamlit-chip-filter-0.0.5/chip_component/frontend/build/static/js/main.301d0b88.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.4/chip_component/frontend/build/static/js/main.301d0b88.js.map` & `streamlit-chip-filter-0.0.5/chip_component/frontend/build/static/js/main.301d0b88.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.4/chip_component/streamlit_callback.py` & `streamlit-chip-filter-0.0.5/chip_component/streamlit_callback.py`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.4/setup.py` & `streamlit-chip-filter-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-chip-filter",
-    version="0.0.4",
+    version="0.0.5",
     author="",
     author_email="",
     # description="Streamlit component that allows you to do X",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-chip-filter-0.0.4/streamlit_chip_filter.egg-info/SOURCES.txt` & `streamlit-chip-filter-0.0.5/streamlit_chip_filter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

