# Comparing `tmp/class_singledispatch-1.1.1.tar.gz` & `tmp/class_singledispatch-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "class_singledispatch-1.1.1.tar", max compression
+gzip compressed data, was "class_singledispatch-1.2.0.tar", max compression
```

## Comparing `class_singledispatch-1.1.1.tar` & `class_singledispatch-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1092 2024-04-14 23:00:27.308082 class_singledispatch-1.1.1/LICENSE
--rw-r--r--   0        0        0     4997 2024-04-14 23:00:27.308082 class_singledispatch-1.1.1/README.md
--rw-r--r--   0        0        0     5841 2024-04-14 23:00:27.308082 class_singledispatch-1.1.1/class_singledispatch/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 23:00:27.308082 class_singledispatch-1.1.1/class_singledispatch/py.typed
--rw-r--r--   0        0        0     5714 2024-04-14 23:00:27.308082 class_singledispatch-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     6037 1970-01-01 00:00:00.000000 class_singledispatch-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-04-20 20:58:52.285433 class_singledispatch-1.2.0/LICENSE
+-rw-r--r--   0        0        0     5253 2024-04-20 20:58:52.285433 class_singledispatch-1.2.0/README.md
+-rw-r--r--   0        0        0     5873 2024-04-20 20:58:52.285433 class_singledispatch-1.2.0/class_singledispatch/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 20:58:52.285433 class_singledispatch-1.2.0/class_singledispatch/py.typed
+-rw-r--r--   0        0        0     5789 2024-04-20 20:58:52.289433 class_singledispatch-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6356 1970-01-01 00:00:00.000000 class_singledispatch-1.2.0/PKG-INFO
```

### Comparing `class_singledispatch-1.1.1/LICENSE` & `class_singledispatch-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `class_singledispatch-1.1.1/README.md` & `class_singledispatch-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![Coverage](https://coverage-badge.samuelcolvin.workers.dev/bswck/class_singledispatch.svg)](https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/class_singledispatch)
 [![Documentation Status](https://readthedocs.org/projects/class-singledispatch/badge/?version=latest)](https://class-singledispatch.readthedocs.io/en/latest/?badge=latest)
 
 A ``singledispatch()`` for arguments that are classes annotated as specific types.
 
 Inspired by https://github.com/python/cpython/issues/100623.
 
-# A simple example
+# A Simple Example
 Use `functools.singledispatch` to singledispatch classes as parameters.
 
 While `functools.singledispatch` examines the class of the first user argument,
 `class_singledispatch` uses the first argument as the class itself and performs
 the same task with it as `functools.singledispatch`.
 
 ```python
@@ -51,14 +51,19 @@
 
 # Installation
 You might simply install it with pip:
 
 ```shell
 pip install class-singledispatch
 ```
