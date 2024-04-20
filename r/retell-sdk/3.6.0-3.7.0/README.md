# Comparing `tmp/retell_sdk-3.6.0.tar.gz` & `tmp/retell_sdk-3.7.0.tar.gz`

## Comparing `retell_sdk-3.6.0.tar` & `retell_sdk-3.7.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/__init__.py
--rw-r--r--   0        0        0    64275 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_base_client.py
--rw-r--r--   0        0        0    15337 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_constants.py
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_files.py
--rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_qs.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_resource.py
--rw-r--r--   0        0        0    28375 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_response.py
--rw-r--r--   0        0        0    10100 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_streaming.py
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_types.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/py.typed
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_utils/__init__.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_utils/_typing.py
--rw-r--r--   0        0        0    11105 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/lib/.keep
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/resources/__init__.py
--rw-r--r--   0        0        0    42897 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/resources/agent.py
--rw-r--r--   0        0        0    25014 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/resources/call.py
--rw-r--r--   0        0        0    26571 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/resources/llm.py
--rw-r--r--   0        0        0    17883 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/resources/phone_number.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/__init__.py
--rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/agent_create_params.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/agent_list_response.py
--rw-r--r--   0        0        0     5663 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/agent_response.py
--rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/agent_update_params.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/call_create_params.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/call_list_params.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/call_list_response.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/call_register_params.py
--rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/call_response.py
--rw-r--r--   0        0        0    17703 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/llm_create_params.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/llm_list_response.py
--rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/llm_response.py
--rw-r--r--   0        0        0    17703 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/llm_update_params.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/phone_number_create_params.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/phone_number_list_response.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/phone_number_response.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/phone_number_update_params.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell/types/register_call_response.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell_ai/lib/.keep
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/retell_sdk/lib/.keep
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/src/toddlzt/lib/.keep
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/.gitignore
--rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/LICENSE
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/pyproject.toml
--rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 retell_sdk-3.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/__init__.py
+-rw-r--r--   0        0        0    64254 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_base_client.py
+-rw-r--r--   0        0        0    15337 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_constants.py
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_files.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_qs.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_resource.py
+-rw-r--r--   0        0        0    28375 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_response.py
+-rw-r--r--   0        0        0    10100 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_streaming.py
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_types.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_utils/__init__.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/lib/.keep
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/resources/__init__.py
+-rw-r--r--   0        0        0    43021 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/resources/agent.py
+-rw-r--r--   0        0        0    25014 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/resources/call.py
+-rw-r--r--   0        0        0    26571 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/resources/llm.py
+-rw-r--r--   0        0        0    17883 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/resources/phone_number.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/__init__.py
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/agent_create_params.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/agent_list_response.py
+-rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/agent_response.py
+-rw-r--r--   0        0        0     5329 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/agent_update_params.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/call_create_params.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/call_list_params.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/call_list_response.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/call_register_params.py
+-rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/call_response.py
+-rw-r--r--   0        0        0    17703 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/llm_create_params.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/llm_list_response.py
+-rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/llm_response.py
+-rw-r--r--   0        0        0    17703 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/llm_update_params.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/phone_number_create_params.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/phone_number_list_response.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/phone_number_response.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/phone_number_update_params.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell/types/register_call_response.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell_ai/lib/.keep
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/retell_sdk/lib/.keep
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/src/toddlzt/lib/.keep
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/.gitignore
+-rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/LICENSE
+-rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/pyproject.toml
+-rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 retell_sdk-3.7.0/PKG-INFO
```

### Comparing `retell_sdk-3.6.0/src/retell/__init__.py` & `retell_sdk-3.7.0/src/retell/__init__.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/_base_client.py` & `retell_sdk-3.7.0/src/retell/_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     Iterator,
     Optional,
     Generator,
     AsyncIterator,
     cast,
     overload,
 )
-from functools import lru_cache
 from typing_extensions import Literal, override, get_origin
 
 import anyio
 import httpx
 import distro
 import pydantic
 from httpx import URL, Limits
