# Comparing `tmp/etudatasphere-0.1.2.tar.gz` & `tmp/etudatasphere-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etudatasphere-0.1.2.tar", last modified: Sat Apr  6 10:08:10 2024, max compression
+gzip compressed data, was "etudatasphere-0.1.3.tar", last modified: Sat Apr 20 10:53:14 2024, max compression
```

## Comparing `etudatasphere-0.1.2.tar` & `etudatasphere-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 10:08:10.762958 etudatasphere-0.1.2/
--rw-rw-rw-   0        0        0     1110 2024-03-27 19:34:50.000000 etudatasphere-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     5803 2024-04-06 10:08:10.762958 etudatasphere-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4765 2024-04-06 10:07:41.000000 etudatasphere-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 10:08:10.747349 etudatasphere-0.1.2/etudatasphere/
--rw-rw-rw-   0        0        0     7745 2024-04-06 09:34:48.000000 etudatasphere-0.1.2/etudatasphere/DataSphereManager.py
--rw-rw-rw-   0        0        0       50 2024-04-02 17:06:36.000000 etudatasphere-0.1.2/etudatasphere/__init__.py
--rw-rw-rw-   0        0        0     1299 2024-04-05 20:14:18.000000 etudatasphere-0.1.2/etudatasphere/exceptions.py
--rw-rw-rw-   0        0        0     2088 2024-04-06 09:17:14.000000 etudatasphere-0.1.2/etudatasphere/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-06 10:08:10.762958 etudatasphere-0.1.2/etudatasphere.egg-info/
--rw-rw-rw-   0        0        0     5803 2024-04-06 10:08:10.000000 etudatasphere-0.1.2/etudatasphere.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2024-04-06 10:08:10.000000 etudatasphere-0.1.2/etudatasphere.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 10:08:10.000000 etudatasphere-0.1.2/etudatasphere.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-04-06 10:08:10.000000 etudatasphere-0.1.2/etudatasphere.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-06 10:08:10.000000 etudatasphere-0.1.2/etudatasphere.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 10:08:10.762958 etudatasphere-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1432 2024-04-06 10:02:35.000000 etudatasphere-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 10:08:10.762958 etudatasphere-0.1.2/tests/
--rw-rw-rw-   0        0        0     1616 2024-04-06 10:01:22.000000 etudatasphere-0.1.2/tests/test_etudatasphere.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:53:14.631583 etudatasphere-0.1.3/
+-rw-rw-rw-   0        0        0     1110 2024-03-27 19:34:50.000000 etudatasphere-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     5796 2024-04-20 10:53:14.631583 etudatasphere-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4758 2024-04-14 09:46:37.000000 etudatasphere-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 10:53:14.585731 etudatasphere-0.1.3/etudatasphere/
+-rw-rw-rw-   0        0        0    11158 2024-04-19 19:03:16.000000 etudatasphere-0.1.3/etudatasphere/DataSphereManager.py
+-rw-rw-rw-   0        0        0      746 2024-04-19 21:08:33.000000 etudatasphere-0.1.3/etudatasphere/OperationManager.py
+-rw-rw-rw-   0        0        0       98 2024-04-19 19:02:15.000000 etudatasphere-0.1.3/etudatasphere/__init__.py
+-rw-rw-rw-   0        0        0     1866 2024-04-17 15:55:36.000000 etudatasphere-0.1.3/etudatasphere/exceptions.py
+-rw-rw-rw-   0        0        0     2127 2024-04-19 18:36:50.000000 etudatasphere-0.1.3/etudatasphere/requests.py
+-rw-rw-rw-   0        0        0     3190 2024-04-19 18:36:50.000000 etudatasphere-0.1.3/etudatasphere/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:53:14.626034 etudatasphere-0.1.3/etudatasphere.egg-info/
+-rw-rw-rw-   0        0        0     5796 2024-04-20 10:53:14.000000 etudatasphere-0.1.3/etudatasphere.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2024-04-20 10:53:14.000000 etudatasphere-0.1.3/etudatasphere.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 10:53:14.000000 etudatasphere-0.1.3/etudatasphere.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-04-20 10:53:14.000000 etudatasphere-0.1.3/etudatasphere.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-20 10:53:14.000000 etudatasphere-0.1.3/etudatasphere.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 10:53:14.631583 etudatasphere-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1432 2024-04-20 10:52:53.000000 etudatasphere-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:53:14.626034 etudatasphere-0.1.3/tests/
+-rw-rw-rw-   0        0        0     1724 2024-04-19 18:40:43.000000 etudatasphere-0.1.3/tests/test_etudatasphere.py
```

### Comparing `etudatasphere-0.1.2/LICENSE` & `etudatasphere-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `etudatasphere-0.1.2/PKG-INFO` & `etudatasphere-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etudatasphere
-Version: 0.1.2
+Version: 0.1.3
 Summary: etudatasphere: Simplifying Cloud Administration. Access Yandex.Cloud services with ease, automating routine tasks for resource management.
 Home-page: https://github.com/sesh00/etudatasphere
 Download-URL: https://github.com/sesh00/etudatasphere/archive/main.zip
 Author: sesh00
 Author-email: ernestrsage@gmail.com
 License: MIT License, see LICENSE file
 Classifier: Operating System :: OS Independent
@@ -29,15 +29,15 @@
 This is a Python library for interacting with Yandex DataSphere API. It provides functions to perform various operations such as getting organizations, billing accounts, projects, managing organization members, creating projects, checking operation status, and adding contributors to projects.
 
 ## Installation
 
 Install the current version with [PyPI](https://pypi.org/project/etudatasphere):
 
 ```bash
