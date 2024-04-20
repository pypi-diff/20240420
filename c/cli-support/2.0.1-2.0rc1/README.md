# Comparing `tmp/cli_support-2.0.1.tar.gz` & `tmp/cli_support-2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli_support-2.0.1.tar", max compression
+gzip compressed data, was "cli_support-2.0rc1.tar", max compression
```

## Comparing `cli_support-2.0.1.tar` & `cli_support-2.0rc1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1142 2024-04-20 09:41:15.706322 cli_support-2.0.1/cli_support/__init__.py
--rw-r--r--   0        0        0     8144 2023-12-24 16:29:14.016357 cli_support-2.0.1/cli_support/CLI.py
--rw-r--r--   0        0        0     3024 2023-12-24 16:02:05.177184 cli_support-2.0.1/cli_support/cli_assessment_summary.py
--rw-r--r--   0        0        0     1427 2023-12-24 16:30:28.500828 cli_support-2.0.1/cli_support/cli_copyright.py
--rw-r--r--   0        0        0     1750 2023-12-24 16:02:05.177184 cli_support-2.0.1/cli_support/cli_export_restriction.py
--rw-r--r--   0        0        0     1585 2023-12-24 16:02:05.177184 cli_support-2.0.1/cli_support/cli_external_id.py
--rw-r--r--   0        0        0     1699 2023-12-24 16:30:28.500828 cli_support-2.0.1/cli_support/cli_file_item_base.py
--rw-r--r--   0        0        0     4668 2023-12-24 16:02:05.177184 cli_support-2.0.1/cli_support/cli_general_information.py
--rw-r--r--   0        0        0     1096 2023-12-24 16:30:28.517009 cli_support-2.0.1/cli_support/cli_irrelevant_files.py
--rw-r--r--   0        0        0     2909 2023-12-24 16:30:28.517009 cli_support-2.0.1/cli_support/cli_license.py
--rw-r--r--   0        0        0     2180 2023-12-24 16:30:28.517009 cli_support-2.0.1/cli_support/cli_obligation.py
--rw-r--r--   0        0        0     5128 2023-12-24 16:30:13.388218 cli_support-2.0.1/cli_support/license_tools.py
--rw-r--r--   0        0        0        0 2023-12-24 16:02:05.177184 cli_support-2.0.1/cli_support/py.typed
--rw-r--r--   0        0        0      988 2023-12-24 16:02:05.177184 cli_support-2.0.1/cli_support/xml_base.py
--rw-r--r--   0        0        0     1127 2022-04-08 09:31:51.136414 cli_support-2.0.1/License.md
--rw-r--r--   0        0        0     1547 2024-04-20 09:41:46.404805 cli_support-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     2747 2024-04-20 09:45:54.722844 cli_support-2.0.1/Readme.md
--rw-r--r--   0        0        0     3562 1970-01-01 00:00:00.000000 cli_support-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1139 2023-12-24 16:02:05.177184 cli_support-2.0rc1/cli_support/__init__.py
+-rw-r--r--   0        0        0     8144 2023-12-24 16:29:14.016357 cli_support-2.0rc1/cli_support/CLI.py
+-rw-r--r--   0        0        0     3024 2023-12-24 16:02:05.177184 cli_support-2.0rc1/cli_support/cli_assessment_summary.py
+-rw-r--r--   0        0        0     1427 2023-12-24 16:30:28.500828 cli_support-2.0rc1/cli_support/cli_copyright.py
+-rw-r--r--   0        0        0     1750 2023-12-24 16:02:05.177184 cli_support-2.0rc1/cli_support/cli_export_restriction.py
+-rw-r--r--   0        0        0     1585 2023-12-24 16:02:05.177184 cli_support-2.0rc1/cli_support/cli_external_id.py
+-rw-r--r--   0        0        0     1699 2023-12-24 16:30:28.500828 cli_support-2.0rc1/cli_support/cli_file_item_base.py
+-rw-r--r--   0        0        0     4668 2023-12-24 16:02:05.177184 cli_support-2.0rc1/cli_support/cli_general_information.py
+-rw-r--r--   0        0        0     1096 2023-12-24 16:30:28.517009 cli_support-2.0rc1/cli_support/cli_irrelevant_files.py
+-rw-r--r--   0        0        0     2909 2023-12-24 16:30:28.517009 cli_support-2.0rc1/cli_support/cli_license.py
+-rw-r--r--   0        0        0     2180 2023-12-24 16:30:28.517009 cli_support-2.0rc1/cli_support/cli_obligation.py
+-rw-r--r--   0        0        0     5128 2023-12-24 16:30:13.388218 cli_support-2.0rc1/cli_support/license_tools.py
+-rw-r--r--   0        0        0        0 2023-12-24 16:02:05.177184 cli_support-2.0rc1/cli_support/py.typed
+-rw-r--r--   0        0        0      988 2023-12-24 16:02:05.177184 cli_support-2.0rc1/cli_support/xml_base.py
+-rw-r--r--   0        0        0     1127 2022-04-08 09:31:51.136414 cli_support-2.0rc1/License.md
+-rw-r--r--   0        0        0     1399 2023-12-24 16:02:05.177184 cli_support-2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     2749 2023-03-05 15:31:46.642596 cli_support-2.0rc1/Readme.md
+-rw-r--r--   0        0        0     3459 1970-01-01 00:00:00.000000 cli_support-2.0rc1/PKG-INFO
```

### Comparing `cli_support-2.0.1/cli_support/__init__.py` & `cli_support-2.0rc1/cli_support/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -------------------------------------------------------------------------------
-# (c) 2019-2024 Siemens AG
+# (c) 2019-2023 Siemens AG
 # All Rights Reserved.
 # Author: thomas.graf@siemens.com
 #
 # Licensed under the MIT license.
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
 
