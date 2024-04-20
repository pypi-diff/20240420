# Comparing `tmp/ctui-0.7.7.tar.gz` & `tmp/ctui-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctui-0.7.7.tar", max compression
+gzip compressed data, was "ctui-0.7.8.tar", max compression
```

## Comparing `ctui-0.7.7.tar` & `ctui-0.7.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35113 2022-05-20 21:48:36.884726 ctui-0.7.7/LICENSE
--rw-r--r--   0        0        0     2045 2023-02-19 14:02:59.554817 ctui-0.7.7/README.md
--rw-r--r--   0        0        0     1443 2024-04-20 03:06:10.990887 ctui-0.7.7/pyproject.toml
--rw-r--r--   0        0        0      676 2023-02-19 16:09:51.611999 ctui-0.7.7/src/ctui/__init__.py
--rw-r--r--   0        0        0     4338 2023-02-22 18:19:42.800943 ctui-0.7.7/src/ctui/application.py
--rw-r--r--   0        0        0     4009 2023-02-19 16:09:57.916994 ctui-0.7.7/src/ctui/base.py
--rw-r--r--   0        0        0    14284 2024-04-20 02:14:28.535777 ctui-0.7.7/src/ctui/commands.py
--rw-r--r--   0        0        0     3463 2023-02-19 16:10:03.786989 ctui-0.7.7/src/ctui/completion.py
--rw-r--r--   0        0        0     8231 2023-02-19 16:10:06.889987 ctui-0.7.7/src/ctui/dialogs.py
--rw-r--r--   0        0        0     4974 2023-02-19 17:26:00.260793 ctui-0.7.7/src/ctui/functions.py
--rw-r--r--   0        0        0      738 2023-02-19 13:30:02.717279 ctui-0.7.7/src/ctui/kaitai/velocio.ksy
--rw-r--r--   0        0        0     7671 2023-02-19 16:10:12.013983 ctui-0.7.7/src/ctui/keybindings.py
--rw-r--r--   0        0        0     4593 2023-02-19 16:10:16.079980 ctui-0.7.7/src/ctui/layout.py
--rw-r--r--   0        0        0     4780 2023-02-19 16:10:19.910977 ctui-0.7.7/src/ctui/style.py
--rw-r--r--   0        0        0     2998 2024-04-20 02:27:03.745400 ctui-0.7.7/src/ctui/types.py
--rw-r--r--   0        0        0     3525 1970-01-01 00:00:00.000000 ctui-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0    35113 2022-05-20 21:48:36.884726 ctui-0.7.8/LICENSE
+-rw-r--r--   0        0        0     2052 2024-04-20 03:32:12.090312 ctui-0.7.8/README.md
+-rw-r--r--   0        0        0     1453 2024-04-20 06:47:34.669875 ctui-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0      676 2023-02-19 16:09:51.611999 ctui-0.7.8/src/ctui/__init__.py
+-rw-r--r--   0        0        0     4338 2023-02-22 18:19:42.800943 ctui-0.7.8/src/ctui/application.py
+-rw-r--r--   0        0        0     4009 2023-02-19 16:09:57.916994 ctui-0.7.8/src/ctui/base.py
+-rw-r--r--   0        0        0    14284 2024-04-20 02:14:28.535777 ctui-0.7.8/src/ctui/commands.py
+-rw-r--r--   0        0        0     3463 2023-02-19 16:10:03.786989 ctui-0.7.8/src/ctui/completion.py
+-rw-r--r--   0        0        0     8231 2023-02-19 16:10:06.889987 ctui-0.7.8/src/ctui/dialogs.py
+-rw-r--r--   0        0        0     4974 2023-02-19 17:26:00.260793 ctui-0.7.8/src/ctui/functions.py
+-rw-r--r--   0        0        0      738 2023-02-19 13:30:02.717279 ctui-0.7.8/src/ctui/kaitai/velocio.ksy
+-rw-r--r--   0        0        0     7671 2023-02-19 16:10:12.013983 ctui-0.7.8/src/ctui/keybindings.py
+-rw-r--r--   0        0        0     4593 2023-02-19 16:10:16.079980 ctui-0.7.8/src/ctui/layout.py
+-rw-r--r--   0        0        0     4780 2023-02-19 16:10:19.910977 ctui-0.7.8/src/ctui/style.py
+-rw-r--r--   0        0        0     2998 2024-04-20 02:27:03.745400 ctui-0.7.8/src/ctui/types.py
+-rw-r--r--   0        0        0     3482 1970-01-01 00:00:00.000000 ctui-0.7.8/PKG-INFO
```

### Comparing `ctui-0.7.7/LICENSE` & `ctui-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ctui-0.7.7/README.md` & `ctui-0.7.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Control Things Serial
+# ControlThings User Interface
 
 The `ctui` is a library for creating terminal-based user interfaces, and is used in all the ControlThings tools at controlthings.io.  It is similar to using Click or Python's standard Cmd library, but with a curses-like interface written in pure Python.
 
 # Installation
 
 Ctui is primarily developed on Linux, but should work in both Mac and Windows as well.
