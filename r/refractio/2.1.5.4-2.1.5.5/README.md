# Comparing `tmp/refractio-2.1.5.4.tar.gz` & `tmp/refractio-2.1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refractio-2.1.5.4.tar", last modified: Tue Mar 19 08:55:44 2024, max compression
+gzip compressed data, was "refractio-2.1.5.5.tar", last modified: Sat Apr 20 08:26:03 2024, max compression
```

## Comparing `refractio-2.1.5.4.tar` & `refractio-2.1.5.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 08:55:44.214082 refractio-2.1.5.4/
--rw-r--r--   0 root         (0) root         (0)    11562 2024-03-19 08:55:44.214082 refractio-2.1.5.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10870 2024-03-19 08:55:01.000000 refractio-2.1.5.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 08:55:44.214082 refractio-2.1.5.4/refractio/
--rw-r--r--   0 root         (0) root         (0)      968 2024-03-19 08:55:01.000000 refractio-2.1.5.4/refractio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3742 2024-03-19 08:54:43.000000 refractio-2.1.5.4/refractio/amazons3.py
--rw-r--r--   0 root         (0) root         (0)     3611 2024-03-19 08:54:43.000000 refractio-2.1.5.4/refractio/azure.py
--rw-r--r--   0 root         (0) root         (0)     1525 2024-03-19 08:54:43.000000 refractio-2.1.5.4/refractio/feature_store.py
--rw-r--r--   0 root         (0) root         (0)     8065 2024-03-19 08:54:43.000000 refractio-2.1.5.4/refractio/hive.py
--rw-r--r--   0 root         (0) root         (0)     4173 2024-03-19 08:55:01.000000 refractio-2.1.5.4/refractio/manager.py
--rw-r--r--   0 root         (0) root         (0)     4488 2024-03-19 08:54:43.000000 refractio-2.1.5.4/refractio/mysql.py
--rw-r--r--   0 root         (0) root         (0)     4795 2024-03-19 08:54:43.000000 refractio-2.1.5.4/refractio/postgres.py
--rw-r--r--   0 root         (0) root         (0)    16424 2024-03-19 08:55:01.000000 refractio-2.1.5.4/refractio/refractio.py
--rw-r--r--   0 root         (0) root         (0)     4290 2024-03-19 08:54:43.000000 refractio-2.1.5.4/refractio/sftp.py
--rw-r--r--   0 root         (0) root         (0)     5918 2024-03-19 08:55:01.000000 refractio-2.1.5.4/refractio/snowflake.py
--rw-r--r--   0 root         (0) root         (0)     6332 2024-03-19 08:54:43.000000 refractio-2.1.5.4/refractio/sqlserver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 08:55:44.214082 refractio-2.1.5.4/refractio.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11562 2024-03-19 08:55:44.000000 refractio-2.1.5.4/refractio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      439 2024-03-19 08:55:44.000000 refractio-2.1.5.4/refractio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-19 08:55:44.000000 refractio-2.1.5.4/refractio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      610 2024-03-19 08:55:44.000000 refractio-2.1.5.4/refractio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-03-19 08:55:44.000000 refractio-2.1.5.4/refractio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-19 08:55:44.214082 refractio-2.1.5.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2041 2024-03-19 08:55:01.000000 refractio-2.1.5.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 08:26:03.050913 refractio-2.1.5.5/
+-rw-r--r--   0 root         (0) root         (0)    11562 2024-04-20 08:26:03.050913 refractio-2.1.5.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10870 2024-04-20 08:25:09.000000 refractio-2.1.5.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 08:26:03.046913 refractio-2.1.5.5/refractio/
+-rw-r--r--   0 root         (0) root         (0)      968 2024-04-20 08:25:09.000000 refractio-2.1.5.5/refractio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3742 2024-04-20 08:24:01.000000 refractio-2.1.5.5/refractio/amazons3.py
+-rw-r--r--   0 root         (0) root         (0)     3611 2024-04-20 08:24:01.000000 refractio-2.1.5.5/refractio/azure.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2024-04-20 08:24:01.000000 refractio-2.1.5.5/refractio/feature_store.py
+-rw-r--r--   0 root         (0) root         (0)     8065 2024-04-20 08:24:01.000000 refractio-2.1.5.5/refractio/hive.py
+-rw-r--r--   0 root         (0) root         (0)     4276 2024-04-20 08:25:09.000000 refractio-2.1.5.5/refractio/manager.py
+-rw-r--r--   0 root         (0) root         (0)     4488 2024-04-20 08:24:01.000000 refractio-2.1.5.5/refractio/mysql.py
+-rw-r--r--   0 root         (0) root         (0)     4795 2024-04-20 08:24:01.000000 refractio-2.1.5.5/refractio/postgres.py
+-rw-r--r--   0 root         (0) root         (0)    16435 2024-04-20 08:25:09.000000 refractio-2.1.5.5/refractio/refractio.py
+-rw-r--r--   0 root         (0) root         (0)     4290 2024-04-20 08:24:01.000000 refractio-2.1.5.5/refractio/sftp.py
+-rw-r--r--   0 root         (0) root         (0)     5929 2024-04-20 08:25:09.000000 refractio-2.1.5.5/refractio/snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     6332 2024-04-20 08:24:01.000000 refractio-2.1.5.5/refractio/sqlserver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 08:26:03.050913 refractio-2.1.5.5/refractio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11562 2024-04-20 08:26:03.000000 refractio-2.1.5.5/refractio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      439 2024-04-20 08:26:03.000000 refractio-2.1.5.5/refractio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 08:26:03.000000 refractio-2.1.5.5/refractio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      610 2024-04-20 08:26:03.000000 refractio-2.1.5.5/refractio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-20 08:26:03.000000 refractio-2.1.5.5/refractio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 08:26:03.050913 refractio-2.1.5.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2041 2024-04-20 08:25:09.000000 refractio-2.1.5.5/setup.py
```

### Comparing `refractio-2.1.5.4/PKG-INFO` & `refractio-2.1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.1.5.4
+Version: 2.1.5.5
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://gitlab.fosfor.com/fosfor-decision-cloud/intelligence/refract-sdk
 Keywords: refractio
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `refractio-2.1.5.4/README.md` & `refractio-2.1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `refractio-2.1.5.4/refractio/__init__.py` & `refractio-2.1.5.5/refractio/__init__.py`

 * *Files identical despite different names*

### Comparing `refractio-2.1.5.4/refractio/amazons3.py` & `refractio-2.1.5.5/refractio/amazons3.py`

 * *Files identical despite different names*

### Comparing `refractio-2.1.5.4/refractio/azure.py` & `refractio-2.1.5.5/refractio/azure.py`

 * *Files identical despite different names*

### Comparing `refractio-2.1.5.4/refractio/feature_store.py` & `refractio-2.1.5.5/refractio/feature_store.py`

 * *Files identical despite different names*

### Comparing `refractio-2.1.5.4/refractio/hive.py` & `refractio-2.1.5.5/refractio/hive.py`

 * *Files identical despite different names*

### Comparing `refractio-2.1.5.4/refractio/manager.py` & `refractio-2.1.5.5/refractio/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,24 +88,28 @@
                     (con["createdBy"].lower() if con["createdBy"] else None) == default_user_name.lower()]
         print(f"Connection names fetched {con_name}, created by {default_user_name}")
     else:
         print("Could not get user id from the OS env.")
     return con_name[0] if con_name else None  # first connection name from all the connections created by user_id
 
 
