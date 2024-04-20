# Comparing `tmp/pypi-cleanup-0.1.5.tar.gz` & `tmp/pypi_cleanup-0.1.6.dev20240420021837.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi-cleanup-0.1.5.tar", last modified: Tue Feb 27 23:13:49 2024, max compression
+gzip compressed data, was "pypi_cleanup-0.1.6.dev20240420021837.tar", last modified: Sat Apr 20 02:18:55 2024, max compression
```

## Comparing `pypi-cleanup-0.1.5.tar` & `pypi_cleanup-0.1.6.dev20240420021837.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 23:13:49.441740 pypi-cleanup-0.1.5/
--rw-rw-r--   0 runner    (1001) docker     (127)       29 2024-02-27 23:13:48.000000 pypi-cleanup-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-02-27 23:13:49.437740 pypi-cleanup-0.1.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 23:13:49.437740 pypi-cleanup-0.1.5/pypi_cleanup/
--rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-02-27 23:13:15.000000 pypi-cleanup-0.1.5/pypi_cleanup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 23:13:49.437740 pypi-cleanup-0.1.5/pypi_cleanup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-02-27 23:13:49.000000 pypi-cleanup-0.1.5/pypi_cleanup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-27 23:13:49.000000 pypi-cleanup-0.1.5/pypi_cleanup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 23:13:49.000000 pypi-cleanup-0.1.5/pypi_cleanup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-27 23:13:49.000000 pypi-cleanup-0.1.5/pypi_cleanup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 23:13:49.000000 pypi-cleanup-0.1.5/pypi_cleanup.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-27 23:13:49.000000 pypi-cleanup-0.1.5/pypi_cleanup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-27 23:13:49.000000 pypi-cleanup-0.1.5/pypi_cleanup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 23:13:49.000000 pypi-cleanup-0.1.5/pypi_cleanup.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 23:13:49.441740 pypi-cleanup-0.1.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     6447 2024-02-27 23:13:48.000000 pypi-cleanup-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:18:55.365093 pypi_cleanup-0.1.6.dev20240420021837/
+-rw-rw-r--   0 runner    (1001) docker     (127)       29 2024-04-20 02:18:53.000000 pypi_cleanup-0.1.6.dev20240420021837/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-20 02:18:55.365093 pypi_cleanup-0.1.6.dev20240420021837/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:18:55.365093 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup/
+-rw-r--r--   0 runner    (1001) docker     (127)    12570 2024-04-20 02:18:28.000000 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:18:55.365093 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-20 02:18:55.000000 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-20 02:18:55.000000 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 02:18:55.000000 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-20 02:18:55.000000 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 02:18:55.000000 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-20 02:18:55.000000 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-20 02:18:55.000000 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 02:18:55.000000 pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 02:18:55.365093 pypi_cleanup-0.1.6.dev20240420021837/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6465 2024-04-20 02:18:53.000000 pypi_cleanup-0.1.6.dev20240420021837/setup.py
```

### Comparing `pypi-cleanup-0.1.5/PKG-INFO` & `pypi_cleanup-0.1.6.dev20240420021837/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-cleanup
-Version: 0.1.5
+Version: 0.1.6.dev20240420021837
 Summary: PyPI Bulk Release Version Cleanup Utility
 Home-page: https://github.com/arcivanov/pypi-cleanup
 Author: Arcadiy Ivanov
 Author-email: arcadiy@ivanov.biz
 Maintainer: Arcadiy Ivanov
 Maintainer-email: arcadiy@ivanov.biz
 License: Apache License, Version 2.0
```

### Comparing `pypi-cleanup-0.1.5/pypi_cleanup/__init__.py` & `pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,24 +67,25 @@
             # If we're in a right form that contains the requested input and csrf is not set
             if (not self._contains_input or self._input_contained) and not self.csrf:
                 self.csrf = self._csrf
             return
 
 
 class PypiCleanup:
-    def __init__(self, url, username, package, do_it, patterns, verbose, days, **_):
+    def __init__(self, url, username, package, do_it, patterns, verbose, days, query_only, **_):
         self.url = urlparse(url).geturl()
         if self.url[-1] == "/":
             self.url = self.url[:-1]
         self.username = username
         self.do_it = do_it
         self.package = package
         self.patterns = patterns or DEFAULT_PATTERNS
         self.verbose = verbose
-        self.date = datetime.datetime.now(datetime.UTC) - datetime.timedelta(days=days)
+        self.query_only = query_only
+        self.date = datetime.datetime.now(datetime.timezone.utc) - datetime.timedelta(days=days)
 
     def run(self):
         csrf = None
 
         if self.verbose:
             logging.root.setLevel(logging.DEBUG)
 
@@ -120,32 +121,38 @@
                                    any(filter(lambda rex: rex.match(k),
                                               self.patterns)) and releases_by_date[k] < self.date,
                                    releases_by_date.keys()))
 
             if not pkg_vers:
                 logging.info(f"No releases were found matching specified patterns "
                              f"and dates in package {self.package!r}")
