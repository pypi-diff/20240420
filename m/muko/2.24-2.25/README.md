# Comparing `tmp/muko-2.24-py3-none-any.whl.zip` & `tmp/muko-2.25-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 1986922 bytes, number of entries: 10
+Zip file size: 2025599 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat       20 b- defN 24-Mar-13 17:30 muko/__init__.py
--rw-rw-rw-  2.0 fat   605184 b- defN 24-Apr-15 17:09 muko/cmuko.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   709120 b- defN 24-Apr-19 18:44 muko/cmuko.cp38-win_amd64.pyd
 -rw-rw-rw-  2.0 fat   883832 b- defN 24-Apr-15 17:08 muko/cmuko.cpython-38-darwin.so
 -rw-rw-rw-  2.0 fat  2082964 b- defN 24-Feb-08 07:11 muko/font/default.otf
--rw-rw-rw-  2.0 fat     1074 b- defN 24-Apr-15 17:09 muko-2.24.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1213 b- defN 24-Apr-15 17:09 muko-2.24.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-15 17:09 muko-2.24.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 24-Apr-15 17:09 muko-2.24.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-15 17:09 muko-2.24.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      786 b- defN 24-Apr-15 17:09 muko-2.24.dist-info/RECORD
-10 files, 3575190 bytes uncompressed, 1985596 bytes compressed:  44.5%
+-rw-rw-rw-  2.0 fat     1074 b- defN 24-Apr-19 18:44 muko-2.25.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1213 b- defN 24-Apr-19 18:44 muko-2.25.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-19 18:44 muko-2.25.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 24-Apr-19 18:44 muko-2.25.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-19 18:44 muko-2.25.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      786 b- defN 24-Apr-19 18:44 muko-2.25.dist-info/RECORD
+10 files, 3679126 bytes uncompressed, 2024273 bytes compressed:  45.0%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: muko/cmuko.cpython-38-darwin.so
 Comment: 
 
 Filename: muko/font/default.otf
 Comment: 
 
-Filename: muko-2.24.dist-info/LICENSE
+Filename: muko-2.25.dist-info/LICENSE
 Comment: 
 
-Filename: muko-2.24.dist-info/METADATA
+Filename: muko-2.25.dist-info/METADATA
 Comment: 
 
-Filename: muko-2.24.dist-info/WHEEL
+Filename: muko-2.25.dist-info/WHEEL
 Comment: 
 
-Filename: muko-2.24.dist-info/entry_points.txt
+Filename: muko-2.25.dist-info/entry_points.txt
 Comment: 
 
-Filename: muko-2.24.dist-info/top_level.txt
+Filename: muko-2.25.dist-info/top_level.txt
 Comment: 
 
-Filename: muko-2.24.dist-info/RECORD
+Filename: muko-2.25.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `muko-2.24.dist-info/LICENSE` & `muko-2.25.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `muko-2.24.dist-info/METADATA` & `muko-2.25.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muko
-Version: 2.24
+Version: 2.25
 Summary: 加速实现AIGC、自动办公的中文编程工具
 Home-page: https://www.mikooo.cn
 Author: Milk
 Author-email: 719496375@qq.com
 License: The MIT License
 Platform: win64
 Classifier: Programming Language :: Python :: 3.8
```

