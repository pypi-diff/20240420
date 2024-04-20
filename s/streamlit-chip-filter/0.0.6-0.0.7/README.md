# Comparing `tmp/streamlit-chip-filter-0.0.6.tar.gz` & `tmp/streamlit-chip-filter-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-chip-filter-0.0.6.tar", last modified: Sat Apr 20 18:38:22 2024, max compression
+gzip compressed data, was "streamlit-chip-filter-0.0.7.tar", last modified: Sat Apr 20 18:47:56 2024, max compression
```

## Comparing `streamlit-chip-filter-0.0.6.tar` & `streamlit-chip-filter-0.0.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 18:38:22.513235 streamlit-chip-filter-0.0.6/
--rw-rw-rw-   0        0        0     1082 2024-04-20 10:03:36.000000 streamlit-chip-filter-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       51 2024-04-20 13:23:30.000000 streamlit-chip-filter-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      177 2024-04-20 18:38:22.509228 streamlit-chip-filter-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-04-20 10:03:36.000000 streamlit-chip-filter-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 18:38:21.290716 streamlit-chip-filter-0.0.6/chip_component/
--rw-rw-rw-   0        0        0     1019 2024-04-20 17:41:52.000000 streamlit-chip-filter-0.0.6/chip_component/__init__.py
--rw-rw-rw-   0        0        0      677 2024-04-20 16:58:58.000000 streamlit-chip-filter-0.0.6/chip_component/example.py
-drwxrwxrwx   0        0        0        0 2024-04-20 18:38:21.100714 streamlit-chip-filter-0.0.6/chip_component/frontend/
-drwxrwxrwx   0        0        0        0 2024-04-20 18:38:21.704504 streamlit-chip-filter-0.0.6/chip_component/frontend/build/
--rw-rw-rw-   0        0        0      374 2024-04-20 18:33:52.000000 streamlit-chip-filter-0.0.6/chip_component/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2024-04-20 10:03:36.000000 streamlit-chip-filter-0.0.6/chip_component/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0   589892 2024-03-23 11:30:35.000000 streamlit-chip-filter-0.0.6/chip_component/frontend/build/bootstrap.min.css.map
--rw-rw-rw-   0        0        0      682 2024-04-20 18:33:52.000000 streamlit-chip-filter-0.0.6/chip_component/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2024-04-20 18:38:21.119708 streamlit-chip-filter-0.0.6/chip_component/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2024-04-20 18:38:21.776499 streamlit-chip-filter-0.0.6/chip_component/frontend/build/static/css/
--rw-rw-rw-   0        0        0      735 2024-04-20 18:33:52.000000 streamlit-chip-filter-0.0.6/chip_component/frontend/build/static/css/main.6fb9e305.css
--rw-rw-rw-   0        0        0     1720 2024-04-20 18:33:52.000000 streamlit-chip-filter-0.0.6/chip_component/frontend/build/static/css/main.6fb9e305.css.map
-drwxrwxrwx   0        0        0        0 2024-04-20 18:38:22.323179 streamlit-chip-filter-0.0.6/chip_component/frontend/build/static/js/
--rw-rw-rw-   0        0        0   342790 2024-04-20 18:33:52.000000 streamlit-chip-filter-0.0.6/chip_component/frontend/build/static/js/main.8eda4e37.js
--rw-rw-rw-   0        0        0     1293 2024-04-20 18:33:52.000000 streamlit-chip-filter-0.0.6/chip_component/frontend/build/static/js/main.8eda4e37.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1370784 2024-04-20 18:33:52.000000 streamlit-chip-filter-0.0.6/chip_component/frontend/build/static/js/main.8eda4e37.js.map
--rw-rw-rw-   0        0        0     1801 2024-04-20 13:35:47.000000 streamlit-chip-filter-0.0.6/chip_component/streamlit_callback.py
--rw-rw-rw-   0        0        0       42 2024-04-20 18:38:22.513235 streamlit-chip-filter-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1058 2024-04-20 18:30:20.000000 streamlit-chip-filter-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 18:38:22.502245 streamlit-chip-filter-0.0.6/streamlit_chip_filter.egg-info/
--rw-rw-rw-   0        0        0      177 2024-04-20 18:38:18.000000 streamlit-chip-filter-0.0.6/streamlit_chip_filter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      852 2024-04-20 18:38:20.000000 streamlit-chip-filter-0.0.6/streamlit_chip_filter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 18:38:18.000000 streamlit-chip-filter-0.0.6/streamlit_chip_filter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-04-20 18:38:18.000000 streamlit-chip-filter-0.0.6/streamlit_chip_filter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-20 18:38:18.000000 streamlit-chip-filter-0.0.6/streamlit_chip_filter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 18:47:56.139614 streamlit-chip-filter-0.0.7/
+-rw-rw-rw-   0        0        0     1082 2024-04-20 10:03:36.000000 streamlit-chip-filter-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0       51 2024-04-20 13:23:30.000000 streamlit-chip-filter-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      177 2024-04-20 18:47:56.135616 streamlit-chip-filter-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-04-20 10:03:36.000000 streamlit-chip-filter-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 18:47:55.824565 streamlit-chip-filter-0.0.7/chip_component/
+-rw-rw-rw-   0        0        0     1075 2024-04-20 18:46:33.000000 streamlit-chip-filter-0.0.7/chip_component/__init__.py
+-rw-rw-rw-   0        0        0      677 2024-04-20 16:58:58.000000 streamlit-chip-filter-0.0.7/chip_component/example.py
+drwxrwxrwx   0        0        0        0 2024-04-20 18:47:55.612277 streamlit-chip-filter-0.0.7/chip_component/frontend/
+drwxrwxrwx   0        0        0        0 2024-04-20 18:47:55.888565 streamlit-chip-filter-0.0.7/chip_component/frontend/build/
+-rw-rw-rw-   0        0        0      374 2024-04-20 18:33:52.000000 streamlit-chip-filter-0.0.7/chip_component/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2024-04-20 10:03:36.000000 streamlit-chip-filter-0.0.7/chip_component/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0   589892 2024-03-23 11:30:35.000000 streamlit-chip-filter-0.0.7/chip_component/frontend/build/bootstrap.min.css.map
+-rw-rw-rw-   0        0        0      682 2024-04-20 18:33:52.000000 streamlit-chip-filter-0.0.7/chip_component/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2024-04-20 18:47:55.726563 streamlit-chip-filter-0.0.7/chip_component/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2024-04-20 18:47:55.938703 streamlit-chip-filter-0.0.7/chip_component/frontend/build/static/css/
+-rw-rw-rw-   0        0        0      735 2024-04-20 18:33:52.000000 streamlit-chip-filter-0.0.7/chip_component/frontend/build/static/css/main.6fb9e305.css
+-rw-rw-rw-   0        0        0     1720 2024-04-20 18:33:52.000000 streamlit-chip-filter-0.0.7/chip_component/frontend/build/static/css/main.6fb9e305.css.map
+drwxrwxrwx   0        0        0        0 2024-04-20 18:47:55.995617 streamlit-chip-filter-0.0.7/chip_component/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   342790 2024-04-20 18:33:52.000000 streamlit-chip-filter-0.0.7/chip_component/frontend/build/static/js/main.8eda4e37.js
+-rw-rw-rw-   0        0        0     1293 2024-04-20 18:33:52.000000 streamlit-chip-filter-0.0.7/chip_component/frontend/build/static/js/main.8eda4e37.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1370784 2024-04-20 18:33:52.000000 streamlit-chip-filter-0.0.7/chip_component/frontend/build/static/js/main.8eda4e37.js.map
+-rw-rw-rw-   0        0        0     1801 2024-04-20 13:35:47.000000 streamlit-chip-filter-0.0.7/chip_component/streamlit_callback.py
+-rw-rw-rw-   0        0        0       42 2024-04-20 18:47:56.140612 streamlit-chip-filter-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1058 2024-04-20 18:47:09.000000 streamlit-chip-filter-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 18:47:56.124617 streamlit-chip-filter-0.0.7/streamlit_chip_filter.egg-info/
+-rw-rw-rw-   0        0        0      177 2024-04-20 18:47:51.000000 streamlit-chip-filter-0.0.7/streamlit_chip_filter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      852 2024-04-20 18:47:54.000000 streamlit-chip-filter-0.0.7/streamlit_chip_filter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 18:47:51.000000 streamlit-chip-filter-0.0.7/streamlit_chip_filter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-04-20 18:47:51.000000 streamlit-chip-filter-0.0.7/streamlit_chip_filter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-20 18:47:51.000000 streamlit-chip-filter-0.0.7/streamlit_chip_filter.egg-info/top_level.txt
```

### Comparing `streamlit-chip-filter-0.0.6/LICENSE` & `streamlit-chip-filter-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.6/chip_component/__init__.py` & `streamlit-chip-filter-0.0.7/chip_component/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,18 +14,18 @@
     )
 else:
 
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/build")
     _chip_filter = components.declare_component("chip_filter", path=build_dir)
 
