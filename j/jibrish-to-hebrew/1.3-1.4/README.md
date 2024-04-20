# Comparing `tmp/jibrish_to_hebrew-1.3.tar.gz` & `tmp/jibrish_to_hebrew-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jibrish_to_hebrew-1.3.tar", last modified: Sat Feb  3 23:25:01 2024, max compression
+gzip compressed data, was "jibrish_to_hebrew-1.4.tar", last modified: Sat Apr 20 18:53:32 2024, max compression
```

## Comparing `jibrish_to_hebrew-1.3.tar` & `jibrish_to_hebrew-1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 23:25:01.444130 jibrish_to_hebrew-1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-02-03 23:24:49.000000 jibrish_to_hebrew-1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-02-03 23:25:01.440130 jibrish_to_hebrew-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-02-03 23:24:49.000000 jibrish_to_hebrew-1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 23:25:01.440130 jibrish_to_hebrew-1.3/jibrish_to_hebrew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-02-03 23:25:01.000000 jibrish_to_hebrew-1.3/jibrish_to_hebrew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-03 23:25:01.000000 jibrish_to_hebrew-1.3/jibrish_to_hebrew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 23:25:01.000000 jibrish_to_hebrew-1.3/jibrish_to_hebrew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-03 23:25:01.000000 jibrish_to_hebrew-1.3/jibrish_to_hebrew.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-02-03 23:24:49.000000 jibrish_to_hebrew-1.3/jibrish_to_hebrew.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-03 23:25:01.444130 jibrish_to_hebrew-1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-03 23:24:49.000000 jibrish_to_hebrew-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:53:32.755848 jibrish_to_hebrew-1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-20 18:53:21.000000 jibrish_to_hebrew-1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-20 18:53:32.755848 jibrish_to_hebrew-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-20 18:53:21.000000 jibrish_to_hebrew-1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:53:32.755848 jibrish_to_hebrew-1.4/jibrish_to_hebrew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-20 18:53:32.000000 jibrish_to_hebrew-1.4/jibrish_to_hebrew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-20 18:53:32.000000 jibrish_to_hebrew-1.4/jibrish_to_hebrew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:53:32.000000 jibrish_to_hebrew-1.4/jibrish_to_hebrew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-20 18:53:32.000000 jibrish_to_hebrew-1.4/jibrish_to_hebrew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-20 18:53:21.000000 jibrish_to_hebrew-1.4/jibrish_to_hebrew.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:53:32.755848 jibrish_to_hebrew-1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-20 18:53:21.000000 jibrish_to_hebrew-1.4/setup.py
```

### Comparing `jibrish_to_hebrew-1.3/LICENSE` & `jibrish_to_hebrew-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jibrish_to_hebrew-1.3/PKG-INFO` & `jibrish_to_hebrew-1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: jibrish_to_hebrew
-Version: 1.3
+Version: 1.4
+Project-URL: Source, https://github.com/NHLOCAL/jibrish-to-hebrew/actions
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# jibrish_to_hebrew
+# jibrish to hebrew
 
 ## Description
 
-`jibrish_to_hebrew` is a Python function that simplifies the conversion between garbled text and Hebrew. It can convert a garbled Hebrew string to plain Hebrew or transform Hebrew text into gibberish and vice versa. 
+`jibrish_to_hebrew` is a Python function that simplifies the conversion between garbled text and Hebrew. It can convert a garbled Hebrew string to plain Hebrew or transform Hebrew text into jibrish and vice versa.
+
+for example: 'ùìåí ìëåìí' --> 'שלום לכולם'
+ 
 
 ## Usage
 
 ### convert function - fix_jibrish
 
 The function takes the following parameters:
 
@@ -20,53 +24,68 @@
   Provide a garbled Hebrew string as input to be converted.
 
 - **Parameter 2 (optional)**: *Conversion mode*  
   You can specify the conversion mode using this optional parameter. It accepts two values:
   - `"heb"`: To convert the input to Hebrew.
   - `"jib"`: To convert the input to gibrish.
   
