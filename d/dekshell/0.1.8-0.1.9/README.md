# Comparing `tmp/dekshell-0.1.8.tar.gz` & `tmp/dekshell-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dekshell-0.1.8.tar", last modified: Fri Feb 16 21:57:14 2024, max compression
+gzip compressed data, was "dekshell-0.1.9.tar", last modified: Mon Feb 26 15:11:13 2024, max compression
```

## Comparing `dekshell-0.1.8.tar` & `dekshell-0.1.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      118 2024-02-16 21:57:12.475119 dekshell-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/__init__.py
--rw-r--r--   0        0        0       42 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/click/__entry__.py
--rw-r--r--   0        0        0       21 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/click/__init__.py
--rw-r--r--   0        0        0       34 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/click/base/__init__.py
--rw-r--r--   0        0        0     2790 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/click/shell.py
--rw-r--r--   0        0        0     4597 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/__init__.py
--rw-r--r--   0        0        0      333 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/contexts/__init__.py
--rw-r--r--   0        0        0     1580 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/contexts/methods.py
--rw-r--r--   0        0        0      668 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/contexts/properties.py
--rw-r--r--   0        0        0      258 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/encode.py
--rw-r--r--   0        0        0     1263 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/__init__.py
--rw-r--r--   0        0        0     4548 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/base/__init__.py
--rw-r--r--   0        0        0     5646 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/base/extra.py
--rw-r--r--   0        0        0      237 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/call.py
--rw-r--r--   0        0        0      307 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/cc.py
--rw-r--r--   0        0        0      853 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/ccb.py
--rw-r--r--   0        0        0     2127 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/cfor.py
--rw-r--r--   0        0        0      996 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/cif.py
--rw-r--r--   0        0        0       83 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/comment.py
--rw-r--r--   0        0        0      286 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/cout.py
--rw-r--r--   0        0        0      916 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/cwhile.py
--rw-r--r--   0        0        0      251 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/echo.py
--rw-r--r--   0        0        0      361 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/empty.py
--rw-r--r--   0        0        0      315 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/env.py
--rw-r--r--   0        0        0      929 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/eval.py
--rw-r--r--   0        0        0      427 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/invoke.py
--rw-r--r--   0        0        0      778 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/pip_.py
--rw-r--r--   0        0        0      242 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/py.py
--rw-r--r--   0        0        0      522 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/pyif.py
--rw-r--r--   0        0        0      246 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/pyo.py
--rw-r--r--   0        0        0      310 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/pyoc.py
--rw-r--r--   0        0        0      695 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/redirect.py
--rw-r--r--   0        0        0      921 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/shell.py
--rw-r--r--   0        0        0      429 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/text.py
--rw-r--r--   0        0        0      469 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/markers/with_.py
--rw-r--r--   0        0        0      698 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/plugin/__init__.py
--rw-r--r--   0        0        0     1015 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/core/redirect.py
--rw-r--r--   0        0        0      311 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/res/windows/ext.reg.tpl
--rw-r--r--   0        0        0        0 2024-02-16 21:57:12.475119 dekshell-0.1.8/dekshell/utils/__init__.py
--rw-r--r--   0        0        0     1337 2024-02-16 21:57:12.479119 dekshell-0.1.8/dekshell/utils/pkg.py
--rw-r--r--   0        0        0      536 2024-02-16 21:57:14.663298 dekshell-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-16 21:57:12.479119 dekshell-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0      127 2024-02-16 21:57:12.479119 dekshell-0.1.8/tests/test_main.py
--rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 dekshell-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      230 2024-02-26 15:11:12.027402 dekshell-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/__init__.py
+-rw-r--r--   0        0        0       42 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/click/__entry__.py
+-rw-r--r--   0        0        0       21 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/click/__init__.py
+-rw-r--r--   0        0        0       34 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/click/base/__init__.py
+-rw-r--r--   0        0        0     2790 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/click/shell.py
+-rw-r--r--   0        0        0     4597 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/__init__.py
+-rw-r--r--   0        0        0      333 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/contexts/__init__.py
+-rw-r--r--   0        0        0     1662 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/contexts/methods.py
+-rw-r--r--   0        0        0      668 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/contexts/properties.py
+-rw-r--r--   0        0        0      258 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/encode.py
+-rw-r--r--   0        0        0     1263 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/__init__.py
+-rw-r--r--   0        0        0     4548 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/base/__init__.py
+-rw-r--r--   0        0        0     5646 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/base/extra.py
+-rw-r--r--   0        0        0      237 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/call.py
+-rw-r--r--   0        0        0      307 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/cc.py
+-rw-r--r--   0        0        0      853 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/ccb.py
+-rw-r--r--   0        0        0     2127 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/cfor.py
+-rw-r--r--   0        0        0      996 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/cif.py
+-rw-r--r--   0        0        0       83 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/comment.py
+-rw-r--r--   0        0        0      286 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/cout.py
+-rw-r--r--   0        0        0      916 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/cwhile.py
+-rw-r--r--   0        0        0      251 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/echo.py
+-rw-r--r--   0        0        0      361 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/empty.py
+-rw-r--r--   0        0        0      315 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/env.py
+-rw-r--r--   0        0        0      929 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/eval.py
+-rw-r--r--   0        0        0      427 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/invoke.py
+-rw-r--r--   0        0        0      778 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/pip_.py
+-rw-r--r--   0        0        0      242 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/py.py
+-rw-r--r--   0        0        0      522 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/pyif.py
+-rw-r--r--   0        0        0      246 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/pyo.py
+-rw-r--r--   0        0        0      310 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/pyoc.py
+-rw-r--r--   0        0        0      695 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/redirect.py
+-rw-r--r--   0        0        0      921 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/shell.py
+-rw-r--r--   0        0        0      429 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/text.py
+-rw-r--r--   0        0        0      469 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/markers/with_.py
+-rw-r--r--   0        0        0      698 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/plugin/__init__.py
+-rw-r--r--   0        0        0     1015 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/core/redirect.py
+-rw-r--r--   0        0        0      311 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/res/windows/ext.reg.tpl
+-rw-r--r--   0        0        0        0 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/utils/__init__.py
+-rw-r--r--   0        0        0     1337 2024-02-26 15:11:12.027402 dekshell-0.1.9/dekshell/utils/pkg.py
+-rw-r--r--   0        0        0      536 2024-02-26 15:11:13.851465 dekshell-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-26 15:11:12.031402 dekshell-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0      127 2024-02-26 15:11:12.031402 dekshell-0.1.9/tests/test_main.py
+-rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 dekshell-0.1.9/PKG-INFO
```

### Comparing `dekshell-0.1.8/dekshell/click/shell.py` & `dekshell-0.1.9/dekshell/click/shell.py`

 * *Files identical despite different names*

### Comparing `dekshell-0.1.8/dekshell/core/__init__.py` & `dekshell-0.1.9/dekshell/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dekshell-0.1.8/dekshell/core/contexts/methods.py` & `dekshell-0.1.9/dekshell/core/contexts/methods.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import tempfile
 from beepy import beep
 from dektools.module import get_module_attr
 from dektools.file import sure_dir, write_file, read_text, remove_path
 from dektools.output import pprint
 from dektools.shell import shell_output
