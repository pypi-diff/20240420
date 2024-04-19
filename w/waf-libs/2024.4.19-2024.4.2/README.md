# Comparing `tmp/waf-libs-2024.4.19.tar.gz` & `tmp/waf-libs-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/waf-libs-2024.4.19.tar", last modified: Fri Apr 19 23:38:06 2024, max compression
+gzip compressed data, was "dist/waf-libs-2024.4.2.tar", last modified: Wed Apr  3 01:32:36 2024, max compression
```

## Comparing `waf-libs-2024.4.19.tar` & `waf-libs-2024.4.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 23:38:06.000000 waf-libs-2024.4.19/
--rw-rw-rw-   0 root         (0) root         (0)    11348 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1029 2024-04-19 23:38:06.000000 waf-libs-2024.4.19/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      228 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/README.rst
--rw-rw-rw-   0 root         (0) root         (0)       10 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/VERSION
--rw-rw-rw-   0 root         (0) root         (0)      590 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       76 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-19 23:38:06.000000 waf-libs-2024.4.19/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 23:38:06.000000 waf-libs-2024.4.19/source/
--rw-rw-rw-   0 root         (0) root         (0)     5860 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 23:38:06.000000 waf-libs-2024.4.19/source/waf_libs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1029 2024-04-19 23:38:06.000000 waf-libs-2024.4.19/source/waf_libs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      996 2024-04-19 23:38:06.000000 waf-libs-2024.4.19/source/waf_libs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 23:38:06.000000 waf-libs-2024.4.19/source/waf_libs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       98 2024-04-19 23:38:06.000000 waf-libs-2024.4.19/source/waf_libs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-19 23:38:06.000000 waf-libs-2024.4.19/source/waf_libs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 23:38:06.000000 waf-libs-2024.4.19/source/waflibs/
--rw-rw-rw-   0 root         (0) root         (0)      394 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/source/waflibs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1886 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/source/waflibs/arg_parse.py
--rw-rw-rw-   0 root         (0) root         (0)     1128 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/source/waflibs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2354 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/source/waflibs/config.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/source/waflibs/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/source/waflibs/database.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 23:38:06.000000 waf-libs-2024.4.19/source/waflibs/dns/
--rw-rw-rw-   0 root         (0) root         (0)     1993 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/source/waflibs/dns/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6757 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/source/waflibs/dns/bind.py
--rw-rw-rw-   0 root         (0) root         (0)    16108 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/source/waflibs/dns/mysql.py
--rw-rw-rw-   0 root         (0) root         (0)      226 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/source/waflibs/domain.py
--rw-rw-rw-   0 root         (0) root         (0)      226 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/source/waflibs/error.py
--rw-rw-rw-   0 root         (0) root         (0)     3519 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/source/waflibs/filedir.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/source/waflibs/git.py
--rw-rw-rw-   0 root         (0) root         (0)     1471 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/source/waflibs/log.py
--rw-rw-rw-   0 root         (0) root         (0)     1016 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/source/waflibs/text.py
--rw-rw-rw-   0 root         (0) root         (0)      879 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/source/waflibs/uri.py
--rw-rw-rw-   0 root         (0) root         (0)     1953 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/source/waflibs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 23:38:06.000000 waf-libs-2024.4.19/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 23:38:06.000000 waf-libs-2024.4.19/tests/dns/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/tests/dns/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4049 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/tests/dns/test_bind.py
--rw-rw-rw-   0 root         (0) root         (0)     2223 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/tests/dns/test_mysql.py
--rw-rw-rw-   0 root         (0) root         (0)     4846 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1285 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/tests/test_database.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/tests/test_dns.py
--rw-rw-rw-   0 root         (0) root         (0)      357 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/tests/test_domain.py
--rw-rw-rw-   0 root         (0) root         (0)     1662 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/tests/test_filedir.py
--rw-rw-rw-   0 root         (0) root         (0)     1124 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/tests/test_log.py
--rw-rw-rw-   0 root         (0) root         (0)      667 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/tests/test_text.py
--rw-rw-rw-   0 root         (0) root         (0)     1321 2024-04-19 23:37:46.000000 waf-libs-2024.4.19/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)    11348 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1028 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      228 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)        9 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      590 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/source/
+-rw-rw-rw-   0 root         (0) root         (0)     5860 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/source/waf_libs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1028 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/source/waf_libs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      996 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/source/waf_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/source/waf_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/source/waf_libs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/source/waf_libs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/source/waflibs/
+-rw-rw-rw-   0 root         (0) root         (0)      394 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/arg_parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2190 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/database.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/source/waflibs/dns/
+-rw-rw-rw-   0 root         (0) root         (0)     1993 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/dns/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6757 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/dns/bind.py
+-rw-rw-rw-   0 root         (0) root         (0)    16108 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/dns/mysql.py
+-rw-rw-rw-   0 root         (0) root         (0)      226 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      226 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/error.py
+-rw-rw-rw-   0 root         (0) root         (0)     3519 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/filedir.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/git.py
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      879 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/uri.py
+-rw-rw-rw-   0 root         (0) root         (0)     1953 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/tests/dns/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/dns/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4049 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/dns/test_bind.py
+-rw-rw-rw-   0 root         (0) root         (0)     2223 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/dns/test_mysql.py
+-rw-rw-rw-   0 root         (0) root         (0)     4846 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/test_database.py
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/test_dns.py
+-rw-rw-rw-   0 root         (0) root         (0)      357 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/test_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     1662 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/test_filedir.py
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/test_log.py
+-rw-rw-rw-   0 root         (0) root         (0)      667 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/test_text.py
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/test_utils.py
```

### Comparing `waf-libs-2024.4.19/LICENSE` & `waf-libs-2024.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/PKG-INFO` & `waf-libs-2024.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waf-libs
-Version: 2024.4.19
+Version: 2024.4.2
 Summary: waf libs
 Home-page: https://bitbucket.org/waf/waf-libs
 Author: Felix Wong
 Author-email: felix@waf.hk
 License: Apache
 Description: ============
         waf-libs
