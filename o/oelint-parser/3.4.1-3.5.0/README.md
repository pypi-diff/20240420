# Comparing `tmp/oelint_parser-3.4.1.tar.gz` & `tmp/oelint_parser-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oelint_parser-3.4.1.tar", last modified: Wed Apr 17 20:21:12 2024, max compression
+gzip compressed data, was "oelint_parser-3.5.0.tar", last modified: Sat Apr 20 06:33:06 2024, max compression
```

## Comparing `oelint_parser-3.4.1.tar` & `oelint_parser-3.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:21:12.713953 oelint_parser-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-17 20:20:53.000000 oelint_parser-3.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-17 20:20:53.000000 oelint_parser-3.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-17 20:21:12.713953 oelint_parser-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-04-17 20:20:53.000000 oelint_parser-3.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:21:12.713953 oelint_parser-3.4.1/oelint_parser/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-17 20:20:53.000000 oelint_parser-3.4.1/oelint_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41574 2024-04-17 20:20:53.000000 oelint_parser-3.4.1/oelint_parser/cls_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    28787 2024-04-17 20:20:53.000000 oelint_parser-3.4.1/oelint_parser/cls_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-17 20:20:53.000000 oelint_parser-3.4.1/oelint_parser/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:21:12.713953 oelint_parser-3.4.1/oelint_parser/data/
--rw-r--r--   0 runner    (1001) docker     (127)    57343 2024-04-17 20:20:53.000000 oelint_parser-3.4.1/oelint_parser/data/const-default.json
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-17 20:20:53.000000 oelint_parser-3.4.1/oelint_parser/helper_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-04-17 20:20:53.000000 oelint_parser-3.4.1/oelint_parser/inlinerep.py
--rw-r--r--   0 runner    (1001) docker     (127)    17990 2024-04-17 20:20:53.000000 oelint_parser-3.4.1/oelint_parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-17 20:20:53.000000 oelint_parser-3.4.1/oelint_parser/rpl_regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:21:12.713953 oelint_parser-3.4.1/oelint_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-17 20:21:12.000000 oelint_parser-3.4.1/oelint_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-17 20:21:12.000000 oelint_parser-3.4.1/oelint_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:21:12.000000 oelint_parser-3.4.1/oelint_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 20:21:12.000000 oelint_parser-3.4.1/oelint_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 20:21:12.000000 oelint_parser-3.4.1/oelint_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-17 20:20:53.000000 oelint_parser-3.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-17 20:21:12.713953 oelint_parser-3.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-17 20:21:12.000000 oelint_parser-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:33:06.971741 oelint_parser-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-20 06:32:44.000000 oelint_parser-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-20 06:32:44.000000 oelint_parser-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-20 06:33:06.971741 oelint_parser-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-04-20 06:32:44.000000 oelint_parser-3.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:33:06.967741 oelint_parser-3.5.0/oelint_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-20 06:32:44.000000 oelint_parser-3.5.0/oelint_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41574 2024-04-20 06:32:44.000000 oelint_parser-3.5.0/oelint_parser/cls_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28787 2024-04-20 06:32:44.000000 oelint_parser-3.5.0/oelint_parser/cls_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-20 06:32:44.000000 oelint_parser-3.5.0/oelint_parser/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:33:06.971741 oelint_parser-3.5.0/oelint_parser/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    57343 2024-04-20 06:32:44.000000 oelint_parser-3.5.0/oelint_parser/data/const-default.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-20 06:32:44.000000 oelint_parser-3.5.0/oelint_parser/helper_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-04-20 06:32:44.000000 oelint_parser-3.5.0/oelint_parser/inlinerep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17990 2024-04-20 06:32:44.000000 oelint_parser-3.5.0/oelint_parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-20 06:32:44.000000 oelint_parser-3.5.0/oelint_parser/rpl_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:33:06.971741 oelint_parser-3.5.0/oelint_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-20 06:33:06.000000 oelint_parser-3.5.0/oelint_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-20 06:33:06.000000 oelint_parser-3.5.0/oelint_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 06:33:06.000000 oelint_parser-3.5.0/oelint_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-20 06:33:06.000000 oelint_parser-3.5.0/oelint_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-20 06:33:06.000000 oelint_parser-3.5.0/oelint_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-20 06:32:44.000000 oelint_parser-3.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-20 06:33:06.971741 oelint_parser-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-20 06:33:06.000000 oelint_parser-3.5.0/setup.py
```

### Comparing `oelint_parser-3.4.1/LICENSE` & `oelint_parser-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oelint_parser-3.4.1/PKG-INFO` & `oelint_parser-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oelint_parser
-Version: 3.4.1
+Version: 3.5.0
 Summary: Alternative parser for bitbake recipes
 Home-page: https://github.com/priv-kweihmann/oelint-parser
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `oelint_parser-3.4.1/README.md` & `oelint_parser-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `oelint_parser-3.4.1/oelint_parser/cls_item.py` & `oelint_parser-3.5.0/oelint_parser/cls_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,24 +395,24 @@
 
     def IsAppend(self) -> bool:
         """Check if operation is an append
 
         Returns:
             bool -- True is variable is appended
         """
