# Comparing `tmp/dataspecs-0.3.0.tar.gz` & `tmp/dataspecs-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataspecs-0.3.0.tar", max compression
+gzip compressed data, was "dataspecs-0.4.0.tar", max compression
```

## Comparing `dataspecs-0.3.0.tar` & `dataspecs-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1076 2024-04-16 15:38:02.824623 dataspecs-0.3.0/LICENSE
--rw-r--r--   0        0        0      876 2024-04-16 15:38:02.824623 dataspecs-0.3.0/README.md
--rw-r--r--   0        0        0      344 2024-04-16 15:38:02.824623 dataspecs-0.3.0/dataspecs/__init__.py
--rw-r--r--   0        0        0      111 2024-04-16 15:38:02.824623 dataspecs-0.3.0/dataspecs/core/__init__.py
--rw-r--r--   0        0        0     5119 2024-04-16 15:38:02.824623 dataspecs-0.3.0/dataspecs/core/api.py
--rw-r--r--   0        0        0     5109 2024-04-16 15:38:02.824623 dataspecs-0.3.0/dataspecs/core/specs.py
--rw-r--r--   0        0        0     2938 2024-04-16 15:38:02.824623 dataspecs-0.3.0/dataspecs/core/typing.py
--rw-r--r--   0        0        0      174 2024-04-16 15:38:02.824623 dataspecs-0.3.0/dataspecs/extras/__init__.py
--rw-r--r--   0        0        0     1406 2024-04-16 15:38:02.824623 dataspecs-0.3.0/dataspecs/extras/replacement.py
--rw-r--r--   0        0        0        0 2024-04-16 15:38:02.824623 dataspecs-0.3.0/dataspecs/py.typed
--rw-r--r--   0        0        0      891 2024-04-16 15:38:02.824623 dataspecs-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 dataspecs-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-20 18:37:57.608342 dataspecs-0.4.0/LICENSE
+-rw-r--r--   0        0        0      876 2024-04-20 18:37:57.608342 dataspecs-0.4.0/README.md
+-rw-r--r--   0        0        0      344 2024-04-20 18:37:57.608342 dataspecs-0.4.0/dataspecs/__init__.py
+-rw-r--r--   0        0        0      111 2024-04-20 18:37:57.608342 dataspecs-0.4.0/dataspecs/core/__init__.py
+-rw-r--r--   0        0        0     5119 2024-04-20 18:37:57.612342 dataspecs-0.4.0/dataspecs/core/api.py
+-rw-r--r--   0        0        0     5109 2024-04-20 18:37:57.612342 dataspecs-0.4.0/dataspecs/core/specs.py
+-rw-r--r--   0        0        0     2938 2024-04-20 18:37:57.612342 dataspecs-0.4.0/dataspecs/core/typing.py
+-rw-r--r--   0        0        0      265 2024-04-20 18:37:57.612342 dataspecs-0.4.0/dataspecs/extras/__init__.py
+-rw-r--r--   0        0        0     1484 2024-04-20 18:37:57.612342 dataspecs-0.4.0/dataspecs/extras/formatting.py
+-rw-r--r--   0        0        0     1424 2024-04-20 18:37:57.612342 dataspecs-0.4.0/dataspecs/extras/replacing.py
+-rw-r--r--   0        0        0        0 2024-04-20 18:37:57.612342 dataspecs-0.4.0/dataspecs/py.typed
+-rw-r--r--   0        0        0      891 2024-04-20 18:37:57.612342 dataspecs-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 dataspecs-0.4.0/PKG-INFO
```

### Comparing `dataspecs-0.3.0/LICENSE` & `dataspecs-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataspecs-0.3.0/README.md` & `dataspecs-0.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 [![Tests](https://img.shields.io/github/actions/workflow/status/astropenguin/dataspecs/tests.yaml?label=Tests&style=flat-square)](https://github.com/astropenguin/dataspecs/actions)
 
 Data specifications by data classes
 
 ## Installation
 
 ```shell
-pip install dataspecs==0.3.0
+pip install dataspecs==0.4.0
 ```
```

### Comparing `dataspecs-0.3.0/dataspecs/core/api.py` & `dataspecs-0.4.0/dataspecs/core/api.py`

 * *Files identical despite different names*

### Comparing `dataspecs-0.3.0/dataspecs/core/specs.py` & `dataspecs-0.4.0/dataspecs/core/specs.py`

 * *Files identical despite different names*

### Comparing `dataspecs-0.3.0/dataspecs/core/typing.py` & `dataspecs-0.4.0/dataspecs/core/typing.py`

 * *Files identical despite different names*

### Comparing `dataspecs-0.3.0/dataspecs/extras/replacement.py` & `dataspecs-0.4.0/dataspecs/extras/replacing.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 # constants
 class Tag(TagBase):
     ID = auto()
     OF = auto()
     SKIPIF = auto()
 
 
-@dataclass
+@dataclass(frozen=True)
 class Replace:
     """Annotation for replacer specs."""
 
     id: Annotated[StrPath, Tag.ID]
     """ID of data spec(s) to be replaced."""
 
     of: Annotated[str, Tag.OF] = "data"
     """Name of data spec attribute to be replaced."""
 
     skipif: Annotated[Any, Tag.SKIPIF] = None
-    """Sentinel value for skipping replacements."""
+    """Sentinel value for which replacing is skipped."""
 
 
 def replace(specs: Specs[TSpec], /) -> Specs[TSpec]:
     """Replace data spec attributes by replacer specs."""
     new = specs.copy()
 
     for replacer in specs:
```

### Comparing `dataspecs-0.3.0/pyproject.toml` & `dataspecs-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataspecs"
-version = "0.3.0"
+version = "0.4.0"
 description = "Data specifications by data classes"
 authors = ["Akio Taniguchi <taniguchi@a.phys.nagoya-u.ac.jp>"]
 documentation = "https://astropenguin.github.io/dataspecs/"
 homepage = "https://github.com/astropenguin/dataspecs/"
 keywords = ["dataclasses", "specifications", "typing"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `dataspecs-0.3.0/PKG-INFO` & `dataspecs-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataspecs
-Version: 0.3.0
+Version: 0.4.0
 Summary: Data specifications by data classes
 Home-page: https://github.com/astropenguin/dataspecs/
 License: MIT
 Keywords: dataclasses,specifications,typing
 Author: Akio Taniguchi
 Author-email: taniguchi@a.phys.nagoya-u.ac.jp
 Requires-Python: >=3.9,<3.13
@@ -27,10 +27,10 @@
 [![Tests](https://img.shields.io/github/actions/workflow/status/astropenguin/dataspecs/tests.yaml?label=Tests&style=flat-square)](https://github.com/astropenguin/dataspecs/actions)
 
 Data specifications by data classes
 
 ## Installation
 
 ```shell
-pip install dataspecs==0.3.0
+pip install dataspecs==0.4.0
 ```
```

