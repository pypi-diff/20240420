# Comparing `tmp/cofutils-1.1.3.tar.gz` & `tmp/cofutils-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cofutils-1.1.3.tar", last modified: Tue Mar  5 07:45:47 2024, max compression
+gzip compressed data, was "cofutils-1.1.4.tar", last modified: Sat Apr 20 03:26:24 2024, max compression
```

## Comparing `cofutils-1.1.3.tar` & `cofutils-1.1.4.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 haiqwa    (1008) haiqwa    (1008)        0 2024-03-05 07:45:47.638561 cofutils-1.1.3/
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     6776 2024-03-05 07:45:47.638561 cofutils-1.1.3/PKG-INFO
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     6429 2024-01-19 12:38:30.000000 cofutils-1.1.3/README.md
-drwxr-xr-x   0 haiqwa    (1008) haiqwa    (1008)        0 2024-03-05 07:45:47.514560 cofutils-1.1.3/cofutils/
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)      691 2024-03-05 07:39:42.000000 cofutils-1.1.3/cofutils/__init__.py
--rw-rw-r--   0 haiqwa    (1008) haiqwa    (1008)     7038 2024-01-17 02:50:48.000000 cofutils-1.1.3/cofutils/cofprofiler.py
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     7456 2023-11-25 11:55:29.000000 cofutils-1.1.3/cofutils/cofwriter.py
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)    12322 2023-12-01 06:46:16.000000 cofutils-1.1.3/cofutils/dispatch.py
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)      285 2024-03-05 07:34:40.000000 cofutils-1.1.3/cofutils/package_info.py
-drwxr-xr-x   0 haiqwa    (1008) haiqwa    (1008)        0 2024-03-05 07:45:47.626561 cofutils-1.1.3/cofutils/parse/
--rw-rw-r--   0 haiqwa    (1008) haiqwa    (1008)      657 2023-11-30 06:42:14.000000 cofutils-1.1.3/cofutils/parse/__init__.py
--rw-rw-r--   0 haiqwa    (1008) haiqwa    (1008)      721 2023-11-30 06:42:14.000000 cofutils-1.1.3/cofutils/parse/__main__.py
--rw-rw-r--   0 haiqwa    (1008) haiqwa    (1008)     2191 2023-11-30 06:42:14.000000 cofutils-1.1.3/cofutils/parse/db.py
--rw-rw-r--   0 haiqwa    (1008) haiqwa    (1008)     7151 2023-12-08 07:46:16.000000 cofutils-1.1.3/cofutils/parse/kernel.py
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     7681 2023-12-02 09:09:57.000000 cofutils-1.1.3/cofutils/parse/nsight.py
--rw-rw-r--   0 haiqwa    (1008) haiqwa    (1008)    11211 2023-11-30 06:42:14.000000 cofutils-1.1.3/cofutils/parse/nvvp.py
--rwxrwxr-x   0 haiqwa    (1008) haiqwa    (1008)     7669 2023-12-08 08:20:35.000000 cofutils-1.1.3/cofutils/parse/parse.py
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)      480 2024-03-05 07:38:00.000000 cofutils-1.1.3/cofutils/torch_version.py
-drwxr-xr-x   0 haiqwa    (1008) haiqwa    (1008)        0 2024-03-05 07:45:47.562560 cofutils-1.1.3/cofutils.egg-info/
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     6776 2024-03-05 07:45:47.000000 cofutils-1.1.3/cofutils.egg-info/PKG-INFO
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)      523 2024-03-05 07:45:47.000000 cofutils-1.1.3/cofutils.egg-info/SOURCES.txt
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)        1 2024-03-05 07:45:47.000000 cofutils-1.1.3/cofutils.egg-info/dependency_links.txt
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)       50 2024-03-05 07:45:47.000000 cofutils-1.1.3/cofutils.egg-info/entry_points.txt
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)       35 2024-03-05 07:45:47.000000 cofutils-1.1.3/cofutils.egg-info/requires.txt
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)        9 2024-03-05 07:45:47.000000 cofutils-1.1.3/cofutils.egg-info/top_level.txt
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)       38 2024-03-05 07:45:47.642561 cofutils-1.1.3/setup.cfg
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     1875 2024-03-05 07:40:43.000000 cofutils-1.1.3/setup.py
+drwxr-xr-x   0 haiqwa    (1008) haiqwa    (1008)        0 2024-04-20 03:26:24.202470 cofutils-1.1.4/
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     7889 2024-04-20 03:26:24.198470 cofutils-1.1.4/PKG-INFO
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     7542 2024-04-20 03:26:01.000000 cofutils-1.1.4/README.md
+drwxr-xr-x   0 haiqwa    (1008) haiqwa    (1008)        0 2024-04-20 03:26:24.090469 cofutils-1.1.4/cofutils/
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)      319 2024-04-20 03:26:23.000000 cofutils-1.1.4/cofutils/__init__.py
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     7791 2024-04-20 03:26:01.000000 cofutils-1.1.4/cofutils/cofprofiler.py
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     7456 2023-11-25 11:55:29.000000 cofutils-1.1.4/cofutils/cofwriter.py
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)    16627 2024-04-20 03:26:01.000000 cofutils-1.1.4/cofutils/dispatch.py
+drwxr-xr-x   0 haiqwa    (1008) haiqwa    (1008)        0 2024-04-20 03:26:24.194470 cofutils-1.1.4/cofutils/parse/
+-rw-rw-r--   0 haiqwa    (1008) haiqwa    (1008)      657 2023-11-30 06:42:14.000000 cofutils-1.1.4/cofutils/parse/__init__.py
+-rw-rw-r--   0 haiqwa    (1008) haiqwa    (1008)      721 2023-11-30 06:42:14.000000 cofutils-1.1.4/cofutils/parse/__main__.py
+-rw-rw-r--   0 haiqwa    (1008) haiqwa    (1008)     2191 2023-11-30 06:42:14.000000 cofutils-1.1.4/cofutils/parse/db.py
+-rw-rw-r--   0 haiqwa    (1008) haiqwa    (1008)     7151 2023-12-08 07:46:16.000000 cofutils-1.1.4/cofutils/parse/kernel.py
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     7681 2023-12-02 09:09:57.000000 cofutils-1.1.4/cofutils/parse/nsight.py
+-rw-rw-r--   0 haiqwa    (1008) haiqwa    (1008)    11211 2023-11-30 06:42:14.000000 cofutils-1.1.4/cofutils/parse/nvvp.py
+-rwxrwxr-x   0 haiqwa    (1008) haiqwa    (1008)     7669 2023-12-08 08:20:35.000000 cofutils-1.1.4/cofutils/parse/parse.py
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)      480 2024-03-05 07:38:00.000000 cofutils-1.1.4/cofutils/torch_version.py
+drwxr-xr-x   0 haiqwa    (1008) haiqwa    (1008)        0 2024-04-20 03:26:24.146470 cofutils-1.1.4/cofutils.egg-info/
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     7889 2024-04-20 03:26:23.000000 cofutils-1.1.4/cofutils.egg-info/PKG-INFO
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)      498 2024-04-20 03:26:23.000000 cofutils-1.1.4/cofutils.egg-info/SOURCES.txt
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)        1 2024-04-20 03:26:23.000000 cofutils-1.1.4/cofutils.egg-info/dependency_links.txt
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)       50 2024-04-20 03:26:23.000000 cofutils-1.1.4/cofutils.egg-info/entry_points.txt
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)       35 2024-04-20 03:26:23.000000 cofutils-1.1.4/cofutils.egg-info/requires.txt
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)        9 2024-04-20 03:26:23.000000 cofutils-1.1.4/cofutils.egg-info/top_level.txt
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)       38 2024-04-20 03:26:24.202470 cofutils-1.1.4/setup.cfg
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     2286 2024-04-20 03:26:01.000000 cofutils-1.1.4/setup.py
```

### Comparing `cofutils-1.1.3/PKG-INFO` & `cofutils-1.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cofutils
-Version: 1.1.3
+Version: 1.1.4
 Summary: Experiment toolkits
 Home-page: https://gitee.com/haiqwa/cofutils.git
 Author: whq1516@mail.ustc.edu.cn
 Maintainer: whq1516@mail.ustc.edu.cn
 License: See https://gitee.com/haiqwa/cofutils/blob/main/LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -86,15 +86,15 @@
 * Organize the result into a string and output it into `STDOUT` which is easy to view for users 
 * Directly return the result time table as `Dict` format
 
 Users can also customize their time log writer by setting `writer`. Currently, cof timer supports `csv`, `tb`, `info`, `debug`, `warn`, `error` as writer function.
 
 Note: if you call `.log` to print time, then **the timer will reset automatically** 
 ```python
-from cofutils import coftimer, coflogger, coftb, cofcsv
+from cofutils import coftimer, coflogger
 import time
 import torch
 coftimer.set_writer(writer = "warn,csv,tb", name="loop_sleep")
 test_1 = coftimer('test1')
 test_2 = coftimer('test2')
 test_3 = coftimer('test3', cuda_timer=True)
 
@@ -117,21 +117,21 @@
 with test_3:
     for _ in range(3):
         m1 = m1+m2
         m1.div_(20)
         m2.div_(10)
 time_dict = coftimer.log(normalizer=3, timedict=True)
 coflogger.info(time_dict)
-cofcsv.save()
+coftimer.save()
 ```
 
 ```bash
-[2023-11-21 23:08:33.670]  [Cof INFO]: time (ms) | test1: 1001.15 | test2: 0.00
-[2023-11-21 23:08:36.674]  [Cof WARNING]: time (ms) | test1: 1001.11 | test2: 0.00
-[2023-11-21 23:08:39.678]  [Cof INFO]: {'test1': 0.0, 'test2': 1001.1359850565592}
+[2024-04-19 08:35:38.241]  [Cof WARNING]: time (ms) | test1: 1001.09 | test2: 0.00 | test3: 0.00
+[2024-04-19 08:35:41.247]  [Cof WARNING]: time (ms) | test1: 0.00 | test2: 1001.09 | test3: 0.00
+[2024-04-19 08:35:42.000]  [Cof INFO]: {'test1': 0.0, 'test2': 0.0, 'test3': 10.247509638468424}
 ```
 
 ### Cof Memory Report
 Print GPU memory states by pytorch cuda API. And it supports to dump memory states into tensorboard of csv, except for printing out to the terminal.
 * `MA`: memory current allocated
 * `MM`: max memory allocated
 * `MR`: memory reserved by pytorch
