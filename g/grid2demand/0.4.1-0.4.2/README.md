# Comparing `tmp/grid2demand-0.4.1.tar.gz` & `tmp/grid2demand-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grid2demand-0.4.1.tar", last modified: Sun Mar 31 04:02:46 2024, max compression
+gzip compressed data, was "grid2demand-0.4.2.tar", last modified: Sat Apr 20 19:14:37 2024, max compression
```

## Comparing `grid2demand-0.4.1.tar` & `grid2demand-0.4.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 04:02:46.045989 grid2demand-0.4.1/
--rw-rw-rw-   0        0        0    11558 2023-09-29 02:14:48.000000 grid2demand-0.4.1/LICENSE
--rw-rw-rw-   0        0        0     6316 2024-03-31 04:02:46.040897 grid2demand-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0    26191 2024-01-21 21:55:25.000000 grid2demand-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 04:02:45.979309 grid2demand-0.4.1/grid2demand/
--rw-rw-rw-   0        0        0      943 2024-03-31 04:01:05.000000 grid2demand-0.4.1/grid2demand/__init__.py
--rw-rw-rw-   0        0        0    27826 2024-03-31 03:45:37.000000 grid2demand-0.4.1/grid2demand/_grid2demand.py
-drwxrwxrwx   0        0        0        0 2024-03-31 04:02:46.025267 grid2demand-0.4.1/grid2demand/func_lib/
--rw-rw-rw-   0        0        0      282 2023-09-29 02:14:49.000000 grid2demand-0.4.1/grid2demand/func_lib/__init__.py
--rw-rw-rw-   0        0        0     2548 2024-03-31 02:03:11.000000 grid2demand-0.4.1/grid2demand/func_lib/gen_agent_demand.py
--rw-rw-rw-   0        0        0    16730 2024-03-31 03:37:37.000000 grid2demand-0.4.1/grid2demand/func_lib/gen_zone.py
--rw-rw-rw-   0        0        0     3818 2024-03-31 02:02:08.000000 grid2demand-0.4.1/grid2demand/func_lib/gravity_model.py
--rw-rw-rw-   0        0        0    14881 2024-03-31 02:36:02.000000 grid2demand-0.4.1/grid2demand/func_lib/read_node_poi.py
--rw-rw-rw-   0        0        0     6994 2024-03-31 03:18:02.000000 grid2demand-0.4.1/grid2demand/func_lib/trip_rate_production_attraction.py
-drwxrwxrwx   0        0        0        0 2024-03-31 04:02:46.025267 grid2demand-0.4.1/grid2demand/utils_lib/
--rw-rw-rw-   0        0        0      282 2023-09-29 02:14:49.000000 grid2demand-0.4.1/grid2demand/utils_lib/__init__.py
--rw-rw-rw-   0        0        0     6018 2024-03-27 02:20:39.000000 grid2demand-0.4.1/grid2demand/utils_lib/net_utils.py
--rw-rw-rw-   0        0        0     3348 2024-01-21 21:42:52.000000 grid2demand-0.4.1/grid2demand/utils_lib/pkg_settings.py
--rw-rw-rw-   0        0        0     9289 2024-03-27 01:31:34.000000 grid2demand-0.4.1/grid2demand/utils_lib/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-31 04:02:46.018909 grid2demand-0.4.1/grid2demand.egg-info/
--rw-rw-rw-   0        0        0     6316 2024-03-31 04:02:45.000000 grid2demand-0.4.1/grid2demand.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      653 2024-03-31 04:02:45.000000 grid2demand-0.4.1/grid2demand.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 04:02:45.000000 grid2demand-0.4.1/grid2demand.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2024-03-31 04:02:45.000000 grid2demand-0.4.1/grid2demand.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-31 04:02:45.000000 grid2demand-0.4.1/grid2demand.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-31 04:02:46.045989 grid2demand-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1997 2024-03-31 04:02:01.000000 grid2demand-0.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-31 04:02:46.040897 grid2demand-0.4.1/tests/
--rw-rw-rw-   0        0        0      552 2024-03-01 23:27:53.000000 grid2demand-0.4.1/tests/test_read_node.py
+drwxrwxrwx   0        0        0        0 2024-04-20 19:14:37.361894 grid2demand-0.4.2/
+-rw-rw-rw-   0        0        0    11558 2023-09-29 02:14:48.000000 grid2demand-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0     6317 2024-04-20 19:14:37.361894 grid2demand-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0    26191 2024-01-21 21:55:25.000000 grid2demand-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 19:14:37.303118 grid2demand-0.4.2/grid2demand/
+-rw-rw-rw-   0        0        0     1008 2024-04-20 19:13:27.000000 grid2demand-0.4.2/grid2demand/__init__.py
+-rw-rw-rw-   0        0        0    27826 2024-03-31 03:45:37.000000 grid2demand-0.4.2/grid2demand/_grid2demand.py
+drwxrwxrwx   0        0        0        0 2024-04-20 19:14:37.354932 grid2demand-0.4.2/grid2demand/func_lib/
+-rw-rw-rw-   0        0        0      282 2023-09-29 02:14:49.000000 grid2demand-0.4.2/grid2demand/func_lib/__init__.py
+-rw-rw-rw-   0        0        0     2548 2024-03-31 02:03:11.000000 grid2demand-0.4.2/grid2demand/func_lib/gen_agent_demand.py
+-rw-rw-rw-   0        0        0    16730 2024-03-31 03:37:37.000000 grid2demand-0.4.2/grid2demand/func_lib/gen_zone.py
+-rw-rw-rw-   0        0        0     3818 2024-03-31 02:02:08.000000 grid2demand-0.4.2/grid2demand/func_lib/gravity_model.py
+-rw-rw-rw-   0        0        0    14881 2024-03-31 02:36:02.000000 grid2demand-0.4.2/grid2demand/func_lib/read_node_poi.py
+-rw-rw-rw-   0        0        0     6994 2024-03-31 03:18:02.000000 grid2demand-0.4.2/grid2demand/func_lib/trip_rate_production_attraction.py
+drwxrwxrwx   0        0        0        0 2024-04-20 19:14:37.361894 grid2demand-0.4.2/grid2demand/utils_lib/
+-rw-rw-rw-   0        0        0      282 2023-09-29 02:14:49.000000 grid2demand-0.4.2/grid2demand/utils_lib/__init__.py
+-rw-rw-rw-   0        0        0     6018 2024-03-27 02:20:39.000000 grid2demand-0.4.2/grid2demand/utils_lib/net_utils.py
+-rw-rw-rw-   0        0        0     3348 2024-01-21 21:42:52.000000 grid2demand-0.4.2/grid2demand/utils_lib/pkg_settings.py
+-rw-rw-rw-   0        0        0     9289 2024-03-27 01:31:34.000000 grid2demand-0.4.2/grid2demand/utils_lib/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-20 19:14:37.342119 grid2demand-0.4.2/grid2demand.egg-info/
+-rw-rw-rw-   0        0        0     6317 2024-04-20 19:14:37.000000 grid2demand-0.4.2/grid2demand.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2024-04-20 19:14:37.000000 grid2demand-0.4.2/grid2demand.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 19:14:37.000000 grid2demand-0.4.2/grid2demand.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2024-04-20 19:14:37.000000 grid2demand-0.4.2/grid2demand.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-20 19:14:37.000000 grid2demand-0.4.2/grid2demand.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 19:14:37.369293 grid2demand-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1998 2024-04-20 19:14:01.000000 grid2demand-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 19:14:37.361894 grid2demand-0.4.2/tests/
+-rw-rw-rw-   0        0        0      552 2024-03-01 23:27:53.000000 grid2demand-0.4.2/tests/test_read_node.py
```

### Comparing `grid2demand-0.4.1/LICENSE` & `grid2demand-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.1/PKG-INFO` & `grid2demand-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: grid2demand
-Version: 0.4.1
+Version: 0.4.2
 Summary: A tool for generating zone-to-zone travel demand based on grid zones and gravity model
 Home-page: https://github.com/xyluo25/grid2demand
 Author: Xiangyong Luo, Dr.Xuesong(Simon) Zhou, Anjun Li, Entai Wang, Taehooie Kim
 Author-email: luoxiangyong01@gmail.com, xzhou74@asu.edu
 Project-URL: Homepage, https://github.com/asu-trans-ai-lab/grid2demand
 Project-URL: Documentation, https://github.com/asu-trans-ai-lab/grid2demand
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Project description
 
 GRID2DEMAND: A tool for generating zone-to-zone travel demand based on grid cells
