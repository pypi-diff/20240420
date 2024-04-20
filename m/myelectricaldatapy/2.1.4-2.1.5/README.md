# Comparing `tmp/myelectricaldatapy-2.1.4.tar.gz` & `tmp/myelectricaldatapy-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myelectricaldatapy-2.1.4.tar", last modified: Sat Apr 13 15:49:57 2024, max compression
+gzip compressed data, was "myelectricaldatapy-2.1.5.tar", last modified: Sat Apr 20 09:11:54 2024, max compression
```

## Comparing `myelectricaldatapy-2.1.4.tar` & `myelectricaldatapy-2.1.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.360177 myelectricaldatapy-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.352177 myelectricaldatapy-2.1.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.356177 myelectricaldatapy-2.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/.github/workflows/dependbot-auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.356177 myelectricaldatapy-2.1.4/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-13 15:49:57.360177 myelectricaldatapy-2.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.356177 myelectricaldatapy-2.1.4/myelectricaldatapy/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/myelectricaldatapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/myelectricaldatapy/analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/myelectricaldatapy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/myelectricaldatapy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/myelectricaldatapy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/myelectricaldatapy/myelectricaldata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/myelectricaldatapy/mypdl.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/myelectricaldatapy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.360177 myelectricaldatapy-2.1.4/myelectricaldatapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-13 15:49:57.000000 myelectricaldatapy-2.1.4/myelectricaldatapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-13 15:49:57.000000 myelectricaldatapy-2.1.4/myelectricaldatapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:49:57.000000 myelectricaldatapy-2.1.4/myelectricaldatapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-13 15:49:57.000000 myelectricaldatapy-2.1.4/myelectricaldatapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-13 15:49:57.000000 myelectricaldatapy-2.1.4/myelectricaldatapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:49:57.360177 myelectricaldatapy-2.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.356177 myelectricaldatapy-2.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/tests/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/tests/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/tests/test_load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:11:54.660608 myelectricaldatapy-2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:11:54.656608 myelectricaldatapy-2.1.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:11:54.656608 myelectricaldatapy-2.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/.github/workflows/dependbot-auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:11:54.656608 myelectricaldatapy-2.1.5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-20 09:11:54.660608 myelectricaldatapy-2.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:11:54.656608 myelectricaldatapy-2.1.5/myelectricaldatapy/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/myelectricaldatapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/myelectricaldatapy/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/myelectricaldatapy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/myelectricaldatapy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/myelectricaldatapy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/myelectricaldatapy/myelectricaldata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/myelectricaldatapy/mypdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/myelectricaldatapy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:11:54.660608 myelectricaldatapy-2.1.5/myelectricaldatapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-20 09:11:54.000000 myelectricaldatapy-2.1.5/myelectricaldatapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-20 09:11:54.000000 myelectricaldatapy-2.1.5/myelectricaldatapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 09:11:54.000000 myelectricaldatapy-2.1.5/myelectricaldatapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-20 09:11:54.000000 myelectricaldatapy-2.1.5/myelectricaldatapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-20 09:11:54.000000 myelectricaldatapy-2.1.5/myelectricaldatapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 09:11:54.660608 myelectricaldatapy-2.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:11:54.660608 myelectricaldatapy-2.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/tests/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/tests/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/tests/test_load_data.py
```

### Comparing `myelectricaldatapy-2.1.4/.github/dependabot.yml` & `myelectricaldatapy-2.1.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.4/.github/workflows/dependbot-auto-approve.yml` & `myelectricaldatapy-2.1.5/.github/workflows/dependbot-auto-approve.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.4/.github/workflows/lint.yml` & `myelectricaldatapy-2.1.5/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.4/.github/workflows/pythonpublish.yml` & `myelectricaldatapy-2.1.5/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.4/.github/workflows/release.yml` & `myelectricaldatapy-2.1.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.4/.gitignore` & `myelectricaldatapy-2.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.4/.pre-commit-config.yaml` & `myelectricaldatapy-2.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.4/LICENSE` & `myelectricaldatapy-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.4/PKG-INFO` & `myelectricaldatapy-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 2.1.4
+Version: 2.1.5
 Summary: Fetch Linky data from myelectricaldata.fr
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `myelectricaldatapy-2.1.4/README.md` & `myelectricaldatapy-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.4/example.py` & `myelectricaldatapy-2.1.5/example.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.4/myelectricaldatapy/analytics.py` & `myelectricaldatapy-2.1.5/myelectricaldatapy/analytics.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.4/myelectricaldatapy/auth.py` & `myelectricaldatapy-2.1.5/myelectricaldatapy/auth.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.4/myelectricaldatapy/myelectricaldata.py` & `myelectricaldatapy-2.1.5/myelectricaldatapy/myelectricaldata.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.4/myelectricaldatapy/mypdl.py` & `myelectricaldatapy-2.1.5/myelectricaldatapy/mypdl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Class for my PDL."""
 
 from __future__ import annotations
 
+from datetime import date, datetime as dt, timedelta
 import logging
-from datetime import date
-from datetime import datetime as dt
-from datetime import timedelta
 from typing import Any, Callable, Tuple
 
 import voluptuous as vol
 
 from myelectricaldatapy import Enedis, EnedisException, LimitReached
 
 from .analytics import EnedisAnalytics
@@ -320,15 +318,15 @@
         for mode, _param in self._params.items():
             dataset = {}
             start = _param[ATTR_START]
             end = _param[ATTR_END]
             if func := _param.get("func"):
                 try:
                     dataset = await func(self.pdl, start, end)
-                    if dataset is None:
+                    if dataset is None or dataset.get("meter_reading") is None:
                         raise EnedisException("Data collect is empty")
                 except EnedisException as error:
                     checked = False
                     _LOGGER.error(error.args[1]["detail"])
                 data = dataset.get("meter_reading", {}).get("interval_reading", {})
                 if len(data) != 0:
                     checked = checked and len(data) != 0
```

### Comparing `myelectricaldatapy-2.1.4/myelectricaldatapy.egg-info/PKG-INFO` & `myelectricaldatapy-2.1.5/myelectricaldatapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 2.1.4
+Version: 2.1.5
 Summary: Fetch Linky data from myelectricaldata.fr
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `myelectricaldatapy-2.1.4/myelectricaldatapy.egg-info/SOURCES.txt` & `myelectricaldatapy-2.1.5/myelectricaldatapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.4/pyproject.toml` & `myelectricaldatapy-2.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.4/tests/conftest.py` & `myelectricaldatapy-2.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.4/tests/consts.py` & `myelectricaldatapy-2.1.5/tests/consts.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.4/tests/test_analytics.py` & `myelectricaldatapy-2.1.5/tests/test_analytics.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.4/tests/test_load_data.py` & `myelectricaldatapy-2.1.5/tests/test_load_data.py`

 * *Files identical despite different names*

