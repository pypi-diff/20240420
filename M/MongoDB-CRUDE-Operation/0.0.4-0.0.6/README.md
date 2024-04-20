# Comparing `tmp/mongodb_crude_operation-0.0.4.tar.gz` & `tmp/mongodb_crude_operation-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodb_crude_operation-0.0.4.tar", last modified: Fri Apr 19 18:22:00 2024, max compression
+gzip compressed data, was "mongodb_crude_operation-0.0.6.tar", last modified: Fri Apr 19 18:46:12 2024, max compression
```

## Comparing `mongodb_crude_operation-0.0.4.tar` & `mongodb_crude_operation-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:22:00.200437 mongodb_crude_operation-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-19 18:22:00.200437 mongodb_crude_operation-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-19 18:21:56.000000 mongodb_crude_operation-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 18:21:56.000000 mongodb_crude_operation-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-19 18:22:00.200437 mongodb_crude_operation-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-19 18:21:56.000000 mongodb_crude_operation-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:22:00.196437 mongodb_crude_operation-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:22:00.200437 mongodb_crude_operation-0.0.4/src/MongoDB_CRUDE_Operation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-19 18:22:00.000000 mongodb_crude_operation-0.0.4/src/MongoDB_CRUDE_Operation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-19 18:22:00.000000 mongodb_crude_operation-0.0.4/src/MongoDB_CRUDE_Operation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:22:00.000000 mongodb_crude_operation-0.0.4/src/MongoDB_CRUDE_Operation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-19 18:22:00.000000 mongodb_crude_operation-0.0.4/src/MongoDB_CRUDE_Operation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 18:22:00.000000 mongodb_crude_operation-0.0.4/src/MongoDB_CRUDE_Operation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:22:00.200437 mongodb_crude_operation-0.0.4/src/mongodb_connect/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 18:21:56.000000 mongodb_crude_operation-0.0.4/src/mongodb_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-19 18:21:56.000000 mongodb_crude_operation-0.0.4/src/mongodb_connect/mongo_crud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:46:12.431886 mongodb_crude_operation-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-19 18:46:12.431886 mongodb_crude_operation-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-19 18:46:08.000000 mongodb_crude_operation-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 18:46:08.000000 mongodb_crude_operation-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-19 18:46:12.431886 mongodb_crude_operation-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-19 18:46:08.000000 mongodb_crude_operation-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:46:12.427886 mongodb_crude_operation-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:46:12.431886 mongodb_crude_operation-0.0.6/src/MongoDB_CRUDE_Operation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-19 18:46:12.000000 mongodb_crude_operation-0.0.6/src/MongoDB_CRUDE_Operation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-19 18:46:12.000000 mongodb_crude_operation-0.0.6/src/MongoDB_CRUDE_Operation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:46:12.000000 mongodb_crude_operation-0.0.6/src/MongoDB_CRUDE_Operation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-19 18:46:12.000000 mongodb_crude_operation-0.0.6/src/MongoDB_CRUDE_Operation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 18:46:12.000000 mongodb_crude_operation-0.0.6/src/MongoDB_CRUDE_Operation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:46:12.431886 mongodb_crude_operation-0.0.6/src/mongodb_connect/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 18:46:08.000000 mongodb_crude_operation-0.0.6/src/mongodb_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-19 18:46:08.000000 mongodb_crude_operation-0.0.6/src/mongodb_connect/mongo_crud.py
```

### Comparing `mongodb_crude_operation-0.0.4/PKG-INFO` & `mongodb_crude_operation-0.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MongoDB_CRUDE_Operation
-Version: 0.0.4
+Version: 0.0.6
 Summary: A python package for connecting with database.
 Home-page: https://github.com/AM-Ankitgit/MongdbPyPI_Package
 Author: AM-Ankitgit
 Author-email: mahalleankit@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/AM-Ankitgit/MongdbPyPI_Package/issues
 Classifier: Programming Language :: Python :: 3.7
