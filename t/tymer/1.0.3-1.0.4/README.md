# Comparing `tmp/tymer-1.0.3.tar.gz` & `tmp/tymer-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tymer-1.0.3.tar", last modified: Tue Mar 14 17:11:12 2023, max compression
+gzip compressed data, was "tymer-1.0.4.tar", last modified: Fri Apr 19 19:40:25 2024, max compression
```

## Comparing `tymer-1.0.3.tar` & `tymer-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 17:11:14.000000 tymer-1.0.3/
--rw-rw-rw-   0        0        0      358 2023-03-14 17:10:48.000000 tymer-1.0.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1060 2023-02-17 15:12:04.000000 tymer-1.0.3/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2022-07-06 14:59:00.000000 tymer-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      166 2023-03-14 17:11:14.000000 tymer-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-02-17 15:13:38.000000 tymer-1.0.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-03-14 17:11:14.000000 tymer-1.0.3/Tymer/
--rw-rw-rw-   0        0        0     1159 2023-03-14 17:09:18.000000 tymer-1.0.3/Tymer/__init__.py
--rw-rw-rw-   0        0        0       42 2023-03-14 17:11:14.000000 tymer-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      341 2023-03-14 17:10:58.000000 tymer-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-14 17:11:14.000000 tymer-1.0.3/tymer.egg-info/
--rw-rw-rw-   0        0        0      166 2023-03-14 17:11:12.000000 tymer-1.0.3/tymer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-03-14 17:11:14.000000 tymer-1.0.3/tymer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 17:11:12.000000 tymer-1.0.3/tymer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-03-14 17:11:14.000000 tymer-1.0.3/tymer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 19:40:25.153710 tymer-1.0.4/
+-rw-rw-rw-   0        0        0      554 2024-04-19 19:39:27.000000 tymer-1.0.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1060 2023-02-17 15:12:04.000000 tymer-1.0.4/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2022-07-06 14:59:00.000000 tymer-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      166 2024-04-19 19:40:25.152709 tymer-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-02-17 15:13:38.000000 tymer-1.0.4/README.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 19:40:25.147982 tymer-1.0.4/Tymer/
+-rw-rw-rw-   0        0        0     2062 2024-04-19 19:19:01.000000 tymer-1.0.4/Tymer/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-19 19:40:25.153710 tymer-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      341 2024-04-19 19:38:41.000000 tymer-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 19:40:25.152709 tymer-1.0.4/tymer.egg-info/
+-rw-rw-rw-   0        0        0      166 2024-04-19 19:40:25.000000 tymer-1.0.4/tymer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-04-19 19:40:25.000000 tymer-1.0.4/tymer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 19:40:25.000000 tymer-1.0.4/tymer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-19 19:40:25.000000 tymer-1.0.4/tymer.egg-info/top_level.txt
```

### Comparing `tymer-1.0.3/LICENCE.txt` & `tymer-1.0.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `tymer-1.0.3/Tymer/__init__.py` & `tymer-1.0.4/Tymer/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,62 @@
 import time as t
 
 class Timer:
-    def __init__(self, seconds):
+    def __init__(self, seconds, countdown=False, integer=False):
         self.sec = seconds
         self.start_time = None
         self.run_timer = True
         self.timer = 0
         self.start_timer = True
+        self.countdown = countdown
+        self.integer = integer
     def start(self):
         if self.start_timer:
             self.start_time = t.time()
             self.start_timer = False
         self.current_time = t.time()
         if self.run_timer:
             if self.start_time != None:
-                self.timer = self.current_time - self.start_time
-        if self.timer >= self.sec:
-            self.run_timer = False
-            self.timer = self.sec
+                if not self.countdown:
+                    if not self.integer:
+                        self.timer = self.current_time - self.start_time
+                    else:
+                        self.timer = int(self.current_time - self.start_time)
+                else:    
+                    if not self.integer:
+                        self.timer = self.sec - (self.current_time - self.start_time)
+                    else:
+                        self.timer = int(self.sec - (self.current_time - self.start_time))
+        if not self.countdown:
+            if self.timer >= self.sec:
+                self.run_timer = False
+                self.timer = self.sec
+        else:
+            if self.timer <= 0:
+                self.run_timer = False
+                self.timer = 0
     def stop(self):
         self.run_timer = False
         pass
-    def restart(self,new_time='default'):
+    def restart(self,seconds='default'):
+        self.new_time = seconds
         self.start_time = None
         self.run_timer = True
-        if new_time == 'default':
-            self.sec = new_time
-        else:
-            self.sec = new_time
+        if self.new_time != 'default':
+            self.sec = self.new_time
         self.start_timer = True
         pass
     def time(self):
         return self.timer
         pass
     def __bool__(self):
-        if self.timer != self.sec:
-            return False
+        if not self.countdown:
+            if self.timer != self.sec:
+                return False
+            else:
+                return True
         else:
-            return True
+            if self.timer != 0:
+                return False
+            else:
+                return True
     pass
```

