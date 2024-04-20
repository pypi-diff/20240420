# Comparing `tmp/seatable-api-2.7.0.tar.gz` & `tmp/seatable-api-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/seatable-api-2.7.0.tar", last modified: Wed Apr 17 01:48:29 2024, max compression
+gzip compressed data, was "dist/seatable-api-2.7.1.tar", last modified: Sat Apr 20 08:59:03 2024, max compression
```

## Comparing `seatable-api-2.7.0.tar` & `seatable-api-2.7.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 ranjiwei   (501) staff       (20)        0 2024-04-17 01:48:29.512951 seatable-api-2.7.0/
--rw-r--r--   0 ranjiwei   (501) staff       (20)      733 2024-04-17 01:48:29.512596 seatable-api-2.7.0/PKG-INFO
--rw-r--r--   0 ranjiwei   (501) staff       (20)      300 2021-01-29 01:36:12.000000 seatable-api-2.7.0/README.md
-drwxr-xr-x   0 ranjiwei   (501) staff       (20)        0 2024-04-17 01:48:29.453836 seatable-api-2.7.0/seatable_api/
--rw-r--r--   0 ranjiwei   (501) staff       (20)      171 2024-01-25 01:33:50.000000 seatable-api-2.7.0/seatable_api/__init__.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)    26810 2024-04-17 01:46:18.000000 seatable-api-2.7.0/seatable_api/api_gateway.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)    11418 2021-01-29 01:36:12.000000 seatable-api-2.7.0/seatable_api/column.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)     1135 2021-12-15 04:05:31.000000 seatable-api-2.7.0/seatable_api/constants.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)     1338 2024-01-25 01:33:50.000000 seatable-api-2.7.0/seatable_api/context.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)    29203 2024-01-25 01:33:50.000000 seatable-api-2.7.0/seatable_api/convert_airtable.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)    13988 2024-03-21 06:02:17.000000 seatable-api-2.7.0/seatable_api/date_utils.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)      235 2024-01-25 01:33:50.000000 seatable-api-2.7.0/seatable_api/exception.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)    49205 2024-04-17 01:44:37.000000 seatable-api-2.7.0/seatable_api/main.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)     2876 2021-07-17 06:11:15.000000 seatable-api-2.7.0/seatable_api/message.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)     3006 2021-01-13 04:11:42.000000 seatable-api-2.7.0/seatable_api/parsetab.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)     9400 2021-02-24 08:59:41.000000 seatable-api-2.7.0/seatable_api/query.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)     2744 2021-07-17 06:11:15.000000 seatable-api-2.7.0/seatable_api/socket_io.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)     7276 2024-03-27 08:04:05.000000 seatable-api-2.7.0/seatable_api/utils.py
-drwxr-xr-x   0 ranjiwei   (501) staff       (20)        0 2024-04-17 01:48:29.485168 seatable-api-2.7.0/seatable_api.egg-info/
--rw-r--r--   0 ranjiwei   (501) staff       (20)      733 2024-04-17 01:48:27.000000 seatable-api-2.7.0/seatable_api.egg-info/PKG-INFO
--rw-r--r--   0 ranjiwei   (501) staff       (20)      591 2024-04-17 01:48:29.000000 seatable-api-2.7.0/seatable_api.egg-info/SOURCES.txt
--rw-r--r--   0 ranjiwei   (501) staff       (20)        1 2024-04-17 01:48:27.000000 seatable-api-2.7.0/seatable_api.egg-info/dependency_links.txt
--rw-r--r--   0 ranjiwei   (501) staff       (20)       47 2024-04-17 01:48:27.000000 seatable-api-2.7.0/seatable_api.egg-info/requires.txt
--rw-r--r--   0 ranjiwei   (501) staff       (20)       19 2024-04-17 01:48:27.000000 seatable-api-2.7.0/seatable_api.egg-info/top_level.txt
--rw-r--r--   0 ranjiwei   (501) staff       (20)       38 2024-04-17 01:48:29.513113 seatable-api-2.7.0/setup.cfg
--rw-r--r--   0 ranjiwei   (501) staff       (20)      723 2024-04-17 01:47:54.000000 seatable-api-2.7.0/setup.py
-drwxr-xr-x   0 ranjiwei   (501) staff       (20)        0 2024-04-17 01:48:29.511343 seatable-api-2.7.0/tests/
--rw-r--r--   0 ranjiwei   (501) staff       (20)        0 2023-04-14 03:49:39.000000 seatable-api-2.7.0/tests/__init__.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)     5261 2023-04-14 03:49:39.000000 seatable-api-2.7.0/tests/dateutils_test.py
+drwxr-xr-x   0 ranjiwei   (501) staff       (20)        0 2024-04-20 08:59:03.393421 seatable-api-2.7.1/
+-rw-r--r--   0 ranjiwei   (501) staff       (20)      733 2024-04-20 08:59:03.392970 seatable-api-2.7.1/PKG-INFO
+-rw-r--r--   0 ranjiwei   (501) staff       (20)      300 2021-01-29 01:36:12.000000 seatable-api-2.7.1/README.md
+drwxr-xr-x   0 ranjiwei   (501) staff       (20)        0 2024-04-20 08:59:03.379384 seatable-api-2.7.1/seatable_api/
+-rw-r--r--   0 ranjiwei   (501) staff       (20)      171 2024-01-25 01:33:50.000000 seatable-api-2.7.1/seatable_api/__init__.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)    26847 2024-04-20 02:17:39.000000 seatable-api-2.7.1/seatable_api/api_gateway.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)    11418 2021-01-29 01:36:12.000000 seatable-api-2.7.1/seatable_api/column.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     1135 2021-12-15 04:05:31.000000 seatable-api-2.7.1/seatable_api/constants.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     1338 2024-01-25 01:33:50.000000 seatable-api-2.7.1/seatable_api/context.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)    29203 2024-01-25 01:33:50.000000 seatable-api-2.7.1/seatable_api/convert_airtable.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)    13988 2024-03-21 06:02:17.000000 seatable-api-2.7.1/seatable_api/date_utils.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)      235 2024-01-25 01:33:50.000000 seatable-api-2.7.1/seatable_api/exception.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)    49211 2024-04-20 04:44:43.000000 seatable-api-2.7.1/seatable_api/main.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     2876 2021-07-17 06:11:15.000000 seatable-api-2.7.1/seatable_api/message.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     3006 2021-01-13 04:11:42.000000 seatable-api-2.7.1/seatable_api/parsetab.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     9400 2021-02-24 08:59:41.000000 seatable-api-2.7.1/seatable_api/query.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     2744 2021-07-17 06:11:15.000000 seatable-api-2.7.1/seatable_api/socket_io.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     7276 2024-03-27 08:04:05.000000 seatable-api-2.7.1/seatable_api/utils.py
+drwxr-xr-x   0 ranjiwei   (501) staff       (20)        0 2024-04-20 08:59:03.386672 seatable-api-2.7.1/seatable_api.egg-info/
+-rw-r--r--   0 ranjiwei   (501) staff       (20)      733 2024-04-20 08:59:03.000000 seatable-api-2.7.1/seatable_api.egg-info/PKG-INFO
+-rw-r--r--   0 ranjiwei   (501) staff       (20)      591 2024-04-20 08:59:03.000000 seatable-api-2.7.1/seatable_api.egg-info/SOURCES.txt
+-rw-r--r--   0 ranjiwei   (501) staff       (20)        1 2024-04-20 08:59:03.000000 seatable-api-2.7.1/seatable_api.egg-info/dependency_links.txt
+-rw-r--r--   0 ranjiwei   (501) staff       (20)       47 2024-04-20 08:59:03.000000 seatable-api-2.7.1/seatable_api.egg-info/requires.txt
+-rw-r--r--   0 ranjiwei   (501) staff       (20)       19 2024-04-20 08:59:03.000000 seatable-api-2.7.1/seatable_api.egg-info/top_level.txt
+-rw-r--r--   0 ranjiwei   (501) staff       (20)       38 2024-04-20 08:59:03.393555 seatable-api-2.7.1/setup.cfg
+-rw-r--r--   0 ranjiwei   (501) staff       (20)      723 2024-04-20 08:58:20.000000 seatable-api-2.7.1/setup.py
+drwxr-xr-x   0 ranjiwei   (501) staff       (20)        0 2024-04-20 08:59:03.391869 seatable-api-2.7.1/tests/
+-rw-r--r--   0 ranjiwei   (501) staff       (20)        0 2023-04-14 03:49:39.000000 seatable-api-2.7.1/tests/__init__.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     5261 2023-04-14 03:49:39.000000 seatable-api-2.7.1/tests/dateutils_test.py
```

### Comparing `seatable-api-2.7.0/PKG-INFO` & `seatable-api-2.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatable-api
-Version: 2.7.0
+Version: 2.7.1
 Summary: Python client for SeaTable web api
 Home-page: https://github.com/seatable/seatable-api-python
 Author: seatable
 Author-email: support@seafile.com
 License: Apache Licence
 Description: # seatable-api-python
