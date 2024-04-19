# Comparing `tmp/wdl_lsp-0.0.82-py3-none-any.whl.zip` & `tmp/wdl_lsp-0.0.83-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 12759 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1232 b- defN 24-Apr-19 22:02 wdl_lsp/__init__.py
--rw-r--r--  2.0 unx     2261 b- defN 24-Apr-19 22:02 wdl_lsp/__main__.py
--rw-r--r--  2.0 unx    17170 b- defN 24-Apr-19 22:02 wdl_lsp/server.py
--rw-r--r--  2.0 unx     1232 b- defN 24-Apr-19 22:02 wdl_lsp/tests/__init__.py
--rw-r--r--  2.0 unx     1232 b- defN 24-Apr-19 22:02 wdl_lsp/tests/unit/__init__.py
--rw-r--r--  2.0 unx     3425 b- defN 24-Apr-19 22:02 wdl_lsp/tests/unit/test_features.py
--rw-r--r--  2.0 unx     5407 b- defN 24-Apr-19 22:02 wdl_lsp-0.0.82.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 22:02 wdl_lsp-0.0.82.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 24-Apr-19 22:02 wdl_lsp-0.0.82.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-19 22:02 wdl_lsp-0.0.82.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      885 b- defN 24-Apr-19 22:02 wdl_lsp-0.0.82.dist-info/RECORD
+-rw-r--r--  2.0 unx     1232 b- defN 24-Apr-19 22:09 wdl_lsp/__init__.py
+-rw-r--r--  2.0 unx     2261 b- defN 24-Apr-19 22:09 wdl_lsp/__main__.py
+-rw-r--r--  2.0 unx    17170 b- defN 24-Apr-19 22:09 wdl_lsp/server.py
+-rw-r--r--  2.0 unx     1232 b- defN 24-Apr-19 22:09 wdl_lsp/tests/__init__.py
+-rw-r--r--  2.0 unx     1232 b- defN 24-Apr-19 22:09 wdl_lsp/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     3425 b- defN 24-Apr-19 22:09 wdl_lsp/tests/unit/test_features.py
+-rw-r--r--  2.0 unx     5407 b- defN 24-Apr-19 22:09 wdl_lsp-0.0.83.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 22:09 wdl_lsp-0.0.83.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 24-Apr-19 22:09 wdl_lsp-0.0.83.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-19 22:09 wdl_lsp-0.0.83.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      885 b- defN 24-Apr-19 22:09 wdl_lsp-0.0.83.dist-info/RECORD
 11 files, 32994 bytes uncompressed, 11265 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: wdl_lsp/tests/unit/__init__.py
 Comment: 
 
 Filename: wdl_lsp/tests/unit/test_features.py
 Comment: 
 
-Filename: wdl_lsp-0.0.82.dist-info/METADATA
+Filename: wdl_lsp-0.0.83.dist-info/METADATA
 Comment: 
 
-Filename: wdl_lsp-0.0.82.dist-info/WHEEL
+Filename: wdl_lsp-0.0.83.dist-info/WHEEL
 Comment: 
 
-Filename: wdl_lsp-0.0.82.dist-info/entry_points.txt
+Filename: wdl_lsp-0.0.83.dist-info/entry_points.txt
 Comment: 
 
-Filename: wdl_lsp-0.0.82.dist-info/top_level.txt
+Filename: wdl_lsp-0.0.83.dist-info/top_level.txt
 Comment: 
 
-Filename: wdl_lsp-0.0.82.dist-info/RECORD
+Filename: wdl_lsp-0.0.83.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `wdl_lsp-0.0.82.dist-info/METADATA` & `wdl_lsp-0.0.83.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wdl-lsp
-Version: 0.0.82
+Version: 0.0.83
 Summary: Language Server Protocol (LSP) implementation for Workflow Definition Language (WDL)
 Home-page: https://github.com/broadinstitute/wdl-ide
 Author: Broad Institute
 License: BSD 3-clause "New" or "Revised" License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Interpreters
```

## Comparing `wdl_lsp-0.0.82.dist-info/RECORD` & `wdl_lsp-0.0.83.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 wdl_lsp/__init__.py,sha256=lMZC-rLprL4e3XxDvySryn-T2h4jmtWWJk94Ecp6zqA,1232
 wdl_lsp/__main__.py,sha256=gKv1XaZKKFj_srZ3cU8e0rjUnc9E3N6IFWi5-IyGOIc,2261
 wdl_lsp/server.py,sha256=WFOCBklvE4ZZnGtDB7flycwzTlmPnAhaccXgeFohmq8,17170
 wdl_lsp/tests/__init__.py,sha256=lMZC-rLprL4e3XxDvySryn-T2h4jmtWWJk94Ecp6zqA,1232
 wdl_lsp/tests/unit/__init__.py,sha256=lMZC-rLprL4e3XxDvySryn-T2h4jmtWWJk94Ecp6zqA,1232
 wdl_lsp/tests/unit/test_features.py,sha256=S-EwVcbJRjwa8S74TJl55bcupiB-QJ_1XggV9GKHdpE,3425
-wdl_lsp-0.0.82.dist-info/METADATA,sha256=30B0mMSzqKLIQKMJKC_O4Dsgfw6np5RT00YV4enSqlw,5407
-wdl_lsp-0.0.82.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-wdl_lsp-0.0.82.dist-info/entry_points.txt,sha256=bXoe3-yK9BxkZx3_rmFzi1jRXnSC4EEJSfpHRCNCYnY,50
-wdl_lsp-0.0.82.dist-info/top_level.txt,sha256=VysaomJqq_3fE9v1Yup93pbHMPzph0p4WoQ8JdYHIdI,8
-wdl_lsp-0.0.82.dist-info/RECORD,,
+wdl_lsp-0.0.83.dist-info/METADATA,sha256=kcGulC4G59f-zTZ6bVDriHYgogCJBz0ZutN4tIyYoMM,5407
+wdl_lsp-0.0.83.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+wdl_lsp-0.0.83.dist-info/entry_points.txt,sha256=bXoe3-yK9BxkZx3_rmFzi1jRXnSC4EEJSfpHRCNCYnY,50
+wdl_lsp-0.0.83.dist-info/top_level.txt,sha256=VysaomJqq_3fE9v1Yup93pbHMPzph0p4WoQ8JdYHIdI,8
+wdl_lsp-0.0.83.dist-info/RECORD,,
```

