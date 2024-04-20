# Comparing `tmp/hasura_ndc-0.8.tar.gz` & `tmp/hasura_ndc-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hasura_ndc-0.8.tar", last modified: Fri Apr 19 20:35:02 2024, max compression
+gzip compressed data, was "hasura_ndc-0.9.tar", last modified: Fri Apr 19 21:13:48 2024, max compression
```

## Comparing `hasura_ndc-0.8.tar` & `hasura_ndc-0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tristen    (502) staff       (20)        0 2024-04-19 20:35:02.073182 hasura_ndc-0.8/
--rw-r--r--   0 tristen    (502) staff       (20)      683 2024-04-19 20:35:02.073053 hasura_ndc-0.8/PKG-INFO
--rw-r--r--   0 tristen    (502) staff       (20)      309 2023-12-17 06:14:09.000000 hasura_ndc-0.8/README.md
-drwxr-xr-x   0 tristen    (502) staff       (20)        0 2024-04-19 20:35:02.072088 hasura_ndc-0.8/hasura_ndc/
--rw-r--r--   0 tristen    (502) staff       (20)       30 2024-04-19 15:18:26.000000 hasura_ndc-0.8/hasura_ndc/__init__.py
--rw-r--r--   0 tristen    (502) staff       (20)     2247 2024-04-19 18:35:54.000000 hasura_ndc-0.8/hasura_ndc/connector.py
--rw-r--r--   0 tristen    (502) staff       (20)     3978 2024-04-19 20:17:06.000000 hasura_ndc-0.8/hasura_ndc/instrumentation.py
--rw-r--r--   0 tristen    (502) staff       (20)     1722 2024-04-19 20:33:51.000000 hasura_ndc-0.8/hasura_ndc/main.py
--rw-r--r--   0 tristen    (502) staff       (20)    22361 2024-04-19 18:28:10.000000 hasura_ndc-0.8/hasura_ndc/models.py
--rw-r--r--   0 tristen    (502) staff       (20)     3692 2024-04-19 20:34:21.000000 hasura_ndc-0.8/hasura_ndc/server.py
-drwxr-xr-x   0 tristen    (502) staff       (20)        0 2024-04-19 20:35:02.072877 hasura_ndc-0.8/hasura_ndc.egg-info/
--rw-r--r--   0 tristen    (502) staff       (20)      683 2024-04-19 20:35:02.000000 hasura_ndc-0.8/hasura_ndc.egg-info/PKG-INFO
--rw-r--r--   0 tristen    (502) staff       (20)      325 2024-04-19 20:35:02.000000 hasura_ndc-0.8/hasura_ndc.egg-info/SOURCES.txt
--rw-r--r--   0 tristen    (502) staff       (20)        1 2024-04-19 20:35:02.000000 hasura_ndc-0.8/hasura_ndc.egg-info/dependency_links.txt
--rw-r--r--   0 tristen    (502) staff       (20)      936 2024-04-19 20:35:02.000000 hasura_ndc-0.8/hasura_ndc.egg-info/requires.txt
--rw-r--r--   0 tristen    (502) staff       (20)       11 2024-04-19 20:35:02.000000 hasura_ndc-0.8/hasura_ndc.egg-info/top_level.txt
--rw-r--r--   0 tristen    (502) staff       (20)       38 2024-04-19 20:35:02.073225 hasura_ndc-0.8/setup.cfg
--rw-r--r--   0 tristen    (502) staff       (20)      844 2024-04-19 20:27:55.000000 hasura_ndc-0.8/setup.py
+drwxr-xr-x   0 tristen    (502) staff       (20)        0 2024-04-19 21:13:48.586608 hasura_ndc-0.9/
+-rw-r--r--   0 tristen    (502) staff       (20)      683 2024-04-19 21:13:48.586495 hasura_ndc-0.9/PKG-INFO
+-rw-r--r--   0 tristen    (502) staff       (20)      309 2023-12-17 06:14:09.000000 hasura_ndc-0.9/README.md
+drwxr-xr-x   0 tristen    (502) staff       (20)        0 2024-04-19 21:13:48.585751 hasura_ndc-0.9/hasura_ndc/
+-rw-r--r--   0 tristen    (502) staff       (20)       30 2024-04-19 15:18:26.000000 hasura_ndc-0.9/hasura_ndc/__init__.py
+-rw-r--r--   0 tristen    (502) staff       (20)     2247 2024-04-19 18:35:54.000000 hasura_ndc-0.9/hasura_ndc/connector.py
+-rw-r--r--   0 tristen    (502) staff       (20)     3978 2024-04-19 20:17:06.000000 hasura_ndc-0.9/hasura_ndc/instrumentation.py
+-rw-r--r--   0 tristen    (502) staff       (20)     1722 2024-04-19 20:33:51.000000 hasura_ndc-0.9/hasura_ndc/main.py
+-rw-r--r--   0 tristen    (502) staff       (20)    23013 2024-04-19 21:13:04.000000 hasura_ndc-0.9/hasura_ndc/models.py
+-rw-r--r--   0 tristen    (502) staff       (20)     3692 2024-04-19 20:34:21.000000 hasura_ndc-0.9/hasura_ndc/server.py
+drwxr-xr-x   0 tristen    (502) staff       (20)        0 2024-04-19 21:13:48.586343 hasura_ndc-0.9/hasura_ndc.egg-info/
+-rw-r--r--   0 tristen    (502) staff       (20)      683 2024-04-19 21:13:48.000000 hasura_ndc-0.9/hasura_ndc.egg-info/PKG-INFO
+-rw-r--r--   0 tristen    (502) staff       (20)      325 2024-04-19 21:13:48.000000 hasura_ndc-0.9/hasura_ndc.egg-info/SOURCES.txt
+-rw-r--r--   0 tristen    (502) staff       (20)        1 2024-04-19 21:13:48.000000 hasura_ndc-0.9/hasura_ndc.egg-info/dependency_links.txt
+-rw-r--r--   0 tristen    (502) staff       (20)      936 2024-04-19 21:13:48.000000 hasura_ndc-0.9/hasura_ndc.egg-info/requires.txt
+-rw-r--r--   0 tristen    (502) staff       (20)       11 2024-04-19 21:13:48.000000 hasura_ndc-0.9/hasura_ndc.egg-info/top_level.txt
+-rw-r--r--   0 tristen    (502) staff       (20)       38 2024-04-19 21:13:48.586644 hasura_ndc-0.9/setup.cfg
+-rw-r--r--   0 tristen    (502) staff       (20)      844 2024-04-19 21:13:32.000000 hasura_ndc-0.9/setup.py
```

### Comparing `hasura_ndc-0.8/PKG-INFO` & `hasura_ndc-0.9/hasura_ndc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hasura_ndc
-Version: 0.8
+Name: hasura-ndc
+Version: 0.9
 Summary: A Hasura Data Connector SDK
 Author: Tristen Harr
 Author-email: tristen.harr@hasura.io
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `hasura_ndc-0.8/hasura_ndc/connector.py` & `hasura_ndc-0.9/hasura_ndc/connector.py`

 * *Files identical despite different names*

