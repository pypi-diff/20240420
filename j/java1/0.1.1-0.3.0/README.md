# Comparing `tmp/java1-0.1.1.tar.gz` & `tmp/java1-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "java1-0.1.1.tar", max compression
+gzip compressed data, was "java1-0.3.0.tar", max compression
```

## Comparing `java1-0.1.1.tar` & `java1-0.3.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0   104411 2024-04-20 12:21:06.000000 java1-0.1.1/java1/__init__.py
--rw-r--r--   0        0        0      287 2024-04-20 03:48:13.318089 java1-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 java1-0.1.1/setup.py
--rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 java1-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    64225 2024-04-17 01:09:02.000000 java1-0.3.0/java1/__init__.py
+-rw-r--r--   0        0        0      287 2024-04-17 01:31:17.832103 java1-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 java1-0.3.0/setup.py
+-rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 java1-0.3.0/PKG-INFO
```

### Comparing `java1-0.1.1/setup.py` & `java1-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['java1']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'java1',
-    'version': '0.1.1',
+    'version': '0.3.0',
     'description': 'A short description of your project',
     'long_description': 'None',
     'author': 'Vinit',
     'author_email': 'suryawanshivinit02@email.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `java1-0.1.1/PKG-INFO` & `java1-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: java1
-Version: 0.1.1
+Version: 0.3.0
 Summary: A short description of your project
 Author: Vinit
 Author-email: suryawanshivinit02@email.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

