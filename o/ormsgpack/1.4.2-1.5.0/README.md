# Comparing `tmp/ormsgpack-1.4.2.tar.gz` & `tmp/ormsgpack-1.5.0.tar.gz`

## Comparing `ormsgpack-1.4.2.tar` & `ormsgpack-1.5.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     2046 1970-01-01 00:00:00.000000 ormsgpack-1.4.2/Cargo.toml
--rw-r--r--   0     1001      127     5815 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/CHANGELOG.md
--rw-r--r--   0     1001      127    10847 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/LICENSE-APACHE
--rw-r--r--   0     1001      127     1023 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/LICENSE-MIT
--rw-r--r--   0     1001      127    40974 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/README.md
--rw-r--r--   0     1001      127      111 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/build.rs
--rw-r--r--   0     1001      127     1176 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/deserialize/cache.rs
--rw-r--r--   0     1001      127    16357 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/deserialize/deserializer.rs
--rw-r--r--   0     1001      127      301 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/deserialize/error.rs
--rw-r--r--   0     1001      127      205 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/deserialize/mod.rs
--rw-r--r--   0     1001      127      578 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/exc.rs
--rw-r--r--   0     1001      127     2207 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/ext.rs
--rw-r--r--   0     1001      127     2393 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/ffi.rs
--rw-r--r--   0     1001      127    10133 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/lib.rs
--rw-r--r--   0     1001      127     1082 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/opt.rs
--rw-r--r--   0     1001      127      743 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/serialize/bytes.rs
--rw-r--r--   0     1001      127     6190 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/serialize/dataclass.rs
--rw-r--r--   0     1001      127     9531 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/serialize/datetime.rs
--rw-r--r--   0     1001      127     2315 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/serialize/default.rs
--rw-r--r--   0     1001      127     8286 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/serialize/dict.rs
--rw-r--r--   0     1001      127     1093 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/serialize/ext.rs
--rw-r--r--   0     1001      127     1143 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/serialize/int.rs
--rw-r--r--   0     1001      127     1536 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/serialize/list.rs
--rw-r--r--   0     1001      127      241 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/serialize/mod.rs
--rw-r--r--   0     1001      127    18628 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/serialize/numpy.rs
--rw-r--r--   0     1001      127    10795 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/serialize/serializer.rs
--rw-r--r--   0     1001      127     1250 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/serialize/str.rs
--rw-r--r--   0     1001      127     1523 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/serialize/tuple.rs
--rw-r--r--   0     1001      127     1945 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/serialize/uuid.rs
--rw-r--r--   0     1001      127     5293 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/serialize/writer.rs
--rw-r--r--   0     1001      127    10433 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/typeref.rs
--rw-r--r--   0     1001      127     5589 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/unicode.rs
--rw-r--r--   0     1001      127     2651 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/src/util.rs
--rw-r--r--   0     1001      127    10891 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/Cargo.lock
--rw-r--r--   0     1001      127     1181 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/pyproject.toml
--rw-r--r--   0     1001      127      558 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/python/ormsgpack/__init__.py
--rw-r--r--   0     1001      127      754 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/python/ormsgpack/__init__.pyi
--rw-r--r--   0     1001      127        0 2024-01-28 16:57:47.000000 ormsgpack-1.4.2/python/ormsgpack/py.typed
--rw-r--r--   0        0        0    42501 1970-01-01 00:00:00.000000 ormsgpack-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     2066 1970-01-01 00:00:00.000000 ormsgpack-1.5.0/Cargo.toml
+-rw-r--r--   0     1001      127     5976 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/CHANGELOG.md
+-rw-r--r--   0     1001      127    10847 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1023 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/LICENSE-MIT
+-rw-r--r--   0     1001      127    42381 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/README.md
+-rw-r--r--   0     1001      127      111 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/build.rs
+-rw-r--r--   0     1001      127     1176 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/deserialize/cache.rs
+-rw-r--r--   0     1001      127    15283 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/deserialize/deserializer.rs
+-rw-r--r--   0     1001      127      301 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/deserialize/error.rs
+-rw-r--r--   0     1001      127      205 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/deserialize/mod.rs
+-rw-r--r--   0     1001      127      351 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/exc.rs
+-rw-r--r--   0     1001      127     2219 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/ext.rs
+-rw-r--r--   0     1001      127     2393 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/ffi.rs
+-rw-r--r--   0     1001      127    10133 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/lib.rs
+-rw-r--r--   0     1001      127     1082 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/opt.rs
+-rw-r--r--   0     1001      127      703 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/serialize/bytes.rs
+-rw-r--r--   0     1001      127     6694 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/serialize/dataclass.rs
+-rw-r--r--   0     1001      127     5598 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/serialize/datetime.rs
+-rw-r--r--   0     1001      127     4512 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/serialize/datetimelike.rs
+-rw-r--r--   0     1001      127     2265 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/serialize/default.rs
+-rw-r--r--   0     1001      127     8288 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/serialize/dict.rs
+-rw-r--r--   0     1001      127     1057 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/serialize/ext.rs
+-rw-r--r--   0     1001      127     1103 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/serialize/int.rs
+-rw-r--r--   0     1001      127     1383 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/serialize/list.rs
+-rw-r--r--   0     1001      127      259 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/serialize/mod.rs
+-rw-r--r--   0     1001      127    27519 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/serialize/numpy.rs
+-rw-r--r--   0     1001      127    10505 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/serialize/serializer.rs
+-rw-r--r--   0     1001      127     1170 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/serialize/str.rs
+-rw-r--r--   0     1001      127     1410 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/serialize/tuple.rs
+-rw-r--r--   0     1001      127     1945 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/serialize/uuid.rs
+-rw-r--r--   0     1001      127     2331 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/serialize/writer.rs
+-rw-r--r--   0     1001      127    11112 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/typeref.rs
+-rw-r--r--   0     1001      127     5589 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/unicode.rs
+-rw-r--r--   0     1001      127     2651 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/src/util.rs
+-rw-r--r--   0     1001      127    11339 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/Cargo.lock
+-rw-r--r--   0     1001      127     1203 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/pyproject.toml
+-rw-r--r--   0     1001      127        0 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/python/ormsgpack/py.typed
+-rw-r--r--   0     1001      127      926 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/python/ormsgpack/__init__.py
+-rw-r--r--   0     1001      127      754 2024-04-19 16:39:09.000000 ormsgpack-1.5.0/python/ormsgpack/__init__.pyi
+-rw-r--r--   0        0        0    43908 1970-01-01 00:00:00.000000 ormsgpack-1.5.0/PKG-INFO
```

### Comparing `ormsgpack-1.4.2/Cargo.toml` & `ormsgpack-1.5.0/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [package]
 name = "ormsgpack"
-version = "1.4.2"
+version = "1.5.0"
 authors = [
     "Aviram Hassan <aviramyhassan@gmail.com>",
     "Emanuele Giaquinta <emanuele.giaquinta@gmail.com>",
 ]
 description = "Fast, correct Python msgpack library supporting dataclasses, datetimes, and numpy"
