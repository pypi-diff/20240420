# Comparing `tmp/ryutils-4.0.1.tar.gz` & `tmp/ryutils-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryutils-4.0.1.tar", last modified: Sat Apr 20 18:07:09 2024, max compression
+gzip compressed data, was "ryutils-4.0.2.tar", last modified: Sat Apr 20 18:09:21 2024, max compression
```

## Comparing `ryutils-4.0.1.tar` & `ryutils-4.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:07:09.395790 ryutils-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 18:07:00.000000 ryutils-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 18:07:00.000000 ryutils-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-20 18:07:09.395790 ryutils-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-20 18:07:00.000000 ryutils-4.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 18:07:00.000000 ryutils-4.0.1/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-20 18:07:00.000000 ryutils-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-20 18:07:00.000000 ryutils-4.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:07:09.395790 ryutils-4.0.1/ryutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/dict_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/email_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/fmt_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    12023 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/short_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:07:09.395790 ryutils-4.0.1/ryutils/sms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/sms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/sms/telegram_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/sms/twilio_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/wait.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/web2_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:07:09.395790 ryutils-4.0.1/ryutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-20 18:07:09.000000 ryutils-4.0.1/ryutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-20 18:07:09.000000 ryutils-4.0.1/ryutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:07:09.000000 ryutils-4.0.1/ryutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-20 18:07:09.000000 ryutils-4.0.1/ryutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 18:07:09.000000 ryutils-4.0.1/ryutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:07:09.395790 ryutils-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-20 18:07:00.000000 ryutils-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:09:21.412836 ryutils-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 18:09:17.000000 ryutils-4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 18:09:17.000000 ryutils-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-20 18:09:21.412836 ryutils-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-20 18:09:17.000000 ryutils-4.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 18:09:17.000000 ryutils-4.0.2/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-20 18:09:17.000000 ryutils-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-20 18:09:17.000000 ryutils-4.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:09:21.412836 ryutils-4.0.2/ryutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/dict_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/email_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/fmt_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/short_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:09:21.412836 ryutils-4.0.2/ryutils/sms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/sms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/sms/telegram_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/sms/twilio_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/wait.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/web2_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:09:21.412836 ryutils-4.0.2/ryutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-20 18:09:21.000000 ryutils-4.0.2/ryutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-20 18:09:21.000000 ryutils-4.0.2/ryutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:09:21.000000 ryutils-4.0.2/ryutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-20 18:09:21.000000 ryutils-4.0.2/ryutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 18:09:21.000000 ryutils-4.0.2/ryutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:09:21.412836 ryutils-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-20 18:09:17.000000 ryutils-4.0.2/setup.py
```

### Comparing `ryutils-4.0.1/LICENSE` & `ryutils-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.1/PKG-INFO` & `ryutils-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryutils
-Version: 4.0.1
+Version: 4.0.2
 Summary: A collection of utilities for Python
 Author: Ross Yeager
 Author-email: ryeager12@email.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ryutils-4.0.1/pyproject.toml` & `ryutils-4.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.1/requirements.txt` & `ryutils-4.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.1/ryutils/async_utils.py` & `ryutils-4.0.2/ryutils/async_utils.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.1/ryutils/csv_logger.py` & `ryutils-4.0.2/ryutils/csv_logger.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.1/ryutils/dict_util.py` & `ryutils-4.0.2/ryutils/dict_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.1/ryutils/email_util.py` & `ryutils-4.0.2/ryutils/email_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.1/ryutils/fmt_util.py` & `ryutils-4.0.2/ryutils/fmt_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.1/ryutils/log.py` & `ryutils-4.0.2/ryutils/log.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 import sys
 import tarfile
 import time
 import typing as T
 
 from ryutils.file_util import make_sure_path_exists
 
+_DEFAULT_DOWNSAMPLE_COUNT = 20
 _ALWAYS_PRINT = False
 _DOWNSAMPLER: T.Dict[str, T.Dict[int, int]] = {}
-_DOWNSAMPLE_COUNT = 20
+_DOWNSAMPLE_COUNT = _DEFAULT_DOWNSAMPLE_COUNT
 
 
 class Colors(enum.Enum):
     HEADER = "\033[95m"
     OKBLUE = "\033[94m"
     OKCYAN = "\033[96m"
     OKGREEN = "\033[92m"
@@ -233,17 +234,25 @@
     with tarfile.open(tar_name, "w:gz") as tar:
         tar.add(logs_dir, arcname="logs")
 
     if remove_after:
         shutil.rmtree(logs_dir)
 
 
-def setup_log(log_level: str, log_dir: str, id_string: str, always_print: bool = False) -> None:
+def setup_log(
+    log_level: str,
+    log_dir: str,
+    id_string: str,
+    always_print: bool = False,
+    downsample_count: int = _DEFAULT_DOWNSAMPLE_COUNT,
+) -> None:
     global _ALWAYS_PRINT  # pylint: disable=global-statement
+    global _DOWNSAMPLE_COUNT  # pylint: disable=global-statement
     _ALWAYS_PRINT = always_print
+    _DOWNSAMPLE_COUNT = downsample_count
 
     if log_level == "NONE":
         return
 
     log_file = os.path.join(log_dir, f"{id_string}.log")
 
     logging.basicConfig(
```

### Comparing `ryutils-4.0.1/ryutils/proxies.py` & `ryutils-4.0.2/ryutils/proxies.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.1/ryutils/sms/telegram_util.py` & `ryutils-4.0.2/ryutils/sms/telegram_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.1/ryutils/sms/twilio_util.py` & `ryutils-4.0.2/ryutils/sms/twilio_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.1/ryutils/web2_client.py` & `ryutils-4.0.2/ryutils/web2_client.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.1/ryutils.egg-info/PKG-INFO` & `ryutils-4.0.2/ryutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryutils
-Version: 4.0.1
+Version: 4.0.2
 Summary: A collection of utilities for Python
 Author: Ross Yeager
 Author-email: ryeager12@email.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ryutils-4.0.1/ryutils.egg-info/SOURCES.txt` & `ryutils-4.0.2/ryutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.1/setup.py` & `ryutils-4.0.2/setup.py`

 * *Files identical despite different names*

