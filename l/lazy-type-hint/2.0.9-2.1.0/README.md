# Comparing `tmp/lazy_type_hint-2.0.9.tar.gz` & `tmp/lazy_type_hint-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_type_hint-2.0.9.tar", max compression
+gzip compressed data, was "lazy_type_hint-2.1.0.tar", max compression
```

## Comparing `lazy_type_hint-2.0.9.tar` & `lazy_type_hint-2.1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-2.0.9/lazy_type_hint/__init__.py
--rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/__init__.py
--rw-r--r--   0        0        0    10586 2024-04-18 12:50:55.117818 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/data_type_tree.py
--rw-r--r--   0        0        0     7262 2024-04-18 12:50:55.128183 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/factory.py
--rw-r--r--   0        0        0     1118 2024-04-18 12:50:55.134208 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/__init__.py
--rw-r--r--   0        0        0    17314 2024-04-18 12:50:55.137251 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
--rw-r--r--   0        0        0     4020 2024-04-17 13:44:57.982002 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
--rw-r--r--   0        0        0      775 2024-04-18 12:50:55.144203 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/iterator_data_type_tree.py
--rw-r--r--   0        0        0     1094 2024-04-18 12:50:55.145202 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
--rw-r--r--   0        0        0     4816 2024-04-18 12:50:55.146209 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
--rw-r--r--   0        0        0      601 2024-04-18 12:50:55.151203 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
--rw-r--r--   0        0        0     5809 2024-04-18 12:50:55.160218 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py
--rw-r--r--   0        0        0      719 2024-04-17 14:44:54.567291 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
--rw-r--r--   0        0        0     6506 2024-04-18 12:50:55.165811 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
--rw-r--r--   0        0        0     1486 2024-04-17 10:55:20.513506 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
--rw-r--r--   0        0        0     2101 2024-04-18 12:50:55.165811 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
--rw-r--r--   0        0        0     1061 2024-04-15 15:41:02.091078 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
--rw-r--r--   0        0        0     3013 2024-04-18 12:50:55.166804 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
--rw-r--r--   0        0        0     1060 2024-04-15 15:41:02.097066 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
--rw-r--r--   0        0        0      368 2024-04-18 12:50:55.171934 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/io_data_type_tree.py
--rw-r--r--   0        0        0      404 2024-04-18 12:50:55.176929 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/module_data_type_tree.py
--rw-r--r--   0        0        0      439 2024-04-18 12:50:55.178906 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/pandas_series_data_type_tree.py
--rw-r--r--   0        0        0     1003 2024-04-14 10:39:38.880313 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
--rw-r--r--   0        0        0      755 2024-04-18 12:50:55.184933 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
--rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-2.0.9/lazy_type_hint/file_modifiers/__init__.py
--rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-2.0.9/lazy_type_hint/file_modifiers/py_file_modifier.py
--rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-2.0.9/lazy_type_hint/file_modifiers/yaml_file_modifier.py
--rw-r--r--   0        0        0     2340 2024-04-15 06:56:34.375018 lazy_type_hint-2.0.9/lazy_type_hint/generators/lazy_type_hint.py
--rw-r--r--   0        0        0     3137 2024-04-16 12:08:47.077767 lazy_type_hint-2.0.9/lazy_type_hint/generators/lazy_type_hint_abc.py
--rw-r--r--   0        0        0     9756 2024-04-16 12:16:29.926108 lazy_type_hint-2.0.9/lazy_type_hint/generators/lazy_type_hint_live.py
--rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-2.0.9/lazy_type_hint/py.typed
--rw-r--r--   0        0        0     2222 2024-04-18 12:50:55.191932 lazy_type_hint-2.0.9/lazy_type_hint/strategies.py
--rw-r--r--   0        0        0      732 2024-04-18 12:50:55.192858 lazy_type_hint-2.0.9/lazy_type_hint/utils/__init__.py
--rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-2.0.9/lazy_type_hint/utils/docstring_formatter.py
--rw-r--r--   0        0        0     5655 2024-04-15 15:41:02.110072 lazy_type_hint-2.0.9/lazy_type_hint/utils/import_manager.py
--rw-r--r--   0        0        0     5008 2024-04-14 13:10:20.018341 lazy_type_hint-2.0.9/lazy_type_hint/utils/mypy.py
--rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.9/lazy_type_hint/utils/ordered_set.py
--rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.9/lazy_type_hint/utils/test_ordered_set.py
--rw-r--r--   0        0        0     3783 2024-04-18 12:50:55.193858 lazy_type_hint-2.0.9/lazy_type_hint/utils/utils.py
--rw-r--r--   0        0        0     2600 2024-04-18 12:50:55.195064 lazy_type_hint-2.0.9/pyproject.toml
--rw-r--r--   0        0        0     7007 2024-04-16 12:16:29.914611 lazy_type_hint-2.0.9/README.md
--rw-r--r--   0        0        0     7392 1970-01-01 00:00:00.000000 lazy_type_hint-2.0.9/PKG-INFO
+-rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-2.1.0/lazy_type_hint/__init__.py
+-rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/__init__.py
+-rw-r--r--   0        0        0    12297 2024-04-20 12:20:31.948128 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/data_type_tree.py
+-rw-r--r--   0        0        0     7268 2024-04-19 13:25:22.421859 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/factory.py
+-rw-r--r--   0        0        0     1118 2024-04-19 13:25:22.427858 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/__init__.py
+-rw-r--r--   0        0        0    17314 2024-04-19 13:25:22.433858 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
+-rw-r--r--   0        0        0     2963 2024-04-20 12:20:31.948128 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
+-rw-r--r--   0        0        0      775 2024-04-19 13:25:22.439859 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/iterator_data_type_tree.py
+-rw-r--r--   0        0        0     1094 2024-04-19 13:25:22.445857 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
+-rw-r--r--   0        0        0     5872 2024-04-20 12:20:31.949822 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
+-rw-r--r--   0        0        0      601 2024-04-19 13:25:22.452857 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
+-rw-r--r--   0        0        0     7038 2024-04-20 12:20:31.950322 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py
+-rw-r--r--   0        0        0     1309 2024-04-20 12:20:31.951328 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
+-rw-r--r--   0        0        0     6506 2024-04-19 13:25:22.458858 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
+-rw-r--r--   0        0        0     1949 2024-04-20 12:20:31.951328 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
+-rw-r--r--   0        0        0     2101 2024-04-19 13:25:22.464857 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
+-rw-r--r--   0        0        0     1061 2024-04-15 15:41:02.091078 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
+-rw-r--r--   0        0        0     3013 2024-04-19 13:25:22.470858 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
+-rw-r--r--   0        0        0     1060 2024-04-15 15:41:02.097066 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
+-rw-r--r--   0        0        0      368 2024-04-19 13:25:22.475858 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/io_data_type_tree.py
+-rw-r--r--   0        0        0      404 2024-04-19 13:25:22.480858 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/module_data_type_tree.py
+-rw-r--r--   0        0        0      439 2024-04-19 13:25:22.487019 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/pandas_series_data_type_tree.py
+-rw-r--r--   0        0        0     1003 2024-04-14 10:39:38.880313 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
+-rw-r--r--   0        0        0      755 2024-04-19 13:25:22.492857 lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
+-rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-2.1.0/lazy_type_hint/file_modifiers/__init__.py
+-rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-2.1.0/lazy_type_hint/file_modifiers/py_file_modifier.py
+-rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-2.1.0/lazy_type_hint/file_modifiers/yaml_file_modifier.py
+-rw-r--r--   0        0        0     2340 2024-04-15 06:56:34.375018 lazy_type_hint-2.1.0/lazy_type_hint/generators/lazy_type_hint.py
+-rw-r--r--   0        0        0     3137 2024-04-18 17:00:26.789320 lazy_type_hint-2.1.0/lazy_type_hint/generators/lazy_type_hint_abc.py
+-rw-r--r--   0        0        0    10092 2024-04-20 12:20:31.952328 lazy_type_hint-2.1.0/lazy_type_hint/generators/lazy_type_hint_live.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-2.1.0/lazy_type_hint/py.typed
+-rw-r--r--   0        0        0     2222 2024-04-19 13:25:22.505265 lazy_type_hint-2.1.0/lazy_type_hint/strategies.py
+-rw-r--r--   0        0        0      732 2024-04-19 13:25:22.511264 lazy_type_hint-2.1.0/lazy_type_hint/utils/__init__.py
+-rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-2.1.0/lazy_type_hint/utils/docstring_formatter.py
+-rw-r--r--   0        0        0     5655 2024-04-15 15:41:02.110072 lazy_type_hint-2.1.0/lazy_type_hint/utils/import_manager.py
+-rw-r--r--   0        0        0     5008 2024-04-14 13:10:20.018341 lazy_type_hint-2.1.0/lazy_type_hint/utils/mypy.py
+-rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-2.1.0/lazy_type_hint/utils/ordered_set.py
+-rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-2.1.0/lazy_type_hint/utils/test_ordered_set.py
+-rw-r--r--   0        0        0     3712 2024-04-20 12:20:31.953328 lazy_type_hint-2.1.0/lazy_type_hint/utils/utils.py
+-rw-r--r--   0        0        0     2602 2024-04-20 12:14:56.856217 lazy_type_hint-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7335 2024-04-20 12:20:31.946128 lazy_type_hint-2.1.0/README.md
+-rw-r--r--   0        0        0     7711 1970-01-01 00:00:00.000000 lazy_type_hint-2.1.0/PKG-INFO
```

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/data_type_tree.py` & `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/data_type_tree.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """`DataTypeTree` object that creates a tree representing all container types within the data type given.
 
 This data can then be parsed to a .py compatible file that will type hint your code.
 """
 
 from __future__ import annotations
 
+import re
 from abc import ABC, abstractmethod
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
     FrozenSet,
     Hashable,
@@ -25,14 +26,15 @@
 from lazy_type_hint.strategies import ParsingStrategies
 from lazy_type_hint.utils import (
     ImportManager,
     OrderedSet,
     cache_returned_value_per_instance,
     is_string_python_keyword_compatible,
 )
+from lazy_type_hint.utils.utils import TAB
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
 
 class DataTypeTreeError(Exception):
     ...
@@ -188,29 +190,63 @@
         return self.get_str_top_node().split("=")[-1].strip()
 
     @final
     def get_str_top_node(self) -> str:
         return self._get_str_top_node()
 
     @final
-    def get_str_all_nodes(self, include_imports: bool = True) -> str:
+    def get_str_all_nodes(
+        self, include_imports: bool = True, make_parent_class_inherit_from_original_type: bool = False
+    ) -> str:
         """String that represents the .py file created from the tree."""
-        return self._format_node_strings(self.get_strs_all_nodes_unformatted(include_imports=include_imports))
+        return self._format_node_strings(
+            self.get_strs_all_nodes_unformatted(
+                include_imports=include_imports,
+                make_parent_class_inherit_from_original_type=make_parent_class_inherit_from_original_type,
+            )
+        )
 
     @final
     @cache_returned_value_per_instance
-    def get_strs_all_nodes_unformatted(self, *, include_imports: bool = True) -> Tuple[str, ...]:
+    def get_strs_all_nodes_unformatted(
+        self, *, include_imports: bool = True, make_parent_class_inherit_from_original_type: bool = False
+    ) -> Tuple[str, ...]:
         """Get, ordered by dependencies, all strings representing the whole tree."""
         strings: OrderedSet[str] = OrderedSet()
         self._get_strs_all_nodes_unformatted(types=strings)
         strings_lst = strings.as_list()
+        if not strings_lst:
+            raise DataTypeTreeError("No type hints could be built")
+
         if include_imports:
             strings_lst.insert(0, self.imports.format())
+
+        if make_parent_class_inherit_from_original_type:
+            strings_lst[-1], old_name = self.rename_declaration(strings_lst[-1], new_name="_{name}")
+            strings_lst.append(f"class {old_name}(_{old_name}):\n{TAB}...")
         return tuple(strings_lst)
 
+    @staticmethod
+    def rename_declaration(declaration: str, new_name: str) -> Tuple[str, str]:
+        if "=" in declaration:
+            declarations = declaration.split("=")
+            old_name = declarations[0].rstrip().strip()
+            new_name = new_name.format(name=old_name)
+            declaration = f"{new_name} =" + "".join(declarations[1:])
+        elif declaration.startswith("class "):
+            pattern = r"class\s+(\w+)\b"
+            match = re.search(pattern, declaration)
+            old_name = match.group(1) if match else ""
+            new_name = new_name.format(name=old_name)
+            if old_name:
+                declaration = re.sub(pattern, f"class {new_name}", declaration)
+        else:
+            old_name = ""
+        return declaration, old_name
+
     @final
     def _get_strs_all_nodes_unformatted(self, *, types: Optional[OrderedSet[str]] = None) -> None:
         if types is None:
             types = OrderedSet()
 
         if self.depth == 0 and not self.children:
             if self.permission_to_be_created_as_type_alias:
@@ -268,16 +304,20 @@
         return len(self.children)
 
     @abstractmethod
     def __next__(self) -> DataTypeTree:
         """Iterate over the children of the tree."""
 
     @final
-    def print_children(self) -> None:
-        print(repr(self))
+    def print_all_children(self, *, recursive: bool = True) -> None:
+        print("    " * self.depth + repr(self))
+        if not self.children:
+            return
+        for child in self:
+            child.print_all_children(recursive=recursive)
 
     @final
     def __eq__(self, other_object: object) -> bool:
         if type(self) is type(other_object):
             return hash(self) == hash(other_object)
         return False
```

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/factory.py` & `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-from typing import TYPE_CHECKING, Iterator, overload
+from typing import TYPE_CHECKING, Any, Iterator, Union, overload
 
 from lazy_type_hint.data_type_tree.data_type_tree import DataTypeTree
 from lazy_type_hint.strategies import ParsingStrategies
 
 if TYPE_CHECKING:
     from types import MappingProxyType, ModuleType
     from typing import (
-        Any,
         Dict,
         FrozenSet,
         Iterator,
         List,
         Mapping,
         Optional,
         Sequence,
         Set,
         TextIO,
         Tuple,
-        Union,
     )
 
     import pandas as pd
 
     from lazy_type_hint.data_type_tree.generic_type.dict_data_type_tree import DictDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.iterator_data_type_tree import IteratorDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.list_data_type_tree import ListDataTypeTree