### Comparing `hasura_ndc-0.8/hasura_ndc/instrumentation.py` & `hasura_ndc-0.9/hasura_ndc/instrumentation.py`

 * *Files identical despite different names*

### Comparing `hasura_ndc-0.8/hasura_ndc/main.py` & `hasura_ndc-0.9/hasura_ndc/main.py`

 * *Files identical despite different names*

### Comparing `hasura_ndc-0.8/hasura_ndc/models.py` & `hasura_ndc-0.9/hasura_ndc/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,166 +12,166 @@
 class Type(RootModel):
     type: Literal["named", "nullable", "array", "predicate"]
     name: Optional[str] = None
     underlying_type: Optional['Type'] = None
     element_type: Optional['Type'] = None
     object_type_name: Optional[str] = None
 
-    @model_validator(mode="before")
-    def validate_fields(self, data):
-        type_t = data.get('type')
-        name = data.get('name')
-        underlying_type = data.get('underlying_type')
-        element_type = data.get('element_type')
-        object_type_name = data.get('object_type_name')
-
-        if type_t == 'named':
-            if not name:
-                raise ValueError("name is required when type is 'named'")
-            if any([underlying_type, element_type, object_type_name]):
-                raise ValueError("Only 'name' should be set when type is 'named'")
-        elif type_t == 'nullable':
-            if not underlying_type:
-                raise ValueError("underlying_type is required when type is 'nullable'")
-            if any([name, element_type, object_type_name]):
-                raise ValueError("Only 'underlying_type' should be set when type is 'nullable'")
-        elif type_t == 'array':
-            if not element_type:
-                raise ValueError("element_type is required when type is 'array'")
-            if any([name, underlying_type, object_type_name]):
-                raise ValueError("Only 'element_type' should be set when type is 'array'")
-        elif type_t == 'predicate':
-            if not object_type_name:
-                raise ValueError("object_type_name is required when type is 'predicate'")
-            if any([name, underlying_type, element_type]):
-                raise ValueError("Only 'object_type_name' should be set when type is 'predicate'")
-        else:
-            raise ValueError(f"Invalid type value: {type_t}")
-        return data
+    # @model_validator(mode="before")
+    # def validate_fields(self, data):
+    #     type_t = data.get('type')
+    #     name = data.get('name')
+    #     underlying_type = data.get('underlying_type')
+    #     element_type = data.get('element_type')
+    #     object_type_name = data.get('object_type_name')
+    #
+    #     if type_t == 'named':
+    #         if not name:
+    #             raise ValueError("name is required when type is 'named'")
+    #         if any([underlying_type, element_type, object_type_name]):
+    #             raise ValueError("Only 'name' should be set when type is 'named'")
+    #     elif type_t == 'nullable':
+    #         if not underlying_type:
+    #             raise ValueError("underlying_type is required when type is 'nullable'")
+    #         if any([name, element_type, object_type_name]):
+    #             raise ValueError("Only 'underlying_type' should be set when type is 'nullable'")
+    #     elif type_t == 'array':
+    #         if not element_type:
+    #             raise ValueError("element_type is required when type is 'array'")
+    #         if any([name, underlying_type, object_type_name]):
+    #             raise ValueError("Only 'element_type' should be set when type is 'array'")
+    #     elif type_t == 'predicate':
+    #         if not object_type_name:
+    #             raise ValueError("object_type_name is required when type is 'predicate'")
+    #         if any([name, underlying_type, element_type]):
+    #             raise ValueError("Only 'object_type_name' should be set when type is 'predicate'")
+    #     else:
+    #         raise ValueError(f"Invalid type value: {type_t}")
+    #     return data
 
 
 class Aggregate(RootModel):
     type: Literal["column_count", "single_column", "star_count"]
     column: Optional[str] = None
     distinct: Optional[bool] = None
     function: Optional[str] = None
 
