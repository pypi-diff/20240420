# Comparing `tmp/ryutils-4.0.2.tar.gz` & `tmp/ryutils-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryutils-4.0.2.tar", last modified: Sat Apr 20 18:09:21 2024, max compression
+gzip compressed data, was "ryutils-4.0.3.tar", last modified: Sat Apr 20 18:11:32 2024, max compression
```

## Comparing `ryutils-4.0.2.tar` & `ryutils-4.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:09:21.412836 ryutils-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 18:09:17.000000 ryutils-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 18:09:17.000000 ryutils-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-20 18:09:21.412836 ryutils-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-20 18:09:17.000000 ryutils-4.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 18:09:17.000000 ryutils-4.0.2/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-20 18:09:17.000000 ryutils-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-20 18:09:17.000000 ryutils-4.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:09:21.412836 ryutils-4.0.2/ryutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/dict_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/email_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/fmt_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/short_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:09:21.412836 ryutils-4.0.2/ryutils/sms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/sms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/sms/telegram_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/sms/twilio_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/wait.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-20 18:09:17.000000 ryutils-4.0.2/ryutils/web2_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:09:21.412836 ryutils-4.0.2/ryutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-20 18:09:21.000000 ryutils-4.0.2/ryutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-20 18:09:21.000000 ryutils-4.0.2/ryutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:09:21.000000 ryutils-4.0.2/ryutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-20 18:09:21.000000 ryutils-4.0.2/ryutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 18:09:21.000000 ryutils-4.0.2/ryutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:09:21.412836 ryutils-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-20 18:09:17.000000 ryutils-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:11:32.064527 ryutils-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 18:11:23.000000 ryutils-4.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 18:11:23.000000 ryutils-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-20 18:11:32.064527 ryutils-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-20 18:11:23.000000 ryutils-4.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 18:11:23.000000 ryutils-4.0.3/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-20 18:11:23.000000 ryutils-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-20 18:11:23.000000 ryutils-4.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:11:32.064527 ryutils-4.0.3/ryutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/dict_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/email_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/fmt_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12360 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/short_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:11:32.064527 ryutils-4.0.3/ryutils/sms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/sms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/sms/telegram_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/sms/twilio_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/wait.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-20 18:11:23.000000 ryutils-4.0.3/ryutils/web2_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:11:32.064527 ryutils-4.0.3/ryutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-20 18:11:32.000000 ryutils-4.0.3/ryutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-20 18:11:32.000000 ryutils-4.0.3/ryutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:11:32.000000 ryutils-4.0.3/ryutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-20 18:11:32.000000 ryutils-4.0.3/ryutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 18:11:32.000000 ryutils-4.0.3/ryutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:11:32.064527 ryutils-4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-20 18:11:23.000000 ryutils-4.0.3/setup.py
```

### Comparing `ryutils-4.0.2/LICENSE` & `ryutils-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.2/PKG-INFO` & `ryutils-4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryutils
-Version: 4.0.2
+Version: 4.0.3
 Summary: A collection of utilities for Python
 Author: Ross Yeager
 Author-email: ryeager12@email.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ryutils-4.0.2/pyproject.toml` & `ryutils-4.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.2/requirements.txt` & `ryutils-4.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.2/ryutils/async_utils.py` & `ryutils-4.0.3/ryutils/async_utils.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.2/ryutils/csv_logger.py` & `ryutils-4.0.3/ryutils/csv_logger.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.2/ryutils/dict_util.py` & `ryutils-4.0.3/ryutils/dict_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.2/ryutils/email_util.py` & `ryutils-4.0.3/ryutils/email_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.2/ryutils/fmt_util.py` & `ryutils-4.0.3/ryutils/fmt_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.2/ryutils/log.py` & `ryutils-4.0.3/ryutils/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,16 @@
     def printer(message, *args, **kwargs):
         is_logger_in_use = logging.getLogger().hasHandlers()
 
         # obtain the backtrace of the caller to use as the key
         frame = sys._getframe(1)  # pylint: disable=protected-access
         key = frame.f_code.co_filename + frame.f_code.co_name + str(frame.f_lineno)
         if key not in _DOWNSAMPLER and downsample > 1:
-            _DOWNSAMPLER[key] = {"downsample": downsample, "count": 0}
+            # set the count to downsample - 1 so that the first message is always printed
+            _DOWNSAMPLER[key] = {"downsample": downsample, "count": downsample - 1}
 
         if _ALWAYS_PRINT:
             print(formatter(message, *args, **kwargs))
         elif key in _DOWNSAMPLER:
             _DOWNSAMPLER[key]["count"] += 1
             if _DOWNSAMPLER[key]["count"] % _DOWNSAMPLER[key]["downsample"] == 0:
                 print(formatter(message, *args, **kwargs))
```

### Comparing `ryutils-4.0.2/ryutils/proxies.py` & `ryutils-4.0.3/ryutils/proxies.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.2/ryutils/sms/telegram_util.py` & `ryutils-4.0.3/ryutils/sms/telegram_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.2/ryutils/sms/twilio_util.py` & `ryutils-4.0.3/ryutils/sms/twilio_util.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.2/ryutils/web2_client.py` & `ryutils-4.0.3/ryutils/web2_client.py`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.2/ryutils.egg-info/PKG-INFO` & `ryutils-4.0.3/ryutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryutils
-Version: 4.0.2
+Version: 4.0.3
 Summary: A collection of utilities for Python
 Author: Ross Yeager
 Author-email: ryeager12@email.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ryutils-4.0.2/ryutils.egg-info/SOURCES.txt` & `ryutils-4.0.3/ryutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ryutils-4.0.2/setup.py` & `ryutils-4.0.3/setup.py`

 * *Files identical despite different names*