@@ -17,39 +17,83 @@
 Provides-Extra: testing
 Requires-Dist: pytest>=7.1.3; extra == "testing"
 Requires-Dist: mypy>=0.971; extra == "testing"
 Requires-Dist: flake8>=5.0.4; extra == "testing"
 Requires-Dist: tox>=3.25.1; extra == "testing"
 Requires-Dist: black>=22.8.0; extra == "testing"
 
-# requirements_dev.txt we use for the testing
+# `Description:`
+
+mongo-operation is a Python library for simplifying MongoDB operations by providing an easy-to-use interface. This library allows users to perform common MongoDB tasks such as creating a client, database, or collection, as well as inserting records into collections and bulk inserting data from CSV or Excel files.
+
+# `Features:`
+
+MongoClient Creation: Easily create a MongoDB client with a given URL.
+Database and Collection Management: Create databases and collections with ease, and automatically handle re-creating them if they already exist.
+Insertion Operations: Insert records into MongoDB collections, whether it's a single record or bulk data from CSV or Excel files.
+
+
+# `Example Usage:`
+
+`python code`
+
+from MongoDB_CRUDE_Operation.mongodb_connect.mongo_crud import  mongo_operation
+
+Initialize MongoDB connection
+client_url = "mongodb://localhost:27017/"
+database_name = "mydatabase"
+collection_name = "mycollection"
+
+mongo_op = mongo_operation(client_url, database_name, collection_name)
+
+Insert a single record
+record = {"name": "John", "age": 30}
+mongo_op.insert_record(record, collection_name)
+
+Bulk insert data from CSV or Excel file
+datafile = "data.csv"
+mongo_op.bulk_insert(datafile, collection_name)
+
+## `Requirements:`
+
+Python 3.x
+pandas
+pymongo
+ensure
+
+
+
+
+
+
+### requirements_dev.txt we use for the testing
 It makes it easier to install and manage dependencies for development and testing, separate from the dependencies required for production.
 
-# difference between requirements_dev.txt and requirements.txt
+### difference between requirements_dev.txt and requirements.txt
 
 requirements.txt is used to specify the dependencies required to run the production code of a Python project, while requirements_dev.txt is used to specify the dependencies required for development and testing purposes.
 
-# tox.ini
+### tox.ini
 We use if for the testing in the python package testing against different version of the python 
 
-## how tox works tox enviornment creation
+### how tox works tox enviornment creation
 1. Install depedencies and packages 
 2. Run commands
 3. Its a combination of the (virtualenvwrapper and makefile)
 4. It creates a .tox
 
 
-# pyproject.toml
+### pyproject.toml
 it is being used for configuration the python project it is a alternative of the setup.cfg file. its containts configuration related to the build system
 such as the build tool used package name version author license and dependencies
 
-# setup.cfg
+### setup.cfg
 In summary, setup.cfg is used by setuptools to configure the packaging and installation of a Python projec
 
-# Testing python application
+### Testing python application
 *types of testing*
 1. Automated testing 
 2. Manual testing
 
 *Mode of testing*
 1. Unit testing
 2. Integration tests
@@ -59,13 +103,13 @@
 1. pytest
 2. unittest
 3. robotframework
 4. selenium
 5. behave
 6. doctest
 
-# check with the code style formatting and syntax(coding standard)
+### check with the code style formatting and syntax(coding standard)
 
 1. pylint
 2. flake8(it is best because it containt 3 library pylint pycodestyle mccabe)
 3. pycodestyle
```

### Comparing `mongodb_crude_operation-0.0.4/setup.cfg` & `mongodb_crude_operation-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `mongodb_crude_operation-0.0.4/setup.py` & `mongodb_crude_operation-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     return requirements'''
 
    
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()     
    
 
-__version__ = "v0.0.4"
+__version__ = "v0.0.6"
 REPO_NAME = "MongdbPyPI_Package"
 PKG_NAME= "MongoDB_CRUDE_Operation"
 AUTHOR_USER_NAME = "AM-Ankitgit"
 
 AUTHOR_EMAIL = "mahalleankit@gmail.com"
 
 setup(
```