-    @model_validator(mode="before")
-    def validate_fields(self, data):
-        type_t = data.get('type')
-        column = data.get('column')
-        distinct = data.get('distinct')
-        function = data.get('function')
-
-        if type_t == 'column_count':
-            if not column:
-                raise ValueError("column is required when type is 'column_count'")
-            if distinct is None:
-                raise ValueError("distinct is required when type is 'column_count'")
-            if function is not None:
-                raise ValueError("Only 'column' and 'distinct' should be set when type is 'column_count'")
-        elif type_t == 'single_column':
-            if not column:
-                raise ValueError("column is required when type is 'single_column'")
-            if function is None:
-                raise ValueError("function is required when type is 'single_column'")
-            if distinct is not None:
-                raise ValueError("Only 'column' and 'function' should be set when type is 'single_column'")
-        elif type_t == 'star_count':
-            if column is not None:
-                raise ValueError("'star_count' does not have any arguments")
-            if distinct is not None:
-                raise ValueError("'star_count' does not have any arguments")
-            if function is not None:
-                raise ValueError("'star_count' does not have any arguments")
-        else:
-            raise ValueError(f"Invalid type value: {type_t}")
-        return data
+    # @model_validator(mode="before")
+    # def validate_fields(self, data):
+    #     type_t = data.get('type')
+    #     column = data.get('column')
+    #     distinct = data.get('distinct')
+    #     function = data.get('function')
+    #
+    #     if type_t == 'column_count':
+    #         if not column:
+    #             raise ValueError("column is required when type is 'column_count'")
+    #         if distinct is None:
+    #             raise ValueError("distinct is required when type is 'column_count'")
+    #         if function is not None:
+    #             raise ValueError("Only 'column' and 'distinct' should be set when type is 'column_count'")
+    #     elif type_t == 'single_column':
+    #         if not column:
+    #             raise ValueError("column is required when type is 'single_column'")
+    #         if function is None:
+    #             raise ValueError("function is required when type is 'single_column'")
+    #         if distinct is not None:
+    #             raise ValueError("Only 'column' and 'function' should be set when type is 'single_column'")
+    #     elif type_t == 'star_count':
+    #         if column is not None:
+    #             raise ValueError("'star_count' does not have any arguments")
+    #         if distinct is not None:
+    #             raise ValueError("'star_count' does not have any arguments")
+    #         if function is not None:
+    #             raise ValueError("'star_count' does not have any arguments")
+    #     else:
+    #         raise ValueError(f"Invalid type value: {type_t}")
+    #     return data
 
 
 class Argument(RootModel):
     type: Literal["variable", "literal"]
     name: Optional[str] = None
     value: Optional[Any] = None
 
