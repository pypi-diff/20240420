# Comparing `tmp/easy_sqla_lib-1.1.0.tar.gz` & `tmp/easy_sqla_lib-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_sqla_lib-1.1.0.tar", max compression
+gzip compressed data, was "easy_sqla_lib-2.0.0.tar", max compression
```

## Comparing `easy_sqla_lib-1.1.0.tar` & `easy_sqla_lib-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     4776 2024-04-01 03:13:38.515287 easy_sqla_lib-1.1.0/README.md
--rw-r--r--   0        0        0     6148 2024-04-01 03:13:38.515287 easy_sqla_lib-1.1.0/easy_sqla/.DS_Store
--rw-r--r--   0        0        0        0 2024-04-01 03:13:38.515287 easy_sqla_lib-1.1.0/easy_sqla/__init__.py
--rw-r--r--   0        0        0     3040 2024-04-01 03:13:38.515287 easy_sqla_lib-1.1.0/easy_sqla/context.py
--rw-r--r--   0        0        0        0 2024-04-01 03:13:38.515287 easy_sqla_lib-1.1.0/easy_sqla/db/__init__.py
--rw-r--r--   0        0        0     2327 2024-04-01 03:13:38.515287 easy_sqla_lib-1.1.0/easy_sqla/db/operators.py
--rw-r--r--   0        0        0    11141 2024-04-01 03:13:38.515287 easy_sqla_lib-1.1.0/easy_sqla/db/query.py
--rw-r--r--   0        0        0       28 2024-04-01 03:13:38.519287 easy_sqla_lib-1.1.0/easy_sqla/db/selector.py
--rw-r--r--   0        0        0      691 2024-04-01 03:13:38.519287 easy_sqla_lib-1.1.0/easy_sqla/db/settings.py
--rw-r--r--   0        0        0      180 2024-04-01 03:13:38.519287 easy_sqla_lib-1.1.0/easy_sqla/exceptions.py
--rw-r--r--   0        0        0       93 2024-04-01 03:13:38.519287 easy_sqla_lib-1.1.0/easy_sqla/logger.py
--rw-r--r--   0        0        0    10348 2024-04-01 03:13:38.519287 easy_sqla_lib-1.1.0/easy_sqla/manager.py
--rw-r--r--   0        0        0     5458 2024-04-01 03:13:38.519287 easy_sqla_lib-1.1.0/easy_sqla/utils.py
--rw-r--r--   0        0        0     1203 2024-04-01 03:13:38.519287 easy_sqla_lib-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       20 2024-04-01 03:13:38.519287 easy_sqla_lib-1.1.0/tests/.coveragerc
--rw-r--r--   0        0        0       71 2024-04-01 03:13:38.519287 easy_sqla_lib-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0      429 2024-04-01 03:13:38.519287 easy_sqla_lib-1.1.0/tests/base_model.py
--rw-r--r--   0        0        0      446 2024-04-01 03:13:38.519287 easy_sqla_lib-1.1.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-01 03:13:38.519287 easy_sqla_lib-1.1.0/tests/db/__init__.py
--rw-r--r--   0        0        0      261 2024-04-01 03:13:38.519287 easy_sqla_lib-1.1.0/tests/db/test_operators.py
--rw-r--r--   0        0        0     3588 2024-04-01 03:13:38.519287 easy_sqla_lib-1.1.0/tests/db/test_query.py
--rw-r--r--   0        0        0      109 2024-04-01 03:13:38.519287 easy_sqla_lib-1.1.0/tests/db/test_settings.py
--rw-r--r--   0        0        0     2342 2024-04-01 03:13:38.519287 easy_sqla_lib-1.1.0/tests/models.py
--rw-r--r--   0        0        0        0 2024-04-01 03:13:38.519287 easy_sqla_lib-1.1.0/tests/test_context.py
--rw-r--r--   0        0        0     3618 2024-04-01 03:13:38.519287 easy_sqla_lib-1.1.0/tests/test_manager.py
--rw-r--r--   0        0        0     2121 2024-04-01 03:13:38.519287 easy_sqla_lib-1.1.0/tests/test_utils.py
--rw-r--r--   0        0        0     5905 1970-01-01 00:00:00.000000 easy_sqla_lib-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4776 2024-03-11 12:55:18.343520 easy_sqla_lib-2.0.0/README.md
+-rw-r--r--   0        0        0     6148 2024-03-11 12:55:18.343791 easy_sqla_lib-2.0.0/easy_sqla/.DS_Store
+-rw-r--r--   0        0        0        0 2024-03-11 12:55:18.343882 easy_sqla_lib-2.0.0/easy_sqla/__init__.py
+-rw-r--r--   0        0        0     3040 2024-04-20 08:23:02.888399 easy_sqla_lib-2.0.0/easy_sqla/context.py
+-rw-r--r--   0        0        0        0 2024-03-11 12:55:18.344563 easy_sqla_lib-2.0.0/easy_sqla/db/__init__.py
+-rw-r--r--   0        0        0     2413 2024-03-11 12:55:18.344805 easy_sqla_lib-2.0.0/easy_sqla/db/operators.py
+-rw-r--r--   0        0        0    11141 2024-03-12 20:50:28.260570 easy_sqla_lib-2.0.0/easy_sqla/db/query.py
+-rw-r--r--   0        0        0       28 2024-03-11 12:55:18.345260 easy_sqla_lib-2.0.0/easy_sqla/db/selector.py
+-rw-r--r--   0        0        0      701 2024-04-20 11:08:51.146881 easy_sqla_lib-2.0.0/easy_sqla/db/settings.py
+-rw-r--r--   0        0        0      180 2024-03-11 12:55:18.345646 easy_sqla_lib-2.0.0/easy_sqla/exceptions.py
+-rw-r--r--   0        0        0       93 2024-03-11 12:55:18.345828 easy_sqla_lib-2.0.0/easy_sqla/logger.py
+-rw-r--r--   0        0        0    10348 2024-03-12 20:50:28.261873 easy_sqla_lib-2.0.0/easy_sqla/manager.py
+-rw-r--r--   0        0        0     5458 2024-03-11 12:55:18.346344 easy_sqla_lib-2.0.0/easy_sqla/utils.py
+-rw-r--r--   0        0        0     1037 2024-04-20 11:56:09.451540 easy_sqla_lib-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       20 2024-03-11 12:55:18.347945 easy_sqla_lib-2.0.0/tests/.coveragerc
+-rw-r--r--   0        0        0       71 2024-03-12 20:50:28.265429 easy_sqla_lib-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      429 2024-03-11 12:55:18.348322 easy_sqla_lib-2.0.0/tests/base_model.py
+-rw-r--r--   0        0        0      446 2024-03-11 12:55:18.348564 easy_sqla_lib-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-11 12:55:18.348897 easy_sqla_lib-2.0.0/tests/db/__init__.py
+-rw-r--r--   0        0        0      261 2024-03-11 12:55:18.349146 easy_sqla_lib-2.0.0/tests/db/test_operators.py
+-rw-r--r--   0        0        0     3588 2024-03-11 12:55:18.349515 easy_sqla_lib-2.0.0/tests/db/test_query.py
+-rw-r--r--   0        0        0      109 2024-03-11 12:55:18.349795 easy_sqla_lib-2.0.0/tests/db/test_settings.py
+-rw-r--r--   0        0        0     2342 2024-03-11 12:55:18.350031 easy_sqla_lib-2.0.0/tests/models.py
+-rw-r--r--   0        0        0        0 2024-03-11 12:55:18.350123 easy_sqla_lib-2.0.0/tests/test_context.py
+-rw-r--r--   0        0        0     3618 2024-03-11 12:55:18.350341 easy_sqla_lib-2.0.0/tests/test_manager.py
+-rw-r--r--   0        0        0     2121 2024-03-11 12:55:18.350620 easy_sqla_lib-2.0.0/tests/test_utils.py
+-rw-r--r--   0        0        0     5560 1970-01-01 00:00:00.000000 easy_sqla_lib-2.0.0/PKG-INFO
```

### Comparing `easy_sqla_lib-1.1.0/README.md` & `easy_sqla_lib-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `easy_sqla_lib-1.1.0/easy_sqla/.DS_Store` & `easy_sqla_lib-2.0.0/easy_sqla/.DS_Store`

 * *Files identical despite different names*

