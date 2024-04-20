# Comparing `tmp/camel_converter-3.1.1.tar.gz` & `tmp/camel_converter-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camel_converter-3.1.1.tar", max compression
+gzip compressed data, was "camel_converter-3.1.2.tar", max compression
```

## Comparing `camel_converter-3.1.1.tar` & `camel_converter-3.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-11-27 00:10:18.267752 camel_converter-3.1.1/LICENSE
--rw-r--r--   0        0        0     4290 2023-11-27 00:10:18.267752 camel_converter-3.1.1/README.md
--rw-r--r--   0        0        0     4890 2023-11-27 00:10:18.267752 camel_converter-3.1.1/camel_converter/__init__.py
--rw-r--r--   0        0        0     1128 2023-11-27 00:10:18.267752 camel_converter-3.1.1/camel_converter/decorators.py
--rw-r--r--   0        0        0        0 2023-11-27 00:10:18.267752 camel_converter-3.1.1/camel_converter/py.typed
--rw-r--r--   0        0        0     1529 2023-11-27 00:10:18.267752 camel_converter-3.1.1/camel_converter/pydantic_base.py
--rw-r--r--   0        0        0     1888 2023-11-27 00:10:18.267752 camel_converter-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     5405 1970-01-01 00:00:00.000000 camel_converter-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-20 01:04:25.432983 camel_converter-3.1.2/LICENSE
+-rw-r--r--   0        0        0     4290 2024-04-20 01:04:25.432983 camel_converter-3.1.2/README.md
+-rw-r--r--   0        0        0     4890 2024-04-20 01:04:25.432983 camel_converter-3.1.2/camel_converter/__init__.py
+-rw-r--r--   0        0        0     1128 2024-04-20 01:04:25.432983 camel_converter-3.1.2/camel_converter/decorators.py
+-rw-r--r--   0        0        0        0 2024-04-20 01:04:25.432983 camel_converter-3.1.2/camel_converter/py.typed
+-rw-r--r--   0        0        0     1585 2024-04-20 01:04:25.432983 camel_converter-3.1.2/camel_converter/pydantic_base.py
+-rw-r--r--   0        0        0     1911 2024-04-20 01:04:25.432983 camel_converter-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5405 1970-01-01 00:00:00.000000 camel_converter-3.1.2/PKG-INFO
```

### Comparing `camel_converter-3.1.1/LICENSE` & `camel_converter-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `camel_converter-3.1.1/README.md` & `camel_converter-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `camel_converter-3.1.1/camel_converter/__init__.py` & `camel_converter-3.1.2/camel_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_converter-3.1.1/camel_converter/decorators.py` & `camel_converter-3.1.2/camel_converter/decorators.py`

 * *Files identical despite different names*

### Comparing `camel_converter-3.1.1/camel_converter/pydantic_base.py` & `camel_converter-3.1.2/camel_converter/pydantic_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from warnings import warn
 
 try:
     import pydantic  # type: ignore
-except ImportError:
-    raise ImportError("camel-converter must be installed with the pydantic extra to use this class")
+except ImportError as e:
+    raise ImportError(
+        "camel-converter must be installed with the pydantic extra to use this class"
+    ) from e
 
 from camel_converter import to_camel
 
 
 class CamelBase(pydantic.BaseModel):
     """A Pydantic model that provides a base configuration for conveting between camel and snake case.
 
@@ -20,14 +22,15 @@
         # Still check the version as a fail safe incase __version__ gets added to verion 1.
         if int(pydantic.__version__[:1]) >= 2:  # type: ignore[attr-defined]
             model_config = pydantic.ConfigDict(alias_generator=to_camel, populate_by_name=True)  # type: ignore[attr-defined]
         else:  # pragma: no cover
             warn(
                 "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
                 DeprecationWarning,
+                stacklevel=2,
             )
 
             # Raise an AttributeError to match the AttributeError on __version__ because in either
             # case we need to get to the same place.
             raise AttributeError
     except AttributeError:  # pragma: no cover
```

### Comparing `camel_converter-3.1.1/pyproject.toml` & `camel_converter-3.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "camel-converter"
-version = "3.1.1"
+version = "3.1.2"
 description = "Converts a string from snake case to camel case or camel case to snake case"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/camel-converter"
 homepage = "https://github.com/sanders41/camel-converter"
 documentation = "https://github.com/sanders41/camel-converter"
@@ -50,18 +50,23 @@
 disallow_untyped_defs = true
 
 [[tool.mypy.overrides]]
 module = ["tests.*"]
 disallow_untyped_defs = false
 
 [tool.ruff]
-select=["E", "F", "T201", "T203", "I001", "UP"]
+line-length = 100
+fix = true
+target-version = "py38"
+
+[tool.ruff.lint]
+select=["E", "B", "F", "T201", "T203", "I001", "UP"]
 ignore=[
-  "E501",
   # Recommened ignores by ruff when using formatter
+  "E501",
   "W191",
   "E111",
   "E114",
   "E117",
   "D206",
   "D300",
   "Q000",
@@ -69,10 +74,7 @@
   "Q002",
   "Q003",
   "COM812",
   "COM819",
   "ISC001",
   "ISC002",
 ]
-line-length = 100
-fix = true
-target-version = "py38"
```

### Comparing `camel_converter-3.1.1/PKG-INFO` & `camel_converter-3.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camel-converter
-Version: 3.1.1
+Version: 3.1.2
 Summary: Converts a string from snake case to camel case or camel case to snake case
 Home-page: https://github.com/sanders41/camel-converter
 License: MIT
 Keywords: python,pydantic
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.8,<4.0
```