-edition = "2018"
+edition = "2021"
 license = "Apache-2.0 OR MIT"
 repository = "https://github.com/aviramha/ormsgpack"
 homepage = "https://github.com/aviramha/ormsgpack"
 readme = "README.md"
 keywords = ["fast", "msgpack", "dataclass", "dataclasses", "datetime"]
 include = [
     "build.rs",
@@ -33,30 +33,31 @@
 # Use SIMD intrinsics. This requires Rust on the nightly channel.
 unstable-simd = [
     "bytecount/generic-simd",
     "encoding_rs/simd-accel",
 ]
 
 [dependencies]
-ahash = { version = "0.8", default_features = false }
-associative-cache = { version = "2", default_features = false }
-bytecount = { version = "^0.6.7", default_features = false, features = ["runtime-dispatch-simd"] }
-encoding_rs = { version = "0.8", default_features = false }
-itoa = { version = "1", default_features = false }
-once_cell = { version = "1", default_features = false, features = ["race"] }
-pyo3 = { version = "^0.20.2", default_features = false, features = ["extension-module"] }
-rmp = { version = "^0.8.10", default_features = false, features = ["std"] }
-rmp-serde = { version = "1", default_features = false }
-serde = { version = "1", default_features = false }
-serde_bytes = { version = "0.11.14", default_features = false, features = ["std"] }
-simdutf8 = { version = "0.1", default_features = false, features = ["std", "aarch64_neon"] }
-smallvec = { version = "^1.13", default_features = false, features = ["union", "write"] }
+ahash = { version = "0.8", default-features = false }
+associative-cache = { version = "2", default-features = false }
+bytecount = { version = "^0.6.7", default-features = false, features = ["runtime-dispatch-simd"] }
+chrono = { version = "0.4.38", default-features = false }
+encoding_rs = { version = "0.8", default-features = false }
+half = { version = "2.4.1", default-features = false }
+itoa = { version = "1", default-features = false }
+once_cell = { version = "1", default-features = false, features = ["race"] }
+pyo3 = { version = "^0.21.2", default-features = false, features = ["extension-module"] }
+rmp = { version = "^0.8.14", default-features = false, features = ["std"] }
+rmp-serde = { version = "1", default-features = false }
+serde = { version = "1", default-features = false }
+serde_bytes = { version = "0.11.14", default-features = false, features = ["std"] }
+smallvec = { version = "^1.13", default-features = false, features = ["union", "write"] }
 
 [build-dependencies]
-pyo3-build-config = { version = "^0.20.0" }
+pyo3-build-config = { version = "^0.21.0" }
 
 [profile.release]
 codegen-units = 1
 debug = false
 incremental = false
 lto = "thin"
 opt-level = 3
```

### Comparing `ormsgpack-1.4.2/CHANGELOG.md` & `ormsgpack-1.5.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## 1.5.0 19/04/2024
+
+- Add support for numpy datetime64 and float16 types
+- Optimize serialization of dataclasses
+- Optimize deserialization of arrays and maps
+
 ## 1.4.2 28/01/2024
 
 ### Fixed
 
 - Fix crash on termination with Python 3.11 (#223)
 
 ### Changed
```

### Comparing `ormsgpack-1.4.2/LICENSE-APACHE` & `ormsgpack-1.5.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.4.2/LICENSE-MIT` & `ormsgpack-1.5.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.4.2/README.md` & `ormsgpack-1.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -68,19 +68,19 @@
 ### Quickstart
 
 This is an example of serializing, with options specified, and deserializing:
 
 ```python
 >>> import ormsgpack, datetime, numpy
 >>> data = {
-    "type": "job",
-    "created_at": datetime.datetime(1970, 1, 1),
-    "status": "🆗",
-    "payload": numpy.array([[1, 2], [3, 4]]),
-}
+...     "type": "job",
+...     "created_at": datetime.datetime(1970, 1, 1),
+...     "status": "🆗",
+...     "payload": numpy.array([[1, 2], [3, 4]]),
+... }
 >>> ormsgpack.packb(data, option=ormsgpack.OPT_NAIVE_UTC | ormsgpack.OPT_SERIALIZE_NUMPY)
 b'\x84\xa4type\xa3job\xaacreated_at\xb91970-01-01T00:00:00+00:00\xa6status\xa4\xf0\x9f\x86\x97\xa7payload\x92\x92\x01\x02\x92\x03\x04'
 >>> ormsgpack.unpackb(_)
 {'type': 'job', 'created_at': '1970-01-01T00:00:00+00:00', 'status': '🆗', 'payload': [[1, 2], [3, 4]]}
 ```
 
 ### Serialize
@@ -134,104 +134,114 @@
 To serialize a subclass or arbitrary types, specify `default` as a
 callable that returns a supported type. `default` may be a function,
 lambda, or callable class instance. To specify that a type was not
 handled by `default`, raise an exception such as `TypeError`.
 
 ```python
 >>> import ormsgpack, decimal
->>>
-def default(obj):
-    if isinstance(obj, decimal.Decimal):
-        return str(obj)
-    raise TypeError
-
+>>> def default(obj):
+...     if isinstance(obj, decimal.Decimal):
+...         return str(obj)
+...     raise TypeError
+...
 >>> ormsgpack.packb(decimal.Decimal("0.0842389659712649442845"))
-MsgpackEncodeError: Type is not msgpack serializable: decimal.Decimal
+TypeError: Type is not msgpack serializable: decimal.Decimal
 >>> ormsgpack.packb(decimal.Decimal("0.0842389659712649442845"), default=default)
 b'\xb80.0842389659712649442845'
 >>> ormsgpack.packb({1, 2}, default=default)
-ormsgpack.MsgpackEncodeError: Type is not msgpack serializable: set
+TypeError: Type is not msgpack serializable: set
 ```
 
 The `default` callable may return an object that itself
 must be handled by `default` up to 254 times before an exception
 is raised.
 
 It is important that `default` raise an exception if a type cannot be handled.
 Python otherwise implicitly returns `None`, which appears to the caller
 like a legitimate value and is serialized:
 
 ```python
->>> import ormsgpack, json, rapidjson
->>>
-def default(obj):
-    if isinstance(obj, decimal.Decimal):
-        return str(obj)
-
->>> ormsgpack.unpackb(ormsgpack.packb({"set":{1, 2}}, default=default))
+>>> import ormsgpack, decimal
+>>> def default(obj):
+...     if isinstance(obj, decimal.Decimal):
+...         return str(obj)
+...
+>>> ormsgpack.packb({"set":{1, 2}}, default=default)
+b'\x81\xa3set\xc0'
+>>> ormsgpack.unpackb(_)
 {'set': None}
 ```
 
 To serialize a type as a MessagePack extension type, return an
 `ormsgpack.Ext` object. The instantiation arguments are an integer in
 the range `[0, 127]` and a `bytes` object, defining the type and
 value, respectively.
 
 ```python
 >>> import ormsgpack, decimal
->>>
-def default(obj):
-    if isinstance(obj, decimal.Decimal):
-        return ormsgpack.Ext(0, str(obj).encode())
-    raise TypeError
-
+>>> def default(obj):
+...     if isinstance(obj, decimal.Decimal):
+...         return ormsgpack.Ext(0, str(obj).encode())
+...     raise TypeError
+...
 >>> ormsgpack.packb(decimal.Decimal("0.0842389659712649442845"), default=default)
 b'\xc7\x18\x000.0842389659712649442845'
 ```
 
 #### option
 
 To modify how data is serialized, specify `option`. Each `option` is an integer
 constant in `ormsgpack`. To specify multiple options, mask them together, e.g.,
 `option=ormsgpack.OPT_NON_STR_KEYS | ormsgpack.OPT_NAIVE_UTC`.
 
 ##### OPT_NAIVE_UTC
 
-Serialize `datetime.datetime` objects without a `tzinfo` as UTC. This
-has no effect on `datetime.datetime` objects that have `tzinfo` set.
+Serialize `datetime.datetime` objects without a `tzinfo` and `numpy.datetime64`
+objects as UTC. This has no effect on `datetime.datetime` objects that have
+`tzinfo` set.
 
 ```python
 >>> import ormsgpack, datetime
->>> ormsgpack.unpackb(ormsgpack.packb(
-        datetime.datetime(1970, 1, 1, 0, 0, 0),
-    ))
-"1970-01-01T00:00:00"
->>> ormsgpack.unpackb(ormsgpack.packb(
-        datetime.datetime(1970, 1, 1, 0, 0, 0),
-        option=ormsgpack.OPT_NAIVE_UTC,
-    ))
-"1970-01-01T00:00:00+00:00"
+>>> ormsgpack.packb(
+...     datetime.datetime(1970, 1, 1, 0, 0, 0),
+... )
+b'\xb31970-01-01T00:00:00'
+>>> ormsgpack.unpackb(_)
+'1970-01-01T00:00:00'
+>>> ormsgpack.packb(
+...     datetime.datetime(1970, 1, 1, 0, 0, 0),
+...     option=ormsgpack.OPT_NAIVE_UTC,
+... )
+b'\xb91970-01-01T00:00:00+00:00'
+>>> ormsgpack.unpackb(_)
+'1970-01-01T00:00:00+00:00'
 ```
 
 ##### OPT_NON_STR_KEYS
 
 Serialize `dict` keys of type other than `str`. This allows `dict` keys
 to be one of `str`, `int`, `float`, `bool`, `None`, `datetime.datetime`,
 `datetime.date`, `datetime.time`, `enum.Enum`, and `uuid.UUID`.
 
 ```python
 >>> import ormsgpack, datetime, uuid
 >>> ormsgpack.packb(
-        {uuid.UUID("7202d115-7ff3-4c81-a7c1-2a1f067b1ece"): [1, 2, 3]},
-        option=ormsgpack.OPT_NON_STR_KEYS,
-    )
->>> ormsgpack.packb(
-        {datetime.datetime(1970, 1, 1, 0, 0, 0): [1, 2, 3]},
-        option=ormsgpack.OPT_NON_STR_KEYS | ormsgpack.OPT_NAIVE_UTC,
-    )
+...     {uuid.UUID("7202d115-7ff3-4c81-a7c1-2a1f067b1ece"): [1, 2, 3]},
+...     option=ormsgpack.OPT_NON_STR_KEYS,
+... )
+b'\x81\xd9$7202d115-7ff3-4c81-a7c1-2a1f067b1ece\x93\x01\x02\x03'
+>>> ormsgpack.unpackb(_)
+{'7202d115-7ff3-4c81-a7c1-2a1f067b1ece': [1, 2, 3]}
+>>> ormsgpack.packb(
+...     {datetime.datetime(1970, 1, 1, 0, 0, 0): [1, 2, 3]},
+...     option=ormsgpack.OPT_NON_STR_KEYS | ormsgpack.OPT_NAIVE_UTC,
+... )
+b'\x81\xb91970-01-01T00:00:00+00:00\x93\x01\x02\x03'
+>>> ormsgpack.unpackb(_)
+{'1970-01-01T00:00:00+00:00': [1, 2, 3]}
 ```
 
 These types are generally serialized how they would be as
 values, e.g., `datetime.datetime` is still an RFC 3339 string and respects
 options affecting it.
 
 This option has the risk of creating duplicate keys. This is because non-`str`
@@ -240,123 +250,126 @@
 The last key to be inserted to the `dict` will be serialized last and a msgpack deserializer will presumably take the last
 occurrence of a key (in the above, `false`). The first value will be lost.
 
 This option is not compatible with `ormsgpack.OPT_SORT_KEYS`.
 
 ##### OPT_OMIT_MICROSECONDS
 
-Do not serialize the `microsecond` field on `datetime.datetime` and
-`datetime.time` instances.
+Do not serialize the microsecond component of `datetime.datetime`,
+`datetime.time` and `numpy.datetime64` instances.
 
 ```python
 >>> import ormsgpack, datetime
 >>> ormsgpack.packb(
-        datetime.datetime(1970, 1, 1, 0, 0, 0, 1),
-    )
->>> ormsgpack.packb(
-        datetime.datetime(1970, 1, 1, 0, 0, 0, 1),
-        option=ormsgpack.OPT_OMIT_MICROSECONDS,
-    )
+...     datetime.datetime(1970, 1, 1, 0, 0, 0, 1),
+... )
+b'\xba1970-01-01T00:00:00.000001'
+>>> ormsgpack.unpackb(_)
+'1970-01-01T00:00:00.000001'
+>>> ormsgpack.packb(
+...     datetime.datetime(1970, 1, 1, 0, 0, 0, 1),
+...     option=ormsgpack.OPT_OMIT_MICROSECONDS,
+... )
+b'\xb31970-01-01T00:00:00'
+>>> ormsgpack.unpackb(_)
+'1970-01-01T00:00:00'
 ```
 
 ##### OPT_PASSTHROUGH_BIG_INT
 
 Enables passthrough of big (Python) ints. By setting this option, one can set a `default` function for ints larger than 63 bits, smaller ints are still serialized efficiently.
 
 ```python
 >>> import ormsgpack
 >>> ormsgpack.packb(
-        2**65,
-    )
+...     2**65,
+... )
 TypeError: Integer exceeds 64-bit range
->>> ormsgpack.unpackb(
-        ormsgpack.packb(
-            2**65,
-            option=ormsgpack.OPT_PASSTHROUGH_BIG_INT,
-            default=lambda _: {"type": "bigint", "value": str(_) }
-        )
-    )
+>>> ormsgpack.packb(
+...     2**65,
+...     option=ormsgpack.OPT_PASSTHROUGH_BIG_INT,
+...     default=lambda _: {"type": "bigint", "value": str(_) }
+... )
+b'\x82\xa4type\xa6bigint\xa5value\xb436893488147419103232'
+>>> ormsgpack.unpackb(_)
 {'type': 'bigint', 'value': '36893488147419103232'}
 ```
 
 ##### OPT_PASSTHROUGH_DATACLASS
 
 Passthrough `dataclasses.dataclass` instances to `default`. This allows
 customizing their output but is much slower.
 
 
 ```python
 >>> import ormsgpack, dataclasses
->>>
-@dataclasses.dataclass
-class User:
-    id: str
-    name: str
-    password: str
-
-def default(obj):
-    if isinstance(obj, User):
-        return {"id": obj.id, "name": obj.name}
-    raise TypeError
-
+>>> @dataclasses.dataclass
+... class User:
+...     id: str
+...     name: str
+...     password: str
+...
+>>> def default(obj):
+...     if isinstance(obj, User):
+...         return {"id": obj.id, "name": obj.name}
+...     raise TypeError
+...
 >>> ormsgpack.packb(User("3b1", "asd", "zxc"))
 b'\x83\xa2id\xa33b1\xa4name\xa3asd\xa8password\xa3zxc'
 >>> ormsgpack.packb(User("3b1", "asd", "zxc"), option=ormsgpack.OPT_PASSTHROUGH_DATACLASS)
 TypeError: Type is not msgpack serializable: User
 >>> ormsgpack.packb(
-        User("3b1", "asd", "zxc"),
-        option=ormsgpack.OPT_PASSTHROUGH_DATACLASS,
-        default=default,
-    )
+...     User("3b1", "asd", "zxc"),
+...     option=ormsgpack.OPT_PASSTHROUGH_DATACLASS,
+...     default=default,
+... )
 b'\x82\xa2id\xa33b1\xa4name\xa3asd'
 ```
 
 ##### OPT_PASSTHROUGH_DATETIME
 
 Passthrough `datetime.datetime`, `datetime.date`, and `datetime.time` instances
 to `default`. This allows serializing datetimes to a custom format, e.g.,
 HTTP dates:
 
 ```python
 >>> import ormsgpack, datetime
->>>
-def default(obj):
-    if isinstance(obj, datetime.datetime):
-        return obj.strftime("%a, %d %b %Y %H:%M:%S GMT")
-    raise TypeError
-
+>>> def default(obj):
+...     if isinstance(obj, datetime.datetime):
+...         return obj.strftime("%a, %d %b %Y %H:%M:%S GMT")
+...     raise TypeError
+...
 >>> ormsgpack.packb({"created_at": datetime.datetime(1970, 1, 1)})
 b'\x81\xaacreated_at\xb31970-01-01T00:00:00'
 >>> ormsgpack.packb({"created_at": datetime.datetime(1970, 1, 1)}, option=ormsgpack.OPT_PASSTHROUGH_DATETIME)
 TypeError: Type is not msgpack serializable: datetime.datetime
 >>> ormsgpack.packb(
-        {"created_at": datetime.datetime(1970, 1, 1)},
-        option=ormsgpack.OPT_PASSTHROUGH_DATETIME,
-        default=default,
-    )
+...     {"created_at": datetime.datetime(1970, 1, 1)},
+...     option=ormsgpack.OPT_PASSTHROUGH_DATETIME,
+...     default=default,
+... )
 b'\x81\xaacreated_at\xbdThu, 01 Jan 1970 00:00:00 GMT'
 ```
 
 This does not affect datetimes in `dict` keys if using OPT_NON_STR_KEYS.
 
 ##### OPT_PASSTHROUGH_SUBCLASS
 
 Passthrough subclasses of builtin types to `default`.
 
 ```python
 >>> import ormsgpack
->>>
-class Secret(str):
-    pass
-
-def default(obj):
-    if isinstance(obj, Secret):
-        return "******"
-    raise TypeError
-
+>>> class Secret(str):
+...     pass
+...
+>>> def default(obj):
+...     if isinstance(obj, Secret):
+...         return "******"
+...     raise TypeError
+...
 >>> ormsgpack.packb(Secret("zxc"))
 b'\xa3zxc'
 >>> ormsgpack.packb(Secret("zxc"), option=ormsgpack.OPT_PASSTHROUGH_SUBCLASS)
 TypeError: Type is not msgpack serializable: Secret
 >>> ormsgpack.packb(Secret("zxc"), option=ormsgpack.OPT_PASSTHROUGH_SUBCLASS, default=default)
 b'\xa6******'
 ```
@@ -366,27 +379,27 @@
 
 ##### OPT_PASSTHROUGH_TUPLE
 
 Passthrough tuples to `default`.
 
 ```python
 >>> import ormsgpack
->>> ormsgpack.unpackb(
-        ormsgpack.packb(
-            (9193, "test", 42),
-        )
-    )
+>>> ormsgpack.packb(
+...     (9193, "test", 42),
+... )
+b'\x93\xcd#\xe9\xa4test*'
+>>> ormsgpack.unpackb(_)
 [9193, 'test', 42]
->>> ormsgpack.unpackb(
-        ormsgpack.packb(
-            (9193, "test", 42),
-            option=ormsgpack.OPT_PASSTHROUGH_TUPLE,
-            default=lambda _: {"type": "tuple", "value": list(_)}
-        )
-    )
+>>> ormsgpack.packb(
+...     (9193, "test", 42),
+...     option=ormsgpack.OPT_PASSTHROUGH_TUPLE,
+...     default=lambda _: {"type": "tuple", "value": list(_)}
+... )
+b'\x82\xa4type\xa5tuple\xa5value\x93\xcd#\xe9\xa4test*'
+>>> ormsgpack.unpackb(_)
 {'type': 'tuple', 'value': [9193, 'test', 42]}
 ```
 
 ##### OPT_SERIALIZE_NUMPY
 
 Serialize `numpy.ndarray` instances. For more, see
 [numpy](#numpy).
@@ -418,28 +431,28 @@
 b'\x83\xa1A\x03\xa1a\x01\xa2\xc3\xa4\x02'
 ```
 
 `dataclass` also serialize as maps but this has no effect on them.
 
 ##### OPT_UTC_Z
 
-Serialize a UTC timezone on `datetime.datetime` instances as `Z` instead
-of `+00:00`.
+Serialize a UTC timezone on `datetime.datetime` and `numpy.datetime64` instances
+as `Z` instead of `+00:00`.
 
 ```python
 >>> import ormsgpack, datetime
 >>> ormsgpack.packb(
-        datetime.datetime(1970, 1, 1, 0, 0, 0, tzinfo=datetime.timezone.utc),
-    )
-b'"1970-01-01T00:00:00+00:00"'
->>> ormsgpack.packb(
-        datetime.datetime(1970, 1, 1, 0, 0, 0, tzinfo=datetime.timezone.utc),
-        option=ormsgpack.OPT_UTC_Z
-    )
-b'"1970-01-01T00:00:00Z"'
+...     datetime.datetime(1970, 1, 1, 0, 0, 0, tzinfo=datetime.timezone.utc),
+... )
+b'\xb91970-01-01T00:00:00+00:00'
+>>> ormsgpack.packb(
+...     datetime.datetime(1970, 1, 1, 0, 0, 0, tzinfo=datetime.timezone.utc),
+...     option=ormsgpack.OPT_UTC_Z
+... )
+b'\xb41970-01-01T00:00:00Z'
 ```
 
 ### Deserialize
 ```python
 def unpackb(
     __obj: Union[bytes, bytearray, memoryview],
     /,
@@ -468,25 +481,25 @@
 
 To deserialize extension types, specify the optional `ext_hook`
 argument. The value should be a callable and is invoked with the
 extension type and value as arguments.
 
 ```python
 >>> import ormsgpack, decimal
->>>
-def ext_hook(tag, data):
-    if tag == 0:
-        return decimal.Decimal(data.decode())
-    raise TypeError
-
+>>> def ext_hook(tag, data):
+...     if tag == 0:
+...         return decimal.Decimal(data.decode())
+...     raise TypeError
+...
 >>> ormsgpack.packb(
-    ormsgpack.Ext(0, str(decimal.Decimal("0.0842389659712649442845")).encode())
-)
+...     ormsgpack.Ext(0, str(decimal.Decimal("0.0842389659712649442845")).encode())
+... )
+b'\xc7\x18\x000.0842389659712649442845'
 >>> ormsgpack.unpackb(_, ext_hook=ext_hook)
-Decimal('0.0842389659712649442845')
+Decimal('0.0842389659712649442845'
 ```
 
 #### option
 `unpackb()` supports the `OPT_NON_STR_KEYS` option, that is similar to original msgpack's `strict_map_key=False`.
 Be aware that this option is considered unsafe and disabled by default in msgpack due to possibility of HashDoS.
 
 ## Types
@@ -503,26 +516,25 @@
 using `__slots__`.
 
 Dataclasses are serialized as maps, with every attribute serialized and in
 the order given on class definition:
 
 ```python
 >>> import dataclasses, ormsgpack, typing
-
-@dataclasses.dataclass
-class Member:
-    id: int
-    active: bool = dataclasses.field(default=False)
-
-@dataclasses.dataclass
-class Object:
-    id: int
-    name: str
-    members: typing.List[Member]
-
+>>> @dataclasses.dataclass
+... class Member:
+...     id: int
+...     active: bool = dataclasses.field(default=False)
+...
+>>> @dataclasses.dataclass
+... class Object:
+...     id: int
+...     name: str
+...     members: typing.List[Member]
+...
 >>> ormsgpack.packb(Object(1, "a", [Member(1, True), Member(2)]))
 b'\x83\xa2id\x01\xa4name\xa1a\xa7members\x92\x82\xa2id\x01\xa6active\xc3\x82\xa2id\x02\xa6active\xc2'
 ```
 #### Performance
 ![alt text](doc/dataclass.svg "dataclass")
 
 ```
@@ -540,51 +552,56 @@
 [RFC 3339](https://tools.ietf.org/html/rfc3339) format,
 e.g., "1970-01-01T00:00:00+00:00". This is a subset of ISO 8601 and is
 compatible with `isoformat()` in the standard library.
 
 ```python
 >>> import ormsgpack, datetime, zoneinfo
 >>> ormsgpack.packb(
-    datetime.datetime(2018, 12, 1, 2, 3, 4, 9, tzinfo=zoneinfo.ZoneInfo('Australia/Adelaide'))
-)
+...     datetime.datetime(2018, 12, 1, 2, 3, 4, 9, tzinfo=zoneinfo.ZoneInfo('Australia/Adelaide'))
+... )
+b'\xd9 2018-12-01T02:03:04.000009+10:30'
 >>> ormsgpack.unpackb(_)
-"2018-12-01T02:03:04.000009+10:30"
+'2018-12-01T02:03:04.000009+10:30'
 >>> ormsgpack.packb(
-    datetime.datetime.fromtimestamp(4123518902).replace(tzinfo=datetime.timezone.utc)
-)
+...     datetime.datetime.fromtimestamp(4123518902).replace(tzinfo=datetime.timezone.utc)
+... )
+b'\xb92100-09-02T00:55:02+00:00'
 >>> ormsgpack.unpackb(_)
-"2100-09-01T21:55:02+00:00"
+'2100-09-02T00:55:02+00:00'
 >>> ormsgpack.packb(
-    datetime.datetime.fromtimestamp(4123518902)
-)
+...     datetime.datetime.fromtimestamp(4123518902)
+... )
+b'\xb32100-09-02T00:55:02'
 >>> ormsgpack.unpackb(_)