@@ -207,27 +205,27 @@
     parent: "Optional[DataTypeTree]" = None,
 ) -> "MappingDataTypeTree":
     ...
 
 
 @overload
 def data_type_tree_factory(  # type: ignore[misc]
-    data: object,
+    data: Union[object, Any],
     name: str,
     *,
     imports: "Optional[ImportManager]" = None,
     depth: int = 0,
     strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
     parent: "Optional[DataTypeTree]" = None,
 ) -> DataTypeTree:
     ...
 
 
 def data_type_tree_factory(
-    data: object,
+    data: Union[object, Any],
     name: str,
     *,
     imports: "Optional[ImportManager]" = None,
     depth: int = 0,
     strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
     parent: "Optional[DataTypeTree]" = None,
 ) -> DataTypeTree:
```

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/__init__.py` & `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py` & `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py` & `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 from abc import abstractmethod
 from typing import (
     Hashable,
     Iterable,
-    Iterator,
     List,
-    Mapping,
     Sequence,
     Tuple,
-    Union,
     final,
 )
 
-from typing_extensions import Self, override
+from typing_extensions import override
 
 from lazy_type_hint.data_type_tree.data_type_tree import ChildrenStructure, DataTypeTree
 
 
 class GenericDataTypeTree(DataTypeTree):
     """Tree that holds any kind of object that must contain other inner structures (children)."""
 
     children: ChildrenStructure[DataTypeTree]
 
-    # Iterable-protocol related
-    _iterator: Union[int, Iterator[Hashable]]
-
     @abstractmethod
     def _instantiate_children(self, data: object) -> ChildrenStructure[DataTypeTree]:
         ...
 
     def get_type_alias_children(self) -> str:
         """Get, in a format manner, a single string with all subtypes found within the generic structure.
 
@@ -79,37 +73,13 @@
         if remove_repeated:
             child_types_set = sorted(set(child_types))
             if "float" in child_types and "int" in child_types:
                 child_types_set.remove("int")
             return tuple(sorted(child_types_set))
         return tuple(child_types)
 
-    def __iter__(self) -> "Self":
-        if isinstance(self.children, Mapping):
-            self._iterator = iter(self.children.keys())
-        else:
-            self._iterator = 0  # Reset the index to zero when starting a new iteration
-        return self
-
-    @override
-    def __next__(self) -> DataTypeTree:
-        # Many type ignores here but everything is safe
-        if isinstance(self.children, Mapping):
-            key = next(self._iterator, None)  # type: ignore
-            if key is not None:
-                return self.children[key]
-            else:
-                raise StopIteration
-        else:
-            if self._iterator < len(self.children):  # type: ignore
-                element = list(self.children)[self._iterator]  # type: ignore
-                self._iterator += 1  # type: ignore
-                return element
-            else:
-                raise StopIteration
-
     @override
     def _get_hash(self) -> Hashable:
         hashes: List[object] = []
         for child in self:
             hashes.append(child._get_hash())
         return tuple(hashes)
```

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/iterator_data_type_tree.py` & `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/iterator_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py` & `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py` & `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,71 @@
 import re