@@ -184,32 +184,53 @@
 ---
 
 ### Cofrun is all you need!
 User can easily launch distributed task by `cofrun`. What users need to do is to provide a template bash file and configuration json file.
 
 You can see the examples in `example/`
 
-```
-usage: cofrun [-h] [--file FILE] [--input INPUT] [--template TEMPLATE] [--output OUTPUT] [--test] [--nsys] [--list] [--range RANGE]
+```bash
+usage: cofrun [-h] [--file FILE] [--input_dir INPUT_DIR] [--template-file TEMPLATE_FILE]
+              [--output_dir OUTPUT_DIR] [--test] [--nsys] [--list] [--range RANGE]
+              [--summary SUMMARY]
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
-  --file FILE, -f FILE  config file path, default is ./config-template.json
-  --input INPUT, -i INPUT
-                        run experiments in batch mode. all config files are placed in input directory
-  --template TEMPLATE, -T TEMPLATE
+  --file FILE, -f FILE  configuration file path
+  --input_dir INPUT_DIR, -i INPUT_DIR
+                        run experiments in batch mode. all config files are placed in input
+                        directory
+  --template-file TEMPLATE_FILE, -T TEMPLATE_FILE
                         provide the path of template .sh file
-  --output OUTPUT, -o OUTPUT
+  --output_dir OUTPUT_DIR, -o OUTPUT_DIR
                         write execution output to specific path