```

### Comparing `seatable-api-2.7.0/seatable_api/api_gateway.py` & `seatable-api-2.7.1/seatable_api/api_gateway.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,16 @@
             'rows': [row_data,]
         }
         if like_table_id(table_name):
             json_data['table_id'] = table_name
         if apply_default is not None:
             json_data['apply_default'] = apply_default
         response = requests.post(url, json=json_data, headers=self.headers, timeout=self.timeout)
-        return parse_response(response)
+        data = parse_response(response)
+        return data.get('first_row')
 
     
     def batch_append_rows(self, table_name, rows_data, apply_default=None):
         """
         :param table_name: str
         :param rows_data: dict
         """
```

### Comparing `seatable-api-2.7.0/seatable_api/column.py` & `seatable-api-2.7.1/seatable_api/column.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.0/seatable_api/constants.py` & `seatable-api-2.7.1/seatable_api/constants.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.0/seatable_api/context.py` & `seatable-api-2.7.1/seatable_api/context.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.0/seatable_api/convert_airtable.py` & `seatable-api-2.7.1/seatable_api/convert_airtable.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.0/seatable_api/date_utils.py` & `seatable-api-2.7.1/seatable_api/date_utils.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.0/seatable_api/main.py` & `seatable-api-2.7.1/seatable_api/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         self.jwt_token = data.get('access_token')
         self.headers = parse_headers(self.jwt_token)
         self.workspace_id = data.get('workspace_id')
         self.dtable_uuid = data.get('dtable_uuid')
         self.dtable_name = data.get('dtable_name')
 
         # api gateway entry
