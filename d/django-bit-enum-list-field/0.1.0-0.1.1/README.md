# Comparing `tmp/django_bit_enum_list_field-0.1.0.tar.gz` & `tmp/django_bit_enum_list_field-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_bit_enum_list_field-0.1.0.tar", max compression
+gzip compressed data, was "django_bit_enum_list_field-0.1.1.tar", max compression
```

## Comparing `django_bit_enum_list_field-0.1.0.tar` & `django_bit_enum_list_field-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35148 2024-03-05 17:24:59.296644 django_bit_enum_list_field-0.1.0/LICENSE
--rw-r--r--   0        0        0     2615 2024-03-05 17:24:59.296777 django_bit_enum_list_field-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-03-05 17:31:50.273745 django_bit_enum_list_field-0.1.0/bit_enum_list_field/__init__.py
--rw-r--r--   0        0        0     1539 2024-03-05 18:02:18.285883 django_bit_enum_list_field-0.1.0/bit_enum_list_field/bit_enum_list_field.py
--rw-r--r--   0        0        0      946 2024-03-05 18:03:03.528491 django_bit_enum_list_field-0.1.0/bit_enum_list_field/lookups/__pycache__/bit_enum_list_all_lookup.cpython-312.pyc
--rw-r--r--   0        0        0      907 2024-03-05 18:03:03.528847 django_bit_enum_list_field-0.1.0/bit_enum_list_field/lookups/__pycache__/bit_enum_list_any_lookup.cpython-312.pyc
--rw-r--r--   0        0        0      911 2024-03-05 18:03:03.529360 django_bit_enum_list_field-0.1.0/bit_enum_list_field/lookups/__pycache__/bit_enum_list_none_lookup.cpython-312.pyc
--rw-r--r--   0        0        0      371 2024-03-05 17:24:59.298047 django_bit_enum_list_field-0.1.0/bit_enum_list_field/lookups/bit_enum_list_all_lookup.py
--rw-r--r--   0        0        0      351 2024-03-05 17:24:59.298140 django_bit_enum_list_field-0.1.0/bit_enum_list_field/lookups/bit_enum_list_any_lookup.py
--rw-r--r--   0        0        0      353 2024-03-05 17:24:59.298228 django_bit_enum_list_field-0.1.0/bit_enum_list_field/lookups/bit_enum_list_none_lookup.py
--rw-r--r--   0        0        0     1079 2024-03-05 18:04:13.454105 django_bit_enum_list_field-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3716 1970-01-01 00:00:00.000000 django_bit_enum_list_field-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-03-05 17:24:59.296644 django_bit_enum_list_field-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2615 2024-03-05 17:24:59.296777 django_bit_enum_list_field-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-05 17:31:50.273745 django_bit_enum_list_field-0.1.1/bit_enum_list_field/__init__.py
+-rw-r--r--   0        0        0     1610 2024-04-20 13:07:03.962577 django_bit_enum_list_field-0.1.1/bit_enum_list_field/bit_enum_list_field.py
+-rw-r--r--   0        0        0      946 2024-03-05 18:03:03.528491 django_bit_enum_list_field-0.1.1/bit_enum_list_field/lookups/__pycache__/bit_enum_list_all_lookup.cpython-312.pyc
+-rw-r--r--   0        0        0      907 2024-03-05 18:03:03.528847 django_bit_enum_list_field-0.1.1/bit_enum_list_field/lookups/__pycache__/bit_enum_list_any_lookup.cpython-312.pyc
+-rw-r--r--   0        0        0      911 2024-03-05 18:03:03.529360 django_bit_enum_list_field-0.1.1/bit_enum_list_field/lookups/__pycache__/bit_enum_list_none_lookup.cpython-312.pyc
+-rw-r--r--   0        0        0      371 2024-03-05 17:24:59.298047 django_bit_enum_list_field-0.1.1/bit_enum_list_field/lookups/bit_enum_list_all_lookup.py
+-rw-r--r--   0        0        0      351 2024-03-05 17:24:59.298140 django_bit_enum_list_field-0.1.1/bit_enum_list_field/lookups/bit_enum_list_any_lookup.py
+-rw-r--r--   0        0        0      353 2024-03-05 17:24:59.298228 django_bit_enum_list_field-0.1.1/bit_enum_list_field/lookups/bit_enum_list_none_lookup.py
+-rw-r--r--   0        0        0     1079 2024-04-20 14:04:56.602904 django_bit_enum_list_field-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3716 1970-01-01 00:00:00.000000 django_bit_enum_list_field-0.1.1/PKG-INFO
```

### Comparing `django_bit_enum_list_field-0.1.0/LICENSE` & `django_bit_enum_list_field-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_bit_enum_list_field-0.1.0/README.md` & `django_bit_enum_list_field-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django_bit_enum_list_field-0.1.0/bit_enum_list_field/bit_enum_list_field.py` & `django_bit_enum_list_field-0.1.1/bit_enum_list_field/bit_enum_list_field.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from bit_enum_list_field.lookups.bit_enum_list_any_lookup import BitEnumListAnyLookup
 from bit_enum_list_field.lookups.bit_enum_list_none_lookup import BitEnumListNoneLookup
 
 
 class BitEnumListField(BigIntegerField):
     def __init__(self, enum: Type[Enum], *args, **kwargs):
         self.enum = enum
+        if "default" not in kwargs:
+            kwargs["default"] = []
         super().__init__(*args, **kwargs)
 
     def deconstruct(self):
         name, path, args, kwargs = super(BitEnumListField, self).deconstruct()
         args = [self.enum] + args
         return name, path, args, kwargs
```

### Comparing `django_bit_enum_list_field-0.1.0/bit_enum_list_field/lookups/__pycache__/bit_enum_list_all_lookup.cpython-312.pyc` & `django_bit_enum_list_field-0.1.1/bit_enum_list_field/lookups/__pycache__/bit_enum_list_all_lookup.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_bit_enum_list_field-0.1.0/bit_enum_list_field/lookups/__pycache__/bit_enum_list_any_lookup.cpython-312.pyc` & `django_bit_enum_list_field-0.1.1/bit_enum_list_field/lookups/__pycache__/bit_enum_list_any_lookup.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_bit_enum_list_field-0.1.0/bit_enum_list_field/lookups/__pycache__/bit_enum_list_none_lookup.cpython-312.pyc` & `django_bit_enum_list_field-0.1.1/bit_enum_list_field/lookups/__pycache__/bit_enum_list_none_lookup.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_bit_enum_list_field-0.1.0/pyproject.toml` & `django_bit_enum_list_field-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-bit-enum-list-field"
-version = "0.1.0"
+version = "0.1.1"
 description = "A field for Django models to store lists of enums as integers"
 authors = ["Emanuele Manfredini <emanuele.manfredini.1992@gmail.com>"]
 license = "GPLv3"
 repository = "https://github.com/tavearn/django-bit-enum-list-field"
 homepage = "https://github.com/tavearn/django-bit-enum-list-field"
 readme = "README.md"
 classifiers = [
```

### Comparing `django_bit_enum_list_field-0.1.0/PKG-INFO` & `django_bit_enum_list_field-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bit-enum-list-field
-Version: 0.1.0
+Version: 0.1.1
 Summary: A field for Django models to store lists of enums as integers
 Home-page: https://github.com/tavearn/django-bit-enum-list-field
 License: GPLv3
 Author: Emanuele Manfredini
 Author-email: emanuele.manfredini.1992@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