-                return
+            else:
+                logging.info("Found the following releases to delete:")
+                for pkg_ver in pkg_vers:
+                    logging.info(f" {pkg_ver}")
 
-            if set(pkg_vers) == set(releases_by_date.keys()):
+            if pkg_vers and set(pkg_vers) == set(releases_by_date.keys()):
                 print(dedent(f"""
                 WARNING:
                 \tYou have selected the following patterns: {self.patterns}
                 \tThese patterns would delete all available released versions of {self.package!r}.
                 \tThis will render your project/package permanently inaccessible.
                 \tSince the costs of an error are too high I'm refusing to do this.
                 \tGoodbye.
                 """), file=sys.stderr)
 
                 if not self.do_it:
                     return 3
 
-            logging.info("Found the following releases to delete:")
-            for pkg_ver in pkg_vers:
-                logging.info(f" {pkg_ver}")
+            if self.query_only:
+                logging.info("Query-only mode - exiting")
+                return
+
+            if not pkg_vers:
+                return
 
             password = os.getenv("PYPI_CLEANUP_PASSWORD")
 
             if self.username is None:
                 realpath = os.path.realpath(os.path.expanduser("~/.pypirc"))
                 parser = configparser.RawConfigParser()
                 try:
@@ -238,38 +245,45 @@
                 else:
                     logging.info(f"Would be deleting {self.package!r} version {pkg_ver}, but not doing it!")
 
 
 def main():
     logging.basicConfig(level=logging.INFO)
 