-        self.use_api_gateway = data.get('use_api_gateway')
+        self.use_api_gateway = data.get('use_api_gateway', True)
         if self.use_api_gateway:
             self.api_gateway = APIGateway(
                 token = self.token,
                 api_gateway_url=self.server_url + '/api-gateway',
                 server_url=self.server_url,
                 headers=self.headers,
                 dtable_uuid=self.dtable_uuid
```

### Comparing `seatable-api-2.7.0/seatable_api/message.py` & `seatable-api-2.7.1/seatable_api/message.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.0/seatable_api/parsetab.py` & `seatable-api-2.7.1/seatable_api/parsetab.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.0/seatable_api/query.py` & `seatable-api-2.7.1/seatable_api/query.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.0/seatable_api/socket_io.py` & `seatable-api-2.7.1/seatable_api/socket_io.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.0/seatable_api/utils.py` & `seatable-api-2.7.1/seatable_api/utils.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.0/seatable_api.egg-info/PKG-INFO` & `seatable-api-2.7.1/seatable_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatable-api
-Version: 2.7.0
+Version: 2.7.1
 Summary: Python client for SeaTable web api
 Home-page: https://github.com/seatable/seatable-api-python
 Author: seatable
 Author-email: support@seafile.com
 License: Apache Licence
 Description: # seatable-api-python
```

### Comparing `seatable-api-2.7.0/seatable_api.egg-info/SOURCES.txt` & `seatable-api-2.7.1/seatable_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.0/setup.py` & `seatable-api-2.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '2.7.0'
+__version__ = '2.7.1'
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='seatable-api',
     version=__version__,
```

### Comparing `seatable-api-2.7.0/tests/dateutils_test.py` & `seatable-api-2.7.1/tests/dateutils_test.py`

 * *Files identical despite different names*

