# Comparing `tmp/textlinebreaker-0.1.0a0.tar.gz` & `tmp/textlinebreaker-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textlinebreaker-0.1.0a0.tar", last modified: Mon Nov 20 00:51:58 2023, max compression
+gzip compressed data, was "textlinebreaker-0.2.0.tar", last modified: Sat Apr 20 19:09:01 2024, max compression
```

## Comparing `textlinebreaker-0.1.0a0.tar` & `textlinebreaker-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-11-20 00:51:58.943639 textlinebreaker-0.1.0a0/
--rw-r--r--   0 simon     (1000) simon     (1000)     1073 2023-11-05 18:23:12.000000 textlinebreaker-0.1.0a0/LICENSE.md
--rw-r--r--   0 simon     (1000) simon     (1000)     4894 2023-11-20 00:51:58.943639 textlinebreaker-0.1.0a0/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)     3824 2023-11-20 00:31:08.000000 textlinebreaker-0.1.0a0/README.md
--rw-r--r--   0 simon     (1000) simon     (1000)     1193 2023-11-20 00:43:06.000000 textlinebreaker-0.1.0a0/pyproject.toml
--rw-r--r--   0 simon     (1000) simon     (1000)       38 2023-11-20 00:51:58.943639 textlinebreaker-0.1.0a0/setup.cfg
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-11-20 00:51:58.943639 textlinebreaker-0.1.0a0/textlinebreaker/
--rw-r--r--   0 simon     (1000) simon     (1000)       86 2023-11-20 00:35:18.000000 textlinebreaker-0.1.0a0/textlinebreaker/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     2811 2023-11-20 00:07:51.000000 textlinebreaker-0.1.0a0/textlinebreaker/textlinebreaker.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-11-20 00:51:58.943639 textlinebreaker-0.1.0a0/textlinebreaker.egg-info/
--rw-r--r--   0 simon     (1000) simon     (1000)     4894 2023-11-20 00:51:58.000000 textlinebreaker-0.1.0a0/textlinebreaker.egg-info/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)      254 2023-11-20 00:51:58.000000 textlinebreaker-0.1.0a0/textlinebreaker.egg-info/SOURCES.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        1 2023-11-20 00:51:58.000000 textlinebreaker-0.1.0a0/textlinebreaker.egg-info/dependency_links.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       16 2023-11-20 00:51:58.000000 textlinebreaker-0.1.0a0/textlinebreaker.egg-info/top_level.txt
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-20 19:09:01.132332 textlinebreaker-0.2.0/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1073 2024-01-04 19:23:58.000000 textlinebreaker-0.2.0/LICENSE.md
+-rw-r--r--   0 simon     (1000) simon     (1000)     4994 2024-04-20 19:09:01.132332 textlinebreaker-0.2.0/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)     3918 2024-04-20 18:27:04.000000 textlinebreaker-0.2.0/README.md
+-rw-r--r--   0 simon     (1000) simon     (1000)     1201 2024-04-20 17:58:23.000000 textlinebreaker-0.2.0/pyproject.toml
+-rw-r--r--   0 simon     (1000) simon     (1000)       38 2024-04-20 19:09:01.132332 textlinebreaker-0.2.0/setup.cfg
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-20 19:09:01.132332 textlinebreaker-0.2.0/textlinebreaker/
+-rw-r--r--   0 simon     (1000) simon     (1000)       80 2024-04-20 17:34:23.000000 textlinebreaker-0.2.0/textlinebreaker/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     5910 2024-04-20 19:07:06.000000 textlinebreaker-0.2.0/textlinebreaker/textlinebreaker.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-20 19:09:01.132332 textlinebreaker-0.2.0/textlinebreaker.egg-info/
+-rw-r--r--   0 simon     (1000) simon     (1000)     4994 2024-04-20 19:09:01.000000 textlinebreaker-0.2.0/textlinebreaker.egg-info/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)      254 2024-04-20 19:09:01.000000 textlinebreaker-0.2.0/textlinebreaker.egg-info/SOURCES.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        1 2024-04-20 19:09:01.000000 textlinebreaker-0.2.0/textlinebreaker.egg-info/dependency_links.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       16 2024-04-20 19:09:01.000000 textlinebreaker-0.2.0/textlinebreaker.egg-info/top_level.txt
```

### Comparing `textlinebreaker-0.1.0a0/LICENSE.md` & `textlinebreaker-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `textlinebreaker-0.1.0a0/PKG-INFO` & `textlinebreaker-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: textlinebreaker
-Version: 0.1.0a0
+Version: 0.2.0
 Summary: A module to format strings. Length and alignment of lines can be specified. In the new version is resolved the issue that caused the string to be splitted in single characters rather than in words. Also a check has been added to establish if the input is a list or a string in order to perform the correct splitting method.
 Author-email: scalvaruso <calvaruso.simone@gmail.com>
 License: MIT License
-Project-URL: Homepage, https://github.com/scalvaruso/textlinebreaker
+Project-URL: Homepage, https://pypi.org/project/textlinebreaker
 Project-URL: Repository, https://github.com/scalvaruso/textlinebreaker
-Keywords: alignment,break,center,centre,format,left,line,right,split,text
+Keywords: alignment,break,center,centre,format,left,line,right,split,string,text,words
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -36,18 +36,18 @@
 
 ## Features
 
 - Split text lines to fit within a specified maximum width.
 - Choose alignment options for the text (left, center, right).
 - Adjust the maximum width (default value is the terminal width).
 
-## Latest Version 0.1.0-alpha
+## Latest Version 0.2.0
 
-- Fixed a bug where the string was split in single characters rather than in words.
-- Added a check for the input to establish if it is a list or a string in order to perform the correct splitting method.
+- Added new parameters (`"min"`, `"2words"`, `"max"`) to set different lines width.
+- Improved algorithm to better split the input in the desired lenght lines.
 
 ## Table of Contents
 
 - [Getting Started](#getting-started)
   - [Prerequisites](#prerequisites)
   - [Installation](#installation)
 - [Usage](#usage)
@@ -65,14 +65,18 @@
 ### Installation
 
 - Install the package with pip
 
 ```bash
   pip install textlinebreaker
 ```
+- or upgrade it with
+```bash
+  pip install --upgrade textlinebreaker
+```
 
 - Import the package in your program
 
 ```python
   from textlinebreaker import split_line
 ```
 
@@ -81,17 +85,22 @@
 This function takes a long string of text as input and breaks it into lines according to the specified maximum width.
 The default length is the width of the terminal.
 
 ### Parameters
 
 The `split_line` function accepts the following parameters:
 
-- `line`: is the main argument, it's the text that needs to be broken down.
-- `max_width`: Allows you to set the maximum length of text on a line. Default value is the terminal width. Allowed values are integers.
-- `alignment`: Allows you to change the alignment of the text inside the frame. Default value is "left". Allowed values are "left", "centre" or "center", and "right".
+- **`line`**: is the main argument, it's the text that needs to be broken down.
+  - allowed values: strings, list of strings
+- **`max_width`**: allows to set the max length of text on a line. 
+  - allowed values: integers, "min", "2words", "max"
+  - default value = "max" (terminal width)
+- **`alignment`**: allows to change the alignment of the text inside the frame.
+  - allowed values: "left", "centre", "center", "right"
+  - default value = "left"
 
 ### Examples
 
 Here's an example of how to use the `split_line` function:
 
 ```python
 from textlinebreaker import split_line
