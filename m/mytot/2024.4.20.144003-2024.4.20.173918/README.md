# Comparing `tmp/mytot-2024.4.20.144003-py3-none-any.whl.zip` & `tmp/mytot-2024.4.20.173918-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 27447 bytes, number of entries: 10
+Zip file size: 27678 bytes, number of entries: 10
 -rwxrwxr-x  2.0 unx     1469 b- defN 24-Apr-18 10:00 home/maxx/.local/share/mytot/TASK
 -rw-rw-r--  2.0 unx        0 b- defN 24-Apr-18 09:16 mytot/__init__.py
--rw-rw-r--  2.0 unx     1168 b- defN 24-Apr-20 06:39 mytot/main.py
--rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-18 09:16 mytot-2024.4.20.144003.data/data/LICENSE
--rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-20 06:40 mytot-2024.4.20.144003.dist-info/LICENSE
--rw-rw-r--  2.0 unx      209 b- defN 24-Apr-20 06:40 mytot-2024.4.20.144003.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-20 06:40 mytot-2024.4.20.144003.dist-info/WHEEL
--rw-rw-r--  2.0 unx       62 b- defN 24-Apr-20 06:40 mytot-2024.4.20.144003.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        6 b- defN 24-Apr-20 06:40 mytot-2024.4.20.144003.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      863 b- defN 24-Apr-20 06:40 mytot-2024.4.20.144003.dist-info/RECORD
-10 files, 74167 bytes uncompressed, 25953 bytes compressed:  65.0%
+-rw-rw-r--  2.0 unx     1790 b- defN 24-Apr-20 09:38 mytot/main.py
+-rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-18 09:16 mytot-2024.4.20.173918.data/data/LICENSE
+-rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-20 09:39 mytot-2024.4.20.173918.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      253 b- defN 24-Apr-20 09:39 mytot-2024.4.20.173918.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-20 09:39 mytot-2024.4.20.173918.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       85 b- defN 24-Apr-20 09:39 mytot-2024.4.20.173918.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        6 b- defN 24-Apr-20 09:39 mytot-2024.4.20.173918.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      863 b- defN 24-Apr-20 09:39 mytot-2024.4.20.173918.dist-info/RECORD
+10 files, 74856 bytes uncompressed, 26184 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: mytot/__init__.py
 Comment: 
 
 Filename: mytot/main.py
 Comment: 
 
-Filename: mytot-2024.4.20.144003.data/data/LICENSE
+Filename: mytot-2024.4.20.173918.data/data/LICENSE
 Comment: 
 
-Filename: mytot-2024.4.20.144003.dist-info/LICENSE
+Filename: mytot-2024.4.20.173918.dist-info/LICENSE
 Comment: 
 
-Filename: mytot-2024.4.20.144003.dist-info/METADATA
+Filename: mytot-2024.4.20.173918.dist-info/METADATA
 Comment: 
 
-Filename: mytot-2024.4.20.144003.dist-info/WHEEL
+Filename: mytot-2024.4.20.173918.dist-info/WHEEL
 Comment: 
 
-Filename: mytot-2024.4.20.144003.dist-info/entry_points.txt
+Filename: mytot-2024.4.20.173918.dist-info/entry_points.txt
 Comment: 
 
-Filename: mytot-2024.4.20.144003.dist-info/top_level.txt
+Filename: mytot-2024.4.20.173918.dist-info/top_level.txt
 Comment: 
 
-Filename: mytot-2024.4.20.144003.dist-info/RECORD
+Filename: mytot-2024.4.20.173918.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mytot/main.py

```diff
@@ -1,11 +1,12 @@
 import os
 import datetime
 import sys
 import subprocess
+import psutil
 
 from loguru import logger
 
 
 def mkdir(path):
     if not os.path.exists(path):
         os.makedirs(path)
@@ -35,13 +36,35 @@
         cwd=path,
         stdout=open(log_file, "a"),
         stderr=open(log_file, "a"),
         shell=True,
     )
 
 
+def KILL():
+    if len(sys.argv) < 2:
+        print("usage: KILL [script_file]")
+        return
+    key = sys.argv[1]
+    signal = 9
+    for arg in sys.argv[1:]:
+        if arg[0] == "-":
+            signal = int(arg[1:])
+            continue
+        key = arg
+        break
+    for process in psutil.process_iter(["pid", "name", "cmdline"]):
+        if process.info["cmdline"] is None:
+            continue
+        cmdline = " ".join(list(process.info["cmdline"]))
+        if key in cmdline:
+            pid = process.info["pid"]
+            print("kill -{signal} {pid}")
+            os.kill(pid, signal)
+
+
 def TASK():
     if len(sys.argv) < 2:
         print("usage TASK [script_file]")
         return
     bash_file = os.path.expanduser("~/.local/share/mytot/TASK")
     subprocess.run(["bash", bash_file] + sys.argv[1:], check=False)
```

## Comparing `mytot-2024.4.20.144003.data/data/LICENSE` & `mytot-2024.4.20.173918.data/data/LICENSE`

 * *Files identical despite different names*

## Comparing `mytot-2024.4.20.144003.dist-info/LICENSE` & `mytot-2024.4.20.173918.dist-info/LICENSE`

 * *Files identical despite different names*