+  Default is `heb`
+  
 
 ### test function - check_jibrish
 
 A function to check if a certain string contains correct Hebrew or corrupted Hebrew
 
 Suitable for checking metadata of songs
 
 - **Parameter**:
-    Parameter = A text string
-
-- **return value**
+  A text string
 
-`True` or `False`
+- **return value**:
+  `True` If the string is garbled, or `False` if she is ok
   
 
 
 ## Example
 
 ```
-from jibrish_to_hebrew import fix_jibrish
+from jibrish_to_hebrew import fix_jibrish, check_jibrish
+
+
+jibrish_string = 'ùìåí ìëåìí'
+hebrew_string = 'שלום לכולם'
 
 # Convert garbled text to plain Hebrew
-result = fix_jibrish("your_garbled_string", conversion_mode="heb")
+heb_result = fix_jibrish(jibrish_string, "heb")
 
-# Convert Hebrew text to gibberish
-result = fix_jibrish("your_hebrew_string", conversion_mode="jib")
+# Convert Hebrew text to gibrish
+jib_result = fix_jibrish(hebrew_string, "jib")
 
 # Check if a string contains garbled text
-result = check_jibrish("your__string")
+bool_result = check_jibrish(jibrish_string)
 
 ```
 
+## Return
+
+```
+print(f'{garbled_string}: {result_heb}')
+print(bool_result)
+
+ùìåí ìëåìí: שלום לכולם
+True
+
+```
 
 
 
 ## Installation
 
 You can install this package using pip:
 
 ```
-pip install jibrish_to_hebrew
+pip install jibrish-to-hebrew
 ```
 
 ## Acknowledgments
 
 This software is created and maintained by nh.local11@gmail.com.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jibrish_to_hebrew-1.3/README.md` & `jibrish_to_hebrew-1.4/jibrish_to_hebrew.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,22 @@
-# jibrish_to_hebrew
+Metadata-Version: 2.1
+Name: jibrish_to_hebrew
+Version: 1.4
+Project-URL: Source, https://github.com/NHLOCAL/jibrish-to-hebrew/actions
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# jibrish to hebrew
 
 ## Description
 
-`jibrish_to_hebrew` is a Python function that simplifies the conversion between garbled text and Hebrew. It can convert a garbled Hebrew string to plain Hebrew or transform Hebrew text into gibberish and vice versa. 
+`jibrish_to_hebrew` is a Python function that simplifies the conversion between garbled text and Hebrew. It can convert a garbled Hebrew string to plain Hebrew or transform Hebrew text into jibrish and vice versa.
+
+for example: 'ùìåí ìëåìí' --> 'שלום לכולם'
+ 
 
 ## Usage
 
 ### convert function - fix_jibrish
 
 The function takes the following parameters:
 
@@ -14,53 +24,68 @@
   Provide a garbled Hebrew string as input to be converted.
 
 - **Parameter 2 (optional)**: *Conversion mode*  
   You can specify the conversion mode using this optional parameter. It accepts two values:
   - `"heb"`: To convert the input to Hebrew.
   - `"jib"`: To convert the input to gibrish.
   
+  Default is `heb`
+  
 
 ### test function - check_jibrish
 
 A function to check if a certain string contains correct Hebrew or corrupted Hebrew
 
 Suitable for checking metadata of songs
 
 - **Parameter**:
-    Parameter = A text string
+  A text string
 
-- **return value**
-
-`True` or `False`
+- **return value**:
+  `True` If the string is garbled, or `False` if she is ok
   
 
 
 ## Example
 
 ```
-from jibrish_to_hebrew import fix_jibrish
+from jibrish_to_hebrew import fix_jibrish, check_jibrish
+
+
+jibrish_string = 'ùìåí ìëåìí'
+hebrew_string = 'שלום לכולם'
 
 # Convert garbled text to plain Hebrew
-result = fix_jibrish("your_garbled_string", conversion_mode="heb")
+heb_result = fix_jibrish(jibrish_string, "heb")
 
-# Convert Hebrew text to gibberish
-result = fix_jibrish("your_hebrew_string", conversion_mode="jib")
+# Convert Hebrew text to gibrish
+jib_result = fix_jibrish(hebrew_string, "jib")
 
 # Check if a string contains garbled text
-result = check_jibrish("your__string")
+bool_result = check_jibrish(jibrish_string)
 
 ```
 
