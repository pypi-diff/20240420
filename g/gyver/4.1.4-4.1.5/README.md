# Comparing `tmp/gyver-4.1.4.tar.gz` & `tmp/gyver-4.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gyver-4.1.4.tar", max compression
+gzip compressed data, was "gyver-4.1.5.tar", max compression
```

## Comparing `gyver-4.1.4.tar` & `gyver-4.1.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1079 2024-03-28 22:08:41.323819 gyver-4.1.4/LICENSE
--rw-r--r--   0        0        0      610 2024-03-28 22:08:41.323819 gyver-4.1.4/README.md
--rw-r--r--   0        0        0      158 2024-04-19 02:04:59.979793 gyver-4.1.4/gyver/__init__.py
--rw-r--r--   0        0        0      795 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/config/__init__.py
--rw-r--r--   0        0        0       78 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/config/adapter/__init__.py
--rw-r--r--   0        0        0     1315 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/config/adapter/attrs.py
--rw-r--r--   0        0        0     1065 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/config/adapter/dataclass.py
--rw-r--r--   0        0        0     7939 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/config/adapter/factory.py
--rw-r--r--   0        0        0     1043 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/config/adapter/gattrs.py
--rw-r--r--   0        0        0     6716 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/config/adapter/helpers.py
--rw-r--r--   0        0        0     2111 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/config/adapter/interface.py
--rw-r--r--   0        0        0     2014 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/config/adapter/mark.py
--rw-r--r--   0        0        0     2105 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/config/adapter/pydantic.py
--rw-r--r--   0        0        0      419 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/context/__init__.py
--rw-r--r--   0        0        0      288 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/context/atomic_/__init__.py
--rw-r--r--   0        0        0     3880 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/context/atomic_/bound.py
--rw-r--r--   0        0        0     2358 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/context/atomic_/core.py
--rw-r--r--   0        0        0     2734 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/context/atomic_/resolver.py
--rw-r--r--   0        0        0     5447 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/context/context.py
--rw-r--r--   0        0        0      102 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/context/interfaces/__init__.py
--rw-r--r--   0        0        0     1984 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/context/interfaces/adapter.py
--rw-r--r--   0        0        0       39 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/context/typedef.py
--rw-r--r--   0        0        0     2667 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/exc.py
--rw-r--r--   0        0        0      225 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/filetree/__init__.py
--rw-r--r--   0        0        0     1748 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/filetree/filetree.py
--rw-r--r--   0        0        0      348 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/filetree/helpers.py
--rw-r--r--   0        0        0     3248 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/filetree/interface.py
--rw-r--r--   0        0        0     2865 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/filetree/typedef.py
--rw-r--r--   0        0        0     2808 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/filetree/virtual.py
--rw-r--r--   0        0        0      111 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/model/__init__.py
--rw-r--r--   0        0        0     1804 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/model/v1.py
--rw-r--r--   0        0        0     1793 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/model/v2.py
--rw-r--r--   0        0        0      101 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/pools/__init__.py
--rw-r--r--   0        0        0     5764 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/pools/asyncio.py
--rw-r--r--   0        0        0     2225 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/pools/resource.py
--rw-r--r--   0        0        0     3855 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/pools/thread.py
--rw-r--r--   0        0        0        0 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/py.typed
--rw-r--r--   0        0        0      186 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/url/__init__.py
--rw-r--r--   0        0        0     7211 2024-04-18 22:41:50.880985 gyver-4.1.4/gyver/url/core.py
--rw-r--r--   0        0        0      423 2024-04-18 20:01:32.234522 gyver-4.1.4/gyver/url/encode.py
--rw-r--r--   0        0        0     1631 2024-04-18 22:41:41.627434 gyver-4.1.4/gyver/url/fragment.py
--rw-r--r--   0        0        0     5027 2024-04-19 02:03:56.058338 gyver-4.1.4/gyver/url/netloc.py
--rw-r--r--   0        0        0     4830 2024-04-18 22:40:58.819756 gyver-4.1.4/gyver/url/path.py
--rw-r--r--   0        0        0     4022 2024-04-18 22:42:15.161559 gyver-4.1.4/gyver/url/query.py
--rw-r--r--   0        0        0     1186 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/url/utils.py
--rw-r--r--   0        0        0      579 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/utils/__init__.py
--rw-r--r--   0        0        0     1041 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/utils/exc.py
--rw-r--r--   0        0        0    12855 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/utils/finder.py
--rw-r--r--   0        0        0     4941 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/utils/helpers.py
--rw-r--r--   0        0        0     1669 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/utils/json.py
--rw-r--r--   0        0        0     2749 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/utils/strings.py
--rw-r--r--   0        0        0     1100 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/utils/timezone.py
--rw-r--r--   0        0        0     1623 2024-04-19 02:04:59.993127 gyver-4.1.4/pyproject.toml
--rw-r--r--   0        0        0     1571 1970-01-01 00:00:00.000000 gyver-4.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-03-28 22:08:41.323819 gyver-4.1.5/LICENSE
+-rw-r--r--   0        0        0      610 2024-03-28 22:08:41.323819 gyver-4.1.5/README.md
+-rw-r--r--   0        0        0      158 2024-04-20 20:07:15.940224 gyver-4.1.5/gyver/__init__.py
+-rw-r--r--   0        0        0      795 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/config/__init__.py
+-rw-r--r--   0        0        0       78 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/config/adapter/__init__.py
+-rw-r--r--   0        0        0     1315 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/config/adapter/attrs.py
+-rw-r--r--   0        0        0     1065 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/config/adapter/dataclass.py
+-rw-r--r--   0        0        0     7939 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/config/adapter/factory.py
+-rw-r--r--   0        0        0     1043 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/config/adapter/gattrs.py
+-rw-r--r--   0        0        0     6716 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/config/adapter/helpers.py
+-rw-r--r--   0        0        0     2111 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/config/adapter/interface.py
+-rw-r--r--   0        0        0     2014 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/config/adapter/mark.py
+-rw-r--r--   0        0        0     2105 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/config/adapter/pydantic.py
+-rw-r--r--   0        0        0      419 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/context/__init__.py
+-rw-r--r--   0        0        0      288 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/context/atomic_/__init__.py
+-rw-r--r--   0        0        0     3880 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/context/atomic_/bound.py
+-rw-r--r--   0        0        0     2358 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/context/atomic_/core.py
+-rw-r--r--   0        0        0     2734 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/context/atomic_/resolver.py
+-rw-r--r--   0        0        0     5447 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/context/context.py
+-rw-r--r--   0        0        0      102 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/context/interfaces/__init__.py
+-rw-r--r--   0        0        0     1984 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/context/interfaces/adapter.py
+-rw-r--r--   0        0        0       39 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/context/typedef.py
+-rw-r--r--   0        0        0     2667 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/exc.py
+-rw-r--r--   0        0        0      225 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/filetree/__init__.py
+-rw-r--r--   0        0        0     1748 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/filetree/filetree.py
+-rw-r--r--   0        0        0      348 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/filetree/helpers.py
+-rw-r--r--   0        0        0     3248 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/filetree/interface.py
+-rw-r--r--   0        0        0     2865 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/filetree/typedef.py
+-rw-r--r--   0        0        0     2808 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/filetree/virtual.py
+-rw-r--r--   0        0        0      111 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/model/__init__.py
+-rw-r--r--   0        0        0     1804 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/model/v1.py
+-rw-r--r--   0        0        0     1793 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/model/v2.py
+-rw-r--r--   0        0        0      101 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/pools/__init__.py
+-rw-r--r--   0        0        0     5764 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/pools/asyncio.py
+-rw-r--r--   0        0        0     2225 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/pools/resource.py
+-rw-r--r--   0        0        0     3855 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/pools/thread.py
+-rw-r--r--   0        0        0        0 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/py.typed
+-rw-r--r--   0        0        0      186 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/url/__init__.py
+-rw-r--r--   0        0        0     7211 2024-04-18 22:41:50.880985 gyver-4.1.5/gyver/url/core.py
+-rw-r--r--   0        0        0      423 2024-04-18 20:01:32.234522 gyver-4.1.5/gyver/url/encode.py
+-rw-r--r--   0        0        0     1631 2024-04-18 22:41:41.627434 gyver-4.1.5/gyver/url/fragment.py
+-rw-r--r--   0        0        0     5027 2024-04-19 02:03:56.058338 gyver-4.1.5/gyver/url/netloc.py
+-rw-r--r--   0        0        0     4830 2024-04-18 22:40:58.819756 gyver-4.1.5/gyver/url/path.py
+-rw-r--r--   0        0        0     4022 2024-04-18 22:42:15.161559 gyver-4.1.5/gyver/url/query.py
+-rw-r--r--   0        0        0     1186 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/url/utils.py
+-rw-r--r--   0        0        0      579 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/utils/__init__.py
+-rw-r--r--   0        0        0     1041 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/utils/exc.py
+-rw-r--r--   0        0        0    12855 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/utils/finder.py
+-rw-r--r--   0        0        0     4762 2024-04-20 18:11:24.474173 gyver-4.1.5/gyver/utils/helpers.py
+-rw-r--r--   0        0        0     1676 2024-04-20 18:13:47.304318 gyver-4.1.5/gyver/utils/json.py
+-rw-r--r--   0        0        0     2749 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/utils/strings.py
+-rw-r--r--   0        0        0     1100 2024-03-28 22:08:41.327153 gyver-4.1.5/gyver/utils/timezone.py
+-rw-r--r--   0        0        0     1623 2024-04-20 20:07:15.950224 gyver-4.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1571 1970-01-01 00:00:00.000000 gyver-4.1.5/PKG-INFO
```

### Comparing `gyver-4.1.4/LICENSE` & `gyver-4.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/README.md` & `gyver-4.1.5/README.md`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/config/__init__.py` & `gyver-4.1.5/gyver/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/config/adapter/attrs.py` & `gyver-4.1.5/gyver/config/adapter/attrs.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/config/adapter/dataclass.py` & `gyver-4.1.5/gyver/config/adapter/dataclass.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/config/adapter/factory.py` & `gyver-4.1.5/gyver/config/adapter/factory.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/config/adapter/gattrs.py` & `gyver-4.1.5/gyver/config/adapter/gattrs.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/config/adapter/helpers.py` & `gyver-4.1.5/gyver/config/adapter/helpers.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/config/adapter/interface.py` & `gyver-4.1.5/gyver/config/adapter/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/config/adapter/mark.py` & `gyver-4.1.5/gyver/config/adapter/mark.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/config/adapter/pydantic.py` & `gyver-4.1.5/gyver/config/adapter/pydantic.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/context/atomic_/bound.py` & `gyver-4.1.5/gyver/context/atomic_/bound.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/context/atomic_/core.py` & `gyver-4.1.5/gyver/context/atomic_/core.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/context/atomic_/resolver.py` & `gyver-4.1.5/gyver/context/atomic_/resolver.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/context/context.py` & `gyver-4.1.5/gyver/context/context.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/context/interfaces/adapter.py` & `gyver-4.1.5/gyver/context/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/exc.py` & `gyver-4.1.5/gyver/exc.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/filetree/filetree.py` & `gyver-4.1.5/gyver/filetree/filetree.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/filetree/interface.py` & `gyver-4.1.5/gyver/filetree/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/filetree/typedef.py` & `gyver-4.1.5/gyver/filetree/typedef.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/filetree/virtual.py` & `gyver-4.1.5/gyver/filetree/virtual.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/model/v1.py` & `gyver-4.1.5/gyver/model/v1.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/model/v2.py` & `gyver-4.1.5/gyver/model/v2.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/pools/asyncio.py` & `gyver-4.1.5/gyver/pools/asyncio.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/pools/resource.py` & `gyver-4.1.5/gyver/pools/resource.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/pools/thread.py` & `gyver-4.1.5/gyver/pools/thread.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/url/core.py` & `gyver-4.1.5/gyver/url/core.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/url/fragment.py` & `gyver-4.1.5/gyver/url/fragment.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/url/netloc.py` & `gyver-4.1.5/gyver/url/netloc.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/url/path.py` & `gyver-4.1.5/gyver/url/path.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/url/query.py` & `gyver-4.1.5/gyver/url/query.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/url/utils.py` & `gyver-4.1.5/gyver/url/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/utils/__init__.py` & `gyver-4.1.5/gyver/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/utils/exc.py` & `gyver-4.1.5/gyver/utils/exc.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/utils/finder.py` & `gyver-4.1.5/gyver/utils/finder.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/utils/helpers.py` & `gyver-4.1.5/gyver/utils/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import functools
 import warnings
 from collections import deque
 from collections.abc import Callable
 from itertools import chain
 from typing import TYPE_CHECKING, Literal, TypeVar, cast
-from weakref import WeakValueDictionary
 
 from typing_extensions import ParamSpec
 
-from gyver.attrs import define, info
 from gyver.exc import MergeConflict
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
 def cache(f: Callable[P, T]) -> Callable[P, T]:
@@ -142,12 +140,7 @@
                 )
             elif on_conflict == "left":
                 output_curr[key] = left_curr[key]
             else:
                 output_curr[key] = value
 
     return output
-
-
-@define
-class Cached:
-    _mapping: WeakValueDictionary = info(default_factory=WeakValueDictionary)
```

