# Comparing `tmp/edgedb_pydantic_codegen-2024.4.1.tar.gz` & `tmp/edgedb_pydantic_codegen-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgedb_pydantic_codegen-2024.4.1.tar", max compression
+gzip compressed data, was "edgedb_pydantic_codegen-2024.4.2.tar", max compression
```

## Comparing `edgedb_pydantic_codegen-2024.4.1.tar` & `edgedb_pydantic_codegen-2024.4.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1063 2024-04-12 23:38:16.281825 edgedb_pydantic_codegen-2024.4.1/LICENSE
--rw-r--r--   0        0        0     2717 2024-04-12 23:38:16.281825 edgedb_pydantic_codegen-2024.4.1/README.md
--rw-r--r--   0        0        0       88 2024-04-12 23:38:16.285825 edgedb_pydantic_codegen-2024.4.1/edgedb_pydantic_codegen/__init__.py
--rw-r--r--   0        0        0      621 2024-04-12 23:38:16.285825 edgedb_pydantic_codegen-2024.4.1/edgedb_pydantic_codegen/__main__.py
--rw-r--r--   0        0        0     7774 2024-04-12 23:38:16.285825 edgedb_pydantic_codegen-2024.4.1/edgedb_pydantic_codegen/generator.py
--rw-r--r--   0        0        0     1475 2024-04-12 23:38:16.285825 edgedb_pydantic_codegen-2024.4.1/edgedb_pydantic_codegen/models.py
--rw-r--r--   0        0        0     1911 2024-04-12 23:38:16.285825 edgedb_pydantic_codegen-2024.4.1/edgedb_pydantic_codegen/template.py.jinja
--rw-r--r--   0        0        0     1198 2024-04-12 23:38:16.285825 edgedb_pydantic_codegen-2024.4.1/edgedb_pydantic_codegen/utils.py
--rw-r--r--   0        0        0      817 2024-04-12 23:38:16.285825 edgedb_pydantic_codegen-2024.4.1/pyproject.toml
--rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 edgedb_pydantic_codegen-2024.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-19 23:39:19.182169 edgedb_pydantic_codegen-2024.4.2/LICENSE
+-rw-r--r--   0        0        0     2946 2024-04-19 23:39:19.182169 edgedb_pydantic_codegen-2024.4.2/README.md
+-rw-r--r--   0        0        0       88 2024-04-19 23:39:19.182169 edgedb_pydantic_codegen-2024.4.2/edgedb_pydantic_codegen/__init__.py
+-rw-r--r--   0        0        0      621 2024-04-19 23:39:19.182169 edgedb_pydantic_codegen-2024.4.2/edgedb_pydantic_codegen/__main__.py
+-rw-r--r--   0        0        0    10297 2024-04-19 23:39:19.182169 edgedb_pydantic_codegen-2024.4.2/edgedb_pydantic_codegen/generator.py
+-rw-r--r--   0        0        0     2013 2024-04-19 23:39:19.182169 edgedb_pydantic_codegen-2024.4.2/edgedb_pydantic_codegen/models.py
+-rw-r--r--   0        0        0     2057 2024-04-19 23:39:19.182169 edgedb_pydantic_codegen-2024.4.2/edgedb_pydantic_codegen/template.py.jinja
+-rw-r--r--   0        0        0     1290 2024-04-19 23:39:19.182169 edgedb_pydantic_codegen-2024.4.2/edgedb_pydantic_codegen/utils.py
+-rw-r--r--   0        0        0      817 2024-04-19 23:39:19.182169 edgedb_pydantic_codegen-2024.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3766 1970-01-01 00:00:00.000000 edgedb_pydantic_codegen-2024.4.2/PKG-INFO
```

### Comparing `edgedb_pydantic_codegen-2024.4.1/LICENSE` & `edgedb_pydantic_codegen-2024.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edgedb_pydantic_codegen-2024.4.1/README.md` & `edgedb_pydantic_codegen-2024.4.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -96,7 +96,14 @@
         EDGEQL_QUERY,
         discord_id=discord_id,
         moecoins=moecoins,
         blood_shards=blood_shards,
     )
     return adapter.validate_json(resp, strict=False)
 ```
+
+## Caveats
+
+Currently this tool does not support:
+
+- `TupleType`, `RangeType` and `MultiRangeType` collections
+- `std::duration`, `cal::relative_duration`, `cal::date_duration`, `cfg::memory` and `ext::pgvector::vector` objects
```