-    @model_validator(mode="before")
-    def validate_fields(self, data):
-        type_t = data.get('type')
-        name = data.get('name')
-        value = data.get('value')
-
-        if type_t == "variable":
-            if not name:
-                raise ValueError("name is required when type is 'variable'")
-            if value is not None:
-                raise ValueError("Only 'name' should be set when type is 'variable'")
-        elif type_t == "literal":
-            if name is not None:
-                raise ValueError("Only 'value' should be set when type is 'literal'")
-        else:
-            raise ValueError(f"Invalid type value: {type_t}")
-        return data
+    # @model_validator(mode="before")
+    # def validate_fields(self, data):
+    #     type_t = data.get('type')
+    #     name = data.get('name')
+    #     value = data.get('value')
+    #
+    #     if type_t == "variable":
+    #         if not name:
+    #             raise ValueError("name is required when type is 'variable'")
+    #         if value is not None:
+    #             raise ValueError("Only 'name' should be set when type is 'variable'")
+    #     elif type_t == "literal":
+    #         if name is not None:
+    #             raise ValueError("Only 'value' should be set when type is 'literal'")
+    #     else:
+    #         raise ValueError(f"Invalid type value: {type_t}")
+    #     return data
 
 
 class ComparisonTarget(RootModel):
     type: Literal["column", "root_collection_column"]
     name: str
     path: Optional['PathElement'] = None
 
-    @model_validator(mode="before")
-    def validate_fields(self, data):
-        type_t = data.get("type")
-        path = data.get("path")
-
-        if type_t == "column":
-            if path is None:
-                raise ValueError("path is required when type is 'column'")
-        elif type_t == "root_collection_column":
-            if path is not None:
-                raise ValueError("Only 'name' should be set when type is 'root_collection_column'")
-        else:
-            raise ValueError(f"Invalid type value: {type_t}")
-        return data
+    # @model_validator(mode="before")
+    # def validate_fields(self, data):
+    #     type_t = data.get("type")
+    #     path = data.get("path")
+    #
+    #     if type_t == "column":
+    #         if path is None:
+    #             raise ValueError("path is required when type is 'column'")
+    #     elif type_t == "root_collection_column":
+    #         if path is not None:
+    #             raise ValueError("Only 'name' should be set when type is 'root_collection_column'")
+    #     else:
+    #         raise ValueError(f"Invalid type value: {type_t}")
+    #     return data
 
 
 class ComparisonValue(RootModel):
     type: Literal["column", "scalar", "variable"]
     column: Optional['ComparisonTarget'] = None
     value: Optional[Any] = None
     name: Optional[str] = None
 
-    @model_validator(mode="before")
-    def validate_fields(self, data):
-        type_t = data.get("type")
-        column = data.get("column")
-        value = data.get("value")
-        name = data.get("name")
-
-        if type_t == "column":
-            if column is None:
-                raise ValueError("column is required when type is 'column'")
-            if value is not None:
-                raise ValueError("Only 'column' should be set when type is 'column'")
-            if name is not None:
-                raise ValueError("Only 'column' should be set when type is 'column'")
-        elif type_t == "scalar":
-            if column is not None:
-                raise ValueError("Only 'value' should be set when type is 'scalar'")
-            if name is not None:
-                raise ValueError("Only 'value' should be set when type is 'scalar'")
-        elif type_t == "variable":
-            if column is not None:
-                raise ValueError("Only 'name' should be set when type is 'variable'")
-            if value is not None:
-                raise ValueError("Only 'name' should be set when type is 'variable'")
-            if name is None:
-                raise ValueError("name is required when type is 'variable'")
-        else:
-            raise ValueError(f"Invalid type value: {type_t}")
-        return data
+    # @model_validator(mode="before")
+    # def validate_fields(self, data):
+    #     type_t = data.get("type")
+    #     column = data.get("column")
+    #     value = data.get("value")
+    #     name = data.get("name")
+    #
+    #     if type_t == "column":
+    #         if column is None:
+    #             raise ValueError("column is required when type is 'column'")
+    #         if value is not None:
+    #             raise ValueError("Only 'column' should be set when type is 'column'")
+    #         if name is not None:
+    #             raise ValueError("Only 'column' should be set when type is 'column'")
+    #     elif type_t == "scalar":
+    #         if column is not None:
+    #             raise ValueError("Only 'value' should be set when type is 'scalar'")
+    #         if name is not None:
+    #             raise ValueError("Only 'value' should be set when type is 'scalar'")
+    #     elif type_t == "variable":
+    #         if column is not None:
+    #             raise ValueError("Only 'name' should be set when type is 'variable'")
+    #         if value is not None:
+    #             raise ValueError("Only 'name' should be set when type is 'variable'")
+    #         if name is None:
+    #             raise ValueError("name is required when type is 'variable'")
+    #     else:
+    #         raise ValueError(f"Invalid type value: {type_t}")
+    #     return data
 
 
 UnaryComparisonOperator = "is_null"
 
 
 class Expression(RootModel):
     type: Literal["and", "or", "not", "unary_comparison_operator", "binary_comparison_operator", "exists"]
