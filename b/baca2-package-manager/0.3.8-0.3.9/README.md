# Comparing `tmp/baca2-package-manager-0.3.8.tar.gz` & `tmp/baca2-package-manager-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baca2-package-manager-0.3.8.tar", last modified: Thu Feb 29 22:53:25 2024, max compression
+gzip compressed data, was "baca2-package-manager-0.3.9.tar", last modified: Thu Mar 14 20:00:16 2024, max compression
```

## Comparing `baca2-package-manager-0.3.8.tar` & `baca2-package-manager-0.3.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:53:25.575507 baca2-package-manager-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-29 22:53:21.000000 baca2-package-manager-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-02-29 22:53:25.575507 baca2-package-manager-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-29 22:53:21.000000 baca2-package-manager-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:53:25.571507 baca2-package-manager-0.3.8/baca2PackageManager/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-29 22:53:21.000000 baca2-package-manager-0.3.8/baca2PackageManager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-02-29 22:53:21.000000 baca2-package-manager-0.3.8/baca2PackageManager/broker_communication.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-29 22:53:21.000000 baca2-package-manager-0.3.8/baca2PackageManager/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    13025 2024-02-29 22:53:21.000000 baca2-package-manager-0.3.8/baca2PackageManager/judge_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    34927 2024-02-29 22:53:21.000000 baca2-package-manager-0.3.8/baca2PackageManager/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-02-29 22:53:21.000000 baca2-package-manager-0.3.8/baca2PackageManager/manager_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-02-29 22:53:21.000000 baca2-package-manager-0.3.8/baca2PackageManager/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-02-29 22:53:21.000000 baca2-package-manager-0.3.8/baca2PackageManager/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-02-29 22:53:21.000000 baca2-package-manager-0.3.8/baca2PackageManager/zipper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:53:25.575507 baca2-package-manager-0.3.8/baca2_package_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-02-29 22:53:25.000000 baca2-package-manager-0.3.8/baca2_package_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-29 22:53:25.000000 baca2-package-manager-0.3.8/baca2_package_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 22:53:25.000000 baca2-package-manager-0.3.8/baca2_package_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-29 22:53:25.000000 baca2-package-manager-0.3.8/baca2_package_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-29 22:53:25.000000 baca2-package-manager-0.3.8/baca2_package_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 22:53:25.575507 baca2-package-manager-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-02-29 22:53:21.000000 baca2-package-manager-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:53:25.575507 baca2-package-manager-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 22:53:21.000000 baca2-package-manager-0.3.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9968 2024-02-29 22:53:21.000000 baca2-package-manager-0.3.8/tests/test_judge_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    28808 2024-02-29 22:53:21.000000 baca2-package-manager-0.3.8/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-02-29 22:53:21.000000 baca2-package-manager-0.3.8/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-02-29 22:53:21.000000 baca2-package-manager-0.3.8/tests/test_zipper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 20:00:16.578169 baca2-package-manager-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-14 20:00:09.000000 baca2-package-manager-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-14 20:00:16.578169 baca2-package-manager-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-14 20:00:09.000000 baca2-package-manager-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 20:00:16.574169 baca2-package-manager-0.3.9/baca2PackageManager/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-14 20:00:09.000000 baca2-package-manager-0.3.9/baca2PackageManager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-03-14 20:00:09.000000 baca2-package-manager-0.3.9/baca2PackageManager/broker_communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-14 20:00:09.000000 baca2-package-manager-0.3.9/baca2PackageManager/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13025 2024-03-14 20:00:09.000000 baca2-package-manager-0.3.9/baca2PackageManager/judge_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35178 2024-03-14 20:00:09.000000 baca2-package-manager-0.3.9/baca2PackageManager/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-14 20:00:09.000000 baca2-package-manager-0.3.9/baca2PackageManager/manager_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-14 20:00:09.000000 baca2-package-manager-0.3.9/baca2PackageManager/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-03-14 20:00:09.000000 baca2-package-manager-0.3.9/baca2PackageManager/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-03-14 20:00:09.000000 baca2-package-manager-0.3.9/baca2PackageManager/zipper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 20:00:16.578169 baca2-package-manager-0.3.9/baca2_package_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-14 20:00:16.000000 baca2-package-manager-0.3.9/baca2_package_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-14 20:00:16.000000 baca2-package-manager-0.3.9/baca2_package_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 20:00:16.000000 baca2-package-manager-0.3.9/baca2_package_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-14 20:00:16.000000 baca2-package-manager-0.3.9/baca2_package_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-14 20:00:16.000000 baca2-package-manager-0.3.9/baca2_package_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 20:00:16.578169 baca2-package-manager-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-14 20:00:09.000000 baca2-package-manager-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 20:00:16.578169 baca2-package-manager-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 20:00:09.000000 baca2-package-manager-0.3.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9968 2024-03-14 20:00:09.000000 baca2-package-manager-0.3.9/tests/test_judge_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28808 2024-03-14 20:00:09.000000 baca2-package-manager-0.3.9/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-14 20:00:09.000000 baca2-package-manager-0.3.9/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-03-14 20:00:09.000000 baca2-package-manager-0.3.9/tests/test_zipper.py
```

### Comparing `baca2-package-manager-0.3.8/LICENSE` & `baca2-package-manager-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `baca2-package-manager-0.3.8/PKG-INFO` & `baca2-package-manager-0.3.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baca2-package-manager
-Version: 0.3.8
+Version: 0.3.9
 Summary: A package manager for Baca2 project
 Home-page: https://github.com/BaCa2-project/BaCa2-package-manager
 Author: Baca2 Team
 Author-email: bartosz.deptula@student.uj.edu.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `baca2-package-manager-0.3.8/baca2PackageManager/__init__.py` & `baca2-package-manager-0.3.9/baca2PackageManager/__init__.py`

 * *Files identical despite different names*

### Comparing `baca2-package-manager-0.3.8/baca2PackageManager/broker_communication.py` & `baca2-package-manager-0.3.9/baca2PackageManager/broker_communication.py`

 * *Files identical despite different names*

### Comparing `baca2-package-manager-0.3.8/baca2PackageManager/judge_manager.py` & `baca2-package-manager-0.3.9/baca2PackageManager/judge_manager.py`

 * *Files identical despite different names*

### Comparing `baca2-package-manager-0.3.8/baca2PackageManager/manager.py` & `baca2-package-manager-0.3.9/baca2PackageManager/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,19 +118,22 @@
 
         :param validators: A dictionary of validators. The keys are the names of the settings, and the values are lists of
         validators. Each validator is a tuple of the form (function, *args, **kwargs). The function is called with the
         setting value as the first argument, followed by the *
 
         :return: The check variable is being returned.
         """
-        for i, j in self._settings.items():
-            check = False
-            for k in validators[i]:
-                check |= k[0](j, *k[1:])
-        return check
+        return True
+        # for i, j in self._settings.items():
+        #     check = False
+        #     for k in validators[i]:
+        #         check |= k[0](j, *k[1:])
+        #     if not check:
+        #         return False
+        # return True
 
     def save_to_config(self, settings):
         """
         It opens a file called config.yml in the directory specified by the path attribute of the object, and writes the
         settings dictionary to it.
 
         :param settings: The settings to save