-def chip_filter(chipData=None, styles=None, key=None, on_change=None, args=None, kwargs=None, default=None):
+def chip_filter(chipData=None, disabledOptions=False, styles=None, key=None, on_change=None, args=None, kwargs=None, default=None):
 
     if on_change is not None:
         if key is None:
             st.error("You must pass a key if you want to use the on_change callback for the chip filter")
         else:
             register(key=key, callback=on_change, args=args, kwargs=kwargs)
     
-    component_value = _chip_filter(chipData=chipData, styles=styles, key=key, default=default)
+    component_value = _chip_filter(chipData=chipData, disabledOptions=disabledOptions, styles=styles, key=key, default=default)
 
     return component_value
```

### Comparing `streamlit-chip-filter-0.0.6/chip_component/example.py` & `streamlit-chip-filter-0.0.7/chip_component/example.py`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.6/chip_component/frontend/build/bootstrap.min.css` & `streamlit-chip-filter-0.0.7/chip_component/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.6/chip_component/frontend/build/bootstrap.min.css.map` & `streamlit-chip-filter-0.0.7/chip_component/frontend/build/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.6/chip_component/frontend/build/index.html` & `streamlit-chip-filter-0.0.7/chip_component/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.6/chip_component/frontend/build/static/css/main.6fb9e305.css` & `streamlit-chip-filter-0.0.7/chip_component/frontend/build/static/css/main.6fb9e305.css`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.6/chip_component/frontend/build/static/css/main.6fb9e305.css.map` & `streamlit-chip-filter-0.0.7/chip_component/frontend/build/static/css/main.6fb9e305.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.6/chip_component/frontend/build/static/js/main.8eda4e37.js` & `streamlit-chip-filter-0.0.7/chip_component/frontend/build/static/js/main.8eda4e37.js`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.6/chip_component/frontend/build/static/js/main.8eda4e37.js.LICENSE.txt` & `streamlit-chip-filter-0.0.7/chip_component/frontend/build/static/js/main.8eda4e37.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.6/chip_component/frontend/build/static/js/main.8eda4e37.js.map` & `streamlit-chip-filter-0.0.7/chip_component/frontend/build/static/js/main.8eda4e37.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.6/chip_component/streamlit_callback.py` & `streamlit-chip-filter-0.0.7/chip_component/streamlit_callback.py`

 * *Files identical despite different names*

### Comparing `streamlit-chip-filter-0.0.6/setup.py` & `streamlit-chip-filter-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-chip-filter",
-    version="0.0.6",
+    version="0.0.7",
     author="",
     author_email="",
     # description="Streamlit component that allows you to do X",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-chip-filter-0.0.6/streamlit_chip_filter.egg-info/SOURCES.txt` & `streamlit-chip-filter-0.0.7/streamlit_chip_filter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

