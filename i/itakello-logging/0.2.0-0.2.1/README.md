# Comparing `tmp/itakello_logging-0.2.0.tar.gz` & `tmp/itakello_logging-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itakello_logging-0.2.0.tar", last modified: Mon Apr 15 11:07:52 2024, max compression
+gzip compressed data, was "itakello_logging-0.2.1.tar", last modified: Sat Apr 20 13:01:53 2024, max compression
```

## Comparing `itakello_logging-0.2.0.tar` & `itakello_logging-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:51.996027 itakello_logging-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-15 11:07:51.996027 itakello_logging-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:07:51.996027 itakello_logging-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:51.992027 itakello_logging-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:51.996027 itakello_logging-0.2.0/src/itakello_logging/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:51.996027 itakello_logging-0.2.0/src/itakello_logging/filters/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/filters/custom_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/filters/ignore_root.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:51.996027 itakello_logging-0.2.0/src/itakello_logging/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/formatters/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:51.996027 itakello_logging-0.2.0/src/itakello_logging/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/loggers/confirmation_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:51.996027 itakello_logging-0.2.0/src/itakello_logging/test_logs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/test_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-15 11:07:42.000000 itakello_logging-0.2.0/src/itakello_logging/test_logs/test_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:51.996027 itakello_logging-0.2.0/src/itakello_logging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-15 11:07:51.000000 itakello_logging-0.2.0/src/itakello_logging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-15 11:07:51.000000 itakello_logging-0.2.0/src/itakello_logging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:07:51.000000 itakello_logging-0.2.0/src/itakello_logging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 11:07:51.000000 itakello_logging-0.2.0/src/itakello_logging.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:01:53.152658 itakello_logging-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-20 13:01:53.152658 itakello_logging-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 13:01:53.152658 itakello_logging-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:01:53.148658 itakello_logging-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:01:53.148658 itakello_logging-0.2.1/src/itakello_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:01:53.148658 itakello_logging-0.2.1/src/itakello_logging/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/filters/custom_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/filters/ignore_root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:01:53.148658 itakello_logging-0.2.1/src/itakello_logging/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/formatters/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:01:53.148658 itakello_logging-0.2.1/src/itakello_logging/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/loggers/custom_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:01:53.148658 itakello_logging-0.2.1/src/itakello_logging/test_logs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/test_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-20 13:01:39.000000 itakello_logging-0.2.1/src/itakello_logging/test_logs/test_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:01:53.152658 itakello_logging-0.2.1/src/itakello_logging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-20 13:01:53.000000 itakello_logging-0.2.1/src/itakello_logging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-20 13:01:53.000000 itakello_logging-0.2.1/src/itakello_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 13:01:53.000000 itakello_logging-0.2.1/src/itakello_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 13:01:53.000000 itakello_logging-0.2.1/src/itakello_logging.egg-info/top_level.txt
```

### Comparing `itakello_logging-0.2.0/LICENSE` & `itakello_logging-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `itakello_logging-0.2.0/PKG-INFO` & `itakello_logging-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itakello_logging
-Version: 0.2.0
+Version: 0.2.1
 Summary: A custom logging library by Itakello
 Home-page: https://github.com/Itakello/itakello_logging
 Author: Itakello
 Author-email: maxste000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `itakello_logging-0.2.0/README.md` & `itakello_logging-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `itakello_logging-0.2.0/setup.py` & `itakello_logging-0.2.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="itakello_logging",
-    version="0.2.0",
+    version="0.2.1",
     author="Itakello",
     author_email="maxste000@gmail.com",
     description="A custom logging library by Itakello",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Itakello/itakello_logging",
     package_dir={"": "src"},
```

### Comparing `itakello_logging-0.2.0/src/itakello_logging/core.py` & `itakello_logging-0.2.1/src/itakello_logging/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 from dataclasses import dataclass, field
 from datetime import datetime
 from typing import cast
 
 from .filters import CustomExcludeFilter, IgnoreRootFilter
 from .formatters import ConsoleFormatter