@@ -183,14 +186,16 @@
         'memory_limit': [[isSize, MAX_SUBMIT_MEMORY]],
         'source_memory': [[isSize, MAX_SOURCE_SIZE]],
         'time_limit': [[isIntBetween, 0, MAX_SUBMIT_TIME], [isFloatBetween, 0, MAX_SUBMIT_TIME]],
         'allowedExtensions': [[isIn, *SUPPORTED_EXTENSIONS],
                               [isList, *SUPPORTED_EXTENSIONS]],
         'hinter': [[isNone], [isPath]],
         'checker': [[isNone], [isPath]],
+        'verifier': [[isNone], [isPath]],
+        'basename': [[isNone], [isStr]],
         'test_generator': [[isNone], [isPath]],
         'network': [[isNone], [isBool]],
         'cpus': [[isNone], [isIntBetween, 1, MAX_CPUS]]
     }
     """
     Validation for ``Package`` settings.
     
@@ -215,14 +220,16 @@
         'memory_limit': '512M',
         'time_limit': 10,
         'allowedExtensions': 'cpp',
         'hinter': None,
         'checker': None,
         'test_generator': None,
         'network': False,
+        'verifier': None,
+        'basename': None,
         'cpus': 1
     }
 
     # TODO: Add auto-discovery of judge manager files
 
     class DocExtension(Enum):
         """
