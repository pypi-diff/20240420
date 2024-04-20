# Comparing `tmp/ctui-0.7.6.tar.gz` & `tmp/ctui-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctui-0.7.6.tar", max compression
+gzip compressed data, was "ctui-0.7.7.tar", max compression
```

## Comparing `ctui-0.7.6.tar` & `ctui-0.7.7.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0    35113 2022-05-20 21:48:36.884726 ctui-0.7.6/LICENSE
--rw-r--r--   0        0        0     2045 2023-02-19 14:02:59.554817 ctui-0.7.6/README.md
--rw-r--r--   0        0        0     1448 2023-02-22 15:56:25.626185 ctui-0.7.6/pyproject.toml
--rw-r--r--   0        0        0      676 2023-02-19 16:09:51.611999 ctui-0.7.6/src/ctui/__init__.py
--rw-r--r--   0        0        0     4338 2023-02-19 18:37:43.112403 ctui-0.7.6/src/ctui/application.py
--rw-r--r--   0        0        0     4009 2023-02-19 16:09:57.916994 ctui-0.7.6/src/ctui/base.py
--rw-r--r--   0        0        0    14284 2023-02-19 17:30:21.294587 ctui-0.7.6/src/ctui/commands.py
--rw-r--r--   0        0        0     3463 2023-02-19 16:10:03.786989 ctui-0.7.6/src/ctui/completion.py
--rw-r--r--   0        0        0     8231 2023-02-19 16:10:06.889987 ctui-0.7.6/src/ctui/dialogs.py
--rw-r--r--   0        0        0     4974 2023-02-19 17:26:00.260793 ctui-0.7.6/src/ctui/functions.py
--rw-r--r--   0        0        0      738 2023-02-19 13:30:02.717279 ctui-0.7.6/src/ctui/kaitai/velocio.ksy
--rw-r--r--   0        0        0     7671 2023-02-19 16:10:12.013983 ctui-0.7.6/src/ctui/keybindings.py
--rw-r--r--   0        0        0     4593 2023-02-19 16:10:16.079980 ctui-0.7.6/src/ctui/layout.py
--rw-r--r--   0        0        0     4780 2023-02-19 16:10:19.910977 ctui-0.7.6/src/ctui/style.py
--rw-r--r--   0        0        0     3065 2023-02-19 16:10:22.365975 ctui-0.7.6/src/ctui/types.py
--rw-r--r--   0        0        0     2994 1970-01-01 00:00:00.000000 ctui-0.7.6/setup.py
--rw-r--r--   0        0        0     3574 1970-01-01 00:00:00.000000 ctui-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0    35113 2022-05-20 21:48:36.884726 ctui-0.7.7/LICENSE
+-rw-r--r--   0        0        0     2045 2023-02-19 14:02:59.554817 ctui-0.7.7/README.md
+-rw-r--r--   0        0        0     1443 2024-04-20 03:06:10.990887 ctui-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0      676 2023-02-19 16:09:51.611999 ctui-0.7.7/src/ctui/__init__.py
+-rw-r--r--   0        0        0     4338 2023-02-22 18:19:42.800943 ctui-0.7.7/src/ctui/application.py
+-rw-r--r--   0        0        0     4009 2023-02-19 16:09:57.916994 ctui-0.7.7/src/ctui/base.py
+-rw-r--r--   0        0        0    14284 2024-04-20 02:14:28.535777 ctui-0.7.7/src/ctui/commands.py
+-rw-r--r--   0        0        0     3463 2023-02-19 16:10:03.786989 ctui-0.7.7/src/ctui/completion.py
+-rw-r--r--   0        0        0     8231 2023-02-19 16:10:06.889987 ctui-0.7.7/src/ctui/dialogs.py
+-rw-r--r--   0        0        0     4974 2023-02-19 17:26:00.260793 ctui-0.7.7/src/ctui/functions.py
+-rw-r--r--   0        0        0      738 2023-02-19 13:30:02.717279 ctui-0.7.7/src/ctui/kaitai/velocio.ksy
+-rw-r--r--   0        0        0     7671 2023-02-19 16:10:12.013983 ctui-0.7.7/src/ctui/keybindings.py
+-rw-r--r--   0        0        0     4593 2023-02-19 16:10:16.079980 ctui-0.7.7/src/ctui/layout.py
+-rw-r--r--   0        0        0     4780 2023-02-19 16:10:19.910977 ctui-0.7.7/src/ctui/style.py
+-rw-r--r--   0        0        0     2998 2024-04-20 02:27:03.745400 ctui-0.7.7/src/ctui/types.py
+-rw-r--r--   0        0        0     3525 1970-01-01 00:00:00.000000 ctui-0.7.7/PKG-INFO
```

### Comparing `ctui-0.7.6/LICENSE` & `ctui-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ctui-0.7.6/README.md` & `ctui-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `ctui-0.7.6/pyproject.toml` & `ctui-0.7.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "ctui"
-version = "0.7.6"
+version = "0.7.7"
 description = "The ctui library is similar to Python's built in cmd library, but with a curses-like user interface"
 authors = ["Justin Searle <justin@controlthings.io>"]
 license = "LGPL"
 readme = "README.md"
 homepage = "https://www.controlthings.io"
 repository = "https://github.com/ControlThings-io/ctserial"
 keywords = ["serial", "fieldbus", "ICS", "control", "ControlThings"]
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Intended Audience :: Information Technology',
     'Intended Audience :: Manufacturing',
-    'Intended Audience :: Other Audience',    
+    'Intended Audience :: Other Audience',
     'Intended Audience :: Science/Research',
     'Operating System :: Unix',
     'Operating System :: POSIX',
     'Operating System :: Microsoft :: Windows',
     'Topic :: Utilities',
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.8"
 prompt-toolkit = "^3.0.36"
 Pygments = "^2.14.0"
 tabulate = "^0.8.0"
 tinydb = "^4.7.1"
 six = "^1.16.0"
 
 [tool.poetry.group.dev.dependencies]
@@ -47,8 +47,7 @@
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
 line_length = 88
-
```