-__version__ = (2, 0, 1)
+__version__ = (2, 0)
 
 # isort: skip_file
 from .cli_copyright import CliCopyright
 from .cli_export_restriction import CliExportRestriction
 from .cli_license import CliLicense
 from .cli_obligation import CliObligation
 from .cli_external_id import CliExternalId
```

### Comparing `cli_support-2.0.1/cli_support/CLI.py` & `cli_support-2.0rc1/cli_support/CLI.py`

 * *Files identical despite different names*

### Comparing `cli_support-2.0.1/cli_support/cli_assessment_summary.py` & `cli_support-2.0rc1/cli_support/cli_assessment_summary.py`

 * *Files identical despite different names*

### Comparing `cli_support-2.0.1/cli_support/cli_copyright.py` & `cli_support-2.0rc1/cli_support/cli_copyright.py`

 * *Files identical despite different names*

### Comparing `cli_support-2.0.1/cli_support/cli_export_restriction.py` & `cli_support-2.0rc1/cli_support/cli_export_restriction.py`

 * *Files identical despite different names*

### Comparing `cli_support-2.0.1/cli_support/cli_external_id.py` & `cli_support-2.0rc1/cli_support/cli_external_id.py`

 * *Files identical despite different names*

### Comparing `cli_support-2.0.1/cli_support/cli_file_item_base.py` & `cli_support-2.0rc1/cli_support/cli_file_item_base.py`

 * *Files identical despite different names*

### Comparing `cli_support-2.0.1/cli_support/cli_general_information.py` & `cli_support-2.0rc1/cli_support/cli_general_information.py`

 * *Files identical despite different names*

### Comparing `cli_support-2.0.1/cli_support/cli_irrelevant_files.py` & `cli_support-2.0rc1/cli_support/cli_irrelevant_files.py`

 * *Files identical despite different names*

### Comparing `cli_support-2.0.1/cli_support/cli_license.py` & `cli_support-2.0rc1/cli_support/cli_license.py`

 * *Files identical despite different names*

### Comparing `cli_support-2.0.1/cli_support/cli_obligation.py` & `cli_support-2.0rc1/cli_support/cli_obligation.py`

 * *Files identical despite different names*

### Comparing `cli_support-2.0.1/cli_support/license_tools.py` & `cli_support-2.0rc1/cli_support/license_tools.py`

 * *Files identical despite different names*

### Comparing `cli_support-2.0.1/cli_support/xml_base.py` & `cli_support-2.0rc1/cli_support/xml_base.py`

 * *Files identical despite different names*

### Comparing `cli_support-2.0.1/License.md` & `cli_support-2.0rc1/License.md`

 * *Files identical despite different names*

### Comparing `cli_support-2.0.1/pyproject.toml` & `cli_support-2.0rc1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 [tool.poetry]
 name = "cli_support"