-from typing import Dict, Final, Hashable, Iterator, List, Literal, Mapping, Set
+from collections import defaultdict
+from typing import Dict, Final, Hashable, Iterator, List, Literal, Mapping, Set, Type
 
-from typing_extensions import override
+from typing_extensions import Self, override
 
 from lazy_type_hint.data_type_tree.data_type_tree import DataTypeTree
 from lazy_type_hint.data_type_tree.factory import data_type_tree_factory
 from lazy_type_hint.data_type_tree.generic_type.generic_data_type_tree import GenericDataTypeTree
 from lazy_type_hint.file_modifiers.yaml_file_modifier import YamlFileModifier
 
 
 class MappingDataTypeTree(GenericDataTypeTree):
     children: Mapping[Hashable, DataTypeTree]
     hidden_keys_prefix: Final = YamlFileModifier.prefix
 
     # Iterable-protocol related
     _keys: Iterator[Hashable]
+    _iterator: Iterator[Hashable]
 
     @override
     def _instantiate_children(self, data: Mapping[Hashable, object]) -> Mapping[Hashable, DataTypeTree]:  # type: ignore
         children: Dict[Hashable, DataTypeTree] = {}
+        children_info: Dict[DataTypeTree, Set[Hashable]] = defaultdict(set)
 
         for key, value in data.items():
             suffix = type(key).__name__ if not isinstance(key, str) else self._to_camel_case(key)
             if isinstance(key, str) and key.startswith(self.hidden_keys_prefix):
                 continue
             child = data_type_tree_factory(
                 data=value,
                 name=f"{self.name}{suffix}",
                 imports=self.imports,
                 depth=self.depth + 1,
                 strategies=self.strategies,
                 parent=self,
             )
