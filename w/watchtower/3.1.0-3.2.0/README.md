# Comparing `tmp/watchtower-3.1.0.tar.gz` & `tmp/watchtower-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower-3.1.0.tar", last modified: Sun Mar 10 22:26:26 2024, max compression
+gzip compressed data, was "watchtower-3.2.0.tar", last modified: Sat Apr 20 02:46:58 2024, max compression
```

## Comparing `watchtower-3.1.0.tar` & `watchtower-3.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-03-10 22:26:26.179433 watchtower-3.1.0/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    11358 2023-10-23 21:53:48.000000 watchtower-3.1.0/LICENSE
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       30 2023-10-23 21:53:48.000000 watchtower-3.1.0/MANIFEST.in
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    15687 2024-03-10 22:26:26.178875 watchtower-3.1.0/PKG-INFO
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    14339 2023-12-11 06:34:53.000000 watchtower-3.1.0/README.rst
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      224 2023-12-11 06:34:53.000000 watchtower-3.1.0/pyproject.toml
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       38 2024-03-10 22:26:26.179497 watchtower-3.1.0/setup.cfg
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1583 2024-03-10 22:25:47.000000 watchtower-3.1.0/setup.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-03-10 22:26:26.173955 watchtower-3.1.0/test/
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)    12966 2024-03-10 22:13:52.000000 watchtower-3.1.0/test/test.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-03-10 22:26:26.175520 watchtower-3.1.0/watchtower/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    23616 2024-03-10 22:10:37.000000 watchtower-3.1.0/watchtower/__init__.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2023-10-23 21:53:48.000000 watchtower-3.1.0/watchtower/py.typed
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-03-10 22:26:26.178171 watchtower-3.1.0/watchtower.egg-info/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    15687 2024-03-10 22:26:26.000000 watchtower-3.1.0/watchtower.egg-info/PKG-INFO
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      279 2024-03-10 22:26:26.000000 watchtower-3.1.0/watchtower.egg-info/SOURCES.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2024-03-10 22:26:26.000000 watchtower-3.1.0/watchtower.egg-info/dependency_links.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       65 2024-03-10 22:26:26.000000 watchtower-3.1.0/watchtower.egg-info/requires.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       11 2024-03-10 22:26:26.000000 watchtower-3.1.0/watchtower.egg-info/top_level.txt
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-20 02:46:58.533237 watchtower-3.2.0/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    11358 2023-10-23 21:53:48.000000 watchtower-3.2.0/LICENSE
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       30 2023-10-23 21:53:48.000000 watchtower-3.2.0/MANIFEST.in
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    15688 2024-04-20 02:46:58.532481 watchtower-3.2.0/PKG-INFO
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    14339 2023-12-11 06:34:53.000000 watchtower-3.2.0/README.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      224 2023-12-11 06:34:53.000000 watchtower-3.2.0/pyproject.toml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       38 2024-04-20 02:46:58.533494 watchtower-3.2.0/setup.cfg
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1584 2024-04-20 02:46:22.000000 watchtower-3.2.0/setup.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-20 02:46:58.527468 watchtower-3.2.0/test/
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)    12966 2024-03-10 22:13:52.000000 watchtower-3.2.0/test/test.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-20 02:46:58.529103 watchtower-3.2.0/watchtower/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    23987 2024-04-20 02:43:50.000000 watchtower-3.2.0/watchtower/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2023-10-23 21:53:48.000000 watchtower-3.2.0/watchtower/py.typed
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-20 02:46:58.531491 watchtower-3.2.0/watchtower.egg-info/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    15688 2024-04-20 02:46:58.000000 watchtower-3.2.0/watchtower.egg-info/PKG-INFO
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      279 2024-04-20 02:46:58.000000 watchtower-3.2.0/watchtower.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2024-04-20 02:46:58.000000 watchtower-3.2.0/watchtower.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       65 2024-04-20 02:46:58.000000 watchtower-3.2.0/watchtower.egg-info/requires.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       11 2024-04-20 02:46:58.000000 watchtower-3.2.0/watchtower.egg-info/top_level.txt
```

### Comparing `watchtower-3.1.0/LICENSE` & `watchtower-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `watchtower-3.1.0/PKG-INFO` & `watchtower-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: watchtower
-Version: 3.1.0
+Version: 3.2.0
 Summary: Python CloudWatch Logging
 Home-page: https://github.com/kislyuk/watchtower
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Platform: MacOS X
 Platform: Posix
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: boto3<2,>=1.9.253
 Provides-Extra: tests
 Requires-Dist: pyyaml; extra == "tests"
 Requires-Dist: ruff; extra == "tests"
 Requires-Dist: coverage; extra == "tests"
 Requires-Dist: build; extra == "tests"
```

