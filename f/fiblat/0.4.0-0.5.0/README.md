# Comparing `tmp/fiblat-0.4.0.tar.gz` & `tmp/fiblat-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiblat-0.4.0.tar", max compression
+gzip compressed data, was "fiblat-0.5.0.tar", max compression
```

## Comparing `fiblat-0.4.0.tar` & `fiblat-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     1070 2019-12-15 22:36:29.090443 fiblat-0.4.0/LICENSE
--rw-r--r--   0        0        0      903 2023-07-26 13:42:05.248327 fiblat-0.4.0/README.md
--rw-r--r--   0        0        0       84 2023-04-19 04:57:59.345473 fiblat-0.4.0/fiblat/__init__.py
--rwxr-xr-x   0        0        0     1029 2022-04-08 04:55:51.541446 fiblat-0.4.0/fiblat/_cube_lattice.py
--rwxr-xr-x   0        0        0      985 2022-04-08 01:50:06.811446 fiblat-0.4.0/fiblat/_irrational.py
--rw-r--r--   0        0        0     2631 2022-04-11 03:59:03.161585 fiblat-0.4.0/fiblat/_sphere_lattice.py
--rw-r--r--   0        0        0      597 2023-07-26 13:43:03.488328 fiblat-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1626 1970-01-01 00:00:00.000000 fiblat-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-19 02:01:01.854741 fiblat-0.5.0/LICENSE
+-rw-r--r--   0        0        0      903 2024-04-19 02:01:01.854860 fiblat-0.5.0/README.md
+-rw-r--r--   0        0        0       84 2024-04-19 02:01:01.855017 fiblat-0.5.0/fiblat/__init__.py
+-rw-r--r--   0        0        0      946 2024-04-20 00:29:21.599537 fiblat-0.5.0/fiblat/_cube_lattice.py
+-rw-r--r--   0        0        0      816 2024-04-20 00:15:59.034630 fiblat-0.5.0/fiblat/_irrational.py
+-rw-r--r--   0        0        0     3642 2024-04-20 15:22:35.139077 fiblat-0.5.0/fiblat/_sphere_lattice.py
+-rw-r--r--   0        0        0      643 2024-04-20 18:15:59.165859 fiblat-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1734 1970-01-01 00:00:00.000000 fiblat-0.5.0/PKG-INFO
```

### Comparing `fiblat-0.4.0/LICENSE` & `fiblat-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fiblat-0.4.0/README.md` & `fiblat-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `fiblat-0.4.0/fiblat/_cube_lattice.py` & `fiblat-0.5.0/fiblat/_cube_lattice.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from itertools import chain, islice, count
 from typing import Iterator, List, Optional, Tuple
 import numpy as np
+import numba as nb
 
-from ._irrational import root_primes
+from ._irrational import n_primes
 
 
-def cube_lattice(
-    dim: int, num_points: int, *, irrationals: Optional[Iterator[float]] = None
-) -> np.ndarray:
+@nb.njit(nb.float64[:, :](nb.int64, nb.int64), fastmath=True, error_model="numpy")
+def cube_lattice(dim: int, num_points: int) -> np.ndarray:  # pragma: nocover
     """Generate num_points points over the dim dimensional cube
 
     Generates `num_points` roughly evenly from the `[0, 1]^dim`.
 
     Parameters
     ----------
     dim : dimension of cube to generate points in
     num_points : the number of points to generate
-    irrationals : an iterator of at least `dim-1` irrational numbers, if
-        omitted the square roots of the primes are used
     """
     if dim < 1:
-        raise ValueError("dimension must be greater than zero")
-    if num_points < 1:
-        raise ValueError("must request at least one point")
-    mult_iter = root_primes() if irrationals is None else irrationals
-    mults = np.fromiter(chain([1 / num_points], mult_iter), float, dim)
+        raise ValueError(f"dimension must be greater than zero: {dim}")
+    elif num_points < 1:
+        raise ValueError(f"must request at least one point: {num_points}")
+    rest = np.sqrt(n_primes(dim - 1))
+    mults = np.concatenate((np.full(1, 1 / num_points), rest))
     return (mults * np.arange(num_points)[:, None]) % 1.0
```

### Comparing `fiblat-0.4.0/pyproject.toml` & `fiblat-0.5.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "fiblat"
-version = "0.4.0"
+version = "0.5.0"
 description = "A package for generating evenly distributed points on a sphere"
 repository = "https://github.com/erikbrinkman/fibonacci_lattice"
 authors = ["Erik Brinkman <erik.brinkman@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.pytest.ini_options]
-addopts = "--cov fiblat --cov-report term-missing"
+addopts = "--cov fiblat --cov-report term-missing -m 'not long'"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-numba = "^0.57"
-numpy = "^1.24"
+numba = "^0.59.1"
+numpy = "^1.26.4"
+pytest-benchmark = "^4.0.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.4"
-pytest-cov = "^4.1"
+pytest = "^8.1"
+pytest-cov = "^5.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fiblat-0.4.0/PKG-INFO` & `fiblat-0.5.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: fiblat
-Version: 0.4.0
+Version: 0.5.0
 Summary: A package for generating evenly distributed points on a sphere
 Home-page: https://github.com/erikbrinkman/fibonacci_lattice
 License: MIT
 Author: Erik Brinkman
 Author-email: erik.brinkman@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numba (>=0.57,<0.58)
-Requires-Dist: numpy (>=1.24,<2.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: numba (>=0.59.1,<0.60.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: pytest-benchmark (>=4.0.0,<5.0.0)
 Project-URL: Repository, https://github.com/erikbrinkman/fibonacci_lattice
 Description-Content-Type: text/markdown
 
 Fibonacci Lattice
 =================
 [![pypi](https://img.shields.io/pypi/v/fiblat)](https://pypi.org/project/fiblat/)
 [![build](https://github.com/erikbrinkman/fibonacci_lattice/actions/workflows/build.yml/badge.svg)](https://github.com/erikbrinkman/fibonacci_lattice/actions/workflows/build.yml)
```

