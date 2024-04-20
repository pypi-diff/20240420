# Comparing `tmp/StringDataDeque-1.0.1.tar.gz` & `tmp/stringdatadeque-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StringDataDeque-1.0.1.tar", last modified: Mon Apr  8 21:10:10 2024, max compression
+gzip compressed data, was "stringdatadeque-1.0.2.tar", last modified: Sat Apr 20 14:14:46 2024, max compression
```

## Comparing `StringDataDeque-1.0.1.tar` & `stringdatadeque-1.0.2.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:10.561592 StringDataDeque-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:10.553592 StringDataDeque-1.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:10.553592 StringDataDeque-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.github/workflows/black.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.github/workflows/dapperdata.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.github/workflows/tomlsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.github/workflows/tox.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/.yamllint
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    43498 2024-04-08 21:10:10.561592 StringDataDeque-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:10.557592 StringDataDeque-1.0.1/StringDataDeque.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43498 2024-04-08 21:10:10.000000 StringDataDeque-1.0.1/StringDataDeque.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-08 21:10:10.000000 StringDataDeque-1.0.1/StringDataDeque.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 21:10:10.000000 StringDataDeque-1.0.1/StringDataDeque.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-08 21:10:10.000000 StringDataDeque-1.0.1/StringDataDeque.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 21:10:10.000000 StringDataDeque-1.0.1/StringDataDeque.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/check_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:10.557592 StringDataDeque-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/docs/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/docs/index.rst.bak
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:10.557592 StringDataDeque-1.0.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/docs/source/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/docs/source/stringdatadeque.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/justfile
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/requirements-optional.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 21:10:10.561592 StringDataDeque-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:10.549592 StringDataDeque-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:10.557592 StringDataDeque-1.0.1/src/stringdatadeque/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/src/stringdatadeque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10390 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/src/stringdatadeque/encryptedstringdeque.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/src/stringdatadeque/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/src/stringdatadeque/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18233 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/src/stringdatadeque/stringdatadeque.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:10.557592 StringDataDeque-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/tests/default.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/tests/private.pem
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/tests/test_encryptedssgtringdeque.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/tests/test_stringdatadeque.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-08 21:10:06.000000 StringDataDeque-1.0.1/tests/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:46.218318 stringdatadeque-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:46.206318 stringdatadeque-1.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:46.210318 stringdatadeque-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/.github/workflows/black.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/.github/workflows/dapperdata.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/.github/workflows/tomlsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/.github/workflows/tox.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    43538 2024-04-20 14:14:46.218318 stringdatadeque-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:46.214318 stringdatadeque-1.0.2/StringDataDeque.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43538 2024-04-20 14:14:46.000000 stringdatadeque-1.0.2/StringDataDeque.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-20 14:14:46.000000 stringdatadeque-1.0.2/StringDataDeque.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 14:14:46.000000 stringdatadeque-1.0.2/StringDataDeque.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-20 14:14:46.000000 stringdatadeque-1.0.2/StringDataDeque.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-20 14:14:46.000000 stringdatadeque-1.0.2/StringDataDeque.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/check_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:46.210318 stringdatadeque-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/docs/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/docs/index.rst.bak
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:46.210318 stringdatadeque-1.0.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/docs/source/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/docs/source/stringdatadeque.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/justfile
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/requirements-optional.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 14:14:46.218318 stringdatadeque-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:46.206318 stringdatadeque-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:46.214318 stringdatadeque-1.0.2/src/stringdatadeque/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/src/stringdatadeque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/src/stringdatadeque/encryptedstringdeque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/src/stringdatadeque/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/src/stringdatadeque/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18362 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/src/stringdatadeque/stringdatadeque.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 14:14:46.214318 stringdatadeque-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/tests/default.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/tests/private.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/tests/test_encryptedssgtringdeque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/tests/test_stringdatadeque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-20 14:14:41.000000 stringdatadeque-1.0.2/tests/timing.py
```

### Comparing `StringDataDeque-1.0.1/.github/workflows/pypi.yaml` & `stringdatadeque-1.0.2/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.1/.github/workflows/tox.yaml` & `stringdatadeque-1.0.2/.github/workflows/tox.yaml`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.1/.gitignore` & `stringdatadeque-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.1/.pre-commit-config.yaml` & `stringdatadeque-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.1/LICENSE` & `stringdatadeque-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.1/PKG-INFO` & `stringdatadeque-1.0.2/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StringDataDeque
-Version: 1.0.1
+Version: 1.0.2
 Summary: Useful when building a string from data that can be converted into a string, in parts.
 Author: R.Broderick
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -705,14 +705,15 @@
 Requires-Dist: autodocsumm; extra == "dev"
 Requires-Dist: snakeviz; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: tox-pyenv-redux; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: perflint; extra == "dev"
+Requires-Dist: snakeviz; extra == "dev"
 Provides-Extra: optional
 Requires-Dist: pycryptodome; extra == "optional"
 
 # StringDataDeque
 
 Useful when building a string from data that can be converted into a string, in parts.
```