### Comparing `watchtower-3.1.0/README.rst` & `watchtower-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `watchtower-3.1.0/setup.py` & `watchtower-3.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="watchtower",
-    version="3.1.0",
+    version="3.2.0",
     url="https://github.com/kislyuk/watchtower",
     license="Apache Software License",
     author="Andrey Kislyuk",
     author_email="kislyuk@gmail.com",
     description="Python CloudWatch Logging",
     long_description=open("README.rst").read(),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=[
         "boto3 >= 1.9.253, < 2",
     ],
     extras_require={
         "tests": [
             "pyyaml",
             "ruff",
@@ -34,17 +34,17 @@
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

### Comparing `watchtower-3.1.0/test/test.py` & `watchtower-3.2.0/test/test.py`

 * *Files identical despite different names*

### Comparing `watchtower-3.1.0/watchtower/__init__.py` & `watchtower-3.2.0/watchtower/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -191,14 +191,15 @@
         objects into strings using the `datetime.isoformat()` method, and uses `repr()` to represent all other objects.
     :param max_message_size:
         Maximum size (in bytes) of a single message.
     """
 
     END = 1
     FLUSH = 2
+    FLUSH_TIMEOUT = 30
 
     # extra size of meta information with each messages
     EXTRA_MSG_PAYLOAD_SIZE = 26
 
     def __init__(
         self,
         log_group_name: str = __name__,
@@ -475,38 +476,42 @@
                     cur_batch.append(msg)
                     my_queue.task_done()
 
     def flush(self):
         """
         Send any queued messages to CloudWatch. This method does nothing if ``use_queues`` is set to False.
         """
-        # fixme: don't add filter if it's already installed
+        # FIXME: don't add filter if it's already installed
         self.addFilter(_boto_filter)
         if self.shutting_down:
             return
         for q in self.queues.values():
             q.put(self.FLUSH)
         for q in self.queues.values():
-            q.join()
+            with q.all_tasks_done:
+                q.all_tasks_done.wait_for(lambda: q.unfinished_tasks == 0, timeout=self.FLUSH_TIMEOUT)
 
     def close(self):
         """
         Send any queued messages to CloudWatch and prevent further processing of messages.
         This method does nothing if ``use_queues`` is set to False.
         """
-        # fixme: don't add filter if it's already installed
+        # FIXME: don't add filter if it's already installed
         self.addFilter(_boto_filter)
         # Avoid waiting on the queue again when the close called twice.
         # Otherwise the second call, as no thread is running, it will hang
         # forever
         if self.shutting_down:
             return
         self.shutting_down = True
         for q in self.queues.values():
             q.put(self.END)
         for q in self.queues.values():
-            q.join()
+            with q.all_tasks_done:
+                q.all_tasks_done.wait_for(lambda: q.unfinished_tasks == 0, timeout=self.FLUSH_TIMEOUT)
+            if not q.empty():
+                warnings.warn("Timed out while delivering logs", WatchtowerWarning)
         super().close()
 
     def __repr__(self):
         name = self.__class__.__name__
         return f"{name}(log_group_name='{self.log_group_name}', log_stream_name='{self.log_stream_name}')"
```

### Comparing `watchtower-3.1.0/watchtower.egg-info/PKG-INFO` & `watchtower-3.2.0/watchtower.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: watchtower
-Version: 3.1.0
+Version: 3.2.0
 Summary: Python CloudWatch Logging
 Home-page: https://github.com/kislyuk/watchtower
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Platform: MacOS X
 Platform: Posix
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: boto3<2,>=1.9.253
 Provides-Extra: tests
 Requires-Dist: pyyaml; extra == "tests"
 Requires-Dist: ruff; extra == "tests"
 Requires-Dist: coverage; extra == "tests"
 Requires-Dist: build; extra == "tests"
```

