# Comparing `tmp/uo_puddles-4.5.tar.gz` & `tmp/uo_puddles-4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uo_puddles-4.5.tar", last modified: Fri Feb 16 18:20:38 2024, max compression
+gzip compressed data, was "uo_puddles-4.6.tar", last modified: Mon Feb 19 16:52:23 2024, max compression
```

## Comparing `uo_puddles-4.5.tar` & `uo_puddles-4.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:20:38.787091 uo_puddles-4.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-16 18:20:23.000000 uo_puddles-4.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-16 18:20:38.787091 uo_puddles-4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-16 18:20:23.000000 uo_puddles-4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-16 18:20:23.000000 uo_puddles-4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 18:20:38.787091 uo_puddles-4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-16 18:20:23.000000 uo_puddles-4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:20:38.783091 uo_puddles-4.5/uo_puddles/
--rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-02-16 18:20:23.000000 uo_puddles-4.5/uo_puddles/CustomTukeyTransformer_unittest.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-16 18:20:23.000000 uo_puddles-4.5/uo_puddles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19518 2024-02-16 18:20:23.000000 uo_puddles-4.5/uo_puddles/cis423.py
--rw-r--r--   0 runner    (1001) docker     (127)    36496 2024-02-16 18:20:23.000000 uo_puddles-4.5/uo_puddles/good_ai.py
--rw-r--r--   0 runner    (1001) docker     (127)    24737 2024-02-16 18:20:23.000000 uo_puddles-4.5/uo_puddles/good_ai_22.py
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-02-16 18:20:23.000000 uo_puddles-4.5/uo_puddles/gremcat_df.py
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-02-16 18:20:23.000000 uo_puddles-4.5/uo_puddles/gremcat_oo.py
--rw-r--r--   0 runner    (1001) docker     (127)    24584 2024-02-16 18:20:23.000000 uo_puddles-4.5/uo_puddles/mlops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:20:38.787091 uo_puddles-4.5/uo_puddles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-16 18:20:38.000000 uo_puddles-4.5/uo_puddles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-02-16 18:20:38.000000 uo_puddles-4.5/uo_puddles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 18:20:38.000000 uo_puddles-4.5/uo_puddles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-16 18:20:38.000000 uo_puddles-4.5/uo_puddles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:52:23.240677 uo_puddles-4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-19 16:52:13.000000 uo_puddles-4.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-19 16:52:23.240677 uo_puddles-4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-19 16:52:13.000000 uo_puddles-4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-19 16:52:13.000000 uo_puddles-4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 16:52:23.240677 uo_puddles-4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-19 16:52:13.000000 uo_puddles-4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:52:23.236677 uo_puddles-4.6/uo_puddles/
+-rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-02-19 16:52:13.000000 uo_puddles-4.6/uo_puddles/CustomTukeyTransformer_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-19 16:52:13.000000 uo_puddles-4.6/uo_puddles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19518 2024-02-19 16:52:13.000000 uo_puddles-4.6/uo_puddles/cis423.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37411 2024-02-19 16:52:13.000000 uo_puddles-4.6/uo_puddles/good_ai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24737 2024-02-19 16:52:13.000000 uo_puddles-4.6/uo_puddles/good_ai_22.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-02-19 16:52:13.000000 uo_puddles-4.6/uo_puddles/gremcat_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-02-19 16:52:13.000000 uo_puddles-4.6/uo_puddles/gremcat_oo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24584 2024-02-19 16:52:13.000000 uo_puddles-4.6/uo_puddles/mlops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:52:23.240677 uo_puddles-4.6/uo_puddles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-19 16:52:23.000000 uo_puddles-4.6/uo_puddles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-02-19 16:52:23.000000 uo_puddles-4.6/uo_puddles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 16:52:23.000000 uo_puddles-4.6/uo_puddles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-19 16:52:23.000000 uo_puddles-4.6/uo_puddles.egg-info/top_level.txt
```

### Comparing `uo_puddles-4.5/LICENSE.txt` & `uo_puddles-4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uo_puddles-4.5/setup.py` & `uo_puddles-4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="uo_puddles",
-    version="4.5",    #also change pypi_version variable at top of library
+    version="4.6",    #also change pypi_version variable at top of library
     author="Stephen Fickas",
     author_email="stephenfickas@gmail.com",
     description="for cis423 class",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `uo_puddles-4.5/uo_puddles/CustomTukeyTransformer_unittest.py` & `uo_puddles-4.6/uo_puddles/CustomTukeyTransformer_unittest.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-4.5/uo_puddles/cis423.py` & `uo_puddles-4.6/uo_puddles/cis423.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-4.5/uo_puddles/good_ai.py` & `uo_puddles-4.6/uo_puddles/good_ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -645,15 +645,15 @@
         update_code_display(None)
 
     def update_code_display(change):
         clear_output(wait=True)
         #display(VBox(order_dropdowns + indentation_dropdowns))
         display(info_button, info_display, VBox(order_dropdowns + indentation_dropdowns))
         
-        code_display_html = "<br><strong>Current Code Configuration:</strong><br><br>"
+        code_display_html = "<br><strong>Current Code Configuration:</strong><br><hr>"
         for i, (order_dropdown, indent_dropdown) in enumerate(zip(order_dropdowns, indentation_dropdowns)):
             if order_dropdown.value == 'Select a statement':
                 statement_display = f"<em># Statement {i+1} not selected</em>"
                 indent_feedback = ""
                 indent_visual = ""
             else:
                 statement_color = "purple" if order_dropdown.value in distractors else "red"
@@ -767,15 +767,45 @@
   ]
   distractors = [
       "print('This is a distractor.')",
       "unused_var = 0"
   ]
   setup_simplified_code_exercise(statement_indent_pairs, distractors)
 
+def parsons_loop_1():
+  statement_indent_pairs = [
+    ('current_list = [4, 5, -7, -8, 9, 0]', 0),
+    ('new_list = []', 0),
+    ('for item in current_list:', 0),
+    ('if item >= 0:', 1),
+    ('new_list += [item]', 2),
+    ("print(f'{new_list=}')  #[4,5,9,0]", 0),
+  ]
+  distractors = [
+  ]
+  setup_simplified_code_exercise(statement_indent_pairs, distractors)
 
+def parsons_loop_2():
+  statement_indent_pairs = [
+    ("list_a = ['a', 'b', 'c']", 0),
+    ("list_b = [1, 2, 3]", 0),
+    ('zipped = []', 0),
+    ('for i in range(len(list_a)):', 0),
+    ('zipped += [[list_a[i], list_b[i]]]', 1),
+    ("print(f'{zipped=}')  #[['a', 1], ['b', 2], ['c', 3]]", 0)
+  ]
+  distractors = [
+  'for item2 in list_b:',
+  'zipped += [item1, item2]',
+  'for item1 in list_a:',
+  'zipped += [list_a[i], list_b[i]]',
+  'for i in range(4):',
+  'zipped = [[]]'
+  ]
+  setup_simplified_code_exercise(statement_indent_pairs, distractors)
```

### Comparing `uo_puddles-4.5/uo_puddles/good_ai_22.py` & `uo_puddles-4.6/uo_puddles/good_ai_22.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-4.5/uo_puddles/gremcat_df.py` & `uo_puddles-4.6/uo_puddles/gremcat_df.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-4.5/uo_puddles/gremcat_oo.py` & `uo_puddles-4.6/uo_puddles/gremcat_oo.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-4.5/uo_puddles/mlops.py` & `uo_puddles-4.6/uo_puddles/mlops.py`

 * *Files identical despite different names*

