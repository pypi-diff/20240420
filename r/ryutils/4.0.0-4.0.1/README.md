# Comparing `tmp/ryutils-4.0.0.tar.gz` & `tmp/ryutils-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryutils-4.0.0.tar", last modified: Mon Apr  8 06:35:47 2024, max compression
+gzip compressed data, was "ryutils-4.0.1.tar", last modified: Sat Apr 20 18:07:09 2024, max compression
```

## Comparing `ryutils-4.0.0.tar` & `ryutils-4.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:35:47.647941 ryutils-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 06:35:43.000000 ryutils-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 06:35:43.000000 ryutils-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-08 06:35:47.647941 ryutils-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-08 06:35:43.000000 ryutils-4.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 06:35:43.000000 ryutils-4.0.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-08 06:35:43.000000 ryutils-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-08 06:35:43.000000 ryutils-4.0.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:35:47.643941 ryutils-4.0.0/ryutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/dict_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/email_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/fmt_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/short_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:35:47.647941 ryutils-4.0.0/ryutils/sms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/sms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/sms/telegram_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/sms/twilio_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/wait.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-08 06:35:43.000000 ryutils-4.0.0/ryutils/web2_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:35:47.647941 ryutils-4.0.0/ryutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-08 06:35:47.000000 ryutils-4.0.0/ryutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-08 06:35:47.000000 ryutils-4.0.0/ryutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 06:35:47.000000 ryutils-4.0.0/ryutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-08 06:35:47.000000 ryutils-4.0.0/ryutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 06:35:47.000000 ryutils-4.0.0/ryutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 06:35:47.647941 ryutils-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-08 06:35:43.000000 ryutils-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:07:09.395790 ryutils-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 18:07:00.000000 ryutils-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 18:07:00.000000 ryutils-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-20 18:07:09.395790 ryutils-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-20 18:07:00.000000 ryutils-4.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 18:07:00.000000 ryutils-4.0.1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-20 18:07:00.000000 ryutils-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-20 18:07:00.000000 ryutils-4.0.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:07:09.395790 ryutils-4.0.1/ryutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/dict_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/email_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/fmt_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12023 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/short_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:07:09.395790 ryutils-4.0.1/ryutils/sms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/sms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/sms/telegram_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/sms/twilio_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/wait.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-20 18:07:00.000000 ryutils-4.0.1/ryutils/web2_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:07:09.395790 ryutils-4.0.1/ryutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-20 18:07:09.000000 ryutils-4.0.1/ryutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-20 18:07:09.000000 ryutils-4.0.1/ryutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:07:09.000000 ryutils-4.0.1/ryutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-20 18:07:09.000000 ryutils-4.0.1/ryutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 18:07:09.000000 ryutils-4.0.1/ryutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:07:09.395790 ryutils-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-20 18:07:00.000000 ryutils-4.0.1/setup.py
```

### Comparing `ryutils-4.0.0/LICENSE` & `ryutils-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.0/PKG-INFO` & `ryutils-4.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryutils
-Version: 4.0.0
+Version: 4.0.1
 Summary: A collection of utilities for Python
 Author: Ross Yeager
 Author-email: ryeager12@email.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ryutils-4.0.0/pyproject.toml` & `ryutils-4.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.0/requirements.txt` & `ryutils-4.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.0/ryutils/async_utils.py` & `ryutils-4.0.1/ryutils/async_utils.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.0/ryutils/csv_logger.py` & `ryutils-4.0.1/ryutils/csv_logger.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.0/ryutils/dict_util.py` & `ryutils-4.0.1/ryutils/dict_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.0/ryutils/email_util.py` & `ryutils-4.0.1/ryutils/email_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 def is_valid_email(email: str) -> bool:
     regex = r"\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,7}\b"
     return re.fullmatch(regex, email) is not None
 
 
 def get_email_accounts_from_password(
-    encrypted_emails: T.List[T.Dict[str, str]],
+    emails: T.List[T.Dict[str, str]],
     dry_run: bool = False,
 ) -> T.List[Email]:
     email_accounts = []