-  --test, -t            use cof run in test mode -> just generate bash script
+  --test, -t            use cofrun in test mode -> just generate bash script
   --nsys, -n            use nsys to profile your cuda programme
   --list, -l            list id of all input files, only available when input dir is provided
   --range RANGE, -r RANGE
-                        support 3 formats: [int | int,int,int... | int-int], and int value must be > 0
+                        support 3 formats: [int | int,int,int... | int-int], and int value must be
+                        > 0; for example, --range 0,1-3,6
+  --summary SUMMARY, -s SUMMARY
+                        provide your directory path which contains output files and cofrun would
+                        give the experiment summary in csv format
 ```
 
 Let's run the example:
 
-```
+```bash
 cofrun -f demo_config.json -T demo_template.sh
 ```
+
+If you use batch mode, there're some tips which maybe helpful for you:
+
+```bash
+Cofrun is ready to execute multiple tasks in batch mode. There're maybe some useful suggestions: 
+    1. install and launch tmux. the following are some necessary related instructions: 
+        * create a new tmux window: tmux new -s cof
+        * detach from the current session: Ctrl+b d
+        * attach to an existing session: tmux attach -t cof
+    2. the process would hang up if distributed task crashes. we strongly recommand you to: 
+        * add "export TORCH_NCCL_ASYNC_ERROR_HANDLING=1, pkill python" to your template script
+        * if process hangs up, you can input "pkill python" command or Ctrl+C to skip the current task
+```
+
 And the execution history of cofrun will be written into `history.cof`
```

### Comparing `cofutils-1.1.3/README.md` & `cofutils-1.1.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 * Organize the result into a string and output it into `STDOUT` which is easy to view for users 
 * Directly return the result time table as `Dict` format
 
 Users can also customize their time log writer by setting `writer`. Currently, cof timer supports `csv`, `tb`, `info`, `debug`, `warn`, `error` as writer function.
 
 Note: if you call `.log` to print time, then **the timer will reset automatically** 
 ```python
-from cofutils import coftimer, coflogger, coftb, cofcsv
+from cofutils import coftimer, coflogger
 import time
 import torch
 coftimer.set_writer(writer = "warn,csv,tb", name="loop_sleep")
 test_1 = coftimer('test1')
 test_2 = coftimer('test2')
 test_3 = coftimer('test3', cuda_timer=True)
 
@@ -105,21 +105,21 @@
 with test_3:
     for _ in range(3):
         m1 = m1+m2
         m1.div_(20)
         m2.div_(10)
 time_dict = coftimer.log(normalizer=3, timedict=True)
 coflogger.info(time_dict)
-cofcsv.save()
+coftimer.save()
 ```
 
 ```bash
-[2023-11-21 23:08:33.670]  [Cof INFO]: time (ms) | test1: 1001.15 | test2: 0.00
-[2023-11-21 23:08:36.674]  [Cof WARNING]: time (ms) | test1: 1001.11 | test2: 0.00
-[2023-11-21 23:08:39.678]  [Cof INFO]: {'test1': 0.0, 'test2': 1001.1359850565592}
+[2024-04-19 08:35:38.241]  [Cof WARNING]: time (ms) | test1: 1001.09 | test2: 0.00 | test3: 0.00
+[2024-04-19 08:35:41.247]  [Cof WARNING]: time (ms) | test1: 0.00 | test2: 1001.09 | test3: 0.00
+[2024-04-19 08:35:42.000]  [Cof INFO]: {'test1': 0.0, 'test2': 0.0, 'test3': 10.247509638468424}
 ```
 
 ### Cof Memory Report
 Print GPU memory states by pytorch cuda API. And it supports to dump memory states into tensorboard of csv, except for printing out to the terminal.
 * `MA`: memory current allocated
 * `MM`: max memory allocated
 * `MR`: memory reserved by pytorch
@@ -172,32 +172,53 @@
 ---
 
 ### Cofrun is all you need!
 User can easily launch distributed task by `cofrun`. What users need to do is to provide a template bash file and configuration json file.
 
 You can see the examples in `example/`
 
-```
-usage: cofrun [-h] [--file FILE] [--input INPUT] [--template TEMPLATE] [--output OUTPUT] [--test] [--nsys] [--list] [--range RANGE]
+```bash
+usage: cofrun [-h] [--file FILE] [--input_dir INPUT_DIR] [--template-file TEMPLATE_FILE]
+              [--output_dir OUTPUT_DIR] [--test] [--nsys] [--list] [--range RANGE]
+              [--summary SUMMARY]
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
-  --file FILE, -f FILE  config file path, default is ./config-template.json
-  --input INPUT, -i INPUT
-                        run experiments in batch mode. all config files are placed in input directory
-  --template TEMPLATE, -T TEMPLATE
+  --file FILE, -f FILE  configuration file path
+  --input_dir INPUT_DIR, -i INPUT_DIR
+                        run experiments in batch mode. all config files are placed in input
+                        directory
+  --template-file TEMPLATE_FILE, -T TEMPLATE_FILE
                         provide the path of template .sh file
-  --output OUTPUT, -o OUTPUT
+  --output_dir OUTPUT_DIR, -o OUTPUT_DIR
                         write execution output to specific path
-  --test, -t            use cof run in test mode -> just generate bash script
+  --test, -t            use cofrun in test mode -> just generate bash script
   --nsys, -n            use nsys to profile your cuda programme
   --list, -l            list id of all input files, only available when input dir is provided
   --range RANGE, -r RANGE