-        return self.VarOp in [" += ", " =+ ", " =. ", " .= "] or "append" in self.SubItems or "prepend" in self.SubItems
+        return self.VarOp.strip() in ["+=", "=+", "=.", ".="] or "append" in self.SubItems or "prepend" in self.SubItems
 
     def AppendOperation(self) -> List[str]:
         """Get variable modifiers
 
         Returns:
             list -- list could contain any combination of 'append', ' += ', 'prepend' and 'remove'
         """
         res = []
-        if self.VarOp in [" += ", " .= ", " =+ ", " =. "]:
+        if self.VarOp.strip() in ["+=", ".=", "=+", "=."]:
             res.append(self.VarOp)
         if "append" in self.SubItems:
             res.append("append")
         if "prepend" in self.SubItems:
             res.append("prepend")
         if "remove" in self.SubItems:
             res.append("remove")
```

### Comparing `oelint_parser-3.4.1/oelint_parser/cls_stash.py` & `oelint_parser-3.5.0/oelint_parser/cls_stash.py`

 * *Files identical despite different names*

### Comparing `oelint_parser-3.4.1/oelint_parser/constants.py` & `oelint_parser-3.5.0/oelint_parser/constants.py`

 * *Files identical despite different names*

### Comparing `oelint_parser-3.4.1/oelint_parser/data/const-default.json` & `oelint_parser-3.5.0/oelint_parser/data/const-default.json`

 * *Files identical despite different names*

### Comparing `oelint_parser-3.4.1/oelint_parser/helper_files.py` & `oelint_parser-3.5.0/oelint_parser/helper_files.py`

 * *Files identical despite different names*

### Comparing `oelint_parser-3.4.1/oelint_parser/inlinerep.py` & `oelint_parser-3.5.0/oelint_parser/inlinerep.py`

 * *Files identical despite different names*

### Comparing `oelint_parser-3.4.1/oelint_parser/parser.py` & `oelint_parser-3.5.0/oelint_parser/parser.py`

 * *Files identical despite different names*

### Comparing `oelint_parser-3.4.1/oelint_parser/rpl_regex.py` & `oelint_parser-3.5.0/oelint_parser/rpl_regex.py`

 * *Files identical despite different names*

### Comparing `oelint_parser-3.4.1/oelint_parser.egg-info/PKG-INFO` & `oelint_parser-3.5.0/oelint_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oelint-parser
-Version: 3.4.1
+Version: 3.5.0
 Summary: Alternative parser for bitbake recipes
 Home-page: https://github.com/priv-kweihmann/oelint-parser
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `oelint_parser-3.4.1/setup.py` & `oelint_parser-3.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 requirements = []
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name='oelint_parser',
-    version='3.4.1',
+    version='3.5.0',
     author='Konrad Weihmann',
     author_email='kweihmann@outlook.com',
     description='Alternative parser for bitbake recipes',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/priv-kweihmann/oelint-parser',
     packages=setuptools.find_packages(),
```