```

### Comparing `grid2demand-0.4.1/README.md` & `grid2demand-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.1/grid2demand/__init__.py` & `grid2demand-0.4.2/grid2demand/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from .func_lib.trip_rate_production_attraction import gen_poi_trip_rate, gen_node_prod_attr
 from .func_lib.gen_zone import net2zone, sync_zone_and_node_geometry, sync_zone_and_poi_geometry, calc_zone_od_matrix
 from .func_lib.gravity_model import run_gravity_model, calc_zone_production_attraction
 from .func_lib.gen_agent_demand import gen_agent_based_demand
 from .utils_lib.pkg_settings import pkg_settings
 from ._grid2demand import GRID2DEMAND
 
-print('grid2demand, version 0.4.1')
+print('grid2demand, version 0.4.2')
+print("Python version for running the model is 3.10 or higher")
 
 
 __all__ = ["read_node", "read_poi", "read_network",
            "gen_poi_trip_rate", "gen_node_prod_attr",
            "net2zone", "sync_zone_and_node_geometry", "sync_zone_and_poi_geometry", "calc_zone_od_matrix",
            "run_gravity_model", "calc_zone_production_attraction",
            "gen_agent_based_demand",
```

### Comparing `grid2demand-0.4.1/grid2demand/_grid2demand.py` & `grid2demand-0.4.2/grid2demand/_grid2demand.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.1/grid2demand/func_lib/gen_agent_demand.py` & `grid2demand-0.4.2/grid2demand/func_lib/gen_agent_demand.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.1/grid2demand/func_lib/gen_zone.py` & `grid2demand-0.4.2/grid2demand/func_lib/gen_zone.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.1/grid2demand/func_lib/gravity_model.py` & `grid2demand-0.4.2/grid2demand/func_lib/gravity_model.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.1/grid2demand/func_lib/read_node_poi.py` & `grid2demand-0.4.2/grid2demand/func_lib/read_node_poi.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.1/grid2demand/func_lib/trip_rate_production_attraction.py` & `grid2demand-0.4.2/grid2demand/func_lib/trip_rate_production_attraction.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.1/grid2demand/utils_lib/net_utils.py` & `grid2demand-0.4.2/grid2demand/utils_lib/net_utils.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.1/grid2demand/utils_lib/pkg_settings.py` & `grid2demand-0.4.2/grid2demand/utils_lib/pkg_settings.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.1/grid2demand/utils_lib/utils.py` & `grid2demand-0.4.2/grid2demand/utils_lib/utils.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.1/grid2demand.egg-info/PKG-INFO` & `grid2demand-0.4.2/grid2demand.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: grid2demand
-Version: 0.4.1
+Version: 0.4.2
 Summary: A tool for generating zone-to-zone travel demand based on grid zones and gravity model
 Home-page: https://github.com/xyluo25/grid2demand
 Author: Xiangyong Luo, Dr.Xuesong(Simon) Zhou, Anjun Li, Entai Wang, Taehooie Kim
 Author-email: luoxiangyong01@gmail.com, xzhou74@asu.edu
 Project-URL: Homepage, https://github.com/asu-trans-ai-lab/grid2demand
 Project-URL: Documentation, https://github.com/asu-trans-ai-lab/grid2demand
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Project description
 
 GRID2DEMAND: A tool for generating zone-to-zone travel demand based on grid cells
```

### Comparing `grid2demand-0.4.1/grid2demand.egg-info/SOURCES.txt` & `grid2demand-0.4.2/grid2demand.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.1/setup.py` & `grid2demand-0.4.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,28 +16,28 @@
     with open("requirements.txt", "r", encoding="utf-8") as f:
         modules_needed = [i.strip() for i in f.readlines()]
 except Exception:
     modules_needed = []
 
 setuptools.setup(
     name="grid2demand",  # Replace with your own username
-    version="0.4.1",
+    version="0.4.2",
     author="Xiangyong Luo, Dr.Xuesong(Simon) Zhou, Anjun Li, Entai Wang, Taehooie Kim",
     author_email="luoxiangyong01@gmail.com, xzhou74@asu.edu",
     description="A tool for generating zone-to-zone travel demand based on grid zones and gravity model",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xyluo25/grid2demand",
 
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.9',
+    python_requires='>=3.10',
     install_requires=modules_needed,
 
     packages=setuptools.find_packages(),
     include_package_data=True,
     package_data={'': ['*.txt', '*.xls', '*.xlsx', '*.csv'],
                   "test_data": ['*.xls']},
     project_urls={
```

### Comparing `grid2demand-0.4.1/tests/test_read_node.py` & `grid2demand-0.4.2/tests/test_read_node.py`

 * *Files identical despite different names*

