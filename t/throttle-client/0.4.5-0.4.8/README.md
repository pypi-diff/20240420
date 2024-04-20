# Comparing `tmp/throttle_client-0.4.5.tar.gz` & `tmp/throttle_client-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "throttle_client-0.4.5.tar", last modified: Fri Dec  8 17:30:35 2023, max compression
+gzip compressed data, was "throttle_client-0.4.8.tar", last modified: Sat Apr 20 20:53:03 2024, max compression
```

## Comparing `throttle_client-0.4.5.tar` & `throttle_client-0.4.8.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 17:30:35.195851 throttle_client-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-12-08 17:30:26.000000 throttle_client-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9993 2023-12-08 17:30:35.195851 throttle_client-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 17:30:35.195851 throttle_client-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      743 2023-12-08 17:30:26.000000 throttle_client-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 17:30:35.191851 throttle_client-0.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2023-12-08 17:30:26.000000 throttle_client-0.4.5/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2023-12-08 17:30:26.000000 throttle_client-0.4.5/tests/test_peer.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-12-08 17:30:26.000000 throttle_client-0.4.5/tests/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)    10386 2023-12-08 17:30:26.000000 throttle_client-0.4.5/tests/test_server_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 17:30:35.191851 throttle_client-0.4.5/throttle_client/
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2023-12-08 17:30:26.000000 throttle_client-0.4.5/throttle_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2023-12-08 17:30:26.000000 throttle_client-0.4.5/throttle_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2023-12-08 17:30:26.000000 throttle_client-0.4.5/throttle_client/peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2023-12-08 17:30:26.000000 throttle_client-0.4.5/throttle_client/status_code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 17:30:35.195851 throttle_client-0.4.5/throttle_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9993 2023-12-08 17:30:35.000000 throttle_client-0.4.5/throttle_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-12-08 17:30:35.000000 throttle_client-0.4.5/throttle_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 17:30:35.000000 throttle_client-0.4.5/throttle_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-08 17:30:35.000000 throttle_client-0.4.5/throttle_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-08 17:30:35.000000 throttle_client-0.4.5/throttle_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:53:03.669805 throttle_client-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-20 20:52:59.000000 throttle_client-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10089 2024-04-20 20:53:03.665805 throttle_client-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9466 2024-04-20 20:52:59.000000 throttle_client-0.4.8/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-20 20:52:59.000000 throttle_client-0.4.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:53:03.661805 throttle_client-0.4.8/python_client/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:53:03.665805 throttle_client-0.4.8/python_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-20 20:52:59.000000 throttle_client-0.4.8/python_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-04-20 20:52:59.000000 throttle_client-0.4.8/python_client/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-20 20:52:59.000000 throttle_client-0.4.8/python_client/tests/test_peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-20 20:52:59.000000 throttle_client-0.4.8/python_client/tests/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10386 2024-04-20 20:52:59.000000 throttle_client-0.4.8/python_client/tests/test_server_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:53:03.665805 throttle_client-0.4.8/python_client/throttle_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-20 20:52:59.000000 throttle_client-0.4.8/python_client/throttle_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-04-20 20:52:59.000000 throttle_client-0.4.8/python_client/throttle_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-20 20:52:59.000000 throttle_client-0.4.8/python_client/throttle_client/peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-20 20:52:59.000000 throttle_client-0.4.8/python_client/throttle_client/status_code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:53:03.665805 throttle_client-0.4.8/python_client/throttle_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10089 2024-04-20 20:53:03.000000 throttle_client-0.4.8/python_client/throttle_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-20 20:53:03.000000 throttle_client-0.4.8/python_client/throttle_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 20:53:03.000000 throttle_client-0.4.8/python_client/throttle_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-20 20:53:03.000000 throttle_client-0.4.8/python_client/throttle_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 20:53:03.000000 throttle_client-0.4.8/python_client/throttle_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 20:53:03.669805 throttle_client-0.4.8/setup.cfg
```

### Comparing `throttle_client-0.4.5/LICENSE` & `throttle_client-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `throttle_client-0.4.5/PKG-INFO` & `throttle_client-0.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: throttle_client
-Version: 0.4.5
+Version: 0.4.8
 Summary: Client for Throttle. Throttle is an http semaphore service, providing semaphores for distributed systems.
-Home-page: https://github.com/pacman82/throttle.git
-Author: Markus Klein
+Author: Markus Klein 
+License: MIT License
+Project-URL: Repository, https://github.com/pacman82/throttle.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: tenacity
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 # Throttle
 
 Semaphores for distributed systems.
 
 ## Motivation
```

### Comparing `throttle_client-0.4.5/tests/test_lock.py` & `throttle_client-0.4.8/python_client/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.4.5/tests/test_peer.py` & `throttle_client-0.4.8/python_client/tests/test_peer.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.4.5/tests/test_server_client.py` & `throttle_client-0.4.8/python_client/tests/test_server_client.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.4.5/throttle_client/__init__.py` & `throttle_client-0.4.8/python_client/throttle_client/__init__.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.4.5/throttle_client/client.py` & `throttle_client-0.4.8/python_client/throttle_client/client.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.4.5/throttle_client/peer.py` & `throttle_client-0.4.8/python_client/throttle_client/peer.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.4.5/throttle_client/status_code.py` & `throttle_client-0.4.8/python_client/throttle_client/status_code.py`

 * *Files identical despite different names*

### Comparing `throttle_client-0.4.5/throttle_client.egg-info/PKG-INFO` & `throttle_client-0.4.8/python_client/throttle_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
-Name: throttle-client
-Version: 0.4.5
+Name: throttle_client
+Version: 0.4.8
 Summary: Client for Throttle. Throttle is an http semaphore service, providing semaphores for distributed systems.
-Home-page: https://github.com/pacman82/throttle.git
-Author: Markus Klein
+Author: Markus Klein 
+License: MIT License
+Project-URL: Repository, https://github.com/pacman82/throttle.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: tenacity
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 # Throttle
 
 Semaphores for distributed systems.
 
 ## Motivation
```

