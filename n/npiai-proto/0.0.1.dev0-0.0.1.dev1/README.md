# Comparing `tmp/npiai_proto-0.0.1.dev0.tar.gz` & `tmp/npiai_proto-0.0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npiai_proto-0.0.1.dev0.tar", max compression
+gzip compressed data, was "npiai_proto-0.0.1.dev1.tar", max compression
```

## Comparing `npiai_proto-0.0.1.dev0.tar` & `npiai_proto-0.0.1.dev1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       30 2024-04-19 21:33:34.559893 npiai_proto-0.0.1.dev0/README.md
--rw-r--r--   0        0        0     5859 2024-04-19 21:50:03.347460 npiai_proto-0.0.1.dev0/npiai_proto/api_pb2.py
--rw-r--r--   0        0        0     7203 2024-04-19 21:50:03.347674 npiai_proto-0.0.1.dev0/npiai_proto/api_pb2.pyi
--rw-r--r--   0        0        0     3822 2024-04-19 21:50:03.347806 npiai_proto-0.0.1.dev0/npiai_proto/api_pb2_grpc.py
--rw-r--r--   0        0        0      567 2024-04-20 00:06:50.790767 npiai_proto-0.0.1.dev0/pyproject.toml
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 npiai_proto-0.0.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0       30 2024-04-19 21:33:34.559893 npiai_proto-0.0.1.dev1/README.md
+-rw-r--r--   0        0        0     5859 2024-04-19 21:50:03.347460 npiai_proto-0.0.1.dev1/npiai_proto/api_pb2.py
+-rw-r--r--   0        0        0     7203 2024-04-19 21:50:03.347674 npiai_proto-0.0.1.dev1/npiai_proto/api_pb2.pyi
+-rw-r--r--   0        0        0     3822 2024-04-19 21:50:03.347806 npiai_proto-0.0.1.dev1/npiai_proto/api_pb2_grpc.py
+-rw-r--r--   0        0        0      567 2024-04-20 01:03:28.950666 npiai_proto-0.0.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 npiai_proto-0.0.1.dev1/PKG-INFO
```

### Comparing `npiai_proto-0.0.1.dev0/npiai_proto/api_pb2.py` & `npiai_proto-0.0.1.dev1/npiai_proto/api_pb2.py`

 * *Files identical despite different names*

### Comparing `npiai_proto-0.0.1.dev0/npiai_proto/api_pb2.pyi` & `npiai_proto-0.0.1.dev1/npiai_proto/api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `npiai_proto-0.0.1.dev0/npiai_proto/api_pb2_grpc.py` & `npiai_proto-0.0.1.dev1/npiai_proto/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `npiai_proto-0.0.1.dev0/pyproject.toml` & `npiai_proto-0.0.1.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "npiai-proto"
-version = "v0.0.1.dev0"
+version = "v0.0.1.dev1"
 description = "The NPI.AI Proto"
 license = "Apache-2.0"
 authors = ["Wells Wang <wells@npi.ai>"]
 readme = "README.md"
 homepage = "https://github.com/npi-ai/proto/python"
 repository = "https://github.com/npi-ai/proto/python"
 packages = [
```

### Comparing `npiai_proto-0.0.1.dev0/PKG-INFO` & `npiai_proto-0.0.1.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npiai-proto
-Version: 0.0.1.dev0
+Version: 0.0.1.dev1
 Summary: The NPI.AI Proto
 Home-page: https://github.com/npi-ai/proto/python
 License: Apache-2.0
 Author: Wells Wang
 Author-email: wells@npi.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