-"2100-09-01T21:55:02"
+'2100-09-02T00:55:02'
 ```
 
 `datetime.datetime` supports instances with a `tzinfo` that is `None`,
 `datetime.timezone.utc`, a timezone instance from the python3.9+ `zoneinfo`
 module, or a timezone instance from the third-party `pendulum`, `pytz`, or
 `dateutil`/`arrow` libraries.
 
 `datetime.time` objects must not have a `tzinfo`.
 
 ```python
 >>> import ormsgpack, datetime
 >>> ormsgpack.packb(datetime.time(12, 0, 15, 290))
+b'\xaf12:00:15.000290'
 >>> ormsgpack.unpackb(_)
-"12:00:15.000290"
+'12:00:15.000290'
 ```
 
 `datetime.date` objects will always serialize.
 
 ```python
 >>> import ormsgpack, datetime
 >>> ormsgpack.packb(datetime.date(1900, 1, 2))
+b'\xaa1900-01-02'
 >>> ormsgpack.unpackb(_)
-"1900-01-02"
+'1900-01-02'
 ```
 
 Errors with `tzinfo` result in `MsgpackEncodeError` being raised.
 
 To disable serialization of `datetime` objects specify the option
 `ormsgpack.OPT_PASSTHROUGH_DATETIME`.
 
@@ -595,44 +612,46 @@
 
 ### enum
 
 ormsgpack serializes enums natively. Options apply to their values.
 
 ```python
 >>> import enum, datetime, ormsgpack
->>>
-class DatetimeEnum(enum.Enum):
-    EPOCH = datetime.datetime(1970, 1, 1, 0, 0, 0)
+>>> class DatetimeEnum(enum.Enum):
+...     EPOCH = datetime.datetime(1970, 1, 1, 0, 0, 0)
+...
 >>> ormsgpack.packb(DatetimeEnum.EPOCH)
+b'\xb31970-01-01T00:00:00'
 >>> ormsgpack.unpackb(_)
-"1970-01-01T00:00:00"
+'1970-01-01T00:00:00'
 >>> ormsgpack.packb(DatetimeEnum.EPOCH, option=ormsgpack.OPT_NAIVE_UTC)
+b'\xb91970-01-01T00:00:00+00:00'
 >>> ormsgpack.unpackb(_)
-"1970-01-01T00:00:00+00:00"
+'1970-01-01T00:00:00+00:00'
 ```
 
 Enums with members that are not supported types can be serialized using
 `default`:
 
 ```python
 >>> import enum, ormsgpack
->>>
-class Custom:
-    def __init__(self, val):
-        self.val = val
-
-def default(obj):
-    if isinstance(obj, Custom):
-        return obj.val
-    raise TypeError
-
-class CustomEnum(enum.Enum):
-    ONE = Custom(1)
-
+>>> class Custom:
+...     def __init__(self, val):
+...         self.val = val
+...
+>>> def default(obj):
+...     if isinstance(obj, Custom):
+...         return obj.val
+...     raise TypeError
+...
+>>> class CustomEnum(enum.Enum):
+...     ONE = Custom(1)
+...
 >>> ormsgpack.packb(CustomEnum.ONE, default=default)
+b'\x01'
 >>> ormsgpack.unpackb(_)
 1
 ```
 
 ### float
 
 ormsgpack serializes and deserializes double precision floats with no loss of
@@ -643,32 +662,35 @@
 ormsgpack serializes and deserializes 64-bit integers by default. The range
 supported is a signed 64-bit integer's minimum (-9223372036854775807) to
 an unsigned 64-bit integer's maximum (18446744073709551615).
 
 ### numpy
 
 ormsgpack natively serializes `numpy.ndarray` and individual
-`numpy.float64`, `numpy.float32`,
+`numpy.float64`, `numpy.float32`, `numpy.float16`,
 `numpy.int64`, `numpy.int32`, `numpy.int16`, `numpy.int8`,
 `numpy.uint64`, `numpy.uint32`, `numpy.uint16`, `numpy.uint8`,
-`numpy.uintp`, `numpy.intp`, and `numpy.bool`
+`numpy.uintp`, `numpy.intp`, `numpy.datetime64`, and `numpy.bool`
 instances.
 
+`numpy.datetime64` instances are serialized as RFC 3339 strings.
+
 ormsgpack is faster than all compared libraries at serializing
 numpy instances. Serializing numpy data requires specifying
 `option=ormsgpack.OPT_SERIALIZE_NUMPY`.
 
 ```python
 >>> import ormsgpack, numpy
 >>> ormsgpack.packb(
-        numpy.array([[1, 2, 3], [4, 5, 6]]),
-        option=ormsgpack.OPT_SERIALIZE_NUMPY,
-)
+...     numpy.array([[1, 2, 3], [4, 5, 6]]),
+...     option=ormsgpack.OPT_SERIALIZE_NUMPY,
+... )
+b'\x92\x93\x01\x02\x03\x93\x04\x05\x06'
 >>> ormsgpack.unpackb(_)
-[[1,2,3],[4,5,6]]
+[[1, 2, 3], [4, 5, 6]]
 ```
 
 The array must be a contiguous C array (`C_CONTIGUOUS`) and one of the
 supported datatypes.
 
 If an array is not a contiguous C array or contains an supported datatype,
 ormsgpack falls through to `default`. In `default`, `obj.tolist()` can be
@@ -724,22 +746,24 @@
 
 ### uuid
 
 ormsgpack serializes `uuid.UUID` instances to
 [RFC 4122](https://tools.ietf.org/html/rfc4122) format, e.g.,
 "f81d4fae-7dec-11d0-a765-00a0c91e6bf6".
 
-``` python
+```python
 >>> import ormsgpack, uuid
 >>> ormsgpack.packb(uuid.UUID('f81d4fae-7dec-11d0-a765-00a0c91e6bf6'))
+b'\xd9$f81d4fae-7dec-11d0-a765-00a0c91e6bf6'
 >>> ormsgpack.unpackb(_)
-"f81d4fae-7dec-11d0-a765-00a0c91e6bf6"
+'f81d4fae-7dec-11d0-a765-00a0c91e6bf6'
 >>> ormsgpack.packb(uuid.uuid5(uuid.NAMESPACE_DNS, "python.org"))
+b'\xd9$886313e1-3b8a-5372-9b90-0c9aee199e5d'
 >>> ormsgpack.unpackb(_)
-"886313e1-3b8a-5372-9b90-0c9aee199e5d"
+'886313e1-3b8a-5372-9b90-0c9aee199e5d
 ```
 
 ### Pydantic
 ormsgpack serializes `pydantic.BaseModel` instances natively.
 
 #### Performance
 ![alt text](doc/pydantic.svg "pydantic")
```

### Comparing `ormsgpack-1.4.2/src/deserialize/cache.rs` & `ormsgpack-1.5.0/src/deserialize/cache.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.4.2/src/deserialize/deserializer.rs` & `ormsgpack-1.5.0/src/deserialize/deserializer.rs`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 use crate::deserialize::DeserializeError;
 use crate::ffi::*;
 use crate::opt::*;
 use crate::typeref::*;
 use crate::unicode::*;
 use serde::de::{self, DeserializeSeed, Deserializer, MapAccess, SeqAccess, Visitor};
 use serde_bytes::ByteBuf;
-use smallvec::SmallVec;
 use std::borrow::Cow;
 use std::fmt;
 use std::os::raw::c_char;
 use std::ptr::NonNull;
 
 pub fn deserialize(
     ptr: *mut pyo3::ffi::PyObject,
@@ -211,38 +210,34 @@
         Ok(nonnull!(ffi!(PyBytes_FromStringAndSize(ptr, len))))
     }
 
     fn visit_seq<A>(self, mut seq: A) -> Result<Self::Value, A::Error>
     where
         A: SeqAccess<'de>,
     {
-        match seq.next_element_seed(self) {
-            Ok(None) => Ok(nonnull!(ffi!(PyList_New(0)))),
-            Ok(Some(elem)) => {
-                let mut elements: SmallVec<[*mut pyo3::ffi::PyObject; 8]> =
-                    SmallVec::with_capacity(8);
-                elements.push(elem.as_ptr());
-                while let Some(elem) = seq.next_element_seed(self)? {
-                    elements.push(elem.as_ptr());
-                }
-                let ptr = ffi!(PyList_New(elements.len() as pyo3::ffi::Py_ssize_t));
-                for (i, &obj) in elements.iter().enumerate() {
-                    ffi!(PyList_SET_ITEM(ptr, i as pyo3::ffi::Py_ssize_t, obj));
-                }
-                Ok(nonnull!(ptr))
-            }
-            Err(err) => std::result::Result::Err(err),
+        let size = seq.size_hint().unwrap() as pyo3::ffi::Py_ssize_t;
+        let ptr = ffi!(PyList_New(size));
+        let mut i = 0;
+        while let Some(elem) = seq.next_element_seed(self)? {
+            ffi!(PyList_SET_ITEM(
+                ptr,
+                i as pyo3::ffi::Py_ssize_t,
+                elem.as_ptr()
+            ));
+            i += 1;
         }
+        Ok(nonnull!(ptr))
     }
 
     fn visit_map<A>(self, mut map: A) -> Result<Self::Value, A::Error>
     where
         A: MapAccess<'de>,
     {
-        let dict_ptr = ffi!(PyDict_New());
+        let size = map.size_hint().unwrap() as pyo3::ffi::Py_ssize_t;
+        let dict_ptr = ffi!(_PyDict_NewPresized(size));
         while let Some(key) = map.next_key::<Cow<str>>()? {
             let value = map.next_value_seed(self)?;
             let pykey: *mut pyo3::ffi::PyObject;
             let pyhash: pyo3::ffi::Py_hash_t;
             if unlikely!(key.len() > 64) {
                 pykey = unicode_from_str(&key);
                 pyhash = hash_str(pykey);
@@ -385,38 +380,34 @@
         Ok(nonnull!(ffi!(PyBytes_FromStringAndSize(ptr, len))))
     }
 
     fn visit_seq<A>(self, mut seq: A) -> Result<Self::Value, A::Error>
     where
         A: SeqAccess<'de>,
     {
-        match seq.next_element_seed(self) {
-            Ok(None) => Ok(nonnull!(ffi!(PyList_New(0)))),
-            Ok(Some(elem)) => {
-                let mut elements: SmallVec<[*mut pyo3::ffi::PyObject; 8]> =
-                    SmallVec::with_capacity(8);
-                elements.push(elem.as_ptr());
-                while let Some(elem) = seq.next_element_seed(self)? {
-                    elements.push(elem.as_ptr());
-                }
-                let ptr = ffi!(PyList_New(elements.len() as pyo3::ffi::Py_ssize_t));
-                for (i, &obj) in elements.iter().enumerate() {
-                    ffi!(PyList_SET_ITEM(ptr, i as pyo3::ffi::Py_ssize_t, obj));
-                }
-                Ok(nonnull!(ptr))
-            }
-            Err(err) => std::result::Result::Err(err),
+        let size = seq.size_hint().unwrap() as pyo3::ffi::Py_ssize_t;
+        let ptr = ffi!(PyList_New(size));
+        let mut i = 0;
+        while let Some(elem) = seq.next_element_seed(self)? {
+            ffi!(PyList_SET_ITEM(
+                ptr,
+                i as pyo3::ffi::Py_ssize_t,
+                elem.as_ptr()
+            ));
+            i += 1;
         }
+        Ok(nonnull!(ptr))
     }
 
     fn visit_map<A>(self, mut map: A) -> Result<Self::Value, A::Error>
     where
         A: MapAccess<'de>,
     {
-        let dict_ptr = ffi!(PyDict_New());
+        let size = map.size_hint().unwrap() as pyo3::ffi::Py_ssize_t;
+        let dict_ptr = ffi!(_PyDict_NewPresized(size));
         while let Some((key, value)) = map.next_entry_seed(MsgpackKey {}, self)? {
             let ret = ffi!(PyDict_SetItem(dict_ptr, key.as_ptr(), value.as_ptr()));
             if unlikely!(ret == -1) {
                 return Err(de::Error::custom("PyDict_SetItem failed"));
             }
             ffi!(Py_DECREF(key.as_ptr()));
             ffi!(Py_DECREF(value.as_ptr()));
@@ -515,26 +506,21 @@
         Ok(nonnull!(ffi!(PyBytes_FromStringAndSize(ptr, len))))
     }
 
     fn visit_seq<A>(self, mut seq: A) -> Result<Self::Value, A::Error>
     where
         A: SeqAccess<'de>,
     {
-        match seq.next_element_seed(self) {
-            Ok(None) => Ok(nonnull!(ffi!(PyTuple_New(0)))),
-            Ok(Some(elem)) => {
-                let mut elements: SmallVec<[*mut pyo3::ffi::PyObject; 8]> =
-                    SmallVec::with_capacity(8);
-                elements.push(elem.as_ptr());
-                while let Some(elem) = seq.next_element_seed(self)? {
-                    elements.push(elem.as_ptr());
-                }
-                let ptr = ffi!(PyTuple_New(elements.len() as pyo3::ffi::Py_ssize_t));
-                for (i, &obj) in elements.iter().enumerate() {
-                    ffi!(PyTuple_SET_ITEM(ptr, i as pyo3::ffi::Py_ssize_t, obj));
-                }
-                Ok(nonnull!(ptr))
-            }
-            Err(err) => std::result::Result::Err(err),
+        let size = seq.size_hint().unwrap() as pyo3::ffi::Py_ssize_t;
+        let ptr = ffi!(PyTuple_New(size));
+        let mut i = 0;
+        while let Some(elem) = seq.next_element_seed(self)? {
+            ffi!(PyTuple_SET_ITEM(
+                ptr,
+                i as pyo3::ffi::Py_ssize_t,
+                elem.as_ptr()
+            ));
+            i += 1;
         }
+        Ok(nonnull!(ptr))
     }
 }
```

### Comparing `ormsgpack-1.4.2/src/ext.rs` & `ormsgpack-1.5.0/src/ext.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use pyo3::ffi::*;
 use std::os::raw::{c_char, c_int, c_uint, c_void};
 use std::ptr::null_mut;
 
 #[repr(C)]
-pub struct Ext {
+pub struct PyExt {
     pub ob_base: PyObject,
     pub tag: *mut PyObject,
     pub data: *mut PyObject,
 }
 
 #[no_mangle]
 unsafe extern "C" fn ext_new(
@@ -36,24 +36,24 @@
             PyExc_TypeError,
             "Ext.__new__() second argument must be bytes\0".as_ptr() as *const c_char,
         );
         return null_mut();
     }
     let obj = (*subtype).tp_alloc.unwrap()(subtype, 0);
     Py_INCREF(tag);