-    parser = argparse.ArgumentParser(description="PyPi Package Cleanup Utility",
-                                     formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    parser.add_argument("-u", "--username", help="authentication username")
-    parser.add_argument("-p", "--package", required=True, help="PyPI package name")
-    parser.add_argument("-t", "--host", default="https://pypi.org/", dest="url", help="PyPI <proto>://<host> prefix")
-    parser.add_argument("-r", "--version-regex", type=re.compile, action="append",
-                        dest="patterns", help="regex to use to match package versions to be deleted")
-    parser.add_argument("--do-it", action="store_true", default=False, help="actually perform the destructive delete")
-    parser.add_argument("-y", "--yes", action="store_true", default=False, dest="confirm",
-                        help="confirm extremely dangerous destructive delete")
-    parser.add_argument("-d", "--days", type=int, default=0,
-                        help="only delete releases where all files are older than X days")
-    parser.add_argument("-v", "--verbose", action="store_const", const=1, default=0, help="be verbose")
-
-    args = parser.parse_args()
-    if args.patterns and not args.confirm and not args.do_it:
-        logging.warning(dedent(f"""
-        WARNING:
-        \tYou're using custom patterns: {args.patterns}.
-        \tIf you make a mistake in your patterns you can potentially wipe critical versions irrecoverably.
-        \tMake sure to test your patterns before running the destructive cleanup.
-        \tOnce you're satisfied the patterns are correct re-run with `-y`/`--yes` to confirm you know what you're doing.
-        \tGoodbye.
-        \t"""))
-        return 3
-
-    return PypiCleanup(**vars(args)).run()
+    try:
+        parser = argparse.ArgumentParser(description="PyPi Package Cleanup Utility",
+                                         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+        parser.add_argument("-u", "--username", help="authentication username")
+        parser.add_argument("-p", "--package", required=True, help="PyPI package name")
+        parser.add_argument("-t", "--host", default="https://pypi.org/", dest="url",
+                            help="PyPI <proto>://<host> prefix")
+        parser.add_argument("-r", "--version-regex", type=re.compile, action="append",
+                            dest="patterns", help="regex to use to match package versions to be deleted")
+        parser.add_argument("--query-only", action="store_true", default=False,
+                            help="only queries and processes the package, no login required")
+        parser.add_argument("--do-it", action="store_true", default=False,
+                            help="actually perform the destructive delete")
+        parser.add_argument("-y", "--yes", action="store_true", default=False, dest="confirm",
+                            help="confirm extremely dangerous destructive delete")
+        parser.add_argument("-d", "--days", type=int, default=0,
+                            help="only delete releases where all files are older than X days")
+        parser.add_argument("-v", "--verbose", action="store_const", const=1, default=0, help="be verbose")
+
+        args = parser.parse_args()
+        if args.patterns and not args.confirm and not args.do_it:
+            logging.warning(dedent(f"""
+            WARNING:
+            \tYou're using custom patterns: {args.patterns}.
+            \tIf you make a mistake in your patterns you can potentially wipe critical versions irrecoverably.
+            \tMake sure to test your patterns before running the destructive cleanup.
+            \tOnce you're satisfied the patterns are correct re-run with `-y`/`--yes` to confirm you know what you're doing.
+            \tGoodbye.
+            \t"""))
+            return 3
+
+        return PypiCleanup(**vars(args)).run()
+    finally:
+        logging.shutdown()
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `pypi-cleanup-0.1.5/pypi_cleanup.egg-info/PKG-INFO` & `pypi_cleanup-0.1.6.dev20240420021837/pypi_cleanup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-cleanup
-Version: 0.1.5
+Version: 0.1.6.dev20240420021837
 Summary: PyPI Bulk Release Version Cleanup Utility
 Home-page: https://github.com/arcivanov/pypi-cleanup
 Author: Arcadiy Ivanov
 Author-email: arcadiy@ivanov.biz
 Maintainer: Arcadiy Ivanov
 Maintainer-email: arcadiy@ivanov.biz
 License: Apache License, Version 2.0
```

### Comparing `pypi-cleanup-0.1.5/setup.py` & `pypi_cleanup-0.1.6.dev20240420021837/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'pypi-cleanup',
-        version = '0.1.5',
+        version = '0.1.6.dev20240420021837',
         description = 'PyPI Bulk Release Version Cleanup Utility',
         long_description = '# PyPI Bulk Release Version Cleanup Utility\n\n[![PyPI Cleanup Version](https://img.shields.io/pypi/v/pypi-cleanup?logo=pypi)](https://pypi.org/project/pypi-cleanup/)\n[![PyPI Cleanup Python Versions](https://img.shields.io/pypi/pyversions/pypi-cleanup?logo=pypi)](https://pypi.org/project/pypi-cleanup/)\n[![Build Status](https://img.shields.io/github/actions/workflow/status/arcivanov/pypi-cleanup/pypi-cleanup.yml?branch=master)](https://github.com/arcivanov/pypi-cleanup/actions/workflows/pypi-cleanup.yml)\n[![PyPI Cleanup Downloads Per Day](https://img.shields.io/pypi/dd/pypi-cleanup?logo=pypi)](https://pypi.org/project/pypi-cleanup/)\n[![PyPI Cleanup Downloads Per Week](https://img.shields.io/pypi/dw/pypi-cleanup?logo=pypi)](https://pypi.org/project/pypi-cleanup/)\n[![PyPI Cleanup Downloads Per Month](https://img.shields.io/pypi/dm/pypi-cleanup?logo=pypi)](https://pypi.org/project/pypi-cleanup/)\n\n## Overview\n\nPyPI Bulk Release Version Cleanup Utility (`pypi-cleanup`) is designed to bulk-delete releases from PyPI that match\nspecified patterns.\nThis utility is most useful when CI/CD method produces a swarm of temporary\n[.devN pre-releases](https://www.python.org/dev/peps/pep-0440/#developmental-releases) in between versioned releases.\n\nBeing able to cleanup past .devN junk helps PyPI cut down on the storage requirements and keeps release history neatly\norganized.\n\n## WARNING\n\nTHIS UTILITY IS DESTRUCTIVE AND CAN POTENTIALLY WRECK YOUR PROJECT RELEASES AND MAKE THE PROJECT INACCESSIBLE ON PYPI.\n\nThis utility is provided on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or\nimplied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY,\nor FITNESS FOR A PARTICULAR PURPOSE.\n\n## Details\n\nThe default package release version selection pattern is `r".*dev\\d+$"`.\n\nAuthentication password may be passed via environment variable\n`PYPI_CLEANUP_PASSWORD`. Otherwise, you will be prompted to enter it.\n\nAuthentication with TOTP is supported.\n\nExamples:\n\n```bash\n$ pypi-cleanup --help\nusage: pypi-cleanup [-h] -u USERNAME -p PACKAGE [-t URL] [-r PATTERNS] [--do-it] [-y] [-v]\n\nPyPi Package Cleanup Utility\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -u USERNAME, --username USERNAME\n                        authentication username (default: None)\n  -p PACKAGE, --package PACKAGE\n                        PyPI package name (default: None)\n  -t URL, --host URL    PyPI <proto>://<host> prefix (default: https://pypi.org/)\n  -r PATTERNS, --version-regex PATTERNS\n                        regex to use to match package versions to be deleted (default: None)\n  --do-it               actually perform the destructive delete (default: False)\n  -y, --yes             confirm extremely dangerous destructive delete (default: False)\n  -v, --verbose         be verbose (default: 0)\n```\n\n```bash\n$ pypi-cleanup -u arcivanov -p pybuilder\nPassword: \nAuthentication code: 123456\nINFO:root:Deleting pybuilder version 0.12.3.dev20200421010849\nINFO:root:Deleted pybuilder version 0.12.3.dev20200421010849\nINFO:root:Deleting pybuilder version 0.12.3.dev20200421010857\nINFO:root:Deleted pybuilder version 0.12.3.dev20200421010857\n```\n\n```bash\n$ pypi-cleanup -u arcivanov -p geventmp -n -r \'.*\\\\.dev1$\'\nPassword:\nWARNING:root:RUNNING IN DRY-RUN MODE\nINFO:root:Will use the following patterns [re.compile(\'.*\\\\.dev1$\')] on package geventmp\nAuthentication code: 123456\nINFO:root:Deleting geventmp version 0.0.1.dev1\n```\n',
         long_description_content_type = 'text/markdown',
         classifiers = [
             'Programming Language :: Python',
             'Programming Language :: Python :: Implementation :: CPython',
             'Programming Language :: Python :: Implementation :: PyPy',
```