```

### Comparing `waf-libs-2024.4.19/pyproject.toml` & `waf-libs-2024.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/setup.py` & `waf-libs-2024.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/source/conf.py` & `waf-libs-2024.4.2/source/conf.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/source/waf_libs.egg-info/PKG-INFO` & `waf-libs-2024.4.2/source/waf_libs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waf-libs
-Version: 2024.4.19
+Version: 2024.4.2
 Summary: waf libs
 Home-page: https://bitbucket.org/waf/waf-libs
 Author: Felix Wong
 Author-email: felix@waf.hk
 License: Apache
 Description: ============
         waf-libs
```

### Comparing `waf-libs-2024.4.19/source/waf_libs.egg-info/SOURCES.txt` & `waf-libs-2024.4.2/source/waf_libs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/source/waflibs/arg_parse.py` & `waf-libs-2024.4.2/source/waflibs/arg_parse.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/source/waflibs/conf.py` & `waf-libs-2024.4.2/source/waflibs/conf.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/source/waflibs/config.py` & `waf-libs-2024.4.2/source/waflibs/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,48 +45,45 @@
             for text in secret_text:
                 if text in k:
                     config_dict[k] = "REDACTED"
 
     return config_dict
 
 
-def get_config_filename(fname, ignore_suffix=False):
+def get_config_filename(fname):
     """get config filename"""
 
     logger.debug(f"config filename: {fname}")
 
     file = pathlib.Path(fname)
-    if not ignore_suffix:
-        exts = [
-            "yml",
-            "yaml",
-        ]
+    exts = [
+        "yml",
+        "yaml",
+    ]
 