### Comparing `StringDataDeque-1.0.1/README.md` & `stringdatadeque-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.1/StringDataDeque.egg-info/PKG-INFO` & `stringdatadeque-1.0.2/StringDataDeque.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StringDataDeque
-Version: 1.0.1
+Version: 1.0.2
 Summary: Useful when building a string from data that can be converted into a string, in parts.
 Author: R.Broderick
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -705,14 +705,15 @@
 Requires-Dist: autodocsumm; extra == "dev"
 Requires-Dist: snakeviz; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: tox-pyenv-redux; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: perflint; extra == "dev"
+Requires-Dist: snakeviz; extra == "dev"
 Provides-Extra: optional
 Requires-Dist: pycryptodome; extra == "optional"
 
 # StringDataDeque
 
 Useful when building a string from data that can be converted into a string, in parts.
```

### Comparing `StringDataDeque-1.0.1/StringDataDeque.egg-info/SOURCES.txt` & `stringdatadeque-1.0.2/StringDataDeque.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
 .python-version
 .yamllint
+CODE_OF_CONDUCT.md
 LICENSE
 README.md
 check_names.py
 justfile
 pyproject.toml
 requirements-dev.txt
 requirements-optional.txt
```

### Comparing `StringDataDeque-1.0.1/check_names.py` & `stringdatadeque-1.0.2/check_names.py`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.1/docs/Makefile` & `stringdatadeque-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.1/docs/conf.py` & `stringdatadeque-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.1/docs/make.bat` & `stringdatadeque-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.1/docs/source/stringdatadeque.rst` & `stringdatadeque-1.0.2/docs/source/stringdatadeque.rst`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.1/justfile` & `stringdatadeque-1.0.2/justfile`

 * *Files 3% similar despite different names*

```diff
@@ -20,26 +20,35 @@
 pre-commit_install:
     pre-commit install
 
 # Setup sphynx autodoc
 setup_autodoc:
     sphinx-apidoc -f -o docs/source {{PACKAGE_SLUG}}
 
+# profiling
+profile:
+    python -m cProfile -s time -o timing.prof tests/timing.py --profile
+    snakeviz timing.prof
+
 #
 # Formatting
 #
 # Run all linting and fixes
-fixes: validate_pyproject ruff_fixes ruff_format_fixes dapperdata_fixes tomlsort_fixes docs pytest
+fixes: validate_pyproject ruff_fixes ruff_format_fixes pylint dapperdata_fixes tomlsort_fixes docs pytest
 
 _fixes_no_ruff: validate_pyproject dapperdata_fixes tomlsort_fixes docs pytest update_dependencies_quiet
 
 # Validate pyproject.toml format
 validate_pyproject:
     {{PYTHON}} -m validate_pyproject pyproject.toml
 
+# Run pylint
+pylint:
+   {{PYTHON}} -m pylint {{PACKAGE_SLUG}}
+
 # Run Ruff and fix
 ruff_fixes:
     {{PYTHON}} -m ruff check . --fix
 
 alias black_check := ruff_format_fixes
 #Run Ruff format fixes
 ruff_format_fixes:
```

### Comparing `StringDataDeque-1.0.1/pyproject.toml` & `stringdatadeque-1.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=67.0", "setuptools_scm[toml]>=7.1"]
 
 [project]
 authors = [{"name" = "R.Broderick"}]
 description = "Useful when building a string from data that can be converted into a string, in parts."
-version = "1.0.1"
+version = "1.0.2"
 license = {"file" = "LICENSE"}
 name = "StringDataDeque"
 readme = {file = "README.md", content-type = "text/markdown"}
 dependencies = ["beartype", "typing-extensions; python_version < '3.12'"]
 requires-python = ">=3.10.0"
 
 [project.optional-dependencies]
@@ -34,15 +34,16 @@
   "sphinx-rtd-theme ",
   "autodocsumm",
   "snakeviz",
   "pre-commit",
   "tox",
   "tox-pyenv-redux",
   "pylint",
-  "perflint"
+  "perflint",
+  "snakeviz"
 ]
 # pep725
 # [external]
 # build-requires = [
 # "virtual:compiler/rust",
 # "virtual:compiler/cargo",
 # ]
@@ -98,15 +99,75 @@
   "E1129",
   "E0213",
   "W0221",
   "E1128",
   "C0321",
   "logging-fstring-interpolation",
   "unnecessary-lambda-assignment",
