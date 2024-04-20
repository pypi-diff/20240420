# Comparing `tmp/pydantic_marshals-0.3.8.tar.gz` & `tmp/pydantic_marshals-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_marshals-0.3.8.tar", max compression
+gzip compressed data, was "pydantic_marshals-0.3.9.tar", max compression
```

## Comparing `pydantic_marshals-0.3.8.tar` & `pydantic_marshals-0.3.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0        0 2023-07-24 18:26:24.247220 pydantic_marshals-0.3.8/pydantic_marshals/__init__.py
--rw-r--r--   0        0        0      124 2023-10-07 11:52:12.574783 pydantic_marshals-0.3.8/pydantic_marshals/base/__init__.py
--rw-r--r--   0        0        0        0 2023-09-19 21:57:54.653062 pydantic_marshals-0.3.8/pydantic_marshals/base/fields/__init__.py
--rw-r--r--   0        0        0     3529 2023-10-07 13:07:30.804019 pydantic_marshals-0.3.8/pydantic_marshals/base/fields/base.py
--rw-r--r--   0        0        0     1795 2023-10-07 13:18:15.338869 pydantic_marshals-0.3.8/pydantic_marshals/base/fields/properties.py
--rw-r--r--   0        0        0        0 2023-09-19 21:57:54.654061 pydantic_marshals-0.3.8/pydantic_marshals/base/fields/py.typed
--rw-r--r--   0        0        0     5000 2023-09-19 21:57:54.654061 pydantic_marshals-0.3.8/pydantic_marshals/base/models.py
--rw-r--r--   0        0        0        0 2023-09-19 21:57:54.654061 pydantic_marshals-0.3.8/pydantic_marshals/base/py.typed
--rw-r--r--   0        0        0      554 2023-09-19 21:57:54.654061 pydantic_marshals-0.3.8/pydantic_marshals/base/type_aliases.py
--rw-r--r--   0        0        0      380 2023-10-07 11:52:12.770436 pydantic_marshals-0.3.8/pydantic_marshals/contains/__init__.py
--rw-r--r--   0        0        0        0 2023-09-19 21:57:54.655036 pydantic_marshals-0.3.8/pydantic_marshals/contains/fields/__init__.py
--rw-r--r--   0        0        0     1701 2023-11-04 18:19:48.979460 pydantic_marshals-0.3.8/pydantic_marshals/contains/fields/constants.py
--rw-r--r--   0        0        0      938 2023-09-19 22:16:36.105055 pydantic_marshals-0.3.8/pydantic_marshals/contains/fields/lists.py
--rw-r--r--   0        0        0     1218 2023-09-19 22:15:54.461171 pydantic_marshals-0.3.8/pydantic_marshals/contains/fields/nested.py
--rw-r--r--   0        0        0        0 2023-09-19 21:57:54.655036 pydantic_marshals-0.3.8/pydantic_marshals/contains/fields/py.typed
--rw-r--r--   0        0        0     1143 2023-09-19 22:15:54.462298 pydantic_marshals-0.3.8/pydantic_marshals/contains/fields/typed.py
--rw-r--r--   0        0        0     1252 2023-09-19 22:15:54.464298 pydantic_marshals-0.3.8/pydantic_marshals/contains/fields/wildcards.py
--rw-r--r--   0        0        0     2010 2023-11-04 17:45:37.954454 pydantic_marshals-0.3.8/pydantic_marshals/contains/models.py
--rw-r--r--   0        0        0      438 2023-11-04 17:31:03.679505 pydantic_marshals-0.3.8/pydantic_marshals/contains/type_aliases.py
--rw-r--r--   0        0        0        0 2023-09-19 21:57:54.656003 pydantic_marshals-0.3.8/pydantic_marshals/contains/type_generators/__init__.py
--rw-r--r--   0        0        0     1142 2023-09-20 15:10:50.373749 pydantic_marshals-0.3.8/pydantic_marshals/contains/type_generators/base.py
--rw-r--r--   0        0        0     1767 2023-09-20 15:51:24.514670 pydantic_marshals-0.3.8/pydantic_marshals/contains/type_generators/collections.py
--rw-r--r--   0        0        0        0 2023-07-24 18:26:24.250219 pydantic_marshals-0.3.8/pydantic_marshals/mypy/__init__.py
--rw-r--r--   0        0        0      823 2023-10-07 13:36:48.716562 pydantic_marshals-0.3.8/pydantic_marshals/mypy/magic.pyi
--rw-r--r--   0        0        0     1910 2023-10-07 15:19:57.262543 pydantic_marshals-0.3.8/pydantic_marshals/mypy/plugin.py
--rw-r--r--   0        0        0        0 2023-07-24 18:26:24.250219 pydantic_marshals-0.3.8/pydantic_marshals/mypy/py.typed
--rw-r--r--   0        0        0        0 2023-07-24 18:26:24.250219 pydantic_marshals-0.3.8/pydantic_marshals/py.typed
--rw-r--r--   0        0        0       91 2023-10-07 11:49:41.435289 pydantic_marshals-0.3.8/pydantic_marshals/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2023-09-19 21:57:54.658000 pydantic_marshals-0.3.8/pydantic_marshals/sqlalchemy/fields/__init__.py
--rw-r--r--   0        0        0     2931 2023-11-12 12:17:43.396366 pydantic_marshals-0.3.8/pydantic_marshals/sqlalchemy/fields/columns.py
--rw-r--r--   0        0        0        0 2023-09-19 21:57:54.658000 pydantic_marshals-0.3.8/pydantic_marshals/sqlalchemy/fields/py.typed
--rw-r--r--   0        0        0     2483 2023-10-07 13:18:15.335869 pydantic_marshals-0.3.8/pydantic_marshals/sqlalchemy/fields/relationships.py
--rw-r--r--   0        0        0     2761 2023-10-07 13:38:45.576762 pydantic_marshals-0.3.8/pydantic_marshals/sqlalchemy/models.py
--rw-r--r--   0        0        0        0 2023-09-19 21:57:54.659002 pydantic_marshals-0.3.8/pydantic_marshals/sqlalchemy/py.typed
--rw-r--r--   0        0        0      262 2023-07-24 18:26:24.251218 pydantic_marshals-0.3.8/pydantic_marshals/utils.py
--rw-r--r--   0        0        0     1533 2023-11-12 12:16:00.322884 pydantic_marshals-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     3216 2023-10-07 13:31:07.622563 pydantic_marshals-0.3.8/README.md
--rw-r--r--   0        0        0     3711 1970-01-01 00:00:00.000000 pydantic_marshals-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-24 18:26:24.247220 pydantic_marshals-0.3.9/pydantic_marshals/__init__.py
+-rw-r--r--   0        0        0      201 2023-11-12 20:16:18.776870 pydantic_marshals-0.3.9/pydantic_marshals/base/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-19 21:57:54.653062 pydantic_marshals-0.3.9/pydantic_marshals/base/fields/__init__.py
+-rw-r--r--   0        0        0     3631 2023-11-12 19:59:51.083920 pydantic_marshals-0.3.9/pydantic_marshals/base/fields/base.py
+-rw-r--r--   0        0        0     1795 2023-10-07 13:18:15.338869 pydantic_marshals-0.3.9/pydantic_marshals/base/fields/properties.py
+-rw-r--r--   0        0        0        0 2023-09-19 21:57:54.654061 pydantic_marshals-0.3.9/pydantic_marshals/base/fields/py.typed
+-rw-r--r--   0        0        0     5000 2023-09-19 21:57:54.654061 pydantic_marshals-0.3.9/pydantic_marshals/base/models.py
+-rw-r--r--   0        0        0        0 2023-09-19 21:57:54.654061 pydantic_marshals-0.3.9/pydantic_marshals/base/py.typed
+-rw-r--r--   0        0        0      554 2023-09-19 21:57:54.654061 pydantic_marshals-0.3.9/pydantic_marshals/base/type_aliases.py
+-rw-r--r--   0        0        0      380 2023-10-07 11:52:12.770436 pydantic_marshals-0.3.9/pydantic_marshals/contains/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-19 21:57:54.655036 pydantic_marshals-0.3.9/pydantic_marshals/contains/fields/__init__.py
+-rw-r--r--   0        0        0     1701 2023-11-04 18:19:48.979460 pydantic_marshals-0.3.9/pydantic_marshals/contains/fields/constants.py
+-rw-r--r--   0        0        0      938 2023-09-19 22:16:36.105055 pydantic_marshals-0.3.9/pydantic_marshals/contains/fields/lists.py
+-rw-r--r--   0        0        0     1218 2023-09-19 22:15:54.461171 pydantic_marshals-0.3.9/pydantic_marshals/contains/fields/nested.py
+-rw-r--r--   0        0        0        0 2023-09-19 21:57:54.655036 pydantic_marshals-0.3.9/pydantic_marshals/contains/fields/py.typed
+-rw-r--r--   0        0        0     1143 2023-09-19 22:15:54.462298 pydantic_marshals-0.3.9/pydantic_marshals/contains/fields/typed.py
+-rw-r--r--   0        0        0     1252 2023-09-19 22:15:54.464298 pydantic_marshals-0.3.9/pydantic_marshals/contains/fields/wildcards.py
+-rw-r--r--   0        0        0     2010 2023-11-04 17:45:37.954454 pydantic_marshals-0.3.9/pydantic_marshals/contains/models.py
+-rw-r--r--   0        0        0      438 2023-11-04 17:31:03.679505 pydantic_marshals-0.3.9/pydantic_marshals/contains/type_aliases.py
+-rw-r--r--   0        0        0        0 2023-09-19 21:57:54.656003 pydantic_marshals-0.3.9/pydantic_marshals/contains/type_generators/__init__.py
+-rw-r--r--   0        0        0     1142 2023-09-20 15:10:50.373749 pydantic_marshals-0.3.9/pydantic_marshals/contains/type_generators/base.py
+-rw-r--r--   0        0        0     1767 2023-09-20 15:51:24.514670 pydantic_marshals-0.3.9/pydantic_marshals/contains/type_generators/collections.py
+-rw-r--r--   0        0        0        0 2023-07-24 18:26:24.250219 pydantic_marshals-0.3.9/pydantic_marshals/mypy/__init__.py
+-rw-r--r--   0        0        0      823 2023-10-07 13:36:48.716562 pydantic_marshals-0.3.9/pydantic_marshals/mypy/magic.pyi
+-rw-r--r--   0        0        0     1910 2023-10-07 15:19:57.262543 pydantic_marshals-0.3.9/pydantic_marshals/mypy/plugin.py
+-rw-r--r--   0        0        0        0 2023-07-24 18:26:24.250219 pydantic_marshals-0.3.9/pydantic_marshals/mypy/py.typed
+-rw-r--r--   0        0        0        0 2023-07-24 18:26:24.250219 pydantic_marshals-0.3.9/pydantic_marshals/py.typed
+-rw-r--r--   0        0        0       91 2023-10-07 11:49:41.435289 pydantic_marshals-0.3.9/pydantic_marshals/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-19 21:57:54.658000 pydantic_marshals-0.3.9/pydantic_marshals/sqlalchemy/fields/__init__.py
+-rw-r--r--   0        0        0     2931 2023-11-12 12:17:43.396366 pydantic_marshals-0.3.9/pydantic_marshals/sqlalchemy/fields/columns.py
+-rw-r--r--   0        0        0        0 2023-09-19 21:57:54.658000 pydantic_marshals-0.3.9/pydantic_marshals/sqlalchemy/fields/py.typed
+-rw-r--r--   0        0        0     2483 2023-10-07 13:18:15.335869 pydantic_marshals-0.3.9/pydantic_marshals/sqlalchemy/fields/relationships.py
+-rw-r--r--   0        0        0     2761 2023-10-07 13:38:45.576762 pydantic_marshals-0.3.9/pydantic_marshals/sqlalchemy/models.py
+-rw-r--r--   0        0        0        0 2023-09-19 21:57:54.659002 pydantic_marshals-0.3.9/pydantic_marshals/sqlalchemy/py.typed
+-rw-r--r--   0        0        0      262 2023-07-24 18:26:24.251218 pydantic_marshals-0.3.9/pydantic_marshals/utils.py
+-rw-r--r--   0        0        0     1533 2023-11-12 20:24:54.658936 pydantic_marshals-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     3216 2023-10-07 13:31:07.622563 pydantic_marshals-0.3.9/README.md
+-rw-r--r--   0        0        0     3711 1970-01-01 00:00:00.000000 pydantic_marshals-0.3.9/PKG-INFO
```

### Comparing `pydantic_marshals-0.3.8/pydantic_marshals/base/fields/base.py` & `pydantic_marshals-0.3.9/pydantic_marshals/base/fields/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from collections.abc import Iterator
+from enum import Enum
 from typing import Any
 
 from pydantic import BaseModel, RootModel
 from pydantic.fields import Field
 from pydantic_core import PydanticUndefined, PydanticUndefinedType
 from typing_extensions import Self
 
