# Comparing `tmp/types-protobuf-4.25.0.20240410.tar.gz` & `tmp/types-protobuf-4.25.0.20240417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-protobuf-4.25.0.20240410.tar", last modified: Wed Apr 10 02:15:07 2024, max compression
+gzip compressed data, was "types-protobuf-4.25.0.20240417.tar", last modified: Wed Apr 17 02:17:03 2024, max compression
```

## Comparing `types-protobuf-4.25.0.20240410.tar` & `types-protobuf-4.25.0.20240417.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:15:07.936002 types-protobuf-4.25.0.20240410/
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-04-10 02:15:06.000000 types-protobuf-4.25.0.20240410/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-10 02:15:06.000000 types-protobuf-4.25.0.20240410/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-10 02:15:07.936002 types-protobuf-4.25.0.20240410/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:15:07.928002 types-protobuf-4.25.0.20240410/google-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-10 02:15:06.000000 types-protobuf-4.25.0.20240410/google-stubs/METADATA.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:15:07.932002 types-protobuf-4.25.0.20240410/google-stubs/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/any_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/api_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:15:07.932002 types-protobuf-4.25.0.20240410/google-stubs/protobuf/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/compiler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/compiler/plugin_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/descriptor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   105834 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/descriptor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/descriptor_pool.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/duration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/empty_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/field_mask_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:15:07.936002 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/api_implementation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/builder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/decoder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/encoder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/enum_type_wrapper.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/extension_dict.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/message_listener.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/python_message.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/type_checkers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/well_known_types.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/wire_format.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/json_format.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/message.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/message_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 02:15:06.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/reflection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/source_context_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/struct_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/symbol_database.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/text_format.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/timestamp_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16542 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/type_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:15:07.936002 types-protobuf-4.25.0.20240410/google-stubs/protobuf/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/util/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/wrappers_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 02:15:07.936002 types-protobuf-4.25.0.20240410/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-10 02:15:06.000000 types-protobuf-4.25.0.20240410/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:15:07.936002 types-protobuf-4.25.0.20240410/types_protobuf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-10 02:15:07.000000 types-protobuf-4.25.0.20240410/types_protobuf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-10 02:15:07.000000 types-protobuf-4.25.0.20240410/types_protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 02:15:07.000000 types-protobuf-4.25.0.20240410/types_protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 02:15:07.000000 types-protobuf-4.25.0.20240410/types_protobuf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:03.077165 types-protobuf-4.25.0.20240417/
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-04-17 02:17:02.000000 types-protobuf-4.25.0.20240417/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 02:17:02.000000 types-protobuf-4.25.0.20240417/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-17 02:17:03.077165 types-protobuf-4.25.0.20240417/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:03.073166 types-protobuf-4.25.0.20240417/google-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-17 02:17:02.000000 types-protobuf-4.25.0.20240417/google-stubs/METADATA.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:03.077165 types-protobuf-4.25.0.20240417/google-stubs/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/any_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/api_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:03.077165 types-protobuf-4.25.0.20240417/google-stubs/protobuf/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/compiler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/compiler/plugin_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/descriptor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   105834 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/descriptor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/descriptor_pool.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/duration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/empty_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/field_mask_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:03.077165 types-protobuf-4.25.0.20240417/google-stubs/protobuf/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/internal/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/internal/api_implementation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/internal/builder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/internal/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/internal/decoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/internal/encoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/internal/enum_type_wrapper.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/internal/extension_dict.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/internal/message_listener.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/internal/python_message.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/internal/type_checkers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/internal/well_known_types.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/internal/wire_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/json_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/message.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/message_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 02:17:02.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/reflection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/source_context_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/struct_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/symbol_database.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/text_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/timestamp_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16542 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/type_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:03.077165 types-protobuf-4.25.0.20240417/google-stubs/protobuf/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/util/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-17 02:16:41.000000 types-protobuf-4.25.0.20240417/google-stubs/protobuf/wrappers_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:17:03.077165 types-protobuf-4.25.0.20240417/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-17 02:17:02.000000 types-protobuf-4.25.0.20240417/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:03.077165 types-protobuf-4.25.0.20240417/types_protobuf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-17 02:17:03.000000 types-protobuf-4.25.0.20240417/types_protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-17 02:17:03.000000 types-protobuf-4.25.0.20240417/types_protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:17:03.000000 types-protobuf-4.25.0.20240417/types_protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 02:17:03.000000 types-protobuf-4.25.0.20240417/types_protobuf.egg-info/top_level.txt
```

### Comparing `types-protobuf-4.25.0.20240410/CHANGELOG.md` & `types-protobuf-4.25.0.20240417/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 4.25.0.20240417 (2024-04-17)
+
+Remove remaining bare `Incomplete`s (#11768)
+
+Enable Y065
+
 ## 4.25.0.20240410 (2024-04-10)
 
 Bump protobuf to v25.3 (#11694)
 
 ## 4.24.0.20240408 (2024-04-08)
 
 Bump protobuf to v24.4 and update generator script (#11693)
```

### Comparing `types-protobuf-4.25.0.20240410/PKG-INFO` & `types-protobuf-4.25.0.20240417/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-protobuf
-Version: 4.25.0.20240410
+Version: 4.25.0.20240417
 Summary: Typing stubs for protobuf
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/protobuf.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -34,10 +34,10 @@
 Generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) on [protobuf v25.3](https://github.com/protocolbuffers/protobuf/releases/tag/v25.3) (python protobuf==4.25.3)
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1af2babc03ca0cbd248f5f2044e68311a671595f` and was tested
-with mypy 1.9.0, pyright 1.1.357, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/any_pb2.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/any_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/api_pb2.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/compiler/plugin_pb2.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/compiler/plugin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/descriptor.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/descriptor.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/descriptor_pb2.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/descriptor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/descriptor_pool.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/descriptor_pool.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/duration_pb2.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/duration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/empty_pb2.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/empty_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/field_mask_pb2.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/field_mask_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/containers.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/internal/containers.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/decoder.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/internal/decoder.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/encoder.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/internal/encoder.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/enum_type_wrapper.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/internal/enum_type_wrapper.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/extension_dict.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/internal/extension_dict.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/well_known_types.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/internal/well_known_types.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,18 @@
 from typing_extensions import TypeAlias
 
 from google.protobuf import struct_pb2
 
 class Any:
     type_url: str
     value: Incomplete
-    def Pack(
-        self, msg: Incomplete, type_url_prefix: str = "type.googleapis.com/", deterministic: Incomplete | None = None
-    ) -> None: ...
-    def Unpack(self, msg: Incomplete) -> bool: ...
+    def Pack(self, msg, type_url_prefix: str = "type.googleapis.com/", deterministic: Incomplete | None = None) -> None: ...
+    def Unpack(self, msg) -> bool: ...
     def TypeName(self) -> str: ...
-    def Is(self, descriptor: Incomplete) -> bool: ...
+    def Is(self, descriptor) -> bool: ...
 
 class Timestamp:
     def ToJsonString(self) -> str: ...
     seconds: int
     nanos: int
     def FromJsonString(self, value: str) -> None: ...
     def GetCurrentTime(self) -> None: ...
```

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/wire_format.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/internal/wire_format.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/json_format.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/json_format.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/message.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/message.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/message_factory.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/message_factory.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/service.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/service.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/source_context_pb2.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/source_context_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/struct_pb2.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/struct_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/symbol_database.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/symbol_database.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/text_format.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/text_format.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/timestamp_pb2.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/timestamp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/type_pb2.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/google-stubs/protobuf/wrappers_pb2.pyi` & `types-protobuf-4.25.0.20240417/google-stubs/protobuf/wrappers_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.25.0.20240410/setup.py` & `types-protobuf-4.25.0.20240417/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 Generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) on [protobuf v25.3](https://github.com/protocolbuffers/protobuf/releases/tag/v25.3) (python protobuf==4.25.3)
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1af2babc03ca0cbd248f5f2044e68311a671595f` and was tested
-with mypy 1.9.0, pyright 1.1.357, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="4.25.0.20240410",
+      version="4.25.0.20240417",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/protobuf.md",
```

### Comparing `types-protobuf-4.25.0.20240410/types_protobuf.egg-info/PKG-INFO` & `types-protobuf-4.25.0.20240417/types_protobuf.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-protobuf
-Version: 4.25.0.20240410
+Version: 4.25.0.20240417
 Summary: Typing stubs for protobuf
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/protobuf.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -34,10 +34,10 @@
 Generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) on [protobuf v25.3](https://github.com/protocolbuffers/protobuf/releases/tag/v25.3) (python protobuf==4.25.3)
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1af2babc03ca0cbd248f5f2044e68311a671595f` and was tested
-with mypy 1.9.0, pyright 1.1.357, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-protobuf-4.25.0.20240410/types_protobuf.egg-info/SOURCES.txt` & `types-protobuf-4.25.0.20240417/types_protobuf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

