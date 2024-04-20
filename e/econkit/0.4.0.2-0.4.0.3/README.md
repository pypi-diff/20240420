# Comparing `tmp/econkit-0.4.0.2.tar.gz` & `tmp/econkit-0.4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econkit-0.4.0.2.tar", last modified: Wed Mar 13 18:50:46 2024, max compression
+gzip compressed data, was "econkit-0.4.0.3.tar", last modified: Sat Apr 20 08:19:02 2024, max compression
```

## Comparing `econkit-0.4.0.2.tar` & `econkit-0.4.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 stefanstavrianos  (1000) stefanstavrianos  (1000)        0 2024-03-13 18:50:46.367998 econkit-0.4.0.2/
--rw-rw-r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)     1519 2024-01-02 09:33:15.000000 econkit-0.4.0.2/LICENSE
--rw-r--r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)     5322 2024-03-13 18:50:46.367998 econkit-0.4.0.2/PKG-INFO
--rw-rw-r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)     2484 2024-01-22 00:07:57.000000 econkit-0.4.0.2/README.md
-drwxrwxr-x   0 stefanstavrianos  (1000) stefanstavrianos  (1000)        0 2024-03-13 18:50:46.367998 econkit-0.4.0.2/econkit/
--rw-rw-r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)     1289 2024-03-13 17:42:56.000000 econkit-0.4.0.2/econkit/__init__.py
--rw-rw-r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)     6433 2024-03-13 18:50:33.000000 econkit-0.4.0.2/econkit/econometrics.py
--rw-rw-r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)     5237 2024-03-13 18:23:15.000000 econkit-0.4.0.2/econkit/finance.py
--rw-rw-r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)     1903 2024-01-25 21:43:21.000000 econkit-0.4.0.2/econkit/plots.py
--rw-rw-r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)       37 2024-03-13 18:50:36.000000 econkit-0.4.0.2/econkit/version.py
-drwxrwxr-x   0 stefanstavrianos  (1000) stefanstavrianos  (1000)        0 2024-03-13 18:50:46.367998 econkit-0.4.0.2/econkit.egg-info/
--rw-r--r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)     5322 2024-03-13 18:50:46.000000 econkit-0.4.0.2/econkit.egg-info/PKG-INFO
--rw-rw-r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)      279 2024-03-13 18:50:46.000000 econkit-0.4.0.2/econkit.egg-info/SOURCES.txt
--rw-rw-r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)        1 2024-03-13 18:50:46.000000 econkit-0.4.0.2/econkit.egg-info/dependency_links.txt
--rw-rw-r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)       46 2024-03-13 18:50:46.000000 econkit-0.4.0.2/econkit.egg-info/requires.txt
--rw-rw-r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)        8 2024-03-13 18:50:46.000000 econkit-0.4.0.2/econkit.egg-info/top_level.txt
--rw-rw-r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)       38 2024-03-13 18:50:46.367998 econkit-0.4.0.2/setup.cfg
--rw-rw-r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)     1302 2024-01-07 15:54:10.000000 econkit-0.4.0.2/setup.py
+drwxr-xr-x   0 stefanstavrianos  (1000) stefanstavrianos  (1000)        0 2024-04-20 08:19:02.976132 econkit-0.4.0.3/
+-rwxr-xr-x   0 stefanstavrianos  (1000) stefanstavrianos  (1000)     1519 2024-01-02 09:33:15.000000 econkit-0.4.0.3/LICENSE
+-rw-r--r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)     5186 2024-04-20 08:19:02.976132 econkit-0.4.0.3/PKG-INFO
+-rwxr-xr-x   0 stefanstavrianos  (1000) stefanstavrianos  (1000)     2484 2024-01-22 00:07:57.000000 econkit-0.4.0.3/README.md
+drwxr-xr-x   0 stefanstavrianos  (1000) stefanstavrianos  (1000)        0 2024-04-20 08:19:02.976132 econkit-0.4.0.3/econkit/
+-rwxr-xr-x   0 stefanstavrianos  (1000) stefanstavrianos  (1000)     1289 2024-03-13 17:42:56.000000 econkit-0.4.0.3/econkit/__init__.py
+-rwxr-xr-x   0 stefanstavrianos  (1000) stefanstavrianos  (1000)     6683 2024-04-20 07:55:26.000000 econkit-0.4.0.3/econkit/econometrics.py
+-rwxr-xr-x   0 stefanstavrianos  (1000) stefanstavrianos  (1000)     5237 2024-03-13 18:23:15.000000 econkit-0.4.0.3/econkit/finance.py
+-rwxr-xr-x   0 stefanstavrianos  (1000) stefanstavrianos  (1000)     1903 2024-01-25 21:43:21.000000 econkit-0.4.0.3/econkit/plots.py
+-rwxr-xr-x   0 stefanstavrianos  (1000) stefanstavrianos  (1000)       37 2024-04-20 08:11:00.000000 econkit-0.4.0.3/econkit/version.py
+drwxr-xr-x   0 stefanstavrianos  (1000) stefanstavrianos  (1000)        0 2024-04-20 08:19:02.976132 econkit-0.4.0.3/econkit.egg-info/
+-rw-r--r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)     5186 2024-04-20 08:19:02.000000 econkit-0.4.0.3/econkit.egg-info/PKG-INFO
+-rw-r--r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)      279 2024-04-20 08:19:02.000000 econkit-0.4.0.3/econkit.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)        1 2024-04-20 08:19:02.000000 econkit-0.4.0.3/econkit.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)       46 2024-04-20 08:19:02.000000 econkit-0.4.0.3/econkit.egg-info/requires.txt
+-rw-r--r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)        8 2024-04-20 08:19:02.000000 econkit-0.4.0.3/econkit.egg-info/top_level.txt
+-rw-r--r--   0 stefanstavrianos  (1000) stefanstavrianos  (1000)       38 2024-04-20 08:19:02.976132 econkit-0.4.0.3/setup.cfg
+-rwxr-xr-x   0 stefanstavrianos  (1000) stefanstavrianos  (1000)     1302 2024-01-07 15:54:10.000000 econkit-0.4.0.3/setup.py
```

### Comparing `econkit-0.4.0.2/LICENSE` & `econkit-0.4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `econkit-0.4.0.2/PKG-INFO` & `econkit-0.4.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econkit
-Version: 0.4.0.2
+Version: 0.4.0.3
 Summary: Advanced Econometric Analysis Tools
 Home-page: https://www.stefanstavrianos.eu/
 Author: Stefanos Stavrianos
 Author-email: contact@stefanstavrianos.eu
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Stefanos Stavrianos
@@ -47,20 +47,14 @@
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: scipy
-Requires-Dist: yfinance
-Requires-Dist: matplotlib
-Requires-Dist: plotly
 
 
 # Econkit
 
 ## Introduction
 Econkit is a comprehensive Python library designed for economic and financial data analysis. It offers a wide range of functionalities, from descriptive statistics to advanced portfolio analysis, making it a valuable tool for economists, financial analysts, and researchers.
```