### Comparing `edgedb_pydantic_codegen-2024.4.1/edgedb_pydantic_codegen/__main__.py` & `edgedb_pydantic_codegen-2024.4.2/edgedb_pydantic_codegen/__main__.py`

 * *Files identical despite different names*

### Comparing `edgedb_pydantic_codegen-2024.4.1/edgedb_pydantic_codegen/generator.py` & `edgedb_pydantic_codegen-2024.4.2/edgedb_pydantic_codegen/generator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,31 @@
+from collections import defaultdict
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 
 import edgedb
 from edgedb import describe
 from edgedb.enums import Cardinality
 from jinja2 import Environment, FileSystemLoader
 
 from edgedb_pydantic_codegen.models import (
     TYPE_MAPPING,
     EdgeQLArgument,
     EdgeQLEnum,
+    EdgeQLEnumMember,
     EdgeQLLiteral,
     EdgeQLModel,
     EdgeQLModelField,
+    EdgeQLNamedTuple,
+    EdgeQLNamedTupleField,
     ProcessData,
 )
 from edgedb_pydantic_codegen.utils import (
     camel_to_snake,
+    escape,
     ruff_fix,
     ruff_format,
     snake_to_camel,
 )
 
 
 class Generator:
@@ -54,38 +59,38 @@
         ruff_format(output_path)
 
     def process_query(self, filestem: str, query: str) -> str:
         process_data = ProcessData(query)
 
         describe_result = self._client._describe_query(query, inject_type_names=True)
 
-        return_model = None
         if describe_result.output_type is not None:
-            return_model_name = snake_to_camel(filestem) + "Result"
-            return_model = self.parse_model(
-                return_model_name,
-                describe_result.output_type,  # type: ignore
+            return_type_str = self.parse_type(
+                "Result",
+                describe_result.output_type,
+                snake_to_camel(filestem),
                 process_data,
+                prefer_literal=False,
             )
 
             return_cardinality = describe_result.output_cardinality
             if return_cardinality is Cardinality.NO_RESULT:
                 process_data.return_type = "None"
                 process_data.return_single = True
             elif return_cardinality is Cardinality.AT_MOST_ONE:
-                process_data.return_type = f"{return_model.name} | None"
+                process_data.return_type = f"{return_type_str} | None"
                 process_data.return_single = True
             elif return_cardinality is Cardinality.ONE:
-                process_data.return_type = f"{return_model.name}"
+                process_data.return_type = f"{return_type_str}"
                 process_data.return_single = True
             elif return_cardinality is Cardinality.MANY:
-                process_data.return_type = f"list[{return_model.name}]"
+                process_data.return_type = f"list[{return_type_str}]"
                 process_data.return_single = False
             elif return_cardinality is Cardinality.AT_LEAST_ONE:
-                process_data.return_type = f"list[{return_model.name}]"
+                process_data.return_type = f"list[{return_type_str}]"
                 process_data.return_single = False
 
         if describe_result.input_type is not None:
             for name, arg in describe_result.input_type.elements.items(  # type: ignore
             ):
                 type_str = self.parse_type(
                     name,
@@ -108,14 +113,15 @@
 
         rendered = template.render(
             stem=filestem,
             query=process_data.query.strip(),
             literals=process_data.literals.values(),
             enums=process_data.enums.values(),
             models=process_data.models.values(),
+            namedtuples=process_data.namedtuples.values(),
             args=(
                 list(process_data.args.values())
                 + list(process_data.optional_args.values())
             ),
             return_type=process_data.return_type,
             return_single=process_data.return_single,
         )
@@ -129,57 +135,101 @@
         type: describe.AnyType,
         parent_model_name: str,
         process_data: ProcessData,
         prefer_literal: bool = False,
     ) -> str:
         type_str = None
 
-        if isinstance(type, describe.ScalarType):
-            assert type.base_type.name is not None
-            type_str = TYPE_MAPPING.get(type.base_type.name, "Any")
-
-        elif isinstance(type, describe.BaseScalarType):
-            assert type.name is not None
-            type_str = TYPE_MAPPING.get(type.name, "Any")
-
-        elif isinstance(type, describe.EnumType):
-            if (
-                not prefer_literal and type.name is not None
-            ):  # an enum present in the schema
-                module, enum_name = type.name.split("::")
-                if module != "default":
-                    enum_name = module.title() + enum_name
-                else:
-                    enum_name = enum_name
-                process_data.enums[enum_name] = EdgeQLEnum(enum_name, type.members)
-                type_str = enum_name
-            else:  # use a literal
-                alias = (camel_to_snake(parent_model_name) + "_" + name).upper()
-                process_data.literals[alias] = EdgeQLLiteral(alias, type.members)
-                type_str = alias
-
-        elif isinstance(type, describe.ObjectType):
-            model_name = parent_model_name + snake_to_camel(name)
-            cls.parse_model(
-                model_name, type, process_data, prefer_literal=prefer_literal
-            )
-            type_str = model_name
+        match type:
+            case describe.BaseScalarType(_, name=tname):
+                assert tname is not None
+                type_str = TYPE_MAPPING.get(tname, "Any")
+
+            case describe.ScalarType(_, _, base_type):
+                assert base_type.name is not None
+                type_str = TYPE_MAPPING.get(base_type.name, "Any")
+
+            case describe.EnumType():
+                type_str = cls.parse_enum(
+                    name, type, parent_model_name, process_data, prefer_literal
+                )
 
-        elif isinstance(type, describe.ArrayType):
-            element_type_str = cls.parse_type(
-                name,
-                type.element_type,
-                parent_model_name,
-                process_data,
-                prefer_literal=prefer_literal,
+            case describe.NamedTupleType():
+                model_name = parent_model_name + snake_to_camel(name)
+                cls.parse_namedtuple(
+                    model_name, type, process_data, prefer_literal=prefer_literal
+                )
+                type_str = model_name
+
+            case describe.ObjectType():
+                model_name = parent_model_name + snake_to_camel(name)
+                cls.parse_model(
+                    model_name, type, process_data, prefer_literal=prefer_literal
+                )
+                type_str = model_name
+
+            case describe.SequenceType():
+                element_type_str = cls.parse_type(
+                    name,
+                    type.element_type,
+                    parent_model_name,
+                    process_data,
+                    prefer_literal=prefer_literal,
+                )
+                match type:
+                    case describe.ArrayType():
+                        type_str = f"list[{element_type_str}]"
+                    case describe.SetType():
+                        type_str = f"set[{element_type_str}]"
+                    case _:
+                        type_str = f"Sequence[{element_type_str}]"
+
+            case _: # TODO: TupleType, RangeType, MultiRangeType
+                raise ValueError(f"Unsupported type: {type}")
+
+        return type_str
+
+    @classmethod
+    def parse_enum(
+        cls,
+        name: str,
+        type: describe.EnumType,
+        parent_model_name: str,
+        process_data: ProcessData,
+        prefer_literal: bool = False,
+    ) -> str:
+        if not prefer_literal and type.name is not None:
+            module, enum_name = type.name.split("::")
+            if module != "default":
+                enum_name = module.title() + enum_name
+            else:
+                enum_name = enum_name
+
+            members: dict[str, EdgeQLEnumMember] = {}
+            name_counts = defaultdict(int)
+            for member in type.members:
+                name = escape(member)
+                # handle duplicate names after escaping (e.g. "a-b" and "a b" -> "a_b" and "a_b1")
+                name_counts[name] += 1
+                if name_counts[name] > 1:
+                    name = f"{name}{name_counts[name]-1}"
+                    # handle invalid names (starting with a number)
+                if not name.isidentifier():
+                    name = f"E{name}"
+                members[name] = EdgeQLEnumMember(name, member)
+
+            process_data.enums[enum_name] = EdgeQLEnum(
+                enum_name, list(members.values())
             )
-            type_str = f"list[{element_type_str}]"
+            type_str = enum_name
 
-        if type_str is None:
-            raise ValueError(f"Unknown type: {type}")
+        else:  # use a literal
+            alias = (camel_to_snake(parent_model_name) + "_" + name).upper()
+            process_data.literals[alias] = EdgeQLLiteral(alias, type.members)
+            type_str = alias
 
         return type_str
 
     @classmethod
     def parse_model(
         cls,
         model_name: str,
@@ -216,7 +266,33 @@
                 fields["id"].optional = False
             elif fields["id"].optional:
                 del fields["id"]
 
         new_model.fields = list(fields.values())
 
         return new_model
+
+    @classmethod
+    def parse_namedtuple(
+        cls,
+        model_name: str,
+        type: describe.NamedTupleType,
+        process_data: ProcessData,
+        prefer_literal: bool = False,
+    ) -> EdgeQLNamedTuple:
+        new_model = EdgeQLNamedTuple(model_name)
+        process_data.namedtuples[model_name] = new_model
+
+        fields: dict[str, EdgeQLNamedTupleField] = {}
+        for name, _type in type.element_types.items():
+            field_type = cls.parse_type(
+                name,
+                _type,
+                model_name,
+                process_data,
+                prefer_literal=prefer_literal,
+            )
+            fields[name] = EdgeQLNamedTupleField(name, field_type)
+
+        new_model.fields = list(fields.values())
+
+        return new_model
```

### Comparing `edgedb_pydantic_codegen-2024.4.1/edgedb_pydantic_codegen/models.py` & `edgedb_pydantic_codegen-2024.4.2/edgedb_pydantic_codegen/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,35 +7,57 @@
     "std::float64": "float",
     "std::int16": "int",
     "std::int32": "int",
     "std::int64": "int",
     "std::bigint": "int",
     "std::bool": "bool",
     "std::uuid": "UUID",
-    "std::bytes": "str",
+    "std::bytes": "bytes",
     "std::decimal": "Decimal",
     "std::datetime": "datetime",
-    "std::duration": "timedelta",
+    # "std::duration": "timedelta",
+    "std::json": "Any",
     "cal::local_date": "date",
     "cal::local_time": "time",
     "cal::local_datetime": "datetime",
-    "std::json": "Any",
+    # "cal::relative_duration": "RelativeDuration",
+    # "cal::date_duration": "DateDuration",
+    # "cfg::memory": "ConfigMemory",
+    # "ext::pgvector::vector": "array",
 }
 
 
 @dataclass
+class EdgeQLEnumMember:
+    name: str
+    value: str
+
+
+@dataclass
 class EdgeQLEnum:
     name: str
-    members: tuple[str]
+    members: list[EdgeQLEnumMember]
 
 
 @dataclass
 class EdgeQLLiteral:
     alias: str
-    values: tuple[str]
+    values: tuple[str, ...]
+
+
+@dataclass
+class EdgeQLNamedTuple:
+    name: str
+    fields: list["EdgeQLNamedTupleField"] = dc_field(default_factory=list)
+
+
+@dataclass
+class EdgeQLNamedTupleField:
+    name: str
+    type_str: str
 
 
 @dataclass
 class EdgeQLModel:
     name: str
     fields: list["EdgeQLModelField"] = dc_field(default_factory=list)
 
@@ -55,11 +77,12 @@
 
 @dataclass
 class ProcessData:
     query: str
     literals: dict[str, EdgeQLLiteral] = dc_field(default_factory=dict)
     enums: dict[str, EdgeQLEnum] = dc_field(default_factory=dict)
     models: dict[str, EdgeQLModel] = dc_field(default_factory=dict)
+    namedtuples: dict[str, EdgeQLNamedTuple] = dc_field(default_factory=dict)
     args: dict[str, EdgeQLArgument] = dc_field(default_factory=dict)
     optional_args: dict[str, EdgeQLArgument] = dc_field(default_factory=dict)
     return_type: str = "None"
     return_single: bool = True
```

### Comparing `edgedb_pydantic_codegen-2024.4.1/edgedb_pydantic_codegen/template.py.jinja` & `edgedb_pydantic_codegen-2024.4.2/edgedb_pydantic_codegen/template.py.jinja`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,44 @@
+from collections.abc import Sequence
+from datetime import date, datetime, time
+from decimal import Decimal
+from enum import StrEnum
+from typing import Any, Literal
+from uuid import UUID
+
 import orjson
 from edgedb import AsyncIOExecutor
 from pydantic import BaseModel, Field, TypeAdapter
 
-from uuid import UUID
-from decimal import Decimal
-from datetime import datetime
-from datetime import timedelta
-from datetime import date
-from datetime import time
-from typing import Any
-
-from typing import Literal
-from enum import StrEnum
-
 EDGEQL_QUERY = r"""
 {{query}}
 """
 
 {% for literal in literals %}
 {{literal.alias}} = Literal[
     {% for value in literal.values %}
     "{{value}}",
     {% endfor %}
 ]
 {% endfor %}
 
 {% for enum in enums %}
 class {{enum.name}}(StrEnum):
-    {%- for value in enum.members %}
-    {{value}} = "{{value}}"
+    {%- for member in enum.members %}
+    {{member.name}} = "{{member.value}}"
     {%- endfor %}
 {% endfor %}
 
+{% for ntuple in namedtuples | reverse %}
+class {{ntuple.name}}(NamedTuple):
+    {% for field in ntuple.fields -%}
+    {{field.name}}: {{field.type_str}}
+    {% endfor %}
+{% endfor %}
+
 {% for model in models | reverse %}
 class {{model.name}}(BaseModel):
     {% for field in model.fields -%}
     {{field.name}}:
     {%- if field.optional -%}
     {{field.type_str}} | None
     {%- else -%}
```

### Comparing `edgedb_pydantic_codegen-2024.4.1/edgedb_pydantic_codegen/utils.py` & `edgedb_pydantic_codegen-2024.4.2/edgedb_pydantic_codegen/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 import re
 import subprocess
 from pathlib import Path
 
 from ruff.__main__ import find_ruff_bin
 
 
+def escape(identifier: str) -> str:
+    return re.sub(r"[^a-zA-Z0-9_]", "_", identifier)
+
+
 def snake_to_camel(snake_str: str) -> str:
     components = snake_str.split("_")
     return "".join(x.title() for x in components)
 
 
 def camel_to_snake(camel_str: str) -> str:
-    return re.sub("([A-Z])", "_\\1", camel_str).lower().lstrip("_")
+    return re.sub(r"([A-Z])", r"_\1", camel_str).lower().lstrip("_")
 
 
 def ruff_fix(path: Path):
     ruff = find_ruff_bin()
     proc = subprocess.run(
         [
             os.fsdecode(ruff),
```

### Comparing `edgedb_pydantic_codegen-2024.4.1/pyproject.toml` & `edgedb_pydantic_codegen-2024.4.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgedb-pydantic-codegen"
-version = "2024.04.1"
+version = "2024.04.2"
 description = "Alternative Python EdgeDB code generator (Pydantic V2 + asyncio, FastAPI compatible)"
 authors = ["NextFire <git@yuru.moe>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Japan7/edgedb-pydantic-codegen"
 
 [tool.poetry.scripts]
@@ -17,15 +17,15 @@
 jinja2 = "^3.0.0"
 ruff = ">=0.1.2,<1"
 # runtime
 pydantic = "^2.0.0"
 orjson = "^3.0.0"
 
 [tool.poetry.group.dev.dependencies]
-pyright = "1.1.358"
+pyright = "1.1.359"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pyright]
 pythonVersion = "3.11"
```

### Comparing `edgedb_pydantic_codegen-2024.4.1/PKG-INFO` & `edgedb_pydantic_codegen-2024.4.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgedb-pydantic-codegen
-Version: 2024.4.1
+Version: 2024.4.2
 Summary: Alternative Python EdgeDB code generator (Pydantic V2 + asyncio, FastAPI compatible)
 Home-page: https://github.com/Japan7/edgedb-pydantic-codegen
 License: MIT
 Author: NextFire
 Author-email: git@yuru.moe
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -118,7 +118,14 @@
         discord_id=discord_id,
         moecoins=moecoins,
         blood_shards=blood_shards,
     )
     return adapter.validate_json(resp, strict=False)
 ```
 
+## Caveats
+
+Currently this tool does not support:
+
+- `TupleType`, `RangeType` and `MultiRangeType` collections
+- `std::duration`, `cal::relative_duration`, `cal::date_duration`, `cfg::memory` and `ext::pgvector::vector` objects
+
```