@@ -179,118 +179,118 @@
     expression: Optional['Expression'] = None
     column: Optional['ComparisonTarget'] = None
     operator: Optional[str] = None
     value: Optional['ComparisonValue'] = None
     in_collection: Optional['ExistsInCollection'] = None
     predicate: Optional['Expression'] = None
 
-    @model_validator(mode="before")
-    def validate_fields(self, data):
-        type_t = data.get("type")
-        expressions = data.get("expressions")
-        expression = data.get("expression")
-        column = data.get("column")
-        operator = data.get("operator")
-        value = data.get("value")
-        in_collection = data.get("in_collection")
-        predicate = data.get("predicate")
-
-        if type_t == "and":
-            if expressions is None:
-                raise ValueError("expressions is required when type is 'and'")
-            elif any([expression, column, operator, value, in_collection, predicate]):
-                raise ValueError("Only 'expressions' should be set when type is 'and'")
-        elif type_t == "or":
-            if expressions is None:
-                raise ValueError("expressions is required when type is 'or'")
-            elif any([expression, column, operator, value, in_collection, predicate]):
-                raise ValueError("Only 'expressions' should be set when type is 'or'")
-        elif type_t == "not":
-            if expression is None:
-                raise ValueError("expression is required when type is 'not'")
-            elif any([expressions, column, operator, value, in_collection, predicate]):
-                raise ValueError("Only 'expression' should be set when type is 'not'")
-        elif type_t == "unary_comparison_operator":
-            if column is None:
-                raise ValueError("column is required when type is 'unary_comparison_operator'")
-            if operator != UnaryComparisonOperator:
-                raise ValueError(f"operator must be {UnaryComparisonOperator} when type is 'unary_comparison_operator'")
-            if any([expressions, expression, value, in_collection, predicate]):
-                raise ValueError("Only 'column' and 'operator' should be set when type is 'unary_comparison_operator'")
-        elif type_t == "binary_comparison_operator":
-            if column is None:
-                raise ValueError("column is required when type is 'binary_comparison_operator'")
-            if operator is None:
-                raise ValueError("operator is required when type is 'binary_comparison_operator'")
-            if value is None:
-                raise ValueError("value is required when type is 'binary_comparison_operator'")
-            if any([expressions, expression, in_collection, predicate]):
-                raise ValueError(
-                    "Only 'column' and 'operator' and 'value' should be set when type is 'binary_comparison_operator'")
-        elif type_t == "exists":
-            if in_collection is None:
-                raise ValueError("in_collection is required when type is 'exists'")
-            if any([expressions, expression, column, operator, value]):
-                raise ValueError("Only 'in_collection' and 'predicate' should be set when type is 'exists'")
-        else:
-            raise ValueError(f"Invalid type value: {type_t}")
-        return data
+    # @model_validator(mode="before")
+    # def validate_fields(self, data):
+    #     type_t = data.get("type")
+    #     expressions = data.get("expressions")
+    #     expression = data.get("expression")
+    #     column = data.get("column")
+    #     operator = data.get("operator")
+    #     value = data.get("value")
+    #     in_collection = data.get("in_collection")
+    #     predicate = data.get("predicate")
+    #
+    #     if type_t == "and":
+    #         if expressions is None:
+    #             raise ValueError("expressions is required when type is 'and'")
+    #         elif any([expression, column, operator, value, in_collection, predicate]):
+    #             raise ValueError("Only 'expressions' should be set when type is 'and'")
+    #     elif type_t == "or":
+    #         if expressions is None:
+    #             raise ValueError("expressions is required when type is 'or'")
+    #         elif any([expression, column, operator, value, in_collection, predicate]):
+    #             raise ValueError("Only 'expressions' should be set when type is 'or'")
+    #     elif type_t == "not":
+    #         if expression is None:
+    #             raise ValueError("expression is required when type is 'not'")
+    #         elif any([expressions, column, operator, value, in_collection, predicate]):
+    #             raise ValueError("Only 'expression' should be set when type is 'not'")
+    #     elif type_t == "unary_comparison_operator":
+    #         if column is None:
+    #             raise ValueError("column is required when type is 'unary_comparison_operator'")
+    #         if operator != UnaryComparisonOperator:
+    #             raise ValueError(f"operator must be {UnaryComparisonOperator} when type is 'unary_comparison_operator'")
+    #         if any([expressions, expression, value, in_collection, predicate]):
+    #             raise ValueError("Only 'column' and 'operator' should be set when type is 'unary_comparison_operator'")
+    #     elif type_t == "binary_comparison_operator":
+    #         if column is None:
+    #             raise ValueError("column is required when type is 'binary_comparison_operator'")
+    #         if operator is None:
+    #             raise ValueError("operator is required when type is 'binary_comparison_operator'")
+    #         if value is None:
+    #             raise ValueError("value is required when type is 'binary_comparison_operator'")
+    #         if any([expressions, expression, in_collection, predicate]):
+    #             raise ValueError(
+    #                 "Only 'column' and 'operator' and 'value' should be set when type is 'binary_comparison_operator'")
+    #     elif type_t == "exists":
+    #         if in_collection is None:
+    #             raise ValueError("in_collection is required when type is 'exists'")
+    #         if any([expressions, expression, column, operator, value]):
+    #             raise ValueError("Only 'in_collection' and 'predicate' should be set when type is 'exists'")
+    #     else:
+    #         raise ValueError(f"Invalid type value: {type_t}")
+    #     return data
 
 
 class PathElement(RootModel):
     relationship: str
     arguments: Dict[str, 'RelationshipArgument']
     predicate: Optional['Expression'] = None
 