### Comparing `econkit-0.4.0.2/README.md` & `econkit-0.4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `econkit-0.4.0.2/econkit/__init__.py` & `econkit-0.4.0.3/econkit/__init__.py`

 * *Files identical despite different names*

### Comparing `econkit-0.4.0.2/econkit/econometrics.py` & `econkit-0.4.0.3/econkit/econometrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,28 +67,32 @@
 
 Returns:
 None
     This function prints the correlation matrix and optionally the p-value
     matrix directly to the console.
 """
 
+import numpy as np
+import pandas as pd
 import scipy.stats
 
-def correlation(df, method="Pearson", p="F"):
+def correlation(df, method="Pearson", p=False):
     def format_p_value(p_value):
         formatted = f"{p_value:0.3f}"
         if formatted.startswith("0."):
             return formatted[1:]
         return formatted
 
     numeric_df = df.select_dtypes(include=[np.number])
     if method == "Pearson":
         print("\n" + "=" * 21 + f"\n {method} Correlation\n" + "=" * 21)
-    else:
+    elif method == "Spearman":
         print("\n" + "=" * 27 + f"\n {method} Rank Correlation\n" + "=" * 27)
+    elif method == "Kendall":
+        print("\n" + "=" * 26 + f"\n {method} Rank Correlation\n" + "=" * 26)
 
     corr_matrix = pd.DataFrame(index=numeric_df.columns, columns=numeric_df.columns)
     pmatrix = pd.DataFrame(index=numeric_df.columns, columns=numeric_df.columns)
 
     keys = numeric_df.columns.tolist()
 
     for i, key1 in enumerate(keys):
@@ -108,45 +112,48 @@
                 corr_matrix.at[key2, key1] = 'nan'
                 continue
 
             if method == 'Spearman':
                 correlation, p_value = scipy.stats.spearmanr(data1, data2)
             elif method == 'Pearson':
                 correlation, p_value = scipy.stats.pearsonr(data1, data2)
+            elif method == 'Kendall':
+                correlation, p_value = scipy.stats.kendalltau(data1, data2)
 
             pmatrix.at[key1, key2] = format_p_value(p_value)
             pmatrix.at[key2, key1] = format_p_value(p_value)
 
             stars = "     "
             if p_value < 0.001:
                 stars = " *** "
             elif p_value < 0.01:
                 stars = " **  "
             elif p_value < 0.05:
-                stars = " *   "               
+                stars = " *   "
             elif p_value < 0.1:
                 stars = " .   "
-                
+
             correlation_str = f"{format_p_value(correlation)}{stars}"
             corr_matrix.at[key1, key2] = correlation_str
             corr_matrix.at[key2, key1] = correlation_str
 
     corr_matrix_str = corr_matrix.to_string(sparsify=True, justify='center')
     explanation = "\n\n--\nSignif. codes:  0.001 '***', 0.01 '**', 0.05 '*', 0.1 '.'"
 
     print("\n\n>> Correlation Matrix <<\n")
     print(corr_matrix_str + explanation)
 
-    if p == "T":
+    if p:
         print("\n\n>> P-Value Matrix <<\n")
-        print(pmatrix)
+        print(pmatrix.to_string())
         print("\n")
-    elif p == "F":
+    else:
         print("\n")
 
+
 ## table(column_name, *dataframes)
 """
 Creates a DataFrame by combining a specified column from multiple DataFrames.
 
 Parameters:
 column_name: str
     The name of the column to be extracted from each DataFrame.