### Comparing `ctui-0.7.6/src/ctui/__init__.py` & `ctui-0.7.7/src/ctui/__init__.py`

 * *Files identical despite different names*

### Comparing `ctui-0.7.6/src/ctui/application.py` & `ctui-0.7.7/src/ctui/application.py`

 * *Files identical despite different names*

### Comparing `ctui-0.7.6/src/ctui/base.py` & `ctui-0.7.7/src/ctui/base.py`

 * *Files identical despite different names*

### Comparing `ctui-0.7.6/src/ctui/commands.py` & `ctui-0.7.7/src/ctui/commands.py`

 * *Files identical despite different names*

### Comparing `ctui-0.7.6/src/ctui/completion.py` & `ctui-0.7.7/src/ctui/completion.py`

 * *Files identical despite different names*

### Comparing `ctui-0.7.6/src/ctui/dialogs.py` & `ctui-0.7.7/src/ctui/dialogs.py`

 * *Files identical despite different names*

### Comparing `ctui-0.7.6/src/ctui/functions.py` & `ctui-0.7.7/src/ctui/functions.py`

 * *Files identical despite different names*

### Comparing `ctui-0.7.6/src/ctui/kaitai/velocio.ksy` & `ctui-0.7.7/src/ctui/kaitai/velocio.ksy`

 * *Files identical despite different names*

### Comparing `ctui-0.7.6/src/ctui/keybindings.py` & `ctui-0.7.7/src/ctui/keybindings.py`

 * *Files identical despite different names*

### Comparing `ctui-0.7.6/src/ctui/layout.py` & `ctui-0.7.7/src/ctui/layout.py`

 * *Files identical despite different names*

### Comparing `ctui-0.7.6/src/ctui/style.py` & `ctui-0.7.7/src/ctui/style.py`

 * *Files identical despite different names*

### Comparing `ctui-0.7.6/src/ctui/types.py` & `ctui-0.7.7/src/ctui/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,16 +78,13 @@
             list_float.append(float(decimal))
         return list_float
 
     elif kwarg.type == GreedyBin or kwarg.type == List[Bin]:
         data = value.lower().replace("0b", "")
         if re.match("^[01\\\\b ]+$", data):
             raw_bin = re.sub("[\\\\b ]", "", data)
-            list_bool = []
-            for bit in raw_bin:
-                list_bool.append(bool(int(bit)))
-            return list_bool
+            return [False if bit == "0" else True for bit in raw_bin]
         else:
             raise AssertionError(f"{kwarg.name} must be sequence of 1s and 0s")
 
     else:
         raise AssertionError("type not implimented yet")
```

### Comparing `ctui-0.7.6/PKG-INFO` & `ctui-0.7.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: ctui
-Version: 0.7.6
+Version: 0.7.7
 Summary: The ctui library is similar to Python's built in cmd library, but with a curses-like user interface
 Home-page: https://www.controlthings.io
 License: LGPL
 Keywords: serial,fieldbus,ICS,control,ControlThings
 Author: Justin Searle
 Author-email: justin@controlthings.io
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Requires-Dist: Pygments (>=2.14.0,<3.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.36,<4.0.0)
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Requires-Dist: tabulate (>=0.8.0,<0.9.0)
 Requires-Dist: tinydb (>=4.7.1,<5.0.0)
 Project-URL: Repository, https://github.com/ControlThings-io/ctserial
```

