# Comparing `tmp/pypi_cleanup-0.1.6.dev20240420021837.tar.gz` & `tmp/pypi_cleanup-0.1.6.dev20240420025215.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_cleanup-0.1.6.dev20240420021837.tar", last modified: Sat Apr 20 02:18:55 2024, max compression
+gzip compressed data, was "pypi_cleanup-0.1.6.dev20240420025215.tar", last modified: Sat Apr 20 02:52:30 2024, max compression
```

## Comparing `pypi_cleanup-0.1.6.dev20240420021837.tar` & `pypi_cleanup-0.1.6.dev20240420025215.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:18:55.365093 pypi_cleanup-0.1.6.dev20240420021837/
--rw-rw-r--   0 runner    (1001) docker     (127)       29 2024-04-20 02:18:53.000000 pypi_cleanup-0.1.6.dev20240420021837/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-20 02:18:55.365093 pypi_cleanup-0.1.6.dev20240420021837/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:18:55.365093 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup/
--rw-r--r--   0 runner    (1001) docker     (127)    12570 2024-04-20 02:18:28.000000 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:18:55.365093 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-20 02:18:55.000000 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-20 02:18:55.000000 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 02:18:55.000000 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-20 02:18:55.000000 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 02:18:55.000000 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-20 02:18:55.000000 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-20 02:18:55.000000 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 02:18:55.000000 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 02:18:55.365093 pypi_cleanup-0.1.6.dev20240420021837/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     6465 2024-04-20 02:18:53.000000 pypi_cleanup-0.1.6.dev20240420021837/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:52:30.660658 pypi_cleanup-0.1.6.dev20240420025215/
+-rw-rw-r--   0 runner    (1001) docker     (127)       29 2024-04-20 02:52:29.000000 pypi_cleanup-0.1.6.dev20240420025215/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-20 02:52:30.660658 pypi_cleanup-0.1.6.dev20240420025215/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:52:30.660658 pypi_cleanup-0.1.6.dev20240420025215/pypi_cleanup/
+-rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-04-20 02:52:09.000000 pypi_cleanup-0.1.6.dev20240420025215/pypi_cleanup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:52:30.660658 pypi_cleanup-0.1.6.dev20240420025215/pypi_cleanup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-20 02:52:30.000000 pypi_cleanup-0.1.6.dev20240420025215/pypi_cleanup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-20 02:52:30.000000 pypi_cleanup-0.1.6.dev20240420025215/pypi_cleanup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 02:52:30.000000 pypi_cleanup-0.1.6.dev20240420025215/pypi_cleanup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-20 02:52:30.000000 pypi_cleanup-0.1.6.dev20240420025215/pypi_cleanup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 02:52:30.000000 pypi_cleanup-0.1.6.dev20240420025215/pypi_cleanup.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-20 02:52:30.000000 pypi_cleanup-0.1.6.dev20240420025215/pypi_cleanup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-20 02:52:30.000000 pypi_cleanup-0.1.6.dev20240420025215/pypi_cleanup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 02:52:30.000000 pypi_cleanup-0.1.6.dev20240420025215/pypi_cleanup.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 02:52:30.660658 pypi_cleanup-0.1.6.dev20240420025215/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6465 2024-04-20 02:52:29.000000 pypi_cleanup-0.1.6.dev20240420025215/setup.py
```

### Comparing `pypi_cleanup-0.1.6.dev20240420021837/PKG-INFO` & `pypi_cleanup-0.1.6.dev20240420025215/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-cleanup
-Version: 0.1.6.dev20240420021837
+Version: 0.1.6.dev20240420025215
 Summary: PyPI Bulk Release Version Cleanup Utility
 Home-page: https://github.com/arcivanov/pypi-cleanup
 Author: Arcadiy Ivanov
 Author-email: arcadiy@ivanov.biz
 Maintainer: Arcadiy Ivanov
 Maintainer-email: arcadiy@ivanov.biz
 License: Apache License, Version 2.0