-                        support 3 formats: [int | int,int,int... | int-int], and int value must be > 0
+                        support 3 formats: [int | int,int,int... | int-int], and int value must be
+                        > 0; for example, --range 0,1-3,6
+  --summary SUMMARY, -s SUMMARY
+                        provide your directory path which contains output files and cofrun would
+                        give the experiment summary in csv format
 ```
 
 Let's run the example:
 
-```
+```bash
 cofrun -f demo_config.json -T demo_template.sh
 ```
+
+If you use batch mode, there're some tips which maybe helpful for you:
+
+```bash
+Cofrun is ready to execute multiple tasks in batch mode. There're maybe some useful suggestions: 
+    1. install and launch tmux. the following are some necessary related instructions: 
+        * create a new tmux window: tmux new -s cof
+        * detach from the current session: Ctrl+b d
+        * attach to an existing session: tmux attach -t cof
+    2. the process would hang up if distributed task crashes. we strongly recommand you to: 
+        * add "export TORCH_NCCL_ASYNC_ERROR_HANDLING=1, pkill python" to your template script
+        * if process hangs up, you can input "pkill python" command or Ctrl+C to skip the current task
+```
+
 And the execution history of cofrun will be written into `history.cof`
```

### Comparing `cofutils-1.1.3/cofutils/cofprofiler.py` & `cofutils-1.1.4/cofutils/cofprofiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,26 +92,59 @@
         if reset:
             self.reset()
         # If timing was in progress, set it back.
         if started_:
             self.start()
         return elapsed_
     
+class _DummyTimer:
+    """Timer."""
+
+    def __init__(self, name, cuda_timer=False):
+        pass
+
+    def __enter__(self):
+        pass
+    def __exit__(self, exc_type, exc_value, traceback):
+        pass
+
+    def start(self):
+        """Start the timer."""
+        pass
+
+    def stop(self):
+        """Stop the timer."""
+        pass
+
+    def reset(self):
+        """Reset timer."""
+        pass
+
+    def elapsed(self, reset=True):
+        """Calculate the elapsed time."""
+        return 0.0
+    
 class Coftimer(BaseProfiler):
     """Group of timers."""
 
     def __init__(self):
         super(Coftimer, self).__init__()
         self.timers = {}
 
     def __call__(self, name, cuda_timer=False):
+        if self.writers is None:
+            return _DummyTimer(name, cuda_timer)
         if name not in self.timers:
             self.timers[name] = _Timer(name, cuda_timer)
         return self.timers[name]
-    
+    def save(self, root_dir='.', reset=True):
+        for writer in self.writers:
+            if writer=='csv':
+                cofcsv.save(root_dir,reset)
+        return None
     def log(self, normalizer=1.0, timedict=False):
         """Log a group of timers."""
         assert normalizer > 0.0
 
         string = 'time (ms)'
         reset=True
         names = self.timers.keys()
```

### Comparing `cofutils-1.1.3/cofutils/cofwriter.py` & `cofutils-1.1.4/cofutils/cofwriter.py`

 * *Files identical despite different names*

### Comparing `cofutils-1.1.3/cofutils/dispatch.py` & `cofutils-1.1.4/cofutils/dispatch.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,97 +4,95 @@
 import subprocess
 import datetime
 import time
 import torch
 import re
 import copy
 import shutil
-
+from tabulate import tabulate
+from collections import defaultdict
+from .cofwriter import cofcsv
 GLOBAL_ARGS = None
 
-def parse_str_range(str_range:str):
-    str_range_list = str_range.split(',')
-    print(str_range_list)
-    int_range = []
-    for each in str_range_list:
-        integers = re.findall(r'\d+', each)
-        if '-' in each:
-            start = int(integers[0])
-            end = int(integers[1])+1
-            int_range += list(range(start, end))
-        else:
-            int_range.append(int(integers[0]))
-    return int_range
+device_name_map={
+    'NVIDIA GeForce GTX 1080 Ti': '1080Ti',
+    'NVIDIA A40': '40A',
+    'NVIDIA GeForce RTX 3090': '3090RTX'
+}
 
+def notion():
+    print("Cofrun is ready to execute multiple tasks in batch mode. \
+There're maybe some useful suggestions: \n\
+    1. install and launch tmux. the following are some necessary related instructions: \n\
+        * create a new tmux window: tmux new -s cof\n\
+        * detach from the current session: Ctrl+b d\n\
+        * attach to an existing session: tmux attach -t cof\n\
+    2. the process would hang up if distributed task crashes. we strongly recommand you to: \n\
+        * add \"export TORCH_NCCL_ASYNC_ERROR_HANDLING=1, pkill python\" to your template script\n\
+        * if process hangs up, you can input \"pkill python\" command or Ctrl+C to skip the current task\n")
+    
 def logging(msg):
     current_time = datetime.datetime.now()
     formatted_time = current_time.strftime("%Y-%m-%d %H:%M:%S")
     print(f"[{formatted_time}] {msg}")
-    with open("history.cof", "a+") as file:
+    if not os.path.exists("cof_workspace/"):
+        os.mkdir("cof_workspace/")
+    with open("cof_workspace/history.cof", "a+") as file:
         file.write(f"[{formatted_time}] {msg}\n")
 
-device_name_map={
-    'NVIDIA GeForce GTX 1080 Ti': '1080Ti',
-    'NVIDIA A40': '40A',
-    'NVIDIA GeForce RTX 3090': '3090RTX'
-}
-
 def auto_exec():
     if GLOBAL_ARGS.test:
         print("cofrun test done")
         logging(f"{GLOBAL_ARGS.config_file} test done")
         return
-    
-    print("executing tasks. we strongly recommend to leverage tmux: \n\
-                                                tmux new -s cof\n\
-                                                tmux attach -t cof\n\
-                                                Ctrl+b d\n\
-          if process hangs up during batch mode, you can input \"pkill python\" to skip the current task\n")
-    if GLOBAL_ARGS.output is not None:
+    if GLOBAL_ARGS.output_dir is not None:
         # check if output directory exists or not
