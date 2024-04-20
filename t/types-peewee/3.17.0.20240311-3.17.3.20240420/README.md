# Comparing `tmp/types-peewee-3.17.0.20240311.tar.gz` & `tmp/types-peewee-3.17.3.20240420.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-peewee-3.17.0.20240311.tar", last modified: Mon Mar 11 02:15:56 2024, max compression
+gzip compressed data, was "types-peewee-3.17.3.20240420.tar", last modified: Sat Apr 20 02:15:03 2024, max compression
```

## Comparing `types-peewee-3.17.0.20240311.tar` & `types-peewee-3.17.3.20240420.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:15:56.385576 types-peewee-3.17.0.20240311/
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-03-11 02:15:55.000000 types-peewee-3.17.0.20240311/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-11 02:15:55.000000 types-peewee-3.17.0.20240311/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-03-11 02:15:56.385576 types-peewee-3.17.0.20240311/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:15:56.385576 types-peewee-3.17.0.20240311/peewee-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-11 02:15:55.000000 types-peewee-3.17.0.20240311/peewee-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)    62306 2024-03-11 02:15:55.000000 types-peewee-3.17.0.20240311/peewee-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 02:15:56.385576 types-peewee-3.17.0.20240311/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-11 02:15:55.000000 types-peewee-3.17.0.20240311/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:15:56.385576 types-peewee-3.17.0.20240311/types_peewee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-03-11 02:15:56.000000 types-peewee-3.17.0.20240311/types_peewee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-11 02:15:56.000000 types-peewee-3.17.0.20240311/types_peewee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 02:15:56.000000 types-peewee-3.17.0.20240311/types_peewee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-11 02:15:56.000000 types-peewee-3.17.0.20240311/types_peewee.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:15:03.676123 types-peewee-3.17.3.20240420/
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-20 02:15:03.000000 types-peewee-3.17.3.20240420/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-20 02:15:03.000000 types-peewee-3.17.3.20240420/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-20 02:15:03.676123 types-peewee-3.17.3.20240420/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:15:03.676123 types-peewee-3.17.3.20240420/peewee-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-20 02:15:03.000000 types-peewee-3.17.3.20240420/peewee-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    63254 2024-04-20 02:15:03.000000 types-peewee-3.17.3.20240420/peewee-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 02:15:03.000000 types-peewee-3.17.3.20240420/peewee-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 02:15:03.676123 types-peewee-3.17.3.20240420/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-20 02:15:03.000000 types-peewee-3.17.3.20240420/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:15:03.676123 types-peewee-3.17.3.20240420/types_peewee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-20 02:15:03.000000 types-peewee-3.17.3.20240420/types_peewee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-20 02:15:03.000000 types-peewee-3.17.3.20240420/types_peewee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 02:15:03.000000 types-peewee-3.17.3.20240420/types_peewee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-20 02:15:03.000000 types-peewee-3.17.3.20240420/types_peewee.egg-info/top_level.txt
```

### Comparing `types-peewee-3.17.0.20240311/CHANGELOG.md` & `types-peewee-3.17.3.20240420/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 3.17.3.20240420 (2024-04-20)
+
+Bump peewee to 3.17.3 and fix stubtest entries (#11787)
+
 ## 3.17.0.20240311 (2024-03-11)
 
 Use PEP 570 syntax in third party stubs (#11554)
 
 ## 3.17.0.20240207 (2024-02-07)
 
 Pin peewee more tightly for stubtest (#11372)
```

### Comparing `types-peewee-3.17.0.20240311/PKG-INFO` & `types-peewee-3.17.3.20240420/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-peewee
-Version: 3.17.0.20240311
+Version: 3.17.3.20240420
 Summary: Typing stubs for peewee
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/peewee.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `peewee`.
 
 This version of `types-peewee` aims to provide accurate annotations
-for `peewee==3.17.0`.
+for `peewee==3.17.3`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/peewee. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `57f3dcac8dbed008479b251512975901a0206deb` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-peewee-3.17.0.20240311/peewee-stubs/__init__.pyi` & `types-peewee-3.17.3.20240420/peewee-stubs/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import itertools
 import logging
 import threading
 from _typeshed import Incomplete, SupportsKeysAndGetItem
-from collections.abc import Callable, Generator, Iterable
+from collections.abc import Callable, Generator, Iterable, Iterator
 from types import TracebackType
-from typing import Any, ClassVar, NamedTuple, TypeVar
+from typing import Any, ClassVar, Literal, NamedTuple, TypeVar
 from typing_extensions import Self
 
 class NullHandler(logging.Handler):
     def emit(self, record) -> None: ...
 
 text_type = str
 bytes_type = bytes
@@ -124,27 +124,31 @@
 
 class _DynamicColumn:
     def __get__(self, instance, instance_type: Incomplete | None = ...): ...
 
 class _ExplicitColumn:
     def __get__(self, instance, instance_type: Incomplete | None = ...): ...
 
+class Star(Node):
+    def __init__(self, source) -> None: ...
+    def __sql__(self, ctx): ...
+
 class Source(Node):
     c: Incomplete
     def __init__(self, alias: Incomplete | None = ...) -> None: ...
     def alias(self, name) -> None: ...
     def select(self, *columns): ...
+    @property
+    def __star__(self) -> Star: ...
     def join(self, dest, join_type=..., on: Incomplete | None = ...): ...
     def left_outer_join(self, dest, on: Incomplete | None = ...): ...
     def cte(self, name, recursive: bool = ..., columns: Incomplete | None = ..., materialized: Incomplete | None = ...): ...
     def get_sort_key(self, ctx): ...
     def apply_alias(self, ctx): ...
     def apply_column(self, ctx): ...
-    @property
-    def star(self) -> NodeList: ...
 
 class _HashableSource:
     def __init__(self, *args, **kwargs) -> None: ...
     def alias(self, name) -> None: ...
     def __hash__(self) -> int: ...
     def __eq__(self, other) -> bool: ...
     def __ne__(self, other) -> bool: ...
@@ -1226,18 +1230,27 @@
     def __init__(self, *args, **kwargs) -> None: ...
     def flag(self, value: Incomplete | None = ...): ...
 
 class BigBitFieldData:
     instance: Incomplete
     name: Incomplete
     def __init__(self, instance, name) -> None: ...
+    def clear(self) -> None: ...
     def set_bit(self, idx) -> None: ...
     def clear_bit(self, idx) -> None: ...
     def toggle_bit(self, idx): ...
     def is_set(self, idx): ...
+    __getitem__ = is_set
+    def __setitem__(self, item: int, value: bool) -> None: ...
+    __delitem__ = clear_bit
+    def __len__(self) -> int: ...
+    def __and__(self, other: BigBitFieldData | bytes | bytearray | memoryview) -> bytearray: ...
+    def __or__(self, other: BigBitFieldData | bytes | bytearray | memoryview) -> bytearray: ...
+    def __xor__(self, other: BigBitFieldData | bytes | bytearray | memoryview) -> bytearray: ...
+    def __iter__(self) -> Iterator[Literal[0, 1]]: ...
     def __bytes__(self) -> bytes: ...
 
 class BigBitFieldAccessor(FieldAccessor):
     def __get__(self, instance, instance_type: Incomplete | None = ...): ...
     def __set__(self, instance, value) -> None: ...
 
 class BigBitField(BlobField):
@@ -1261,57 +1274,75 @@
 
 class DateTimeField(_BaseFormattedField):
     field_type: str
     formats: Incomplete
     def adapt(self, value): ...
     def to_timestamp(self): ...
     def truncate(self, part): ...
-    year: Incomplete
-    month: Incomplete
-    day: Incomplete
-    hour: Incomplete
-    minute: Incomplete
-    second: Incomplete
+    @property
+    def year(self): ...
+    @property
+    def month(self): ...
+    @property
+    def day(self): ...
+    @property
+    def hour(self): ...
+    @property
+    def minute(self): ...
+    @property
+    def second(self): ...
 
 class DateField(_BaseFormattedField):
     field_type: str
     formats: Incomplete
     def adapt(self, value): ...
     def to_timestamp(self): ...
     def truncate(self, part): ...
-    year: Incomplete
-    month: Incomplete
-    day: Incomplete
+    @property
+    def year(self): ...
+    @property
+    def month(self): ...
+    @property
+    def day(self): ...
 
 class TimeField(_BaseFormattedField):
     field_type: str
     formats: Incomplete
     def adapt(self, value): ...
-    hour: Incomplete
-    minute: Incomplete
-    second: Incomplete
+    @property
+    def hour(self): ...
+    @property
+    def minute(self): ...
+    @property
+    def second(self): ...
 
 class TimestampField(BigIntegerField):
     valid_resolutions: Incomplete
     resolution: Incomplete
     ticks_to_microsecond: Incomplete
     utc: Incomplete
     def __init__(self, *args, **kwargs) -> None: ...
     def local_to_utc(self, dt): ...
     def utc_to_local(self, dt): ...
     def get_timestamp(self, value): ...
     def db_value(self, value): ...
     def python_value(self, value): ...
     def from_timestamp(self): ...
-    year: Incomplete
-    month: Incomplete
-    day: Incomplete
-    hour: Incomplete
-    minute: Incomplete
-    second: Incomplete
+    @property
+    def year(self): ...
+    @property
+    def month(self): ...
+    @property
+    def day(self): ...
+    @property
+    def hour(self): ...
+    @property
+    def minute(self): ...
+    @property
+    def second(self): ...
 
 class IPField(BigIntegerField):
     def db_value(self, val): ...
     def python_value(self, val): ...
 
 class BooleanField(Field):
     field_type: str
```

### Comparing `types-peewee-3.17.0.20240311/setup.py` & `types-peewee-3.17.3.20240420/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,40 +11,40 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `peewee`.
 
 This version of `types-peewee` aims to provide accurate annotations
-for `peewee==3.17.0`.
+for `peewee==3.17.3`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/peewee. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `57f3dcac8dbed008479b251512975901a0206deb` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="3.17.0.20240311",
+      version="3.17.3.20240420",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/peewee.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['peewee-stubs'],
-      package_data={'peewee-stubs': ['__init__.pyi', 'METADATA.toml']},
+      package_data={'peewee-stubs': ['__init__.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-peewee-3.17.0.20240311/types_peewee.egg-info/PKG-INFO` & `types-peewee-3.17.3.20240420/types_peewee.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-peewee
-Version: 3.17.0.20240311
+Version: 3.17.3.20240420
 Summary: Typing stubs for peewee
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/peewee.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `peewee`.
 
 This version of `types-peewee` aims to provide accurate annotations
-for `peewee==3.17.0`.
+for `peewee==3.17.3`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/peewee. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `57f3dcac8dbed008479b251512975901a0206deb` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