-  "protected-access"
+  "protected-access",
+  # codes in ruff
+  "C0105",
+  "C0131",
+  "C0132",
+  "C0205",
+  "C0208",
+  "C0414",
+  "C3002",
+  "E0100",
+  "E0101",
+  "E0116",
+  "E0117",
+  "E0118",
+  "E0237",
+  "E0241",
+  "E0302",
+  "E0307",
+  "E0604",
+  "E0605",
+  "E1142",
+  "E1205",
+  "E1206",
+  "E1300",
+  "E1307",
+  "E1310",
+  "E1507",
+  "E1700",
+  "E2502",
+  "E2510",
+  "E2512",
+  "E2513",
+  "E2514",
+  "E2515",
+  "R0124",
+  "R0133",
+  "R0206",
+  "R0402",
+  "R0911",
+  "R0912",
+  "R0913",
+  "R0915",
+  "R1701",
+  "R1711",
+  "R1714",
+  "R1722",
+  # "R2004",
+  # "R5501",
+  "W0120",
+  "W0127",
+  "W0129",
+  "W0131",
+  "W0406",
+  "W0602",
+  "W0603",
+  "W0711",
+  "W1508",
+  "W1509",
+  "W1510",
+  # "W2901",
+  "W3301"
 ]
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 
 [tool.ruff]
 exclude = [".venv", "./stringdatadeque/_version.py"]
```

### Comparing `StringDataDeque-1.0.1/requirements-dev.txt` & `stringdatadeque-1.0.2/requirements-dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 astroid==3.1.0
     # via pylint
 attrs==23.2.0
     # via glom
 autodocsumm==0.2.12
 babel==2.14.0
     # via sphinx
-beartype==0.18.2
+beartype==0.18.4
 boltons==24.0.0
     # via
     #   face
     #   glom
 build==1.2.1
 cachetools==5.3.3
     # via tox
@@ -48,22 +48,22 @@
     # via
     #   dom-toml
     #   sphinx-pyproject
 face==20.1.1
     # via glom
 fastjsonschema==2.19.1
     # via validate-pyproject
-filelock==3.13.3
+filelock==3.13.4
     # via
     #   tox
     #   virtualenv
 glom==23.5.0
 identify==2.5.35
     # via pre-commit
-idna==3.6
+idna==3.7
     # via requests
 imagesize==1.4.1
     # via sphinx
 iniconfig==2.0.0
     # via pytest
 isort==5.13.2
     # via pylint
@@ -98,19 +98,19 @@
     #   tox
     #   virtualenv
 pluggy==1.4.0
     # via
     #   pytest
     #   tox
 pre-commit==3.7.0
-pydantic==2.6.4
+pydantic==2.7.0
     # via
     #   dapperdata
     #   pydantic-settings
-pydantic-core==2.16.3
+pydantic-core==2.18.1
     # via pydantic
 pydantic-settings==2.2.1
     # via dapperdata
 pyenv-inspect==0.4.0
     # via virtualenv-pyenv
 pygments==2.17.2
     # via
@@ -138,30 +138,30 @@
     # via
     #   pytest-pretty
     #   typer
 ruamel-yaml==0.18.6
     # via dapperdata
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-ruff==0.3.5
-setuptools==69.2.0
+ruff==0.4.1
+setuptools==69.5.1
     # via nodeenv
 shellingham==1.5.4
     # via typer
 snakeviz==2.2.0
 snowballstemmer==2.2.0
     # via sphinx
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   sphinx-autodoc-typehints
     #   sphinx-rtd-size
     #   sphinx-rtd-theme
     #   sphinxcontrib-jquery
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
 sphinx-pyproject==0.3.0
 sphinx-rtd-size==0.2.0
 sphinx-rtd-theme==2.0.0
 sphinxcontrib-applehelp==1.0.8
     # via sphinx
 sphinxcontrib-devhelp==1.0.6
     # via sphinx
@@ -183,27 +183,27 @@
     #   pylint
     #   toml-sort
 tornado==6.4
     # via snakeviz
 tox==4.14.2
     # via tox-pyenv-redux
 tox-pyenv-redux==1.1.0
-typer==0.12.2
+typer==0.12.3
     # via dapperdata
 typing-extensions==4.11.0
     # via
     #   domdf-python-tools
     #   mypy
     #   pydantic
     #   pydantic-core
     #   typer
 urllib3==2.2.1
     # via requests
-uv==0.1.29
+uv==0.1.35
 validate-pyproject==0.16
-virtualenv==20.25.1
+virtualenv==20.25.3
     # via
     #   pre-commit
     #   tox
     #   virtualenv-pyenv
 virtualenv-pyenv==0.5.0
     # via tox-pyenv-redux