-        if not os.path.exists(GLOBAL_ARGS.output):
-            os.mkdir(GLOBAL_ARGS.output)
+        if not os.path.exists(GLOBAL_ARGS.output_dir):
+            os.mkdir(GLOBAL_ARGS.output_dir)
         now = datetime.datetime.now()
         gpu_name = torch.cuda.get_device_properties(torch.device("cuda")).name
         def extract_gpu_info(name):
             if name in device_name_map.keys():
                 return device_name_map[name]
             else:
-                return ''
+                return 'GPU'
         formatted_time = now.strftime("%m%d%H%M%S")
         # mkdir
-        log_dir = os.path.join(GLOBAL_ARGS.output, extract_gpu_info(gpu_name)+formatted_time)
+        log_dir = os.path.join(GLOBAL_ARGS.output_dir, extract_gpu_info(gpu_name)+formatted_time)
         os.mkdir(log_dir)
         # write config file
         with open(GLOBAL_ARGS.config_file) as fp:
             config_list = json.load(fp)
         
         # save config json file
         with open(f'{log_dir}/config.json', "w") as fp:
             json.dump(config_list,fp=fp, indent=4, separators=(',', ': '))
         # save template bash script
-        shutil.copy(GLOBAL_ARGS.template, f'{log_dir}/run.sh')
+        shutil.copy(GLOBAL_ARGS.template_file, f'{log_dir}/run.sh')
         # launch task
         print("launch task and current time: ", extract_gpu_info(gpu_name)+formatted_time)
         with open(f'{log_dir}/log', 'w') as fp:
             try: 
                 result = subprocess.run(['bash', 'cof_workspace/launch-all.sh'], stdout=fp, stderr=subprocess.STDOUT, text=True)
                 logging(f"process return code: {result.returncode}")
             except KeyboardInterrupt:
                 logging(f"process killed by users")
+        GLOBAL_ARGS.log_file_list.append(f'{log_dir}/log')
+
         nsys_file = 'target.nsys-rep'
         sqlite_file = 'target.sqlite'
         if os.path.exists(f'/tmp/{nsys_file}'):
             shutil.move(f'/tmp/{nsys_file}', f'{log_dir}/{nsys_file}')
         else:
             logging(f'/tmp/{nsys_file} not exist!')
         if os.path.exists(f'/tmp/{sqlite_file}'):
             shutil.move(f'/tmp/{sqlite_file}', f'{log_dir}/{sqlite_file}')
         else:
             logging(f'/tmp/{sqlite_file} not exist!')
+        logging(f"saving to {log_dir} ...")
     else:
         subprocess.run(['bash','cof_workspace/launch-all.sh'])
 
 def auto_gen():
     host_file_name="cof_workspace/hostfile"
     launch_file_name="cof_workspace/launch-all.sh"
     script_file_name=f'cof_workspace/target.sh'
@@ -118,30 +116,25 @@
         modified_lines = [compile(line, config_table) if line.startswith('%') else line for line in lines]
         modified_lines = [ '_'.join(line.strip('\n').split('&'))+f"={ipx}\n"if line.startswith('&') else line for line in modified_lines]
         return ''.join(modified_lines)
 
     with open(GLOBAL_ARGS.config_file) as f:
         config_list = json.load(f)
     config_table = {k:v for each in config_list for k,v in each.items()}
+    logging("\n"+tabulate([[k,v] for k,v in config_table.items()], headers=["Configuration Key", "Value"], tablefmt="rounded_outline"))
     cluster_ip_list = [each for each in config_table["CLUSTER_IPS"].split(" ") if each]
     
     ##########################################
     # generate launch-all.sh!
     ##########################################
     NNODES = config_table['NNODES']
     
     current_dir = os.getcwd()
     nsys_cmd = 'pkill nsys; nsys start --stop-on-exit=false --stats=true -c cudaProfilerApi -f true -o /tmp/target ;nsys launch --wait=primary --trace=cuda,nvtx '
-    launch_all_content = f'mpirun -np {NNODES} \\\n\
-    --hostfile {current_dir}/cof_workspace/hostfile  \\\n\
-    -bind-to none -map-by slot \\\n\
-    --allow-run-as-root \\\n\
-    -x LD_LIBRARY_PATH -x PATH \\\n\
-    pkill python \n\
-{nsys_cmd if GLOBAL_ARGS.nsys else ""}mpirun -np {NNODES} \\\n\
+    launch_all_content = f'{nsys_cmd if GLOBAL_ARGS.nsys else ""}mpirun -np {NNODES} \\\n\
     --hostfile {current_dir}/cof_workspace/hostfile  \\\n\
     -bind-to none -map-by slot \\\n\
     --allow-run-as-root \\\n\
     -x LD_LIBRARY_PATH -x PATH \\\n\
     bash /tmp/target.sh \n\
 second_return_code=$?\n\
 if [ $second_return_code -ne 0 ]; then \n\
@@ -150,15 +143,15 @@
 exit 0'
     if not os.path.exists("cof_workspace/"):
         os.mkdir("cof_workspace/")
 
     with open(launch_file_name,"w") as fp:
         fp.write(launch_all_content)
     for host_idx,host_ip in enumerate(cluster_ip_list[:NNODES]):
-        script_content = autogen_from_template(config_table, GLOBAL_ARGS.template, host_idx)
+        script_content = autogen_from_template(config_table, GLOBAL_ARGS.template_file, host_idx)
         with open(script_file_name,'w') as f:
             f.write(script_content)
         dispatch_cmd=f'scp {script_file_name} {host_ip}:/tmp/'
         return_code=os.system(dispatch_cmd)
         return_code="successfully" if return_code==0 else "failed"
         print(f"{dispatch_cmd}------------{return_code}")
     if return_code!="successfully":
@@ -176,53 +169,72 @@
             fp.write(each_ip + " slots=1\n")
     return 0
 
 def process_file():
     assert auto_gen()==0
     start = time.time()
     auto_exec()