```

### Comparing `pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup/__init__.py` & `pypi_cleanup-0.1.6.dev20240420025215/pypi_cleanup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,16 @@
 
                 project_info = r.json()
                 releases_by_date = {}
                 for version in project_info["versions"]:
                     releases_by_date[version] = max(
                         [datetime.datetime.strptime(f["upload-time"], '%Y-%m-%dT%H:%M:%S.%f%z')
                          for f in project_info["files"]
-                         if f["filename"].lower().startswith(f"{self.package}-{version}")])
+                         if f["filename"].lower().startswith(f"{self.package}-{version}") or
+                         f["filename"].lower().startswith(f"{self.package.replace('-', '_')}-{version}")])
 
             if not releases_by_date:
                 logging.info(f"No releases for package {self.package!r} have been found")
                 return
 
             pkg_vers = list(filter(lambda k:
                                    any(filter(lambda rex: rex.match(k),
```

### Comparing `pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup.egg-info/PKG-INFO` & `pypi_cleanup-0.1.6.dev20240420025215/pypi_cleanup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-cleanup
-Version: 0.1.6.dev20240420021837
+Version: 0.1.6.dev20240420025215
 Summary: PyPI Bulk Release Version Cleanup Utility
 Home-page: https://github.com/arcivanov/pypi-cleanup
 Author: Arcadiy Ivanov
 Author-email: arcadiy@ivanov.biz
 Maintainer: Arcadiy Ivanov
 Maintainer-email: arcadiy@ivanov.biz
 License: Apache License, Version 2.0
```

### Comparing `pypi_cleanup-0.1.6.dev20240420021837/setup.py` & `pypi_cleanup-0.1.6.dev20240420025215/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'pypi-cleanup',
-        version = '0.1.6.dev20240420021837',
+        version = '0.1.6.dev20240420025215',
         description = 'PyPI Bulk Release Version Cleanup Utility',
         long_description = '# PyPI Bulk Release Version Cleanup Utility\n\n[![PyPI Cleanup Version](https://img.shields.io/pypi/v/pypi-cleanup?logo=pypi)](https://pypi.org/project/pypi-cleanup/)\n[![PyPI Cleanup Python Versions](https://img.shields.io/pypi/pyversions/pypi-cleanup?logo=pypi)](https://pypi.org/project/pypi-cleanup/)\n[![Build Status](https://img.shields.io/github/actions/workflow/status/arcivanov/pypi-cleanup/pypi-cleanup.yml?branch=master)](https://github.com/arcivanov/pypi-cleanup/actions/workflows/pypi-cleanup.yml)\n[![PyPI Cleanup Downloads Per Day](https://img.shields.io/pypi/dd/pypi-cleanup?logo=pypi)](https://pypi.org/project/pypi-cleanup/)\n[![PyPI Cleanup Downloads Per Week](https://img.shields.io/pypi/dw/pypi-cleanup?logo=pypi)](https://pypi.org/project/pypi-cleanup/)\n[![PyPI Cleanup Downloads Per Month](https://img.shields.io/pypi/dm/pypi-cleanup?logo=pypi)](https://pypi.org/project/pypi-cleanup/)\n\n## Overview\n\nPyPI Bulk Release Version Cleanup Utility (`pypi-cleanup`) is designed to bulk-delete releases from PyPI that match\nspecified patterns.\nThis utility is most useful when CI/CD method produces a swarm of temporary\n[.devN pre-releases](https://www.python.org/dev/peps/pep-0440/#developmental-releases) in between versioned releases.\n\nBeing able to cleanup past .devN junk helps PyPI cut down on the storage requirements and keeps release history neatly\norganized.\n\n## WARNING\n\nTHIS UTILITY IS DESTRUCTIVE AND CAN POTENTIALLY WRECK YOUR PROJECT RELEASES AND MAKE THE PROJECT INACCESSIBLE ON PYPI.\n\nThis utility is provided on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or\nimplied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY,\nor FITNESS FOR A PARTICULAR PURPOSE.\n\n## Details\n\nThe default package release version selection pattern is `r".*dev\\d+$"`.\n\nAuthentication password may be passed via environment variable\n`PYPI_CLEANUP_PASSWORD`. Otherwise, you will be prompted to enter it.\n\nAuthentication with TOTP is supported.\n\nExamples:\n\n```bash\n$ pypi-cleanup --help\nusage: pypi-cleanup [-h] -u USERNAME -p PACKAGE [-t URL] [-r PATTERNS] [--do-it] [-y] [-v]\n\nPyPi Package Cleanup Utility\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -u USERNAME, --username USERNAME\n                        authentication username (default: None)\n  -p PACKAGE, --package PACKAGE\n                        PyPI package name (default: None)\n  -t URL, --host URL    PyPI <proto>://<host> prefix (default: https://pypi.org/)\n  -r PATTERNS, --version-regex PATTERNS\n                        regex to use to match package versions to be deleted (default: None)\n  --do-it               actually perform the destructive delete (default: False)\n  -y, --yes             confirm extremely dangerous destructive delete (default: False)\n  -v, --verbose         be verbose (default: 0)\n```\n\n```bash\n$ pypi-cleanup -u arcivanov -p pybuilder\nPassword: \nAuthentication code: 123456\nINFO:root:Deleting pybuilder version 0.12.3.dev20200421010849\nINFO:root:Deleted pybuilder version 0.12.3.dev20200421010849\nINFO:root:Deleting pybuilder version 0.12.3.dev20200421010857\nINFO:root:Deleted pybuilder version 0.12.3.dev20200421010857\n```\n\n```bash\n$ pypi-cleanup -u arcivanov -p geventmp -n -r \'.*\\\\.dev1$\'\nPassword:\nWARNING:root:RUNNING IN DRY-RUN MODE\nINFO:root:Will use the following patterns [re.compile(\'.*\\\\.dev1$\')] on package geventmp\nAuthentication code: 123456\nINFO:root:Deleting geventmp version 0.0.1.dev1\n```\n',
         long_description_content_type = 'text/markdown',
         classifiers = [
             'Programming Language :: Python',
             'Programming Language :: Python :: Implementation :: CPython',
             'Programming Language :: Python :: Implementation :: PyPy',
```

