# Comparing `tmp/cloudpy_org-1.4.7.tar.gz` & `tmp/cloudpy_org-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpy_org-1.4.7.tar", last modified: Sat Apr 20 06:30:19 2024, max compression
+gzip compressed data, was "dist\cloudpy_org-1.4.8.tar", last modified: Sat Apr 20 07:32:12 2024, max compression
```

## Comparing `cloudpy_org-1.4.7.tar` & `cloudpy_org-1.4.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 06:30:19.006675 cloudpy_org-1.4.7/
--rw-rw-rw-   0        0        0      935 2024-04-20 06:30:19.006174 cloudpy_org-1.4.7/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.4.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 06:30:18.862113 cloudpy_org-1.4.7/cloudpy_org/
--rw-rw-rw-   0        0        0     1819 2024-04-20 05:15:05.000000 cloudpy_org-1.4.7/cloudpy_org/__init__.py
--rw-rw-rw-   0        0        0    31391 2024-04-20 05:38:00.000000 cloudpy_org-1.4.7/cloudpy_org/aws.py
--rw-rw-rw-   0        0        0    12316 2024-02-26 22:47:47.000000 cloudpy_org-1.4.7/cloudpy_org/docs.py
--rw-rw-rw-   0        0        0     2618 2024-02-22 21:16:50.000000 cloudpy_org-1.4.7/cloudpy_org/imgedit.py
--rw-rw-rw-   0        0        0    49191 2024-04-19 17:14:28.000000 cloudpy_org-1.4.7/cloudpy_org/tools.py
--rw-rw-rw-   0        0        0     3701 2023-12-20 02:08:16.000000 cloudpy_org-1.4.7/cloudpy_org/web.py
-drwxrwxrwx   0        0        0        0 2024-04-20 06:30:18.983904 cloudpy_org-1.4.7/cloudpy_org.egg-info/
--rw-rw-rw-   0        0        0      935 2024-04-20 06:30:16.000000 cloudpy_org-1.4.7/cloudpy_org.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-04-20 06:30:17.000000 cloudpy_org-1.4.7/cloudpy_org.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 06:30:16.000000 cloudpy_org-1.4.7/cloudpy_org.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-20 06:30:16.000000 cloudpy_org-1.4.7/cloudpy_org.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-20 06:30:16.000000 cloudpy_org-1.4.7/cloudpy_org.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 06:30:19.007179 cloudpy_org-1.4.7/setup.cfg
--rw-rw-rw-   0        0        0     1324 2024-04-20 03:03:10.000000 cloudpy_org-1.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:32:12.496070 cloudpy_org-1.4.8/
+-rw-rw-rw-   0        0        0      935 2024-04-20 07:32:12.495070 cloudpy_org-1.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.4.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 07:32:12.365898 cloudpy_org-1.4.8/cloudpy_org/
+-rw-rw-rw-   0        0        0     1794 2024-04-20 07:29:46.000000 cloudpy_org-1.4.8/cloudpy_org/__init__.py
+-rw-rw-rw-   0        0        0    31391 2024-04-20 05:38:00.000000 cloudpy_org-1.4.8/cloudpy_org/aws.py
+-rw-rw-rw-   0        0        0    12316 2024-02-26 22:47:47.000000 cloudpy_org-1.4.8/cloudpy_org/docs.py
+-rw-rw-rw-   0        0        0     2618 2024-02-22 21:16:50.000000 cloudpy_org-1.4.8/cloudpy_org/imgedit.py
+-rw-rw-rw-   0        0        0    49191 2024-04-19 17:14:28.000000 cloudpy_org-1.4.8/cloudpy_org/tools.py
+-rw-rw-rw-   0        0        0     3701 2023-12-20 02:08:16.000000 cloudpy_org-1.4.8/cloudpy_org/web.py
+drwxrwxrwx   0        0        0        0 2024-04-20 07:32:12.472542 cloudpy_org-1.4.8/cloudpy_org.egg-info/
+-rw-rw-rw-   0        0        0      935 2024-04-20 07:32:12.000000 cloudpy_org-1.4.8/cloudpy_org.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-04-20 07:32:12.000000 cloudpy_org-1.4.8/cloudpy_org.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 07:32:12.000000 cloudpy_org-1.4.8/cloudpy_org.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-20 07:32:12.000000 cloudpy_org-1.4.8/cloudpy_org.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-20 07:32:12.000000 cloudpy_org-1.4.8/cloudpy_org.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 07:32:12.496070 cloudpy_org-1.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     1324 2024-04-20 07:30:02.000000 cloudpy_org-1.4.8/setup.py
```

### Comparing `cloudpy_org-1.4.7/PKG-INFO` & `cloudpy_org-1.4.8/cloudpy_org.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cloudpy_org
-Version: 1.4.7
+Name: cloudpy-org
+Version: 1.4.8
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.4.7/cloudpy_org/__init__.py` & `cloudpy_org-1.4.8/cloudpy_org/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,14 @@
  'eu-west-1': {'long_name': 'Europe (Ireland)', 'code': 'euw1'},
  'eu-west-2': {'long_name': 'Europe (London)', 'code': 'euw2'},
  'eu-west-3': {'long_name': 'Europe (Paris)', 'code': 'euw3'},
  'eu-north-1': {'long_name': 'Europe (Stockholm)', 'code': 'eun1'},
  'sa-east-1': {'long_name': 'South America (São Paulo)', 'code': 'sae1'}}
 subscription_url = 'https://www.cloudpy.org'
 msh = 'secure'