-    print(f"{GLOBAL_ARGS.config_file} done execution time: {time.time()-start:.2f}s")
-    logging(f"{GLOBAL_ARGS.config_file} done execution time: {time.time()-start:.2f}s")
+    end = time.time()
+    GLOBAL_ARGS.total_time+=end-start
+    print(f"{GLOBAL_ARGS.config_file} done execution time: {end-start:.2f}s")
+    logging(f"{GLOBAL_ARGS.config_file} done execution time: {end-start:.2f}s")
 
 def process_batched_files():
     global GLOBAL_ARGS
-    assert os.path.exists(GLOBAL_ARGS.input), GLOBAL_ARGS.input+" not exist"
+    assert os.path.exists(GLOBAL_ARGS.input_dir), GLOBAL_ARGS.input_dir+" not exist"
     config_file_list = []
-    for _, _, files in os.walk(GLOBAL_ARGS.input):
+    for _, _, files in os.walk(GLOBAL_ARGS.input_dir):
         for file in files:
-            config_file_list.append(os.path.join(GLOBAL_ARGS.input, file))
+            config_file_list.append(os.path.join(GLOBAL_ARGS.input_dir, file))
     config_file_list.sort()
-
     if GLOBAL_ARGS.list:
         print("="*25)
         print("     Print Log List")
         print("="*25)
 
         print(f"log num: {len(config_file_list)}")
         print("id         name")
         for id, dir in enumerate(config_file_list):
             print(f"{id}    {dir}")
 
         print("-"*25)
         logging("list input files done")
+        GLOBAL_ARGS.config_file_list=[]
+        GLOBAL_ARGS.log_file_list=[]
     else:
-        
+        notion()
+        def parse_str_range(str_range:str):
+            str_range_list = str_range.split(',')
+            print(str_range_list)
+            int_range = []
+            for each in str_range_list:
+                integers = re.findall(r'\d+', each)
+                if '-' in each:
+                    start = int(integers[0])
+                    end = int(integers[1])+1
+                    int_range += list(range(start, end))
+                else:
+                    int_range.append(int(integers[0]))
+            return int_range
         candidate_config_file_list = [config_file_list[each] for each in parse_str_range(GLOBAL_ARGS.range)] if GLOBAL_ARGS.range is not None else config_file_list
-        for id, config_file in enumerate(candidate_config_file_list):
-            print(f"{id+1}/{len(candidate_config_file_list)} executing: {config_file}")
-            logging(f"{id+1}/{len(candidate_config_file_list)} executing: {config_file}")
+        GLOBAL_ARGS.config_file_list=candidate_config_file_list
+        GLOBAL_ARGS.log_file_list=[]
+        GLOBAL_ARGS.total_time=0
+        for idx, config_file in enumerate(candidate_config_file_list):
+            logging(f"{idx+1}/{len(candidate_config_file_list)} executing: {config_file}")
             GLOBAL_ARGS.config_file = config_file
             process_file()
+            logging(f"estimated remaining time: {GLOBAL_ARGS.total_time/(idx+1)*(len(candidate_config_file_list)-idx-1)}s")
 
 def task_setup():
     global GLOBAL_ARGS
     logging(f"task setup ...")
-    if GLOBAL_ARGS.input is not None:
+    if GLOBAL_ARGS.input_dir is not None:
         process_batched_files()
-    else:
+    elif GLOBAL_ARGS.file and GLOBAL_ARGS.template_file:
         def check_inner_list(config_file):
             json_gen_dir = 'cof-gen/'
             with open(config_file) as f:
                 config_list = json.load(f)
 
             def find_lists_and_generate_combinations(config_list, setting_lists):
                 # setting_lists = []
@@ -255,48 +267,103 @@
                     config_copy = copy.deepcopy(config_list)
                     _, _ = find_lists_and_generate_combinations(config_copy, setting_lists[idx])
                     with open(f'{json_gen_dir}/config-{str(idx).zfill(len(str(setting_num)))}'+".json", "w") as fp:
                         json.dump(config_copy, fp=fp, indent=4, separators=(',', ': '))
             return bool(setting_lists)
 
         if check_inner_list(GLOBAL_ARGS.file):
-            GLOBAL_ARGS.input = 'cof-gen/'
+            GLOBAL_ARGS.input_dir = 'cof-gen/'
             process_batched_files()
         else:
             GLOBAL_ARGS.config_file = GLOBAL_ARGS.file
             process_file()
 