@@ -57,15 +56,15 @@
     ProxiesTypes,
     RequestFiles,
     HttpxSendArgs,
     AsyncTransport,
     RequestOptions,
     ModelBuilderProtocol,
 )
-from ._utils import is_dict, is_list, is_given, is_mapping
+from ._utils import is_dict, is_list, is_given, lru_cache, is_mapping
 from ._compat import model_copy, model_dump
 from ._models import GenericModel, FinalRequestOptions, validate_type, construct_type
 from ._response import (
     APIResponse,
     BaseAPIResponse,
     AsyncAPIResponse,
     extract_response_type,
```

### Comparing `retell_sdk-3.6.0/src/retell/_client.py` & `retell_sdk-3.7.0/src/retell/_client.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/_compat.py` & `retell_sdk-3.7.0/src/retell/_compat.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/_exceptions.py` & `retell_sdk-3.7.0/src/retell/_exceptions.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/_files.py` & `retell_sdk-3.7.0/src/retell/_files.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/_models.py` & `retell_sdk-3.7.0/src/retell/_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import os
 import inspect
 from typing import TYPE_CHECKING, Any, Type, Union, Generic, TypeVar, Callable, cast
 from datetime import date, datetime
-from functools import lru_cache
 from typing_extensions import (
     Unpack,
     Literal,
     ClassVar,
     Protocol,
     Required,
     TypedDict,
@@ -33,14 +32,15 @@
     AnyMapping,
     HttpxRequestFiles,
 )
 from ._utils import (
     PropertyInfo,
     is_list,
     is_given,
+    lru_cache,
     is_mapping,
     parse_date,
     coerce_boolean,
     parse_datetime,
     strip_not_given,
     extract_type_arg,
     is_annotated_type,
@@ -374,15 +374,15 @@
     """
     # we allow `object` as the input type because otherwise, passing things like
     # `Literal['value']` will be reported as a type error by type checkers
     type_ = cast("type[object]", type_)
 
     # unwrap `Annotated[T, ...]` -> `T`
     if is_annotated_type(type_):
-        meta = get_args(type_)[1:]
+        meta: tuple[Any, ...] = get_args(type_)[1:]
         type_ = extract_type_arg(type_, 0)
     else:
         meta = tuple()
 
     # we need to use the origin class for any types that are subscripted generics
     # e.g. Dict[str, object]
     origin = get_origin(type_) or type_
```

### Comparing `retell_sdk-3.6.0/src/retell/_qs.py` & `retell_sdk-3.7.0/src/retell/_qs.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/_resource.py` & `retell_sdk-3.7.0/src/retell/_resource.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/_response.py` & `retell_sdk-3.7.0/src/retell/_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/_streaming.py` & `retell_sdk-3.7.0/src/retell/_streaming.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/_types.py` & `retell_sdk-3.7.0/src/retell/_types.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/_utils/__init__.py` & `retell_sdk-3.7.0/src/retell/_utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from ._proxy import LazyProxy as LazyProxy
 from ._utils import (
     flatten as flatten,
     is_dict as is_dict,
     is_list as is_list,
     is_given as is_given,
     is_tuple as is_tuple,
+    lru_cache as lru_cache,
     is_mapping as is_mapping,
     is_tuple_t as is_tuple_t,
     parse_date as parse_date,
     is_iterable as is_iterable,
     is_sequence as is_sequence,
     coerce_float as coerce_float,
     is_mapping_t as is_mapping_t,
```

### Comparing `retell_sdk-3.6.0/src/retell/_utils/_logs.py` & `retell_sdk-3.7.0/src/retell/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/_utils/_proxy.py` & `retell_sdk-3.7.0/src/retell/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/_utils/_sync.py` & `retell_sdk-3.7.0/src/retell/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/_utils/_transform.py` & `retell_sdk-3.7.0/src/retell/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/_utils/_typing.py` & `retell_sdk-3.7.0/src/retell/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/_utils/_utils.py` & `retell_sdk-3.7.0/src/retell/_utils/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,14 +261,16 @@
             else:  # no break
                 if len(variants) > 1:
                     variations = human_join(
                         ["(" + human_join([quote(arg) for arg in variant], final="and") + ")" for variant in variants]
                     )
                     msg = f"Missing required arguments; Expected either {variations} arguments to be given"
                 else:
+                    assert len(variants) > 0
+
                     # TODO: this error message is not deterministic
                     missing = list(set(variants[0]) - given_params)
                     if len(missing) > 1:
                         msg = f"Missing required arguments: {human_join([quote(arg) for arg in missing])}"
                     else:
                         msg = f"Missing required argument: {quote(missing[0])}"
                 raise TypeError(msg)
@@ -385,7 +387,17 @@
 
 
 def get_async_library() -> str:
     try:
         return sniffio.current_async_library()
     except Exception:
         return "false"
+
+
+def lru_cache(*, maxsize: int | None = 128) -> Callable[[CallableT], CallableT]:
+    """A version of functools.lru_cache that retains the type signature
+    for the wrapped function arguments.
+    """
+    wrapper = functools.lru_cache(  # noqa: TID251
+        maxsize=maxsize,
+    )
+    return cast(Any, wrapper)  # type: ignore[no-any-return]
```

### Comparing `retell_sdk-3.6.0/src/retell/resources/__init__.py` & `retell_sdk-3.7.0/src/retell/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/resources/agent.py` & `retell_sdk-3.7.0/src/retell/resources/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,17 @@
         ambient_sound: Optional[
             Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor", "static-noise"]
         ]
         | NotGiven = NOT_GIVEN,
         boosted_keywords: Optional[List[str]] | NotGiven = NOT_GIVEN,
         enable_backchannel: bool | NotGiven = NOT_GIVEN,
         interruption_sensitivity: float | NotGiven = NOT_GIVEN,
-        language: Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR"]
+        language: Literal[
+            "en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR", "fr-FR"
+        ]
         | NotGiven = NOT_GIVEN,
         opt_out_sensitive_data_storage: bool | NotGiven = NOT_GIVEN,
         responsiveness: float | NotGiven = NOT_GIVEN,
         voice_speed: float | NotGiven = NOT_GIVEN,
         voice_temperature: float | NotGiven = NOT_GIVEN,
         webhook_url: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
@@ -231,15 +233,17 @@
         ambient_sound: Optional[
             Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor", "static-noise"]
         ]
         | NotGiven = NOT_GIVEN,
         boosted_keywords: Optional[List[str]] | NotGiven = NOT_GIVEN,
         enable_backchannel: bool | NotGiven = NOT_GIVEN,
         interruption_sensitivity: float | NotGiven = NOT_GIVEN,
-        language: Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR"]
+        language: Literal[
+            "en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR", "fr-FR"
+        ]
         | NotGiven = NOT_GIVEN,
         llm_websocket_url: str | NotGiven = NOT_GIVEN,
         opt_out_sensitive_data_storage: bool | NotGiven = NOT_GIVEN,
         responsiveness: float | NotGiven = NOT_GIVEN,
         voice_id: str | NotGiven = NOT_GIVEN,
         voice_speed: float | NotGiven = NOT_GIVEN,
         voice_temperature: float | NotGiven = NOT_GIVEN,
@@ -452,15 +456,17 @@
         ambient_sound: Optional[
             Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor", "static-noise"]
         ]
         | NotGiven = NOT_GIVEN,
         boosted_keywords: Optional[List[str]] | NotGiven = NOT_GIVEN,
         enable_backchannel: bool | NotGiven = NOT_GIVEN,
         interruption_sensitivity: float | NotGiven = NOT_GIVEN,
-        language: Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR"]
+        language: Literal[
+            "en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR", "fr-FR"
+        ]
         | NotGiven = NOT_GIVEN,
         opt_out_sensitive_data_storage: bool | NotGiven = NOT_GIVEN,
         responsiveness: float | NotGiven = NOT_GIVEN,
         voice_speed: float | NotGiven = NOT_GIVEN,
         voice_temperature: float | NotGiven = NOT_GIVEN,
         webhook_url: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
@@ -637,15 +643,17 @@
         ambient_sound: Optional[
             Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor", "static-noise"]
         ]
         | NotGiven = NOT_GIVEN,
         boosted_keywords: Optional[List[str]] | NotGiven = NOT_GIVEN,
         enable_backchannel: bool | NotGiven = NOT_GIVEN,
         interruption_sensitivity: float | NotGiven = NOT_GIVEN,
-        language: Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR"]
+        language: Literal[
+            "en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR", "fr-FR"
+        ]
         | NotGiven = NOT_GIVEN,
         llm_websocket_url: str | NotGiven = NOT_GIVEN,
         opt_out_sensitive_data_storage: bool | NotGiven = NOT_GIVEN,
         responsiveness: float | NotGiven = NOT_GIVEN,
         voice_id: str | NotGiven = NOT_GIVEN,
         voice_speed: float | NotGiven = NOT_GIVEN,
         voice_temperature: float | NotGiven = NOT_GIVEN,
```

### Comparing `retell_sdk-3.6.0/src/retell/resources/call.py` & `retell_sdk-3.7.0/src/retell/resources/call.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/resources/llm.py` & `retell_sdk-3.7.0/src/retell/resources/llm.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/resources/phone_number.py` & `retell_sdk-3.7.0/src/retell/resources/phone_number.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/types/__init__.py` & `retell_sdk-3.7.0/src/retell/types/__init__.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/types/agent_create_params.py` & `retell_sdk-3.7.0/src/retell/types/agent_create_params.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,15 +71,17 @@
 
     Value ranging from [0,1]. Lower value means it will take longer / more words for
     user to interrupt agent, while higher value means it's easier for user to
     interrupt agent. If unset, default value 1 will apply. When this is set to 0,
     agent would never be interrupted.
     """
 
-    language: Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR"]
+    language: Literal[
+        "en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR", "fr-FR"
+    ]
     """`Beta feature, use with caution.`
 
     This setting specifies the agent's operational language, including base language
     and dialect. Speech recognition considers both elements, but text-to-speech
     currently only recognizes the base language.
 
     For instance, selecting `en-GB` optimizes speech recognition for British
```

### Comparing `retell_sdk-3.6.0/src/retell/types/agent_response.py` & `retell_sdk-3.7.0/src/retell/types/agent_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     Value ranging from [0,1]. Lower value means it will take longer / more words for
     user to interrupt agent, while higher value means it's easier for user to
     interrupt agent. If unset, default value 1 will apply. When this is set to 0,
     agent would never be interrupted.
     """
 
     language: Optional[
-        Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR"]
+        Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR", "fr-FR"]
     ] = None
     """`Beta feature, use with caution.`
 
     This setting specifies the agent's operational language, including base language
     and dialect. Speech recognition considers both elements, but text-to-speech
     currently only recognizes the base language.
```

### Comparing `retell_sdk-3.6.0/src/retell/types/agent_update_params.py` & `retell_sdk-3.7.0/src/retell/types/agent_update_params.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,17 @@
 
     Value ranging from [0,1]. Lower value means it will take longer / more words for
     user to interrupt agent, while higher value means it's easier for user to
     interrupt agent. If unset, default value 1 will apply. When this is set to 0,
     agent would never be interrupted.
     """
 
-    language: Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR"]
+    language: Literal[
+        "en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR", "fr-FR"
+    ]
     """`Beta feature, use with caution.`
 
     This setting specifies the agent's operational language, including base language
     and dialect. Speech recognition considers both elements, but text-to-speech
     currently only recognizes the base language.
 
     For instance, selecting `en-GB` optimizes speech recognition for British
```

### Comparing `retell_sdk-3.6.0/src/retell/types/call_create_params.py` & `retell_sdk-3.7.0/src/retell/types/call_create_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/types/call_list_params.py` & `retell_sdk-3.7.0/src/retell/types/call_list_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/types/call_register_params.py` & `retell_sdk-3.7.0/src/retell/types/call_register_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/types/call_response.py` & `retell_sdk-3.7.0/src/retell/types/call_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/types/llm_create_params.py` & `retell_sdk-3.7.0/src/retell/types/llm_create_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/types/llm_response.py` & `retell_sdk-3.7.0/src/retell/types/llm_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/types/llm_update_params.py` & `retell_sdk-3.7.0/src/retell/types/llm_update_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/types/phone_number_create_params.py` & `retell_sdk-3.7.0/src/retell/types/phone_number_create_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/types/phone_number_response.py` & `retell_sdk-3.7.0/src/retell/types/phone_number_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/src/retell/types/register_call_response.py` & `retell_sdk-3.7.0/src/retell/types/register_call_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/LICENSE` & `retell_sdk-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.6.0/pyproject.toml` & `retell_sdk-3.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "retell-sdk"
-version = "3.6.0"
+version = "3.7.0"
 description = "The official Python library for the retell API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Retell", email = "founders@retellai.com" },
 ]
 dependencies = [
@@ -44,15 +44,15 @@
 
 
 
 [tool.rye]
 managed = true
 # version pins are in requirements-dev.lock
 dev-dependencies = [
-    "pyright",
+    "pyright>=1.1.359",
     "mypy",
     "respx",
     "pytest",
     "pytest-asyncio",
     "ruff",
     "time-machine",
     "nox",
@@ -157,15 +157,17 @@
   "E722",
   # unused arguments
   "ARG",
   # print statements
   "T201",
   "T203",
   # misuse of typing.TYPE_CHECKING
-  "TCH004"
+  "TCH004",
+  # import rules
+  "TID251",
 ]
 ignore = [
   # mutable defaults
   "B006",
 ]
 unfixable = [
   # disable auto fix for print statements
@@ -173,14 +175,17 @@
   "T203",
 ]
 ignore-init-module-imports = true
 
 [tool.ruff.format]
 docstring-code-format = true
 
+[tool.ruff.lint.flake8-tidy-imports.banned-api]
+"functools.lru_cache".msg = "This function does not retain type information for the wrapped function's arguments; The `lru_cache` function from `_utils` should be used instead"
+
 [tool.ruff.lint.isort]
 length-sort = true
 length-sort-straight = true
 combine-as-imports = true
 extra-standard-library = ["typing_extensions"]
 known-first-party = ["retell", "tests"]
```

### Comparing `retell_sdk-3.6.0/PKG-INFO` & `retell_sdk-3.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: retell-sdk
-Version: 3.6.0
+Version: 3.7.0
 Summary: The official Python library for the retell API
 Project-URL: Homepage, https://github.com/RetellAI/retell-python-sdk
 Project-URL: Repository, https://github.com/RetellAI/retell-python-sdk
 Author-email: Retell <founders@retellai.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -54,17 +54,15 @@
 ## Usage
 
 The full API of this library can be found in [api.md](https://github.com/RetellAI/retell-python-sdk/tree/main/api.md).
 
 ```python
 from retell import Retell
 
-client = Retell(
-    api_key="YOUR_RETELL_API_KEY",
-)
+client = Retell()
 
 agent_response = client.agent.create(
     llm_websocket_url="wss://your-websocket-endpoint",
     voice_id="11labs-Adrian",
 )
 print(agent_response.agent_id)
 ```
@@ -73,17 +71,15 @@
 
 Simply import `AsyncRetell` instead of `Retell` and use `await` with each API call:
 
 ```python
 import asyncio
 from retell import AsyncRetell
 
-client = AsyncRetell(
-    api_key="YOUR_RETELL_API_KEY",
-)
+client = AsyncRetell()
 
 
 async def main() -> None:
     agent_response = await client.agent.create(
         llm_websocket_url="wss://your-websocket-endpoint",
         voice_id="11labs-Adrian",
     )
```

