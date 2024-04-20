# Comparing `tmp/streamlit-chip-filter-0.0.1.tar.gz` & `tmp/streamlit-chip-filter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-chip-filter-0.0.1.tar", last modified: Sat Apr 20 13:28:15 2024, max compression
+gzip compressed data, was "streamlit-chip-filter-0.0.2.tar", last modified: Sat Apr 20 13:42:22 2024, max compression
```

## Comparing `streamlit-chip-filter-0.0.1.tar` & `streamlit-chip-filter-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 13:28:15.406234 streamlit-chip-filter-0.0.1/
--rw-rw-rw-   0        0        0     1082 2024-04-20 10:03:36.000000 streamlit-chip-filter-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       51 2024-04-20 13:23:30.000000 streamlit-chip-filter-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      177 2024-04-20 13:28:15.399055 streamlit-chip-filter-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-04-20 10:03:36.000000 streamlit-chip-filter-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 13:28:13.874627 streamlit-chip-filter-0.0.1/chip_component/
--rw-rw-rw-   0        0        0      641 2024-04-20 13:28:08.000000 streamlit-chip-filter-0.0.1/chip_component/__init__.py
--rw-rw-rw-   0        0        0      573 2024-04-20 13:20:50.000000 streamlit-chip-filter-0.0.1/chip_component/example.py
-drwxrwxrwx   0        0        0        0 2024-04-20 13:28:13.713593 streamlit-chip-filter-0.0.1/chip_component/frontend/
-drwxrwxrwx   0        0        0        0 2024-04-20 13:28:14.164639 streamlit-chip-filter-0.0.1/chip_component/frontend/build/
--rw-rw-rw-   0        0        0      374 2024-04-20 13:26:01.000000 streamlit-chip-filter-0.0.1/chip_component/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2024-04-20 10:03:36.000000 streamlit-chip-filter-0.0.1/chip_component/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0   589892 2024-03-23 11:30:35.000000 streamlit-chip-filter-0.0.1/chip_component/frontend/build/bootstrap.min.css.map
--rw-rw-rw-   0        0        0      682 2024-04-20 13:26:01.000000 streamlit-chip-filter-0.0.1/chip_component/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2024-04-20 13:28:13.724159 streamlit-chip-filter-0.0.1/chip_component/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2024-04-20 13:28:14.236354 streamlit-chip-filter-0.0.1/chip_component/frontend/build/static/css/
--rw-rw-rw-   0        0        0      684 2024-04-20 13:26:01.000000 streamlit-chip-filter-0.0.1/chip_component/frontend/build/static/css/main.c5d93354.css
--rw-rw-rw-   0        0        0     1610 2024-04-20 13:26:01.000000 streamlit-chip-filter-0.0.1/chip_component/frontend/build/static/css/main.c5d93354.css.map
-drwxrwxrwx   0        0        0        0 2024-04-20 13:28:14.764978 streamlit-chip-filter-0.0.1/chip_component/frontend/build/static/js/
--rw-rw-rw-   0        0        0   342644 2024-04-20 13:26:01.000000 streamlit-chip-filter-0.0.1/chip_component/frontend/build/static/js/main.b89b78b8.js
--rw-rw-rw-   0        0        0     1293 2024-04-20 13:26:01.000000 streamlit-chip-filter-0.0.1/chip_component/frontend/build/static/js/main.b89b78b8.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1370055 2024-04-20 13:26:01.000000 streamlit-chip-filter-0.0.1/chip_component/frontend/build/static/js/main.b89b78b8.js.map
--rw-rw-rw-   0        0        0       42 2024-04-20 13:28:15.406234 streamlit-chip-filter-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1058 2024-04-20 13:24:07.000000 streamlit-chip-filter-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 13:28:15.390977 streamlit-chip-filter-0.0.1/streamlit_chip_filter.egg-info/
--rw-rw-rw-   0        0        0      177 2024-04-20 13:28:12.000000 streamlit-chip-filter-0.0.1/streamlit_chip_filter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      815 2024-04-20 13:28:13.000000 streamlit-chip-filter-0.0.1/streamlit_chip_filter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 13:28:12.000000 streamlit-chip-filter-0.0.1/streamlit_chip_filter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-04-20 13:28:12.000000 streamlit-chip-filter-0.0.1/streamlit_chip_filter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-20 13:28:12.000000 streamlit-chip-filter-0.0.1/streamlit_chip_filter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 13:42:22.515206 streamlit-chip-filter-0.0.2/
+-rw-rw-rw-   0        0        0     1082 2024-04-20 10:03:36.000000 streamlit-chip-filter-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       51 2024-04-20 13:23:30.000000 streamlit-chip-filter-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      177 2024-04-20 13:42:22.512207 streamlit-chip-filter-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-04-20 10:03:36.000000 streamlit-chip-filter-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 13:42:21.943143 streamlit-chip-filter-0.0.2/chip_component/
+-rw-rw-rw-   0        0        0     1019 2024-04-20 13:40:29.000000 streamlit-chip-filter-0.0.2/chip_component/__init__.py
+-rw-rw-rw-   0        0        0      571 2024-04-20 13:31:00.000000 streamlit-chip-filter-0.0.2/chip_component/example.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:42:21.732143 streamlit-chip-filter-0.0.2/chip_component/frontend/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:42:22.024169 streamlit-chip-filter-0.0.2/chip_component/frontend/build/
+-rw-rw-rw-   0        0        0      374 2024-04-20 13:26:01.000000 streamlit-chip-filter-0.0.2/chip_component/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2024-04-20 10:03:36.000000 streamlit-chip-filter-0.0.2/chip_component/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0   589892 2024-03-23 11:30:35.000000 streamlit-chip-filter-0.0.2/chip_component/frontend/build/bootstrap.min.css.map
+-rw-rw-rw-   0        0        0      682 2024-04-20 13:26:01.000000 streamlit-chip-filter-0.0.2/chip_component/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:42:21.740142 streamlit-chip-filter-0.0.2/chip_component/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:42:22.095145 streamlit-chip-filter-0.0.2/chip_component/frontend/build/static/css/
+-rw-rw-rw-   0        0        0      684 2024-04-20 13:26:01.000000 streamlit-chip-filter-0.0.2/chip_component/frontend/build/static/css/main.c5d93354.css
+-rw-rw-rw-   0        0        0     1610 2024-04-20 13:26:01.000000 streamlit-chip-filter-0.0.2/chip_component/frontend/build/static/css/main.c5d93354.css.map
+drwxrwxrwx   0        0        0        0 2024-04-20 13:42:22.155148 streamlit-chip-filter-0.0.2/chip_component/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   342644 2024-04-20 13:26:01.000000 streamlit-chip-filter-0.0.2/chip_component/frontend/build/static/js/main.b89b78b8.js
+-rw-rw-rw-   0        0        0     1293 2024-04-20 13:26:01.000000 streamlit-chip-filter-0.0.2/chip_component/frontend/build/static/js/main.b89b78b8.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1370055 2024-04-20 13:26:01.000000 streamlit-chip-filter-0.0.2/chip_component/frontend/build/static/js/main.b89b78b8.js.map
+-rw-rw-rw-   0        0        0     1801 2024-04-20 13:35:47.000000 streamlit-chip-filter-0.0.2/chip_component/streamlit_callback.py
+-rw-rw-rw-   0        0        0       42 2024-04-20 13:42:22.516210 streamlit-chip-filter-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1058 2024-04-20 13:40:31.000000 streamlit-chip-filter-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:42:22.507207 streamlit-chip-filter-0.0.2/streamlit_chip_filter.egg-info/
+-rw-rw-rw-   0        0        0      177 2024-04-20 13:42:18.000000 streamlit-chip-filter-0.0.2/streamlit_chip_filter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      852 2024-04-20 13:42:20.000000 streamlit-chip-filter-0.0.2/streamlit_chip_filter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 13:42:18.000000 streamlit-chip-filter-0.0.2/streamlit_chip_filter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-04-20 13:42:18.000000 streamlit-chip-filter-0.0.2/streamlit_chip_filter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-20 13:42:18.000000 streamlit-chip-filter-0.0.2/streamlit_chip_filter.egg-info/top_level.txt
```

### Comparing `streamlit-chip-filter-0.0.1/LICENSE` & `streamlit-chip-filter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.1/chip_component/frontend/build/bootstrap.min.css` & `streamlit-chip-filter-0.0.2/chip_component/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.1/chip_component/frontend/build/bootstrap.min.css.map` & `streamlit-chip-filter-0.0.2/chip_component/frontend/build/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.1/chip_component/frontend/build/index.html` & `streamlit-chip-filter-0.0.2/chip_component/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.1/chip_component/frontend/build/static/css/main.c5d93354.css` & `streamlit-chip-filter-0.0.2/chip_component/frontend/build/static/css/main.c5d93354.css`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.1/chip_component/frontend/build/static/css/main.c5d93354.css.map` & `streamlit-chip-filter-0.0.2/chip_component/frontend/build/static/css/main.c5d93354.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.1/chip_component/frontend/build/static/js/main.b89b78b8.js` & `streamlit-chip-filter-0.0.2/chip_component/frontend/build/static/js/main.b89b78b8.js`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.1/chip_component/frontend/build/static/js/main.b89b78b8.js.LICENSE.txt` & `streamlit-chip-filter-0.0.2/chip_component/frontend/build/static/js/main.b89b78b8.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.1/chip_component/frontend/build/static/js/main.b89b78b8.js.map` & `streamlit-chip-filter-0.0.2/chip_component/frontend/build/static/js/main.b89b78b8.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.1/setup.py` & `streamlit-chip-filter-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-chip-filter",
-    version="0.0.1",
+    version="0.0.2",
     author="",
     author_email="",
     # description="Streamlit component that allows you to do X",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-chip-filter-0.0.1/streamlit_chip_filter.egg-info/SOURCES.txt` & `streamlit-chip-filter-0.0.2/streamlit_chip_filter.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 chip_component/__init__.py
 chip_component/example.py
+chip_component/streamlit_callback.py
 chip_component/frontend/build/asset-manifest.json
 chip_component/frontend/build/bootstrap.min.css
 chip_component/frontend/build/bootstrap.min.css.map
 chip_component/frontend/build/index.html
 chip_component/frontend/build/static/css/main.c5d93354.css
 chip_component/frontend/build/static/css/main.c5d93354.css.map
 chip_component/frontend/build/static/js/main.b89b78b8.js
```