-            if child in children.values():
-                self._replace_old_children_by_new_one(child, children)
-                children[key] = child
-            else:
-                children[key] = child
+            children_info[child].add(key)
+            children[key] = child
+        self._assign_same_data_type_tree_to_keys_with_same_value_type(children, children_info=children_info)
         return children
 
-    def _replace_old_children_by_new_one(self, child: DataTypeTree, children: Dict[Hashable, DataTypeTree]) -> None:
+    def _assign_same_data_type_tree_to_keys_with_same_value_type(
+        self, children: Dict[Hashable, DataTypeTree], *, children_info: Dict[DataTypeTree, Set[Hashable]]
+    ) -> None:
         """
-        Replaces old child nodes with a new one in the given dictionary of children.
+        Simplify the tree.
 
-        Only replaced those children that are equal to the given child. In addition, naming is updated to
-        make them match.
+        Find all values sharing the same data type tree, create a unique one and use this new one to replace all same
+        values.
         """
-        name = f"{self.name}{type(child.data).__name__.capitalize()}"
-        modified_name = name
-        count = 2
-        while modified_name in children.values():
-            modified_name = f"{name}{count}"
-            count += 1
-        child.name = modified_name
-        for inserted_key in children:
-            if children[inserted_key] == child:
-                children[inserted_key] = child
+        last_name_added: Dict[Type[object], int] = {}
+        for data_type_tree, values in children_info.items():
+            if len(values) > 1:  # Perform replacement if some values were detected to be the same in terms of types
+                parent_name = data_type_tree.parent.name if data_type_tree.parent is not None else ""
+                new_name = f"{parent_name}{data_type_tree.holding_type.__name__.capitalize()}"
+                if data_type_tree.holding_type in last_name_added:
+                    new_name += str(last_name_added[data_type_tree.holding_type] + 1)
+                    last_name_added[data_type_tree.holding_type] += 1
+                else:
+                    last_name_added[data_type_tree.holding_type] = 1
+                data_type_tree.rename(new_name)
+                for hashable in values:
+                    children[hashable] = data_type_tree
 
     def _get_str_top_node(self) -> str:
         return self._parse_dict(self.children)
 
     def _parse_dict(self, children: Mapping[Hashable, DataTypeTree]) -> str:
         """Get a string representation of the dictionary for this same top node.
 
@@ -86,14 +92,16 @@
     @staticmethod
     def _to_camel_case(string: str) -> str:
         """Make it camel case and compatible with Python keywords."""
         # Remove any initial number within the string
         match = re.match(r"^\d+", string)
         if match:
             number = match.group()
+            if not string[len(number) :]:
+                return string
             string = string[len(number) :]
 
         new_string = [""] * len(string)
         idx_to_remove: Set[int] = set()
         removed = False
         for idx, char in enumerate(string):
             if not char.isalpha() and not char.isnumeric():
@@ -115,7 +123,20 @@
 
     @override
     def _get_hash(self) -> Hashable:
         hashes: List[object] = []
         for name, child in self.children.items():
             hashes.append(("mapping", hash(type(name)), child._get_hash()))
         return frozenset(hashes)
+
+    @override
+    def __iter__(self) -> "Self":
+        self._iterator = iter(self.children.keys())
+        return self
+
+    @override
+    def __next__(self) -> DataTypeTree:
+        key = next(self._iterator, None)
+        if key is not None:
+            return self.children[key]
+        else:
+            raise StopIteration
```

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py` & `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py` & `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 from typing import (
     Dict,
     Final,
+    Hashable,
     List,
     Mapping,
     Set,
+    Tuple,
     Type,
+    Union,
+    cast,
 )
 
 import pandas as pd
 from typing_extensions import override
 
 from lazy_type_hint.data_type_tree import data_type_tree_factory
 from lazy_type_hint.data_type_tree.data_type_tree import DataTypeTree
 from lazy_type_hint.data_type_tree.generic_type.mapping_data_type_tree import MappingDataTypeTree
+from lazy_type_hint.utils.utils import cache_returned_value_per_instance
 
+LITERAL_OVERLOAD_TEMPLATE: Final = """    @overload  # type: ignore
+    def __getitem__(self, key: Literal[{literal}]) -> {rtype}:
+        ...
+"""
 OVERLOAD_TEMPLATE: Final = """    @overload  # type: ignore
