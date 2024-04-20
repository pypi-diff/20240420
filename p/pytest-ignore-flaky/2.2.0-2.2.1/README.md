# Comparing `tmp/pytest-ignore-flaky-2.2.0.tar.gz` & `tmp/pytest_ignore_flaky-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-ignore-flaky-2.2.0.tar", last modified: Mon Apr  8 07:29:47 2024, max compression
+gzip compressed data, was "pytest_ignore_flaky-2.2.1.tar", last modified: Sat Apr 20 01:51:29 2024, max compression
```

## Comparing `pytest-ignore-flaky-2.2.0.tar` & `pytest_ignore_flaky-2.2.1.tar`

### file list

```diff
@@ -1,16 +1,37 @@
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-08 07:29:47.903984 pytest-ignore-flaky-2.2.0/
--rw-r--r--   0 jaraco     (501) staff       (20)     1087 2024-04-07 22:10:00.000000 pytest-ignore-flaky-2.2.0/LICENSE
--rw-r--r--   0 jaraco     (501) staff       (20)     2746 2024-04-08 07:29:47.903912 pytest-ignore-flaky-2.2.0/PKG-INFO
--rw-r--r--   0 jaraco     (501) staff       (20)     1630 2024-04-08 07:21:54.000000 pytest-ignore-flaky-2.2.0/README.rst
--rw-r--r--   0 jaraco     (501) staff       (20)       85 2024-04-07 22:10:00.000000 pytest-ignore-flaky-2.2.0/pyproject.toml
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-08 07:29:47.903748 pytest-ignore-flaky-2.2.0/pytest_ignore_flaky.egg-info/
--rw-r--r--   0 jaraco     (501) staff       (20)     2746 2024-04-08 07:29:47.000000 pytest-ignore-flaky-2.2.0/pytest_ignore_flaky.egg-info/PKG-INFO
--rw-r--r--   0 jaraco     (501) staff       (20)      351 2024-04-08 07:29:47.000000 pytest-ignore-flaky-2.2.0/pytest_ignore_flaky.egg-info/SOURCES.txt
--rw-r--r--   0 jaraco     (501) staff       (20)        1 2024-04-08 07:29:47.000000 pytest-ignore-flaky-2.2.0/pytest_ignore_flaky.egg-info/dependency_links.txt
--rw-r--r--   0 jaraco     (501) staff       (20)       53 2024-04-08 07:29:47.000000 pytest-ignore-flaky-2.2.0/pytest_ignore_flaky.egg-info/entry_points.txt
--rw-r--r--   0 jaraco     (501) staff       (20)       12 2024-04-08 07:29:47.000000 pytest-ignore-flaky-2.2.0/pytest_ignore_flaky.egg-info/requires.txt
--rw-r--r--   0 jaraco     (501) staff       (20)       20 2024-04-08 07:29:47.000000 pytest-ignore-flaky-2.2.0/pytest_ignore_flaky.egg-info/top_level.txt
--rw-r--r--   0 jaraco     (501) staff       (20)     1346 2024-04-07 22:10:00.000000 pytest-ignore-flaky-2.2.0/pytest_ignore_flaky.py
--rw-r--r--   0 jaraco     (501) staff       (20)     1153 2024-04-08 07:29:47.904215 pytest-ignore-flaky-2.2.0/setup.cfg
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-08 07:29:47.903613 pytest-ignore-flaky-2.2.0/tests/
--rw-r--r--   0 jaraco     (501) staff       (20)     1365 2024-04-07 22:10:00.000000 pytest-ignore-flaky-2.2.0/tests/test_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:51:29.649450 pytest_ignore_flaky-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:51:29.645450 pytest_ignore_flaky-2.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:51:29.645450 pytest_ignore_flaky-2.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-20 01:51:29.649450 pytest_ignore_flaky-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:51:29.645450 pytest_ignore_flaky-2.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:51:29.649450 pytest_ignore_flaky-2.2.1/pytest_ignore_flaky/
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/pytest_ignore_flaky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:51:29.649450 pytest_ignore_flaky-2.2.1/pytest_ignore_flaky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-20 01:51:29.000000 pytest_ignore_flaky-2.2.1/pytest_ignore_flaky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-20 01:51:29.000000 pytest_ignore_flaky-2.2.1/pytest_ignore_flaky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:51:29.000000 pytest_ignore_flaky-2.2.1/pytest_ignore_flaky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-20 01:51:29.000000 pytest_ignore_flaky-2.2.1/pytest_ignore_flaky.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-20 01:51:29.000000 pytest_ignore_flaky-2.2.1/pytest_ignore_flaky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-20 01:51:29.000000 pytest_ignore_flaky-2.2.1/pytest_ignore_flaky.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 01:51:29.649450 pytest_ignore_flaky-2.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:51:29.649450 pytest_ignore_flaky-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/tests/sample succeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/tests/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-20 01:51:10.000000 pytest_ignore_flaky-2.2.1/tox.ini
```

### Comparing `pytest-ignore-flaky-2.2.0/LICENSE` & `pytest_ignore_flaky-2.2.1/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,17 @@
-
-
-The MIT License
-
-Copyright (c) 2015 Eduardo Naufel Schettino
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
+of this software and associated documentation files (the "Software"), to
+deal in the Software without restriction, including without limitation the
+rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
+sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in
 all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
+IN THE SOFTWARE.
```

### Comparing `pytest-ignore-flaky-2.2.0/PKG-INFO` & `pytest_ignore_flaky-2.2.1/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,25 @@
-Metadata-Version: 2.1
-Name: pytest-ignore-flaky
-Version: 2.2.0
-Summary: ignore failures from flaky tests (pytest plugin)
-Home-page: https://github.com/coherent-oss/pytest-ignore-flaky
-Author: Eduardo Naufel Schettino, Marcos Alfredo Camargo Leal Pinto
-Author-email: schettino72@gmail.com, marcos.alfredo@gmail.com
-Maintainer: Jason R. Coombs
-Maintainer-email: jaraco@jaraco.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.8
-License-File: LICENSE
-Requires-Dist: pytest>=6.0
-
 .. image:: https://img.shields.io/pypi/v/pytest-ignore-flaky.svg
-   :target: https://pypi.python.org/pypi/pytest-ignore-flaky
+   :target: https://pypi.org/project/pytest-ignore-flaky
 
 .. image:: https://img.shields.io/pypi/pyversions/pytest-ignore-flaky.svg
-   :target: https://pypi.python.org/pypi/pytest-ignore-flaky
 
 .. image:: https://github.com/coherent-oss/pytest-ignore-flaky/actions/workflows/main.yml/badge.svg
-   :target: https://github.com/coherent-oss/pytest-ignore-flaky/actions?query=workflow%3Atests
+   :target: https://github.com/coherent-oss/pytest-ignore-flaky/actions?query=workflow%3A%22tests%22
+   :alt: tests
+
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
+.. image:: https://readthedocs.org/projects/pytest-ignore-flaky/badge/?version=latest
+   :target: https://pytest-ignore-flaky.readthedocs.io/en/latest/?badge=latest
+
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
+   :target: https://blog.jaraco.com/skeleton
 
 
 pytest-ignore-flaky
 ====================
 
 ignore failures from flaky tests (pytest plugin)
```

### Comparing `pytest-ignore-flaky-2.2.0/pytest_ignore_flaky.py` & `pytest_ignore_flaky-2.2.1/pytest_ignore_flaky/__init__.py`

 * *Files identical despite different names*