-from .loggers import ConfirmationLogger
+from .loggers import CustomLogger
 
 
 @dataclass
 class ItakelloLogging:
 
     debug_mode: bool = field(init=False)
     handlers: list[logging.Handler] = field(init=False)
@@ -18,23 +18,23 @@
 
     def __init__(
         self,
         excluded_modules: list[str] = [],
         debug: bool = False,
         exclude_root: bool = False,
     ) -> None:
-        logging.setLoggerClass(ConfirmationLogger)
+        logging.setLoggerClass(CustomLogger)
         self.debug_mode = debug
         self.folder = self._create_folder("logs")
         handlers = self._get_handlers(excluded_modules, exclude_root)
         logging.basicConfig(level=logging.DEBUG, handlers=handlers, force=True)
 
     @staticmethod
-    def get_logger(name: str) -> ConfirmationLogger:
-        return cast(ConfirmationLogger, logging.getLogger(name))
+    def get_logger(name: str) -> CustomLogger:
+        return cast(CustomLogger, logging.getLogger(name))
 
     def _create_folder(self, f_name: str) -> pathlib.Path:
         folder = pathlib.Path(f_name)
         folder.mkdir(exist_ok=True, parents=True)
         return folder
 
     def _get_handlers(
@@ -58,17 +58,15 @@
         if exclude_root:
             filters.append(IgnoreRootFilter())
         return filters
 
     def _get_stream_handler(self) -> logging.StreamHandler:
         s_handler = logging.StreamHandler()
         s_handler.setLevel(logging.DEBUG if self.debug_mode else logging.INFO)
-        console_formatter = ConsoleFormatter(
-            "%(asctime)s - %(name)s - %(message)s", "%H:%M:%S"
-        )
+        console_formatter = ConsoleFormatter("%(message)s")
         s_handler.setFormatter(console_formatter)
         return s_handler
 
     def _get_file_handler(self) -> logging.FileHandler:
         current_time = datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
         f_handler = logging.FileHandler(self.folder / f"{current_time}.log")
         f_handler.setLevel(logging.DEBUG)
```

### Comparing `itakello_logging-0.2.0/src/itakello_logging/formatters/console.py` & `itakello_logging-0.2.1/src/itakello_logging/formatters/console.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import logging
 
 
 class ConsoleFormatter(logging.Formatter):
     """Custom formatter to add colors to logging levels."""
 
     CONFIRMATION_LEVEL = 25
+    INSTRUCTION_LEVEL = 24
 
     color_codes = {
         logging.DEBUG: "\033[94m",  # Blue
         CONFIRMATION_LEVEL: "\033[92m",  # Green
+        INSTRUCTION_LEVEL: "\033[33m",  # Orange
         logging.WARNING: "\033[93m",  # Yellow
         logging.ERROR: "\033[91m",  # Red
         logging.CRITICAL: "\033[95m",  # Magenta
     }
 
     def format(self, record):
         level_color = self.color_codes.get(
```

### Comparing `itakello_logging-0.2.0/src/itakello_logging.egg-info/PKG-INFO` & `itakello_logging-0.2.1/src/itakello_logging.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itakello_logging
-Version: 0.2.0
+Version: 0.2.1
 Summary: A custom logging library by Itakello
 Home-page: https://github.com/Itakello/itakello_logging
 Author: Itakello
 Author-email: maxste000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `itakello_logging-0.2.0/src/itakello_logging.egg-info/SOURCES.txt` & `itakello_logging-0.2.1/src/itakello_logging.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 src/itakello_logging.egg-info/top_level.txt
 src/itakello_logging/filters/__init__.py
 src/itakello_logging/filters/custom_exclude.py
 src/itakello_logging/filters/ignore_root.py
 src/itakello_logging/formatters/__init__.py
 src/itakello_logging/formatters/console.py
 src/itakello_logging/loggers/__init__.py
-src/itakello_logging/loggers/confirmation_logger.py
+src/itakello_logging/loggers/custom_logger.py
 src/itakello_logging/test_logs/__init__.py
 src/itakello_logging/test_logs/test_logs.py
```