+from dektools.net import get_available_port
 from ..encode import encode_run_str
 from ..redirect import search_bin_by_path_tree
 
 
 def _is_true(x):
     if isinstance(x, str):
         x = x.lower()
@@ -48,9 +49,11 @@
     'value': lambda x: x,
     'true': lambda *x: True,
     'false': lambda *x: False,
 
     'istrue': _is_true,
     'isfalse': lambda x: not _is_true(x),
     'isequal': lambda x, y: x == y,
-    'beep': lambda x=True: beep('coin' if x else 'robot_error')
+    'beep': lambda x=True: beep('coin' if x else 'robot_error'),
+
+    'net_port': get_available_port,
 }
```

### Comparing `dekshell-0.1.8/dekshell/core/contexts/properties.py` & `dekshell-0.1.9/dekshell/core/contexts/properties.py`

 * *Files identical despite different names*

### Comparing `dekshell-0.1.8/dekshell/core/markers/__init__.py` & `dekshell-0.1.9/dekshell/core/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `dekshell-0.1.8/dekshell/core/markers/base/__init__.py` & `dekshell-0.1.9/dekshell/core/markers/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dekshell-0.1.8/dekshell/core/markers/base/extra.py` & `dekshell-0.1.9/dekshell/core/markers/base/extra.py`

 * *Files identical despite different names*

### Comparing `dekshell-0.1.8/dekshell/core/markers/ccb.py` & `dekshell-0.1.9/dekshell/core/markers/ccb.py`

 * *Files identical despite different names*

### Comparing `dekshell-0.1.8/dekshell/core/markers/cfor.py` & `dekshell-0.1.9/dekshell/core/markers/cfor.py`

 * *Files identical despite different names*

### Comparing `dekshell-0.1.8/dekshell/core/markers/cif.py` & `dekshell-0.1.9/dekshell/core/markers/cif.py`

 * *Files identical despite different names*

### Comparing `dekshell-0.1.8/dekshell/core/markers/cwhile.py` & `dekshell-0.1.9/dekshell/core/markers/cwhile.py`

 * *Files identical despite different names*

### Comparing `dekshell-0.1.8/dekshell/core/markers/eval.py` & `dekshell-0.1.9/dekshell/core/markers/eval.py`

 * *Files identical despite different names*

### Comparing `dekshell-0.1.8/dekshell/core/markers/pip_.py` & `dekshell-0.1.9/dekshell/core/markers/pip_.py`

 * *Files identical despite different names*

### Comparing `dekshell-0.1.8/dekshell/core/markers/pyif.py` & `dekshell-0.1.9/dekshell/core/markers/pyif.py`

 * *Files identical despite different names*

### Comparing `dekshell-0.1.8/dekshell/core/markers/redirect.py` & `dekshell-0.1.9/dekshell/core/markers/redirect.py`

 * *Files identical despite different names*

### Comparing `dekshell-0.1.8/dekshell/core/markers/shell.py` & `dekshell-0.1.9/dekshell/core/markers/shell.py`

 * *Files identical despite different names*

### Comparing `dekshell-0.1.8/dekshell/core/plugin/__init__.py` & `dekshell-0.1.9/dekshell/core/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dekshell-0.1.8/dekshell/core/redirect.py` & `dekshell-0.1.9/dekshell/core/redirect.py`

 * *Files identical despite different names*

### Comparing `dekshell-0.1.8/dekshell/utils/pkg.py` & `dekshell-0.1.9/dekshell/utils/pkg.py`

 * *Files identical despite different names*

### Comparing `dekshell-0.1.8/pyproject.toml` & `dekshell-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dekshell"
-version = "0.1.8"
+version = "0.1.9"
 description = "Being shell by mixing python and bash and cmd"
 authors = [
     { name = "sanzenwin", email = "sanzenwin@gmail.com" },
 ]
 dependencies = [
     "beepy<=1.0.7",
     "packaging<=23.1",
```