```

### Comparing `textlinebreaker-0.1.0a0/README.md` & `textlinebreaker-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 
 ## Features
 
 - Split text lines to fit within a specified maximum width.
 - Choose alignment options for the text (left, center, right).
 - Adjust the maximum width (default value is the terminal width).
 
-## Latest Version 0.1.0-alpha
+## Latest Version 0.2.0
 
-- Fixed a bug where the string was split in single characters rather than in words.
-- Added a check for the input to establish if it is a list or a string in order to perform the correct splitting method.
+- Added new parameters (`"min"`, `"2words"`, `"max"`) to set different lines width.
+- Improved algorithm to better split the input in the desired lenght lines.
 
 ## Table of Contents
 
 - [Getting Started](#getting-started)
   - [Prerequisites](#prerequisites)
   - [Installation](#installation)
 - [Usage](#usage)
@@ -46,14 +46,18 @@
 ### Installation
 
 - Install the package with pip
 
 ```bash
   pip install textlinebreaker
 ```
+- or upgrade it with
+```bash
+  pip install --upgrade textlinebreaker
+```
 
 - Import the package in your program
 
 ```python
   from textlinebreaker import split_line
 ```
 
@@ -62,17 +66,22 @@
 This function takes a long string of text as input and breaks it into lines according to the specified maximum width.
 The default length is the width of the terminal.
 
 ### Parameters
 
 The `split_line` function accepts the following parameters:
 
-- `line`: is the main argument, it's the text that needs to be broken down.
-- `max_width`: Allows you to set the maximum length of text on a line. Default value is the terminal width. Allowed values are integers.
-- `alignment`: Allows you to change the alignment of the text inside the frame. Default value is "left". Allowed values are "left", "centre" or "center", and "right".
+- **`line`**: is the main argument, it's the text that needs to be broken down.
+  - allowed values: strings, list of strings
+- **`max_width`**: allows to set the max length of text on a line. 
+  - allowed values: integers, "min", "2words", "max"
+  - default value = "max" (terminal width)
+- **`alignment`**: allows to change the alignment of the text inside the frame.
+  - allowed values: "left", "centre", "center", "right"
+  - default value = "left"
 
 ### Examples
 
 Here's an example of how to use the `split_line` function:
 
 ```python
 from textlinebreaker import split_line
```

### Comparing `textlinebreaker-0.1.0a0/pyproject.toml` & `textlinebreaker-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [project]
 name = "textlinebreaker"
-version = "0.1.0-alpha"
+version = "0.2.0"
 dependencies = [ ]
 requires-python = ">=3.9"
 authors = [
     { name="scalvaruso", email="calvaruso.simone@gmail.com" },
 ]
 description = "A module to format strings. Length and alignment of lines can be specified. In the new version is resolved the issue that caused the string to be splitted in single characters rather than in words. Also a check has been added to establish if the input is a list or a string in order to perform the correct splitting method."
 readme = "README.md"
 license = {text = "MIT License"}
-keywords = ["alignment", "break", "center", "centre", "format", "left", "line", "right", "split", "text"]
+keywords = ["alignment", "break", "center", "centre", "format", "left", "line", "right", "split", "string", "text", "words"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-Homepage = "https://github.com/scalvaruso/textlinebreaker"
+Homepage = "https://pypi.org/project/textlinebreaker"
 Repository = "https://github.com/scalvaruso/textlinebreaker"
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `textlinebreaker-0.1.0a0/textlinebreaker.egg-info/PKG-INFO` & `textlinebreaker-0.2.0/textlinebreaker.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: textlinebreaker
-Version: 0.1.0a0
+Version: 0.2.0
 Summary: A module to format strings. Length and alignment of lines can be specified. In the new version is resolved the issue that caused the string to be splitted in single characters rather than in words. Also a check has been added to establish if the input is a list or a string in order to perform the correct splitting method.
 Author-email: scalvaruso <calvaruso.simone@gmail.com>
 License: MIT License
-Project-URL: Homepage, https://github.com/scalvaruso/textlinebreaker
+Project-URL: Homepage, https://pypi.org/project/textlinebreaker
 Project-URL: Repository, https://github.com/scalvaruso/textlinebreaker
-Keywords: alignment,break,center,centre,format,left,line,right,split,text
+Keywords: alignment,break,center,centre,format,left,line,right,split,string,text,words
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -36,18 +36,18 @@
 
 ## Features
 
 - Split text lines to fit within a specified maximum width.
 - Choose alignment options for the text (left, center, right).
 - Adjust the maximum width (default value is the terminal width).
 
-## Latest Version 0.1.0-alpha
+## Latest Version 0.2.0
 
-- Fixed a bug where the string was split in single characters rather than in words.
-- Added a check for the input to establish if it is a list or a string in order to perform the correct splitting method.
+- Added new parameters (`"min"`, `"2words"`, `"max"`) to set different lines width.
+- Improved algorithm to better split the input in the desired lenght lines.
 
 ## Table of Contents
 
 - [Getting Started](#getting-started)
   - [Prerequisites](#prerequisites)
   - [Installation](#installation)
 - [Usage](#usage)
@@ -65,14 +65,18 @@
 ### Installation
 
 - Install the package with pip
 
 ```bash
   pip install textlinebreaker
 ```
+- or upgrade it with
+```bash
+  pip install --upgrade textlinebreaker
+```
 
 - Import the package in your program
 
 ```python
   from textlinebreaker import split_line
 ```
 
@@ -81,17 +85,22 @@
 This function takes a long string of text as input and breaks it into lines according to the specified maximum width.
 The default length is the width of the terminal.
 
 ### Parameters
 
 The `split_line` function accepts the following parameters:
 
-- `line`: is the main argument, it's the text that needs to be broken down.
-- `max_width`: Allows you to set the maximum length of text on a line. Default value is the terminal width. Allowed values are integers.
-- `alignment`: Allows you to change the alignment of the text inside the frame. Default value is "left". Allowed values are "left", "centre" or "center", and "right".
+- **`line`**: is the main argument, it's the text that needs to be broken down.
+  - allowed values: strings, list of strings
+- **`max_width`**: allows to set the max length of text on a line. 
+  - allowed values: integers, "min", "2words", "max"
+  - default value = "max" (terminal width)
+- **`alignment`**: allows to change the alignment of the text inside the frame.
+  - allowed values: "left", "centre", "center", "right"
+  - default value = "left"
 
 ### Examples
 
 Here's an example of how to use the `split_line` function:
 
 ```python
 from textlinebreaker import split_line
```

