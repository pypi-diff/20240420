# Comparing `tmp/predibase-api-2024.4.6.tar.gz` & `tmp/predibase-api-2024.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predibase-api-2024.4.6.tar", last modified: Thu Apr 18 20:52:44 2024, max compression
+gzip compressed data, was "predibase-api-2024.4.7.tar", last modified: Sat Apr 20 00:38:10 2024, max compression
```

## Comparing `predibase-api-2024.4.6.tar` & `predibase-api-2024.4.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:52:44.184653 predibase-api-2024.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 20:50:28.000000 predibase-api-2024.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-18 20:52:44.184653 predibase-api-2024.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-18 20:50:28.000000 predibase-api-2024.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:52:44.184653 predibase-api-2024.4.6/predibase_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:50:28.000000 predibase-api-2024.4.6/predibase_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:52:44.184653 predibase-api-2024.4.6/predibase_api/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:50:28.000000 predibase-api-2024.4.6/predibase_api/artifacts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:52:44.184653 predibase-api-2024.4.6/predibase_api/artifacts/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:50:28.000000 predibase-api-2024.4.6/predibase_api/artifacts/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-18 20:50:28.000000 predibase-api-2024.4.6/predibase_api/artifacts/v1/artifacts_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:52:44.184653 predibase-api-2024.4.6/predibase_api/foobar/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:50:28.000000 predibase-api-2024.4.6/predibase_api/foobar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:52:44.184653 predibase-api-2024.4.6/predibase_api/foobar/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:50:28.000000 predibase-api-2024.4.6/predibase_api/foobar/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-18 20:50:28.000000 predibase-api-2024.4.6/predibase_api/foobar/v1/bar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-18 20:50:28.000000 predibase-api-2024.4.6/predibase_api/foobar/v1/foo_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:52:44.184653 predibase-api-2024.4.6/predibase_api/iterml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:50:28.000000 predibase-api-2024.4.6/predibase_api/iterml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:52:44.184653 predibase-api-2024.4.6/predibase_api/iterml/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:50:28.000000 predibase-api-2024.4.6/predibase_api/iterml/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-18 20:50:28.000000 predibase-api-2024.4.6/predibase_api/iterml/v1/iterml_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:52:44.184653 predibase-api-2024.4.6/predibase_api/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:50:28.000000 predibase-api-2024.4.6/predibase_api/profiles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:52:44.184653 predibase-api-2024.4.6/predibase_api/profiles/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:50:28.000000 predibase-api-2024.4.6/predibase_api/profiles/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-04-18 20:50:28.000000 predibase-api-2024.4.6/predibase_api/profiles/v1/dataset_profile_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:52:44.184653 predibase-api-2024.4.6/predibase_api/tenants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:50:28.000000 predibase-api-2024.4.6/predibase_api/tenants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:52:44.184653 predibase-api-2024.4.6/predibase_api/tenants/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:50:28.000000 predibase-api-2024.4.6/predibase_api/tenants/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-18 20:50:28.000000 predibase-api-2024.4.6/predibase_api/tenants/v1/tenants_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:52:44.184653 predibase-api-2024.4.6/predibase_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-18 20:52:44.000000 predibase-api-2024.4.6/predibase_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-18 20:52:44.000000 predibase-api-2024.4.6/predibase_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:52:44.000000 predibase-api-2024.4.6/predibase_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:51:53.000000 predibase-api-2024.4.6/predibase_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 20:52:44.000000 predibase-api-2024.4.6/predibase_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 20:52:44.000000 predibase-api-2024.4.6/predibase_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 20:50:28.000000 predibase-api-2024.4.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:52:44.184653 predibase-api-2024.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-18 20:50:28.000000 predibase-api-2024.4.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 20:52:39.000000 predibase-api-2024.4.6/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:38:10.364692 predibase-api-2024.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-20 00:35:49.000000 predibase-api-2024.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-20 00:38:10.364692 predibase-api-2024.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-20 00:35:49.000000 predibase-api-2024.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:38:10.360692 predibase-api-2024.4.7/predibase_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:35:49.000000 predibase-api-2024.4.7/predibase_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:38:10.360692 predibase-api-2024.4.7/predibase_api/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:35:49.000000 predibase-api-2024.4.7/predibase_api/artifacts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:38:10.360692 predibase-api-2024.4.7/predibase_api/artifacts/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:35:49.000000 predibase-api-2024.4.7/predibase_api/artifacts/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-20 00:38:07.000000 predibase-api-2024.4.7/predibase_api/artifacts/v1/artifacts_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:38:10.360692 predibase-api-2024.4.7/predibase_api/foobar/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:35:49.000000 predibase-api-2024.4.7/predibase_api/foobar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:38:10.364692 predibase-api-2024.4.7/predibase_api/foobar/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:35:49.000000 predibase-api-2024.4.7/predibase_api/foobar/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-20 00:38:05.000000 predibase-api-2024.4.7/predibase_api/foobar/v1/bar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-20 00:38:04.000000 predibase-api-2024.4.7/predibase_api/foobar/v1/foo_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:38:10.364692 predibase-api-2024.4.7/predibase_api/iterml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:35:49.000000 predibase-api-2024.4.7/predibase_api/iterml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:38:10.364692 predibase-api-2024.4.7/predibase_api/iterml/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:35:49.000000 predibase-api-2024.4.7/predibase_api/iterml/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-20 00:38:08.000000 predibase-api-2024.4.7/predibase_api/iterml/v1/iterml_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:38:10.364692 predibase-api-2024.4.7/predibase_api/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:35:49.000000 predibase-api-2024.4.7/predibase_api/profiles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:38:10.364692 predibase-api-2024.4.7/predibase_api/profiles/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:35:49.000000 predibase-api-2024.4.7/predibase_api/profiles/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-04-20 00:38:09.000000 predibase-api-2024.4.7/predibase_api/profiles/v1/dataset_profile_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:38:10.364692 predibase-api-2024.4.7/predibase_api/tenants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:35:49.000000 predibase-api-2024.4.7/predibase_api/tenants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:38:10.364692 predibase-api-2024.4.7/predibase_api/tenants/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:35:49.000000 predibase-api-2024.4.7/predibase_api/tenants/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-20 00:38:06.000000 predibase-api-2024.4.7/predibase_api/tenants/v1/tenants_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:38:10.360692 predibase-api-2024.4.7/predibase_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-20 00:38:10.000000 predibase-api-2024.4.7/predibase_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-20 00:38:10.000000 predibase-api-2024.4.7/predibase_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 00:38:10.000000 predibase-api-2024.4.7/predibase_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 00:37:19.000000 predibase-api-2024.4.7/predibase_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 00:38:10.000000 predibase-api-2024.4.7/predibase_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-20 00:38:10.000000 predibase-api-2024.4.7/predibase_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 00:35:49.000000 predibase-api-2024.4.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 00:38:10.364692 predibase-api-2024.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-20 00:35:49.000000 predibase-api-2024.4.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 00:38:02.000000 predibase-api-2024.4.7/version.txt
```

### Comparing `predibase-api-2024.4.6/predibase_api/artifacts/v1/artifacts_pb2.py` & `predibase-api-2024.4.7/predibase_api/artifacts/v1/artifacts_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: predibase_api/artifacts/v1/artifacts.proto
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -14,20 +15,19 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*predibase_api/artifacts/v1/artifacts.proto\x12\x12proto.artifacts.v1\"E\n\rLudwigDataset\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05tasks\x18\x02 \x03(\t\x12\x17\n\x0f\x64\x61ta_modalities\x18\x03 \x03(\t\"P\n\x19\x41vailableDatasetsResponse\x12\x33\n\x08\x64\x61tasets\x18\x01 \x03(\x0b\x32!.proto.artifacts.v1.LudwigDataset\"\x82\x01\n\x1cPresignedUrlForUploadRequest\x12\x11\n\tmime_type\x18\x01 \x01(\t\x12\x16\n\x0e\x65xpiry_seconds\x18\x02 \x01(\x05\x12\x37\n\rartifact_type\x18\x03 \x01(\x0e\x32 .proto.artifacts.v1.ArtifactType\"\xdb\x01\n\x1dPresignedUrlForUploadResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x13\n\x0bobject_name\x18\x02 \x01(\t\x12`\n\x10required_headers\x18\x03 \x03(\x0b\x32\x46.proto.artifacts.v1.PresignedUrlForUploadResponse.RequiredHeadersEntry\x1a\x36\n\x14RequiredHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"d\n$RegisterUploadedFileAsDatasetRequest\x12\x14\n\x0c\x64\x61taset_name\x18\x01 \x01(\t\x12\x13\n\x0bobject_name\x18\x02 \x01(\t\x12\x11\n\tfile_name\x18\x03 \x01(\t*\xab\x02\n\x0c\x41rtifactType\x12\x1d\n\x19\x41RTIFACT_TYPE_UNSPECIFIED\x10\x00\x12\x1b\n\x17\x41RTIFACT_TYPE_THUMBNAIL\x10\x01\x12\x1e\n\x1a\x41RTIFACT_TYPE_QUERY_RESULT\x10\x02\x12\x19\n\x15\x41RTIFACT_TYPE_DATASET\x10\x03\x12\x1c\n\x18\x41RTIFACT_TYPE_DEPLOYMENT\x10\x04\x12\x17\n\x13\x41RTIFACT_TYPE_MODEL\x10\x05\x12\x15\n\x11\x41RTIFACT_TYPE_VIZ\x10\x06\x12\x17\n\x13\x41RTIFACT_TYPE_CACHE\x10\x07\x12\x1b\n\x17\x41RTIFACT_TYPE_WORKSPACE\x10\x08\x12 \n\x1c\x41RTIFACT_TYPE_EXPORTED_MODEL\x10\tB1Z/github.com/predibase/predibase_api/artifacts/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'predibase_api.artifacts.v1.artifacts_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z/github.com/predibase/predibase_api/artifacts/v1'
-  _PRESIGNEDURLFORUPLOADRESPONSE_REQUIREDHEADERSENTRY._options = None
-  _PRESIGNEDURLFORUPLOADRESPONSE_REQUIREDHEADERSENTRY._serialized_options = b'8\001'
+if not _descriptor._USE_C_DESCRIPTORS:
+  _globals['DESCRIPTOR']._loaded_options = None
+  _globals['DESCRIPTOR']._serialized_options = b'Z/github.com/predibase/predibase_api/artifacts/v1'
+  _globals['_PRESIGNEDURLFORUPLOADRESPONSE_REQUIREDHEADERSENTRY']._loaded_options = None
+  _globals['_PRESIGNEDURLFORUPLOADRESPONSE_REQUIREDHEADERSENTRY']._serialized_options = b'8\001'
   _globals['_ARTIFACTTYPE']._serialized_start=677
   _globals['_ARTIFACTTYPE']._serialized_end=976
   _globals['_LUDWIGDATASET']._serialized_start=66
   _globals['_LUDWIGDATASET']._serialized_end=135
   _globals['_AVAILABLEDATASETSRESPONSE']._serialized_start=137
   _globals['_AVAILABLEDATASETSRESPONSE']._serialized_end=217
   _globals['_PRESIGNEDURLFORUPLOADREQUEST']._serialized_start=220
```

### Comparing `predibase-api-2024.4.6/predibase_api/foobar/v1/bar_pb2.py` & `predibase-api-2024.4.7/predibase_api/foobar/v1/bar_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: predibase_api/foobar/v1/bar.proto
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -14,14 +15,13 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!predibase_api/foobar/v1/bar.proto\x12\x06\x66oobar\"\x13\n\x03\x42\x61r\x12\x0c\n\x04name\x18\x01 \x01(\tB\"Z github.com/predibase/api/test/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'predibase_api.foobar.v1.bar_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z github.com/predibase/api/test/v1'
+if not _descriptor._USE_C_DESCRIPTORS:
+  _globals['DESCRIPTOR']._loaded_options = None
+  _globals['DESCRIPTOR']._serialized_options = b'Z github.com/predibase/api/test/v1'
   _globals['_BAR']._serialized_start=45
   _globals['_BAR']._serialized_end=64
 # @@protoc_insertion_point(module_scope)
```

### Comparing `predibase-api-2024.4.6/predibase_api/foobar/v1/foo_pb2.py` & `predibase-api-2024.4.7/predibase_api/foobar/v1/foo_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: predibase_api/foobar/v1/foo.proto
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,14 +16,13 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!predibase_api/foobar/v1/foo.proto\x12\x06\x66oobar\x1a!predibase_api/foobar/v1/bar.proto\"\x1f\n\x03\x46oo\x12\x18\n\x03\x62\x61r\x18\x01 \x01(\x0b\x32\x0b.foobar.BarB\"Z github.com/predibase/api/test/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'predibase_api.foobar.v1.foo_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z github.com/predibase/api/test/v1'
+if not _descriptor._USE_C_DESCRIPTORS:
+  _globals['DESCRIPTOR']._loaded_options = None
+  _globals['DESCRIPTOR']._serialized_options = b'Z github.com/predibase/api/test/v1'
   _globals['_FOO']._serialized_start=80
   _globals['_FOO']._serialized_end=111
 # @@protoc_insertion_point(module_scope)
```

### Comparing `predibase-api-2024.4.6/predibase_api/iterml/v1/iterml_pb2.py` & `predibase-api-2024.4.7/predibase_api/iterml/v1/iterml_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: predibase_api/iterml/v1/iterml.proto
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -14,18 +15,17 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$predibase_api/iterml/v1/iterml.proto\x12\x0fproto.iterml.v1\"\xd4\x01\n\x15RecommendedExperiment\x12\x17\n\x0f\x62\x61se_model_uuid\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12!\n\x19model_version_description\x18\x04 \x01(\t\x12\x1e\n\x16new_config_json_string\x18\x05 \x01(\t\x12;\n\x11parameter_changes\x18\x06 \x03(\x0b\x32 .proto.iterml.v1.ParameterChange\"d\n\x19RecommendedExperimentList\x12G\n\x17recommended_experiments\x18\x01 \x03(\x0b\x32&.proto.iterml.v1.RecommendedExperiment\"j\n\x0fParameterChange\x12\x16\n\x0eparameter_name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\x16\n\x0eoriginal_value\x18\x03 \x01(\t\x12\x11\n\tnew_value\x18\x04 \x01(\tB.Z,github.com/predibase/predibase_api/iterml/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'predibase_api.iterml.v1.iterml_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z,github.com/predibase/predibase_api/iterml/v1'
+if not _descriptor._USE_C_DESCRIPTORS:
+  _globals['DESCRIPTOR']._loaded_options = None
+  _globals['DESCRIPTOR']._serialized_options = b'Z,github.com/predibase/predibase_api/iterml/v1'
   _globals['_RECOMMENDEDEXPERIMENT']._serialized_start=58
   _globals['_RECOMMENDEDEXPERIMENT']._serialized_end=270
   _globals['_RECOMMENDEDEXPERIMENTLIST']._serialized_start=272
   _globals['_RECOMMENDEDEXPERIMENTLIST']._serialized_end=372
   _globals['_PARAMETERCHANGE']._serialized_start=374
   _globals['_PARAMETERCHANGE']._serialized_end=480
 # @@protoc_insertion_point(module_scope)
```

### Comparing `predibase-api-2024.4.6/predibase_api/profiles/v1/dataset_profile_pb2.py` & `predibase-api-2024.4.7/predibase_api/profiles/v1/dataset_profile_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: predibase_api/profiles/v1/dataset_profile.proto
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -14,24 +15,23 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/predibase_api/profiles/v1/dataset_profile.proto\x12\x0f\x64\x61taset_profile\"\x8b\x02\n\x0e\x44\x61tasetProfile\x12\x11\n\ttimestamp\x18\x01 \x01(\x05\x12\x14\n\x0cnum_examples\x18\x02 \x01(\x05\x12\x12\n\nsize_bytes\x18\x03 \x01(\x01\x12\x13\n\x0bnum_samples\x18\x04 \x01(\x05\x12N\n\x10\x66\x65\x61ture_profiles\x18\x32 \x03(\x0b\x32\x34.dataset_profile.DatasetProfile.FeatureProfilesEntry\x1aW\n\x14\x46\x65\x61tureProfilesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12.\n\x05value\x18\x02 \x01(\x0b\x32\x1f.dataset_profile.FeatureProfile:\x02\x38\x01\"\xc0\x06\n\x0e\x46\x65\x61tureProfile\x12\x14\n\x0c\x66\x65\x61ture_name\x18\x01 \x01(\t\x12\x14\n\x0csource_dtype\x18\x02 \x01(\t\x12\x15\n\rshould_enable\x18\x03 \x01(\x08\x12\x1f\n\x17should_enable_reasoning\x18\x04 \x01(\t\x12\x15\n\rinferred_type\x18\x05 \x01(\t\x12\x1f\n\x17inferred_type_reasoning\x18\x06 \x01(\t\x12\x61\n\x1a\x61lternative_inferred_types\x18\x07 \x03(\x0b\x32=.dataset_profile.FeatureProfile.AlternativeInferredTypesEntry\x12P\n\x11\x63ross_correlation\x18\x08 \x03(\x0b\x32\x35.dataset_profile.FeatureProfile.CrossCorrelationEntry\x12>\n\x11per_sample_tokens\x18\t \x01(\x0b\x32#.dataset_profile.NumberDistribution\x12\x43\n\x15type_agnostic_profile\x18\x32 \x01(\x0b\x32$.dataset_profile.TypeAgnosticProfile\x12\x36\n\x0e\x62inary_profile\x18\x33 \x01(\x0b\x32\x1e.dataset_profile.BinaryProfile\x12\x36\n\x0enumber_profile\x18\x34 \x01(\x0b\x32\x1e.dataset_profile.NumberProfile\x12:\n\x10\x63\x61tegory_profile\x18\x35 \x01(\x0b\x32 .dataset_profile.CategoryProfile\x12\x32\n\x0ctext_profile\x18\x36 \x01(\x0b\x32\x1c.dataset_profile.TextProfile\x1a?\n\x1d\x41lternativeInferredTypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x37\n\x15\x43rossCorrelationEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01:\x02\x38\x01\"\xe8\x01\n\x13TypeAgnosticProfile\x12#\n\x16percent_missing_values\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\"\n\x15percent_unique_values\x18\x02 \x01(\x01H\x01\x88\x01\x01\x12\x1e\n\x11num_unique_values\x18\x03 \x01(\x05H\x02\x88\x01\x01\x12\x1d\n\x15sampled_unique_values\x18\x04 \x03(\tB\x19\n\x17_percent_missing_valuesB\x18\n\x16_percent_unique_valuesB\x14\n\x12_num_unique_values\"\x9e\x01\n\rBinaryProfile\x12\x12\n\ntrue_label\x18\x01 \x01(\t\x12\x13\n\x0b\x66\x61lse_label\x18\x02 \x01(\t\x12\x14\n\x0cpercent_true\x18\x03 \x01(\x01\x12\x15\n\rpercent_false\x18\x04 \x01(\x01\x12\x17\n\x0fimbalance_ratio\x18\x05 \x01(\x01\x12\x1e\n\x16\x61re_conventional_bools\x18\x06 \x01(\x08\"J\n\rNumberProfile\x12\x39\n\x0c\x64istribution\x18\x01 \x01(\x0b\x32#.dataset_profile.NumberDistribution\"*\n\x0cHistogramBin\x12\x0b\n\x03\x62in\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\x05\"\x88\x02\n\x12NumberDistribution\x12\x0c\n\x04mean\x18\x01 \x01(\x01\x12\r\n\x05stdev\x18\x02 \x01(\x01\x12\x0b\n\x03min\x18\x03 \x01(\x01\x12\n\n\x02p1\x18\x04 \x01(\x01\x12\n\n\x02p5\x18\x05 \x01(\x01\x12\x0b\n\x03p10\x18\x06 \x01(\x01\x12\x0b\n\x03p25\x18\x07 \x01(\x01\x12\x0e\n\x06median\x18\x08 \x01(\x01\x12\x0b\n\x03p75\x18\t \x01(\x01\x12\x0b\n\x03p95\x18\n \x01(\x01\x12\x0b\n\x03p99\x18\x0b \x01(\x01\x12\x0b\n\x03max\x18\x0c \x01(\x01\x12\x35\n\x0ehistogram_bins\x18\x14 \x03(\x0b\x32\x1d.dataset_profile.HistogramBin\x12\x1b\n\x13percentage_outliers\x18\x15 \x01(\x01\"\xac\x02\n\x0f\x43\x61tegoryProfile\x12:\n\x13most_frequent_items\x18\x01 \x03(\x0b\x32\x1d.dataset_profile.FrequentItem\x12;\n\x14least_frequent_items\x18\x02 \x03(\x0b\x32\x1d.dataset_profile.FrequentItem\x12\x39\n\x12\x61ll_frequent_items\x18\x05 \x03(\x0b\x32\x1d.dataset_profile.FrequentItem\x12\x1f\n\x17majority_minority_ratio\x18\x03 \x01(\x01\x12\x44\n\x17percentage_distribution\x18\x04 \x01(\x0b\x32#.dataset_profile.NumberDistribution\"9\n\x0c\x46requentItem\x12\r\n\x05label\x18\x01 \x01(\t\x12\x1a\n\x12percent_occurrence\x18\x02 \x01(\x01\"o\n\x0bTextProfile\x12\x19\n\x11\x64\x65tected_language\x18\x01 \x01(\t\x12\x45\n\x18word_length_distribution\x18\x02 \x01(\x0b\x32#.dataset_profile.NumberDistribution\"\xb3\x01\n\x0b\x44\x61teProfile\x12\x15\n\rearliest_date\x18\x01 \x01(\t\x12\x13\n\x0blatest_date\x18\x02 \x01(\t\x12\x38\n\x0f\x64\x61te_resolution\x18\x03 \x01(\x0e\x32\x1f.dataset_profile.DateResolution\x12>\n\x11\x64\x61te_distribution\x18\x04 \x01(\x0b\x32#.dataset_profile.NumberDistribution*\xd4\x01\n\x0e\x44\x61teResolution\x12\x1f\n\x1b\x44\x41TE_RESOLUTION_UNSPECIFIED\x10\x00\x12\x18\n\x14\x44\x41TE_RESOLUTION_YEAR\x10\x01\x12\x19\n\x15\x44\x41TE_RESOLUTION_MONTH\x10\x02\x12\x17\n\x13\x44\x41TE_RESOLUTION_DAY\x10\x03\x12\x19\n\x15\x44\x41TE_RESOLUTION_HOURS\x10\x04\x12\x1b\n\x17\x44\x41TE_RESOLUTION_MINUTES\x10\x05\x12\x1b\n\x17\x44\x41TE_RESOLUTION_SECONDS\x10\x06\x42\x30Z.github.com/predibase/predibase_api/profiles/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'predibase_api.profiles.v1.dataset_profile_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z.github.com/predibase/predibase_api/profiles/v1'
-  _DATASETPROFILE_FEATUREPROFILESENTRY._options = None
-  _DATASETPROFILE_FEATUREPROFILESENTRY._serialized_options = b'8\001'
-  _FEATUREPROFILE_ALTERNATIVEINFERREDTYPESENTRY._options = None
-  _FEATUREPROFILE_ALTERNATIVEINFERREDTYPESENTRY._serialized_options = b'8\001'
-  _FEATUREPROFILE_CROSSCORRELATIONENTRY._options = None
-  _FEATUREPROFILE_CROSSCORRELATIONENTRY._serialized_options = b'8\001'
+if not _descriptor._USE_C_DESCRIPTORS:
+  _globals['DESCRIPTOR']._loaded_options = None
+  _globals['DESCRIPTOR']._serialized_options = b'Z.github.com/predibase/predibase_api/profiles/v1'
+  _globals['_DATASETPROFILE_FEATUREPROFILESENTRY']._loaded_options = None
+  _globals['_DATASETPROFILE_FEATUREPROFILESENTRY']._serialized_options = b'8\001'
+  _globals['_FEATUREPROFILE_ALTERNATIVEINFERREDTYPESENTRY']._loaded_options = None
+  _globals['_FEATUREPROFILE_ALTERNATIVEINFERREDTYPESENTRY']._serialized_options = b'8\001'
+  _globals['_FEATUREPROFILE_CROSSCORRELATIONENTRY']._loaded_options = None
+  _globals['_FEATUREPROFILE_CROSSCORRELATIONENTRY']._serialized_options = b'8\001'
   _globals['_DATERESOLUTION']._serialized_start=2614
   _globals['_DATERESOLUTION']._serialized_end=2826
   _globals['_DATASETPROFILE']._serialized_start=69
   _globals['_DATASETPROFILE']._serialized_end=336
   _globals['_DATASETPROFILE_FEATUREPROFILESENTRY']._serialized_start=249
   _globals['_DATASETPROFILE_FEATUREPROFILESENTRY']._serialized_end=336
   _globals['_FEATUREPROFILE']._serialized_start=339
```

### Comparing `predibase-api-2024.4.6/predibase_api/tenants/v1/tenants_pb2.py` & `predibase-api-2024.4.7/predibase_api/tenants/v1/tenants_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: predibase_api/tenants/v1/tenants.proto
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,20 +16,19 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&predibase_api/tenants/v1/tenants.proto\x12\x16proto.internal.tenants\x1a\x1egoogle/protobuf/duration.proto\"\xd4\x02\n\x13\x43reateTenantRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rbilling_email\x18\x02 \x01(\t\x12\x43\n\x11subscription_tier\x18\x03 \x01(\x0e\x32(.proto.internal.tenants.SubscriptionTier\x12\x36\n\x13subscription_length\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x1d\n\x15subscription_is_trial\x18\x07 \x01(\x08\x12\x41\n\x10\x65nvironment_type\x18\x05 \x01(\x0e\x32\'.proto.internal.tenants.EnvironmentType\x12#\n\x1b\x63reate_predibase_admin_user\x18\x06 \x01(\x08\x12\x14\n\x0c\x63loud_region\x18\x08 \x01(\t\"\xc7\x01\n\x14\x43reateTenantResponse\x12\x13\n\x0btenant_name\x18\x01 \x01(\t\x12\x13\n\x0btenant_uuid\x18\x02 \x01(\t\x12\x18\n\x10tenant_shortcode\x18\x03 \x01(\t\x12\x18\n\x10user_invite_link\x18\x04 \x01(\t\x12\x1d\n\x15predibase_admin_email\x18\x05 \x01(\t\x12\x14\n\x0c\x63loud_region\x18\x06 \x01(\t\x12\x1c\n\x14predibase_admin_uuid\x18\x07 \x01(\t\"2\n\tTenantRef\x12\x0e\n\x04uuid\x18\x01 \x01(\tH\x00\x12\x0f\n\x05\x64\x62_id\x18\x02 \x01(\x04H\x00\x42\x04\n\x02id*\xe3\x01\n\x10SubscriptionTier\x12!\n\x1dSUBSCRIPTION_TIER_UNSPECIFIED\x10\x00\x12\x1a\n\x16SUBSCRIPTION_TIER_FREE\x10\x01\x12\x1d\n\x19SUBSCRIPTION_TIER_PREMIUM\x10\x02\x12%\n!SUBSCRIPTION_TIER_ENTERPRISE_SAAS\x10\x04\x12$\n SUBSCRIPTION_TIER_ENTERPRISE_VPC\x10\x05\x12$\n\x1cSUBSCRIPTION_TIER_ENTERPRISE\x10\x03\x1a\x02\x08\x01*\x8d\x01\n\x0f\x45nvironmentType\x12 \n\x1c\x45NVIRONMENT_TYPE_UNSPECIFIED\x10\x00\x12 \n\x1c\x45NVIRONMENT_TYPE_SHARED_SAAS\x10\x01\x12\x18\n\x14\x45NVIRONMENT_TYPE_VPC\x10\x02\x12\x1c\n\x18\x45NVIRONMENT_TYPE_ON_PREM\x10\x03\x42%Z#github.com/predibase/api/tenants/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'predibase_api.tenants.v1.tenants_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z#github.com/predibase/api/tenants/v1'
-  _SUBSCRIPTIONTIER.values_by_name["SUBSCRIPTION_TIER_ENTERPRISE"]._options = None
-  _SUBSCRIPTIONTIER.values_by_name["SUBSCRIPTION_TIER_ENTERPRISE"]._serialized_options = b'\010\001'
+if not _descriptor._USE_C_DESCRIPTORS:
+  _globals['DESCRIPTOR']._loaded_options = None
+  _globals['DESCRIPTOR']._serialized_options = b'Z#github.com/predibase/api/tenants/v1'
+  _globals['_SUBSCRIPTIONTIER'].values_by_name["SUBSCRIPTION_TIER_ENTERPRISE"]._loaded_options = None
+  _globals['_SUBSCRIPTIONTIER'].values_by_name["SUBSCRIPTION_TIER_ENTERPRISE"]._serialized_options = b'\010\001'
   _globals['_SUBSCRIPTIONTIER']._serialized_start=696
   _globals['_SUBSCRIPTIONTIER']._serialized_end=923
   _globals['_ENVIRONMENTTYPE']._serialized_start=926
   _globals['_ENVIRONMENTTYPE']._serialized_end=1067
   _globals['_CREATETENANTREQUEST']._serialized_start=99
   _globals['_CREATETENANTREQUEST']._serialized_end=439
   _globals['_CREATETENANTRESPONSE']._serialized_start=442
```

### Comparing `predibase-api-2024.4.6/predibase_api.egg-info/SOURCES.txt` & `predibase-api-2024.4.7/predibase_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.6/setup.py` & `predibase-api-2024.4.7/setup.py`

 * *Files identical despite different names*