```

### Comparing `StringDataDeque-1.0.1/src/stringdatadeque/__init__.py` & `stringdatadeque-1.0.2/src/stringdatadeque/__init__.py`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.1/src/stringdatadeque/encryptedstringdeque.py` & `stringdatadeque-1.0.2/src/stringdatadeque/encryptedstringdeque.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,14 +188,16 @@
     :type data: SequenceNonstrOfStr | str | None
     :param format_func: The function used to format the encrypted data.
     :type format_func: Callable[[RSAMessage], str]
     :param sep: The separator used when joining the strings.
     :type sep: str
     """
 
+    __slots__ = ("type", "public_key", "session_key", "enc_session_key", "_data")
+
     @staticmethod
     def __keep_encrypted(msg: RSAMessage) -> str:  # pragma: no cover
         """Keep the message encrypted.
 
         :param msg: The encrypted message.
         :type msg: RSAMessage
```

### Comparing `StringDataDeque-1.0.1/src/stringdatadeque/protocols.py` & `stringdatadeque-1.0.2/src/stringdatadeque/protocols.py`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.1/src/stringdatadeque/stringdatadeque.py` & `stringdatadeque-1.0.2/src/stringdatadeque/stringdatadeque.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 # class REqual(str):
 #     "Override str.__eq__ to match a regex pattern."
 #     def __eq__(self, pattern):
 #         return re.fullmatch(pattern, self)
 
 
-class LikeMatch(str):
+class InMatch(str):
     """A class representing a custom string type used for 'like' matching.
 
     :param pattern: Pattern string to match against.
     :type pattern: str
     :return: True if pattern matches.
     """
 
@@ -72,14 +72,16 @@
     :param data: The data to be stored in the deque.
     :type data: SequenceNonStr[ConvertibleToDataType] | ConvertibleToDataType | None
     :param sep: The separator to join elements when converting to a string.
         defaults to ''
     :type sep: str
     """
 
+    __slots__ = ("_data", "convert_func", "format_func", "sep")
+
     @overload
     def __init__(
         self,
         convert_func: Callable[[ConvertibleToDataType], DataType],
         format_func: Callable[[DataType], str],
         data: SequenceNonStr[ConvertibleToDataType] | None = None,
         sep: str = "",
@@ -151,15 +153,15 @@
 
         :param format_spec: A string specifying the format.
         :type format_spec: str
 
         :return: The formatted string.
         :rtype: str
         """
-        match LikeMatch(format_spec):
+        match InMatch(format_spec):
             case "sep=":
                 old_sep, self.sep = (
                     self.sep,
                     format_spec.partition("sep=")[2].strip("'\""),
                 )
                 ret = str(self)
                 self.sep = old_sep
@@ -371,14 +373,16 @@
         return ret
 
 
 @beartype
 class StringDeque(StringDataDeque[str, Builtin_or_DefinesDunderStr]):
     """A class representing a StringDeque."""
 
+    __slots__ = ()
+
     @overload
     def __init__(
         self,
         data: SequenceNonStr[Builtin_or_DefinesDunderStr] | None = None,
         sep: str = "",
     ) -> None: ...
 
@@ -410,14 +414,16 @@
         super().__init__(convert_func=str, format_func=str, data=data, sep=sep)
 
 
 @beartype
 class CircularStringDeque(StringDeque):
     """A circular StringBuffer, overwrites once maxlen reached."""
 
+    __slots__ = ("_size",)
+
     @overload
     def __init__(
         self,
         size: int,
         data: SequenceNonStr[Builtin_or_DefinesDunderStr] | None = None,
         sep: str = "",
     ) -> None: ...
@@ -470,14 +476,16 @@
     - clear: Clearing all items from the deque is not allowed.
     - __delitem__: Deleting items from the deque is not allowed.
 
     :raises NotImplementedError: When trying to perform unsupported operations on
         WORMStringDeque.
     """
 
+    __slots__ = ()
+
     @overload
     def __init__(
         self,
         data: SequenceNonStr[Builtin_or_DefinesDunderStr] | None = None,
         sep: str = "",
     ) -> None: ...
```

### Comparing `StringDataDeque-1.0.1/tests/private.pem` & `stringdatadeque-1.0.2/tests/private.pem`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.1/tests/test_encryptedssgtringdeque.py` & `stringdatadeque-1.0.2/tests/test_encryptedssgtringdeque.py`

 * *Files identical despite different names*

### Comparing `StringDataDeque-1.0.1/tests/test_stringdatadeque.py` & `stringdatadeque-1.0.2/tests/test_stringdatadeque.py`

 * *Files identical despite different names*