-    for email_account in encrypted_emails:
+    for email_account in emails:
         assert email_account["password"], "Missing password!"
         email_password = email_account["password"]
         email_accounts.append(
             Email(
                 address=email_account["user"],
                 password=email_password,
                 quiet=dry_run,
```

### Comparing `ryutils-4.0.0/ryutils/fmt_util.py` & `ryutils-4.0.1/ryutils/fmt_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.0/ryutils/log.py` & `ryutils-4.0.1/ryutils/log.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import tarfile
 import time
 import typing as T
 
 from ryutils.file_util import make_sure_path_exists
 
 _ALWAYS_PRINT = False
+_DOWNSAMPLER: T.Dict[str, T.Dict[int, int]] = {}
+_DOWNSAMPLE_COUNT = 20
 
 
 class Colors(enum.Enum):
     HEADER = "\033[95m"
     OKBLUE = "\033[94m"
     OKCYAN = "\033[96m"
     OKGREEN = "\033[92m"
@@ -137,14 +139,15 @@
 
 
 def make_formatter_printer(
     color: str,
     log_level: int = logging.INFO,
     prefix: str = "",
     return_formatter: bool = False,
+    downsample: int = 1,
 ) -> T.Callable:
     logger = logging.getLogger(__name__)
 
     def formatter(message, *args, **kwargs):
         message = str(message)
 
         if args or kwargs:
@@ -167,16 +170,29 @@
         if sys.stdout.encoding is not None:
             return formatted_text.encode("utf-8").decode(sys.stdout.encoding, errors="ignore")
 
         return formatted_text
 
     def printer(message, *args, **kwargs):
         is_logger_in_use = logging.getLogger().hasHandlers()
+
+        # obtain the backtrace of the caller to use as the key
+        frame = sys._getframe(1)  # pylint: disable=protected-access
+        key = frame.f_code.co_filename + frame.f_code.co_name + str(frame.f_lineno)
+        if key not in _DOWNSAMPLER and downsample > 1:
+            _DOWNSAMPLER[key] = {"downsample": downsample, "count": 0}
+
         if _ALWAYS_PRINT:
             print(formatter(message, *args, **kwargs))
+        elif key in _DOWNSAMPLER:
+            _DOWNSAMPLER[key]["count"] += 1
+            if _DOWNSAMPLER[key]["count"] % _DOWNSAMPLER[key]["downsample"] == 0:
+                print(formatter(message, *args, **kwargs))
+            else:
+                is_logger_in_use = False
         elif not is_logger_in_use or logging.getLogger().isEnabledFor(log_level):
             print(formatter(message, *args, **kwargs))
 
         if is_logger_in_use:
             if log_level == logging.DEBUG:
                 logger.debug(message)
             elif log_level == logging.WARNING:
@@ -255,14 +271,60 @@
 )
 print_bold = make_formatter_printer(Colors.BOLD.value, log_level=logging.CRITICAL)
 print_normal = make_formatter_printer(Colors.ENDC.value, log_level=logging.DEBUG)
 print_normal_arrow = make_formatter_printer(
     Colors.ENDC.value, prefix=Prefixes.ARROW.value, log_level=logging.DEBUG
 )
 
+print_ok_blue_slow = make_formatter_printer(
+    Colors.OKBLUE.value, log_level=logging.INFO, downsample=_DOWNSAMPLE_COUNT
+)
+print_ok_blue_arrow_slow = make_formatter_printer(
+    Colors.OKBLUE.value,
+    prefix=Prefixes.ARROW.value,
+    log_level=logging.INFO,
+    downsample=_DOWNSAMPLE_COUNT,
+)
+print_ok_slow = make_formatter_printer(
+    Colors.OKGREEN.value, log_level=logging.CRITICAL, downsample=_DOWNSAMPLE_COUNT
+)
+print_ok_arrow_slow = make_formatter_printer(
+    Colors.OKGREEN.value,
+    prefix=Prefixes.ARROW.value,
+    log_level=logging.CRITICAL,
+    downsample=_DOWNSAMPLE_COUNT,
+)
+print_bright_slow = make_formatter_printer(
+    Colors.OKCYAN.value, log_level=logging.WARNING, downsample=_DOWNSAMPLE_COUNT
+)
+print_warn_slow = make_formatter_printer(
+    Colors.WARNING.value, log_level=logging.WARNING, downsample=_DOWNSAMPLE_COUNT
+)
+print_fail_slow = make_formatter_printer(
+    Colors.FAIL.value, log_level=logging.CRITICAL, downsample=_DOWNSAMPLE_COUNT
+)
+print_fail_arrow_slow = make_formatter_printer(
+    Colors.FAIL.value,
+    prefix=Prefixes.ARROW.value,
+    log_level=logging.CRITICAL,
+    downsample=_DOWNSAMPLE_COUNT,
+)
+print_bold_slow = make_formatter_printer(
+    Colors.BOLD.value, log_level=logging.CRITICAL, downsample=_DOWNSAMPLE_COUNT
+)
+print_normal_slow = make_formatter_printer(
+    Colors.ENDC.value, log_level=logging.DEBUG, downsample=_DOWNSAMPLE_COUNT
+)
+print_normal_arrow_slow = make_formatter_printer(
+    Colors.ENDC.value,
+    prefix=Prefixes.ARROW.value,
+    log_level=logging.DEBUG,
+    downsample=_DOWNSAMPLE_COUNT,
+)
+
 
 format_ok_blue = make_formatter_printer(Colors.OKBLUE.value, return_formatter=True)
 format_ok = make_formatter_printer(Colors.OKGREEN.value, return_formatter=True)
 format_bright = make_formatter_printer(Colors.OKCYAN.value, return_formatter=True)
 format_warn = make_formatter_printer(Colors.WARNING.value, return_formatter=True)
 format_fail = make_formatter_printer(Colors.FAIL.value, return_formatter=True)
 format_bold = make_formatter_printer(Colors.BOLD.value, return_formatter=True)
```

### Comparing `ryutils-4.0.0/ryutils/proxies.py` & `ryutils-4.0.1/ryutils/proxies.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.0/ryutils/sms/telegram_util.py` & `ryutils-4.0.1/ryutils/sms/telegram_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.0/ryutils/sms/twilio_util.py` & `ryutils-4.0.1/ryutils/sms/twilio_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.0/ryutils/web2_client.py` & `ryutils-4.0.1/ryutils/web2_client.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.0/ryutils.egg-info/PKG-INFO` & `ryutils-4.0.1/ryutils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryutils
-Version: 4.0.0
+Version: 4.0.1
 Summary: A collection of utilities for Python
 Author: Ross Yeager
 Author-email: ryeager12@email.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ryutils-4.0.0/ryutils.egg-info/SOURCES.txt` & `ryutils-4.0.1/ryutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.0/setup.py` & `ryutils-4.0.1/setup.py`

 * *Files identical despite different names*

