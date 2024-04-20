# Comparing `tmp/weedata-0.2.3.tar.gz` & `tmp/weedata-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weedata-0.2.3.tar", last modified: Sat Apr 13 16:03:22 2024, max compression
+gzip compressed data, was "weedata-0.2.4.tar", last modified: Fri Apr 19 13:11:04 2024, max compression
```

## Comparing `weedata-0.2.3.tar` & `weedata-0.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 16:03:22.374601 weedata-0.2.3/
--rw-rw-rw-   0        0        0     1084 2024-02-06 11:15:24.000000 weedata-0.2.3/LICENSE
--rw-rw-rw-   0        0        0    19037 2024-04-13 16:03:22.368601 weedata-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    16059 2024-04-13 16:00:55.000000 weedata-0.2.3/README.md
--rw-rw-rw-   0        0        0     1417 2024-04-13 16:01:14.000000 weedata-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-13 16:03:22.375601 weedata-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-13 16:03:21.416551 weedata-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-13 16:03:21.495567 weedata-0.2.3/src/weedata/
--rw-rw-rw-   0        0        0      497 2024-04-13 16:01:26.000000 weedata-0.2.3/src/weedata/__init__.py
--rw-rw-rw-   0        0        0    31685 2024-03-25 21:24:11.000000 weedata-0.2.3/src/weedata/client.py
--rw-rw-rw-   0        0        0    15500 2024-04-13 15:58:34.000000 weedata-0.2.3/src/weedata/fields.py
--rw-rw-rw-   0        0        0     9591 2024-03-09 14:46:27.000000 weedata-0.2.3/src/weedata/model.py
--rw-rw-rw-   0        0        0     8012 2024-02-27 13:14:36.000000 weedata-0.2.3/src/weedata/queries.py
-drwxrwxrwx   0        0        0        0 2024-04-13 16:03:22.359601 weedata-0.2.3/src/weedata.egg-info/
--rw-rw-rw-   0        0        0    19037 2024-04-13 16:03:21.000000 weedata-0.2.3/src/weedata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2024-04-13 16:03:21.000000 weedata-0.2.3/src/weedata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 16:03:21.000000 weedata-0.2.3/src/weedata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-13 16:03:21.000000 weedata-0.2.3/src/weedata.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-13 16:03:22.116601 weedata-0.2.3/tests/
--rw-rw-rw-   0        0        0     4294 2024-03-16 22:05:45.000000 weedata-0.2.3/tests/test_base.py
--rw-rw-rw-   0        0        0     3366 2024-02-24 09:33:45.000000 weedata-0.2.3/tests/test_connection.py
--rw-rw-rw-   0        0        0     3085 2024-02-25 15:24:02.000000 weedata-0.2.3/tests/test_delete.py
--rw-rw-rw-   0        0        0     9765 2024-02-25 23:41:43.000000 weedata-0.2.3/tests/test_fields.py
--rw-rw-rw-   0        0        0     9033 2024-02-26 00:16:26.000000 weedata-0.2.3/tests/test_queries.py
--rw-rw-rw-   0        0        0     1017 2024-02-24 09:34:08.000000 weedata-0.2.3/tests/test_save.py
--rw-rw-rw-   0        0        0     5398 2024-02-25 17:34:27.000000 weedata-0.2.3/tests/test_update.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.329059 weedata-0.2.4/
+-rw-rw-rw-   0        0        0     1084 2024-02-06 11:15:24.000000 weedata-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0    19142 2024-04-19 13:11:04.325058 weedata-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    16160 2024-04-19 13:09:41.000000 weedata-0.2.4/README.md
+-rw-rw-rw-   0        0        0     1417 2024-04-19 13:09:58.000000 weedata-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-19 13:11:04.330059 weedata-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.214048 weedata-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.265048 weedata-0.2.4/src/weedata/
+-rw-rw-rw-   0        0        0      497 2024-04-19 13:07:05.000000 weedata-0.2.4/src/weedata/__init__.py
+-rw-rw-rw-   0        0        0    32289 2024-04-19 13:07:40.000000 weedata-0.2.4/src/weedata/client.py
+-rw-rw-rw-   0        0        0    15500 2024-04-13 15:58:34.000000 weedata-0.2.4/src/weedata/fields.py
+-rw-rw-rw-   0        0        0     9844 2024-04-19 13:05:58.000000 weedata-0.2.4/src/weedata/model.py
+-rw-rw-rw-   0        0        0     8132 2024-04-19 12:41:56.000000 weedata-0.2.4/src/weedata/queries.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.322058 weedata-0.2.4/src/weedata.egg-info/
+-rw-rw-rw-   0        0        0    19142 2024-04-19 13:11:04.000000 weedata-0.2.4/src/weedata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2024-04-19 13:11:04.000000 weedata-0.2.4/src/weedata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 13:11:04.000000 weedata-0.2.4/src/weedata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-19 13:11:04.000000 weedata-0.2.4/src/weedata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.317057 weedata-0.2.4/tests/
+-rw-rw-rw-   0        0        0     4294 2024-03-16 22:05:45.000000 weedata-0.2.4/tests/test_base.py
+-rw-rw-rw-   0        0        0     3366 2024-02-24 09:33:45.000000 weedata-0.2.4/tests/test_connection.py
+-rw-rw-rw-   0        0        0     3085 2024-02-25 15:24:02.000000 weedata-0.2.4/tests/test_delete.py
+-rw-rw-rw-   0        0        0     9765 2024-02-25 23:41:43.000000 weedata-0.2.4/tests/test_fields.py
+-rw-rw-rw-   0        0        0     9033 2024-02-26 00:16:26.000000 weedata-0.2.4/tests/test_queries.py
+-rw-rw-rw-   0        0        0     1017 2024-02-24 09:34:08.000000 weedata-0.2.4/tests/test_save.py
+-rw-rw-rw-   0        0        0     5398 2024-02-25 17:34:27.000000 weedata-0.2.4/tests/test_update.py
```

### Comparing `weedata-0.2.3/LICENSE` & `weedata-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `weedata-0.2.3/PKG-INFO` & `weedata-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weedata
-Version: 0.2.3
+Version: 0.2.4
 Summary: an ORM/ODM for Google Cloud Datastore/MongoDB/redis, featuring a compatible interface with Peewee.
 Author-email: cdhigh <akindleear@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 cdhigh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -479,14 +479,18 @@
 User.replace(name='python', score=100, birthdate=datetime.datetime(2024,1,1)).execute()
 
 ```
 
 
 # Changelog  
 