```

### Comparing `econkit-0.4.0.2/econkit/finance.py` & `econkit-0.4.0.3/econkit/finance.py`

 * *Files identical despite different names*

### Comparing `econkit-0.4.0.2/econkit/plots.py` & `econkit-0.4.0.3/econkit/plots.py`

 * *Files identical despite different names*

### Comparing `econkit-0.4.0.2/econkit.egg-info/PKG-INFO` & `econkit-0.4.0.3/econkit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econkit
-Version: 0.4.0.2
+Version: 0.4.0.3
 Summary: Advanced Econometric Analysis Tools
 Home-page: https://www.stefanstavrianos.eu/
 Author: Stefanos Stavrianos
 Author-email: contact@stefanstavrianos.eu
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Stefanos Stavrianos
@@ -47,20 +47,14 @@
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: scipy
-Requires-Dist: yfinance
-Requires-Dist: matplotlib
-Requires-Dist: plotly
 
 
 # Econkit
 
 ## Introduction
 Econkit is a comprehensive Python library designed for economic and financial data analysis. It offers a wide range of functionalities, from descriptive statistics to advanced portfolio analysis, making it a valuable tool for economists, financial analysts, and researchers.
```

### Comparing `econkit-0.4.0.2/setup.py` & `econkit-0.4.0.3/setup.py`

 * *Files identical despite different names*

