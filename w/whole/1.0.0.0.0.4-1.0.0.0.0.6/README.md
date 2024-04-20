# Comparing `tmp/whole-1.0.0.0.0.4.tar.gz` & `tmp/whole-1.0.0.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whole-1.0.0.0.0.4.tar", last modified: Sat Apr  8 06:23:20 2023, max compression
+gzip compressed data, was "whole-1.0.0.0.0.6.tar", last modified: Sat Apr 20 12:23:47 2024, max compression
```

## Comparing `whole-1.0.0.0.0.4.tar` & `whole-1.0.0.0.0.6.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 06:23:20.275176 whole-1.0.0.0.0.4/
--rw-rw-rw-   0        0        0      146 2023-04-08 06:23:20.275176 whole-1.0.0.0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-08 06:23:20.275176 whole-1.0.0.0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      240 2023-04-08 06:20:44.000000 whole-1.0.0.0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 06:23:20.275176 whole-1.0.0.0.0.4/whole/
--rw-rw-rw-   0        0        0   294247 2023-03-13 12:29:26.000000 whole-1.0.0.0.0.4/whole/PinYin.py
--rw-rw-rw-   0        0        0     4314 2023-03-13 13:40:03.000000 whole-1.0.0.0.0.4/whole/Run.py
--rw-rw-rw-   0        0        0     5130 2023-03-17 12:02:16.000000 whole-1.0.0.0.0.4/whole/Stock.py
--rw-rw-rw-   0        0        0     2494 2023-03-26 10:36:16.000000 whole-1.0.0.0.0.4/whole/TCP_UDP.py
--rw-rw-rw-   0        0        0        0 2023-03-12 13:55:32.000000 whole-1.0.0.0.0.4/whole/__init__.py
--rw-rw-rw-   0        0        0      786 2023-03-14 11:44:52.000000 whole-1.0.0.0.0.4/whole/w.py
-drwxrwxrwx   0        0        0        0 2023-04-08 06:23:20.275176 whole-1.0.0.0.0.4/whole.egg-info/
--rw-rw-rw-   0        0        0      146 2023-04-08 06:23:20.000000 whole-1.0.0.0.0.4/whole.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-04-08 06:23:20.000000 whole-1.0.0.0.0.4/whole.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 06:23:20.000000 whole-1.0.0.0.0.4/whole.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-04-08 06:23:20.000000 whole-1.0.0.0.0.4/whole.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-04-08 06:23:20.000000 whole-1.0.0.0.0.4/whole.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 12:23:47.882775 whole-1.0.0.0.0.6/
+-rw-rw-rw-   0        0        0       58 2024-04-20 12:23:47.882775 whole-1.0.0.0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-20 12:23:47.882775 whole-1.0.0.0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      261 2024-04-20 12:20:48.000000 whole-1.0.0.0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 12:23:47.882775 whole-1.0.0.0.0.6/whole/
+-rw-rw-rw-   0        0        0     4331 2023-04-15 11:29:49.000000 whole-1.0.0.0.0.6/whole/Run.py
+-rw-rw-rw-   0        0        0     2494 2023-04-12 12:25:03.000000 whole-1.0.0.0.0.6/whole/TCP_UDP.py
+-rw-rw-rw-   0        0        0        0 2023-03-12 13:55:32.000000 whole-1.0.0.0.0.6/whole/__init__.py
+-rw-rw-rw-   0        0        0      786 2023-03-14 11:44:52.000000 whole-1.0.0.0.0.6/whole/w.py
+drwxrwxrwx   0        0        0        0 2024-04-20 12:23:47.882775 whole-1.0.0.0.0.6/whole.egg-info/
+-rw-rw-rw-   0        0        0       58 2024-04-20 12:23:47.000000 whole-1.0.0.0.0.6/whole.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2024-04-20 12:23:47.000000 whole-1.0.0.0.0.6/whole.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 12:23:47.000000 whole-1.0.0.0.0.6/whole.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-20 12:23:47.000000 whole-1.0.0.0.0.6/whole.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-04-20 12:23:47.000000 whole-1.0.0.0.0.6/whole.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-20 12:23:47.000000 whole-1.0.0.0.0.6/whole.egg-info/top_level.txt
```

### Comparing `whole-1.0.0.0.0.4/whole/Run.py` & `whole-1.0.0.0.0.6/whole/Run.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 import time
 '''
 from whole.Run import R,Start,Stop,Restart
 
 pid_file = "/var/run/r.pid"
 log_file = "/var/log/r.log"
 
-R("spr","r")
+R(sys.argv[1],"r")#后台运行
 Start(pid_file, log_file):#启动软件
 Stop(pid_file):#停止软件运行
 Restart(pid_file, log_file):#重新启动软件
 '''
-
 def write_pid_file(pid_file, pid):
     import fcntl
     import stat
     try:
         fd = os.open(pid_file, os.O_RDWR | os.O_CREAT, stat.S_IRUSR | stat.S_IWUSR)
     except OSError as e:
         return -1
@@ -140,17 +139,17 @@
 def Restart(pid_file, log_file):#重新启动软件
     Stop(pid_file)
     Start(pid_file, log_file)
 
 def R(t,n):
     pid="/var/run/"+n+".pid"
     log="/var/log/"+n+".log"
-    if t == 's':##启动软件
+    if t == '1':##启动软件
         Start(pid, log)
-    elif t == 'p':#停止软件运行
+    elif t == '2':#停止软件运行
         Stop(pid)
         sys.exit(0)
-    elif t == 'r':#重新启动软件
+    elif t == '3':#重新启动软件
         Restart(pid, log)
     else:
         print("输入错误:"+t)
         sys.exit(0)
```

### Comparing `whole-1.0.0.0.0.4/whole/TCP_UDP.py` & `whole-1.0.0.0.0.6/whole/TCP_UDP.py`

 * *Files identical despite different names*

### Comparing `whole-1.0.0.0.0.4/whole/w.py` & `whole-1.0.0.0.0.6/whole/w.py`

 * *Files identical despite different names*