-        filename = None
-        for ext in exts:
-            suffix = f".{ext}"
-            logger.debug(f"suffix: {suffix}")
-            file_suffix = file.suffix
-            logger.debug(f"file suffix: {file_suffix}")
+    filename = None
+    for ext in exts:
+        suffix = f".{ext}"
+        logger.debug(f"suffix: {suffix}")
+        file_suffix = file.suffix
+        logger.debug(f"file suffix: {file_suffix}")
 
-            if file_suffix == suffix:
-                logger.debug(f"filename: {filename}")
+        if file_suffix == suffix:
+            logger.debug(f"filename: {filename}")
 
-                file = file.with_suffix(suffix)
+            return file.with_suffix(suffix)
 
-    return file
 
-
-def parse_yaml_file(fname, ignore_suffix=False):
+def parse_yaml_file(fname):
     """parse yaml config by filename"""
 
-    filename = get_config_filename(fname, ignore_suffix)
+    filename = get_config_filename(fname)
 
     if not filename:
-        raise Exception(f"no yaml config file found at {fname}")
+        raise Exception("no yaml config file found")
     else:
         with open(pathlib.Path(filename)) as f:
             config = parse_yaml(f.read())
 
         return config
```

### Comparing `waf-libs-2024.4.19/source/waflibs/constants.py` & `waf-libs-2024.4.2/source/waflibs/constants.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/source/waflibs/database.py` & `waf-libs-2024.4.2/source/waflibs/database.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/source/waflibs/dns/__init__.py` & `waf-libs-2024.4.2/source/waflibs/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/source/waflibs/dns/bind.py` & `waf-libs-2024.4.2/source/waflibs/dns/bind.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/source/waflibs/dns/mysql.py` & `waf-libs-2024.4.2/source/waflibs/dns/mysql.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/source/waflibs/filedir.py` & `waf-libs-2024.4.2/source/waflibs/filedir.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/source/waflibs/git.py` & `waf-libs-2024.4.2/source/waflibs/git.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/source/waflibs/log.py` & `waf-libs-2024.4.2/source/waflibs/log.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/source/waflibs/text.py` & `waf-libs-2024.4.2/source/waflibs/text.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,25 +28,18 @@
     else:
         print(output)
 
 
 def stderrprint(*args, **kwargs):
     logger.debug(f"original kwargs: {kwargs}")
 
-    output = sys.stderr
-    if "stdout" in kwargs and kwargs["stdout"]:
-        output = sys.stdout
-        kwargs.pop("stdout")
-    logger.debug(f"file output is {output.name}")
-
     if "newline" in kwargs and not kwargs["newline"]:
         kwargs["flush"] = True
         kwargs["end"] = ""
         kwargs.pop("newline")
     logger.debug(f"after kwargs: {kwargs}")
 
-    print(*args, **kwargs, file=output)
+    print(*args, **kwargs, file=sys.stderr)
 
 
 eprint = stderrprint
 errprint = stderrprint
-errorprint = stderrprint
```

### Comparing `waf-libs-2024.4.19/source/waflibs/uri.py` & `waf-libs-2024.4.2/source/waflibs/uri.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/source/waflibs/utils.py` & `waf-libs-2024.4.2/source/waflibs/utils.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/tests/dns/test_bind.py` & `waf-libs-2024.4.2/tests/dns/test_bind.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/tests/dns/test_mysql.py` & `waf-libs-2024.4.2/tests/dns/test_mysql.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/tests/test_config.py` & `waf-libs-2024.4.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/tests/test_database.py` & `waf-libs-2024.4.2/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/tests/test_dns.py` & `waf-libs-2024.4.2/tests/test_dns.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/tests/test_filedir.py` & `waf-libs-2024.4.2/tests/test_filedir.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/tests/test_log.py` & `waf-libs-2024.4.2/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/tests/test_text.py` & `waf-libs-2024.4.2/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.4.19/tests/test_utils.py` & `waf-libs-2024.4.2/tests/test_utils.py`

 * *Files identical despite different names*

