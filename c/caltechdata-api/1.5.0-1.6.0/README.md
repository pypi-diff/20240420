# Comparing `tmp/caltechdata_api-1.5.0.tar.gz` & `tmp/caltechdata_api-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caltechdata_api-1.5.0.tar", last modified: Wed Nov 15 21:45:57 2023, max compression
+gzip compressed data, was "caltechdata_api-1.6.0.tar", last modified: Fri Apr 19 22:17:10 2024, max compression
```

## Comparing `caltechdata_api-1.5.0.tar` & `caltechdata_api-1.6.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 21:45:57.362888 caltechdata_api-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2023-11-15 21:45:51.000000 caltechdata_api-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2023-11-15 21:45:57.362888 caltechdata_api-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2023-11-15 21:45:51.000000 caltechdata_api-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 21:45:57.362888 caltechdata_api-1.5.0/caltechdata_api/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2023-11-15 21:45:51.000000 caltechdata_api-1.5.0/caltechdata_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2023-11-15 21:45:51.000000 caltechdata_api-1.5.0/caltechdata_api/caltechdata_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2023-11-15 21:45:51.000000 caltechdata_api-1.5.0/caltechdata_api/caltechdata_write.py
--rw-r--r--   0 runner    (1001) docker     (127)    16239 2023-11-15 21:45:51.000000 caltechdata_api-1.5.0/caltechdata_api/customize_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2023-11-15 21:45:51.000000 caltechdata_api-1.5.0/caltechdata_api/download_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2023-11-15 21:45:51.000000 caltechdata_api-1.5.0/caltechdata_api/get_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2023-11-15 21:45:51.000000 caltechdata_api-1.5.0/caltechdata_api/get_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2023-11-15 21:45:51.000000 caltechdata_api-1.5.0/caltechdata_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 21:45:57.362888 caltechdata_api-1.5.0/caltechdata_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2023-11-15 21:45:57.000000 caltechdata_api-1.5.0/caltechdata_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      476 2023-11-15 21:45:57.000000 caltechdata_api-1.5.0/caltechdata_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 21:45:57.000000 caltechdata_api-1.5.0/caltechdata_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-11-15 21:45:57.000000 caltechdata_api-1.5.0/caltechdata_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-15 21:45:57.000000 caltechdata_api-1.5.0/caltechdata_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-15 21:45:57.362888 caltechdata_api-1.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4595 2023-11-15 21:45:51.000000 caltechdata_api-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:17:10.670002 caltechdata_api-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-19 22:17:10.670002 caltechdata_api-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:17:10.670002 caltechdata_api-1.6.0/caltechdata_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/caltechdata_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9278 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/caltechdata_api/caltechdata_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/caltechdata_api/caltechdata_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22623 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/caltechdata_api/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16237 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/caltechdata_api/customize_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/caltechdata_api/download_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/caltechdata_api/get_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/caltechdata_api/get_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/caltechdata_api/md_to_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/caltechdata_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:17:10.670002 caltechdata_api-1.6.0/caltechdata_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-19 22:17:10.000000 caltechdata_api-1.6.0/caltechdata_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-19 22:17:10.000000 caltechdata_api-1.6.0/caltechdata_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 22:17:10.000000 caltechdata_api-1.6.0/caltechdata_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-19 22:17:10.000000 caltechdata_api-1.6.0/caltechdata_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-19 22:17:10.000000 caltechdata_api-1.6.0/caltechdata_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 22:17:10.000000 caltechdata_api-1.6.0/caltechdata_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 22:17:10.670002 caltechdata_api-1.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4774 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/setup.py
```

### Comparing `caltechdata_api-1.5.0/LICENSE` & `caltechdata_api-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.5.0/PKG-INFO` & `caltechdata_api-1.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caltechdata_api
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python wrapper for CaltechDATA API.
 Home-page: https://github.com/caltechlibrary/caltechdata_api
 Author: Thomas E Morrell
 Author-email: tmorrell@caltech.edu
 License: https://data.caltech.edu/license
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
@@ -14,46 +14,64 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# caltechdata_api
+# CaltechDATA API Python Library
 