+def summary():
+    global GLOBAL_ARGS
+    if not (hasattr(GLOBAL_ARGS, 'config_file_list') and hasattr(GLOBAL_ARGS, 'log_file_list')):
+        sub_dir_list = sorted([each for each in os.listdir(GLOBAL_ARGS.summary) if os.path.isdir(os.path.join(GLOBAL_ARGS.summary,each))])
+        GLOBAL_ARGS.config_file_list = [os.path.join(GLOBAL_ARGS.summary, sub_dir, 'config.json') for sub_dir in sub_dir_list]
+        GLOBAL_ARGS.log_file_list = [os.path.join(GLOBAL_ARGS.summary, sub_dir, 'log') for sub_dir in sub_dir_list]
+    logging(f"tasks summary: cofrun executes {len(GLOBAL_ARGS.config_file_list)} tasks and generate {len(GLOBAL_ARGS.log_file_list)} logs at all")
+    if len(GLOBAL_ARGS.config_file_list)!=len(GLOBAL_ARGS.log_file_list) or len(GLOBAL_ARGS.log_file_list)==0:
+        print("some tasks did not generate log files properly, skipping summary!")
+        return
+    
+    def process_log_files(file_paths):
+        throughput_value_list=[]
+        for file in file_paths:
+            with open(file, 'r') as fp:
+                log_data = fp.read()
+            pattern = r' iteration        \d+/       \d+ \| .*throughput per GPU \(TFLOP/s/GPU\): (\d+\.\d+|\d+) \|.*'
+            matches = re.findall(pattern, log_data)
+            # print(matches)
+            throughput_value_list.append(0)
+            if matches:
+                throughput_value_list[-1]=float(matches[-1])
+        return throughput_value_list
+    
+    def process_json_files(file_paths):
+        json_file_table = defaultdict(list)
+        same_value = dict()
+        diff_value = dict()
+        for file_path in file_paths:
+            with open(file_path, 'r') as f:
+                data = json.load(f)
+                data = {k:v for each in data for k,v in each.items()}
+            # key_list = data.keys()
+            for k,v in data.items():
+                json_file_table[k].append(v) 
+        for k,v in json_file_table.items():
+            if len(set(v))==1:
+                same_value[k]=v[0]
+            else:
+                diff_value[k]=v
+        return same_value, diff_value
+    same_value, diff_value = process_json_files(GLOBAL_ARGS.config_file_list)
+    diff_value['throughput per GPU (TFLOP/s/GPU)']=process_log_files(GLOBAL_ARGS.log_file_list)
+    diff_value['configuration file']=GLOBAL_ARGS.config_file_list
+    
+    logging("same parameter:\n"+tabulate([[k,v] for k,v in same_value.items()], headers=["Same Argument", "Value"], tablefmt="rounded_outline"))
+    logging("different parameter and result:\n"+tabulate([[value[idx] for value in diff_value.values()] for idx in range(len(GLOBAL_ARGS.config_file_list))], headers=diff_value.keys(), tablefmt="rounded_outline"))
+    
+    csv_table = cofcsv('summary')
+    for idx in range(len(GLOBAL_ARGS.config_file_list)):
+        csv_table.write({k:v[idx] for k,v in diff_value.items()})
+    cofcsv.save(root_dir=GLOBAL_ARGS.summary)
+    
 def main():
     global GLOBAL_ARGS
     parser = argparse.ArgumentParser()
-    parser.add_argument('--file','-f', type=str, default="config-template.json", help="config file path, default is ./config-template.json")
-    parser.add_argument('--input', '-i', type=str, default=None, help="run experiments in batch mode. all config files are placed in input directory")
-    parser.add_argument('--template','-T', type=str, default=None, help='provide the path of template .sh file')
-    parser.add_argument('--output','-o', type=str, default=None,
+    parser.add_argument('--file','-f', type=str, default=None, help="configuration file path")
+    parser.add_argument('--input_dir', '-i', type=str, default=None, help="run experiments in batch mode. all config files are placed in input directory")
+    parser.add_argument('--template-file','-T', type=str, default=None, help='provide the path of template .sh file')
+    parser.add_argument('--output_dir','-o', type=str, default=None,
                        help='write execution output to specific path')
     parser.add_argument('--test','-t', action='store_true',
-                        help='use cof run in test mode -> just generate bash script')
+                        help='use cofrun in test mode -> just generate bash script')
     parser.add_argument('--nsys','-n', action='store_true',
                         help='use nsys to profile your cuda programme')
     parser.add_argument('--list','-l', action='store_true',
                         help='list id of all input files, only available when input dir is provided')
     parser.add_argument('--range','-r', type=str, default=None,
-                        help='support 3 formats: [int | int,int,int... | int-int], and int value must be > 0')
+                        help='support 3 formats: [int | int,int,int... | int-int], and int value must be > 0; for example, --range 0,1-3,6')
+    parser.add_argument('--summary','-s', type=str, default=None,
+                        help='provide your directory path which contains output files and cofrun would give the experiment summary in csv format')
     GLOBAL_ARGS = parser.parse_args()
-    
-    logging("-"*10+"cofrun begin"+"-"*10)
-    args_str = "\n"
 
-    # find the longest var name
-    max_arg_length = max(len(arg) for arg in vars(GLOBAL_ARGS))
+    logging("\n\n\n"+"-"*20+"cofrun begin"+"-"*20)
 
+    args_str = "cofrun arguments\n"
     # alignment
+    argument_table_data = list()
     for arg in vars(GLOBAL_ARGS):
-        args_str += f"{arg.ljust(max_arg_length)}: {getattr(GLOBAL_ARGS, arg)}\n"
-    logging(args_str)
-
-
-    task_setup()
+        argument_table_data.append([arg, getattr(GLOBAL_ARGS, arg)])
+    table = tabulate(argument_table_data, headers=["Cofrun Argument", "Value"], tablefmt="rounded_outline")
+    logging(args_str+table)
+    if GLOBAL_ARGS.summary is None:
+        GLOBAL_ARGS.summary = GLOBAL_ARGS.output_dir
+        task_setup()
+    summary()
     logging("="*10 + "All submitted cofrun tasks done" + "="*10)
 
 if __name__ == "__main__":
     main()
