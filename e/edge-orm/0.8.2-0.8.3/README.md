# Comparing `tmp/edge_orm-0.8.2.tar.gz` & `tmp/edge_orm-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge_orm-0.8.2.tar", max compression
+gzip compressed data, was "edge_orm-0.8.3.tar", max compression
```

## Comparing `edge_orm-0.8.2.tar` & `edge_orm-0.8.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       10 2023-02-08 20:21:01.345400 edge_orm-0.8.2/README.md
--rw-r--r--   0        0        0      842 2023-06-02 19:51:59.698747 edge_orm-0.8.2/edge_orm/__init__.py
--rw-r--r--   0        0        0     1729 2023-02-08 20:21:01.355224 edge_orm-0.8.2/edge_orm/cache.py
--rw-r--r--   0        0        0      108 2023-02-08 20:21:01.355283 edge_orm-0.8.2/edge_orm/errors.py
--rw-r--r--   0        0        0     2191 2023-02-08 20:21:01.355352 edge_orm-0.8.2/edge_orm/execute.py
--rw-r--r--   0        0        0     5463 2023-06-02 18:07:35.502233 edge_orm-0.8.2/edge_orm/external/encoders.py
--rw-r--r--   0        0        0     1036 2023-02-08 20:21:01.355536 edge_orm-0.8.2/edge_orm/helpers.py
--rw-r--r--   0        0        0     2194 2023-02-08 20:21:01.355611 edge_orm-0.8.2/edge_orm/logs.py
--rw-r--r--   0        0        0      302 2023-02-08 20:21:01.355706 edge_orm-0.8.2/edge_orm/node/__init__.py
--rw-r--r--   0        0        0       41 2023-02-08 20:21:01.355784 edge_orm-0.8.2/edge_orm/node/errors.py
--rw-r--r--   0        0        0     4514 2023-06-02 17:45:03.025272 edge_orm-0.8.2/edge_orm/node/models.py
--rw-r--r--   0        0        0      287 2023-04-19 17:57:56.361008 edge_orm-0.8.2/edge_orm/resolver/__init__.py
--rw-r--r--   0        0        0      180 2023-02-08 20:21:01.356047 edge_orm-0.8.2/edge_orm/resolver/enums.py
--rw-r--r--   0        0        0      135 2023-02-27 21:40:59.506123 edge_orm-0.8.2/edge_orm/resolver/errors.py
--rw-r--r--   0        0        0     5270 2023-02-08 20:21:01.356166 edge_orm-0.8.2/edge_orm/resolver/merging.py
--rw-r--r--   0        0        0    42417 2023-06-02 18:10:30.983018 edge_orm-0.8.2/edge_orm/resolver/model.py
--rw-r--r--   0        0        0     5300 2023-05-26 15:22:47.425858 edge_orm-0.8.2/edge_orm/resolver/nested_resolvers.py
--rw-r--r--   0        0        0     3975 2023-06-02 18:08:35.542034 edge_orm-0.8.2/edge_orm/resolver/utils.py
--rw-r--r--   0        0        0      957 2023-02-08 20:21:01.356588 edge_orm-0.8.2/edge_orm/span.py
--rw-r--r--   0        0        0      251 2023-02-08 20:21:01.356691 edge_orm-0.8.2/edge_orm/types_generator/__init__.py
--rw-r--r--   0        0        0     8120 2023-04-04 16:56:52.369943 edge_orm-0.8.2/edge_orm/types_generator/introspection.py
--rw-r--r--   0        0        0    38602 2023-06-02 20:46:59.525691 edge_orm-0.8.2/edge_orm/types_generator/main.py
--rw-r--r--   0        0        0      791 2023-02-08 20:21:01.357019 edge_orm-0.8.2/edge_orm/unset.py
--rw-r--r--   0        0        0     1080 2023-06-02 20:49:32.592882 edge_orm-0.8.2/edge_orm/validators.py
--rw-r--r--   0        0        0      277 2023-06-02 20:41:12.570547 edge_orm-0.8.2/edge_orm/validators_v2.py
--rw-r--r--   0        0        0      803 2023-06-21 16:33:33.205578 edge_orm-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      546 1970-01-01 00:00:00.000000 edge_orm-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0       10 2023-02-08 20:21:01.345400 edge_orm-0.8.3/README.md
+-rw-r--r--   0        0        0      842 2023-06-02 19:51:59.698747 edge_orm-0.8.3/edge_orm/__init__.py
+-rw-r--r--   0        0        0     1729 2023-02-08 20:21:01.355224 edge_orm-0.8.3/edge_orm/cache.py
+-rw-r--r--   0        0        0      108 2023-02-08 20:21:01.355283 edge_orm-0.8.3/edge_orm/errors.py
+-rw-r--r--   0        0        0     2191 2023-02-08 20:21:01.355352 edge_orm-0.8.3/edge_orm/execute.py
+-rw-r--r--   0        0        0     5463 2023-06-02 18:07:35.502233 edge_orm-0.8.3/edge_orm/external/encoders.py
+-rw-r--r--   0        0        0     1036 2023-02-08 20:21:01.355536 edge_orm-0.8.3/edge_orm/helpers.py
+-rw-r--r--   0        0        0     2194 2023-02-08 20:21:01.355611 edge_orm-0.8.3/edge_orm/logs.py
+-rw-r--r--   0        0        0      302 2023-02-08 20:21:01.355706 edge_orm-0.8.3/edge_orm/node/__init__.py
+-rw-r--r--   0        0        0       41 2023-02-08 20:21:01.355784 edge_orm-0.8.3/edge_orm/node/errors.py
+-rw-r--r--   0        0        0     4514 2023-06-02 17:45:03.025272 edge_orm-0.8.3/edge_orm/node/models.py
+-rw-r--r--   0        0        0      287 2023-04-19 17:57:56.361008 edge_orm-0.8.3/edge_orm/resolver/__init__.py
+-rw-r--r--   0        0        0      180 2023-02-08 20:21:01.356047 edge_orm-0.8.3/edge_orm/resolver/enums.py
+-rw-r--r--   0        0        0      135 2023-02-27 21:40:59.506123 edge_orm-0.8.3/edge_orm/resolver/errors.py
+-rw-r--r--   0        0        0     5270 2023-02-08 20:21:01.356166 edge_orm-0.8.3/edge_orm/resolver/merging.py
+-rw-r--r--   0        0        0    42417 2023-06-02 18:10:30.983018 edge_orm-0.8.3/edge_orm/resolver/model.py
+-rw-r--r--   0        0        0     5300 2023-05-26 15:22:47.425858 edge_orm-0.8.3/edge_orm/resolver/nested_resolvers.py
+-rw-r--r--   0        0        0     3975 2023-06-02 18:08:35.542034 edge_orm-0.8.3/edge_orm/resolver/utils.py
+-rw-r--r--   0        0        0      957 2023-02-08 20:21:01.356588 edge_orm-0.8.3/edge_orm/span.py
+-rw-r--r--   0        0        0      251 2023-02-08 20:21:01.356691 edge_orm-0.8.3/edge_orm/types_generator/__init__.py
+-rw-r--r--   0        0        0     8120 2023-04-04 16:56:52.369943 edge_orm-0.8.3/edge_orm/types_generator/introspection.py
+-rw-r--r--   0        0        0    38602 2023-06-02 20:46:59.525691 edge_orm-0.8.3/edge_orm/types_generator/main.py
+-rw-r--r--   0        0        0      791 2023-02-08 20:21:01.357019 edge_orm-0.8.3/edge_orm/unset.py
+-rw-r--r--   0        0        0     1080 2023-06-02 20:49:32.592882 edge_orm-0.8.3/edge_orm/validators.py
+-rw-r--r--   0        0        0      277 2023-06-02 20:41:12.570547 edge_orm-0.8.3/edge_orm/validators_v2.py
+-rw-r--r--   0        0        0      806 2023-06-21 16:36:02.616505 edge_orm-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 edge_orm-0.8.3/PKG-INFO
```

### Comparing `edge_orm-0.8.2/edge_orm/__init__.py` & `edge_orm-0.8.3/edge_orm/__init__.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.8.2/edge_orm/cache.py` & `edge_orm-0.8.3/edge_orm/cache.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.8.2/edge_orm/execute.py` & `edge_orm-0.8.3/edge_orm/execute.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.8.2/edge_orm/external/encoders.py` & `edge_orm-0.8.3/edge_orm/external/encoders.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.8.2/edge_orm/helpers.py` & `edge_orm-0.8.3/edge_orm/helpers.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.8.2/edge_orm/logs.py` & `edge_orm-0.8.3/edge_orm/logs.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.8.2/edge_orm/node/models.py` & `edge_orm-0.8.3/edge_orm/node/models.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.8.2/edge_orm/resolver/merging.py` & `edge_orm-0.8.3/edge_orm/resolver/merging.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.8.2/edge_orm/resolver/model.py` & `edge_orm-0.8.3/edge_orm/resolver/model.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.8.2/edge_orm/resolver/nested_resolvers.py` & `edge_orm-0.8.3/edge_orm/resolver/nested_resolvers.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.8.2/edge_orm/resolver/utils.py` & `edge_orm-0.8.3/edge_orm/resolver/utils.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.8.2/edge_orm/span.py` & `edge_orm-0.8.3/edge_orm/span.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.8.2/edge_orm/types_generator/introspection.py` & `edge_orm-0.8.3/edge_orm/types_generator/introspection.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.8.2/edge_orm/types_generator/main.py` & `edge_orm-0.8.3/edge_orm/types_generator/main.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.8.2/edge_orm/unset.py` & `edge_orm-0.8.3/edge_orm/unset.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.8.2/edge_orm/validators.py` & `edge_orm-0.8.3/edge_orm/validators.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.8.2/pyproject.toml` & `edge_orm-0.8.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "edge-orm"
-version = "0.8.2"
+version = "0.8.3"
 description = ""
 authors = ["Jeremy Berman <jerber@sas.upenn.edu>"]
 readme = "README.md"
 packages = [{ include = "edge_orm" }]
 exclude = ["tests/**/*"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 edgedb = "^1.2.0"
-pydantic = { version = ">=2", allow-prereleases = true, extras = ['email'] }
+pydantic = { version = "^2.0a1", allow-prereleases = true, extras = ['email'] }
 #pydantic = { extras = ["email"], version = "^1.10" }
 orjson = "^3.8.0"
 devtools = "*"
 black = "*"
 
 
 mkdocs-material = { version = "^8.5.7", optional = true }
```

### Comparing `edge_orm-0.8.2/PKG-INFO` & `edge_orm-0.8.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: edge-orm
-Version: 0.8.2
+Version: 0.8.3
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: black
 Requires-Dist: devtools
 Requires-Dist: edgedb (>=1.2.0,<2.0.0)
 Requires-Dist: mkdocs-material (>=8.5.7,<9.0.0) ; extra == "docs"
 Requires-Dist: orjson (>=3.8.0,<4.0.0)
-Requires-Dist: pydantic[email] (>=2)
+Requires-Dist: pydantic[email] (>=2.0a1,<3.0)
 Description-Content-Type: text/markdown
 
 # edge orm
```

