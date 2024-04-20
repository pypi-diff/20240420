# Comparing `tmp/muko-2.25-py3-none-any.whl.zip` & `tmp/muko-2.26-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 2025599 bytes, number of entries: 10
+Zip file size: 2026468 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat       20 b- defN 24-Mar-13 17:30 muko/__init__.py
--rw-rw-rw-  2.0 fat   709120 b- defN 24-Apr-19 18:44 muko/cmuko.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   710144 b- defN 24-Apr-20 03:53 muko/cmuko.cp38-win_amd64.pyd
 -rw-rw-rw-  2.0 fat   883832 b- defN 24-Apr-15 17:08 muko/cmuko.cpython-38-darwin.so
 -rw-rw-rw-  2.0 fat  2082964 b- defN 24-Feb-08 07:11 muko/font/default.otf
--rw-rw-rw-  2.0 fat     1074 b- defN 24-Apr-19 18:44 muko-2.25.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1213 b- defN 24-Apr-19 18:44 muko-2.25.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-19 18:44 muko-2.25.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 24-Apr-19 18:44 muko-2.25.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-19 18:44 muko-2.25.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      786 b- defN 24-Apr-19 18:44 muko-2.25.dist-info/RECORD
-10 files, 3679126 bytes uncompressed, 2024273 bytes compressed:  45.0%
+-rw-rw-rw-  2.0 fat     1074 b- defN 24-Apr-20 03:53 muko-2.26.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1213 b- defN 24-Apr-20 03:53 muko-2.26.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-20 03:53 muko-2.26.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 24-Apr-20 03:53 muko-2.26.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-20 03:53 muko-2.26.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      786 b- defN 24-Apr-20 03:53 muko-2.26.dist-info/RECORD
+10 files, 3680150 bytes uncompressed, 2025142 bytes compressed:  45.0%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: muko/cmuko.cpython-38-darwin.so
 Comment: 
 
 Filename: muko/font/default.otf
 Comment: 
 
-Filename: muko-2.25.dist-info/LICENSE
+Filename: muko-2.26.dist-info/LICENSE
 Comment: 
 
-Filename: muko-2.25.dist-info/METADATA
+Filename: muko-2.26.dist-info/METADATA
 Comment: 
 
-Filename: muko-2.25.dist-info/WHEEL
+Filename: muko-2.26.dist-info/WHEEL
 Comment: 
 
-Filename: muko-2.25.dist-info/entry_points.txt
+Filename: muko-2.26.dist-info/entry_points.txt
 Comment: 
 
-Filename: muko-2.25.dist-info/top_level.txt
+Filename: muko-2.26.dist-info/top_level.txt
 Comment: 
 
-Filename: muko-2.25.dist-info/RECORD
+Filename: muko-2.26.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `muko-2.25.dist-info/LICENSE` & `muko-2.26.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `muko-2.25.dist-info/METADATA` & `muko-2.26.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muko
-Version: 2.25
+Version: 2.26
 Summary: 加速实现AIGC、自动办公的中文编程工具
 Home-page: https://www.mikooo.cn
 Author: Milk
 Author-email: 719496375@qq.com
 License: The MIT License
 Platform: win64
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `muko-2.25.dist-info/RECORD` & `muko-2.26.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 muko/__init__.py,sha256=CCRGa1csLmHKI_CslhtoPnqhEJA3mszIsRjACQuz5iE,20
-muko/cmuko.cp38-win_amd64.pyd,sha256=1CWvS7xQ3SbKGwSQAemQ285ZIDiz385_yTEoKHFHJi8,709120
+muko/cmuko.cp38-win_amd64.pyd,sha256=6SlZ-ToASjrSOvOtRlK6Su5SgSHXan84AtOg5ogElzA,710144
 muko/cmuko.cpython-38-darwin.so,sha256=ohiQYqcfXY9okYZbpInk9vEUKr07FwlXLytekb58txo,883832
 muko/font/default.otf,sha256=ZMqD7VMsbmTwwTRN4d72gVQLIekvjl5SSCvxs8-O4GA,2082964
-muko-2.25.dist-info/LICENSE,sha256=RwagnXR-4KxFgkvsh5PWaPhlca1CH_BNf-ozi5vp0fw,1074
-muko-2.25.dist-info/METADATA,sha256=W371_8hKHnQp8zxobX4nq0-s7mDKVnn-SsLC2Zhx-r4,1213
-muko-2.25.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-muko-2.25.dist-info/entry_points.txt,sha256=eqGnTHtEVMYwfXVk1Z9MhC8O2N8wuqAbr0lisLmrkxs,20
-muko-2.25.dist-info/top_level.txt,sha256=fp2J4q9iyOPhu1UrXQqzVFSagtatDPDXHXAFWfVJk2M,5
-muko-2.25.dist-info/RECORD,,
+muko-2.26.dist-info/LICENSE,sha256=RwagnXR-4KxFgkvsh5PWaPhlca1CH_BNf-ozi5vp0fw,1074
+muko-2.26.dist-info/METADATA,sha256=lRA7bUm13xEiJ8SbSuYBEeseNk4W39JvBin4GZBeUq8,1213
+muko-2.26.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+muko-2.26.dist-info/entry_points.txt,sha256=eqGnTHtEVMYwfXVk1Z9MhC8O2N8wuqAbr0lisLmrkxs,20
+muko-2.26.dist-info/top_level.txt,sha256=fp2J4q9iyOPhu1UrXQqzVFSagtatDPDXHXAFWfVJk2M,5
+muko-2.26.dist-info/RECORD,,
```