### Comparing `easy_sqla_lib-1.1.0/easy_sqla/context.py` & `easy_sqla_lib-2.0.0/easy_sqla/context.py`

 * *Files identical despite different names*

### Comparing `easy_sqla_lib-1.1.0/easy_sqla/db/query.py` & `easy_sqla_lib-2.0.0/easy_sqla/db/query.py`

 * *Files identical despite different names*

### Comparing `easy_sqla_lib-1.1.0/easy_sqla/db/settings.py` & `easy_sqla_lib-2.0.0/easy_sqla/db/settings.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from enum import Enum
 from typing import Optional
 
-from pydantic import BaseSettings
-from pydantic import PyObject
+from pydantic import Field
+from pydantic.v1 import BaseSettings, PyObject
 
 
 class DriverEnum(str, Enum):
     SQLITE = "sqlite"
     MYSQL = "mysql"
     POSTGRES = "postgresql"
```

### Comparing `easy_sqla_lib-1.1.0/easy_sqla/manager.py` & `easy_sqla_lib-2.0.0/easy_sqla/manager.py`

 * *Files identical despite different names*

### Comparing `easy_sqla_lib-1.1.0/easy_sqla/utils.py` & `easy_sqla_lib-2.0.0/easy_sqla/utils.py`

 * *Files identical despite different names*

### Comparing `easy_sqla_lib-1.1.0/tests/db/test_query.py` & `easy_sqla_lib-2.0.0/tests/db/test_query.py`

 * *Files identical despite different names*

### Comparing `easy_sqla_lib-1.1.0/tests/models.py` & `easy_sqla_lib-2.0.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `easy_sqla_lib-1.1.0/tests/test_manager.py` & `easy_sqla_lib-2.0.0/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `easy_sqla_lib-1.1.0/tests/test_utils.py` & `easy_sqla_lib-2.0.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `easy_sqla_lib-1.1.0/PKG-INFO` & `easy_sqla_lib-2.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 Metadata-Version: 2.1
 Name: easy-sqla-lib
-Version: 1.1.0
+Version: 2.0.0
 Summary: A wrapper on top of sqlalchemy that allow to make django orm style query
 License: GNU GPLv3
 Author: Soumaila Kouriba
 Author-email: admin@softmali.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: SQLAlchemy (>=1.4.41,<2.0.0)
-Requires-Dist: cfgv (>=3.3.1,<4.0.0)
-Requires-Dist: distlib (>=0.3.6,<0.4.0)
-Requires-Dist: filelock (>=3.8.0,<4.0.0)
-Requires-Dist: greenlet (>=1.1.3,<2.0.0)
-Requires-Dist: identify (>=2.5.5,<3.0.0)
-Requires-Dist: nodeenv (>=1.7.0,<2.0.0)
-Requires-Dist: platformdirs (>=2.5.2,<3.0.0)
+Requires-Dist: SQLAlchemy (>=2,<3)
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: typing-extensions (>=4.3.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Description
 
 Easy-sqla-lib is a Python library intended to make beautiful SQLAlchemy query syntax.
 
 SQLAlchemy is an awesome and powerful ORM which mades interaction with database very painless. However powerful, sometime mean complex to use.
```