-def get_dataframe_query(table_name, row_count, filter_condition, top=None):
+def get_dataframe_query(table_name, row_count, filter_condition, top=None, snow=None):
     """
     To get the query to fetch dataframe
     :param table_name:
     :param row_count:
     :param filter_condition:
     :param top:
+    :param snow:
     :return: query
     """
-    query = f"SELECT * FROM {table_name}"
+    if snow:
+        query = f'SELECT * FROM "{table_name}"'
+    else:
+        query = f"SELECT * FROM {table_name}"
     if top and int(row_count) > 0:
         print(f"fetching {row_count} records!")
         query = f"SELECT TOP {row_count} * FROM {table_name}"
     if filter_condition:
         query = query + " " + filter_condition
     if not top and int(row_count) > 0:
         print(f"fetching {row_count} records!")
```

### Comparing `refractio-2.1.5.4/refractio/mysql.py` & `refractio-2.1.5.5/refractio/mysql.py`

 * *Files identical despite different names*

### Comparing `refractio-2.1.5.4/refractio/postgres.py` & `refractio-2.1.5.5/refractio/postgres.py`

 * *Files identical despite different names*

### Comparing `refractio-2.1.5.4/refractio/refractio.py` & `refractio-2.1.5.5/refractio/refractio.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         schema=connection_details["params"]["READER"]["schema"],
         wareHouse=connection_details["params"]["READER"]["wareHouse"],
         region=connection_details["params"]["READER"]["region"] + ".gcp" if connection_details["params"]["READER"]["cloudPlatform"] == "gcp" else connection_details["params"]["READER"]["region"]
     )
     # Create cursor
     cur = con.cursor()
     query = get_dataframe_query(connection_details['params']['READER']['tables'],
-                                row_count, filter_condition)  # Get query to fetch details
+                                row_count, filter_condition, snow=True)  # Get query to fetch details
 
     cur.execute(f"use warehouse {connection_details['params']['READER']['wareHouse']};")  # Setting up warehouse, it is needed in new snowflake gcp connections.
 
     cur.execute(query)  # Execute query
 
     # Read results into a pandas DataFrame
     data_frame = cur.fetch_pandas_all()