-    def __getitem__(self, key: Literal["{literal}"]) -> {rtype}:
+    def __getitem__(self, key: {input_type}) -> {rtype}:
         ...
 """
 TEMPLATE: Final = """class {class_name}(pd.DataFrame):
 
 {overloads}
     @overload
     def __getitem__(
@@ -68,63 +77,82 @@
 class PandasDataFrameDataTypeTree(MappingDataTypeTree):
     wraps = (pd.DataFrame,)
     data: pd.DataFrame
     children: Mapping[str, DataTypeTree]  # type: ignore[assignment]
 
     @override
     @property
+    @cache_returned_value_per_instance
     def permission_to_be_created_as_type_alias(self) -> bool:
-        return bool(len(self) >= 1 and self.are_columns_either_all_str_or_all_tuple)
+        """
+        Set the permissions of this class to be created as a type alias.
+
+        Situations where permission is given:
+            - If columns are tuples: And first level are str, int or bool
+            - If columns are not tuples: And columns are str, int, bool
+
+        Otherwise delegate to super class
+        """
+        if all(isinstance(column, tuple) for column in self.data.columns):
+            if all(isinstance(column[0], (str, bool, int)) for column in self.data.columns):
+                return True
+        else:
+            if all(isinstance(column, (str, bool, int)) for column in self.data.columns):
+                return True
+        return super().permission_to_be_created_as_type_alias
 
     @property
+    @cache_returned_value_per_instance
     def can_be_accessed_multilevel(self) -> bool:
         return self.all_columns_are(tuple)
 
     @property
     def are_column_same_type(self) -> bool:
         return len({type(column) for column in self.data.columns}) == 1
 
     def all_columns_are(self, type_: Type[object]) -> bool:
         return all(isinstance(column, type_) for column in self.data.columns)
 
     @property
     def are_columns_either_all_str_or_all_tuple(self) -> bool:
         if self.are_column_same_type:
-            return all(isinstance(column, (str, tuple)) for column in self.data.columns)
+            return all(isinstance(column, (str, int, tuple)) for column in self.data.columns)
         return False
 
-    def _create_child(self, column: str) -> DataTypeTree:
-        suffix = self._to_camel_case(column)
+    def _create_child(self, column: Hashable) -> DataTypeTree:
+        suffix = self._to_camel_case(str(column))
         return data_type_tree_factory(  # type: ignore
             data=self.data[column],
             name=f"{self.name}{suffix}",
             imports=self.imports,
             depth=self.depth + 1,
             strategies=self.strategies,
             parent=self,
         )
 
     @override
-    def _instantiate_children(self, data: Mapping[str, object]) -> Mapping[str, DataTypeTree]:  # type: ignore
-        children: Dict[str, DataTypeTree] = {}
+    def _instantiate_children(self, data: pd.DataFrame) -> Mapping[Hashable, DataTypeTree]:
+        children: Dict[Hashable, DataTypeTree] = {}
         if not self.are_columns_either_all_str_or_all_tuple:
-            return children
+            return {}
 
         # Corner case to avoid infinite recursion
         if all(isinstance(column, tuple) and len(column) == 1 for column in self.data.columns):
             return {}
 
-        for column in self.data.columns:
-            if not self.can_be_accessed_multilevel:  # Here all columns will  be str
+        for column in data.columns:
+            if not self.can_be_accessed_multilevel:  # Here all columns will  be Hashable
+                column = cast(Hashable, column)
                 children[column] = self._create_child(column)
             else:  # Here all columns will be tuple
-                columns_processed: Set[str] = set()
-                for column in self.data.columns:
-                    if column[0] not in columns_processed:
-                        columns_processed.add(column[0])
+                multi_column = cast(Tuple[Hashable, ...], column)
+                columns_processed: Set[Union[bool, str, int]] = set()
+                if multi_column[0] not in columns_processed:
+                    if isinstance(multi_column[0], (str, int, bool)):
+                        columns_processed.add(multi_column[0])
                         children[column[0]] = self._create_child(column[0])
         return children
 
     @override
     def _get_hash(self) -> str:
         if self.strategies.pandas_strategies == "Do not type hint columns":
             return "pd.DataFrame"
@@ -145,19 +173,19 @@
         self.imports.add("Hashable")
         self.imports.add("numpy")
         self.imports.add("pd.Scalar")
 
         overloads: List[str] = []
         for literal, child in self.children.items():
             if child.permission_to_be_created_as_type_alias:
-                overloads.append(OVERLOAD_TEMPLATE.format(literal=literal, rtype=child.name))
+                overloads.append(LITERAL_OVERLOAD_TEMPLATE.format(literal=repr(literal), rtype=child.name))
             else:
-                rtype = "Union[pd.DataFrame, pd.Series]"
-                overloads.append(OVERLOAD_TEMPLATE.format(literal=literal, rtype=rtype))
+                rtype = "pd.Series" if isinstance(self.data[literal], pd.Series) else "pd.DataFrame"
+                overloads.append(LITERAL_OVERLOAD_TEMPLATE.format(literal=repr(literal), rtype=rtype))
         if self.strategies.pandas_strategies == "Full type hint":
-            all_literals = ", ".join(f'"{key}"' for key in self.children)
+            all_literals = ", ".join(repr(key) for key in self.children)
             allowed_types = f"Literal[{all_literals}]"
             template = TEMPLATE_NO_PD
         else:
             allowed_types = "str"
             template = TEMPLATE
         return template.format(class_name=self.name, overloads="\n".join(overloads), allowed_types=allowed_types)
```

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py` & `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py` & `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from typing import Any, Hashable, Literal, Sequence, Set, Tuple
 
-from typing_extensions import override
+from typing_extensions import Self, override
 
 from lazy_type_hint.data_type_tree.data_type_tree import DataTypeTree
 from lazy_type_hint.data_type_tree.generic_type.generic_data_type_tree import (
     GenericDataTypeTree,
 )
 from lazy_type_hint.data_type_tree.generic_type.set_and_sequence_operations import SetAndSequenceOperations
 
 
 class SetDataTypeTree(GenericDataTypeTree):
     wraps = (frozenset, set)
     children: Sequence[DataTypeTree]
     operations: SetAndSequenceOperations
 
+    _iterator: int
+
     @override
     def __pre_child_instantiation__(self) -> None:
         self.operations = SetAndSequenceOperations(self)
 
     @override
     def _instantiate_children(self, data: Sequence[Any]) -> Tuple[DataTypeTree, ...]:  # type: ignore
         return self.operations.instantiate_children(data, allow_repeated_children=False)
@@ -33,7 +35,21 @@
 
     @override
     def _get_hash(self) -> Hashable:
         hashes: Set[object] = set()
         for child in self:
             hashes.add(child._get_hash())
         return frozenset(hashes)
+
+    @override
+    def __iter__(self) -> "Self":
+        self._iterator = 0  # Reset the index to zero when starting a new iteration
+        return self
+
+    @override
+    def __next__(self) -> "DataTypeTree":
+        if self._iterator < len(self.children):
+            element = list(self.children)[self._iterator]
+            self._iterator += 1
+            return element
+        else:
+            raise StopIteration
```

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py` & `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py` & `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py` & `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py` & `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py` & `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py` & `lazy_type_hint-2.1.0/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/file_modifiers/py_file_modifier.py` & `lazy_type_hint-2.1.0/lazy_type_hint/file_modifiers/py_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/file_modifiers/yaml_file_modifier.py` & `lazy_type_hint-2.1.0/lazy_type_hint/file_modifiers/yaml_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/generators/lazy_type_hint.py` & `lazy_type_hint-2.1.0/lazy_type_hint/generators/lazy_type_hint.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/generators/lazy_type_hint_abc.py` & `lazy_type_hint-2.1.0/lazy_type_hint/generators/lazy_type_hint_abc.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/generators/lazy_type_hint_live.py` & `lazy_type_hint-2.1.0/lazy_type_hint/generators/lazy_type_hint_live.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,20 +9,22 @@
     Final,
     Literal,
     Mapping,
     Optional,
     Sequence,
     TypeVar,
     Union,
+    cast,
     final,
     overload,  # noqa: F401
 )
 
 from typing_extensions import TypeAlias, override
 