+> [!Note]
+> `class-singledispatch` supports modern type hinting.<br/>
+> To use [PEP 585](https://peps.python.org/pep-0585/)
+> or [PEP 604](https://peps.python.org/pep-0604/) annotations on Python <3.10, install
+> `class-singledispatch[modern-type-hints]`.
 
 If you use [Poetry](https://python-poetry.org/), then you might want to run:
 
 ```shell
 poetry add class-singledispatch
 ```
```

### Comparing `class_singledispatch-1.1.1/class_singledispatch/__init__.py` & `class_singledispatch-1.2.0/class_singledispatch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     from typing import ParamSpec
 
     OldFashionGenericAlias = type(Type[object])
 
 try:
     from eval_type_backport import ForwardRef  # type: ignore  # noqa: PGH003
 except ImportError:  # pragma: no cover
-    from typing import ForwardRef
+    from typing import ForwardRef  # type: ignore  # noqa: PGH003
 
 
 __all__ = (
     "class_singledispatch",
     "resolve_annotated_type",
 )
```

### Comparing `class_singledispatch-1.1.1/pyproject.toml` & `class_singledispatch-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was generated from skeleton-ci/skeleton-python@0.0.2rc-218-g8123b8a.
 # Instead of changing this particular file, you might want to alter the template:
 # https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-218-g8123b8a/project/pyproject.toml.jinja
 
 [tool.poetry]
 name = "class_singledispatch"
-version = "1.1.1"
+version = "1.2.0"
 description = "A ``singledispatch()`` for arguments that are classes annotated as specific types."
 authors = ["bswck <bartoszpiotrslawecki@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "class_singledispatch/" }]
 homepage = "https://github.com/bswck/class_singledispatch"
 
@@ -16,14 +16,15 @@
 Documentation = "https://class-singledispatch.readthedocs.io/en/latest/"
 Issues = "https://github.com/bswck/class_singledispatch/issues"
 Distribution = "https://pypi.org/project/class-singledispatch/"
 Coverage = "https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/class_singledispatch"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
+eval-type-backport = {version = ">=0.2.0", extras = ["modern-type-hints"]}
 
 [tool.poetry.group.dev.dependencies]
 
 [tool.poetry.group.dev-skeleton.dependencies]
 # This dependency group was generated from skeleton-ci/skeleton-python@0.0.2rc-218-g8123b8a.
 # Instead of changing this particular file, you might want to alter the template:
 # https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-218-g8123b8a/project/pyproject.toml.jinja
```

### Comparing `class_singledispatch-1.1.1/PKG-INFO` & `class_singledispatch-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: class_singledispatch
-Version: 1.1.1
+Version: 1.2.0
 Summary: A ``singledispatch()`` for arguments that are classes annotated as specific types.
 Home-page: https://github.com/bswck/class_singledispatch
 License: MIT
 Author: bswck
 Author-email: bartoszpiotrslawecki@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: eval-type-backport[modern-type-hints] (>=0.2.0)
 Project-URL: Coverage, https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/class_singledispatch
 Project-URL: Documentation, https://class-singledispatch.readthedocs.io/en/latest/
 Project-URL: Distribution, https://pypi.org/project/class-singledispatch/
 Project-URL: Issues, https://github.com/bswck/class_singledispatch/issues
 Description-Content-Type: text/markdown
 
 # <div align="center">class_singledispatch<br>[![skeleton](https://img.shields.io/badge/0.0.2rc–218–g8123b8a-skeleton?label=%F0%9F%92%80%20skeleton-ci/skeleton-python&labelColor=black&color=grey&link=https%3A//github.com/skeleton-ci/skeleton-python)](https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-218-g8123b8a) [![Supported Python versions](https://img.shields.io/pypi/pyversions/class-singledispatch.svg?logo=python&label=Python)](https://pypi.org/project/class-singledispatch/) [![Package version](https://img.shields.io/pypi/v/class-singledispatch?label=PyPI)](https://pypi.org/project/class-singledispatch/)</div>
@@ -26,15 +27,15 @@
 [![Coverage](https://coverage-badge.samuelcolvin.workers.dev/bswck/class_singledispatch.svg)](https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/class_singledispatch)
 [![Documentation Status](https://readthedocs.org/projects/class-singledispatch/badge/?version=latest)](https://class-singledispatch.readthedocs.io/en/latest/?badge=latest)
 
 A ``singledispatch()`` for arguments that are classes annotated as specific types.
 
 Inspired by https://github.com/python/cpython/issues/100623.
 
-# A simple example
+# A Simple Example
 Use `functools.singledispatch` to singledispatch classes as parameters.
 
 While `functools.singledispatch` examines the class of the first user argument,
 `class_singledispatch` uses the first argument as the class itself and performs
 the same task with it as `functools.singledispatch`.
 
 ```python
@@ -73,14 +74,19 @@
 
 # Installation
 You might simply install it with pip:
 
 ```shell
 pip install class-singledispatch
 ```
+> [!Note]
+> `class-singledispatch` supports modern type hinting.<br/>
+> To use [PEP 585](https://peps.python.org/pep-0585/)
+> or [PEP 604](https://peps.python.org/pep-0604/) annotations on Python <3.10, install
+> `class-singledispatch[modern-type-hints]`.
 
 If you use [Poetry](https://python-poetry.org/), then you might want to run:
 
 ```shell
 poetry add class-singledispatch
 ```
```

