# Comparing `tmp/aracnid_api-2.1.1.tar.gz` & `tmp/aracnid_api-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aracnid_api-2.1.1.tar", max compression
+gzip compressed data, was "aracnid_api-2.2.0.tar", max compression
```

## Comparing `aracnid_api-2.1.1.tar` & `aracnid_api-2.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1079 2024-01-28 16:08:27.919049 aracnid_api-2.1.1/LICENSE
--rw-r--r--   0        0        0      976 2024-01-28 16:08:27.919049 aracnid_api-2.1.1/README.md
--rw-r--r--   0        0        0      136 2024-01-28 16:08:27.919049 aracnid_api-2.1.1/aracnid_api/__init__.py
--rw-r--r--   0        0        0     5566 2024-01-28 16:08:27.919049 aracnid_api-2.1.1/aracnid_api/i_airtable.py
--rw-r--r--   0        0        0      732 2024-01-28 16:08:27.919049 aracnid_api-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     1804 1970-01-01 00:00:00.000000 aracnid_api-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-20 11:26:40.939240 aracnid_api-2.2.0/LICENSE
+-rw-r--r--   0        0        0      976 2024-04-20 11:26:40.939240 aracnid_api-2.2.0/README.md
+-rw-r--r--   0        0        0      136 2024-04-20 11:26:40.939240 aracnid_api-2.2.0/aracnid_api/__init__.py
+-rw-r--r--   0        0        0     6084 2024-04-20 11:26:40.939240 aracnid_api-2.2.0/aracnid_api/i_airtable.py
+-rw-r--r--   0        0        0      712 2024-04-20 11:26:40.939240 aracnid_api-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 aracnid_api-2.2.0/PKG-INFO
```

### Comparing `aracnid_api-2.1.1/LICENSE` & `aracnid_api-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aracnid_api-2.1.1/README.md` & `aracnid_api-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aracnid_api-2.1.1/aracnid_api/i_airtable.py` & `aracnid_api-2.2.0/aracnid_api/i_airtable.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Class module to interface with Airtable.
 """
+# pylint: disable=logging-too-many-args
 import os
 
 from aracnid_logger import Logger
 from dateutil.parser import parse
-from pyairtable import Table
+from pyairtable import Api, Table
 from pyairtable.formulas import match
 
 
 # initialize logging
 logger = Logger(__name__).get_logger()
 
 
@@ -30,17 +31,36 @@
 
         Args:
             base_id: The identifier of the Airtable base.
         """
         # read environment variables
         self.air_api_key = os.environ.get('AIRTABLE_API_KEY')
 
+        # initialize api
+        self.api = Api(self.air_api_key)
+
         # set the base id for the interface
         self.base_id = base_id
 
+        # retrieve the base
+        bases = self.api.bases()
+        self.base = None
+        for base in bases:
+            if base.id == self.base_id:
+                self.base = base
+                break
+
+    def get_base_name(self) -> str:
+        """Returns the name of the Base
+
+        Returns:
+            str: Name of the Base.
+        """
+        return self.base.name
+
     def get_table(self, table_name):
         """Returns the specified Airtable table.
 
         Args:
             table_name: The name of the table in the Airtable Base.
         """
         table = Table(self.air_api_key, self.base_id, table_name)
@@ -67,16 +87,17 @@
                 field_val = record['fields'][field_name]
 
             if isinstance(field_val, list):
                 if len(field_val) == 1:
                     field_val = field_val[0]
                 else:
                     if not suppress_warnings:
-                        logger.warning(f'{field_name} has multiple values: '
-                            f'{field_val}')
+                        logger.warning(
+                            '%s has multiple values: %s', field_name, field_val
+                        )
 
         return field_val
 
     @staticmethod
     def get_airtable_list(record, field_name, default=None):
         """Retrieves a list from an Airtable record field.
```

### Comparing `aracnid_api-2.1.1/pyproject.toml` & `aracnid_api-2.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "aracnid-api"
-version = "2.1.1"
+version = "2.2.0"
 description = "This package contains custom wrappers around a variety of Web App APIs."
 authors = ["Jason Romano <aracnid@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/aracnid/aracnid-api"
 keywords = ["api", "airtable"]
 packages = [{include = "aracnid_api"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aracnid-logger = "^1.0"
-pyairtable = "^1.4.0"
+pyairtable = "^2.3"
 python-dateutil = "2.8.2"
-pylint = "^3.0.3"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^3.0"
 pytest = "^7.2"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `aracnid_api-2.1.1/PKG-INFO` & `aracnid_api-2.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: aracnid-api
-Version: 2.1.1
+Version: 2.2.0
 Summary: This package contains custom wrappers around a variety of Web App APIs.
 Home-page: https://github.com/aracnid/aracnid-api
 License: MIT
 Keywords: api,airtable
 Author: Jason Romano
 Author-email: aracnid@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aracnid-logger (>=1.0,<2.0)
-Requires-Dist: pyairtable (>=1.4.0,<2.0.0)
-Requires-Dist: pylint (>=3.0.3,<4.0.0)
+Requires-Dist: pyairtable (>=2.3,<3.0)
 Requires-Dist: python-dateutil (==2.8.2)
 Project-URL: Repository, https://github.com/aracnid/aracnid-api
 Description-Content-Type: text/markdown
 
 # Aracnid API
 
 This package contains custom wrappers around a variety of Web App APIs.
```