### Comparing `gyver-4.1.4/gyver/utils/json.py` & `gyver-4.1.5/gyver/utils/json.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         val (typing.Any): The Python object to be serialized.
         default (typing.Any, optional): A default value to be used if an object is not serializable.
             Defaults to None.
 
     Returns:
         str: The JSON-formatted string representing the serialized object.
     """
-    return orjson.dumps(val, default=default).decode()
+    return orjson.dumps(val, default=default).decode("utf-8")
 
 
 def load(fdes: typing.TextIO) -> str:
     """
     Deserialize a JSON-formatted string from a text file object.
 
     Args:
```

### Comparing `gyver-4.1.4/gyver/utils/strings.py` & `gyver-4.1.5/gyver/utils/strings.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/gyver/utils/timezone.py` & `gyver-4.1.5/gyver/utils/timezone.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.4/pyproject.toml` & `gyver-4.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gyver"
-version = "4.1.4"
+version = "4.1.5"
 description = "Toolbox for web development"
 authors = ["Gustavo Correa <self.gustavocorrea@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/guscardvs/gyver"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gyver-4.1.4/PKG-INFO` & `gyver-4.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gyver
-Version: 4.1.4
+Version: 4.1.5
 Summary: Toolbox for web development
 Home-page: https://github.com/guscardvs/gyver
 Author: Gustavo Correa
 Author-email: self.gustavocorrea@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