+from lazy_type_hint.data_type_tree import DataTypeTree
 from lazy_type_hint.file_modifiers.py_file_modifier import PyFileModifier
 from lazy_type_hint.file_modifiers.yaml_file_modifier import YAML_COMMENTS_POSITION
 from lazy_type_hint.generators.lazy_type_hint_abc import LazyTypeHintABC
 from lazy_type_hint.strategies import ParsingStrategies
 from lazy_type_hint.utils import (
     TAB,
     is_string_python_keyword_compatible,
@@ -60,15 +62,15 @@
     _custom_class_dir_path: Final = _this_file_pyi_path.parent / "build"
     """Path where the new classes will be generated.c"""
 
     @final
     def __init__(
         self,
         strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
-        if_type_hint_exists: Literal["overwrite", "validate"] = "validate",
+        if_type_hint_exists: Literal["overwrite", "validate"] = "overwrite",
     ) -> None:
         self.strategies = strategies
         self.if_type_hint_exists = if_type_hint_exists
 
         if not self._this_file_pyi_path.exists():
             self.this_file_pyi = self._generate_this_file_pyi()
         else:
@@ -117,24 +119,28 @@
         if not is_string_python_keyword_compatible(class_name):
             raise LazyTypeHintLiveError(
                 f"Given class_name is not compatible with Python class naming conventions: {class_name}"
             )
         custom_class_file_path = self._custom_class_dir_path / f"{class_name}.py"
 
         if class_name in self._get_classes_added() and self.if_type_hint_exists == "validate":
-            string_representation = str(super().from_data(data=data, class_name=class_name))
+            string_representation = cast(
+                DataTypeTree, super().from_data(data=data, class_name=class_name)
+            ).get_str_all_nodes(make_parent_class_inherit_from_original_type=False)
             if self._remove_docstrings(string_representation) != self._remove_docstrings(
                 custom_class_file_path.read_text(encoding="utf-8")
             ):
                 raise LazyTypeHintLiveError(
-                    "The given object did not generate the same string representation (type hints) for "
-                    f"the existing `{class_name}`"
+                    f"Error in validation: Existing type hints were found for `{class_name}` and this one does not "
+                    "match the inner structure of the input data given."
                 )
         else:
-            string_representation = str(super().from_data(data=data, class_name=class_name))
+            string_representation = cast(
+                DataTypeTree, super().from_data(data=data, class_name=class_name)
+            ).get_str_all_nodes(make_parent_class_inherit_from_original_type=False)
 
         self._create_custom_class_py(string_representation, class_name)
         if class_name in self._get_classes_added():
             return data
         self._add_new_class_to_loader_pyi(new_class=class_name)
         return data
```

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/strategies.py` & `lazy_type_hint-2.1.0/lazy_type_hint/strategies.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/utils/__init__.py` & `lazy_type_hint-2.1.0/lazy_type_hint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/utils/docstring_formatter.py` & `lazy_type_hint-2.1.0/lazy_type_hint/utils/docstring_formatter.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/utils/import_manager.py` & `lazy_type_hint-2.1.0/lazy_type_hint/utils/import_manager.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/utils/mypy.py` & `lazy_type_hint-2.1.0/lazy_type_hint/utils/mypy.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/utils/ordered_set.py` & `lazy_type_hint-2.1.0/lazy_type_hint/utils/ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/utils/test_ordered_set.py` & `lazy_type_hint-2.1.0/lazy_type_hint/utils/test_ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.9/lazy_type_hint/utils/utils.py` & `lazy_type_hint-2.1.0/lazy_type_hint/utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import ast
 import os
-import re
 import subprocess
 from itertools import zip_longest
 from typing import Any, Final, List, Protocol, TypeVar, Union, cast
 
 TAB: Final = "    "
 
 
@@ -14,18 +13,15 @@
 
     Args:
         string (str): The string to be checked.
 
     Returns:
         bool: True if the string is compatible with Python keywords, False otherwise.
     """
-    if bool(re.compile(r"^[a-zA-Z0-9_]+$").match(string)):
-        if not string[0].isnumeric():
-            return True
-    return False
+    return bool(string.replace("_", "").isalnum() and not string[0].isnumeric())
 
 
 def compare_ast(
     node1: Union[ast.expr, List[ast.expr], ast.Module],
     node2: Union[ast.expr, List[ast.expr], ast.Module],
     ignore_args: bool = False,
     ignore_imports: bool = False,
```

### Comparing `lazy_type_hint-2.0.9/pyproject.toml` & `lazy_type_hint-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "lazy-type-hint"
-version = "2.0.9"
-description = "Automate type hint generation in an easy way."
+version = "2.1.0"
+description = "Automate type hint generation in a single line."
 authors = ["Manuel Floriano Vázquez <mflovaa@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.urls]
 Source = "https://github.com/mflova/lazy-type-hint"
 
 [tool.poetry.dependencies]
```

### Comparing `lazy_type_hint-2.0.9/README.md` & `lazy_type_hint-2.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,25 @@
 
 Type hint any Python (nested) data structure! Dictionaries, callables, Pandas DataFrames...
 
 ```
 pip install lazy-type-hint
 ```
 
+## Quick examples
+
+```py
+from lazy_type_hint import LazyTypeHint, LazyTypeHintLive
+
+data = [1,2,3]
+LazyTypeHint().from_data(data, class_name="MyClass").to_file("file.py")
+LazyTypeHint().from_data(data, class_name="MyClass").to_string()
+data_type_hinted = LazyTypeHintLive().from_data(data, class_name="MyClass")
+```
+
 ## Main features
 
 1. Get corresponding type hints from any given data structure and with mutltiple parsing
    options. Export it as a file or as a string.
 
    ```py
       from lazy_type_hint import LazyTypeHint, ParsingStrategies
```

### Comparing `lazy_type_hint-2.0.9/PKG-INFO` & `lazy_type_hint-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: lazy-type-hint
-Version: 2.0.9
-Summary: Automate type hint generation in an easy way.
+Version: 2.1.0
+Summary: Automate type hint generation in a single line.
 Author: Manuel Floriano Vázquez
 Author-email: mflovaa@gmail.com
 Requires-Python: >=3.8,<=3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -18,14 +18,25 @@
 
 Type hint any Python (nested) data structure! Dictionaries, callables, Pandas DataFrames...
 
 ```
 pip install lazy-type-hint
 ```
 
+## Quick examples
+
+```py
+from lazy_type_hint import LazyTypeHint, LazyTypeHintLive
+
+data = [1,2,3]
+LazyTypeHint().from_data(data, class_name="MyClass").to_file("file.py")
+LazyTypeHint().from_data(data, class_name="MyClass").to_string()
+data_type_hinted = LazyTypeHintLive().from_data(data, class_name="MyClass")
+```
+
 ## Main features
 
 1. Get corresponding type hints from any given data structure and with mutltiple parsing
    options. Export it as a file or as a string.
 
    ```py
       from lazy_type_hint import LazyTypeHint, ParsingStrategies
```