@@ -69,15 +70,19 @@
             Field(**dict(self.generate_field_data())),
         )
 
     def generate_root_model(self) -> type[BaseModel]:
         return RootModel[self.generate_type()]  # type: ignore[no-any-return, misc]
 
 
-PatchDefault = object()
+class PatchDefaultType(Enum):
+    PatchDefault = -1
+
+
+PatchDefault = PatchDefaultType.PatchDefault
 
 
 class PatchMarshalField(MarshalField):
     def __init__(self, alias: str | None = None, patch: bool = False) -> None:
         """
         :param alias: same as Field(alias=...), can be None for no alias
         :param patch: use PatchDefault as a default for the filed
```

### Comparing `pydantic_marshals-0.3.8/pydantic_marshals/base/fields/properties.py` & `pydantic_marshals-0.3.9/pydantic_marshals/base/fields/properties.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.3.8/pydantic_marshals/base/models.py` & `pydantic_marshals-0.3.9/pydantic_marshals/base/models.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.3.8/pydantic_marshals/base/type_aliases.py` & `pydantic_marshals-0.3.9/pydantic_marshals/base/type_aliases.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.3.8/pydantic_marshals/contains/fields/constants.py` & `pydantic_marshals-0.3.9/pydantic_marshals/contains/fields/constants.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.3.8/pydantic_marshals/contains/fields/lists.py` & `pydantic_marshals-0.3.9/pydantic_marshals/contains/fields/lists.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.3.8/pydantic_marshals/contains/fields/nested.py` & `pydantic_marshals-0.3.9/pydantic_marshals/contains/fields/nested.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.3.8/pydantic_marshals/contains/fields/typed.py` & `pydantic_marshals-0.3.9/pydantic_marshals/contains/fields/typed.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.3.8/pydantic_marshals/contains/fields/wildcards.py` & `pydantic_marshals-0.3.9/pydantic_marshals/contains/fields/wildcards.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.3.8/pydantic_marshals/contains/models.py` & `pydantic_marshals-0.3.9/pydantic_marshals/contains/models.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.3.8/pydantic_marshals/contains/type_generators/base.py` & `pydantic_marshals-0.3.9/pydantic_marshals/contains/type_generators/base.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.3.8/pydantic_marshals/contains/type_generators/collections.py` & `pydantic_marshals-0.3.9/pydantic_marshals/contains/type_generators/collections.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.3.8/pydantic_marshals/mypy/magic.pyi` & `pydantic_marshals-0.3.9/pydantic_marshals/mypy/magic.pyi`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.3.8/pydantic_marshals/mypy/plugin.py` & `pydantic_marshals-0.3.9/pydantic_marshals/mypy/plugin.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.3.8/pydantic_marshals/sqlalchemy/fields/columns.py` & `pydantic_marshals-0.3.9/pydantic_marshals/sqlalchemy/fields/columns.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.3.8/pydantic_marshals/sqlalchemy/fields/relationships.py` & `pydantic_marshals-0.3.9/pydantic_marshals/sqlalchemy/fields/relationships.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.3.8/pydantic_marshals/sqlalchemy/models.py` & `pydantic_marshals-0.3.9/pydantic_marshals/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.3.8/pyproject.toml` & `pydantic_marshals-0.3.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-marshals"
-version = "0.3.8"
+version = "0.3.9"
 description = "Library for creating partial pydantic models (automatic converters) from different mappings"
 authors = ["niqzart <niqzart@gmail.com>"]
 readme = "README.md"
 exclude = [
     "examples",
     "tests",
     "docs",
```

### Comparing `pydantic_marshals-0.3.8/README.md` & `pydantic_marshals-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_marshals-0.3.8/PKG-INFO` & `pydantic_marshals-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-marshals
-Version: 0.3.8
+Version: 0.3.9
 Summary: Library for creating partial pydantic models (automatic converters) from different mappings
 Author: niqzart
 Author-email: niqzart@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