-Python library for using the CaltechDATA API
+The `caltechdata_api` Python library provides a convenient interface for interacting with the CaltechDATA API. It allows users to write files, create DataCite 4 standard JSON records, edit existing records, and retrieve metadata from the CaltechDATA repository.
 
-- caltechdata_write write files and a DataCite 4 standard json record to CaltechDATA repository
-- caltechdata_edit edits records in CaltechDATA
-- get_metadata gets metadata from CaltechDATA records
+## Features
 
-Requires Python 3 (Recommended via Anaconda https://www.anaconda.com/download) with reqests library.
+### Writing and Editing Records
+- `caltechdata_write`: Writes files and a DataCite 4 standard JSON record to the CaltechDATA repository.
+- `caltechdata_edit`: Edits existing records in CaltechDATA.
+
+### Metadata Operations
+- `get_metadata`: Retrieves metadata from CaltechDATA records.
+
+## Requirements
+
+- Python 3 (Anaconda is recommended)
+- `requests` library
+
+## Installation
+
+Install the library via pip:
+
+```shell
+pip install caltechdata_api
+```
 
 ## Examples
 
 There are some example python scripts in the GitHub repository.
 
-Create a record:
+###Create a record:
 
 ```shell
 python write.py example.json -fnames logo.gif
-pbkn6-m9y63
+# Output: pbkn6-m9y63 (unique identifier)
 ```
-The response will be the unique identifier for the record. You can put this at
+> The response will be the unique identifier for the record. You can put this at
 the end of a url to visit the record (e.g.
 https://data.caltechlibrary.dev/records/pbkn6-m9y63)
 
-Edit a record (make changes to the example.json file to see a change)
+###Edit a record 
+Make changes to the example.json file to see a change)
 ```
 python edit.py example.json -id pbkn6-m9y63
 10.33569/pbkn6-m9y63
 ```
-The response is the DOI for the record, which includes the unique identifier
+> The response is the DOI for the record, which includes the unique identifier
 for the record in the default configuration.
 
+## Using Custom DOIs 
 Some groups have worked with the library to create custom DOIs. These can be
 passed in the metadata like:
 
 ```shell
 python write.py example_custom.json -fnames logo.gif
 m6zxz-p4j22
 ```
@@ -62,23 +80,21 @@
 ```
 python edit.py example_custom.json -id m6zxz-p4j22
 10.5281/inveniordm.1234
 ```
 
 This returns the custom DOI of the record if it is successful.
 
-## Setup 
 
-Install by typing 'pip install caltechdata_api'
+## Setup and Authentication
 
-## Usage
+1. Acquire a personal access token from your CaltechDATA account (found under "Applications" at the top right of your screen).
+2. Copy the token to a file named token.bash.
+3. Load the token in the command line using source token.bash.
 
-You need to acquire a personal access token from your CaltechDATA account
-(find it at the top right of your screen under "Applications").
-Then copy the token to token.bash.  Type `source token.bash` in 
-the command line to load the token.  
+## Note on Testing
 
-Only test your application on the test repository (data.caltechlibrary.dev).  Testing the API on the public 
+Only test your application on the test repository (`data.caltechlibrary.dev`).  Testing the API on the public 
 repository will generate junk records that are annoying to delete.
```

### Comparing `caltechdata_api-1.5.0/README.md` & `caltechdata_api-1.6.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,57 @@
-# caltechdata_api
+# CaltechDATA API Python Library
 
-Python library for using the CaltechDATA API
+The `caltechdata_api` Python library provides a convenient interface for interacting with the CaltechDATA API. It allows users to write files, create DataCite 4 standard JSON records, edit existing records, and retrieve metadata from the CaltechDATA repository.
 
-- caltechdata_write write files and a DataCite 4 standard json record to CaltechDATA repository
-- caltechdata_edit edits records in CaltechDATA
-- get_metadata gets metadata from CaltechDATA records
+## Features
 
-Requires Python 3 (Recommended via Anaconda https://www.anaconda.com/download) with reqests library.
+### Writing and Editing Records
+- `caltechdata_write`: Writes files and a DataCite 4 standard JSON record to the CaltechDATA repository.
+- `caltechdata_edit`: Edits existing records in CaltechDATA.
+
+### Metadata Operations
+- `get_metadata`: Retrieves metadata from CaltechDATA records.
+
+## Requirements
+
+- Python 3 (Anaconda is recommended)
+- `requests` library
+
+## Installation
+
+Install the library via pip:
+
+```shell
+pip install caltechdata_api
+```
 
 ## Examples
 
 There are some example python scripts in the GitHub repository.
 
-Create a record:
+###Create a record:
 
 ```shell
 python write.py example.json -fnames logo.gif
-pbkn6-m9y63
+# Output: pbkn6-m9y63 (unique identifier)
 ```
-The response will be the unique identifier for the record. You can put this at
+> The response will be the unique identifier for the record. You can put this at
 the end of a url to visit the record (e.g.
 https://data.caltechlibrary.dev/records/pbkn6-m9y63)
 
-Edit a record (make changes to the example.json file to see a change)
+###Edit a record 
+Make changes to the example.json file to see a change)
 ```
 python edit.py example.json -id pbkn6-m9y63
 10.33569/pbkn6-m9y63
 ```
-The response is the DOI for the record, which includes the unique identifier
+> The response is the DOI for the record, which includes the unique identifier
 for the record in the default configuration.
 
+## Using Custom DOIs 
 Some groups have worked with the library to create custom DOIs. These can be
 passed in the metadata like:
 
 ```shell
 python write.py example_custom.json -fnames logo.gif
 m6zxz-p4j22
 ```
@@ -42,21 +60,19 @@
 ```
 python edit.py example_custom.json -id m6zxz-p4j22
 10.5281/inveniordm.1234
 ```
 
 This returns the custom DOI of the record if it is successful.
 
-## Setup 
 
-Install by typing 'pip install caltechdata_api'
+## Setup and Authentication
 
-## Usage
+1. Acquire a personal access token from your CaltechDATA account (found under "Applications" at the top right of your screen).
+2. Copy the token to a file named token.bash.
+3. Load the token in the command line using source token.bash.
 
-You need to acquire a personal access token from your CaltechDATA account
-(find it at the top right of your screen under "Applications").
-Then copy the token to token.bash.  Type `source token.bash` in 
-the command line to load the token.  
+## Note on Testing
 
-Only test your application on the test repository (data.caltechlibrary.dev).  Testing the API on the public 
+Only test your application on the test repository (`data.caltechlibrary.dev`).  Testing the API on the public 
 repository will generate junk records that are annoying to delete.
```

### Comparing `caltechdata_api-1.5.0/caltechdata_api/caltechdata_edit.py` & `caltechdata_api-1.6.0/caltechdata_api/caltechdata_edit.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
     headers = {
         "Authorization": "Bearer %s" % token,
         "Content-type": "application/json",
     }
 
     for idv in ids:
-
         result = requests.get(
             url + "/api/records/" + idv + "/draft/review", headers=headers
         )
 
         accept_link = result.json()["links"]["actions"]["accept"]
         data = comment = {
             "payload": {
```

### Comparing `caltechdata_api-1.5.0/caltechdata_api/caltechdata_write.py` & `caltechdata_api-1.6.0/caltechdata_api/caltechdata_write.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,17 +63,17 @@
             if result.status_code != 204:
                 raise Exception(result.text)
 
 
 def add_file_links(
     metadata, file_links, file_descriptions=[], additional_descriptions="", s3_link=None
 ):
-    # Currently configured for OSN S3 links
+    # Currently configured for S3 links, assuming all are at same endpoint
     link_string = ""
-    endpoint = "https://renc.osn.xsede.org/"
+    endpoint = "https://" + file_links[0].split("/")[2]
     s3 = s3fs.S3FileSystem(anon=True, client_kwargs={"endpoint_url": endpoint})
     index = 0
     for link in file_links:
         file = link.split("/")[-1]
         path = link.split(endpoint)[1]
         size = s3.info(path)["size"]
         size = humanbytes(size)
@@ -98,15 +98,14 @@
 
     description = {"description": link_string, "descriptionType": "files"}
     metadata["descriptions"].append(description)
     return metadata
 
 
 def send_to_community(review_link, data, headers, publish, community, message=None):
-
     if not message:
         message = "This record is submitted automatically with the CaltechDATA API"
 
     data = {
         "receiver": {"community": community},
         "type": "community-submission",
     }
```

### Comparing `caltechdata_api-1.5.0/caltechdata_api/customize_schema.py` & `caltechdata_api-1.6.0/caltechdata_api/customize_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
                         datacite = props["datacite"]
                     individual_vocab[datacite] = entry["id"]
             vocabularies[vocab_id] = individual_vocab
     return vocabularies
 
 
 def customize_schema(json_record, schema="43"):
-
     if schema == "43":
         return customize_schema_rdm(json_record)
     else:
         raise ValueError(f"Error: We currently only support schema 43")
 
 
 def change_label(json, from_label, to_label):
@@ -130,15 +129,14 @@
             new_cre["role"] = {"id": peopleroles[cre.pop("contributorType")]}
         new_cre["person_or_org"] = cre
         new.append(new_cre)
     return new
 
 
 def customize_schema_rdm(json_record):
-
     # Get vocabularies used in InvenioRDM
     vocabularies = get_vocabularies()
 
     peopleroles = vocabularies["crr"]
     resourcetypes = vocabularies["rsrct"]
     descriptiontypes = vocabularies["dty"]
     datetypes = vocabularies["dat"]
```

### Comparing `caltechdata_api-1.5.0/caltechdata_api/download_file.py` & `caltechdata_api-1.6.0/caltechdata_api/download_file.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.5.0/caltechdata_api/get_files.py` & `caltechdata_api-1.6.0/caltechdata_api/get_files.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.5.0/caltechdata_api/get_metadata.py` & `caltechdata_api-1.6.0/caltechdata_api/get_metadata.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.5.0/caltechdata_api/utils.py` & `caltechdata_api-1.6.0/caltechdata_api/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
             # and further down in the decimals, so it doesn't matter at all.
             num /= unit_step
 
     return PRECISION_FORMATS[precision].format("-" if is_negative else "", num, unit)
 
 
 if __name__ == "__main__":
-
     print(humanbytes(2251799813685247))  # 2 pebibytes
     print(humanbytes(2000000000000000, True))  # 2 petabytes
     print(humanbytes(1099511627776))  # 1 tebibyte
     print(humanbytes(1000000000000, True))  # 1 terabyte
     print(humanbytes(1000000000, True))  # 1 gigabyte
     print(humanbytes(4318498233, precision=3))  # 4.022 gibibytes
     print(humanbytes(4318498233, True, 3))  # 4.318 gigabytes
```

### Comparing `caltechdata_api-1.5.0/caltechdata_api.egg-info/PKG-INFO` & `caltechdata_api-1.6.0/caltechdata_api.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caltechdata-api
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python wrapper for CaltechDATA API.
 Home-page: https://github.com/caltechlibrary/caltechdata_api
 Author: Thomas E Morrell
 Author-email: tmorrell@caltech.edu
 License: https://data.caltech.edu/license
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
@@ -14,46 +14,64 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# caltechdata_api
+# CaltechDATA API Python Library
 
-Python library for using the CaltechDATA API
+The `caltechdata_api` Python library provides a convenient interface for interacting with the CaltechDATA API. It allows users to write files, create DataCite 4 standard JSON records, edit existing records, and retrieve metadata from the CaltechDATA repository.
 
-- caltechdata_write write files and a DataCite 4 standard json record to CaltechDATA repository
-- caltechdata_edit edits records in CaltechDATA
-- get_metadata gets metadata from CaltechDATA records
+## Features
 
-Requires Python 3 (Recommended via Anaconda https://www.anaconda.com/download) with reqests library.
+### Writing and Editing Records
+- `caltechdata_write`: Writes files and a DataCite 4 standard JSON record to the CaltechDATA repository.
+- `caltechdata_edit`: Edits existing records in CaltechDATA.
+
+### Metadata Operations
+- `get_metadata`: Retrieves metadata from CaltechDATA records.
+
+## Requirements
+
+- Python 3 (Anaconda is recommended)
+- `requests` library
+
+## Installation
+
+Install the library via pip:
+
+```shell
+pip install caltechdata_api
+```
 
 ## Examples
 
 There are some example python scripts in the GitHub repository.
 
-Create a record:
+###Create a record:
 
 ```shell
 python write.py example.json -fnames logo.gif
-pbkn6-m9y63
+# Output: pbkn6-m9y63 (unique identifier)
 ```
-The response will be the unique identifier for the record. You can put this at
+> The response will be the unique identifier for the record. You can put this at
 the end of a url to visit the record (e.g.
 https://data.caltechlibrary.dev/records/pbkn6-m9y63)
 
-Edit a record (make changes to the example.json file to see a change)
+###Edit a record 
+Make changes to the example.json file to see a change)
 ```
 python edit.py example.json -id pbkn6-m9y63
 10.33569/pbkn6-m9y63
 ```
-The response is the DOI for the record, which includes the unique identifier
+> The response is the DOI for the record, which includes the unique identifier
 for the record in the default configuration.
 
+## Using Custom DOIs 
 Some groups have worked with the library to create custom DOIs. These can be
 passed in the metadata like:
 
 ```shell
 python write.py example_custom.json -fnames logo.gif
 m6zxz-p4j22
 ```
@@ -62,23 +80,21 @@
 ```
 python edit.py example_custom.json -id m6zxz-p4j22
 10.5281/inveniordm.1234
 ```
 
 This returns the custom DOI of the record if it is successful.
 
-## Setup 
 
-Install by typing 'pip install caltechdata_api'
+## Setup and Authentication
 
-## Usage
+1. Acquire a personal access token from your CaltechDATA account (found under "Applications" at the top right of your screen).
+2. Copy the token to a file named token.bash.
+3. Load the token in the command line using source token.bash.
 
-You need to acquire a personal access token from your CaltechDATA account
-(find it at the top right of your screen under "Applications").
-Then copy the token to token.bash.  Type `source token.bash` in 
-the command line to load the token.  
+## Note on Testing
 
-Only test your application on the test repository (data.caltechlibrary.dev).  Testing the API on the public 
+Only test your application on the test repository (`data.caltechlibrary.dev`).  Testing the API on the public 
 repository will generate junk records that are annoying to delete.
```

### Comparing `caltechdata_api-1.5.0/setup.py` & `caltechdata_api-1.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,23 @@
 download = meta["downloadUrl"]
 license = meta["license"]
 name = meta["name"]
 
 REQUIRES_PYTHON = ">=3.6.0"
 
 # What packages are required for this module to be executed?
-REQUIRED = ["requests", "datacite>1.1.0", "tqdm>=4.62.3", "pyyaml", "s3fs"]
+REQUIRED = [
+    "requests",
+    "datacite>1.1.0",
+    "tqdm>=4.62.3",
+    "pyyaml",
+    "s3fs",
+    "configparser",
+    "awscli",
+]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 files = package_files("caltechdata_api", "vocabularies")
@@ -159,8 +167,13 @@
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
     # $ setup.py publish support.
     cmdclass={
         "upload": UploadCommand,
     },
+    entry_points={
+        "console_scripts": [
+            "caltechdata_api=caltechdata_api.cli:main",
+        ],
+    },
 )
```

