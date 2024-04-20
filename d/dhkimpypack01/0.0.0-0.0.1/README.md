# Comparing `tmp/dhkimpypack01-0.0.0-py3-none-any.whl.zip` & `tmp/dhkimpypack01-0.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2185 bytes, number of entries: 6
--rw-r--r--  2.0 unx      139 b- defN 24-Apr-20 14:13 mycalc/calculator.py
--rw-r--r--  2.0 unx     1065 b- defN 24-Apr-20 14:39 dhkimpypack01-0.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      259 b- defN 24-Apr-20 14:39 dhkimpypack01-0.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-20 14:39 dhkimpypack01-0.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-20 14:39 dhkimpypack01-0.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      490 b- defN 24-Apr-20 14:39 dhkimpypack01-0.0.0.dist-info/RECORD
-6 files, 2052 bytes uncompressed, 1289 bytes compressed:  37.2%
+Zip file size: 2186 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       95 b- defN 24-Apr-20 14:54 mycalc/calculator.py
+-rw-r--r--  2.0 unx     1065 b- defN 24-Apr-20 14:55 dhkimpypack01-0.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      259 b- defN 24-Apr-20 14:55 dhkimpypack01-0.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-20 14:55 dhkimpypack01-0.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-20 14:55 dhkimpypack01-0.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      489 b- defN 24-Apr-20 14:55 dhkimpypack01-0.0.1.dist-info/RECORD
+6 files, 2007 bytes uncompressed, 1290 bytes compressed:  35.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: mycalc/calculator.py
 Comment: 
 
-Filename: dhkimpypack01-0.0.0.dist-info/LICENSE
+Filename: dhkimpypack01-0.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: dhkimpypack01-0.0.0.dist-info/METADATA
+Filename: dhkimpypack01-0.0.1.dist-info/METADATA
 Comment: 
 
-Filename: dhkimpypack01-0.0.0.dist-info/WHEEL
+Filename: dhkimpypack01-0.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: dhkimpypack01-0.0.0.dist-info/top_level.txt
+Filename: dhkimpypack01-0.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: dhkimpypack01-0.0.0.dist-info/RECORD
+Filename: dhkimpypack01-0.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mycalc/calculator.py

```diff
@@ -1,8 +1,4 @@
-def add(a, b):
-  return a + b
-def subtract(a, b):
-  return a - b
-def multiply(a, b):
-  return a * b
-def divide(a, b):
-  return a / b
+import numpy as np
+import pandas as pd
+import matplotlib.pyplot as plt
+from scipy import stats
```

## Comparing `dhkimpypack01-0.0.0.dist-info/LICENSE` & `dhkimpypack01-0.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