+* v0.2.4
+1. Optimize the modification logic for JSONField, saving to the database at any time.    
+
+
 * v0.2.3
 1. bugfix: TextField/BlobField/JSONField initial params not worked.   
 
 
 * v0.2.2
 1. Delays connecting to the pymongo database until the first operation.   
 2. The default Index property of TextField/BlobField/JSONField is set to False.
```

### Comparing `weedata-0.2.3/README.md` & `weedata-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -429,14 +429,18 @@
 User.replace(name='python', score=100, birthdate=datetime.datetime(2024,1,1)).execute()
 
 ```
 
 
 # Changelog  
 
+* v0.2.4
+1. Optimize the modification logic for JSONField, saving to the database at any time.    
+
+
 * v0.2.3
 1. bugfix: TextField/BlobField/JSONField initial params not worked.   
 
 
 * v0.2.2
 1. Delays connecting to the pymongo database until the first operation.   
 2. The default Index property of TextField/BlobField/JSONField is set to False.
```

### Comparing `weedata-0.2.3/pyproject.toml` & `weedata-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "weedata"
-version = "0.2.3"
+version = "0.2.4"
 description = "an ORM/ODM for Google Cloud Datastore/MongoDB/redis, featuring a compatible interface with Peewee."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.6"
 keywords = ["peewee", "ORM", "ODM", "google cloud datastore", "MongoDB", "redis"]
 dependencies = [
 #  "google-cloud-datastore",
```

### Comparing `weedata-0.2.3/src/weedata/client.py` & `weedata-0.2.4/src/weedata/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 #An ORM/ODM for Google Cloud Datastore/MongoDB/redis, featuring a compatible interface with Peewee.
 #Author: cdhigh <http://github.com/cdhigh>
 #Repository: <https://github.com/cdhigh/weedata>
 #Pypi package: <https://pypi.org/project/weedata>
-import os, sys, uuid, pickle, shutil
+import os, sys, uuid, pickle, shutil, logging
 from itertools import chain
 from operator import attrgetter
 from collections import defaultdict
 from urllib.parse import urlparse, parse_qs
 
 try:
     from google.cloud import datastore
     from google.cloud.datastore import Key
     from google.cloud.datastore import query as qr
-except ImportError:  # pragma: no cover
+except:  # pragma: no cover
     datastore = None
 
 try:
     import pymongo
     from bson.objectid import ObjectId
-except ImportError:  # pragma: no cover
+except:  # pragma: no cover
     pymongo = None
 
 try:
     import redis
-except ImportError:  # pragma: no cover
+except:  # pragma: no cover
     redis = None
 
 from .model import Model, BaseModel
 from .fields import Filter
 
 #if os.environ.get('WEEDATA_TEST_BACKEND') == 'datastore':
 #    from fake_datastore import *
 #    print('Alert: using fake datastore stub!!!')
 
 class NosqlClient(object):
     bytes_store = False #For redis, it's True
+    def __init__(self, *args, **kwargs):
+        self.log = logging.getLogger('weedata')
 
     def bind(self, models):
         for model in models:
             model.bind(self)
     def drop_tables(self, models, **kwargs):
         for model in models:
             self.drop_table(model)
@@ -63,14 +65,15 @@
         return fakeTransation()
     @classmethod
     def op_map(cls, op):
         return op
     
 class DatastoreClient(NosqlClient):
     def __init__(self, project=None, namespace=None, credentials=None, _http=None):
+        super().__init__()
         self.project = project or os.getenv("GOOGLE_CLOUD_PROJECT", None)
         self.credentials = credentials
         self.namespace = namespace
         self._http = _http
         self.client = datastore.Client(project=self.project, namespace=self.namespace, 
             credentials=self.credentials, _http=self._http)
     
@@ -122,23 +125,23 @@
         keys = [e._key for e in models if e._key]
         if keys:
             self.client.delete_multi(keys)
             return len(keys)
         else:
             return 0
 
-    def execute(self, queryObj, page_size=500, parent_key=None, limit=None):
+    def execute(self, queryObj, page_size=500, parent_key=None, limit=None, as_dict=False):
         klass = queryObj.model_class
         kind = klass._meta.name
         query = self.client.query(kind=kind, ancestor=parent_key)
         self.apply_query_condition(queryObj, query)
 
         limit = limit if limit else queryObj._limit
         batch_size = min(page_size, limit) if limit else page_size
-        yield from self.query_fetch(query, batch_size, limit, klass)
+        yield from self.query_fetch(query, batch_size, limit, klass, as_dict)
 
     #count aggregation query
     def count(self, queryObj, parent_key=None):
         return self.aggre_execute(queryObj, parent_key, 'count')
         
     #sum aggregation query
     def sum(self, queryObj, field, parent_key=None):  # pragma: no cover
@@ -159,24 +162,24 @@
         self.apply_query_condition(queryObj, query)
         query_func = getattr(self.client.aggregation_query(query=query), func)
         query = query_func(arg) if arg else query_func()
         with query.fetch() as result:
             return next(result).value if result else 0
 
     #generate model instance(klass!=None) or entity(klass=None)
-    def query_fetch(self, query, batch_size=500, limit=0, klass=None):
+    def query_fetch(self, query, batch_size=500, limit=0, klass=None, as_dict=False):
         cursor = None
         count = 0
         while True:
             last_entity = None
             result = query.fetch(start_cursor=cursor, limit=batch_size)
 
             for entity in result:
                 last_entity = self.make_instance(klass, entity) if klass else entity
-                yield last_entity
+                yield last_entity.dicts() if (last_entity and as_dict) else last_entity
                 count += 1
             cursor = result.next_page_token
             if not cursor or (last_entity is None) or (limit and (count >= limit)):
                 break
 
     #make Model instance from database data
     def make_instance(self, klass, raw):
@@ -288,14 +291,15 @@
             self.client.delete_multi(keys)
 
     def close(self):
         self.client.close()
 
 class MongoDbClient(NosqlClient):
     def __init__(self, project, dbUrl='mongodb://127.0.0.1:27017/'):
+        super().__init__()
         self.project = project
         self.dbUrl = dbUrl
         self.client = pymongo.MongoClient(self.dbUrl, connect=False)
         self._db = self.client[project]
     
     @classmethod
     def db_id_name(cls):
@@ -330,15 +334,15 @@
             return self._db[model._meta.name].delete_one({'_id': model._id}).deleted_count
         else:
             return 0
 
     def delete_many(self, models):
         return sum([self.delete_one(model) for model in models])
         
-    def execute(self, queryObj, page_size=500, parent_key=None, limit=None):
+    def execute(self, queryObj, page_size=500, parent_key=None, limit=None, as_dict=False):
         klass = queryObj.model_class
         collection = self._db[klass._meta.name]
         sort = [(item[1:], pymongo.DESCENDING) if item.startswith('-') else (item, pymongo.ASCENDING) for item in queryObj._order]
         projection = self.build_projection(queryObj)
         limit = limit if limit else queryObj._limit
         if queryObj._distinct:
             for data in collection.distinct(queryObj._distinct[0], queryObj.filters()):
@@ -346,15 +350,16 @@
         else:
             with collection.find(queryObj.filters(), projection=projection) as cursor:
                 if sort:
                     cursor = cursor.sort(sort)
                 if limit:
                     cursor = cursor.limit(limit)
                 for item in cursor:
-                    yield self.make_instance(klass, item)
+                    inst = self.make_instance(klass, item)
+                    yield inst.dicts() if (inst and as_dict) else inst
 
     def count(self, queryObj, parent_key=None):
         return self._db[queryObj.model_class._meta.name].count_documents(queryObj.filters())
 
     #make Model instance from database data
     def make_instance(self, klass, raw):
         inst = klass()
@@ -401,14 +406,15 @@
 
 
 class RedisDbClient(NosqlClient):
     bytes_store = True
     urlsafe_alphabet = '0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz'
 
     def __init__(self, project, dbUrl='redis://127.0.0.1:6379/0', key_sep=':'):
+        super().__init__()
         self.redis = redis.from_url(dbUrl)
         self.prefix = f'{project}{key_sep}'
         self.key_sep = key_sep
         self.indexes = defaultdict(set)
 
     @classmethod
     def op_map(cls, op):
@@ -488,24 +494,25 @@
             if cnt and self.indexes.get(model._meta.name, None): #delete index if exists
                 self.drop_index(model)
         return cnt
 
     def delete_many(self, models):
         return sum([self.delete_one(model) for model in models])
         
-    def execute(self, queryObj, page_size=500, parent_key=None, limit=None):
+    def execute(self, queryObj, page_size=500, parent_key=None, limit=None, as_dict=False):
         klass = queryObj.model_class
         _filters = queryObj._filters
         if len(_filters) == 1:
             flt = _filters[0]
             if flt.isFilterById(self.db_id_name()):
-                yield self.get_by_id(klass, flt.value)
+                inst = self.get_by_id(klass, flt.value)
+                yield inst.dicts() if (inst and as_dict) else inst
                 return
             elif self.indexes.get(klass._meta.name) and self.isFilterByIndex(klass, flt):
-                yield from self.get_by_index(klass, flt)
+                yield from self.get_by_index(klass, flt, as_dict)
                 return
             
         filters = [flt.clone('utf-8') for flt in _filters]
         fields = {name.encode('utf-8'): inst for name, inst in klass._meta.fields.items()}
         results = []
         key_sep = self.key_sep.encode('utf-8')
         id_name = self.db_id_name().encode('utf-8')
@@ -523,15 +530,16 @@
                 if not order and limit and cnt >= limit:
                     break
 
         results = [self.make_instance(klass, r) for r in results]
         if order:
             results.sort(key=attrgetter(*order), reverse=reverse)
 
-        yield from (results[:limit] if limit else results)
+        for inst in (results[:limit] if limit else results):
+            yield inst.dicts() if (inst and as_dict) else inst
 
     def isFilterByIndex(self, model, flt):
         return (not flt.bit_op and flt.op == Filter.EQ and flt.item in self.indexes.get(model._meta.name, []))
 
     #type_: key | index | key_data
     def iter_data(self, klass, type_='key'):
         cursor = 0
@@ -550,18 +558,19 @@
         data = self.redis.hgetall(self.build_key(klass, id_=id_))
         if data:
             data[self.db_id_name()] = id_
             return self.make_instance(klass, data)
         else:
             return None
 
-    def get_by_index(self, klass, flt):
+    def get_by_index(self, klass, flt, as_dict=False):
         key = self.build_key(klass, index=(flt.item, flt.value))
         for id_ in self.redis.smembers(key):
-            yield self.get_by_id(klass, id_)
+            inst = self.get_by_id(klass, id_)
+            yield inst.dicts() if (inst and as_dict) else inst
 
     def _matches_query(self, data: dict, flt: Filter, fields: dict):
         if not flt.bit_op:
             item = flt.item
             if item not in fields:
                 return False
 
@@ -652,14 +661,15 @@
         for key in self.iter_data(model, type_='key'):
             self.redis.delete(key)
 
 #use pickle instead of json for pickle can save bytes directly
 class PickleDbClient(RedisDbClient):
     #pickle://dbName?bakBeforeWrite=yes
     def __init__(self, dbName, bakBeforeWrite=True):
+        NosqlClient.__init__(self)
         if '://' in dbName:
             ret = urlparse(dbName)
             dbName = ret.netloc or ret.path
             _plat = sys.platform.lower()
             if ('win32' in _plat or 'win64' in _plat): #windows平台
                 dbName = dbName.lstrip('/')
             elif dbName.startswith('//'):
```

### Comparing `weedata-0.2.3/src/weedata/fields.py` & `weedata-0.2.4/src/weedata/fields.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.3/src/weedata/model.py` & `weedata-0.2.4/src/weedata/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 #An ORM/ODM for Google Cloud Datastore/MongoDB/redis, featuring a compatible interface with Peewee.
 #Author: cdhigh <http://github.com/cdhigh>
 #Repository: <https://github.com/cdhigh/weedata>
 #Pypi package: <https://pypi.org/project/weedata>
 import copy
-from .fields import Field, FieldDescriptor, PrimaryKeyField, ForeignKeyField, DoesNotExist, Filter
+from .fields import (Field, FieldDescriptor, PrimaryKeyField, ForeignKeyField, DoesNotExist, 
+        Filter, JSONField)
 from .queries import (QueryBuilder, DeleteQueryBuilder, InsertQueryBuilder, UpdateQueryBuilder,
     ReplaceQueryBuilder)
 
 class BaseModel(type):
     inheritable_options = ['client', 'order_by', 'primary_key']
 
     def __new__(cls, name, bases, attrs):
@@ -184,35 +185,38 @@
 
     #Convert model into a dict
     #: params only=[Model.title, ...]
     #: params exclude=[Model.title, ...]
     #: remove_id - remove key and id field from dict
     #: db_value - if prepared for saving to db
     #: only_dirty - export items unsaved only
-    def dicts(self, **kwargs):
-        only = [x.name for x in kwargs.get('only', [])]
-        exclude = [x.name for x in kwargs.get('exclude', [])]
+    def dicts(self, only=None, exclude=None, remove_id=False, db_value=False, only_dirty=False):
+        only = [(x if isinstance(x, str) else x.name) for x in (only or [])]
+        exclude = [(x if isinstance(x, str) else x.name) for x in (exclude or [])]
         should_skip = lambda n: (n in exclude) or (only and (n not in only))
-        db_value = kwargs.get('db_value', False)
-        only_dirty = kwargs.get('only_dirty', False)
-
+        
         data = {}
         for name, field in self._meta.fields.items():
-            if not should_skip(name) and (not only_dirty or self._dirty.get(name, False)):
+            if should_skip(name):
+                continue
+            
+            # JSONField is mutable and sometimes its changes cannot be determined
+            if not only_dirty or (self._dirty.get(name) or isinstance(field, JSONField)):
                 value = getattr(self, name, None)
                 if value and isinstance(field, ForeignKeyField) and isinstance(value, Model):
                     value = value.get_id()
                 if db_value:
                     value = field.db_value(value)
                 data[name] = value
 
-        if kwargs.get('remove_id'):
+        if remove_id:
             data.pop('_key', None)
             data.pop('id', None)
             data.pop('_id', None)
+        self.client.log.debug(self._meta.name + '.dicts: \n' + str(data))
         return data
 
     @classmethod
     def bind(cls, client):
         cls._meta.client = client
         for field in cls._meta.fields.values():
             field.bytes_store = client.bytes_store
```

### Comparing `weedata-0.2.3/src/weedata/queries.py` & `weedata-0.2.4/src/weedata/queries.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,18 @@
         distinct_field = field.name if isinstance(field, Field) else field
         self._distinct = [distinct_field]
         return self
 
     #the parameter limit will override the property of query object
     def execute(self, page_size=500, parent_key=None, limit=None):
         return self.client.execute(self, page_size=page_size, parent_key=parent_key, limit=limit)
-        
+    
+    def dicts(self):
+        return self.client.execute(self, page_size=page_size, parent_key=parent_key, as_dict=True)
+
     def get(self):
         result = None
         try:
             result = next(self.execute(page_size=1, limit=1))
         except (TypeError, StopIteration):
             pass
         return result
```

### Comparing `weedata-0.2.3/src/weedata.egg-info/PKG-INFO` & `weedata-0.2.4/src/weedata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weedata
-Version: 0.2.3
+Version: 0.2.4
 Summary: an ORM/ODM for Google Cloud Datastore/MongoDB/redis, featuring a compatible interface with Peewee.
 Author-email: cdhigh <akindleear@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 cdhigh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -479,14 +479,18 @@
 User.replace(name='python', score=100, birthdate=datetime.datetime(2024,1,1)).execute()
 
 ```
 
 
 # Changelog  
 
+* v0.2.4
+1. Optimize the modification logic for JSONField, saving to the database at any time.    
+
+
 * v0.2.3
 1. bugfix: TextField/BlobField/JSONField initial params not worked.   
 
 
 * v0.2.2
 1. Delays connecting to the pymongo database until the first operation.   
 2. The default Index property of TextField/BlobField/JSONField is set to False.
```

### Comparing `weedata-0.2.3/tests/test_base.py` & `weedata-0.2.4/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.3/tests/test_connection.py` & `weedata-0.2.4/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.3/tests/test_delete.py` & `weedata-0.2.4/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.3/tests/test_fields.py` & `weedata-0.2.4/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.3/tests/test_queries.py` & `weedata-0.2.4/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.3/tests/test_save.py` & `weedata-0.2.4/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.3/tests/test_update.py` & `weedata-0.2.4/tests/test_update.py`

 * *Files identical despite different names*

