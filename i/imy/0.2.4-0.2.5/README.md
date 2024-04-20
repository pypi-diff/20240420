# Comparing `tmp/imy-0.2.4.tar.gz` & `tmp/imy-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imy-0.2.4.tar", max compression
+gzip compressed data, was "imy-0.2.5.tar", max compression
```

## Comparing `imy-0.2.4.tar` & `imy-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.2.4/LICENSE
--rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.2.4/README.md
--rw-r--r--   0        0        0        0 2024-04-08 18:10:47.446922 imy-0.2.4/imy/__init__.py
--rw-r--r--   0        0        0     6715 2024-04-07 17:04:35.179837 imy-0.2.4/imy/assets.py
--rw-r--r--   0        0        0     6011 2024-03-27 19:30:58.658694 imy-0.2.4/imy/async_utils.py
--rw-r--r--   0        0        0     9815 2024-04-01 09:46:55.130648 imy-0.2.4/imy/config.py
--rw-r--r--   0        0        0       71 2024-04-18 06:50:34.243007 imy-0.2.4/imy/docstrings/__init__.py
--rw-r--r--   0        0        0     5072 2024-04-18 07:34:38.648724 imy-0.2.4/imy/docstrings/data_models.py
--rw-r--r--   0        0        0    16728 2024-04-18 07:37:22.300844 imy-0.2.4/imy/docstrings/parsers.py
--rw-r--r--   0        0        0     8572 2024-04-10 14:07:52.133967 imy-0.2.4/imy/inject.py
--rw-r--r--   0        0        0    13613 2024-04-10 14:10:43.230681 imy-0.2.4/imy/logs.py
--rw-r--r--   0        0        0     2167 2024-04-11 21:48:52.558560 imy-0.2.4/imy/package_metadata.py
--rw-r--r--   0        0        0      754 2024-04-18 18:57:24.091110 imy-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 imy-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.2.5/LICENSE
+-rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.2.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 18:10:47.446922 imy-0.2.5/imy/__init__.py
+-rw-r--r--   0        0        0     6715 2024-04-07 17:04:35.179837 imy-0.2.5/imy/assets.py
+-rw-r--r--   0        0        0     6011 2024-03-27 19:30:58.658694 imy-0.2.5/imy/async_utils.py
+-rw-r--r--   0        0        0     9815 2024-04-01 09:46:55.130648 imy-0.2.5/imy/config.py
+-rw-r--r--   0        0        0       71 2024-04-18 06:50:34.243007 imy-0.2.5/imy/docstrings/__init__.py
+-rw-r--r--   0        0        0     5072 2024-04-18 07:34:38.648724 imy-0.2.5/imy/docstrings/data_models.py
+-rw-r--r--   0        0        0    16728 2024-04-19 11:26:09.630358 imy-0.2.5/imy/docstrings/parsers.py
+-rw-r--r--   0        0        0     8572 2024-04-10 14:07:52.133967 imy-0.2.5/imy/inject.py
+-rw-r--r--   0        0        0    13613 2024-04-10 14:10:43.230681 imy-0.2.5/imy/logs.py
+-rw-r--r--   0        0        0     3185 2024-04-19 18:44:30.576908 imy-0.2.5/imy/package_metadata.py
+-rw-r--r--   0        0        0      754 2024-04-19 18:58:35.067677 imy-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 imy-0.2.5/PKG-INFO
```

### Comparing `imy-0.2.4/LICENSE` & `imy-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `imy-0.2.4/imy/assets.py` & `imy-0.2.5/imy/assets.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.4/imy/async_utils.py` & `imy-0.2.5/imy/async_utils.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.4/imy/config.py` & `imy-0.2.5/imy/config.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.4/imy/docstrings/data_models.py` & `imy-0.2.5/imy/docstrings/data_models.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.4/imy/docstrings/parsers.py` & `imy-0.2.5/imy/docstrings/parsers.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.4/imy/inject.py` & `imy-0.2.5/imy/inject.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.4/imy/logs.py` & `imy-0.2.5/imy/logs.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.4/imy/package_metadata.py` & `imy-0.2.5/imy/package_metadata.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Utilities for getting metadata about your own package.
 """
 
 import importlib.metadata
 import inspect
 import sys
 from pathlib import Path
+from typing import *  # type: ignore
 
 
 def _get_root_directory(caller: inspect.FrameInfo) -> Path:
     """
     Return the root directory of the calling module, accounting for submodules.
 
     For example, if the calling module is `foo.bar.baz`, and `foo` is located
@@ -27,14 +28,38 @@
 
     for _ in range(depth):
         caller_path = caller_path.parent
 
     return caller_path
 
 
+def _find_pyproject_toml(module_directory: Path) -> Path:
+    """
+    Attempts to locate a project's `pyproject.toml` file. It will look in common
+    locations and return the path if found, or raise a `FileNotFoundError` if
+    not.
+    """
+
+    def _iter_toml_paths() -> Iterable[Path]:
+        # In a typicical project the toml is right next to the module
+        yield module_directory.parent / "pyproject.toml"
+
+        # However, some projects have a `src` directory
+        if module_directory.parent.name == "src":
+            yield module_directory.parent.parent / "pyproject.toml"
+
+    # Try to find the toml
+    for toml_path in _iter_toml_paths():
+        if toml_path.exists():
+            return toml_path
+
+    # Nothing was found
+    raise FileNotFoundError("Could not find `pyproject.toml`")
+
+
 def get_package_version(own_package_pypi_name: str) -> str:
     """
     Determine the version of **the calling package**. `own_package_pypi_name` is
     the name of the package, as you would type to install it from pypi.
 
     You can **not use this function to look up any packages other than your
     own**.
@@ -47,25 +72,33 @@
         pass
 
     # While the approach above is clean, it fails during development. In that
     # case, read the version from the `pyproject.toml` file.
     import tomllib
 
     caller_frame = inspect.stack()[1]
-    toml_path = _get_root_directory(caller_frame).parent / "pyproject.toml"
+    toml_path = _find_pyproject_toml(_get_root_directory(caller_frame))
 
     try:
         with open(toml_path, "rb") as f:
             toml_contents = tomllib.load(f)
 
     except FileNotFoundError:
         raise RuntimeError(f"Cannot find `pyproject.toml` at `{toml_path}`") from None
 
     except tomllib.TOMLDecodeError as e:
         raise RuntimeError(f"`{toml_path}` is invalid TOML: {e}") from None
 
+    # The version can be stored in different places, depending on the tooling
+    try:
+        return toml_contents["project"]["version"]
+    except KeyError:
+        pass
+
     try:
         return toml_contents["tool"]["poetry"]["version"]
     except KeyError:
-        raise RuntimeError(
-            f"`{toml_path}` does not contain a `tool.poetry.version` field"
-        ) from None
+        pass
+
+    raise RuntimeError(
+        f"`{toml_path}` does not contain a `tool.poetry.version` field"
+    ) from None
```

### Comparing `imy-0.2.4/pyproject.toml` & `imy-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "imy"
-version = "0.2.4"
+version = "0.2.5"
 description = "Random utilities I can't go without"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
 license = "MIT"
 repository = "https://gitlab.com/Vivern/i-miss-you"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `imy-0.2.4/PKG-INFO` & `imy-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imy
-Version: 0.2.4
+Version: 0.2.5
 Summary: Random utilities I can't go without
 Home-page: https://gitlab.com/Vivern/i-miss-you
 License: MIT
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

