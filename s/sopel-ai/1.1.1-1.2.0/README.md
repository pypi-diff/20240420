# Comparing `tmp/sopel_ai-1.1.1-py3-none-any.whl.zip` & `tmp/sopel_ai-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11508 bytes, number of entries: 11
+Zip file size: 11510 bytes, number of entries: 11
 -rw-r--r--  2.0 unx     2531 b- defN 24-Mar-08 16:08 sopel_ai/__init__.py
 -rw-r--r--  2.0 unx      867 b- defN 24-Mar-08 16:08 sopel_ai/config.py
 -rw-r--r--  2.0 unx     7240 b- defN 24-Mar-08 16:08 sopel_ai/core.py
 -rw-r--r--  2.0 unx      192 b- defN 24-Mar-08 16:08 sopel_ai/errors.py
 -rw-r--r--  2.0 unx     6800 b- defN 24-Mar-08 16:08 sopel_ai/plugin.py
--rw-r--r--  2.0 unx     1531 b- defN 24-Mar-22 02:53 sopel_ai-1.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6200 b- defN 24-Mar-22 02:53 sopel_ai-1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-22 02:53 sopel_ai-1.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       43 b- defN 24-Mar-22 02:53 sopel_ai-1.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-Mar-22 02:53 sopel_ai-1.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      863 b- defN 24-Mar-22 02:53 sopel_ai-1.1.1.dist-info/RECORD
-11 files, 26368 bytes uncompressed, 10052 bytes compressed:  61.9%
+-rw-r--r--  2.0 unx     1531 b- defN 24-Apr-20 02:16 sopel_ai-1.2.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6200 b- defN 24-Apr-20 02:16 sopel_ai-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-20 02:16 sopel_ai-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       43 b- defN 24-Apr-20 02:16 sopel_ai-1.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-20 02:16 sopel_ai-1.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      863 b- defN 24-Apr-20 02:16 sopel_ai-1.2.0.dist-info/RECORD
+11 files, 26368 bytes uncompressed, 10054 bytes compressed:  61.9%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: sopel_ai/errors.py
 Comment: 
 
 Filename: sopel_ai/plugin.py
 Comment: 
 
-Filename: sopel_ai-1.1.1.dist-info/LICENSE.txt
+Filename: sopel_ai-1.2.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: sopel_ai-1.1.1.dist-info/METADATA
+Filename: sopel_ai-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: sopel_ai-1.1.1.dist-info/WHEEL
+Filename: sopel_ai-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: sopel_ai-1.1.1.dist-info/entry_points.txt
+Filename: sopel_ai-1.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: sopel_ai-1.1.1.dist-info/top_level.txt
+Filename: sopel_ai-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sopel_ai-1.1.1.dist-info/RECORD
+Filename: sopel_ai-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `sopel_ai-1.1.1.dist-info/LICENSE.txt` & `sopel_ai-1.2.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `sopel_ai-1.1.1.dist-info/METADATA` & `sopel_ai-1.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel-ai
-Version: 1.1.1
+Version: 1.2.0
 Summary: Sopel AI - an LLM enhanced chat bot plug-in
 Author-email: The SopelAI team <sopel_ai@cime.net>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/pr3d4t0r/sopel_ai
 Project-URL: Bug Tracker, https://github.com/pr3d4t0r/sopel_ai/issues
 Keywords: ai,bot,irc,llm,plugin,sopel
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: perplexipy
 Requires-Dist: sopel (>=7.1)
 Requires-Dist: tinydb
 
-% sopel_ai(1) Version 1.1.1 chatbot plugin
+% sopel_ai(1) Version 1.2.0 chatbot plugin
 
 Name
 ====
 
 **Sopel AI** - AI query/response plugin
```

## Comparing `sopel_ai-1.1.1.dist-info/RECORD` & `sopel_ai-1.2.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 sopel_ai/__init__.py,sha256=UXSuXZj_p860rLAiewSe5nbKg-qbIEcXq6jkqYmaMnI,2531
 sopel_ai/config.py,sha256=y0vbvfeDjjfLUOvTJ3W56mAGVpJxeizrXJbCaFW4ZXk,867
 sopel_ai/core.py,sha256=r5lnH8lcXenc2Ln3Qha2hoAggWUP5ZyZniZrdl9IIsQ,7240
 sopel_ai/errors.py,sha256=XMVgFk4Rw64Z0UO3ZInp-N6LP0GRG8NFIuXKnhu5rLo,192
 sopel_ai/plugin.py,sha256=51mYp6B_mUtgS6mL-IMhK8Qiz_Rw_qAwmTLdML-qQ2o,6800
-sopel_ai-1.1.1.dist-info/LICENSE.txt,sha256=I8aHapysmbM9F3y-rUfp011GQoosNO5L8pzl7IKgPnE,1531
-sopel_ai-1.1.1.dist-info/METADATA,sha256=9_KZvSmAhclhUN0B1SxFnO03tTxzJcfQrN8cVA1olYQ,6200
-sopel_ai-1.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-sopel_ai-1.1.1.dist-info/entry_points.txt,sha256=7Juxcn6L4j6F83TjkviiTwiyXLM4gZxAAXFQDR2G_m4,43
-sopel_ai-1.1.1.dist-info/top_level.txt,sha256=kpNMzNEGbhCXkyn7oc3uQPmrX1J6qLxn59IcZBpwSYg,9
-sopel_ai-1.1.1.dist-info/RECORD,,
+sopel_ai-1.2.0.dist-info/LICENSE.txt,sha256=I8aHapysmbM9F3y-rUfp011GQoosNO5L8pzl7IKgPnE,1531
+sopel_ai-1.2.0.dist-info/METADATA,sha256=mzBWiQuuRZjTrk9efPFkhOXnvUr7PmAz7lttRYazRtc,6200
+sopel_ai-1.2.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+sopel_ai-1.2.0.dist-info/entry_points.txt,sha256=7Juxcn6L4j6F83TjkviiTwiyXLM4gZxAAXFQDR2G_m4,43
+sopel_ai-1.2.0.dist-info/top_level.txt,sha256=kpNMzNEGbhCXkyn7oc3uQPmrX1J6qLxn59IcZBpwSYg,9
+sopel_ai-1.2.0.dist-info/RECORD,,
```