-    (*(obj as *mut Ext)).tag = tag;
+    (*(obj as *mut PyExt)).tag = tag;
     Py_INCREF(data);
-    (*(obj as *mut Ext)).data = data;
+    (*(obj as *mut PyExt)).data = data;
     obj
 }
 
 #[no_mangle]
 unsafe extern "C" fn ext_dealloc(op: *mut PyObject) {
-    Py_DECREF((*(op as *mut Ext)).tag);
-    Py_DECREF((*(op as *mut Ext)).data);
+    Py_DECREF((*(op as *mut PyExt)).tag);
+    Py_DECREF((*(op as *mut PyExt)).data);
     (*ob_type!(op)).tp_free.unwrap()(op as *mut c_void);
 }
 
 pub unsafe fn create_ext_type() -> *mut PyTypeObject {
     let mut slots: [PyType_Slot; 3] = [
         PyType_Slot {
             slot: Py_tp_new,
@@ -66,14 +66,14 @@
         PyType_Slot {
             slot: 0,
             pfunc: null_mut(),
         },
     ];
     let mut spec = PyType_Spec {
         name: "ormsgpack.Ext\0".as_ptr() as *const c_char,
-        basicsize: std::mem::size_of::<Ext>() as c_int,
+        basicsize: std::mem::size_of::<PyExt>() as c_int,
         itemsize: 0,
         flags: Py_TPFLAGS_DEFAULT as c_uint,
         slots: slots.as_mut_ptr(),
     };
     PyType_FromSpec(&mut spec) as *mut PyTypeObject
 }
```

### Comparing `ormsgpack-1.4.2/src/ffi.rs` & `ormsgpack-1.5.0/src/ffi.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.4.2/src/lib.rs` & `ormsgpack-1.5.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.4.2/src/opt.rs` & `ormsgpack-1.5.0/src/opt.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.4.2/src/serialize/bytes.rs` & `ormsgpack-1.5.0/src/serialize/bytes.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 // SPDX-License-Identifier: (Apache-2.0 OR MIT)
 
 use crate::ffi::*;
 
 use serde::ser::{Serialize, Serializer};
 
 #[repr(transparent)]
-pub struct BytesSerializer {
+pub struct Bytes {
     ptr: *mut pyo3::ffi::PyObject,
 }
 
-impl BytesSerializer {
+impl Bytes {
     pub fn new(ptr: *mut pyo3::ffi::PyObject) -> Self {
-        BytesSerializer { ptr: ptr }
+        Bytes { ptr: ptr }
     }
 }
 
-impl Serialize for BytesSerializer {
+impl Serialize for Bytes {
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
         let buffer = unsafe { PyBytes_AS_STRING(self.ptr) as *const u8 };
         let length = unsafe { PyBytes_GET_SIZE(self.ptr) as usize };
         let contents = unsafe { std::slice::from_raw_parts(buffer, length) };
```

### Comparing `ormsgpack-1.4.2/src/serialize/dataclass.rs` & `ormsgpack-1.5.0/src/serialize/dataclass.rs`

 * *Files 10% similar despite different names*

```diff
@@ -5,187 +5,203 @@
 use crate::opt::*;
 use crate::serialize::serializer::*;
 use crate::typeref::*;
 use crate::unicode::*;
 
 use serde::ser::{Serialize, SerializeMap, Serializer};
 
+use smallvec::SmallVec;
 use std::ptr::NonNull;
 
-pub struct DataclassGenericSerializer {
+pub struct Dataclass {
     ptr: *mut pyo3::ffi::PyObject,
     opts: Opt,
     default_calls: u8,
     recursion: u8,
     default: Option<NonNull<pyo3::ffi::PyObject>>,
 }
 
-impl DataclassGenericSerializer {
+impl Dataclass {
     pub fn new(
         ptr: *mut pyo3::ffi::PyObject,
         opts: Opt,
         default_calls: u8,
         recursion: u8,
         default: Option<NonNull<pyo3::ffi::PyObject>>,
     ) -> Self {
-        DataclassGenericSerializer {
+        Dataclass {
             ptr: ptr,
             opts: opts,
             default_calls: default_calls,
             recursion: recursion,
             default: default,
         }
     }
 }
 
-impl Serialize for DataclassGenericSerializer {
+impl Serialize for Dataclass {
     #[inline(never)]
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
-        let dict = ffi!(PyObject_GetAttr(self.ptr, DICT_STR));
         let ob_type = ob_type!(self.ptr);
-        if unlikely!(dict.is_null()) {
-            ffi!(PyErr_Clear());
-            DataclassFallbackSerializer::new(
+        if pydict_contains!(ob_type, SLOTS_STR) {
+            DataclassFields::new(
                 self.ptr,
                 self.opts,
                 self.default_calls,
                 self.recursion,
                 self.default,
             )
             .serialize(serializer)
-        } else if pydict_contains!(ob_type, SLOTS_STR) {
-            let ret = DataclassFallbackSerializer::new(
-                self.ptr,
-                self.opts,
-                self.default_calls,
-                self.recursion,
-                self.default,
-            )
-            .serialize(serializer);
-            ffi!(Py_DECREF(dict));
-            ret
         } else {
-            let ret = DataclassFastSerializer::new(
-                dict,
+            match AttributeDict::new(
+                self.ptr,
                 self.opts,
                 self.default_calls,
                 self.recursion,
                 self.default,
-            )
-            .serialize(serializer);
-            ffi!(Py_DECREF(dict));
-            ret
+            ) {
+                Ok(val) => val.serialize(serializer),
+                Err(AttributeDictError::DictMissing) => DataclassFields::new(
+                    self.ptr,
+                    self.opts,
+                    self.default_calls,
+                    self.recursion,
+                    self.default,
+                )
+                .serialize(serializer),
+            }
         }
     }
 }
 
-pub struct DataclassFastSerializer {
+pub enum AttributeDictError {
+    DictMissing,
+}
+
+pub struct AttributeDict {
     ptr: *mut pyo3::ffi::PyObject,
     opts: Opt,
     default_calls: u8,
     recursion: u8,
     default: Option<NonNull<pyo3::ffi::PyObject>>,
 }
 
-impl DataclassFastSerializer {
+impl AttributeDict {
     pub fn new(
         ptr: *mut pyo3::ffi::PyObject,
         opts: Opt,
         default_calls: u8,
         recursion: u8,
         default: Option<NonNull<pyo3::ffi::PyObject>>,
-    ) -> Self {
-        DataclassFastSerializer {
-            ptr: ptr,
+    ) -> Result<Self, AttributeDictError> {
+        let dict = ffi!(PyObject_GetAttr(ptr, DICT_STR));
+        if unlikely!(dict.is_null()) {
+            ffi!(PyErr_Clear());
+            return Err(AttributeDictError::DictMissing);
+        }
+        Ok(AttributeDict {
+            ptr: dict,
             opts: opts,
             default_calls: default_calls,
             recursion: recursion,
             default: default,
-        }
+        })
     }
 }
 
-impl Serialize for DataclassFastSerializer {
+impl Drop for AttributeDict {
+    fn drop(&mut self) {
+        ffi!(Py_DECREF(self.ptr));
+    }
+}
+
+impl Serialize for AttributeDict {
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
-        let len = ffi!(Py_SIZE(self.ptr));
+        let len = ffi!(Py_SIZE(self.ptr)) as usize;
         if unlikely!(len == 0) {
             return serializer.serialize_map(Some(0)).unwrap().end();
         }
-        let mut map = serializer.serialize_map(None).unwrap();
+        let mut items: SmallVec<[(&str, *mut pyo3::ffi::PyObject); 8]> =
+            SmallVec::with_capacity(len);
         for (key, value) in PyDictIter::from_pyobject(self.ptr) {
             if unlikely!(!is_type!(ob_type!(key.as_ptr()), STR_TYPE)) {
                 err!(KEY_MUST_BE_STR)
             }
             let data = unicode_to_str(key.as_ptr());
             if unlikely!(data.is_none()) {
                 err!(INVALID_STR)
             }
             let key_as_str = data.unwrap();
             if unlikely!(key_as_str.as_bytes()[0] == b'_') {
                 continue;
             }
+            items.push((key_as_str, value.as_ptr()));
+        }
 
-            let pyvalue = PyObjectSerializer::new(
-                value.as_ptr(),
+        let mut map = serializer.serialize_map(Some(items.len())).unwrap();
+        for (key, value) in items.iter() {
+            let pyvalue = PyObject::new(
+                *value,
                 self.opts,
                 self.default_calls,
                 self.recursion + 1,
                 self.default,
             );
-            map.serialize_key(key_as_str).unwrap();
+            map.serialize_key(key).unwrap();
             map.serialize_value(&pyvalue)?;
         }
         map.end()
     }
 }
 
-pub struct DataclassFallbackSerializer {
+pub struct DataclassFields {
     ptr: *mut pyo3::ffi::PyObject,
     opts: Opt,
     default_calls: u8,
     recursion: u8,
     default: Option<NonNull<pyo3::ffi::PyObject>>,
 }
 
-impl DataclassFallbackSerializer {
+impl DataclassFields {
     pub fn new(
         ptr: *mut pyo3::ffi::PyObject,
         opts: Opt,
         default_calls: u8,
         recursion: u8,
         default: Option<NonNull<pyo3::ffi::PyObject>>,
     ) -> Self {
-        DataclassFallbackSerializer {
+        DataclassFields {
             ptr: ptr,
             opts: opts,
             default_calls: default_calls,
             recursion: recursion,
             default: default,
         }
     }
 }
 
-impl Serialize for DataclassFallbackSerializer {
+impl Serialize for DataclassFields {
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
         let fields = ffi!(PyObject_GetAttr(self.ptr, DATACLASS_FIELDS_STR));
         ffi!(Py_DECREF(fields));
-        let len = ffi!(Py_SIZE(fields));
+        let len = ffi!(Py_SIZE(fields)) as usize;
         if unlikely!(len == 0) {
             return serializer.serialize_map(Some(0)).unwrap().end();
         }
-        let mut map = serializer.serialize_map(None).unwrap();
+        let mut items: SmallVec<[(&str, *mut pyo3::ffi::PyObject); 8]> =
+            SmallVec::with_capacity(len);
         for (attr, field) in PyDictIter::from_pyobject(fields) {
             let field_type = ffi!(PyObject_GetAttr(field.as_ptr(), FIELD_TYPE_STR));
             ffi!(Py_DECREF(field_type));
             if !is_type!(field_type as *mut pyo3::ffi::PyTypeObject, FIELD_TYPE) {
                 continue;
             }
             let data = unicode_to_str(attr.as_ptr());
@@ -195,20 +211,25 @@
             let key_as_str = data.unwrap();
             if key_as_str.as_bytes()[0] == b'_' {
                 continue;
             }
 
             let value = ffi!(PyObject_GetAttr(self.ptr, attr.as_ptr()));
             ffi!(Py_DECREF(value));
-            let pyvalue = PyObjectSerializer::new(
-                value,
+            items.push((key_as_str, value));
+        }
+
+        let mut map = serializer.serialize_map(Some(items.len())).unwrap();
+        for (key, value) in items.iter() {
+            let pyvalue = PyObject::new(
+                *value,
                 self.opts,
                 self.default_calls,
                 self.recursion + 1,
                 self.default,
             );
-            map.serialize_key(key_as_str).unwrap();
+            map.serialize_key(key).unwrap();
             map.serialize_value(&pyvalue)?
         }
         map.end()
     }
 }
```

### Comparing `ormsgpack-1.4.2/src/serialize/default.rs` & `ormsgpack-1.5.0/src/serialize/default.rs`

 * *Files 6% similar despite different names*

```diff
@@ -11,41 +11,41 @@
 #[cold]
 #[inline(never)]
 fn format_err(ptr: *mut pyo3::ffi::PyObject) -> String {
     let name = unsafe { CStr::from_ptr((*ob_type!(ptr)).tp_name).to_string_lossy() };
     format_args!("Type is not msgpack serializable: {name}").to_string()
 }
 
-pub struct DefaultSerializer {
+pub struct Default {
     ptr: *mut pyo3::ffi::PyObject,
     opts: Opt,
     default_calls: u8,
     recursion: u8,
     default: Option<NonNull<pyo3::ffi::PyObject>>,
 }
 
-impl DefaultSerializer {
+impl Default {
     pub fn new(
         ptr: *mut pyo3::ffi::PyObject,
         opts: Opt,
         default_calls: u8,
         recursion: u8,
         default: Option<NonNull<pyo3::ffi::PyObject>>,
     ) -> Self {
-        DefaultSerializer {
+        Default {
             ptr: ptr,
             opts: opts,
             default_calls: default_calls,
             recursion: recursion,
             default: default,
         }
     }
 }
 
-impl Serialize for DefaultSerializer {
+impl Serialize for Default {
     #[inline(never)]
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
         match self.default {
             Some(callable) => {
@@ -57,15 +57,15 @@
                     callable.as_ptr(),
                     self.ptr,
                     std::ptr::null_mut() as *mut pyo3::ffi::PyObject
                 ));
                 if unlikely!(default_obj.is_null()) {
                     err!(format_err(self.ptr))
                 } else {
-                    let res = PyObjectSerializer::new(
+                    let res = PyObject::new(
                         default_obj,
                         self.opts,
                         self.default_calls + 1,
                         self.recursion,
                         self.default,
                     )
                     .serialize(serializer);
```

### Comparing `ormsgpack-1.4.2/src/serialize/dict.rs` & `ormsgpack-1.5.0/src/serialize/dict.rs`

 * *Files 19% similar despite different names*

```diff
@@ -7,109 +7,109 @@
 use crate::serialize::serializer::*;
 use crate::typeref::*;
 use crate::unicode::*;
 use serde::ser::{Serialize, SerializeMap, Serializer};
 use smallvec::SmallVec;
 use std::ptr::NonNull;
 
-pub struct DictGenericSerializer {
+pub struct Dict {
     ptr: *mut pyo3::ffi::PyObject,
     opts: Opt,
     default_calls: u8,
     recursion: u8,
     default: Option<NonNull<pyo3::ffi::PyObject>>,
 }
 
-impl DictGenericSerializer {
+impl Dict {
     pub fn new(
         ptr: *mut pyo3::ffi::PyObject,
         opts: Opt,
         default_calls: u8,
         recursion: u8,
         default: Option<NonNull<pyo3::ffi::PyObject>>,
     ) -> Self {
-        DictGenericSerializer {
+        Dict {
             ptr: ptr,
             opts: opts,
             default_calls: default_calls,
             recursion: recursion,
             default: default,
         }
     }
 }
 
-impl Serialize for DictGenericSerializer {
+impl Serialize for Dict {
     #[inline]
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
         if unlikely!(ffi!(Py_SIZE(self.ptr)) == 0) {
             serializer.serialize_map(Some(0)).unwrap().end()
         } else if self.opts & (NON_STR_KEYS | SORT_KEYS) == 0 {
-            Dict::new(
+            DictWithStrKeys::new(
                 self.ptr,
                 self.opts,
                 self.default_calls,
                 self.recursion,
                 self.default,
             )
             .serialize(serializer)
         } else if self.opts & NON_STR_KEYS != 0 {
             if self.opts & SORT_KEYS != 0 {
                 err!("OPT_NON_STR_KEYS is not compatible with OPT_SORT_KEYS")
             }
-            DictNonStrKey::new(
+            DictWithNonStrKeys::new(
                 self.ptr,
                 self.opts,
                 self.default_calls,
                 self.recursion,
                 self.default,
             )
             .serialize(serializer)
         } else {
-            DictSortedKey::new(
+            DictWithSortedStrKeys::new(
                 self.ptr,
                 self.opts,
                 self.default_calls,
                 self.recursion,
                 self.default,
             )
             .serialize(serializer)
         }
     }
 }
 
-pub struct Dict {
+pub struct DictWithStrKeys {
     ptr: *mut pyo3::ffi::PyObject,
     opts: Opt,
     default_calls: u8,
     recursion: u8,
     default: Option<NonNull<pyo3::ffi::PyObject>>,
 }
 
-impl Dict {
+impl DictWithStrKeys {
     pub fn new(
         ptr: *mut pyo3::ffi::PyObject,
         opts: Opt,
         default_calls: u8,
         recursion: u8,
         default: Option<NonNull<pyo3::ffi::PyObject>>,
     ) -> Self {
-        Dict {
+        DictWithStrKeys {
             ptr: ptr,
             opts: opts,
             default_calls: default_calls,
             recursion: recursion,
             default: default,
         }
     }
 }
 
-impl Serialize for Dict {
+impl Serialize for DictWithStrKeys {
     #[inline(always)]
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
         let len = ffi!(Py_SIZE(self.ptr)) as usize;
         let mut map = serializer.serialize_map(Some(len)).unwrap();
@@ -117,55 +117,55 @@
             if unlikely!(!is_type!(ob_type!(key.as_ptr()), STR_TYPE)) {
                 err!(KEY_MUST_BE_STR)
             }
             let data = unicode_to_str(key.as_ptr());
             if unlikely!(data.is_none()) {
                 err!(INVALID_STR)
             }
-            let pyvalue = PyObjectSerializer::new(
+            let pyvalue = PyObject::new(
                 value.as_ptr(),
                 self.opts,
                 self.default_calls,
                 self.recursion + 1,
                 self.default,
             );
             map.serialize_key(data.unwrap()).unwrap();
             map.serialize_value(&pyvalue)?;
         }
         map.end()
     }
 }
 
-pub struct DictSortedKey {
+pub struct DictWithSortedStrKeys {
     ptr: *mut pyo3::ffi::PyObject,
     opts: Opt,
     default_calls: u8,
     recursion: u8,
     default: Option<NonNull<pyo3::ffi::PyObject>>,
 }
 
-impl DictSortedKey {
+impl DictWithSortedStrKeys {
     pub fn new(
         ptr: *mut pyo3::ffi::PyObject,
         opts: Opt,
         default_calls: u8,
         recursion: u8,
         default: Option<NonNull<pyo3::ffi::PyObject>>,
     ) -> Self {
-        DictSortedKey {
+        DictWithSortedStrKeys {
             ptr: ptr,
             opts: opts,
             default_calls: default_calls,
             recursion: recursion,
             default: default,
         }
     }
 }
 
-impl Serialize for DictSortedKey {
+impl Serialize for DictWithSortedStrKeys {
     #[inline(never)]
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
         let len = ffi!(Py_SIZE(self.ptr)) as usize;
         let mut items: SmallVec<[(&str, *mut pyo3::ffi::PyObject); 8]> =
@@ -181,55 +181,55 @@
             items.push((data.unwrap(), value.as_ptr()));
         }
 
         items.sort_unstable_by(|a, b| a.0.cmp(b.0));
 
         let mut map = serializer.serialize_map(Some(len)).unwrap();
         for (key, val) in items.iter() {
-            let pyvalue = PyObjectSerializer::new(
+            let pyvalue = PyObject::new(
                 *val,
                 self.opts,
                 self.default_calls,
                 self.recursion + 1,
                 self.default,
             );
             map.serialize_key(key).unwrap();
             map.serialize_value(&pyvalue)?;
         }
         map.end()
     }
 }
 
-pub struct DictNonStrKey {
+pub struct DictWithNonStrKeys {
     ptr: *mut pyo3::ffi::PyObject,
     opts: Opt,
     default_calls: u8,
     recursion: u8,
     default: Option<NonNull<pyo3::ffi::PyObject>>,
 }
 
-impl DictNonStrKey {
+impl DictWithNonStrKeys {
     pub fn new(
         ptr: *mut pyo3::ffi::PyObject,
         opts: Opt,
         default_calls: u8,
         recursion: u8,
         default: Option<NonNull<pyo3::ffi::PyObject>>,
     ) -> Self {
-        DictNonStrKey {
+        DictWithNonStrKeys {
             ptr: ptr,
             opts: opts,
             default_calls: default_calls,
             recursion: recursion,
             default: default,
         }
     }
 }
 
-impl Serialize for DictNonStrKey {
+impl Serialize for DictWithNonStrKeys {
     #[inline(never)]
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
         let opts = self.opts & NOT_PASSTHROUGH;
         let len = ffi!(Py_SIZE(self.ptr)) as usize;
@@ -238,15 +238,15 @@
             if is_type!(ob_type!(key.as_ptr()), STR_TYPE) {
                 let data = unicode_to_str(key.as_ptr());
                 if unlikely!(data.is_none()) {
                     err!(INVALID_STR)
                 }
                 map.serialize_entry(
                     data.unwrap(),
-                    &PyObjectSerializer::new(
+                    &PyObject::new(
                         value.as_ptr(),
                         self.opts,
                         self.default_calls,
                         self.recursion + 1,
                         self.default,
                     ),
                 )?;
@@ -260,22 +260,22 @@
                     | ObType::Pydantic
                     | ObType::Unknown => {
                         err!("Dict key must a type serializable with OPT_NON_STR_KEYS")
                     }
                     _ => (),
                 }
                 map.serialize_entry(
-                    &PyObjectSerializer::new(
+                    &PyObject::new(
                         key.as_ptr(),
                         opts,
                         self.default_calls,
                         self.recursion + 1,
                         self.default,
                     ),
-                    &PyObjectSerializer::new(
+                    &PyObject::new(
                         value.as_ptr(),
                         self.opts,
                         self.default_calls,
                         self.recursion + 1,
                         self.default,
                     ),
                 )?;
```

### Comparing `ormsgpack-1.4.2/src/serialize/int.rs` & `ormsgpack-1.5.0/src/serialize/int.rs`

 * *Files 9% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 use crate::ffi::pylong_is_positive;
 use serde::ser::{Serialize, Serializer};
 
 // https://tools.ietf.org/html/rfc7159#section-6
 // "[-(2**53)+1, (2**53)-1]"
 
 #[repr(transparent)]
-pub struct IntSerializer {
+pub struct Int {
     ptr: *mut pyo3::ffi::PyObject,
 }
 
-impl IntSerializer {
+impl Int {
     pub fn new(ptr: *mut pyo3::ffi::PyObject) -> Self {
-        IntSerializer { ptr: ptr }
+        Int { ptr: ptr }
     }
 }
 
-impl Serialize for IntSerializer {
+impl Serialize for Int {
     #[inline]
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
         if pylong_is_positive(self.ptr) {
             let val = ffi!(PyLong_AsUnsignedLongLong(self.ptr));
```

### Comparing `ormsgpack-1.4.2/src/serialize/list.rs` & `ormsgpack-1.5.0/src/serialize/list.rs`

 * *Files 11% similar despite different names*

```diff
@@ -2,53 +2,51 @@
 
 use crate::opt::*;
 use crate::serialize::serializer::*;
 
 use serde::ser::{Serialize, SerializeSeq, Serializer};
 use std::ptr::NonNull;
 
-pub struct ListSerializer {
+pub struct List {
     ptr: *mut pyo3::ffi::PyObject,
     opts: Opt,
     default_calls: u8,
     recursion: u8,
     default: Option<NonNull<pyo3::ffi::PyObject>>,
 }
 
-impl ListSerializer {
+impl List {
     pub fn new(
         ptr: *mut pyo3::ffi::PyObject,
         opts: Opt,
         default_calls: u8,
         recursion: u8,
         default: Option<NonNull<pyo3::ffi::PyObject>>,
     ) -> Self {
-        ListSerializer {
+        List {
             ptr: ptr,
             opts: opts,
             default_calls: default_calls,
             recursion: recursion,
             default: default,
         }
     }
 }
 
-impl Serialize for ListSerializer {
+impl Serialize for List {
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
         let len = ffi!(PyList_GET_SIZE(self.ptr)) as usize;
         let mut seq = serializer.serialize_seq(Some(len)).unwrap();
-        let slice: &[*mut pyo3::ffi::PyObject] = unsafe {
-            std::slice::from_raw_parts((*(self.ptr as *mut pyo3::ffi::PyListObject)).ob_item, len)
-        };
-        for &each in slice {
-            let value = PyObjectSerializer::new(
-                each,
+        for i in 0..len {
+            let item = ffi!(PyList_GET_ITEM(self.ptr, i as isize));
+            let value = PyObject::new(
+                item,
                 self.opts,
                 self.default_calls,
                 self.recursion + 1,
                 self.default,
             );
             seq.serialize_element(&value)?;
         }
```

### Comparing `ormsgpack-1.4.2/src/serialize/serializer.rs` & `ormsgpack-1.5.0/src/serialize/serializer.rs`

 * *Files 3% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 use crate::serialize::list::*;
 use crate::serialize::numpy::*;
 use crate::serialize::str::*;
 use crate::serialize::tuple::*;
 use crate::serialize::uuid::*;
 use crate::serialize::writer::*;
 use crate::typeref::*;
-use serde::ser::{Serialize, SerializeSeq, Serializer};
+use serde::ser::{Serialize, Serializer};
 use std::ptr::NonNull;
 
 pub const RECURSION_LIMIT: u8 = 255;
 
 pub fn serialize(
     ptr: *mut pyo3::ffi::PyObject,
     default: Option<NonNull<pyo3::ffi::PyObject>>,
     opts: Opt,
 ) -> Result<NonNull<pyo3::ffi::PyObject>, String> {
     let mut buf = BytesWriter::default();
-    let obj = PyObjectSerializer::new(ptr, opts, 0, 0, default);
+    let obj = PyObject::new(ptr, opts, 0, 0, default);
     let mut ser = rmp_serde::Serializer::new(&mut buf);
     let res = obj.serialize(&mut ser);
     match res {
         Ok(_) => Ok(buf.finish()),
         Err(err) => {
             ffi!(_Py_Dealloc(buf.finish().as_ptr()));
             Err(err.to_string())
@@ -151,165 +151,165 @@
     } else if is_type!(ob_type, EXT_TYPE) {
         ObType::Ext
     } else {
         ObType::Unknown
     }
 }
 
-pub struct PyObjectSerializer {
+pub struct PyObject {
     ptr: *mut pyo3::ffi::PyObject,
     obtype: ObType,
     opts: Opt,
     default_calls: u8,
     recursion: u8,
     default: Option<NonNull<pyo3::ffi::PyObject>>,
 }
 
-impl PyObjectSerializer {
+impl PyObject {
     pub fn new(
         ptr: *mut pyo3::ffi::PyObject,
         opts: Opt,
         default_calls: u8,
         recursion: u8,
         default: Option<NonNull<pyo3::ffi::PyObject>>,
     ) -> Self {
-        PyObjectSerializer {
+        PyObject {
             ptr: ptr,
             obtype: pyobject_to_obtype(ptr, opts),
             opts: opts,
             default_calls: default_calls,
             recursion: recursion,
             default: default,
         }
     }
 }
 
-impl Serialize for PyObjectSerializer {
+impl Serialize for PyObject {
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
         match self.obtype {
-            ObType::Str => StrSerializer::new(self.ptr).serialize(serializer),
-            ObType::Bytes => BytesSerializer::new(self.ptr).serialize(serializer),
-            ObType::StrSubclass => StrSubclassSerializer::new(self.ptr).serialize(serializer),
-            ObType::Int => IntSerializer::new(self.ptr).serialize(serializer),
+            ObType::Str => Str::new(self.ptr).serialize(serializer),
+            ObType::Bytes => Bytes::new(self.ptr).serialize(serializer),
+            ObType::StrSubclass => StrSubclass::new(self.ptr).serialize(serializer),
+            ObType::Int => Int::new(self.ptr).serialize(serializer),
             ObType::None => serializer.serialize_unit(),
             ObType::Float => serializer.serialize_f64(ffi!(PyFloat_AS_DOUBLE(self.ptr))),
             ObType::Bool => serializer.serialize_bool(unsafe { self.ptr == TRUE }),
-            ObType::Datetime => DateTime::new(self.ptr, self.opts).serialize(serializer),
+            ObType::Datetime => match DateTime::new(self.ptr, self.opts) {
+                Ok(val) => val.serialize(serializer),
+                Err(err) => err!(err),
+            },
             ObType::Date => Date::new(self.ptr).serialize(serializer),
             ObType::Time => match Time::new(self.ptr, self.opts) {
                 Ok(val) => val.serialize(serializer),
-                Err(TimeError::HasTimezone) => err!(TIME_HAS_TZINFO),
+                Err(err) => err!(err),
             },
             ObType::Uuid => UUID::new(self.ptr).serialize(serializer),
             ObType::Dict => {
                 if unlikely!(self.recursion == RECURSION_LIMIT) {
                     err!(RECURSION_LIMIT_REACHED)
                 }
-                DictGenericSerializer::new(
+                Dict::new(
                     self.ptr,
                     self.opts,
                     self.default_calls,
                     self.recursion,
                     self.default,
                 )
                 .serialize(serializer)
             }
             ObType::List => {
                 if unlikely!(self.recursion == RECURSION_LIMIT) {
                     err!(RECURSION_LIMIT_REACHED)
                 }
-                if unlikely!(ffi!(PyList_GET_SIZE(self.ptr)) == 0) {
-                    serializer.serialize_seq(Some(0)).unwrap().end()
-                } else {
-                    ListSerializer::new(
-                        self.ptr,
-                        self.opts,
-                        self.default_calls,
-                        self.recursion,
-                        self.default,
-                    )
-                    .serialize(serializer)
+                List::new(
+                    self.ptr,
+                    self.opts,
+                    self.default_calls,
+                    self.recursion,
+                    self.default,
+                )
+                .serialize(serializer)
+            }
+            ObType::Tuple => {
+                if unlikely!(self.recursion == RECURSION_LIMIT) {
+                    err!(RECURSION_LIMIT_REACHED)
                 }
+                Tuple::new(
+                    self.ptr,
+                    self.opts,
+                    self.default_calls,
+                    self.recursion,
+                    self.default,
+                )
+                .serialize(serializer)
             }
-            ObType::Tuple => TupleSerializer::new(
-                self.ptr,
-                self.opts,
-                self.default_calls,
-                self.recursion,
-                self.default,
-            )
-            .serialize(serializer),
             ObType::Dataclass => {
                 if unlikely!(self.recursion == RECURSION_LIMIT) {
                     err!(RECURSION_LIMIT_REACHED)
                 }
-                DataclassGenericSerializer::new(
+                Dataclass::new(
                     self.ptr,
                     self.opts,
                     self.default_calls,
                     self.recursion,
                     self.default,
                 )
                 .serialize(serializer)
             }
             ObType::Pydantic => {
                 if unlikely!(self.recursion == RECURSION_LIMIT) {
                     err!(RECURSION_LIMIT_REACHED)
                 }
-                let dict = ffi!(PyObject_GetAttr(self.ptr, DICT_STR));
-                if unlikely!(dict.is_null()) {
-                    err!(PYDANTIC_MUST_HAVE_DICT)
-                } else {
-                    ffi!(Py_DECREF(dict));
-                    DataclassFastSerializer::new(
-                        dict,
-                        self.opts,
-                        self.default_calls,
-                        self.recursion,
-                        self.default,
-                    )
-                    .serialize(serializer)
+                match AttributeDict::new(
+                    self.ptr,
+                    self.opts,
+                    self.default_calls,
+                    self.recursion,
+                    self.default,
+                ) {
+                    Ok(val) => val.serialize(serializer),
+                    Err(AttributeDictError::DictMissing) => err!(PYDANTIC_MUST_HAVE_DICT),
                 }
             }
             ObType::Enum => {
                 let value = ffi!(PyObject_GetAttr(self.ptr, VALUE_STR));
                 ffi!(Py_DECREF(value));
-                PyObjectSerializer::new(
+                PyObject::new(
                     value,
                     self.opts,
                     self.default_calls,
                     self.recursion,
                     self.default,
                 )
                 .serialize(serializer)
             }
-            ObType::NumpyArray => match NumpyArray::new(self.ptr) {
+            ObType::NumpyArray => match NumpyArray::new(self.ptr, self.opts) {
                 Ok(val) => val.serialize(serializer),
                 Err(PyArrayError::Malformed) => err!("numpy array is malformed"),
                 Err(PyArrayError::NotContiguous) | Err(PyArrayError::UnsupportedDataType) => {
                     if self.default.is_none() {
                         err!("numpy array is not C contiguous; use ndarray.tolist() in default")
                     } else {
-                        DefaultSerializer::new(
+                        Default::new(
                             self.ptr,
                             self.opts,
                             self.default_calls,
                             self.recursion,
                             self.default,
                         )
                         .serialize(serializer)
                     }
                 }
             },
-            ObType::NumpyScalar => NumpyScalar::new(self.ptr).serialize(serializer),
-            ObType::Ext => ExtSerializer::new(self.ptr).serialize(serializer),
-            ObType::Unknown => DefaultSerializer::new(
+            ObType::NumpyScalar => NumpyScalar::new(self.ptr, self.opts).serialize(serializer),
+            ObType::Ext => Ext::new(self.ptr).serialize(serializer),
+            ObType::Unknown => Default::new(
                 self.ptr,
                 self.opts,
                 self.default_calls,
                 self.recursion,
                 self.default,
             )
             .serialize(serializer),
```

### Comparing `ormsgpack-1.4.2/src/serialize/tuple.rs` & `ormsgpack-1.5.0/src/serialize/tuple.rs`

 * *Files 12% similar despite different names*

```diff
@@ -2,56 +2,55 @@
 
 use crate::opt::*;
 use crate::serialize::serializer::*;
 
 use serde::ser::{Serialize, SerializeSeq, Serializer};
 use std::ptr::NonNull;
 
-pub struct TupleSerializer {
+pub struct Tuple {
     ptr: *mut pyo3::ffi::PyObject,
     opts: Opt,
     default_calls: u8,
     recursion: u8,
     default: Option<NonNull<pyo3::ffi::PyObject>>,
 }
 
-impl TupleSerializer {
+impl Tuple {
     pub fn new(
         ptr: *mut pyo3::ffi::PyObject,
         opts: Opt,
         default_calls: u8,
         recursion: u8,
         default: Option<NonNull<pyo3::ffi::PyObject>>,
     ) -> Self {
-        TupleSerializer {
+        Tuple {
             ptr: ptr,
             opts: opts,
             default_calls: default_calls,
             recursion: recursion,
             default: default,
         }
     }
 }
 
-impl Serialize for TupleSerializer {
+impl Serialize for Tuple {
     #[inline(never)]
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
         let len = ffi!(PyTuple_GET_SIZE(self.ptr)) as usize;
         let mut seq = serializer.serialize_seq(Some(len)).unwrap();
-        if len > 0 {
-            for i in 0..=len - 1 {
-                let elem = nonnull!(ffi!(PyTuple_GET_ITEM(self.ptr, i as isize)));
-                seq.serialize_element(&PyObjectSerializer::new(
-                    elem.as_ptr(),
-                    self.opts,
-                    self.default_calls,
-                    self.recursion + 1,
-                    self.default,
-                ))?
-            }
+        for i in 0..len {
+            let item = ffi!(PyTuple_GET_ITEM(self.ptr, i as isize));
+            let value = PyObject::new(
+                item,
+                self.opts,
+                self.default_calls,
+                self.recursion + 1,
+                self.default,
+            );
+            seq.serialize_element(&value)?;
         }
         seq.end()
     }
 }
```

### Comparing `ormsgpack-1.4.2/src/serialize/uuid.rs` & `ormsgpack-1.5.0/src/serialize/uuid.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.4.2/src/typeref.rs` & `ormsgpack-1.5.0/src/typeref.rs`

 * *Files 8% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 
 use crate::ext::create_ext_type;
 
 pub struct NumpyTypes {
     pub array: *mut PyTypeObject,
     pub float64: *mut PyTypeObject,
     pub float32: *mut PyTypeObject,
+    pub float16: *mut PyTypeObject,
     pub int64: *mut PyTypeObject,
     pub int32: *mut PyTypeObject,
     pub int16: *mut PyTypeObject,
     pub int8: *mut PyTypeObject,
     pub uint64: *mut PyTypeObject,
     pub uint32: *mut PyTypeObject,
     pub uint16: *mut PyTypeObject,
     pub uint8: *mut PyTypeObject,
     pub bool_: *mut PyTypeObject,
+    pub datetime64: *mut PyTypeObject,
 }
 
 pub static mut DEFAULT: *mut PyObject = null_mut();
 pub static mut EXT_HOOK: *mut PyObject = null_mut();
 pub static mut OPTION: *mut PyObject = null_mut();
 
 pub static mut NONE: *mut PyObject = null_mut();
@@ -61,14 +63,16 @@
 pub static mut DICT_STR: *mut PyObject = null_mut();
 pub static mut DATACLASS_FIELDS_STR: *mut PyObject = null_mut();
 pub static mut SLOTS_STR: *mut PyObject = null_mut();
 pub static mut PYDANTIC_FIELDS_STR: *mut PyObject = null_mut();
 pub static mut PYDANTIC2_FIELDS_STR: *mut PyObject = null_mut();
 pub static mut FIELD_TYPE_STR: *mut PyObject = null_mut();
 pub static mut ARRAY_STRUCT_STR: *mut PyObject = null_mut();
+pub static mut DTYPE_STR: *mut PyObject = null_mut();
+pub static mut DESCR_STR: *mut PyObject = null_mut();
 pub static mut VALUE_STR: *mut PyObject = null_mut();
 pub static mut INT_ATTR_STR: *mut PyObject = null_mut();
 
 pub static mut HASH_BUILDER: OnceBox<ahash::RandomState> = OnceBox::new();
 
 pub fn ahash_init() -> Box<ahash::RandomState> {
     unsafe {
@@ -141,59 +145,63 @@
         SLOTS_STR = PyUnicode_InternFromString("__slots__\0".as_ptr() as *const c_char);
         PYDANTIC_FIELDS_STR = PyUnicode_InternFromString("__fields__\0".as_ptr() as *const c_char);
         PYDANTIC2_FIELDS_STR =
             PyUnicode_InternFromString("model_fields\0".as_ptr() as *const c_char);
         FIELD_TYPE_STR = PyUnicode_InternFromString("_field_type\0".as_ptr() as *const c_char);
         ARRAY_STRUCT_STR =
             PyUnicode_InternFromString("__array_struct__\0".as_ptr() as *const c_char);
+        DTYPE_STR = PyUnicode_InternFromString("dtype\0".as_ptr() as *const c_char);
+        DESCR_STR = PyUnicode_InternFromString("descr\0".as_ptr() as *const c_char);
         VALUE_STR = PyUnicode_InternFromString("value\0".as_ptr() as *const c_char);
         DEFAULT = PyUnicode_InternFromString("default\0".as_ptr() as *const c_char);
         EXT_HOOK = PyUnicode_InternFromString("ext_hook\0".as_ptr() as *const c_char);
         OPTION = PyUnicode_InternFromString("option\0".as_ptr() as *const c_char);
         Py_INCREF(PyExc_TypeError);
         MsgpackEncodeError = PyExc_TypeError;
         Py_INCREF(PyExc_ValueError);
         MsgpackDecodeError = PyExc_ValueError;
 
         HASH_BUILDER.get_or_init(ahash_init);
     });
 }
 
 #[cold]
-unsafe fn look_up_numpy_type(numpy_module: *mut PyObject, np_type: &str) -> *mut PyTypeObject {
-    let mod_dict = PyObject_GenericGetDict(numpy_module, null_mut());
-    let ptr = PyMapping_GetItemString(mod_dict, np_type.as_ptr() as *const c_char);
+unsafe fn look_up_numpy_type(numpy_module_dict: *mut PyObject, np_type: &str) -> *mut PyTypeObject {
+    let ptr = PyMapping_GetItemString(numpy_module_dict, np_type.as_ptr() as *const c_char);
     Py_XDECREF(ptr);
-    Py_XDECREF(mod_dict);
     ptr as *mut PyTypeObject
 }
 
 #[cold]
 pub fn load_numpy_types() -> Box<Option<NonNull<NumpyTypes>>> {
     unsafe {
         let numpy = PyImport_ImportModule("numpy\0".as_ptr() as *const c_char);
         if numpy.is_null() {
             PyErr_Clear();
             return Box::new(None);
         }
 
+        let numpy_module_dict = PyObject_GenericGetDict(numpy, null_mut());
         let types = Box::new(NumpyTypes {
-            array: look_up_numpy_type(numpy, "ndarray\0"),
-            float32: look_up_numpy_type(numpy, "float32\0"),
-            float64: look_up_numpy_type(numpy, "float64\0"),
-            int8: look_up_numpy_type(numpy, "int8\0"),
-            int16: look_up_numpy_type(numpy, "int16\0"),
-            int32: look_up_numpy_type(numpy, "int32\0"),
-            int64: look_up_numpy_type(numpy, "int64\0"),
-            uint16: look_up_numpy_type(numpy, "uint16\0"),
-            uint32: look_up_numpy_type(numpy, "uint32\0"),
-            uint64: look_up_numpy_type(numpy, "uint64\0"),
-            uint8: look_up_numpy_type(numpy, "uint8\0"),
-            bool_: look_up_numpy_type(numpy, "bool_\0"),
+            array: look_up_numpy_type(numpy_module_dict, "ndarray\0"),
+            float16: look_up_numpy_type(numpy_module_dict, "half\0"),
+            float32: look_up_numpy_type(numpy_module_dict, "float32\0"),
+            float64: look_up_numpy_type(numpy_module_dict, "float64\0"),
+            int8: look_up_numpy_type(numpy_module_dict, "int8\0"),
+            int16: look_up_numpy_type(numpy_module_dict, "int16\0"),
+            int32: look_up_numpy_type(numpy_module_dict, "int32\0"),
+            int64: look_up_numpy_type(numpy_module_dict, "int64\0"),
+            uint16: look_up_numpy_type(numpy_module_dict, "uint16\0"),
+            uint32: look_up_numpy_type(numpy_module_dict, "uint32\0"),
+            uint64: look_up_numpy_type(numpy_module_dict, "uint64\0"),
+            uint8: look_up_numpy_type(numpy_module_dict, "uint8\0"),
+            bool_: look_up_numpy_type(numpy_module_dict, "bool_\0"),
+            datetime64: look_up_numpy_type(numpy_module_dict, "datetime64\0"),
         });
+        Py_XDECREF(numpy_module_dict);
         Py_XDECREF(numpy);
         Box::new(Some(nonnull!(Box::<NumpyTypes>::into_raw(types))))
     }
 }
 
 #[cold]
 unsafe fn look_up_field_type() -> *mut PyTypeObject {
```

### Comparing `ormsgpack-1.4.2/src/unicode.rs` & `ormsgpack-1.5.0/src/unicode.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.4.2/src/util.rs` & `ormsgpack-1.5.0/src/util.rs`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.4.2/Cargo.lock` & `ormsgpack-1.5.0/Cargo.lock`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "ahash"
-version = "0.8.7"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77c3a9648d43b9cd48db467b3f87fdd6e146bcc88ab0180006cef2179fe11d01"
+checksum = "e89da841a80418a9b391ebaea17f5c112ffaaa96f621d2c285b5174da76b9011"
 dependencies = [
  "cfg-if",
  "once_cell",
  "version_check",
  "zerocopy",
 ]
 
 [[package]]
+name = "any_all_workaround"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88fea40735f2cc320a5133ce772d39c571bd6c9b0d4c1a326926eecdd5af2e86"
+dependencies = [
+ "cfg-if",
+]
+
+[[package]]
 name = "associative-cache"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b993cd767a2bc7307dd87622311ca22c44329cc7a21366206bfa0896827b2bad"
 
 [[package]]
 name = "autocfg"
@@ -30,62 +39,78 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bytecount"
-version = "0.6.7"
+version = "0.6.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1e5f035d16fc623ae5f74981db80a439803888314e3a555fd6f04acd51a3205"
-dependencies = [
- "packed_simd",
-]
+checksum = "5ce89b21cab1437276d2650d57e971f9d548a2d9037cc231abdc0562b97498ce"
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "chrono"
+version = "0.4.38"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
+name = "crunchy"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
+
+[[package]]
 name = "encoding_rs"
-version = "0.8.33"
+version = "0.8.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7268b386296a025e474d5140678f75d6de9493ae55a5d709eeb9dd08149945e1"
+checksum = "b45de904aa0b010bce2ab45264d0631681847fa7b6f2eaa7dab7619943bc4f59"
 dependencies = [
+ "any_all_workaround",
  "cfg-if",
- "packed_simd",
+]
+
+[[package]]
+name = "half"
+version = "2.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6dd08c532ae367adf81c312a4580bc67f1d0fe8bc9c460520283f4c0ff277888"
+dependencies = [
+ "cfg-if",
+ "crunchy",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "libc"
 version = "0.2.151"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "302d7ab3130588088d277783b1e2d2e10c9e9e4a16dd9050e6ec93fb3e7048f4"
 
 [[package]]
-name = "libm"
-version = "0.2.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
-
-[[package]]
 name = "lock_api"
 version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
@@ -103,54 +128,44 @@
 [[package]]
 name = "num-traits"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "39e3200413f237f41ab11ad6d161bc7239c84dcb631773ccd7de3dfe4b5c267c"
 dependencies = [
  "autocfg",
- "libm",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "ormsgpack"
-version = "1.4.2"
+version = "1.5.0"
 dependencies = [
  "ahash",
  "associative-cache",
  "bytecount",
+ "chrono",
  "encoding_rs",
+ "half",
  "itoa",
  "once_cell",
  "pyo3",
  "pyo3-build-config",
  "rmp",
  "rmp-serde",
  "serde",
  "serde_bytes",
- "simdutf8",
  "smallvec",
 ]
 
 [[package]]
-name = "packed_simd"
-version = "0.3.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f9f08af0c877571712e2e3e686ad79efad9657dbf0f7c3c8ba943ff6c38932d"
-dependencies = [
- "cfg-if",
- "num-traits",
-]
-
-[[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
@@ -172,51 +187,58 @@
 [[package]]
 name = "paste"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.74"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2de98502f212cfcea8d0bb305bd0f49d7ebdd75b64ba0a68f937d888f4e0d6db"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a89dc7a5850d0e983be1ec2a463a171d20990487c3cfcd68b5363f1ee3d6fe0"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07426f0d8fe5a601f26293f300afd1a7b1ed5e78b2a705870c5f30893c5163be"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbb7dec17e17766b46bca4f1a4215a85006b4c2ecde122076c562dd058da6cf1"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "quote"
@@ -234,45 +256,45 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rmp"
-version = "0.8.12"
+version = "0.8.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f9860a6cc38ed1da53456442089b4dfa35e7cedaa326df63017af88385e6b20"
+checksum = "228ed7c16fa39782c3b3468e974aec2795e9089153cd08ee2e9aefb3613334c4"
 dependencies = [
  "byteorder",
  "num-traits",
  "paste",
 ]
 
 [[package]]
 name = "rmp-serde"
-version = "1.1.2"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bffea85eea980d8a74453e5d02a8d93028f3c34725de143085a844ebe953258a"
+checksum = "938a142ab806f18b88a97b0dea523d39e0fd730a064b035726adcfc58a8a5188"
 dependencies = [
  "byteorder",
  "rmp",
  "serde",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.195"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "63261df402c67811e9ac6def069e4786148c4563f4b50fd4bf30aa370d626b02"
+checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_bytes"
 version = "0.11.14"
@@ -280,34 +302,28 @@
 checksum = "8b8497c313fd43ab992087548117643f6fcd935cbf36f176ffda0aacf9591734"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.195"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46fe8f8603d81ba86327b23a2e9cdf49e1255fb94a4c5f297f6ee0547178ea2c"
+checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
-name = "simdutf8"
-version = "0.1.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
-
-[[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
 version = "2.0.46"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89456b690ff72fddcecf231caedbe615c59480c93358a93dfae7fc29e3ebbf0e"
 dependencies = [
```

### Comparing `ormsgpack-1.4.2/pyproject.toml` & `ormsgpack-1.5.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -26,16 +26,24 @@
 build-backend = "maturin"
 requires = ["maturin>=1.0,<2.0"]
 
 [tool.maturin]
 python-source = "python"
 strip = true
 
-[tool.black]
+[tool.ruff]
 line-length = 88
-target-version = ['py38', 'py39', 'py310', 'py311']
-include = '\.pyi?$'
+target-version = "py38"
 
-[tool.isort]
-line_length = 88
-profile = "black"
-skip_gitignore = true
+[tool.ruff.lint]
+select = [
+  "F",
+  "E",
+  "I",
+  "RUF",
+]
+ignore = [
+  "E501",
+]
+
+[tool.ruff.lint.isort]
+known-first-party = ["ormsgpack"]
```

### Comparing `ormsgpack-1.4.2/python/ormsgpack/__init__.pyi` & `ormsgpack-1.5.0/python/ormsgpack/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ormsgpack-1.4.2/PKG-INFO` & `ormsgpack-1.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ormsgpack
-Version: 1.4.2
+Version: 1.5.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
@@ -100,19 +100,19 @@
 ### Quickstart
 
 This is an example of serializing, with options specified, and deserializing:
 
 ```python
 >>> import ormsgpack, datetime, numpy
 >>> data = {
-    "type": "job",
-    "created_at": datetime.datetime(1970, 1, 1),
-    "status": "🆗",
-    "payload": numpy.array([[1, 2], [3, 4]]),
-}
+...     "type": "job",
+...     "created_at": datetime.datetime(1970, 1, 1),
+...     "status": "🆗",
+...     "payload": numpy.array([[1, 2], [3, 4]]),
+... }
 >>> ormsgpack.packb(data, option=ormsgpack.OPT_NAIVE_UTC | ormsgpack.OPT_SERIALIZE_NUMPY)
 b'\x84\xa4type\xa3job\xaacreated_at\xb91970-01-01T00:00:00+00:00\xa6status\xa4\xf0\x9f\x86\x97\xa7payload\x92\x92\x01\x02\x92\x03\x04'
 >>> ormsgpack.unpackb(_)
 {'type': 'job', 'created_at': '1970-01-01T00:00:00+00:00', 'status': '🆗', 'payload': [[1, 2], [3, 4]]}
 ```
 
 ### Serialize
@@ -166,104 +166,114 @@
 To serialize a subclass or arbitrary types, specify `default` as a
 callable that returns a supported type. `default` may be a function,
 lambda, or callable class instance. To specify that a type was not
 handled by `default`, raise an exception such as `TypeError`.
 
 ```python
 >>> import ormsgpack, decimal
->>>
-def default(obj):
-    if isinstance(obj, decimal.Decimal):
-        return str(obj)
-    raise TypeError
-
+>>> def default(obj):
+...     if isinstance(obj, decimal.Decimal):
+...         return str(obj)
+...     raise TypeError
+...
 >>> ormsgpack.packb(decimal.Decimal("0.0842389659712649442845"))
-MsgpackEncodeError: Type is not msgpack serializable: decimal.Decimal
+TypeError: Type is not msgpack serializable: decimal.Decimal
 >>> ormsgpack.packb(decimal.Decimal("0.0842389659712649442845"), default=default)
 b'\xb80.0842389659712649442845'
 >>> ormsgpack.packb({1, 2}, default=default)
-ormsgpack.MsgpackEncodeError: Type is not msgpack serializable: set
+TypeError: Type is not msgpack serializable: set
 ```
 
 The `default` callable may return an object that itself
 must be handled by `default` up to 254 times before an exception
 is raised.
 
 It is important that `default` raise an exception if a type cannot be handled.
 Python otherwise implicitly returns `None`, which appears to the caller
 like a legitimate value and is serialized:
 
 ```python
->>> import ormsgpack, json, rapidjson
->>>
-def default(obj):
-    if isinstance(obj, decimal.Decimal):
-        return str(obj)
-
->>> ormsgpack.unpackb(ormsgpack.packb({"set":{1, 2}}, default=default))
+>>> import ormsgpack, decimal
+>>> def default(obj):
+...     if isinstance(obj, decimal.Decimal):
+...         return str(obj)
+...
+>>> ormsgpack.packb({"set":{1, 2}}, default=default)
+b'\x81\xa3set\xc0'
+>>> ormsgpack.unpackb(_)
 {'set': None}
 ```
 
 To serialize a type as a MessagePack extension type, return an
 `ormsgpack.Ext` object. The instantiation arguments are an integer in
 the range `[0, 127]` and a `bytes` object, defining the type and
 value, respectively.
 
 ```python
 >>> import ormsgpack, decimal
->>>
-def default(obj):
-    if isinstance(obj, decimal.Decimal):
-        return ormsgpack.Ext(0, str(obj).encode())
-    raise TypeError
-
+>>> def default(obj):
+...     if isinstance(obj, decimal.Decimal):
+...         return ormsgpack.Ext(0, str(obj).encode())
+...     raise TypeError
+...
 >>> ormsgpack.packb(decimal.Decimal("0.0842389659712649442845"), default=default)
 b'\xc7\x18\x000.0842389659712649442845'
 ```
 
 #### option
 
 To modify how data is serialized, specify `option`. Each `option` is an integer
 constant in `ormsgpack`. To specify multiple options, mask them together, e.g.,
 `option=ormsgpack.OPT_NON_STR_KEYS | ormsgpack.OPT_NAIVE_UTC`.
 
 ##### OPT_NAIVE_UTC
 
-Serialize `datetime.datetime` objects without a `tzinfo` as UTC. This
-has no effect on `datetime.datetime` objects that have `tzinfo` set.
+Serialize `datetime.datetime` objects without a `tzinfo` and `numpy.datetime64`
+objects as UTC. This has no effect on `datetime.datetime` objects that have
+`tzinfo` set.
 
 ```python
 >>> import ormsgpack, datetime
->>> ormsgpack.unpackb(ormsgpack.packb(
-        datetime.datetime(1970, 1, 1, 0, 0, 0),
-    ))
-"1970-01-01T00:00:00"
->>> ormsgpack.unpackb(ormsgpack.packb(
-        datetime.datetime(1970, 1, 1, 0, 0, 0),
-        option=ormsgpack.OPT_NAIVE_UTC,
-    ))
-"1970-01-01T00:00:00+00:00"
+>>> ormsgpack.packb(
+...     datetime.datetime(1970, 1, 1, 0, 0, 0),
+... )
+b'\xb31970-01-01T00:00:00'
+>>> ormsgpack.unpackb(_)
+'1970-01-01T00:00:00'
+>>> ormsgpack.packb(
+...     datetime.datetime(1970, 1, 1, 0, 0, 0),
+...     option=ormsgpack.OPT_NAIVE_UTC,
+... )
+b'\xb91970-01-01T00:00:00+00:00'
+>>> ormsgpack.unpackb(_)
+'1970-01-01T00:00:00+00:00'
 ```
 
 ##### OPT_NON_STR_KEYS
 
 Serialize `dict` keys of type other than `str`. This allows `dict` keys
 to be one of `str`, `int`, `float`, `bool`, `None`, `datetime.datetime`,
 `datetime.date`, `datetime.time`, `enum.Enum`, and `uuid.UUID`.
 
 ```python
 >>> import ormsgpack, datetime, uuid
 >>> ormsgpack.packb(
-        {uuid.UUID("7202d115-7ff3-4c81-a7c1-2a1f067b1ece"): [1, 2, 3]},
-        option=ormsgpack.OPT_NON_STR_KEYS,
-    )
->>> ormsgpack.packb(
-        {datetime.datetime(1970, 1, 1, 0, 0, 0): [1, 2, 3]},
-        option=ormsgpack.OPT_NON_STR_KEYS | ormsgpack.OPT_NAIVE_UTC,
-    )
+...     {uuid.UUID("7202d115-7ff3-4c81-a7c1-2a1f067b1ece"): [1, 2, 3]},
+...     option=ormsgpack.OPT_NON_STR_KEYS,
+... )
+b'\x81\xd9$7202d115-7ff3-4c81-a7c1-2a1f067b1ece\x93\x01\x02\x03'
+>>> ormsgpack.unpackb(_)
+{'7202d115-7ff3-4c81-a7c1-2a1f067b1ece': [1, 2, 3]}
+>>> ormsgpack.packb(
+...     {datetime.datetime(1970, 1, 1, 0, 0, 0): [1, 2, 3]},
+...     option=ormsgpack.OPT_NON_STR_KEYS | ormsgpack.OPT_NAIVE_UTC,
+... )
+b'\x81\xb91970-01-01T00:00:00+00:00\x93\x01\x02\x03'
+>>> ormsgpack.unpackb(_)
+{'1970-01-01T00:00:00+00:00': [1, 2, 3]}
 ```
 
 These types are generally serialized how they would be as
 values, e.g., `datetime.datetime` is still an RFC 3339 string and respects
 options affecting it.
 
 This option has the risk of creating duplicate keys. This is because non-`str`
@@ -272,123 +282,126 @@
 The last key to be inserted to the `dict` will be serialized last and a msgpack deserializer will presumably take the last
 occurrence of a key (in the above, `false`). The first value will be lost.
 
 This option is not compatible with `ormsgpack.OPT_SORT_KEYS`.
 
 ##### OPT_OMIT_MICROSECONDS
 
-Do not serialize the `microsecond` field on `datetime.datetime` and
-`datetime.time` instances.
+Do not serialize the microsecond component of `datetime.datetime`,
+`datetime.time` and `numpy.datetime64` instances.
 
 ```python
 >>> import ormsgpack, datetime
 >>> ormsgpack.packb(
-        datetime.datetime(1970, 1, 1, 0, 0, 0, 1),
-    )
->>> ormsgpack.packb(
-        datetime.datetime(1970, 1, 1, 0, 0, 0, 1),
-        option=ormsgpack.OPT_OMIT_MICROSECONDS,
-    )
+...     datetime.datetime(1970, 1, 1, 0, 0, 0, 1),
+... )
+b'\xba1970-01-01T00:00:00.000001'
+>>> ormsgpack.unpackb(_)
+'1970-01-01T00:00:00.000001'
+>>> ormsgpack.packb(
+...     datetime.datetime(1970, 1, 1, 0, 0, 0, 1),
+...     option=ormsgpack.OPT_OMIT_MICROSECONDS,
+... )
+b'\xb31970-01-01T00:00:00'
+>>> ormsgpack.unpackb(_)
+'1970-01-01T00:00:00'
 ```
 
 ##### OPT_PASSTHROUGH_BIG_INT
 
 Enables passthrough of big (Python) ints. By setting this option, one can set a `default` function for ints larger than 63 bits, smaller ints are still serialized efficiently.
 
 ```python
 >>> import ormsgpack
 >>> ormsgpack.packb(
-        2**65,
-    )
+...     2**65,
+... )
 TypeError: Integer exceeds 64-bit range
->>> ormsgpack.unpackb(
-        ormsgpack.packb(
-            2**65,
-            option=ormsgpack.OPT_PASSTHROUGH_BIG_INT,
-            default=lambda _: {"type": "bigint", "value": str(_) }
-        )
-    )
+>>> ormsgpack.packb(
+...     2**65,
+...     option=ormsgpack.OPT_PASSTHROUGH_BIG_INT,
+...     default=lambda _: {"type": "bigint", "value": str(_) }
+... )
+b'\x82\xa4type\xa6bigint\xa5value\xb436893488147419103232'
+>>> ormsgpack.unpackb(_)
 {'type': 'bigint', 'value': '36893488147419103232'}
 ```
 
 ##### OPT_PASSTHROUGH_DATACLASS
 
 Passthrough `dataclasses.dataclass` instances to `default`. This allows
 customizing their output but is much slower.
 
 
 ```python
 >>> import ormsgpack, dataclasses
->>>
-@dataclasses.dataclass
-class User:
-    id: str
-    name: str
-    password: str
-
-def default(obj):
-    if isinstance(obj, User):
-        return {"id": obj.id, "name": obj.name}
-    raise TypeError
-
+>>> @dataclasses.dataclass
+... class User:
+...     id: str
+...     name: str
+...     password: str
+...
+>>> def default(obj):
+...     if isinstance(obj, User):
+...         return {"id": obj.id, "name": obj.name}
+...     raise TypeError
+...
 >>> ormsgpack.packb(User("3b1", "asd", "zxc"))
 b'\x83\xa2id\xa33b1\xa4name\xa3asd\xa8password\xa3zxc'
 >>> ormsgpack.packb(User("3b1", "asd", "zxc"), option=ormsgpack.OPT_PASSTHROUGH_DATACLASS)
 TypeError: Type is not msgpack serializable: User
 >>> ormsgpack.packb(
-        User("3b1", "asd", "zxc"),
-        option=ormsgpack.OPT_PASSTHROUGH_DATACLASS,
-        default=default,
-    )
+...     User("3b1", "asd", "zxc"),
+...     option=ormsgpack.OPT_PASSTHROUGH_DATACLASS,
+...     default=default,
+... )
 b'\x82\xa2id\xa33b1\xa4name\xa3asd'
 ```
 
 ##### OPT_PASSTHROUGH_DATETIME
 
 Passthrough `datetime.datetime`, `datetime.date`, and `datetime.time` instances
 to `default`. This allows serializing datetimes to a custom format, e.g.,
 HTTP dates:
 
 ```python
 >>> import ormsgpack, datetime
->>>
-def default(obj):
-    if isinstance(obj, datetime.datetime):
-        return obj.strftime("%a, %d %b %Y %H:%M:%S GMT")
-    raise TypeError
-
+>>> def default(obj):
+...     if isinstance(obj, datetime.datetime):
+...         return obj.strftime("%a, %d %b %Y %H:%M:%S GMT")
+...     raise TypeError
+...
 >>> ormsgpack.packb({"created_at": datetime.datetime(1970, 1, 1)})
 b'\x81\xaacreated_at\xb31970-01-01T00:00:00'
 >>> ormsgpack.packb({"created_at": datetime.datetime(1970, 1, 1)}, option=ormsgpack.OPT_PASSTHROUGH_DATETIME)
 TypeError: Type is not msgpack serializable: datetime.datetime
 >>> ormsgpack.packb(
-        {"created_at": datetime.datetime(1970, 1, 1)},
-        option=ormsgpack.OPT_PASSTHROUGH_DATETIME,
-        default=default,
-    )
+...     {"created_at": datetime.datetime(1970, 1, 1)},
+...     option=ormsgpack.OPT_PASSTHROUGH_DATETIME,
+...     default=default,
+... )
 b'\x81\xaacreated_at\xbdThu, 01 Jan 1970 00:00:00 GMT'
 ```
 
 This does not affect datetimes in `dict` keys if using OPT_NON_STR_KEYS.
 
 ##### OPT_PASSTHROUGH_SUBCLASS
 
 Passthrough subclasses of builtin types to `default`.
 
 ```python
 >>> import ormsgpack
->>>
-class Secret(str):
-    pass
-
-def default(obj):
-    if isinstance(obj, Secret):
-        return "******"
-    raise TypeError
-
+>>> class Secret(str):
+...     pass
+...
+>>> def default(obj):
+...     if isinstance(obj, Secret):
+...         return "******"
+...     raise TypeError
+...
 >>> ormsgpack.packb(Secret("zxc"))
 b'\xa3zxc'
 >>> ormsgpack.packb(Secret("zxc"), option=ormsgpack.OPT_PASSTHROUGH_SUBCLASS)
 TypeError: Type is not msgpack serializable: Secret
 >>> ormsgpack.packb(Secret("zxc"), option=ormsgpack.OPT_PASSTHROUGH_SUBCLASS, default=default)
 b'\xa6******'
 ```
@@ -398,27 +411,27 @@
 
 ##### OPT_PASSTHROUGH_TUPLE
 
 Passthrough tuples to `default`.
 
 ```python
 >>> import ormsgpack
->>> ormsgpack.unpackb(
-        ormsgpack.packb(
-            (9193, "test", 42),
-        )
-    )
+>>> ormsgpack.packb(
+...     (9193, "test", 42),
+... )
+b'\x93\xcd#\xe9\xa4test*'
+>>> ormsgpack.unpackb(_)
 [9193, 'test', 42]
->>> ormsgpack.unpackb(
-        ormsgpack.packb(
-            (9193, "test", 42),
-            option=ormsgpack.OPT_PASSTHROUGH_TUPLE,
-            default=lambda _: {"type": "tuple", "value": list(_)}
-        )
-    )
+>>> ormsgpack.packb(
+...     (9193, "test", 42),
+...     option=ormsgpack.OPT_PASSTHROUGH_TUPLE,
+...     default=lambda _: {"type": "tuple", "value": list(_)}
+... )
+b'\x82\xa4type\xa5tuple\xa5value\x93\xcd#\xe9\xa4test*'
+>>> ormsgpack.unpackb(_)
 {'type': 'tuple', 'value': [9193, 'test', 42]}
 ```
 
 ##### OPT_SERIALIZE_NUMPY
 
 Serialize `numpy.ndarray` instances. For more, see
 [numpy](#numpy).
@@ -450,28 +463,28 @@
 b'\x83\xa1A\x03\xa1a\x01\xa2\xc3\xa4\x02'
 ```
 
 `dataclass` also serialize as maps but this has no effect on them.
 
 ##### OPT_UTC_Z
 
-Serialize a UTC timezone on `datetime.datetime` instances as `Z` instead
-of `+00:00`.
+Serialize a UTC timezone on `datetime.datetime` and `numpy.datetime64` instances
+as `Z` instead of `+00:00`.
 
 ```python
 >>> import ormsgpack, datetime
 >>> ormsgpack.packb(
-        datetime.datetime(1970, 1, 1, 0, 0, 0, tzinfo=datetime.timezone.utc),
-    )
-b'"1970-01-01T00:00:00+00:00"'
->>> ormsgpack.packb(
-        datetime.datetime(1970, 1, 1, 0, 0, 0, tzinfo=datetime.timezone.utc),
-        option=ormsgpack.OPT_UTC_Z
-    )
-b'"1970-01-01T00:00:00Z"'
+...     datetime.datetime(1970, 1, 1, 0, 0, 0, tzinfo=datetime.timezone.utc),
+... )
+b'\xb91970-01-01T00:00:00+00:00'
+>>> ormsgpack.packb(
+...     datetime.datetime(1970, 1, 1, 0, 0, 0, tzinfo=datetime.timezone.utc),
+...     option=ormsgpack.OPT_UTC_Z
+... )
+b'\xb41970-01-01T00:00:00Z'
 ```
 
 ### Deserialize
 ```python
 def unpackb(
     __obj: Union[bytes, bytearray, memoryview],
     /,
@@ -500,25 +513,25 @@
 
 To deserialize extension types, specify the optional `ext_hook`
 argument. The value should be a callable and is invoked with the
 extension type and value as arguments.
 
 ```python
 >>> import ormsgpack, decimal
->>>
-def ext_hook(tag, data):
-    if tag == 0:
-        return decimal.Decimal(data.decode())
-    raise TypeError
-
+>>> def ext_hook(tag, data):
+...     if tag == 0:
+...         return decimal.Decimal(data.decode())
+...     raise TypeError
+...
 >>> ormsgpack.packb(
-    ormsgpack.Ext(0, str(decimal.Decimal("0.0842389659712649442845")).encode())
-)
+...     ormsgpack.Ext(0, str(decimal.Decimal("0.0842389659712649442845")).encode())
+... )
+b'\xc7\x18\x000.0842389659712649442845'
 >>> ormsgpack.unpackb(_, ext_hook=ext_hook)
-Decimal('0.0842389659712649442845')
+Decimal('0.0842389659712649442845'
 ```
 
 #### option
 `unpackb()` supports the `OPT_NON_STR_KEYS` option, that is similar to original msgpack's `strict_map_key=False`.
 Be aware that this option is considered unsafe and disabled by default in msgpack due to possibility of HashDoS.
 
 ## Types
@@ -535,26 +548,25 @@
 using `__slots__`.
 
 Dataclasses are serialized as maps, with every attribute serialized and in
 the order given on class definition:
 
 ```python
 >>> import dataclasses, ormsgpack, typing
-
-@dataclasses.dataclass
-class Member:
-    id: int
-    active: bool = dataclasses.field(default=False)
-
-@dataclasses.dataclass
-class Object:
-    id: int
-    name: str
-    members: typing.List[Member]
-
+>>> @dataclasses.dataclass
+... class Member:
+...     id: int
+...     active: bool = dataclasses.field(default=False)
+...
+>>> @dataclasses.dataclass
+... class Object:
+...     id: int
+...     name: str
+...     members: typing.List[Member]
+...
 >>> ormsgpack.packb(Object(1, "a", [Member(1, True), Member(2)]))
 b'\x83\xa2id\x01\xa4name\xa1a\xa7members\x92\x82\xa2id\x01\xa6active\xc3\x82\xa2id\x02\xa6active\xc2'
 ```
 #### Performance
 ![alt text](doc/dataclass.svg "dataclass")
 
 ```
@@ -572,51 +584,56 @@
 [RFC 3339](https://tools.ietf.org/html/rfc3339) format,
 e.g., "1970-01-01T00:00:00+00:00". This is a subset of ISO 8601 and is
 compatible with `isoformat()` in the standard library.
 
 ```python
 >>> import ormsgpack, datetime, zoneinfo
 >>> ormsgpack.packb(
-    datetime.datetime(2018, 12, 1, 2, 3, 4, 9, tzinfo=zoneinfo.ZoneInfo('Australia/Adelaide'))
-)
+...     datetime.datetime(2018, 12, 1, 2, 3, 4, 9, tzinfo=zoneinfo.ZoneInfo('Australia/Adelaide'))
+... )
+b'\xd9 2018-12-01T02:03:04.000009+10:30'
 >>> ormsgpack.unpackb(_)
-"2018-12-01T02:03:04.000009+10:30"
+'2018-12-01T02:03:04.000009+10:30'
 >>> ormsgpack.packb(
-    datetime.datetime.fromtimestamp(4123518902).replace(tzinfo=datetime.timezone.utc)
-)
+...     datetime.datetime.fromtimestamp(4123518902).replace(tzinfo=datetime.timezone.utc)
+... )
+b'\xb92100-09-02T00:55:02+00:00'
 >>> ormsgpack.unpackb(_)
-"2100-09-01T21:55:02+00:00"
+'2100-09-02T00:55:02+00:00'
 >>> ormsgpack.packb(
-    datetime.datetime.fromtimestamp(4123518902)
-)
+...     datetime.datetime.fromtimestamp(4123518902)
+... )
+b'\xb32100-09-02T00:55:02'
 >>> ormsgpack.unpackb(_)
-"2100-09-01T21:55:02"
+'2100-09-02T00:55:02'
 ```
 
 `datetime.datetime` supports instances with a `tzinfo` that is `None`,
 `datetime.timezone.utc`, a timezone instance from the python3.9+ `zoneinfo`
 module, or a timezone instance from the third-party `pendulum`, `pytz`, or
 `dateutil`/`arrow` libraries.
 
 `datetime.time` objects must not have a `tzinfo`.
 
 ```python
 >>> import ormsgpack, datetime
 >>> ormsgpack.packb(datetime.time(12, 0, 15, 290))
+b'\xaf12:00:15.000290'
 >>> ormsgpack.unpackb(_)
-"12:00:15.000290"
+'12:00:15.000290'
 ```
 
 `datetime.date` objects will always serialize.
 
 ```python
 >>> import ormsgpack, datetime
 >>> ormsgpack.packb(datetime.date(1900, 1, 2))
+b'\xaa1900-01-02'
 >>> ormsgpack.unpackb(_)
-"1900-01-02"
+'1900-01-02'
 ```
 
 Errors with `tzinfo` result in `MsgpackEncodeError` being raised.
 
 To disable serialization of `datetime` objects specify the option
 `ormsgpack.OPT_PASSTHROUGH_DATETIME`.
 
@@ -627,44 +644,46 @@
 
 ### enum
 
 ormsgpack serializes enums natively. Options apply to their values.
 
 ```python
 >>> import enum, datetime, ormsgpack
->>>
-class DatetimeEnum(enum.Enum):
-    EPOCH = datetime.datetime(1970, 1, 1, 0, 0, 0)
+>>> class DatetimeEnum(enum.Enum):
+...     EPOCH = datetime.datetime(1970, 1, 1, 0, 0, 0)
+...
 >>> ormsgpack.packb(DatetimeEnum.EPOCH)
+b'\xb31970-01-01T00:00:00'
 >>> ormsgpack.unpackb(_)
-"1970-01-01T00:00:00"
+'1970-01-01T00:00:00'
 >>> ormsgpack.packb(DatetimeEnum.EPOCH, option=ormsgpack.OPT_NAIVE_UTC)
+b'\xb91970-01-01T00:00:00+00:00'
 >>> ormsgpack.unpackb(_)
-"1970-01-01T00:00:00+00:00"
+'1970-01-01T00:00:00+00:00'
 ```
 
 Enums with members that are not supported types can be serialized using
 `default`:
 
 ```python
 >>> import enum, ormsgpack
->>>
-class Custom:
-    def __init__(self, val):
-        self.val = val
-
-def default(obj):
-    if isinstance(obj, Custom):
-        return obj.val
-    raise TypeError
-
-class CustomEnum(enum.Enum):
-    ONE = Custom(1)
-
+>>> class Custom:
+...     def __init__(self, val):
+...         self.val = val
+...
+>>> def default(obj):
+...     if isinstance(obj, Custom):
+...         return obj.val
+...     raise TypeError
+...
+>>> class CustomEnum(enum.Enum):
+...     ONE = Custom(1)
+...
 >>> ormsgpack.packb(CustomEnum.ONE, default=default)
+b'\x01'
 >>> ormsgpack.unpackb(_)
 1
 ```
 
 ### float
 
 ormsgpack serializes and deserializes double precision floats with no loss of
@@ -675,32 +694,35 @@
 ormsgpack serializes and deserializes 64-bit integers by default. The range
 supported is a signed 64-bit integer's minimum (-9223372036854775807) to
 an unsigned 64-bit integer's maximum (18446744073709551615).
 
 ### numpy
 
 ormsgpack natively serializes `numpy.ndarray` and individual
-`numpy.float64`, `numpy.float32`,
+`numpy.float64`, `numpy.float32`, `numpy.float16`,
 `numpy.int64`, `numpy.int32`, `numpy.int16`, `numpy.int8`,
 `numpy.uint64`, `numpy.uint32`, `numpy.uint16`, `numpy.uint8`,
-`numpy.uintp`, `numpy.intp`, and `numpy.bool`
+`numpy.uintp`, `numpy.intp`, `numpy.datetime64`, and `numpy.bool`
 instances.
 
+`numpy.datetime64` instances are serialized as RFC 3339 strings.
+
 ormsgpack is faster than all compared libraries at serializing
 numpy instances. Serializing numpy data requires specifying
 `option=ormsgpack.OPT_SERIALIZE_NUMPY`.
 
 ```python
 >>> import ormsgpack, numpy
 >>> ormsgpack.packb(
-        numpy.array([[1, 2, 3], [4, 5, 6]]),
-        option=ormsgpack.OPT_SERIALIZE_NUMPY,
-)
+...     numpy.array([[1, 2, 3], [4, 5, 6]]),
+...     option=ormsgpack.OPT_SERIALIZE_NUMPY,
+... )
+b'\x92\x93\x01\x02\x03\x93\x04\x05\x06'
 >>> ormsgpack.unpackb(_)
-[[1,2,3],[4,5,6]]
+[[1, 2, 3], [4, 5, 6]]
 ```
 
 The array must be a contiguous C array (`C_CONTIGUOUS`) and one of the
 supported datatypes.
 
 If an array is not a contiguous C array or contains an supported datatype,
 ormsgpack falls through to `default`. In `default`, `obj.tolist()` can be
@@ -756,22 +778,24 @@
 
 ### uuid
 
 ormsgpack serializes `uuid.UUID` instances to
 [RFC 4122](https://tools.ietf.org/html/rfc4122) format, e.g.,
 "f81d4fae-7dec-11d0-a765-00a0c91e6bf6".
 
-``` python
+```python
 >>> import ormsgpack, uuid
 >>> ormsgpack.packb(uuid.UUID('f81d4fae-7dec-11d0-a765-00a0c91e6bf6'))
+b'\xd9$f81d4fae-7dec-11d0-a765-00a0c91e6bf6'
 >>> ormsgpack.unpackb(_)
-"f81d4fae-7dec-11d0-a765-00a0c91e6bf6"
+'f81d4fae-7dec-11d0-a765-00a0c91e6bf6'
 >>> ormsgpack.packb(uuid.uuid5(uuid.NAMESPACE_DNS, "python.org"))
+b'\xd9$886313e1-3b8a-5372-9b90-0c9aee199e5d'
 >>> ormsgpack.unpackb(_)
-"886313e1-3b8a-5372-9b90-0c9aee199e5d"
+'886313e1-3b8a-5372-9b90-0c9aee199e5d
 ```
 
 ### Pydantic
 ormsgpack serializes `pydantic.BaseModel` instances natively.
 
 #### Performance
 ![alt text](doc/pydantic.svg "pydantic")
```