@@ -676,14 +683,16 @@
         'name': [[isStr]],
         'weight': [[isInt], [isFloat]],
         'points': [[isInt], [isFloat]],
         'memory_limit': [[isNone], [isSize, Package.MAX_SUBMIT_MEMORY]],
         'time_limit': [[isNone], [isIntBetween, 0, Package.MAX_SUBMIT_TIME],
                        [isFloatBetween, 0, Package.MAX_SUBMIT_TIME]],
         'checker': [[isNone], [isPath]],
+        'verifier': [[isNone], [isPath]],
+        'basename': [[isNone], [isPath]],
         'test_generator': [[isNone], [isPath]],
         'tests': [[isNone], [isAny]],
         'makefile': [[isNone], [isPath]]
     }
 
     """
         Validation for ``TSet`` settings.
@@ -702,18 +711,16 @@
     #: Default values for set settings
     DEFAULT_SETTINGS = {
         'name': '_unnamed',
         'weight': 1,
         'points': 0,
         'memory_limit': '512M',
         'time_limit': 1,
-        'checker': None,
-        'test_generator': None,
         'tests': {},
-        'makefile': None
+        'makefile': None,
     }
 
     def __init__(self, path: Path):
         """
         It reads the config file and creates a list of tests
 
         :param path: Path - path to the test set
```

### Comparing `baca2-package-manager-0.3.8/baca2PackageManager/manager_exceptions.py` & `baca2-package-manager-0.3.9/baca2PackageManager/manager_exceptions.py`

 * *Files identical despite different names*

### Comparing `baca2-package-manager-0.3.8/baca2PackageManager/tools.py` & `baca2-package-manager-0.3.9/baca2PackageManager/tools.py`

 * *Files identical despite different names*

### Comparing `baca2-package-manager-0.3.8/baca2PackageManager/validators.py` & `baca2-package-manager-0.3.9/baca2PackageManager/validators.py`

 * *Files identical despite different names*

### Comparing `baca2-package-manager-0.3.8/baca2PackageManager/zipper.py` & `baca2-package-manager-0.3.9/baca2PackageManager/zipper.py`

 * *Files identical despite different names*

### Comparing `baca2-package-manager-0.3.8/baca2_package_manager.egg-info/PKG-INFO` & `baca2-package-manager-0.3.9/baca2_package_manager.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baca2-package-manager
-Version: 0.3.8
+Version: 0.3.9
 Summary: A package manager for Baca2 project
 Home-page: https://github.com/BaCa2-project/BaCa2-package-manager
 Author: Baca2 Team
 Author-email: bartosz.deptula@student.uj.edu.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `baca2-package-manager-0.3.8/baca2_package_manager.egg-info/SOURCES.txt` & `baca2-package-manager-0.3.9/baca2_package_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baca2-package-manager-0.3.8/setup.py` & `baca2-package-manager-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `baca2-package-manager-0.3.8/tests/test_judge_manager.py` & `baca2-package-manager-0.3.9/tests/test_judge_manager.py`

 * *Files identical despite different names*

### Comparing `baca2-package-manager-0.3.8/tests/test_manager.py` & `baca2-package-manager-0.3.9/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `baca2-package-manager-0.3.8/tests/test_tools.py` & `baca2-package-manager-0.3.9/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `baca2-package-manager-0.3.8/tests/test_zipper.py` & `baca2-package-manager-0.3.9/tests/test_zipper.py`

 * *Files identical despite different names*