-    @model_validator(mode="before")
-    def validate_fields(self, data):
-        relationship = data.get("relationship")
-        arguments = data.get("arguments")
-
-        if not relationship:
-            raise ValueError("relationship is required")
-        if not arguments:
-            raise ValueError("arguments must not be empty")
-        return data
+    # @model_validator(mode="before")
+    # def validate_fields(self, data):
+    #     relationship = data.get("relationship")
+    #     arguments = data.get("arguments")
+    #
+    #     if not relationship:
+    #         raise ValueError("relationship is required")
+    #     if not arguments:
+    #         raise ValueError("arguments must not be empty")
+    #     return data
 
 
 OrderDirection = Literal["asc", "desc"]
 
 
 class OrderByTarget(RootModel):
     type: Literal["column", "single_column_aggregate", "star_count_aggregate"]
     name: Optional[str]
     column: Optional[str]
     function: Optional[str]
     path: List['PathElement']
 
-    @model_validator(mode="before")
-    def validate_fields(self, data):
-        type_t = data.get('type')
-        name = data.get('name')
-        column = data.get('column')
-        function = data.get('function')
-
-        if type_t == 'column':
-            if not name:
-                raise ValueError("name is required when type is 'column'")
-            if any([column, function]):
-                raise ValueError("Only 'name' and 'path' should be set when type is 'column'")
-        elif type_t == 'single_column_aggregate':
-            if not column or not function:
-                raise ValueError("both 'column' and 'function' are required when type is 'single_column_aggregate'")
-            if name is not None:
-                raise ValueError(
-                    "Only 'column', 'function', and 'path' should be set when type is 'single_column_aggregate'")
-        elif type_t == 'star_count_aggregate':
-            if any([name, column, function]):
-                raise ValueError("Only 'path' should be set when type is 'star_count_aggregate'")
-        else:
-            raise ValueError(f"Invalid type value: {type_t}")
-        return data
+    # @model_validator(mode="before")
+    # def validate_fields(self, data):
+    #     type_t = data.get('type')
+    #     name = data.get('name')
+    #     column = data.get('column')
+    #     function = data.get('function')
+    #
+    #     if type_t == 'column':
+    #         if not name:
+    #             raise ValueError("name is required when type is 'column'")
+    #         if any([column, function]):
+    #             raise ValueError("Only 'name' and 'path' should be set when type is 'column'")
+    #     elif type_t == 'single_column_aggregate':
+    #         if not column or not function:
+    #             raise ValueError("both 'column' and 'function' are required when type is 'single_column_aggregate'")
+    #         if name is not None:
+    #             raise ValueError(
+    #                 "Only 'column', 'function', and 'path' should be set when type is 'single_column_aggregate'")
+    #     elif type_t == 'star_count_aggregate':
+    #         if any([name, column, function]):
+    #             raise ValueError("Only 'path' should be set when type is 'star_count_aggregate'")
+    #     else:
+    #         raise ValueError(f"Invalid type value: {type_t}")
+    #     return data
 
 
 class OrderBy(RootModel):
     elements: List['OrderByElement']
 
 
 class OrderByElement(RootModel):
@@ -308,119 +308,119 @@
 
 
 class RelationshipArgument(RootModel):
     type: Literal["variable", "literal", "column"]
     name: Optional[str] = None
     value: Optional[Any] = None
 
