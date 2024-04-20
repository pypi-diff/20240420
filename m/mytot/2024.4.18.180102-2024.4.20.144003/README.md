# Comparing `tmp/mytot-2024.4.18.180102-py3-none-any.whl.zip` & `tmp/mytot-2024.4.20.144003-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 27106 bytes, number of entries: 10
+Zip file size: 27447 bytes, number of entries: 10
 -rwxrwxr-x  2.0 unx     1469 b- defN 24-Apr-18 10:00 home/maxx/.local/share/mytot/TASK
 -rw-rw-r--  2.0 unx        0 b- defN 24-Apr-18 09:16 mytot/__init__.py
--rw-rw-r--  2.0 unx      184 b- defN 24-Apr-18 10:00 mytot/main.py
--rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-18 09:16 mytot-2024.4.18.180102.data/data/LICENSE
--rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-18 10:01 mytot-2024.4.18.180102.dist-info/LICENSE
--rw-rw-r--  2.0 unx      209 b- defN 24-Apr-18 10:01 mytot-2024.4.18.180102.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-18 10:01 mytot-2024.4.18.180102.dist-info/WHEEL
--rw-rw-r--  2.0 unx       41 b- defN 24-Apr-18 10:01 mytot-2024.4.18.180102.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        6 b- defN 24-Apr-18 10:01 mytot-2024.4.18.180102.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      862 b- defN 24-Apr-18 10:01 mytot-2024.4.18.180102.dist-info/RECORD
-10 files, 73161 bytes uncompressed, 25612 bytes compressed:  65.0%
+-rw-rw-r--  2.0 unx     1168 b- defN 24-Apr-20 06:39 mytot/main.py
+-rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-18 09:16 mytot-2024.4.20.144003.data/data/LICENSE
+-rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-20 06:40 mytot-2024.4.20.144003.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      209 b- defN 24-Apr-20 06:40 mytot-2024.4.20.144003.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-20 06:40 mytot-2024.4.20.144003.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       62 b- defN 24-Apr-20 06:40 mytot-2024.4.20.144003.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        6 b- defN 24-Apr-20 06:40 mytot-2024.4.20.144003.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      863 b- defN 24-Apr-20 06:40 mytot-2024.4.20.144003.dist-info/RECORD
+10 files, 74167 bytes uncompressed, 25953 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: mytot/__init__.py
 Comment: 
 
 Filename: mytot/main.py
 Comment: 
 
-Filename: mytot-2024.4.18.180102.data/data/LICENSE
+Filename: mytot-2024.4.20.144003.data/data/LICENSE
 Comment: 
 
-Filename: mytot-2024.4.18.180102.dist-info/LICENSE
+Filename: mytot-2024.4.20.144003.dist-info/LICENSE
 Comment: 
 
-Filename: mytot-2024.4.18.180102.dist-info/METADATA
+Filename: mytot-2024.4.20.144003.dist-info/METADATA
 Comment: 
 
-Filename: mytot-2024.4.18.180102.dist-info/WHEEL
+Filename: mytot-2024.4.20.144003.dist-info/WHEEL
 Comment: 
 
-Filename: mytot-2024.4.18.180102.dist-info/entry_points.txt
+Filename: mytot-2024.4.20.144003.dist-info/entry_points.txt
 Comment: 
 
-Filename: mytot-2024.4.18.180102.dist-info/top_level.txt
+Filename: mytot-2024.4.20.144003.dist-info/top_level.txt
 Comment: 
 
-Filename: mytot-2024.4.18.180102.dist-info/RECORD
+Filename: mytot-2024.4.20.144003.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mytot/main.py

```diff
@@ -1,8 +1,47 @@
 import os
+import datetime
 import sys
 import subprocess
 
+from loguru import logger
+
+
+def mkdir(path):
+    if not os.path.exists(path):
+        os.makedirs(path)
+
+
+def RUN():
+    if len(sys.argv) < 2:
+        print("usage RUN [script_file]")
+        return
+    script_file = os.path.abspath(sys.argv[1])
+    path, name = os.path.split(script_file)
+    log_path = os.path.join(path, "log")
+    log_file = os.path.join(path, "log", f"{name}.run")
+    mkdir(log_path)
+    now = datetime.datetime.now()
+    if name.endswith(".py"):
+        cmd = f"nohup python -Wignore {script_file} &"
+    elif name.endswith(".sh"):
+        cmd = f"nohup bash {script_file} &"
+    else:
+        cmd = f"nohup {script_file} &"
+
+    with open(log_file, "a") as f:
+        f.write(f"{now} | start run {name}\n")
+    subprocess.Popen(
+        cmd,
+        cwd=path,
+        stdout=open(log_file, "a"),
+        stderr=open(log_file, "a"),
+        shell=True,
+    )
+
 
 def TASK():
+    if len(sys.argv) < 2:
+        print("usage TASK [script_file]")
+        return
     bash_file = os.path.expanduser("~/.local/share/mytot/TASK")
-    subprocess.run(["bash", bash_file] + sys.argv[1:], check=True)
+    subprocess.run(["bash", bash_file] + sys.argv[1:], check=False)
```

## Comparing `mytot-2024.4.18.180102.data/data/LICENSE` & `mytot-2024.4.20.144003.data/data/LICENSE`

 * *Files identical despite different names*

## Comparing `mytot-2024.4.18.180102.dist-info/LICENSE` & `mytot-2024.4.20.144003.dist-info/LICENSE`

 * *Files identical despite different names*

