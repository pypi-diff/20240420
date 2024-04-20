# Comparing `tmp/meritous-1.2.0.tar.gz` & `tmp/meritous-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meritous-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "meritous-1.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `meritous-1.2.0.tar` & `meritous-1.2.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0      159 2023-06-08 11:00:10.322398 meritous-1.2.0/.codeclimate.yml
--rw-r--r--   0        0        0     3078 2023-03-04 08:09:15.684878 meritous-1.2.0/.gitignore
--rw-r--r--   0        0        0       13 2023-02-23 13:38:24.154245 meritous-1.2.0/.python-version
--rw-r--r--   0        0        0     1077 2023-03-04 08:01:19.863201 meritous-1.2.0/LICENSE
--rw-r--r--   0        0        0     1704 2024-02-17 08:54:41.449491 meritous-1.2.0/README.md
--rw-r--r--   0        0        0      634 2023-06-02 05:33:09.164663 meritous-1.2.0/docs/Makefile
--rw-r--r--   0        0        0     1033 2023-06-02 07:09:12.763159 meritous-1.2.0/docs/concepts.rst
--rw-r--r--   0        0        0      522 2023-06-08 10:49:50.666394 meritous-1.2.0/docs/conf.py
--rw-r--r--   0        0        0      184 2023-06-02 07:28:36.492517 meritous-1.2.0/docs/extensions.rst
--rw-r--r--   0        0        0     1719 2023-06-02 07:28:54.564570 meritous-1.2.0/docs/index.rst
--rw-r--r--   0        0        0      800 2023-06-02 05:33:09.164663 meritous-1.2.0/docs/make.bat
--rw-r--r--   0        0        0     3441 2023-06-02 12:05:39.116053 meritous-1.2.0/docs/properties.rst
--rw-r--r--   0        0        0     1415 2024-02-17 08:08:25.739482 meritous-1.2.0/docs/start.rst
--rw-r--r--   0        0        0      180 2023-06-02 07:27:15.188275 meritous-1.2.0/docs/stores.rst
--rw-r--r--   0        0        0      173 2023-05-20 06:32:12.910513 meritous-1.2.0/noxfile.py
--rw-r--r--   0        0        0     1109 2024-03-06 21:27:24.241957 meritous-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      116 2024-03-06 21:48:02.943924 meritous-1.2.0/samples/event.json
--rw-r--r--   0        0        0      692 2024-03-06 06:36:03.154026 meritous-1.2.0/samples/event.py
--rw-r--r--   0        0        0      955 2024-03-06 21:44:38.122078 meritous-1.2.0/samples/serializers.py
--rw-r--r--   0        0        0      678 2024-03-06 22:01:48.520648 meritous-1.2.0/samples/store.py
--rw-r--r--   0        0        0       28 2023-06-08 10:44:39.606940 meritous-1.2.0/setup.cfg
--rw-r--r--   0        0        0     6084 2024-03-06 22:00:16.090382 meritous-1.2.0/src/meritous/core/__init__.py
--rw-r--r--   0        0        0      184 2024-03-05 21:58:24.887867 meritous-1.2.0/src/meritous/core/exceptions.py
--rw-r--r--   0        0        0      357 2024-02-17 08:17:16.569609 meritous-1.2.0/src/meritous/core/i18n.py
--rw-r--r--   0        0        0      392 2024-03-07 06:30:47.486455 meritous-1.2.0/src/meritous/core/i18n_data/en.toml
--rw-r--r--   0        0        0      947 2024-03-06 06:54:02.407663 meritous-1.2.0/src/meritous/core/properties.py
--rw-r--r--   0        0        0      559 2024-03-06 21:43:50.569893 meritous-1.2.0/src/meritous/core/serializers.py
--rw-r--r--   0        0        0      269 2024-03-06 21:59:48.177709 meritous-1.2.0/src/meritous/core/stores.py
--rw-r--r--   0        0        0      115 2024-03-07 06:53:12.526328 meritous-1.2.0/tests/meritous/data.py
--rw-r--r--   0        0        0       77 2024-02-17 08:35:51.627256 meritous-1.2.0/tests/meritous/properties/data.py
--rw-r--r--   0        0        0      892 2024-03-07 06:39:31.269815 meritous-1.2.0/tests/meritous/properties/test_property_date.py
--rw-r--r--   0        0        0      437 2024-03-06 22:06:27.563767 meritous-1.2.0/tests/meritous/properties/test_property_int.py
--rw-r--r--   0        0        0      452 2024-03-06 22:06:39.204071 meritous-1.2.0/tests/meritous/properties/test_property_str.py
--rw-r--r--   0        0        0      358 2024-03-06 22:06:48.348310 meritous-1.2.0/tests/meritous/properties/test_uuid.py
--rw-r--r--   0        0        0      116 2024-03-07 06:52:12.653399 meritous-1.2.0/tests/meritous/stores/data.py
--rw-r--r--   0        0        0      723 2024-03-07 06:54:03.503119 meritous-1.2.0/tests/meritous/stores/test_file.py
--rw-r--r--   0        0        0     1813 2024-03-06 22:20:21.067938 meritous-1.2.0/tests/meritous/test_model.py
--rw-r--r--   0        0        0     1472 2024-03-06 22:11:25.417408 meritous-1.2.0/tests/meritous/test_property.py
--rw-r--r--   0        0        0      459 2024-03-06 22:07:14.216988 meritous-1.2.0/tests/meritous/test_schema.py
--rw-r--r--   0        0        0      752 2024-03-07 06:31:04.414677 meritous-1.2.0/tests/meritous/test_serializer.py
--rw-r--r--   0        0        0      526 2024-03-07 06:36:31.247192 meritous-1.2.0/tests/meritous/test_store.py
--rw-r--r--   0        0        0     2645 1970-01-01 00:00:00.000000 meritous-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      159 2023-06-08 11:00:10.322398 meritous-1.2.1/.codeclimate.yml
+-rw-r--r--   0        0        0     3078 2023-03-04 08:09:15.684878 meritous-1.2.1/.gitignore
+-rw-r--r--   0        0        0       13 2023-02-23 13:38:24.154245 meritous-1.2.1/.python-version
+-rw-r--r--   0        0        0      168 2024-03-07 07:11:42.076445 meritous-1.2.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1077 2023-03-04 08:01:19.863201 meritous-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1714 2024-03-07 07:04:03.043504 meritous-1.2.1/README.md
+-rw-r--r--   0        0        0      634 2023-06-02 05:33:09.164663 meritous-1.2.1/docs/Makefile
+-rw-r--r--   0        0        0     1054 2024-03-07 07:00:43.549153 meritous-1.2.1/docs/concepts.rst
+-rw-r--r--   0        0        0      522 2023-06-08 10:49:50.666394 meritous-1.2.1/docs/conf.py
+-rw-r--r--   0        0        0      184 2023-06-02 07:28:36.492517 meritous-1.2.1/docs/extensions.rst
+-rw-r--r--   0        0        0     1762 2024-03-07 07:03:23.406844 meritous-1.2.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-06-02 05:33:09.164663 meritous-1.2.1/docs/make.bat
+-rw-r--r--   0        0        0     3486 2024-03-07 07:01:54.517773 meritous-1.2.1/docs/properties.rst
+-rw-r--r--   0        0        0       40 2024-03-07 07:11:11.488361 meritous-1.2.1/docs/requirements.txt
+-rw-r--r--   0        0        0     1425 2024-03-07 14:49:25.315692 meritous-1.2.1/docs/start.rst
+-rw-r--r--   0        0        0      180 2023-06-02 07:27:15.188275 meritous-1.2.1/docs/stores.rst
+-rw-r--r--   0        0        0      173 2023-05-20 06:32:12.910513 meritous-1.2.1/noxfile.py
+-rw-r--r--   0        0        0     1109 2024-03-06 21:27:24.241957 meritous-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      116 2024-03-06 21:48:02.943924 meritous-1.2.1/samples/event.json
+-rw-r--r--   0        0        0      692 2024-03-06 06:36:03.154026 meritous-1.2.1/samples/event.py
+-rw-r--r--   0        0        0      955 2024-03-06 21:44:38.122078 meritous-1.2.1/samples/serializers.py
+-rw-r--r--   0        0        0      678 2024-03-06 22:01:48.520648 meritous-1.2.1/samples/store.py
+-rw-r--r--   0        0        0       28 2023-06-08 10:44:39.606940 meritous-1.2.1/setup.cfg
+-rw-r--r--   0        0        0     6465 2024-04-20 09:47:41.028804 meritous-1.2.1/src/meritous/core/__init__.py
+-rw-r--r--   0        0        0      184 2024-03-05 21:58:24.887867 meritous-1.2.1/src/meritous/core/exceptions.py
+-rw-r--r--   0        0        0      357 2024-02-17 08:17:16.569609 meritous-1.2.1/src/meritous/core/i18n.py
+-rw-r--r--   0        0        0      415 2024-03-25 13:46:32.745291 meritous-1.2.1/src/meritous/core/i18n_data/en.toml
+-rw-r--r--   0        0        0     1473 2024-03-17 08:31:06.806985 meritous-1.2.1/src/meritous/core/properties.py
+-rw-r--r--   0        0        0      559 2024-03-06 21:43:50.569893 meritous-1.2.1/src/meritous/core/serializers.py
+-rw-r--r--   0        0        0      269 2024-03-06 21:59:48.177709 meritous-1.2.1/src/meritous/core/stores.py
+-rw-r--r--   0        0        0      115 2024-03-07 06:53:12.526328 meritous-1.2.1/tests/meritous/data.py
+-rw-r--r--   0        0        0      147 2024-04-20 09:42:37.333991 meritous-1.2.1/tests/meritous/properties/data.py
+-rw-r--r--   0        0        0     1069 2024-04-20 09:46:10.251209 meritous-1.2.1/tests/meritous/properties/test_property_basics.py
+-rw-r--r--   0        0        0      892 2024-03-07 06:39:31.269815 meritous-1.2.1/tests/meritous/properties/test_property_date.py
+-rw-r--r--   0        0        0      358 2024-03-06 22:06:48.348310 meritous-1.2.1/tests/meritous/properties/test_uuid.py
+-rw-r--r--   0        0        0      116 2024-03-07 06:52:12.653399 meritous-1.2.1/tests/meritous/stores/data.py
+-rw-r--r--   0        0        0      723 2024-03-07 06:54:03.503119 meritous-1.2.1/tests/meritous/stores/test_file.py
+-rw-r--r--   0        0        0     2135 2024-03-15 09:56:12.040182 meritous-1.2.1/tests/meritous/test_model.py
+-rw-r--r--   0        0        0     1472 2024-03-06 22:11:25.417408 meritous-1.2.1/tests/meritous/test_property.py
+-rw-r--r--   0        0        0      459 2024-03-06 22:07:14.216988 meritous-1.2.1/tests/meritous/test_schema.py
+-rw-r--r--   0        0        0      752 2024-03-07 06:31:04.414677 meritous-1.2.1/tests/meritous/test_serializer.py
+-rw-r--r--   0        0        0      526 2024-03-07 06:36:31.247192 meritous-1.2.1/tests/meritous/test_store.py
+-rw-r--r--   0        0        0     2655 1970-01-01 00:00:00.000000 meritous-1.2.1/PKG-INFO
```

### Comparing `meritous-1.2.0/.gitignore` & `meritous-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `meritous-1.2.0/LICENSE` & `meritous-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meritous-1.2.0/README.md` & `meritous-1.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 ```bash
 pip install meritous
 ```
 
 ## Basic Usage
 
 ```python