```

### Comparing `refractio-2.1.5.4/refractio/sftp.py` & `refractio-2.1.5.5/refractio/sftp.py`

 * *Files identical despite different names*

### Comparing `refractio-2.1.5.4/refractio/snowflake.py` & `refractio-2.1.5.5/refractio/snowflake.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             self.__connection_details = get_conn_details_from_ds_name(dataset_name=dataset_name, project_id=project_id)
             # Creating new connection attached to dataset_id for reading the dataset.
             self._get_connection()
 
             cur = self.con_obj.cursor()     # Creating cursor for executing query
 
             query = get_dataframe_query(self.__connection_details['params']['READER']['tables'],
-                                        row_count, filter_condition)     # Get query to fetch details
+                                        row_count, filter_condition, snow=True)     # Get query to fetch details
 
             cur.execute(f"use warehouse {self.__connection_details['params']['READER']['wareHouse']};")     # Setting up warehouse, it is needed in new snowflake gcp connections.
 
             cur.execute(query)      # Execute query
 
             data_frame = cur.fetch_pandas_all()     # Fetch all records in pandas dataframe
```

### Comparing `refractio-2.1.5.4/refractio/sqlserver.py` & `refractio-2.1.5.5/refractio/sqlserver.py`

 * *Files identical despite different names*

### Comparing `refractio-2.1.5.4/refractio.egg-info/PKG-INFO` & `refractio-2.1.5.5/refractio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.1.5.4
+Version: 2.1.5.5
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://gitlab.fosfor.com/fosfor-decision-cloud/intelligence/refract-sdk
 Keywords: refractio
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `refractio-2.1.5.4/refractio.egg-info/requires.txt` & `refractio-2.1.5.5/refractio.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `refractio-2.1.5.4/setup.py` & `refractio-2.1.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # read the contents of README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
-VERSION = '2.1.5.4'
+VERSION = '2.1.5.5'
 DESCRIPTION = 'REFRACT-IO: To read and write dataframe from different connectors.'
 
 extras_require = {
     "all": [
         "snowflake-connector-python[pandas]==3.6.0",
         "boto3==1.26.116",
         "azure==4.0.0",
```