-pip install etudatasphere==0.1.1
+pip install etudatasphere
 ```
 
 Or from GitHub:
 ```bash
 pip install https://github.com/sesh00/etudatasphere/archive/main.zip
 ```
 ## Usage
```

### Comparing `etudatasphere-0.1.2/README.md` & `etudatasphere-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 This is a Python library for interacting with Yandex DataSphere API. It provides functions to perform various operations such as getting organizations, billing accounts, projects, managing organization members, creating projects, checking operation status, and adding contributors to projects.
 
 ## Installation
 
 Install the current version with [PyPI](https://pypi.org/project/etudatasphere):
 
 ```bash
-pip install etudatasphere==0.1.1
+pip install etudatasphere
 ```
 
 Or from GitHub:
 ```bash
 pip install https://github.com/sesh00/etudatasphere/archive/main.zip
 ```
 ## Usage
```

### Comparing `etudatasphere-0.1.2/etudatasphere.egg-info/PKG-INFO` & `etudatasphere-0.1.3/etudatasphere.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etudatasphere
-Version: 0.1.2
+Version: 0.1.3
 Summary: etudatasphere: Simplifying Cloud Administration. Access Yandex.Cloud services with ease, automating routine tasks for resource management.
 Home-page: https://github.com/sesh00/etudatasphere
 Download-URL: https://github.com/sesh00/etudatasphere/archive/main.zip
 Author: sesh00
 Author-email: ernestrsage@gmail.com
 License: MIT License, see LICENSE file
 Classifier: Operating System :: OS Independent
@@ -29,15 +29,15 @@
 This is a Python library for interacting with Yandex DataSphere API. It provides functions to perform various operations such as getting organizations, billing accounts, projects, managing organization members, creating projects, checking operation status, and adding contributors to projects.
 
 ## Installation
 
 Install the current version with [PyPI](https://pypi.org/project/etudatasphere):
 
 ```bash
-pip install etudatasphere==0.1.1
+pip install etudatasphere
 ```
 
 Or from GitHub:
 ```bash
 pip install https://github.com/sesh00/etudatasphere/archive/main.zip
 ```
 ## Usage
```

### Comparing `etudatasphere-0.1.2/setup.py` & `etudatasphere-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from io import open
 from setuptools import setup
 
-version = '0.1.2'
+version = '0.1.3'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='etudatasphere',
     version=version,
```

### Comparing `etudatasphere-0.1.2/tests/test_etudatasphere.py` & `etudatasphere-0.1.3/tests/test_etudatasphere.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import pytest
+import os
 from etudatasphere import DataSphereManager
 
 
 @pytest.fixture(scope="module")
 def data_sphere_manager():
-    data_sphere_manager = DataSphereManager(oauth_token="")
+    oauth_token = os.environ.get("OAUTH_TOKEN")
+    data_sphere_manager = DataSphereManager(oauth_token=oauth_token)
     return data_sphere_manager
 
 
 def test_get_organizations(data_sphere_manager):
-    organizations = data_sphere_manager.get_organizations()
+    data_sphere_manager.get_organizations()
 
 
 def test_get_communities(data_sphere_manager):
     organization_id = "bpfa94oocmi345p7tpv7"
-    communities = data_sphere_manager.get_organization_communities(organization_id)
+    communities = data_sphere_manager.get_organization_communities(organization_id, parse_communities_flag=True)
     print(communities)
 
 
 def test_get_projects(data_sphere_manager):
     community_id = "bt1u8sr3l01444sc22gm"
-    projects = data_sphere_manager.get_projects(community_id=community_id)
+    projects = data_sphere_manager.get_projects(community_id=community_id, parse_projects_flag=True)
     print(projects)
 
 
 def test_get_unit_balance(data_sphere_manager):
     project_id = "bt15an734pcprskkvjkt"
     print(data_sphere_manager.get_unit_balance(project_id))
```