+## Return
+
+```
+print(f'{garbled_string}: {result_heb}')
+print(bool_result)
+
+ùìåí ìëåìí: שלום לכולם
+True
+
+```
 
 
 
 ## Installation
 
 You can install this package using pip:
 
 ```
-pip install jibrish_to_hebrew
+pip install jibrish-to-hebrew
 ```
 
 ## Acknowledgments
 
-This software is created and maintained by nh.local11@gmail.com.
+This software is created and maintained by nh.local11@gmail.com.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jibrish_to_hebrew-1.3/jibrish_to_hebrew.egg-info/PKG-INFO` & `jibrish_to_hebrew-1.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-Metadata-Version: 2.1
-Name: jibrish_to_hebrew
-Version: 1.3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# jibrish_to_hebrew
+# jibrish to hebrew
 
 ## Description
 
-`jibrish_to_hebrew` is a Python function that simplifies the conversion between garbled text and Hebrew. It can convert a garbled Hebrew string to plain Hebrew or transform Hebrew text into gibberish and vice versa. 
+`jibrish_to_hebrew` is a Python function that simplifies the conversion between garbled text and Hebrew. It can convert a garbled Hebrew string to plain Hebrew or transform Hebrew text into jibrish and vice versa.
+
+for example: 'ùìåí ìëåìí' --> 'שלום לכולם'
+ 
 
 ## Usage
 
 ### convert function - fix_jibrish
 
 The function takes the following parameters:
 
@@ -20,53 +17,68 @@
   Provide a garbled Hebrew string as input to be converted.
 
 - **Parameter 2 (optional)**: *Conversion mode*  
   You can specify the conversion mode using this optional parameter. It accepts two values:
   - `"heb"`: To convert the input to Hebrew.
   - `"jib"`: To convert the input to gibrish.
   
+  Default is `heb`
+  
 
 ### test function - check_jibrish
 
 A function to check if a certain string contains correct Hebrew or corrupted Hebrew
 
 Suitable for checking metadata of songs
 
 - **Parameter**:
-    Parameter = A text string
+  A text string
 
-- **return value**
-
-`True` or `False`
+- **return value**:
+  `True` If the string is garbled, or `False` if she is ok
   
 
 
 ## Example
 
 ```
-from jibrish_to_hebrew import fix_jibrish
+from jibrish_to_hebrew import fix_jibrish, check_jibrish
+
+
+jibrish_string = 'ùìåí ìëåìí'
+hebrew_string = 'שלום לכולם'
 
 # Convert garbled text to plain Hebrew
-result = fix_jibrish("your_garbled_string", conversion_mode="heb")
+heb_result = fix_jibrish(jibrish_string, "heb")
 
-# Convert Hebrew text to gibberish
-result = fix_jibrish("your_hebrew_string", conversion_mode="jib")
+# Convert Hebrew text to gibrish
+jib_result = fix_jibrish(hebrew_string, "jib")
 
 # Check if a string contains garbled text
-result = check_jibrish("your__string")
+bool_result = check_jibrish(jibrish_string)
 
 ```
 
+## Return
+
+```
+print(f'{garbled_string}: {result_heb}')
+print(bool_result)
+
+ùìåí ìëåìí: שלום לכולם
+True
+
+```
 
 
 
 ## Installation
 
 You can install this package using pip:
 
 ```
-pip install jibrish_to_hebrew
+pip install jibrish-to-hebrew
 ```
 
 ## Acknowledgments
 
 This software is created and maintained by nh.local11@gmail.com.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jibrish_to_hebrew-1.3/jibrish_to_hebrew.py` & `jibrish_to_hebrew-1.4/jibrish_to_hebrew.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,9 +62,9 @@
         return True
     else:
         return False
         
 
 if __name__ == '__main__':
     string = "àìáåí ìà éãåò & - 3"
-    print(jibrish_to_hebrew(string))
+    print(fix_jibrish(string))
```