-    @model_validator(mode="before")
-    def validate_fields(self, data):
-        type_t = data.get('type')
-        name = data.get('name')
-        value = data.get('value')
-
-        if type_t == "variable":
-            if not name:
-                raise ValueError("name is required when type is 'variable'")
-            if value is not None:
-                raise ValueError("value should not be set when type is 'variable'")
-        elif type_t == "literal":
-            if name is not None:
-                raise ValueError("name should not be set when type is 'literal'")
-        elif type_t == "column":
-            if not name:
-                raise ValueError("name is required when type is 'column'")
-            if value is not None:
-                raise ValueError("value should not be set when type is 'column'")
-        else:
-            raise ValueError(f"Invalid type value: {type_t}")
-        return data
+    # @model_validator(mode="before")
+    # def validate_fields(self, data):
+    #     type_t = data.get('type')
+    #     name = data.get('name')
+    #     value = data.get('value')
+    #
+    #     if type_t == "variable":
+    #         if not name:
+    #             raise ValueError("name is required when type is 'variable'")
+    #         if value is not None:
+    #             raise ValueError("value should not be set when type is 'variable'")
+    #     elif type_t == "literal":
+    #         if name is not None:
+    #             raise ValueError("name should not be set when type is 'literal'")
+    #     elif type_t == "column":
+    #         if not name:
+    #             raise ValueError("name is required when type is 'column'")
+    #         if value is not None:
+    #             raise ValueError("value should not be set when type is 'column'")
+    #     else:
+    #         raise ValueError(f"Invalid type value: {type_t}")
+    #     return data
 
 
 class NestedField(RootModel):
     type: Literal["object", "array"]
     fields: Union[Dict[str, 'Field'], 'NestedField']
 
-    @model_validator(mode="before")
-    def validate_fields(self, data):
-        type_t = data.get("type")
-        fields = data.get("fields")
-
-        if type_t == "object":
-            if not isinstance(fields, dict):
-                raise ValueError("fields must be a dictionary when type is 'object'")
-        elif type_t == "array":
-            if not isinstance(fields, NestedField):
-                raise ValueError("fields must be a NestedField instance when type is 'array'")
-        else:
-            raise ValueError(f"Invalid type value: {type_t}")
-        return data
+    # @model_validator(mode="before")
+    # def validate_fields(self, data):
+    #     type_t = data.get("type")
+    #     fields = data.get("fields")
+    #
+    #     if type_t == "object":
+    #         if not isinstance(fields, dict):
+    #             raise ValueError("fields must be a dictionary when type is 'object'")
+    #     elif type_t == "array":
+    #         if not isinstance(fields, NestedField):
+    #             raise ValueError("fields must be a NestedField instance when type is 'array'")
+    #     else:
+    #         raise ValueError(f"Invalid type value: {type_t}")
+    #     return data
 
 
 class Field(RootModel):
     type: Literal["column", "relationship"]
     column: Optional[str] = None
     fields: Optional['NestedField'] = None
     query: Optional['Query'] = None
     relationship: Optional[str] = None
     arguments: Optional[Dict[str, 'RelationshipArgument']] = None
 
-    @model_validator(mode="before")
-    def validate_fields(self, data):
-        type_t = data.get('type')
-        column = data.get('column')
-        fields = data.get('fields')
-        query = data.get('query')
-        relationship = data.get('relationship')
-        arguments = data.get('arguments')
-
-        if type_t == "column":
-            if not column:
-                raise ValueError("column is required when type is 'column'")
-            if any([query, relationship, arguments]):
-                raise ValueError("Only 'column' and 'fields' should be set when type is 'column'")
-        elif type_t == "relationship":
-            if not query or not relationship or not arguments:
-                raise ValueError("query, relationship, and arguments are required when type is 'relationship'")
-            if column is not None or fields is not None:
-                raise ValueError("column and fields should not be set when type is 'relationship'")
-        else:
-            raise ValueError(f"Invalid type value: {type_t}")
-        return data
+    # @model_validator(mode="before")
+    # def validate_fields(self, data):
+    #     type_t = data.get('type')
+    #     column = data.get('column')
+    #     fields = data.get('fields')
+    #     query = data.get('query')
+    #     relationship = data.get('relationship')
+    #     arguments = data.get('arguments')
+    #
+    #     if type_t == "column":
+    #         if not column:
+    #             raise ValueError("column is required when type is 'column'")
+    #         if any([query, relationship, arguments]):
+    #             raise ValueError("Only 'column' and 'fields' should be set when type is 'column'")
+    #     elif type_t == "relationship":
+    #         if not query or not relationship or not arguments:
+    #             raise ValueError("query, relationship, and arguments are required when type is 'relationship'")
+    #         if column is not None or fields is not None:
+    #             raise ValueError("column and fields should not be set when type is 'relationship'")
+    #     else:
+    #         raise ValueError(f"Invalid type value: {type_t}")
+    #     return data
 
 
 class ExistsInCollection(RootModel):
     type: Literal["related", "unrelated"]
     relationship: Optional[str] = None
     collection: Optional[str] = None
     arguments: Dict[str, 'RelationshipArgument']
 
