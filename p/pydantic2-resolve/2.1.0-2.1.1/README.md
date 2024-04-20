# Comparing `tmp/pydantic2_resolve-2.1.0.tar.gz` & `tmp/pydantic2_resolve-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic2_resolve-2.1.0.tar", max compression
+gzip compressed data, was "pydantic2_resolve-2.1.1.tar", max compression
```

## Comparing `pydantic2_resolve-2.1.0.tar` & `pydantic2_resolve-2.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-11-01 02:38:24.970361 pydantic2_resolve-2.1.0/LICENSE
--rw-r--r--   0        0        0     3914 2024-04-08 13:13:13.052286 pydantic2_resolve-2.1.0/README.md
--rw-r--r--   0        0        0      815 2024-04-08 12:50:08.904200 pydantic2_resolve-2.1.0/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0      425 2024-04-08 12:50:08.904487 pydantic2_resolve-2.1.0/pydantic_resolve/constant.py
--rw-r--r--   0        0        0    14051 2024-04-08 12:50:08.904882 pydantic2_resolve-2.1.0/pydantic_resolve/core.py
--rw-r--r--   0        0        0      280 2024-02-29 13:58:11.436236 pydantic2_resolve-2.1.0/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0     9366 2024-04-08 12:51:17.738611 pydantic2_resolve-2.1.0/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0    13455 2024-04-08 12:55:52.837311 pydantic2_resolve-2.1.0/pydantic_resolve/util.py
--rw-r--r--   0        0        0      826 2024-04-08 13:14:11.402036 pydantic2_resolve-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     4746 1970-01-01 00:00:00.000000 pydantic2_resolve-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-11-01 02:38:24.970361 pydantic2_resolve-2.1.1/LICENSE
+-rw-r--r--   0        0        0     3912 2024-04-08 14:46:31.661342 pydantic2_resolve-2.1.1/README.md
+-rw-r--r--   0        0        0      815 2024-04-08 12:50:08.904200 pydantic2_resolve-2.1.1/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0      425 2024-04-08 12:50:08.904487 pydantic2_resolve-2.1.1/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0    14354 2024-04-20 14:57:07.306453 pydantic2_resolve-2.1.1/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      280 2024-02-29 13:58:11.436236 pydantic2_resolve-2.1.1/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0    10039 2024-04-20 15:03:05.631058 pydantic2_resolve-2.1.1/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0    13455 2024-04-08 12:55:52.837311 pydantic2_resolve-2.1.1/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      826 2024-04-20 15:04:40.730494 pydantic2_resolve-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4744 1970-01-01 00:00:00.000000 pydantic2_resolve-2.1.1/PKG-INFO
```

### Comparing `pydantic2_resolve-2.1.0/LICENSE` & `pydantic2_resolve-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic2_resolve-2.1.0/README.md` & `pydantic2_resolve-2.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 1. use declaretive way to define view data, easy to maintain and develop
 2. enhance the traditional restful response, to support gql-like style data structure.
 3. provide post_method and other tools to craft resolved data.
 
 
 [Discord](https://discord.com/channels/1197929379951558797/1197929379951558800)
 
+
 ## Install
 
 > If you are using pydantic v1, please use [pydantic-resolve](https://github.com/allmonday/pydantic-resolve) instead.
 
 
 ```shell
 pip install pydantic-resolve
@@ -43,15 +44,15 @@
                 content
             }
             # comment_count
         }
         # comment_count
     }
 }
-```
+
 
 This is how we do queries in GraphQL, dive by describing schema and field names.
 
 Assuming `comment_count` is a extra field (length of comment), which is required and calculated by client after fetching the data.
 
 client side so need to iterate over the blogs to get the length and the sum, which is boring (things gets worse if the structure is deeper).
```

### Comparing `pydantic2_resolve-2.1.0/pydantic_resolve/__init__.py` & `pydantic2_resolve-2.1.1/pydantic_resolve/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic2_resolve-2.1.0/pydantic_resolve/core.py` & `pydantic2_resolve-2.1.1/pydantic_resolve/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,25 +76,29 @@
         return target.__class__
 
 
 def _scan_resolve_method(method, field: str):
     result = {
         'trim_field': field.replace(const.RESOLVE_PREFIX, ''),
         'context': False,
+        'parent': False,
         'ancestor_context': False,
         'dataloaders': []  # collect func or class, do not create instance
     }
     signature = inspect.signature(method)
 
     if signature.parameters.get('context'):
         result['context'] = True
 
     if signature.parameters.get('ancestor_context'):
         result['ancestor_context'] = True
 
+    if signature.parameters.get('parent'):
+        result['parent'] = True
+
     for name, param in signature.parameters.items():
         if isinstance(param.default, Depends):
             info = { 
                 'param': name,
                 'kls': param.default.dependency,  # for later initialization
                 'path': util.get_kls_full_path(param.default.dependency) }
             result['dataloaders'].append(info)
@@ -106,24 +110,28 @@
     return result
 
 
 def _scan_post_method(method, field):
     result = {
         'trim_field': field.replace(const.POST_PREFIX, ''),
         'context': False,
+        'parent': False,
         'ancestor_context': False,
         'collectors': []
     }
     signature = inspect.signature(method)
 
     if signature.parameters.get('context'):
         result['context'] = True
 
     if signature.parameters.get('ancestor_context'):
         result['ancestor_context'] = True
+
+    if signature.parameters.get('parent'):
+        result['parent'] = True
     
     for name, param in signature.parameters.items():
         if isinstance(param.default, ICollector):
             info = {
                 'field': field,
                 'param': name,
                 'instance': param.default,
@@ -132,24 +140,28 @@
             
     return result
 
 
 def _scan_post_default_handler(method):
     result = {
         'context': False,
+        'parent': False,
         'ancestor_context': False,
     }
     signature = inspect.signature(method)
 
     if signature.parameters.get('context'):
         result['context'] = True
 
     if signature.parameters.get('ancestor_context'):
         result['ancestor_context'] = True
 
+    if signature.parameters.get('parent'):
+        result['parent'] = True
+
     return result
 
 
 def validate_and_create_loader_instance(
         loader_params,
         global_loader_param,
         loader_instances,
```

### Comparing `pydantic2_resolve-2.1.0/pydantic_resolve/resolver.py` & `pydantic2_resolve-2.1.1/pydantic_resolve/resolver.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,14 +24,15 @@
             loader_instances: Optional[Dict[Any, Any]] = None,
             ensure_type=False,
             context: Optional[Dict[str, Any]] = None):
         self.loader_instance_cache = {}
 
         self.ancestor_vars = {}
         self.collector_contextvars = {}
+        self.parent_contextvars = {}
 
         # for dataloader which has class attributes, you can assign the value at here
         if loader_filters:
             warnings.warn('loader_filters is deprecated, use loader_params instead.', DeprecationWarning)
             self.loader_params = loader_filters
         else:
             self.loader_params = loader_params or {}
@@ -79,14 +80,19 @@
     def _add_values_into_collectors(self, target, kls):
         for field, alias in core.iter_over_collectable_fields(kls, self.metadata):
             for _, instance in self.collector_contextvars[alias].get().items():
                 collector = instance
                 val = getattr(target, field)
                 collector.add(val)
 
+    def _add_parent(self, target):
+        if not self.parent_contextvars.get('parent'):
+            self.parent_contextvars['parent'] = contextvars.ContextVar('parent')
+        self.parent_contextvars['parent'].set(target)
+
     def _add_expose_fields(self, target):
         expose_dict: Optional[dict] = getattr(target, const.EXPOSE_TO_DESCENDANT, None)
         if expose_dict:
             for field, alias in expose_dict.items():  # eg: {'name': 'bar_name'}
                 if not self.ancestor_vars.get(alias):
                     self.ancestor_vars[alias] = contextvars.ContextVar(alias)
 
@@ -103,49 +109,53 @@
     def _execute_resolver_method(self, kls, field, method):
         params = {}
         resolve_param = core.get_resolve_param(kls, field, self.metadata)
         if resolve_param['context']:
             params['context'] = self.context
         if resolve_param['ancestor_context']:
             params['ancestor_context'] = self._prepare_ancestor_context()
+        if resolve_param['parent']:
+            params['parent'] = self.parent_contextvars['parent'].get()
         
         for loader in resolve_param['dataloaders']:
             cache_key = loader['path']
             loader_instance = self.loader_instance_cache[cache_key]
             params[loader['param']] = loader_instance
 
         return method(**params)
     
     def _execute_post_method(self, target, kls, kls_path, post_field, method):
         params = {}
         post_param = core.get_post_params(kls, post_field , self.metadata)
         if post_param['context']:
             params['context'] = self.context
-
         if post_param['ancestor_context']:
             params['ancestor_context'] = self._prepare_ancestor_context()
+        if post_param['parent']:
+            params['parent'] = self.parent_contextvars['parent'].get()
 
         alias_map = self.object_collect_alias_map_store.get(id(target), {})
         if alias_map:
             for collector in post_param['collectors']:
                 alias, param = collector['alias'], collector['param']
                 signature = (kls_path, post_field, param)
                 params[param] = alias_map[alias][signature]
         
         return method(**params)
 
     def _execute_post_default_handler(self, kls, method):
         params = {}
-        resolve_param = core.get_post_default_handler_params(kls, self.metadata)
+        post_default_param = core.get_post_default_handler_params(kls, self.metadata)
 
-        if resolve_param['context']:
+        if post_default_param['context']:
             params['context'] = self.context
-
-        if resolve_param['ancestor_context']:
+        if post_default_param['ancestor_context']:
             params['ancestor_context'] = self._prepare_ancestor_context()
+        if post_default_param['parent']:
+            params['parent'] = self.parent_contextvars['parent'].get()
 
         ret_val = method(**params)
         return ret_val
 
     async def _resolve_obj_field(self, target, kls, field, trim_field, method):
         if self.ensure_type:
             if not method.__annotations__:
@@ -155,37 +165,38 @@
         while iscoroutine(val) or asyncio.isfuture(val):
             val = await val
 
         if not getattr(method, const.HAS_MAPPER_FUNCTION, False):  # defined in util.mapper
             val = util.try_parse_data_to_target_field_type(target, trim_field, val)
 
         # continue dive deeper
-        val = await self._resolve(val)
+        val = await self._resolve(val, target)
 
         setattr(target, trim_field, val)
 
-    async def _resolve(self, target: T) -> T:
+    async def _resolve(self, target: T, parent) -> T:
         if isinstance(target, (list, tuple)):
-            await asyncio.gather(*[self._resolve(t) for t in target])
+            await asyncio.gather(*[self._resolve(t, parent) for t in target])
 
         if core.is_acceptable_instance(target):
             kls = target.__class__
             kls_path = util.get_kls_full_path(kls)
 
             self._prepare_collectors(target, kls)
             self._add_expose_fields(target)
+            self._add_parent(parent)
 
             tasks = []
 
             # traversal and fetching data by resolve methods
             resolve_list, attribute_list = core.iter_over_object_resolvers_and_acceptable_fields(target, kls, self.metadata)
             for field, resolve_trim_field, method in resolve_list:
                 tasks.append(self._resolve_obj_field(target, kls, field, resolve_trim_field, method))
             for field, attr_object in attribute_list:
-                tasks.append(self._resolve(attr_object))
+                tasks.append(self._resolve(attr_object, target))
             await asyncio.gather(*tasks)
 
             # reverse traversal and run post methods
             for post_field, post_trim_field in core.iter_over_object_post_methods(kls, self.metadata):
                 post_method = getattr(target, post_field)
                 result = self._execute_post_method(target, kls, kls_path, post_field, post_method)
                 result = util.try_parse_data_to_target_field_type(target, post_trim_field, result)
@@ -213,9 +224,9 @@
             self.loader_instances,
             self.metadata)
         
         has_context = core.has_context(self.metadata)
         if has_context and self.context is None:
             raise AttributeError('context is missing')
             
-        await self._resolve(target)
+        await self._resolve(target, None)
         return target
```

### Comparing `pydantic2_resolve-2.1.0/pydantic_resolve/util.py` & `pydantic2_resolve-2.1.1/pydantic_resolve/util.py`

 * *Files identical despite different names*

### Comparing `pydantic2_resolve-2.1.0/pyproject.toml` & `pydantic2_resolve-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic2-resolve"
-version = "2.1.0"
+version = "2.1.1"
 description = "create nested data structure easily"
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic2_resolve"
 keywords = ["pydantic2", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
```

### Comparing `pydantic2_resolve-2.1.0/PKG-INFO` & `pydantic2_resolve-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic2-resolve
-Version: 2.1.0
+Version: 2.1.1
 Summary: create nested data structure easily
 Home-page: https://github.com/allmonday/pydantic2_resolve
 License: MIT
 Keywords: pydantic2,fastapi
 Author: tangkikodo
 Author-email: allmonday@126.com
 Requires-Python: >=3.7,<4.0
@@ -38,14 +38,15 @@
 1. use declaretive way to define view data, easy to maintain and develop
 2. enhance the traditional restful response, to support gql-like style data structure.
 3. provide post_method and other tools to craft resolved data.
 
 
 [Discord](https://discord.com/channels/1197929379951558797/1197929379951558800)
 
+
 ## Install
 
 > If you are using pydantic v1, please use [pydantic-resolve](https://github.com/allmonday/pydantic-resolve) instead.
 
 
 ```shell
 pip install pydantic-resolve
@@ -65,15 +66,15 @@
                 content
             }
             # comment_count
         }
         # comment_count
     }
 }
-```
+
 
 This is how we do queries in GraphQL, dive by describing schema and field names.
 
 Assuming `comment_count` is a extra field (length of comment), which is required and calculated by client after fetching the data.
 
 client side so need to iterate over the blogs to get the length and the sum, which is boring (things gets worse if the structure is deeper).
```