### Comparing `mongodb_crude_operation-0.0.4/src/MongoDB_CRUDE_Operation.egg-info/PKG-INFO` & `mongodb_crude_operation-0.0.6/src/MongoDB_CRUDE_Operation.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MongoDB_CRUDE_Operation
-Version: 0.0.4
+Version: 0.0.6
 Summary: A python package for connecting with database.
 Home-page: https://github.com/AM-Ankitgit/MongdbPyPI_Package
 Author: AM-Ankitgit
 Author-email: mahalleankit@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/AM-Ankitgit/MongdbPyPI_Package/issues
 Classifier: Programming Language :: Python :: 3.7
@@ -17,39 +17,83 @@
 Provides-Extra: testing
 Requires-Dist: pytest>=7.1.3; extra == "testing"
 Requires-Dist: mypy>=0.971; extra == "testing"
 Requires-Dist: flake8>=5.0.4; extra == "testing"
 Requires-Dist: tox>=3.25.1; extra == "testing"
 Requires-Dist: black>=22.8.0; extra == "testing"
 
-# requirements_dev.txt we use for the testing
+# `Description:`
+
+mongo-operation is a Python library for simplifying MongoDB operations by providing an easy-to-use interface. This library allows users to perform common MongoDB tasks such as creating a client, database, or collection, as well as inserting records into collections and bulk inserting data from CSV or Excel files.
+
+# `Features:`
+
+MongoClient Creation: Easily create a MongoDB client with a given URL.
+Database and Collection Management: Create databases and collections with ease, and automatically handle re-creating them if they already exist.
+Insertion Operations: Insert records into MongoDB collections, whether it's a single record or bulk data from CSV or Excel files.
+
+
+# `Example Usage:`
+
+`python code`
+
+from MongoDB_CRUDE_Operation.mongodb_connect.mongo_crud import  mongo_operation
+
+Initialize MongoDB connection
+client_url = "mongodb://localhost:27017/"
+database_name = "mydatabase"
+collection_name = "mycollection"
+
+mongo_op = mongo_operation(client_url, database_name, collection_name)
+
+Insert a single record
+record = {"name": "John", "age": 30}
+mongo_op.insert_record(record, collection_name)
+
+Bulk insert data from CSV or Excel file
+datafile = "data.csv"
+mongo_op.bulk_insert(datafile, collection_name)
+
+## `Requirements:`
+
+Python 3.x
+pandas
+pymongo
+ensure
+
+
+
+
+
+
+### requirements_dev.txt we use for the testing
 It makes it easier to install and manage dependencies for development and testing, separate from the dependencies required for production.
 
-# difference between requirements_dev.txt and requirements.txt
+### difference between requirements_dev.txt and requirements.txt
 
 requirements.txt is used to specify the dependencies required to run the production code of a Python project, while requirements_dev.txt is used to specify the dependencies required for development and testing purposes.
 
-# tox.ini
+### tox.ini
 We use if for the testing in the python package testing against different version of the python 
 
-## how tox works tox enviornment creation
+### how tox works tox enviornment creation
 1. Install depedencies and packages 
 2. Run commands
 3. Its a combination of the (virtualenvwrapper and makefile)
 4. It creates a .tox
 
 
-# pyproject.toml
+### pyproject.toml
 it is being used for configuration the python project it is a alternative of the setup.cfg file. its containts configuration related to the build system
 such as the build tool used package name version author license and dependencies
 
-# setup.cfg
+### setup.cfg
 In summary, setup.cfg is used by setuptools to configure the packaging and installation of a Python projec
 
-# Testing python application
+### Testing python application
 *types of testing*
 1. Automated testing 
 2. Manual testing
 
 *Mode of testing*
 1. Unit testing
 2. Integration tests
@@ -59,13 +103,13 @@
 1. pytest
 2. unittest
 3. robotframework
 4. selenium
 5. behave
 6. doctest
 
-# check with the code style formatting and syntax(coding standard)
+### check with the code style formatting and syntax(coding standard)
 
 1. pylint
 2. flake8(it is best because it containt 3 library pylint pycodestyle mccabe)
 3. pycodestyle
```

### Comparing `mongodb_crude_operation-0.0.4/src/mongodb_connect/mongo_crud.py` & `mongodb_crude_operation-0.0.6/src/mongodb_connect/mongo_crud.py`

 * *Files identical despite different names*