-    @model_validator(mode="before")
-    def validate_fields(self, data):
-        type_t = data.get("type")
-        relationship = data.get("relationship")
-        collection = data.get("collection")
-        arguments = data.get("arguments")
-
-        if type_t == "related":
-            if not relationship:
-                raise ValueError("relationship is required when type is 'related'")
-            if collection is not None:
-                raise ValueError("collection should not be set when type is 'related'")
-        elif type_t == "unrelated":
-            if not collection:
-                raise ValueError("collection is required when type is 'unrelated'")
-            if relationship is not None:
-                raise ValueError("relationship should not be set when type is 'unrelated'")
-        else:
-            raise ValueError(f"Invalid type value: {type_t}")
-
-        if not arguments:
-            raise ValueError("arguments must not be empty")
-        return data
+    # @model_validator(mode="before")
+    # def validate_fields(self, data):
+    #     type_t = data.get("type")
+    #     relationship = data.get("relationship")
+    #     collection = data.get("collection")
+    #     arguments = data.get("arguments")
+    #
+    #     if type_t == "related":
+    #         if not relationship:
+    #             raise ValueError("relationship is required when type is 'related'")
+    #         if collection is not None:
+    #             raise ValueError("collection should not be set when type is 'related'")
+    #     elif type_t == "unrelated":
+    #         if not collection:
+    #             raise ValueError("collection is required when type is 'unrelated'")
+    #         if relationship is not None:
+    #             raise ValueError("relationship should not be set when type is 'unrelated'")
+    #     else:
+    #         raise ValueError(f"Invalid type value: {type_t}")
+    #
+    #     if not arguments:
+    #         raise ValueError("arguments must not be empty")
+    #     return data
 
 
 RelationshipType = Literal["object", "array"]
 
 
 class RowSet(RootModel):
     aggregates: Optional[Dict[str, Any]] = None
@@ -507,31 +507,31 @@
     one_of: Optional[List[str]] = None
 
 
 class ComparisonOperatorDefinition(RootModel):
     type: Literal["equal", "in", "custom"]
     argument_type: Optional['Type'] = None
 
-    @model_validator(mode="before")
-    def validate_fields(self, data):
-        type_t = data.get("type")
-        argument_type = data.get("argument_type")
-
-        if type_t == "equal":
-            if argument_type is not None:
-                raise ValueError("argument_type should not be set when type is 'equal'")
-        elif type_t == "in":
-            if argument_type is not None:
-                raise ValueError("argument_type should not be set when type is 'equal'")
-        elif type_t == "custom":
-            if argument_type is None:
-                raise ValueError("argument_type should be set when type is 'custom'")
-        else:
-            raise ValueError(f"Invalid type value: {type_t}")
-        return data
+    # @model_validator(mode="before")
+    # def validate_fields(self, data):
+    #     type_t = data.get("type")
+    #     argument_type = data.get("argument_type")
+    #
+    #     if type_t == "equal":
+    #         if argument_type is not None:
+    #             raise ValueError("argument_type should not be set when type is 'equal'")
+    #     elif type_t == "in":
+    #         if argument_type is not None:
+    #             raise ValueError("argument_type should not be set when type is 'equal'")
+    #     elif type_t == "custom":
+    #         if argument_type is None:
+    #             raise ValueError("argument_type should be set when type is 'custom'")
+    #     else:
+    #         raise ValueError(f"Invalid type value: {type_t}")
+    #     return data
 
 
 class ScalarType(RootModel):
     representation: Optional['TypeRepresentation'] = None
     aggregate_functions: Dict[str, 'AggregateFunctionDefinition']
     comparison_operators: Dict[str, 'ComparisonOperatorDefinition']
```

### Comparing `hasura_ndc-0.8/hasura_ndc/server.py` & `hasura_ndc-0.9/hasura_ndc/server.py`

 * *Files identical despite different names*

### Comparing `hasura_ndc-0.8/hasura_ndc.egg-info/PKG-INFO` & `hasura_ndc-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hasura-ndc
-Version: 0.8
+Name: hasura_ndc
+Version: 0.9
 Summary: A Hasura Data Connector SDK
 Author: Tristen Harr
 Author-email: tristen.harr@hasura.io
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `hasura_ndc-0.8/hasura_ndc.egg-info/requires.txt` & `hasura_ndc-0.9/hasura_ndc.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hasura_ndc-0.8/setup.py` & `hasura_ndc-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='hasura_ndc',
-    version='0.08',
+    version='0.09',
     packages=find_packages(),
     install_requires=[
         # This line reads the requirements from your `requirements.txt`
         line.strip() for line in open('requirements.txt', 'r').readlines()
     ],
     author='Tristen Harr',
     author_email='tristen.harr@hasura.io',
```