-from meritous import Model
-from meritous.properties import UUIDProperty, StrProperty, DateProperty
+from meritous.core import Model
+from meritous.core.properties import UUIDProperty, StrProperty, DateProperty
 
 from datetime import date
 
 class EventModel(Model):
 
     _schema = {
         "id"          : UUID4Property(),
```

### Comparing `meritous-1.2.0/docs/Makefile` & `meritous-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `meritous-1.2.0/docs/concepts.rst` & `meritous-1.2.1/docs/concepts.rst`

 * *Files 11% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 * Model
     The main data structure containing a Schema of defined Properties
 * Schema
     Represents the expected data structure of a Model
 * Property
     The main data values of the Model referenced in a Schema
-* Store
-    Stores are used to transform models for storage or transport
+* Serializers
+    Serializers are used to transform models into different formats for storage
 
 
 Models
 ------
 
 Models represent the main data structure of Meritous.
```

### Comparing `meritous-1.2.0/docs/conf.py` & `meritous-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `meritous-1.2.0/docs/index.rst` & `meritous-1.2.1/docs/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 Sample Usage
 ------------
 
 Here is an example demonstrating a full use case for Meritous (utilising optional integrations for AWS DynamoDB).
 
 .. code-block:: python
 
-  from meritous import Model
-  from meritous.properties import UUIDProperty, StrProperty, DateProperty
+  from meritous.core import Model
+  from meritous.core.properties import UUIDProperty, StrProperty, DateProperty
 
-  from meritous.aws.stores.dynamodb import DynamoDBStore
+  from meritous.aws.dynamodb import DynamodbStore, DynamodbSerializer
 
   import boto3, datetime
 
   class EventModel(Model):
 
       _schema = {
           "id"    : UUIDProperty(),
@@ -41,15 +41,15 @@
 
   event = Event()
   event.title = 'Sample Event'
   event.date = datetime.date.fromisoformat('2023-01-10')
 
   dynamodb = boto3.resource('dynamodb')
 
-  store = DynamoDBStore(dynamodb.Table('sample_event_table'))
+  store = DynamodbStore(dynamodb.Table('sample_event_table'), DynamodbSerializer)
 
   store.save(KeyProperties=['id'], Item=event)
 
   event_recover = store.get(Key={'id' : event.id}, Model=EventModel)
 
   print(event.id == event_recover.id)
```

### Comparing `meritous-1.2.0/docs/make.bat` & `meritous-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `meritous-1.2.0/docs/properties.rst` & `meritous-1.2.1/docs/properties.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,52 +2,52 @@
 ======================================
 
 Properties are the data primitives of Meritous. Several are included as built-in and you can quickly and easily define your own as well.
 
 Built-in Properties
 -------------------
 
-.. autoclass:: meritous.properties::StrProperty
+.. autoclass:: meritous.core.properties::StrProperty
 
-.. autoclass:: meritous.properties::IntProperty
+.. autoclass:: meritous.core.properties::IntProperty
 
-.. autoclass:: meritous.properties::UUID4Property
+.. autoclass:: meritous.core.properties::UUID4Property
 
 Creating additional Properties
 ------------------------------
 
 Properties are created simply by sub-classing Property. For example, imagine we wanted a Property representing string data (this is one of Meritous' built-in properties):
 
 .. code-block:: python
 
   from meritous.core import Property
 
-  class StrProperty:
+  class StrProperty(Property):
     pass
 
 
 In itself this isn't very helpful other than giving our Property a special name. However, we can overload the `__init__` method to make this class validate specifically strings:
 
 .. code-block:: python
 
   from meritous.core import Property
 
-  class StrProperty:
+  class StrProperty(Property):
 
     def __init__(self, **kwargs):
       super().__init__(str, **kwargs)
 
 
 We can take advantage of 'type' being the only positional argument in the original `Property.__init__` definition to carry any keyword arguments whilst forcing `type` to be str.
 
 This is a very simple property for which the `validate` method will test values against the str type. For example:
 
 .. code-block:: python
 
-  >>> from meritous.properties import StrProperty
+  >>> from meritous.core.properties import StrProperty
   >>> p = StrProperty()
   >>> p.validate('a string')
   'True'
   >>> p.validate(1)
   'False'
 
 
@@ -92,15 +92,15 @@
         return False
       return True
 
 This will now validate several ways.
 
 .. code-block:: python
 
-  >>> from meritous.properties import UUID4Property
+  >>> from meritous.core.properties import UUID4Property
   >>> import uuid
   >>> p = UUID4Property()
   >>> str(p.default)
   '0382d829-0fd7-4587-9446-fb7371369e94'
   >>> p.validate(str(p.default))
   'True'
   >>> p.validate(uuid.UUID4())
```

### Comparing `meritous-1.2.0/docs/start.rst` & `meritous-1.2.1/docs/start.rst`

 * *Files 5% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 Basic Usage
 -----------
 
 Meritous can be used to quickly bootstrap simple Models with defined data elements. The following example demonstrates the basic functionality in the context of an "Event" data structure.
 
 .. code-block:: python
 
-  from meritous import Model
-  from meritous.properties import UUIDProperty, StrProperty, DateProperty
+  from meritous.core import Model
+  from meritous.core.properties import UUIDProperty, StrProperty, DateProperty
 
   from datetime import date
 
   class EventModel(Model):
 
       _schema = {
           "id"          : UUID4Property(),
```

### Comparing `meritous-1.2.0/pyproject.toml` & `meritous-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meritous-1.2.0/samples/event.py` & `meritous-1.2.1/samples/event.py`

 * *Files identical despite different names*

### Comparing `meritous-1.2.0/samples/serializers.py` & `meritous-1.2.1/samples/serializers.py`

 * *Files identical despite different names*

### Comparing `meritous-1.2.0/samples/store.py` & `meritous-1.2.1/samples/store.py`

 * *Files identical despite different names*

### Comparing `meritous-1.2.0/src/meritous/core/__init__.py` & `meritous-1.2.1/src/meritous/core/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Simple Python Models
 """
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 
 from .exceptions import *
 from .i18n import text
 
 
 class Property:
     """
@@ -14,44 +14,50 @@
     Parameters
     ----------
     type
         Valid Python type representing the expected type of this property
     default
         The default value for the property
     required
-        Indicates weather this property is a required value
+        Indicates whether this property is a required value
     """
     _type = None
     _default = None
     _required = None
+    _nullable = None
 
-    def __init__(self, type, default=None, required=True):
+    def __init__(self, type, default=None, required=True, nullable=False):
         self._type = type
         self._required = required
+        self._nullable = nullable
 
         if default and not self.validate(default):
-            raise PropertyException(text.error.prop.type.format(self.__class__.__name__, type(default)))
+            raise PropertyException(text.error.prop.type.format(self.__class__.__name__, type(default), type))
 
         self._default = default
 
     def validate(self, value):
         """
         Validate a property against a provided value
 
 
         Parameters
         ----------
         value
             Value to be tested against the set Property type
         """
-        return type(value) == self._type
+        return True if self.is_nullable and value == None else type(value) == self._type
 
     @property
     def is_required(self):
         return self._required
+    
+    @property
+    def is_nullable(self):
+        return self._nullable
 
     @property
     def default(self):
         return self._default
 
     @property
     def type(self):
@@ -65,18 +71,18 @@
     def classname(self):
         return self.__class__.__name__
 
     def _add_name(self, name):
         self._name = name
 
     def serialize(self, value):
-        return self._type(value)
+        return None if self.is_nullable and value == None else  self._type(value)
     
     def deserialize(self, value):
-        return self._type(value)
+        return None if self.is_nullable and value == None else self._type(value)
 
 
 class Schema(dict):
 
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
         for name in self:
@@ -150,28 +156,31 @@
         if name != '_data' and name in self._data:
             if not self._schema[name].validate(value):
                 raise PropertyException(text.error.prop.set.format(self.__class__.__name__, value, self._type, self._schema[name]._type))
             self._data[name] = value
         else:
             self.__dict__[name] = value
 
+    def __eq__(self, other):
+        return self.items() == other.items()
+
     def items(self):
         return self._data.items()
     
     @property
     def schema(self):
         return self._schema
     
     def validate(self):
         for name, value in self._data.items():
             if name not in self._schema:
                 raise ModelException(text.error.model.validate.format(name))
             if not self._schema[name].validate(value):
                 property = self._schema[name]
-                raise PropertyException(text.error.prop.type.format(property.classname, property.type))
+                raise PropertyException(text.error.prop.type.format(property.name, property.type, type(value)))
         return True
     
     @classmethod
     def new(cls, data):
         return cls(_data=data)
```

### Comparing `meritous-1.2.0/src/meritous/core/serializers.py` & `meritous-1.2.1/src/meritous/core/serializers.py`

 * *Files identical despite different names*

### Comparing `meritous-1.2.0/tests/meritous/properties/test_property_date.py` & `meritous-1.2.1/tests/meritous/properties/test_property_date.py`

 * *Files identical despite different names*

### Comparing `meritous-1.2.0/tests/meritous/stores/test_file.py` & `meritous-1.2.1/tests/meritous/stores/test_file.py`

 * *Files identical despite different names*

### Comparing `meritous-1.2.0/tests/meritous/test_model.py` & `meritous-1.2.1/tests/meritous/test_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-
-
 import pytest
 
 import data
 
 from meritous.core import Model, Schema, Property
 import meritous.core.exceptions
 
@@ -58,8 +56,18 @@
 def test_model_validate_invalid_property():
     m = ModelTest(_data = {data.TEST_STR_ALT : data.TEST_INT})
     with pytest.raises(meritous.core.exceptions.ModelException):
         m.validate()
     
 def test_model_new():
     m = ModelTest.new({data.TEST_STR : data.TEST_STR_ALT})
-    assert m.TEST == data.TEST_STR_ALT
+    assert m.TEST == data.TEST_STR_ALT
+
+def test_model_eq():
+    m = ModelTest.new({data.TEST_STR : data.TEST_STR_ALT})
+    m2 = ModelTest.new({data.TEST_STR : data.TEST_STR_ALT})
+    assert m == m2
+
+def test_model_not_eq():
+    m = ModelTest.new({data.TEST_STR : data.TEST_STR_ALT})
+    m2 = ModelTest.new({data.TEST_STR_ALT : data.TEST_STR})
+    assert m != m2
```

### Comparing `meritous-1.2.0/tests/meritous/test_property.py` & `meritous-1.2.1/tests/meritous/test_property.py`

 * *Files identical despite different names*

### Comparing `meritous-1.2.0/tests/meritous/test_serializer.py` & `meritous-1.2.1/tests/meritous/test_serializer.py`

 * *Files identical despite different names*

### Comparing `meritous-1.2.0/tests/meritous/test_store.py` & `meritous-1.2.1/tests/meritous/test_store.py`

 * *Files identical despite different names*

### Comparing `meritous-1.2.0/PKG-INFO` & `meritous-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meritous
-Version: 1.2.0
+Version: 1.2.1
 Summary: Simple Python Models
 Keywords: model
 Author-email: Tom Morton <tom@errant.me.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
@@ -46,16 +46,16 @@
 ```bash
 pip install meritous
 ```
 
 ## Basic Usage
 
 ```python
-from meritous import Model
-from meritous.properties import UUIDProperty, StrProperty, DateProperty
+from meritous.core import Model
+from meritous.core.properties import UUIDProperty, StrProperty, DateProperty
 
 from datetime import date
 
 class EventModel(Model):
 
     _schema = {
         "id"          : UUID4Property(),
```