-version = "2.0.1"
+version = "2.0.pre1"
 description = "Support component license information (CLI) files"
 authors = ["Thomas Graf <thomas.graf@siemens.com>"]
 license = "MIT"
 readme="Readme.md"
 include = ["LICENSE.md"]
-repository = "https://github.com/sw360/clipython"
-homepage = "https://github.com/sw360/clipython"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
-[tool.poetry.group.dev.dependencies]
+[tool.poetry.dev-dependencies]
 colorama = "^0.4.3"
 flake8 = ">=3.9.2"
+requests = "^2.22.0"
 pytest = ">=7.2.0"
 coverage = ">=6.5.0"
-mypy = "^1.8.0"
-isort = "^5.13.2"
-types-colorama = "^0.4.15.12"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.mypy]
 exclude = [
```

### Comparing `cli_support-2.0.1/Readme.md` & `cli_support-2.0rc1/Readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # CLI Support for Python
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/sw360/clipython/blob/master/License.md)
-[![Python Version](https://img.shields.io/badge/python-3.8%2C3.9%2C3.10%2C3.11-yellow?logo=python)](https://www.python.org/doc/versions/)
-[![PyPI](https://shields.io/pypi/v/cli-support)](https://pypi.org/project/cli-support)
+[![Python Version](https://img.shields.io/badge/python-3.8%2C3.9-yellow?logo=python)](https://www.python.org/doc/versions/)
+[![PyPI version](https://img.shields.io/badge/pypi%20package-1.2.1-green)](https://pypi.org/project/cli-support)
 [![Static checks](https://github.com/sw360/clipython/actions/workflows/python-package.yml/badge.svg)](https://github.com/sw360/clipython/actions/workflows/python-package.yml)
 [![Unit tests](https://github.com/sw360/clipython/actions/workflows/unit-test.yml/badge.svg)](https://github.com/sw360/clipython/actions/workflows/unit-test.yml)
 
-Python library to read and write Component License Information (CLI) files. They can be
+Python library to read Component License Information (CLI) files. They can be
 created by [FOSSology](https://www.fossology.org) and stored in
 [SW360](https://www.eclipse.org/sw360/).
 
 For more information about the CLI file format, please have a look at
 [ComponentLicenseInformation.md](ComponentLicenseInformation.md).
 
 ## Usage
```

### Comparing `cli_support-2.0.1/PKG-INFO` & `cli_support-2.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: cli-support
-Version: 2.0.1
+Version: 2.0rc1
 Summary: Support component license information (CLI) files
-Home-page: https://github.com/sw360/clipython
 License: MIT
 Author: Thomas Graf
 Author-email: thomas.graf@siemens.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,26 +13,25 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Project-URL: Repository, https://github.com/sw360/clipython
 Description-Content-Type: text/markdown
 
 # CLI Support for Python
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/sw360/clipython/blob/master/License.md)
-[![Python Version](https://img.shields.io/badge/python-3.8%2C3.9%2C3.10%2C3.11-yellow?logo=python)](https://www.python.org/doc/versions/)
-[![PyPI](https://shields.io/pypi/v/cli-support)](https://pypi.org/project/cli-support)
+[![Python Version](https://img.shields.io/badge/python-3.8%2C3.9-yellow?logo=python)](https://www.python.org/doc/versions/)
+[![PyPI version](https://img.shields.io/badge/pypi%20package-1.2.1-green)](https://pypi.org/project/cli-support)
 [![Static checks](https://github.com/sw360/clipython/actions/workflows/python-package.yml/badge.svg)](https://github.com/sw360/clipython/actions/workflows/python-package.yml)
 [![Unit tests](https://github.com/sw360/clipython/actions/workflows/unit-test.yml/badge.svg)](https://github.com/sw360/clipython/actions/workflows/unit-test.yml)
 
-Python library to read and write Component License Information (CLI) files. They can be
+Python library to read Component License Information (CLI) files. They can be
 created by [FOSSology](https://www.fossology.org) and stored in
 [SW360](https://www.eclipse.org/sw360/).
 
 For more information about the CLI file format, please have a look at
 [ComponentLicenseInformation.md](ComponentLicenseInformation.md).
 
 ## Usage
```

