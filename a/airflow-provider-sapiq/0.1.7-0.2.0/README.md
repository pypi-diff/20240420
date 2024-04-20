# Comparing `tmp/airflow_provider_sapiq-0.1.7.tar.gz` & `tmp/airflow_provider_sapiq-0.2.0.tar.gz`

## Comparing `airflow_provider_sapiq-0.1.7.tar` & `airflow_provider_sapiq-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.1.7/requirements.txt
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.1.7/src/airflow_provider_sapiq/__about__.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.1.7/src/airflow_provider_sapiq/__init__.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.1.7/src/airflow_provider_sapiq/get_provider_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.1.7/src/airflow_provider_sapiq/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.1.7/src/airflow_provider_sapiq/hooks/__init__.py
--rw-r--r--   0        0        0     5112 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.1.7/src/airflow_provider_sapiq/hooks/sapiq.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.1.7/src/airflow_provider_sapiq/operators/__init__.py
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.1.7/src/airflow_provider_sapiq/operators/sapiq.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.1.7/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.1.7/LICENSE.txt
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.1.7/README.md
--rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.2.0/requirements.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.2.0/src/airflow_provider_sapiq/__about__.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.2.0/src/airflow_provider_sapiq/__init__.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.2.0/src/airflow_provider_sapiq/get_provider_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.2.0/src/airflow_provider_sapiq/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.2.0/src/airflow_provider_sapiq/hooks/__init__.py
+-rw-r--r--   0        0        0     5112 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.2.0/src/airflow_provider_sapiq/hooks/sapiq.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.2.0/src/airflow_provider_sapiq/operators/__init__.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.2.0/src/airflow_provider_sapiq/operators/sapiq.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.2.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.2.0/README.md
+-rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 airflow_provider_sapiq-0.2.0/PKG-INFO
```

### Comparing `airflow_provider_sapiq-0.1.7/src/airflow_provider_sapiq/get_provider_info.py` & `airflow_provider_sapiq-0.2.0/src/airflow_provider_sapiq/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `airflow_provider_sapiq-0.1.7/src/airflow_provider_sapiq/hooks/sapiq.py` & `airflow_provider_sapiq-0.2.0/src/airflow_provider_sapiq/hooks/sapiq.py`

 * *Files identical despite different names*

### Comparing `airflow_provider_sapiq-0.1.7/src/airflow_provider_sapiq/operators/sapiq.py` & `airflow_provider_sapiq-0.2.0/src/airflow_provider_sapiq/operators/sapiq.py`

 * *Files identical despite different names*

### Comparing `airflow_provider_sapiq-0.1.7/.gitignore` & `airflow_provider_sapiq-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `airflow_provider_sapiq-0.1.7/LICENSE.txt` & `airflow_provider_sapiq-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `airflow_provider_sapiq-0.1.7/README.md` & `airflow_provider_sapiq-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `airflow_provider_sapiq-0.1.7/pyproject.toml` & `airflow_provider_sapiq-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `airflow_provider_sapiq-0.1.7/PKG-INFO` & `airflow_provider_sapiq-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: airflow-provider-sapiq
-Version: 0.1.7
+Version: 0.2.0
 Summary: SAP IQ provider for Apache Airflow
 Project-URL: Documentation, https://github.com/ask1/airflow-provider-sapiq#readme
 Project-URL: Issues, https://github.com/ask1/airflow-provider-sapiq/issues
 Project-URL: Source, https://github.com/ask1/airflow-provider-sapiq
 Author: Anatoli Skovpen
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

