# Comparing `tmp/jeffutils-0.4.8.tar.gz` & `tmp/jeffutils-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.4.8.tar", last modified: Wed Apr 10 18:59:47 2024, max compression
+gzip compressed data, was "jeffutils-0.4.9.tar", last modified: Sat Apr 20 03:45:47 2024, max compression
```

## Comparing `jeffutils-0.4.8.tar` & `jeffutils-0.4.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-10 18:59:47.768322 jeffutils-0.4.8/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.4.8/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-04-10 18:59:47.768322 jeffutils-0.4.8/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.4.8/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.4.8/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-04-10 18:59:47.768322 jeffutils-0.4.8/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-04-10 18:59:35.000000 jeffutils-0.4.8/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-10 18:59:47.768322 jeffutils-0.4.8/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-10 18:59:47.768322 jeffutils-0.4.8/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.4.8/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    14879 2024-04-10 18:59:25.000000 jeffutils-0.4.8/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-10 18:59:47.768322 jeffutils-0.4.8/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-04-10 18:59:47.000000 jeffutils-0.4.8/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-04-10 18:59:47.000000 jeffutils-0.4.8/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-04-10 18:59:47.000000 jeffutils-0.4.8/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-04-10 18:59:47.000000 jeffutils-0.4.8/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-20 03:45:47.973482 jeffutils-0.4.9/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.4.9/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-04-20 03:45:47.973482 jeffutils-0.4.9/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.4.9/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.4.9/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-04-20 03:45:47.973482 jeffutils-0.4.9/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-04-20 03:45:39.000000 jeffutils-0.4.9/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-20 03:45:47.973482 jeffutils-0.4.9/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-20 03:45:47.973482 jeffutils-0.4.9/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.4.9/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    16086 2024-04-20 03:45:14.000000 jeffutils-0.4.9/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-04-20 03:45:47.973482 jeffutils-0.4.9/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-04-20 03:45:47.000000 jeffutils-0.4.9/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-04-20 03:45:47.000000 jeffutils-0.4.9/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-04-20 03:45:47.000000 jeffutils-0.4.9/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-04-20 03:45:47.000000 jeffutils-0.4.9/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.4.8/LICENSE.txt` & `jeffutils-0.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.4.8/setup.py` & `jeffutils-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.4.8',
+    version='0.4.9',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description='A series of useful functions and decorators I use in most of my projects. Feel free to use them as well :)',
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `jeffutils-0.4.8/src/jeffutils/utils.py` & `jeffutils-0.4.9/src/jeffutils/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -139,14 +139,49 @@
     global print_time_p
     if string is not None:
         print(f"{string}...", end="", flush=True)
         print_time_p = perf_counter()
     else:
         print("DONE", round(perf_counter() - print_time_p, 3), "sec", flush=True)
         
+        
+def format_text_to_lines(input_text, max_line_length=60):
+    """
+    Format the input text into lines with a maximum line length of 'max_line_length'.
+
+    Args:
+        input_text (str): The input text to be formatted.
+        max_line_length (int): Maximum desired length of each line.
+
+    Returns:
+        str: The formatted text with newlines inserted appropriately.
+    """
+    words = input_text.split()
+    lines = []
+    current_line = ""
+
+    for word in words:
+        if len(current_line) + len(word) + 1 > max_line_length:  # Check if adding this word exceeds the max line length
+            lines.append(current_line)  # Add the current line to the list of lines
+            current_line = word  # Start a new line with the current word
+        else:
+            if current_line:  # Add a space if the current line is not empty
+                current_line += " "
+            current_line += word  # Add the word to the current line
+
+    # Add the last line to the list of lines
+    if current_line:
+        lines.append(current_line)
+
+    # Join the lines with newline characters to form the formatted text
+    formatted_text = "\n".join(lines)
+
+    return formatted_text
+
+        
 
 ###################
 # PANDA FUNCTIONS #
 ###################
 
 def set_np_pd_display_params(np, pd):
     """sets numpy and pandas display properties"""
```