-cloudpy_org_version='1.4.7'
+cloudpy_org_version='1.4.8'
 gsep = {'user_email_sep': '-0-', '@': '-1-', '.': '-2-'}
-from cloudpy_org_base.tools import processing_tools
-from cloudpy_org_base.docs import auto_document,convert_jupiter_notebook_to_html,documentation_from_folder
-from cloudpy_org_base.aws import aws_framework_manager,aws_framework_manager_client,gen_aws_auth_token,gen_new_service_token,configure_aws,get_my_aws_service_token,authenticate_with_token,delete_biscuit,co_token_auth
-from cloudpy_org_base.web import flask_website
-from cloudpy_org_base.imgedit import colors
+from cloudpy_org.tools import processing_tools
+from cloudpy_org.docs import auto_document,convert_jupiter_notebook_to_html,documentation_from_folder
+from cloudpy_org.aws import aws_framework_manager,aws_framework_manager_client,gen_aws_auth_token,gen_new_service_token,configure_aws,get_my_aws_service_token,authenticate_with_token,delete_biscuit,co_token_auth
+from cloudpy_org.web import flask_website
+from cloudpy_org.imgedit import colors
```

### Comparing `cloudpy_org-1.4.7/cloudpy_org/aws.py` & `cloudpy_org-1.4.8/cloudpy_org/aws.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.4.7/cloudpy_org/docs.py` & `cloudpy_org-1.4.8/cloudpy_org/docs.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.4.7/cloudpy_org/imgedit.py` & `cloudpy_org-1.4.8/cloudpy_org/imgedit.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.4.7/cloudpy_org/tools.py` & `cloudpy_org-1.4.8/cloudpy_org/tools.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.4.7/cloudpy_org/web.py` & `cloudpy_org-1.4.8/cloudpy_org/web.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.4.7/cloudpy_org.egg-info/PKG-INFO` & `cloudpy_org-1.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cloudpy-org
-Version: 1.4.7
+Name: cloudpy_org
+Version: 1.4.8
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.4.7/setup.py` & `cloudpy_org-1.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from os import path
 
 
 long_description = 'A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.'
 
 setup(
     name="cloudpy_org",
-    version="1.4.7",
+    version="1.4.8",
     description="Cloud data pipeline organization and automation library. Includes AWS framework manager API.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://www.cloudpy.org/",
     author="cloudpy.org",
     author_email="admin@cloudpy.org",
     license="MIT",
```