```

### Comparing `ctui-0.7.7/pyproject.toml` & `ctui-0.7.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ctui"
-version = "0.7.7"
+version = "0.7.8"
 description = "The ctui library is similar to Python's built in cmd library, but with a curses-like user interface"
 authors = ["Justin Searle <justin@controlthings.io>"]
 license = "LGPL"
 readme = "README.md"
 homepage = "https://www.controlthings.io"
 repository = "https://github.com/ControlThings-io/ctserial"
 keywords = ["serial", "fieldbus", "ICS", "control", "ControlThings"]
@@ -18,15 +18,15 @@
     'Operating System :: Unix',
     'Operating System :: POSIX',
     'Operating System :: Microsoft :: Windows',
     'Topic :: Utilities',
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">= 3.8, < 3.12"
 prompt-toolkit = "^3.0.36"
 Pygments = "^2.14.0"
 tabulate = "^0.8.0"
 tinydb = "^4.7.1"
 six = "^1.16.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `ctui-0.7.7/src/ctui/__init__.py` & `ctui-0.7.8/src/ctui/__init__.py`

 * *Files identical despite different names*

### Comparing `ctui-0.7.7/src/ctui/application.py` & `ctui-0.7.8/src/ctui/application.py`

 * *Files identical despite different names*

### Comparing `ctui-0.7.7/src/ctui/base.py` & `ctui-0.7.8/src/ctui/base.py`

 * *Files identical despite different names*

### Comparing `ctui-0.7.7/src/ctui/commands.py` & `ctui-0.7.8/src/ctui/commands.py`

 * *Files identical despite different names*

### Comparing `ctui-0.7.7/src/ctui/completion.py` & `ctui-0.7.8/src/ctui/completion.py`

 * *Files identical despite different names*

### Comparing `ctui-0.7.7/src/ctui/dialogs.py` & `ctui-0.7.8/src/ctui/dialogs.py`

 * *Files identical despite different names*

### Comparing `ctui-0.7.7/src/ctui/functions.py` & `ctui-0.7.8/src/ctui/functions.py`

 * *Files identical despite different names*

### Comparing `ctui-0.7.7/src/ctui/kaitai/velocio.ksy` & `ctui-0.7.8/src/ctui/kaitai/velocio.ksy`

 * *Files identical despite different names*

### Comparing `ctui-0.7.7/src/ctui/keybindings.py` & `ctui-0.7.8/src/ctui/keybindings.py`

 * *Files identical despite different names*

### Comparing `ctui-0.7.7/src/ctui/layout.py` & `ctui-0.7.8/src/ctui/layout.py`

 * *Files identical despite different names*

### Comparing `ctui-0.7.7/src/ctui/style.py` & `ctui-0.7.8/src/ctui/style.py`

 * *Files identical despite different names*

### Comparing `ctui-0.7.7/src/ctui/types.py` & `ctui-0.7.8/src/ctui/types.py`

 * *Files identical despite different names*

### Comparing `ctui-0.7.7/PKG-INFO` & `ctui-0.7.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ctui
-Version: 0.7.7
+Version: 0.7.8
 Summary: The ctui library is similar to Python's built in cmd library, but with a curses-like user interface
 Home-page: https://www.controlthings.io
 License: LGPL
 Keywords: serial,fieldbus,ICS,control,ControlThings
 Author: Justin Searle
 Author-email: justin@controlthings.io
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
@@ -19,25 +19,24 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Requires-Dist: Pygments (>=2.14.0,<3.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.36,<4.0.0)
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Requires-Dist: tabulate (>=0.8.0,<0.9.0)
 Requires-Dist: tinydb (>=4.7.1,<5.0.0)
 Project-URL: Repository, https://github.com/ControlThings-io/ctserial
 Description-Content-Type: text/markdown
 
-# Control Things Serial
+# ControlThings User Interface
 
 The `ctui` is a library for creating terminal-based user interfaces, and is used in all the ControlThings tools at controlthings.io.  It is similar to using Click or Python's standard Cmd library, but with a curses-like interface written in pure Python.
 
 # Installation
 
 Ctui is primarily developed on Linux, but should work in both Mac and Windows as well.
```

