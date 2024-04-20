# Comparing `tmp/jarvis_orm-0.0.2.tar.gz` & `tmp/jarvis_orm-0.0.3.tar.gz`

## Comparing `jarvis_orm-0.0.2.tar` & `jarvis_orm-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,10 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 jarvis_orm-0.0.2/src/jarvis_orm/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 jarvis_orm-0.0.2/src/jarvis_orm/commands/__init__.py
--rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 jarvis_orm-0.0.2/src/jarvis_orm/commands/commands.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 jarvis_orm-0.0.2/src/jarvis_orm/commands/parse.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jarvis_orm-0.0.2/src/jarvis_orm/core/__init__.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 jarvis_orm-0.0.2/src/jarvis_orm/core/engine.py
--rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 jarvis_orm-0.0.2/src/jarvis_orm/core/model.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 jarvis_orm-0.0.2/src/jarvis_orm/core/utilities.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 jarvis_orm-0.0.2/LICENSE
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jarvis_orm-0.0.2/README.md
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 jarvis_orm-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 jarvis_orm-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 jarvis_orm-0.0.3/src/jarvis_orm/__init__.py
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 jarvis_orm-0.0.3/src/jarvis_orm/commands.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 jarvis_orm-0.0.3/src/jarvis_orm/engine.py
+-rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 jarvis_orm-0.0.3/src/jarvis_orm/model.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 jarvis_orm-0.0.3/src/jarvis_orm/parse.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 jarvis_orm-0.0.3/src/jarvis_orm/utilities.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 jarvis_orm-0.0.3/LICENSE
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jarvis_orm-0.0.3/README.md
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 jarvis_orm-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 jarvis_orm-0.0.3/PKG-INFO
```

### Comparing `jarvis_orm-0.0.2/src/jarvis_orm/commands/commands.py` & `jarvis_orm-0.0.3/src/jarvis_orm/commands.py`

 * *Files identical despite different names*

### Comparing `jarvis_orm-0.0.2/src/jarvis_orm/commands/parse.py` & `jarvis_orm-0.0.3/src/jarvis_orm/parse.py`

 * *Files identical despite different names*

### Comparing `jarvis_orm-0.0.2/src/jarvis_orm/core/engine.py` & `jarvis_orm-0.0.3/src/jarvis_orm/engine.py`

 * *Files identical despite different names*

### Comparing `jarvis_orm-0.0.2/src/jarvis_orm/core/model.py` & `jarvis_orm-0.0.3/src/jarvis_orm/model.py`

 * *Files identical despite different names*

### Comparing `jarvis_orm-0.0.2/src/jarvis_orm/core/utilities.py` & `jarvis_orm-0.0.3/src/jarvis_orm/utilities.py`

 * *Files identical despite different names*

### Comparing `jarvis_orm-0.0.2/LICENSE` & `jarvis_orm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jarvis_orm-0.0.2/pyproject.toml` & `jarvis_orm-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jarvis-orm"
-version = "0.0.2"
+version = "0.0.3"
 requires-python = ">=3.10"
 authors = [
   {name = "Luke Jarvis", email = "jarvislukeldj@gmail.com"},
 ]
 maintainers = [
   {name = "Luke Jarvis", email = "jarvislukeldj@gmail.com"}
 ]
```

### Comparing `jarvis_orm-0.0.2/PKG-INFO` & `jarvis_orm-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jarvis-orm
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python Object-Relational Mapping
 Project-URL: Homepage, https://github.com/jarvisluke/jarvis-orm
 Project-URL: Repository, https://github.com/jarvisluke/jarvis-orm.git
 Project-URL: Bug Tracker, https://github.com/jarvisluke/jarvis-orm/issues
 Project-URL: Changelog, https://github.com/me/jarvis-orm/blob/master/CHANGELOG.md
 Author-email: Luke Jarvis <jarvislukeldj@gmail.com>
 Maintainer-email: Luke Jarvis <jarvislukeldj@gmail.com>
```