```

### Comparing `cofutils-1.1.3/cofutils/parse/__init__.py` & `cofutils-1.1.4/cofutils/parse/__init__.py`

 * *Files identical despite different names*

### Comparing `cofutils-1.1.3/cofutils/parse/__main__.py` & `cofutils-1.1.4/cofutils/parse/__main__.py`

 * *Files identical despite different names*

### Comparing `cofutils-1.1.3/cofutils/parse/db.py` & `cofutils-1.1.4/cofutils/parse/db.py`

 * *Files identical despite different names*

### Comparing `cofutils-1.1.3/cofutils/parse/kernel.py` & `cofutils-1.1.4/cofutils/parse/kernel.py`

 * *Files identical despite different names*

### Comparing `cofutils-1.1.3/cofutils/parse/nsight.py` & `cofutils-1.1.4/cofutils/parse/nsight.py`

 * *Files identical despite different names*

### Comparing `cofutils-1.1.3/cofutils/parse/nvvp.py` & `cofutils-1.1.4/cofutils/parse/nvvp.py`

 * *Files identical despite different names*

### Comparing `cofutils-1.1.3/cofutils/parse/parse.py` & `cofutils-1.1.4/cofutils/parse/parse.py`

 * *Files identical despite different names*

### Comparing `cofutils-1.1.3/cofutils.egg-info/PKG-INFO` & `cofutils-1.1.4/cofutils.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cofutils
-Version: 1.1.3
+Version: 1.1.4
 Summary: Experiment toolkits
 Home-page: https://gitee.com/haiqwa/cofutils.git
 Author: whq1516@mail.ustc.edu.cn
 Maintainer: whq1516@mail.ustc.edu.cn
 License: See https://gitee.com/haiqwa/cofutils/blob/main/LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -86,15 +86,15 @@
 * Organize the result into a string and output it into `STDOUT` which is easy to view for users 
 * Directly return the result time table as `Dict` format
 
 Users can also customize their time log writer by setting `writer`. Currently, cof timer supports `csv`, `tb`, `info`, `debug`, `warn`, `error` as writer function.
 
 Note: if you call `.log` to print time, then **the timer will reset automatically** 
 ```python
-from cofutils import coftimer, coflogger, coftb, cofcsv
+from cofutils import coftimer, coflogger
 import time
 import torch
 coftimer.set_writer(writer = "warn,csv,tb", name="loop_sleep")
 test_1 = coftimer('test1')
 test_2 = coftimer('test2')
 test_3 = coftimer('test3', cuda_timer=True)
 
@@ -117,21 +117,21 @@
 with test_3:
     for _ in range(3):
         m1 = m1+m2
         m1.div_(20)
         m2.div_(10)
 time_dict = coftimer.log(normalizer=3, timedict=True)
 coflogger.info(time_dict)
-cofcsv.save()
+coftimer.save()
 ```
 
 ```bash
-[2023-11-21 23:08:33.670]  [Cof INFO]: time (ms) | test1: 1001.15 | test2: 0.00
-[2023-11-21 23:08:36.674]  [Cof WARNING]: time (ms) | test1: 1001.11 | test2: 0.00
-[2023-11-21 23:08:39.678]  [Cof INFO]: {'test1': 0.0, 'test2': 1001.1359850565592}
+[2024-04-19 08:35:38.241]  [Cof WARNING]: time (ms) | test1: 1001.09 | test2: 0.00 | test3: 0.00
+[2024-04-19 08:35:41.247]  [Cof WARNING]: time (ms) | test1: 0.00 | test2: 1001.09 | test3: 0.00
+[2024-04-19 08:35:42.000]  [Cof INFO]: {'test1': 0.0, 'test2': 0.0, 'test3': 10.247509638468424}
 ```
 
 ### Cof Memory Report
 Print GPU memory states by pytorch cuda API. And it supports to dump memory states into tensorboard of csv, except for printing out to the terminal.
 * `MA`: memory current allocated
 * `MM`: max memory allocated
 * `MR`: memory reserved by pytorch
@@ -184,32 +184,53 @@
 ---
 
 ### Cofrun is all you need!
 User can easily launch distributed task by `cofrun`. What users need to do is to provide a template bash file and configuration json file.
 
 You can see the examples in `example/`
 
-```
-usage: cofrun [-h] [--file FILE] [--input INPUT] [--template TEMPLATE] [--output OUTPUT] [--test] [--nsys] [--list] [--range RANGE]
+```bash
+usage: cofrun [-h] [--file FILE] [--input_dir INPUT_DIR] [--template-file TEMPLATE_FILE]
+              [--output_dir OUTPUT_DIR] [--test] [--nsys] [--list] [--range RANGE]
+              [--summary SUMMARY]
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
-  --file FILE, -f FILE  config file path, default is ./config-template.json
-  --input INPUT, -i INPUT
-                        run experiments in batch mode. all config files are placed in input directory
-  --template TEMPLATE, -T TEMPLATE
+  --file FILE, -f FILE  configuration file path
+  --input_dir INPUT_DIR, -i INPUT_DIR
+                        run experiments in batch mode. all config files are placed in input
+                        directory
+  --template-file TEMPLATE_FILE, -T TEMPLATE_FILE
                         provide the path of template .sh file
-  --output OUTPUT, -o OUTPUT
+  --output_dir OUTPUT_DIR, -o OUTPUT_DIR
                         write execution output to specific path
-  --test, -t            use cof run in test mode -> just generate bash script
+  --test, -t            use cofrun in test mode -> just generate bash script
   --nsys, -n            use nsys to profile your cuda programme
   --list, -l            list id of all input files, only available when input dir is provided
   --range RANGE, -r RANGE
-                        support 3 formats: [int | int,int,int... | int-int], and int value must be > 0
+                        support 3 formats: [int | int,int,int... | int-int], and int value must be
+                        > 0; for example, --range 0,1-3,6
+  --summary SUMMARY, -s SUMMARY
+                        provide your directory path which contains output files and cofrun would
+                        give the experiment summary in csv format
 ```
 
 Let's run the example:
 
-```
+```bash
 cofrun -f demo_config.json -T demo_template.sh
 ```
+
+If you use batch mode, there're some tips which maybe helpful for you:
+
+```bash
+Cofrun is ready to execute multiple tasks in batch mode. There're maybe some useful suggestions: 
+    1. install and launch tmux. the following are some necessary related instructions: 
+        * create a new tmux window: tmux new -s cof
+        * detach from the current session: Ctrl+b d
+        * attach to an existing session: tmux attach -t cof
+    2. the process would hang up if distributed task crashes. we strongly recommand you to: 
+        * add "export TORCH_NCCL_ASYNC_ERROR_HANDLING=1, pkill python" to your template script
+        * if process hangs up, you can input "pkill python" command or Ctrl+C to skip the current task
+```
+
 And the execution history of cofrun will be written into `history.cof`
```

