# Comparing `tmp/room_env-1.0.3.tar.gz` & `tmp/room_env-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "room_env-1.0.3.tar", last modified: Fri Apr  5 15:08:21 2024, max compression
+gzip compressed data, was "room_env-2.0.0.tar", last modified: Sat Apr 20 09:24:56 2024, max compression
```

## Comparing `room_env-1.0.3.tar` & `room_env-2.0.0.tar`

### file list

```diff
@@ -1,50 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:08:21.236081 room_env-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-05 15:08:11.000000 room_env-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-05 15:08:21.236081 room_env-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-05 15:08:11.000000 room_env-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:08:21.224081 room_env-1.0.3/room_env/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18450 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/create_room2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:08:21.236081 room_env-1.0.3/room_env/data/
--rw-r--r--   0 runner    (1001) docker     (127)   429221 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/conceptnet-data.json
--rw-r--r--   0 runner    (1001) docker     (127)    47857 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/des-config-l-v1.json
--rw-r--r--   0 runner    (1001) docker     (127)    17989 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/des-config-m-v1.json
--rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/des-config-s-v1.json
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/des-config-xs-v1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/des-config-xxs-v1.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/human-locations
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/human-names
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/ms-coco-80-categories
--rw-r--r--   0 runner    (1001) docker     (127)     9817 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/names-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)   108782 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/room-config-dev-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)  3908646 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/room-config-foo-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)    30841 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/room-config-l-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)    57836 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/room-config-l2-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)    10030 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/room-config-m-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/room-config-s-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)   110453 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/room-config-xl-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/room-config-xs-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)  3912948 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/room-config-xxl-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/room-config-xxs-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/semantic-knowledge-small.json
--rw-r--r--   0 runner    (1001) docker     (127)     9801 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/semantic-knowledge.json
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/top-human-names
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/top-human-names-small
--rw-r--r--   0 runner    (1001) docker     (127)     8484 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/des.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:08:21.236081 room_env-1.0.3/room_env/envs/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16548 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/envs/room0.py
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/envs/room1.py
--rw-r--r--   0 runner    (1001) docker     (127)    35816 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/envs/room2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19876 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:08:21.224081 room_env-1.0.3/room_env.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-05 15:08:21.000000 room_env-1.0.3/room_env.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-05 15:08:21.000000 room_env-1.0.3/room_env.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:08:21.000000 room_env-1.0.3/room_env.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 15:08:21.000000 room_env-1.0.3/room_env.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 15:08:21.000000 room_env-1.0.3/room_env.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-05 15:08:21.240081 room_env-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 15:08:11.000000 room_env-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:08:21.236081 room_env-1.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-05 15:08:11.000000 room_env-1.0.3/test/test_des.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-05 15:08:11.000000 room_env-1.0.3/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:24:56.139458 room_env-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 09:24:47.000000 room_env-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-20 09:24:56.143458 room_env-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-20 09:24:47.000000 room_env-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:24:56.131458 room_env-2.0.0/room_env/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18450 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/create_room2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:24:56.139458 room_env-2.0.0/room_env/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   429221 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/conceptnet-data.json
+-rw-r--r--   0 runner    (1001) docker     (127)    47857 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/des-config-l-v1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17989 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/des-config-m-v1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/des-config-s-v1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/des-config-xs-v1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/des-config-xxs-v1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/human-locations
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/human-names
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/ms-coco-80-categories
+-rw-r--r--   0 runner    (1001) docker     (127)     9817 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/names-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)   108782 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/room-config-dev-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)  3908646 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/room-config-foo-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30841 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/room-config-l-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10030 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/room-config-m-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/room-config-s-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)   110149 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/room-config-xl-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/room-config-xs-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)   411708 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/room-config-xxl-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/room-config-xxs-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/semantic-knowledge-small.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9801 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/semantic-knowledge.json
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/top-human-names
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/data/top-human-names-small
+-rw-r--r--   0 runner    (1001) docker     (127)     8484 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/des.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:24:56.139458 room_env-2.0.0/room_env/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16548 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/envs/room0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/envs/room1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35910 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/envs/room2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19876 2024-04-20 09:24:47.000000 room_env-2.0.0/room_env/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:24:56.131458 room_env-2.0.0/room_env.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-20 09:24:56.000000 room_env-2.0.0/room_env.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-20 09:24:56.000000 room_env-2.0.0/room_env.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 09:24:56.000000 room_env-2.0.0/room_env.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-20 09:24:56.000000 room_env-2.0.0/room_env.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 09:24:56.000000 room_env-2.0.0/room_env.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-20 09:24:56.143458 room_env-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-20 09:24:47.000000 room_env-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:24:56.139458 room_env-2.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-20 09:24:47.000000 room_env-2.0.0/test/test_des.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-20 09:24:47.000000 room_env-2.0.0/test/test_utils.py
```

### Comparing `room_env-1.0.3/LICENSE` & `room_env-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/PKG-INFO` & `room_env-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: room_env
-Version: 1.0.3
+Version: 2.0.0
 Summary: The Room environment
 Home-page: https://github.com/humemai/room-env
 Author: Taewoon Kim
 Author-email: info@humem.ai
 Project-URL: Bug Tracker, https://github.com/humemai/room-env/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `room_env-1.0.3/README.md` & `room_env-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/create_room2.py` & `room_env-2.0.0/room_env/create_room2.py`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/data/conceptnet-data.json` & `room_env-2.0.0/room_env/data/conceptnet-data.json`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/data/des-config-l-v1.json` & `room_env-2.0.0/room_env/data/des-config-l-v1.json`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/data/des-config-m-v1.json` & `room_env-2.0.0/room_env/data/des-config-m-v1.json`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/data/des-config-s-v1.json` & `room_env-2.0.0/room_env/data/des-config-s-v1.json`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/data/des-config-xs-v1.json` & `room_env-2.0.0/room_env/data/des-config-xs-v1.json`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/data/des-config-xxs-v1.json` & `room_env-2.0.0/room_env/data/des-config-xxs-v1.json`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/data/human-names` & `room_env-2.0.0/room_env/data/human-names`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/data/ms-coco-80-categories` & `room_env-2.0.0/room_env/data/ms-coco-80-categories`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/data/names-v2.json` & `room_env-2.0.0/room_env/data/names-v2.json`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/data/room-config-dev-v2.json` & `room_env-2.0.0/room_env/data/room-config-dev-v2.json`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/data/room-config-foo-v2.json` & `room_env-2.0.0/room_env/data/room-config-foo-v2.json`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/data/room-config-l-v2.json` & `room_env-2.0.0/room_env/data/room-config-l-v2.json`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/data/room-config-m-v2.json` & `room_env-2.0.0/room_env/data/room-config-m-v2.json`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/data/room-config-s-v2.json` & `room_env-2.0.0/room_env/data/room-config-s-v2.json`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/data/room-config-xl-v2.json` & `room_env-2.0.0/room_env/data/room-config-xl-v2.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9021387021208381%*

 * *Differences: {"'grid'": '{0: {insert: [(3, 0)], delete: [6]}, 1: {insert: [(0, 0)], delete: [6]}, 3: {insert: '*

 * *           '[(0, 0), (1, 0)], delete: [6, 5]}, 4: {insert: [(0, 0), (6, 1)], delete: [5, 0]}, 5: '*

 * *           '{insert: [(1, 1)], delete: [0]}, 6: {insert: [(3, 0), (4, 0), (6, 0)], delete: [3, 1, '*

 * *           '0]}, insert: [(2, [0, 0, 0, 1, 0, 1, 1])], delete: [1]}',*

 * * "'object_init_config'": "{'static': {'sta_000': {'room_023': 1, 'room_031': 0}, 'sta_001': "*

 * *                         "{'room_007': 1, 'room_01 […]*

```diff
@@ -1,71 +1,71 @@
 {
     "grid": [
         [
             0,
             1,
             1,
             0,
+            0,
             1,
-            1,
-            0
+            1
         ],
         [
             0,
-            0,
             1,
-            0,
-            1,
-            1,
-            0
-        ],
-        [
             1,
             1,
             1,
             1,
+            1
+        ],
+        [
+            0,
+            0,
+            0,
             1,
+            0,
             1,
-            0
+            1
         ],
         [
+            0,
+            0,
             1,
             1,
             1,
             1,
-            1,
-            0,
-            0
+            1
         ],
         [
-            1,
+            0,
             0,
             1,
             1,
             1,
             0,
-            0
+            1
         ],
         [
-            1,
             0,
             1,
             1,
             1,
             1,
+            1,
             1
         ],
         [
-            0,
-            0,
             1,
-            0,
             1,
             1,
-            1
+            0,
+            0,
+            1,
+            0
         ]
     ],
     "names": {
         "dependent_objects": [
             "dep_000",
             "dep_001",
             "dep_002",
@@ -184,41 +184,41 @@
                 "room_012": 0,
                 "room_013": 0,
                 "room_014": 0,
                 "room_015": 0,
                 "room_016": 0,
                 "room_017": 0,
                 "room_018": 0,
-                "room_019": 0,
+                "room_019": 1,
                 "room_020": 0,
                 "room_021": 0,
                 "room_022": 0,
                 "room_023": 0,
-                "room_024": 1,
+                "room_024": 0,
                 "room_025": 0,
                 "room_026": 0,
                 "room_027": 0,
                 "room_028": 0,
                 "room_029": 0,
                 "room_030": 0,
                 "room_031": 0
             },
             "dep_001": {
-                "room_000": 0,
+                "room_000": 1,
                 "room_001": 0,
                 "room_002": 0,
                 "room_003": 0,
                 "room_004": 0,
                 "room_005": 0,
                 "room_006": 0,
                 "room_007": 0,
                 "room_008": 0,
                 "room_009": 0,
                 "room_010": 0,
-                "room_011": 1,
+                "room_011": 0,
                 "room_012": 0,
                 "room_013": 0,
                 "room_014": 0,
                 "room_015": 0,
                 "room_016": 0,
                 "room_017": 0,
                 "room_018": 0,
@@ -241,24 +241,24 @@
                 "room_001": 0,
                 "room_002": 0,
                 "room_003": 0,
                 "room_004": 0,
                 "room_005": 0,
                 "room_006": 0,
                 "room_007": 0,
-                "room_008": 0,
+                "room_008": 1,
                 "room_009": 0,
                 "room_010": 0,
                 "room_011": 0,
                 "room_012": 0,
                 "room_013": 0,
                 "room_014": 0,
                 "room_015": 0,
                 "room_016": 0,
-                "room_017": 1,
+                "room_017": 0,
                 "room_018": 0,
                 "room_019": 0,
                 "room_020": 0,
                 "room_021": 0,
                 "room_022": 0,
                 "room_023": 0,
                 "room_024": 0,
@@ -293,33 +293,33 @@
                 "room_019": 0,
                 "room_020": 0,
                 "room_021": 0,
                 "room_022": 0,
                 "room_023": 0,
                 "room_024": 0,
                 "room_025": 0,
-                "room_026": 1,
+                "room_026": 0,
                 "room_027": 0,
                 "room_028": 0,
-                "room_029": 0,
+                "room_029": 1,
                 "room_030": 0,
                 "room_031": 0
             },
             "dep_004": {
-                "room_000": 1,
+                "room_000": 0,
                 "room_001": 0,
                 "room_002": 0,
                 "room_003": 0,
                 "room_004": 0,
                 "room_005": 0,
                 "room_006": 0,
                 "room_007": 0,
                 "room_008": 0,
                 "room_009": 0,
-                "room_010": 0,
+                "room_010": 1,
                 "room_011": 0,
                 "room_012": 0,
                 "room_013": 0,
                 "room_014": 0,
                 "room_015": 0,
                 "room_016": 0,
                 "room_017": 0,
@@ -356,23 +356,23 @@
                 "room_014": 0,
                 "room_015": 0,
                 "room_016": 0,
                 "room_017": 0,
                 "room_018": 0,
                 "room_019": 0,
                 "room_020": 0,
-                "room_021": 1,
+                "room_021": 0,
                 "room_022": 0,
                 "room_023": 0,
                 "room_024": 0,
                 "room_025": 0,
                 "room_026": 0,
                 "room_027": 0,
                 "room_028": 0,
-                "room_029": 0,
+                "room_029": 1,
                 "room_030": 0,
                 "room_031": 0
             },
             "dep_006": {
                 "room_000": 0,
                 "room_001": 0,
                 "room_002": 0,
@@ -391,27 +391,27 @@
                 "room_015": 0,
                 "room_016": 0,
                 "room_017": 0,
                 "room_018": 0,
                 "room_019": 0,
                 "room_020": 0,
                 "room_021": 0,
-                "room_022": 1,
+                "room_022": 0,
                 "room_023": 0,
                 "room_024": 0,
                 "room_025": 0,
                 "room_026": 0,
                 "room_027": 0,
                 "room_028": 0,
                 "room_029": 0,
                 "room_030": 0,
-                "room_031": 0
+                "room_031": 1
             },
             "dep_007": {
-                "room_000": 0,
+                "room_000": 1,
                 "room_001": 0,
                 "room_002": 0,
                 "room_003": 0,
                 "room_004": 0,
                 "room_005": 0,
                 "room_006": 0,
                 "room_007": 0,
@@ -424,15 +424,15 @@
                 "room_014": 0,
                 "room_015": 0,
                 "room_016": 0,
                 "room_017": 0,
                 "room_018": 0,
                 "room_019": 0,
                 "room_020": 0,
-                "room_021": 1,
+                "room_021": 0,
                 "room_022": 0,
                 "room_023": 0,
                 "room_024": 0,
                 "room_025": 0,
                 "room_026": 0,
                 "room_027": 0,
                 "room_028": 0,
@@ -441,15 +441,15 @@
                 "room_031": 0
             }
         },
         "independent": {
             "ind_000": {
                 "room_000": 0,
                 "room_001": 0,
-                "room_002": 0,
+                "room_002": 1,
                 "room_003": 0,
                 "room_004": 0,
                 "room_005": 0,
                 "room_006": 0,
                 "room_007": 0,
                 "room_008": 0,
                 "room_009": 0,
@@ -458,15 +458,15 @@
                 "room_012": 0,
                 "room_013": 0,
                 "room_014": 0,
                 "room_015": 0,
                 "room_016": 0,
                 "room_017": 0,
                 "room_018": 0,
-                "room_019": 1,
+                "room_019": 0,
                 "room_020": 0,
                 "room_021": 0,
                 "room_022": 0,
                 "room_023": 0,
                 "room_024": 0,
                 "room_025": 0,
                 "room_026": 0,
@@ -479,26 +479,26 @@
             "ind_001": {
                 "room_000": 0,
                 "room_001": 0,
                 "room_002": 0,
                 "room_003": 0,
                 "room_004": 0,
                 "room_005": 0,
-                "room_006": 1,
+                "room_006": 0,
                 "room_007": 0,
                 "room_008": 0,
                 "room_009": 0,
                 "room_010": 0,
                 "room_011": 0,
                 "room_012": 0,
                 "room_013": 0,
                 "room_014": 0,
                 "room_015": 0,
                 "room_016": 0,
-                "room_017": 0,
+                "room_017": 1,
                 "room_018": 0,
                 "room_019": 0,
                 "room_020": 0,
                 "room_021": 0,
                 "room_022": 0,
                 "room_023": 0,
                 "room_024": 0,
@@ -525,34 +525,34 @@
                 "room_011": 0,
                 "room_012": 0,
                 "room_013": 0,
                 "room_014": 0,
                 "room_015": 0,
                 "room_016": 0,
                 "room_017": 0,
-                "room_018": 1,
+                "room_018": 0,
                 "room_019": 0,
                 "room_020": 0,
                 "room_021": 0,
                 "room_022": 0,
                 "room_023": 0,
                 "room_024": 0,
                 "room_025": 0,
                 "room_026": 0,
                 "room_027": 0,
                 "room_028": 0,
-                "room_029": 0,
+                "room_029": 1,
                 "room_030": 0,
                 "room_031": 0
             },
             "ind_003": {
                 "room_000": 0,
                 "room_001": 0,
-                "room_002": 0,
-                "room_003": 1,
+                "room_002": 1,
+                "room_003": 0,
                 "room_004": 0,
                 "room_005": 0,
                 "room_006": 0,
                 "room_007": 0,
                 "room_008": 0,
                 "room_009": 0,
                 "room_010": 0,
@@ -589,29 +589,29 @@
                 "room_007": 0,
                 "room_008": 0,
                 "room_009": 0,
                 "room_010": 0,
                 "room_011": 0,
                 "room_012": 0,
                 "room_013": 0,
-                "room_014": 1,
+                "room_014": 0,
                 "room_015": 0,
                 "room_016": 0,
                 "room_017": 0,
                 "room_018": 0,
                 "room_019": 0,
                 "room_020": 0,
                 "room_021": 0,
                 "room_022": 0,
                 "room_023": 0,
                 "room_024": 0,
                 "room_025": 0,
                 "room_026": 0,
                 "room_027": 0,
-                "room_028": 0,
+                "room_028": 1,
                 "room_029": 0,
                 "room_030": 0,
                 "room_031": 0
             },
             "ind_005": {
                 "room_000": 0,
                 "room_001": 0,
@@ -620,26 +620,26 @@
                 "room_004": 0,
                 "room_005": 0,
                 "room_006": 0,
                 "room_007": 0,
                 "room_008": 0,
                 "room_009": 0,
                 "room_010": 0,
-                "room_011": 0,
+                "room_011": 1,
                 "room_012": 0,
                 "room_013": 0,
                 "room_014": 0,
                 "room_015": 0,
                 "room_016": 0,
                 "room_017": 0,
                 "room_018": 0,
                 "room_019": 0,
                 "room_020": 0,
                 "room_021": 0,
-                "room_022": 1,
+                "room_022": 0,
                 "room_023": 0,
                 "room_024": 0,
                 "room_025": 0,
                 "room_026": 0,
                 "room_027": 0,
                 "room_028": 0,
                 "room_029": 0,
@@ -652,30 +652,30 @@
                 "room_002": 0,
                 "room_003": 0,
                 "room_004": 0,
                 "room_005": 0,
                 "room_006": 0,
                 "room_007": 0,
                 "room_008": 0,
-                "room_009": 0,
+                "room_009": 1,
                 "room_010": 0,
                 "room_011": 0,
                 "room_012": 0,
                 "room_013": 0,
                 "room_014": 0,
                 "room_015": 0,
                 "room_016": 0,
                 "room_017": 0,
                 "room_018": 0,
                 "room_019": 0,
                 "room_020": 0,
                 "room_021": 0,
                 "room_022": 0,
                 "room_023": 0,
-                "room_024": 1,
+                "room_024": 0,
                 "room_025": 0,
                 "room_026": 0,
                 "room_027": 0,
                 "room_028": 0,
                 "room_029": 0,
                 "room_030": 0,
                 "room_031": 0
@@ -706,16 +706,16 @@
                 "room_022": 0,
                 "room_023": 0,
                 "room_024": 0,
                 "room_025": 0,
                 "room_026": 0,
                 "room_027": 0,
                 "room_028": 0,
-                "room_029": 1,
-                "room_030": 0,
+                "room_029": 0,
+                "room_030": 1,
                 "room_031": 0
             }
         },
         "static": {
             "sta_000": {
                 "room_000": 0,
                 "room_001": 0,
@@ -736,44 +736,44 @@
                 "room_016": 0,
                 "room_017": 0,
                 "room_018": 0,
                 "room_019": 0,
                 "room_020": 0,
                 "room_021": 0,
                 "room_022": 0,
-                "room_023": 0,
+                "room_023": 1,
                 "room_024": 0,
                 "room_025": 0,
                 "room_026": 0,
                 "room_027": 0,
                 "room_028": 0,
                 "room_029": 0,
                 "room_030": 0,
-                "room_031": 1
+                "room_031": 0
             },
             "sta_001": {
                 "room_000": 0,
                 "room_001": 0,
                 "room_002": 0,
                 "room_003": 0,
                 "room_004": 0,
                 "room_005": 0,
                 "room_006": 0,
-                "room_007": 0,
+                "room_007": 1,
                 "room_008": 0,
                 "room_009": 0,
                 "room_010": 0,
                 "room_011": 0,
                 "room_012": 0,
                 "room_013": 0,
                 "room_014": 0,
                 "room_015": 0,
                 "room_016": 0,
                 "room_017": 0,
-                "room_018": 1,
+                "room_018": 0,
                 "room_019": 0,
                 "room_020": 0,
                 "room_021": 0,
                 "room_022": 0,
                 "room_023": 0,
                 "room_024": 0,
                 "room_025": 0,
@@ -789,15 +789,15 @@
                 "room_001": 0,
                 "room_002": 0,
                 "room_003": 0,
                 "room_004": 0,
                 "room_005": 0,
                 "room_006": 0,
                 "room_007": 0,
-                "room_008": 0,
+                "room_008": 1,
                 "room_009": 0,
                 "room_010": 0,
                 "room_011": 0,
                 "room_012": 0,
                 "room_013": 0,
                 "room_014": 0,
                 "room_015": 0,
@@ -810,15 +810,15 @@
                 "room_022": 0,
                 "room_023": 0,
                 "room_024": 0,
                 "room_025": 0,
                 "room_026": 0,
                 "room_027": 0,
                 "room_028": 0,
-                "room_029": 1,
+                "room_029": 0,
                 "room_030": 0,
                 "room_031": 0
             },
             "sta_003": {
                 "room_000": 0,
                 "room_001": 0,
                 "room_002": 0,
@@ -830,40 +830,40 @@
                 "room_008": 0,
                 "room_009": 0,
                 "room_010": 0,
                 "room_011": 0,
                 "room_012": 0,
                 "room_013": 0,
                 "room_014": 0,
-                "room_015": 0,
+                "room_015": 1,
                 "room_016": 0,
                 "room_017": 0,
                 "room_018": 0,
                 "room_019": 0,
                 "room_020": 0,
                 "room_021": 0,
                 "room_022": 0,
                 "room_023": 0,
                 "room_024": 0,
-                "room_025": 1,
+                "room_025": 0,
                 "room_026": 0,
                 "room_027": 0,
                 "room_028": 0,
                 "room_029": 0,
                 "room_030": 0,
                 "room_031": 0
             },
             "sta_004": {
                 "room_000": 0,
                 "room_001": 0,
                 "room_002": 0,
                 "room_003": 0,
                 "room_004": 0,
                 "room_005": 0,
-                "room_006": 0,
+                "room_006": 1,
                 "room_007": 0,
                 "room_008": 0,
                 "room_009": 0,
                 "room_010": 0,
                 "room_011": 0,
                 "room_012": 0,
                 "room_013": 0,
@@ -880,20 +880,20 @@
                 "room_024": 0,
                 "room_025": 0,
                 "room_026": 0,
                 "room_027": 0,
                 "room_028": 0,
                 "room_029": 0,
                 "room_030": 0,
-                "room_031": 1
+                "room_031": 0
             },
             "sta_005": {
                 "room_000": 0,
                 "room_001": 0,
-                "room_002": 1,
+                "room_002": 0,
                 "room_003": 0,
                 "room_004": 0,
                 "room_005": 0,
                 "room_006": 0,
                 "room_007": 0,
                 "room_008": 0,
                 "room_009": 0,
@@ -904,29 +904,29 @@
                 "room_014": 0,
                 "room_015": 0,
                 "room_016": 0,
                 "room_017": 0,
                 "room_018": 0,
                 "room_019": 0,
                 "room_020": 0,
-                "room_021": 0,
+                "room_021": 1,
                 "room_022": 0,
                 "room_023": 0,
                 "room_024": 0,
                 "room_025": 0,
                 "room_026": 0,
                 "room_027": 0,
                 "room_028": 0,
                 "room_029": 0,
                 "room_030": 0,
                 "room_031": 0
             },
             "sta_006": {
                 "room_000": 0,
-                "room_001": 1,
+                "room_001": 0,
                 "room_002": 0,
                 "room_003": 0,
                 "room_004": 0,
                 "room_005": 0,
                 "room_006": 0,
                 "room_007": 0,
                 "room_008": 0,
@@ -942,38 +942,38 @@
                 "room_018": 0,
                 "room_019": 0,
                 "room_020": 0,
                 "room_021": 0,
                 "room_022": 0,
                 "room_023": 0,
                 "room_024": 0,
-                "room_025": 0,
+                "room_025": 1,
                 "room_026": 0,
                 "room_027": 0,
                 "room_028": 0,
                 "room_029": 0,
                 "room_030": 0,
                 "room_031": 0
             },
             "sta_007": {
                 "room_000": 0,
                 "room_001": 0,
-                "room_002": 0,
+                "room_002": 1,
                 "room_003": 0,
                 "room_004": 0,
                 "room_005": 0,
                 "room_006": 0,
                 "room_007": 0,
                 "room_008": 0,
                 "room_009": 0,
                 "room_010": 0,
                 "room_011": 0,
                 "room_012": 0,
                 "room_013": 0,
-                "room_014": 1,
+                "room_014": 0,
                 "room_015": 0,
                 "room_016": 0,
                 "room_017": 0,
                 "room_018": 0,
                 "room_019": 0,
                 "room_020": 0,
                 "room_021": 0,
@@ -991,1937 +991,1937 @@
         }
     },
     "object_question_probs": {
         "agent": {
             "agent": 0.0
         },
         "dependent": {
-            "dep_000": 0.015362596260210977,
-            "dep_001": 0.014776466282346933,
-            "dep_002": 0.023445601340987523,
-            "dep_003": 0.0016345886499845059,
-            "dep_004": 0.003571560719997937,
-            "dep_005": 0.04026265876214573,
-            "dep_006": 0.10199626471363166,
-            "dep_007": 0.005313227944272331
+            "dep_000": 0.0022663102653724472,
+            "dep_001": 0.014685282036481678,
+            "dep_002": 0.10101025266139947,
+            "dep_003": 0.026976497291859615,
+            "dep_004": 7.236845205592738e-06,
+            "dep_005": 0.09287214175542319,
+            "dep_006": 0.0020638279901311904,
+            "dep_007": 0.022929936337438315
         },
         "independent": {
-            "ind_000": 0.012727603626771637,
-            "ind_001": 0.07447008647105027,
-            "ind_002": 0.03607881956257715,
-            "ind_003": 0.07636425821364862,
-            "ind_004": 0.09940502314725334,
-            "ind_005": 0.014631442224346276,
-            "ind_006": 0.06473372844228621,
-            "ind_007": 0.07342083052749099
+            "ind_000": 0.010546379327719697,
+            "ind_001": 0.11878574023961112,
+            "ind_002": 0.06749886550508111,
+            "ind_003": 0.0014138849043265293,
+            "ind_004": 0.022253178874070235,
+            "ind_005": 0.015494468196316955,
+            "ind_006": 0.007064306980980398,
+            "ind_007": 0.04456854565607142
         },
         "static": {
-            "sta_000": 0.0033394813710483384,
-            "sta_001": 0.03834581705574367,
-            "sta_002": 0.04674321509284692,
-            "sta_003": 0.002587299549681935,
-            "sta_004": 0.03214634035471116,
-            "sta_005": 0.08954904429051222,
-            "sta_006": 0.07215184201313082,
-            "sta_007": 0.056942203383322836
+            "sta_000": 0.011267229883543034,
+            "sta_001": 0.007717681239925757,
+            "sta_002": 0.11925163280664475,
+            "sta_003": 0.04476333566195444,
+            "sta_004": 0.05843900892269737,
+            "sta_005": 0.09113045317800013,
+            "sta_006": 0.11698834841163121,
+            "sta_007": 5.455028114389916e-06
         }
     },
     "object_transition_config": {
         "agent": {
             "agent": null
         },
         "dependent": {
             "dep_000": {
-                "ind_000": 0.8634397833783154,
-                "ind_001": 0.7570261989193423,
-                "ind_002": 0.15778886593659183,
-                "ind_003": 0.9339974692242846,
-                "ind_004": 0.833070787624315,
-                "ind_005": 0.47338790155511273,
-                "ind_006": 0.9376295162228548,
-                "ind_007": 0.9386138465201427
+                "ind_000": 0.9188310994324984,
+                "ind_001": 0.7546048151683147,
+                "ind_002": 0.5609056191081652,
+                "ind_003": 0.8136569250635987,
+                "ind_004": 0.010621189154327243,
+                "ind_005": 0.981861561785355,
+                "ind_006": 0.9998749297229952,
+                "ind_007": 0.17748832009800808
             },
             "dep_001": {
-                "ind_000": 0.10169278782052842,
-                "ind_001": 0.7201334172074583,
-                "ind_002": 0.059327960221440636,
-                "ind_003": 0.7147809451452275,
-                "ind_004": 0.4890451783874595,
-                "ind_005": 0.9847819444643297,
-                "ind_006": 0.8335271355666917,
-                "ind_007": 0.7532802539380649
+                "ind_000": 0.9510154037290763,
+                "ind_001": 0.9774193387919629,
+                "ind_002": 0.4038539772693749,
+                "ind_003": 0.008317966521270067,
+                "ind_004": 0.18462688551183218,
+                "ind_005": 0.8429593585679264,
+                "ind_006": 0.38285523819151346,
+                "ind_007": 0.8084668881551642
             },
             "dep_002": {
-                "ind_000": 0.8493181330364273,
-                "ind_001": 0.3476579078767452,
-                "ind_002": 0.9947365506397292,
-                "ind_003": 0.21260100033985735,
-                "ind_004": 0.1580386529570318,
-                "ind_005": 0.3420561419405248,
-                "ind_006": 0.999484395364773,
-                "ind_007": 0.9838172280165629
+                "ind_000": 0.9392358510417698,
+                "ind_001": 0.12983690435040718,
+                "ind_002": 0.1292599290573525,
+                "ind_003": 0.648051900059395,
+                "ind_004": 0.48519812298545384,
+                "ind_005": 0.021930649349994454,
+                "ind_006": 0.8415086643026927,
+                "ind_007": 0.9118096435358779
             },
             "dep_003": {
-                "ind_000": 0.28254741577916087,
-                "ind_001": 0.3770666546885573,
-                "ind_002": 0.1552177036594073,
-                "ind_003": 0.8564788773239562,
-                "ind_004": 0.4897659136782435,
-                "ind_005": 0.9750828829431667,
-                "ind_006": 0.0023941257041906537,
-                "ind_007": 0.6382518278033107
+                "ind_000": 0.43290012412738205,
+                "ind_001": 0.6676467208337155,
+                "ind_002": 0.5727251019724482,
+                "ind_003": 0.40529276304806733,
+                "ind_004": 0.9488990125382546,
+                "ind_005": 0.6599950538033508,
+                "ind_006": 0.39740285049495266,
+                "ind_007": 0.05418856021841453
             },
             "dep_004": {
-                "ind_000": 0.19026482875982803,
-                "ind_001": 0.995573085326699,
-                "ind_002": 0.39513460163656755,
-                "ind_003": 0.4400328493936636,
-                "ind_004": 0.9682554721832352,
-                "ind_005": 0.488262955619429,
-                "ind_006": 0.7847811576123075,
-                "ind_007": 0.9921529201428053
+                "ind_000": 0.9999591916607997,
+                "ind_001": 0.6379249869434817,
+                "ind_002": 0.5398479985501113,
+                "ind_003": 0.03834129994602044,
+                "ind_004": 0.8541009336196688,
+                "ind_005": 0.18765816431956087,
+                "ind_006": 0.722639210710709,
+                "ind_007": 0.9444974199268373
             },
             "dep_005": {
-                "ind_000": 0.025654251261200228,
-                "ind_001": 0.4409219442254312,
-                "ind_002": 0.7567802884350497,
-                "ind_003": 0.023674539142185005,
-                "ind_004": 0.5633280595434516,
-                "ind_005": 0.9386977194068374,
-                "ind_006": 0.11835459440029282,
-                "ind_007": 0.12997981032738717
+                "ind_000": 0.3852960651173566,
+                "ind_001": 0.41763871769657285,
+                "ind_002": 0.8287201668086416,
+                "ind_003": 0.7683522314090495,
+                "ind_004": 0.9049370437273039,
+                "ind_005": 0.5222477452604793,
+                "ind_006": 0.8884409831965299,
+                "ind_007": 0.8363032001047498
             },
             "dep_006": {
-                "ind_000": 0.5936618513760653,
-                "ind_001": 0.9702981893225837,
-                "ind_002": 0.0034699336965954277,
-                "ind_003": 0.7248917670097004,
-                "ind_004": 0.5174404157935757,
-                "ind_005": 0.4875427405701829,
-                "ind_006": 0.7421527285612387,
-                "ind_007": 0.058035230499647296
+                "ind_000": 0.043076102270963215,
+                "ind_001": 0.999924594212706,
+                "ind_002": 0.7234368001095278,
+                "ind_003": 0.007811225895528365,
+                "ind_004": 0.5223097534510319,
+                "ind_005": 0.19852332606051482,
+                "ind_006": 0.302266428218352,
+                "ind_007": 0.4457705447735336
             },
             "dep_007": {
-                "ind_000": 0.9915400828989163,
-                "ind_001": 0.3957071667235167,
-                "ind_002": 0.6392062743625212,
-                "ind_003": 0.9181132259386,
-                "ind_004": 0.11656007988030555,
-                "ind_005": 0.00014843750445328225,
-                "ind_006": 0.9961028652692923,
-                "ind_007": 0.8593783693476251
+                "ind_000": 0.9250221959996686,
+                "ind_001": 0.2689724827202166,
+                "ind_002": 0.8109023798689093,
+                "ind_003": 0.04028221856399241,
+                "ind_004": 0.9999232747897157,
+                "ind_005": 0.7299256392667581,
+                "ind_006": 0.4506435058679548,
+                "ind_007": 0.18857452449086878
             }
         },
         "independent": {
             "ind_000": {
                 "room_000": {
-                    "east": 0.3100429931218375,
+                    "east": 0.14853868680148252,
                     "north": 0.0,
-                    "south": 0.0,
-                    "stay": 0.6899570068781625,
+                    "south": 0.1313951699044732,
+                    "stay": 0.7200661432940443,
                     "west": 0.0
                 },
                 "room_001": {
                     "east": 0.0,
                     "north": 0.0,
-                    "south": 0.0626205198920241,
-                    "stay": 0.7604727274931893,
-                    "west": 0.17690675261478658
+                    "south": 0.11848107529504656,
+                    "stay": 0.7242705684891328,
+                    "west": 0.1572483562158206
                 },
                 "room_002": {
-                    "east": 0.00658893982059903,
+                    "east": 0.06843747767958186,
                     "north": 0.0,
-                    "south": 0.11449012103440971,
-                    "stay": 0.8789209391449913,
+                    "south": 0.130780875261297,
+                    "stay": 0.8007816470591211,
                     "west": 0.0
                 },
                 "room_003": {
                     "east": 0.0,
                     "north": 0.0,
-                    "south": 0.004007745613161838,
-                    "stay": 0.8322061856443308,
-                    "west": 0.16378606874250737
+                    "south": 0.11348932494252688,
+                    "stay": 0.6272269152107335,
+                    "west": 0.2592837598467397
                 },
                 "room_004": {
-                    "east": 0.0,
-                    "north": 0.24671248100764684,
-                    "south": 0.08551709584919952,
-                    "stay": 0.6677704231431536,
+                    "east": 0.015195607713666617,
+                    "north": 0.10111432098823542,
+                    "south": 0.0,
+                    "stay": 0.883690071298098,
                     "west": 0.0
                 },
                 "room_005": {
-                    "east": 0.2202654905100068,
-                    "north": 0.05464690454124409,
-                    "south": 0.11980984057816016,
-                    "stay": 0.605277764370589,
-                    "west": 0.0
+                    "east": 0.1867854176509734,
+                    "north": 0.13508863711934682,
+                    "south": 0.0,
+                    "stay": 0.6561953934025936,
+                    "west": 0.02193055182708623
                 },
                 "room_006": {
-                    "east": 0.0,
-                    "north": 0.093053889722333,
-                    "south": 0.011083553644704407,
-                    "stay": 0.8019041180192308,
-                    "west": 0.09395843861373182
+                    "east": 0.010863165564059462,
+                    "north": 0.0,
+                    "south": 0.07488681442588668,
+                    "stay": 0.8830750010028438,
+                    "west": 0.031175019007210095
                 },
                 "room_007": {
-                    "east": 0.005985602950951384,
+                    "east": 0.08502914013101187,
                     "north": 0.0,
-                    "south": 0.0863028706958885,
-                    "stay": 0.9077115263531601,
-                    "west": 0.0
+                    "south": 0.0,
+                    "stay": 0.8891332193997656,
+                    "west": 0.025837640469222496
                 },
                 "room_008": {
-                    "east": 0.010993834264792142,
-                    "north": 0.0,
-                    "south": 0.022281765190735874,
-                    "stay": 0.7313165307891445,
-                    "west": 0.23540786975532746
+                    "east": 0.0034511636428879275,
+                    "north": 0.022108740737024287,
+                    "south": 0.23309935364798845,
+                    "stay": 0.6414911754806641,
+                    "west": 0.09984956649143516
                 },
                 "room_009": {
-                    "east": 0.029472236750185524,
-                    "north": 0.05528722849078994,
-                    "south": 0.011954051093391626,
-                    "stay": 0.8906293333057513,
-                    "west": 0.01265715035988159
+                    "east": 0.0,
+                    "north": 0.002412753898245097,
+                    "south": 0.00497851298557219,
+                    "stay": 0.9872638639892896,
+                    "west": 0.005344869126893154
                 },
                 "room_010": {
-                    "east": 0.1668144353233639,
-                    "north": 0.0,
-                    "south": 0.17144053411552918,
-                    "stay": 0.655248977876956,
-                    "west": 0.0064960526841509065
+                    "east": 0.0,
+                    "north": 0.012259183256589107,
+                    "south": 0.235498045839356,
+                    "stay": 0.7522427709040549,
+                    "west": 0.0
                 },
                 "room_011": {
-                    "east": 0.022356739123175248,
-                    "north": 0.04095066339697197,
-                    "south": 0.019286336397864614,
-                    "stay": 0.8762179153818961,
-                    "west": 0.04118834570009209
+                    "east": 0.03401715125880606,
+                    "north": 0.009989225355690625,
+                    "south": 0.02240887031243577,
+                    "stay": 0.9335847530730675,
+                    "west": 0.0
                 },
                 "room_012": {
                     "east": 0.0,
-                    "north": 0.04322106186852561,
-                    "south": 0.0,
-                    "stay": 0.6908226949618269,
-                    "west": 0.2659562431696475
+                    "north": 0.05060741718387057,
+                    "south": 0.04254678448899541,
+                    "stay": 0.8152719402369906,
+                    "west": 0.09157385809014346
                 },
                 "room_013": {
-                    "east": 0.17301843027390967,
-                    "north": 0.13164287037279507,
-                    "south": 0.012023824062415828,
-                    "stay": 0.6833148752908794,
+                    "east": 0.1344959191204806,
+                    "north": 0.0,
+                    "south": 0.07905173775492165,
+                    "stay": 0.7864523431245978,
                     "west": 0.0
                 },
                 "room_014": {
-                    "east": 0.10080446043814605,
-                    "north": 0.04945471662703372,
-                    "south": 0.0,
-                    "stay": 0.8392660182043753,
-                    "west": 0.010474804730444941
+                    "east": 0.02712494042429278,
+                    "north": 0.026469760733602802,
+                    "south": 0.01653067753473112,
+                    "stay": 0.902021975779338,
+                    "west": 0.02785264552803535
                 },
                 "room_015": {
-                    "east": 0.10957734379542715,
-                    "north": 0.037824457878015666,
-                    "south": 0.012881545984817317,
-                    "stay": 0.7239312419180701,
-                    "west": 0.11578541042366976
+                    "east": 0.18524089335002772,
+                    "north": 0.0,
+                    "south": 0.012439473298629777,
+                    "stay": 0.6576525520726879,
+                    "west": 0.14466708127865463
                 },
                 "room_016": {
-                    "east": 0.01899648926647655,
-                    "north": 0.04514986888704923,
-                    "south": 0.03567709351035097,
-                    "stay": 0.8993051493128105,
-                    "west": 0.0008713990233127691
+                    "east": 0.08820403150004989,
+                    "north": 0.061285877473347516,
+                    "south": 0.0,
+                    "stay": 0.7041065304988241,
+                    "west": 0.14640356052777848
                 },
                 "room_017": {
                     "east": 0.0,
-                    "north": 0.017905194162471428,
-                    "south": 0.02921343160297414,
-                    "stay": 0.951483282026322,
-                    "west": 0.0013980922082323906
+                    "north": 0.02821640539646261,
+                    "south": 0.022092075685640557,
+                    "stay": 0.9495585490044242,
+                    "west": 0.00013296991347267923
                 },
                 "room_018": {
-                    "east": 0.0,
-                    "north": 0.23320062156250407,
-                    "south": 0.10289602734944062,
-                    "stay": 0.6639033510880553,
+                    "east": 0.04995003655366441,
+                    "north": 0.18815336674110023,
+                    "south": 0.01504691387502871,
+                    "stay": 0.7468496828302067,
                     "west": 0.0
                 },
                 "room_019": {
-                    "east": 0.00013864583378867383,
-                    "north": 0.046153601074627244,
-                    "south": 0.00189167976215978,
-                    "stay": 0.9518160733294243,
-                    "west": 0.0
+                    "east": 0.11318120285477636,
+                    "north": 0.09319581007793211,
+                    "south": 0.12262699920446918,
+                    "stay": 0.6296875089103945,
+                    "west": 0.04130847895242789
                 },
                 "room_020": {
-                    "east": 0.023839882728646972,
-                    "north": 0.03333945871841219,
-                    "south": 0.1269820996079363,
-                    "stay": 0.6780482376891466,
-                    "west": 0.13779032125585794
+                    "east": 0.0,
+                    "north": 0.19319087585516156,
+                    "south": 0.023872200337553214,
+                    "stay": 0.6543243712210628,
+                    "west": 0.12861255258622248
                 },
                 "room_021": {
                     "east": 0.0,
-                    "north": 0.051893588089240876,
-                    "south": 0.19126140158622162,
-                    "stay": 0.6655454257885651,
-                    "west": 0.09129958453597238
+                    "north": 0.263353966349588,
+                    "south": 0.03483077736901092,
+                    "stay": 0.7018152562814011,
+                    "west": 0.0
                 },
                 "room_022": {
-                    "east": 0.0,
-                    "north": 0.12958218135521404,
-                    "south": 0.0,
-                    "stay": 0.870417818644786,
+                    "east": 0.09501010051945116,
+                    "north": 0.0,
+                    "south": 0.04524238857852068,
+                    "stay": 0.8597475109020282,
                     "west": 0.0
                 },
                 "room_023": {
-                    "east": 0.002020753641187437,
-                    "north": 0.02744954501517995,
-                    "south": 0.03113032690479669,
-                    "stay": 0.9393993744388359,
-                    "west": 0.0
+                    "east": 0.008248097480470765,
+                    "north": 0.004933976640318741,
+                    "south": 0.00982912266292222,
+                    "stay": 0.9675897418006075,
+                    "west": 0.009399061415680744
                 },
                 "room_024": {
-                    "east": 0.000313233510222371,
-                    "north": 0.0006250115633540718,
+                    "east": 0.0013968799840317022,
+                    "north": 0.09222365104295767,
                     "south": 0.0,
-                    "stay": 0.9865159864829947,
-                    "west": 0.012545768443428902
+                    "stay": 0.7881804825462981,
+                    "west": 0.1181989864267125
                 },
                 "room_025": {
-                    "east": 0.11183440338239505,
-                    "north": 0.09340972041439086,
-                    "south": 0.13393342697365127,
-                    "stay": 0.648078500151867,
-                    "west": 0.012743949077695894
+                    "east": 0.0013698313699793427,
+                    "north": 0.04903115676390186,
+                    "south": 0.0,
+                    "stay": 0.9065767604932876,
+                    "west": 0.04302225137283118
                 },
                 "room_026": {
-                    "east": 0.2579165176422963,
+                    "east": 0.1496374247929589,
                     "north": 0.0,
-                    "south": 0.04688692336646173,
-                    "stay": 0.6683744933846784,
-                    "west": 0.026822065606563604
+                    "south": 0.013326563943977458,
+                    "stay": 0.7157352343131522,
+                    "west": 0.12130077694991141
                 },
                 "room_027": {
                     "east": 0.0,
-                    "north": 0.0,
-                    "south": 0.07348010034660786,
-                    "stay": 0.730527474771464,
-                    "west": 0.1959924248819282
+                    "north": 0.028228645711521706,
+                    "south": 0.0,
+                    "stay": 0.8826589321334362,
+                    "west": 0.08911242215504213
                 },
                 "room_028": {
-                    "east": 0.0,
-                    "north": 0.2680012842046534,
+                    "east": 0.11624831882917575,
+                    "north": 0.0,
                     "south": 0.0,
-                    "stay": 0.7319987157953466,
+                    "stay": 0.8837516811708243,
                     "west": 0.0
                 },
                 "room_029": {
-                    "east": 0.012286858577389183,
-                    "north": 0.02306681898708931,
+                    "east": 0.00018097249570866238,
+                    "north": 0.14688328811039147,
                     "south": 0.0,
-                    "stay": 0.9646463224355215,
-                    "west": 0.0
+                    "stay": 0.8337382214744617,
+                    "west": 0.019197517919438075
                 },
                 "room_030": {
-                    "east": 0.1387135640779557,
-                    "north": 0.07407205783191093,
+                    "east": 0.0,
+                    "north": 0.08035505198390394,
                     "south": 0.0,
-                    "stay": 0.7064264741522137,
-                    "west": 0.08078790393791965
+                    "stay": 0.8447741709761943,
+                    "west": 0.07487077703990173
                 },
                 "room_031": {
                     "east": 0.0,
-                    "north": 0.08704229914217962,
+                    "north": 0.22503147205378982,
                     "south": 0.0,
-                    "stay": 0.8735050400642868,
-                    "west": 0.03945266079353363
+                    "stay": 0.7749685279462102,
+                    "west": 0.0
                 }
             },
             "ind_001": {
                 "room_000": {
-                    "east": 0.17226304481690802,
+                    "east": 0.06316445648908249,
                     "north": 0.0,
-                    "south": 0.0,
-                    "stay": 0.827736955183092,
+                    "south": 0.31207511003777616,
+                    "stay": 0.6247604334731414,
                     "west": 0.0
                 },
                 "room_001": {
                     "east": 0.0,
                     "north": 0.0,
-                    "south": 0.03942963089594493,
-                    "stay": 0.9028276481442544,
-                    "west": 0.057742720959800646
+                    "south": 0.052858116424431015,
+                    "stay": 0.923728526310666,
+                    "west": 0.02341335726490294
                 },
                 "room_002": {
-                    "east": 0.005310515466553341,
+                    "east": 0.07434498525161014,
                     "north": 0.0,
-                    "south": 0.09223315909059583,
-                    "stay": 0.9024563254428508,
+                    "south": 0.0020984122759323412,
+                    "stay": 0.9235566024724575,
                     "west": 0.0
                 },
                 "room_003": {
                     "east": 0.0,
                     "north": 0.0,
-                    "south": 0.10586321831286366,
-                    "stay": 0.7753941125433987,
-                    "west": 0.11874266914373761
+                    "south": 0.025892715960094875,
+                    "stay": 0.9711240060925673,
+                    "west": 0.0029832779473377958
                 },
                 "room_004": {
-                    "east": 0.0,
-                    "north": 0.06887180623668847,
-                    "south": 0.041884983634053755,
-                    "stay": 0.8892432101292578,
+                    "east": 0.03476512794108741,
+                    "north": 0.000810980554494832,
+                    "south": 0.0,
+                    "stay": 0.9644238915044178,
                     "west": 0.0
                 },
                 "room_005": {
-                    "east": 0.01816995283784134,
-                    "north": 0.051582306258872064,
-                    "south": 0.13538697076749276,
-                    "stay": 0.7948607701357938,
-                    "west": 0.0
+                    "east": 0.19119169998544863,
+                    "north": 0.060738114134438456,
+                    "south": 0.0,
+                    "stay": 0.7086580079579672,
+                    "west": 0.039412177922145734
                 },
                 "room_006": {
-                    "east": 0.0,
-                    "north": 0.09485777227475634,
-                    "south": 0.007526588186337811,
-                    "stay": 0.7708215697379945,
-                    "west": 0.12679406980091132
+                    "east": 0.1353282203202429,
+                    "north": 0.0,
+                    "south": 0.2107271969661554,
+                    "stay": 0.6500424991830517,
+                    "west": 0.0039020835305500195
                 },
                 "room_007": {
-                    "east": 0.16776844484492492,
+                    "east": 0.01755197538225322,
                     "north": 0.0,
-                    "south": 0.14327340407007058,
-                    "stay": 0.6889581510850045,
-                    "west": 0.0
+                    "south": 0.0,
+                    "stay": 0.9467204276105091,
+                    "west": 0.035727597007237655
                 },
                 "room_008": {
-                    "east": 0.024338282636918555,
-                    "north": 0.0,
-                    "south": 0.0006148316947897132,
-                    "stay": 0.836974163801832,
-                    "west": 0.13807272186645975
+                    "east": 0.04991978442415036,
+                    "north": 0.00452040436141678,
+                    "south": 0.1561102009503956,
+                    "stay": 0.7227521865340232,
+                    "west": 0.06669742373001403
                 },
                 "room_009": {
-                    "east": 0.08108997458571104,
-                    "north": 0.0049989245613790145,
-                    "south": 0.07497383979096604,
-                    "stay": 0.6960024391166475,
-                    "west": 0.14293482194529641
+                    "east": 0.0,
+                    "north": 0.010681165261374413,
+                    "south": 0.0008434895552610459,
+                    "stay": 0.8580119182721866,
+                    "west": 0.13046342691117793
                 },
                 "room_010": {
-                    "east": 0.10272303210330534,
-                    "north": 0.0,
-                    "south": 0.09769791691405741,
-                    "stay": 0.7370142404537886,
-                    "west": 0.06256481052884866
+                    "east": 0.0,
+                    "north": 0.04684600559562984,
+                    "south": 0.04570830888405948,
+                    "stay": 0.9074456855203107,
+                    "west": 0.0
                 },
                 "room_011": {
-                    "east": 0.00014389699929026693,
-                    "north": 0.1540104345476887,
-                    "south": 0.09583300814587573,
-                    "stay": 0.6970004239951214,
-                    "west": 0.05301223631202391
+                    "east": 0.2023057257842549,
+                    "north": 0.10712205509382206,
+                    "south": 0.02628627575172963,
+                    "stay": 0.6642859433701934,
+                    "west": 0.0
                 },
                 "room_012": {
                     "east": 0.0,
-                    "north": 0.09915323870647157,
-                    "south": 0.0,
-                    "stay": 0.6918959078449898,
-                    "west": 0.20895085344853864
+                    "north": 0.10573587394066514,
+                    "south": 0.0009883372584064418,
+                    "stay": 0.8007939616235754,
+                    "west": 0.09248182717735301
                 },
                 "room_013": {
-                    "east": 0.13323611439260413,
-                    "north": 0.12746318863382275,
-                    "south": 0.13457075643282362,
-                    "stay": 0.6047299405407495,
+                    "east": 0.2535789744620287,
+                    "north": 0.0,
+                    "south": 0.017609523347331877,
+                    "stay": 0.7288115021906394,
                     "west": 0.0
                 },
                 "room_014": {
-                    "east": 0.11999124290801381,
-                    "north": 0.10090302341909556,
-                    "south": 0.0,
-                    "stay": 0.6392978191391394,
-                    "west": 0.1398079145337512
+                    "east": 0.12311770711079603,
+                    "north": 0.09311041909553806,
+                    "south": 0.01737230816767588,
+                    "stay": 0.6426634712985815,
+                    "west": 0.12373609432740852
                 },
                 "room_015": {
-                    "east": 0.00015377000430798787,
-                    "north": 0.003928393665729976,
-                    "south": 0.0048444712147713825,
-                    "stay": 0.9892298244389637,
-                    "west": 0.0018435406762269747
+                    "east": 0.06401884204129453,
+                    "north": 0.0,
+                    "south": 0.03995980742144249,
+                    "stay": 0.8410014471748909,
+                    "west": 0.05501990336237212
                 },
                 "room_016": {
-                    "east": 0.13629622662243998,
-                    "north": 0.05291299797915632,
-                    "south": 0.10344144339968032,
-                    "stay": 0.6963493524395881,
-                    "west": 0.010999979559135306
+                    "east": 0.25970237365891197,
+                    "north": 0.0052464001251736085,
+                    "south": 0.0,
+                    "stay": 0.6136060397061206,
+                    "west": 0.1214451865097939
                 },
                 "room_017": {
                     "east": 0.0,
-                    "north": 0.03828512772450059,
-                    "south": 0.017741387197744537,
-                    "stay": 0.9195150313116176,
-                    "west": 0.024458453766137277
+                    "north": 0.003692487820599745,
+                    "south": 0.0935094992933769,
+                    "stay": 0.8547323247638446,
+                    "west": 0.0480656881221787
                 },
                 "room_018": {
-                    "east": 0.0,
-                    "north": 0.0007155088791273522,
-                    "south": 0.2783466375486951,
-                    "stay": 0.7209378535721775,
+                    "east": 0.04576873613869367,
+                    "north": 0.16569560996794297,
+                    "south": 0.07384028800388502,
+                    "stay": 0.7146953658894784,
                     "west": 0.0
                 },
                 "room_019": {
-                    "east": 0.0013529859550470867,
-                    "north": 0.0011466501479081234,
-                    "south": 0.0006953646159699907,
-                    "stay": 0.9968049992810748,
-                    "west": 0.0
+                    "east": 0.002065765762009434,
+                    "north": 0.0009358016021453698,
+                    "south": 0.0017827233049171956,
+                    "stay": 0.9922861344601586,
+                    "west": 0.002929574870769436
                 },
                 "room_020": {
-                    "east": 0.04805869136425815,
-                    "north": 0.00152158129538817,
-                    "south": 0.07184382244761878,
-                    "stay": 0.8351968298766788,
-                    "west": 0.043379075016056125
+                    "east": 0.0,
+                    "north": 0.09808865283114966,
+                    "south": 0.06404722851773599,
+                    "stay": 0.7429473106597622,
+                    "west": 0.09491680799135219
                 },
                 "room_021": {
                     "east": 0.0,
-                    "north": 0.08868259052569148,
-                    "south": 0.1653235586332661,
-                    "stay": 0.606211288095898,
-                    "west": 0.1397825627451445
+                    "north": 0.14667555982037894,
+                    "south": 0.13789849587084457,
+                    "stay": 0.7154259443087765,
+                    "west": 0.0
                 },
                 "room_022": {
-                    "east": 0.0,
-                    "north": 0.2678107428665035,
-                    "south": 0.0,
-                    "stay": 0.7321892571334965,
+                    "east": 0.01002223316076298,
+                    "north": 0.0,
+                    "south": 0.02233293633292024,
+                    "stay": 0.9676448305063168,
                     "west": 0.0
                 },
                 "room_023": {
-                    "east": 0.156392008076261,
-                    "north": 0.16891514659171872,
-                    "south": 4.279270947755914e-06,
-                    "stay": 0.6746885660610725,
-                    "west": 0.0
+                    "east": 0.06187914860750345,
+                    "north": 0.12545431279416816,
+                    "south": 0.12615133282921726,
+                    "stay": 0.671419117736966,
+                    "west": 0.015096088032145131
                 },
                 "room_024": {
-                    "east": 0.07584505010854807,
-                    "north": 0.05479281878415133,
+                    "east": 0.017115625219998373,
+                    "north": 0.029022979823675823,
                     "south": 0.0,
-                    "stay": 0.7352396174793452,
-                    "west": 0.13412251362795544
+                    "stay": 0.92374777398686,
+                    "west": 0.030113620969465776
                 },
                 "room_025": {
-                    "east": 0.06682742916985031,
-                    "north": 0.0119195190746372,
-                    "south": 0.001704711891672725,
-                    "stay": 0.8146353094314075,
-                    "west": 0.10491303043243227
+                    "east": 0.0005847330919973754,
+                    "north": 0.07959260977606912,
+                    "south": 0.0,
+                    "stay": 0.9195203128932131,
+                    "west": 0.0003023442387203915
                 },
                 "room_026": {
-                    "east": 0.0009061055738348905,
+                    "east": 0.21903153334638423,
                     "north": 0.0,
-                    "south": 0.11722635846318007,
-                    "stay": 0.7638551841854134,
-                    "west": 0.11801235177757165
+                    "south": 0.010309967665298604,
+                    "stay": 0.7103407489270097,
+                    "west": 0.06031775006130739
                 },
                 "room_027": {
                     "east": 0.0,
-                    "north": 0.0,
-                    "south": 0.10268725361724737,
-                    "stay": 0.8486446545998025,
-                    "west": 0.048668091782950104
+                    "north": 0.0201073205218719,
+                    "south": 0.0,
+                    "stay": 0.8418750584681113,
+                    "west": 0.13801762101001683
                 },
                 "room_028": {
-                    "east": 0.0,
-                    "north": 0.09319752887231936,
+                    "east": 0.37564064835893707,
+                    "north": 0.0,
                     "south": 0.0,
-                    "stay": 0.9068024711276806,
+                    "stay": 0.6243593516410629,
                     "west": 0.0
                 },
                 "room_029": {
-                    "east": 0.01608956051697946,
-                    "north": 0.06409661542507257,
+                    "east": 0.0847387944266825,
+                    "north": 0.17816795232569493,
                     "south": 0.0,
-                    "stay": 0.919813824057948,
-                    "west": 0.0
+                    "stay": 0.6490292231917736,
+                    "west": 0.088064030055849
                 },
                 "room_030": {
-                    "east": 0.040203189457193235,
-                    "north": 0.016448390868692944,
+                    "east": 0.0,
+                    "north": 0.2385756224078008,
                     "south": 0.0,
-                    "stay": 0.8658214391237851,
-                    "west": 0.07752698055032876
+                    "stay": 0.6991883405166982,
+                    "west": 0.062236037075500975
                 },
                 "room_031": {
                     "east": 0.0,
-                    "north": 0.05565587118193706,
+                    "north": 0.24650114066782788,
                     "south": 0.0,
-                    "stay": 0.8860226814366174,
-                    "west": 0.0583214473814455
+                    "stay": 0.7534988593321721,
+                    "west": 0.0
                 }
             },
             "ind_002": {
                 "room_000": {
-                    "east": 0.30707812430598314,
+                    "east": 0.13596580095471839,
                     "north": 0.0,
-                    "south": 0.0,
-                    "stay": 0.6929218756940169,
+                    "south": 0.029974829128217317,
+                    "stay": 0.8340593699170643,
                     "west": 0.0
                 },
                 "room_001": {
                     "east": 0.0,
                     "north": 0.0,
-                    "south": 0.017687255543576825,
-                    "stay": 0.6699285955229948,
-                    "west": 0.3123841489334284
+                    "south": 0.031906660136423584,
+                    "stay": 0.8616124940970544,
+                    "west": 0.10648084576652198
                 },
                 "room_002": {
-                    "east": 0.05909761337231476,
+                    "east": 0.08292492544852789,
                     "north": 0.0,
-                    "south": 0.11359034082259648,
-                    "stay": 0.8273120458050888,
+                    "south": 0.0016065239325238347,
+                    "stay": 0.9154685506189483,
                     "west": 0.0
                 },
                 "room_003": {
                     "east": 0.0,
                     "north": 0.0,
-                    "south": 0.02985370360147128,
-                    "stay": 0.961189756884539,
-                    "west": 0.008956539513989717
+                    "south": 0.03487588594461257,
+                    "stay": 0.8662276584238182,
+                    "west": 0.09889645563156922
                 },
                 "room_004": {
-                    "east": 0.0,
-                    "north": 0.2668290264222995,
-                    "south": 0.04858952181904639,
-                    "stay": 0.6845814517586541,
+                    "east": 0.05001058992450659,
+                    "north": 0.33653507892415613,
+                    "south": 0.0,
+                    "stay": 0.6134543311513373,
                     "west": 0.0
                 },
                 "room_005": {
-                    "east": 0.2162862053843694,
-                    "north": 0.016659104318146378,
-                    "south": 0.0007262563299938369,
-                    "stay": 0.7663284339674904,
-                    "west": 0.0
+                    "east": 0.07608860389123365,
+                    "north": 0.07748913930105701,
+                    "south": 0.0,
+                    "stay": 0.7637791913860847,
+                    "west": 0.08264306542162461
                 },
                 "room_006": {
-                    "east": 0.0,
-                    "north": 0.045888111957312225,
-                    "south": 0.04839908998101224,
-                    "stay": 0.9055884512352917,
-                    "west": 0.00012434682638378506
+                    "east": 0.12340497810947658,
+                    "north": 0.0,
+                    "south": 0.11724940333086716,
+                    "stay": 0.6278332745563066,
+                    "west": 0.13151234400334966
                 },
                 "room_007": {
-                    "east": 0.038843487118213414,
+                    "east": 0.01345711253743419,
                     "north": 0.0,
-                    "south": 0.11907645377346819,
-                    "stay": 0.8420800591083184,
-                    "west": 0.0
+                    "south": 0.0,
+                    "stay": 0.9370267265070131,
+                    "west": 0.04951616095555267
                 },
                 "room_008": {
-                    "east": 0.0992473035199129,
-                    "north": 0.0,
-                    "south": 0.08457370972939553,
-                    "stay": 0.7266593712410898,
-                    "west": 0.08951961550960177
+                    "east": 0.0606156806782611,
+                    "north": 0.07218071395508369,
+                    "south": 0.06935362647996558,
+                    "stay": 0.6437754045117442,
+                    "west": 0.15407457437494543
                 },
                 "room_009": {
-                    "east": 3.4422609106649847e-05,
-                    "north": 0.05875465991600551,
-                    "south": 0.10265609883074797,
-                    "stay": 0.806813927726965,
-                    "west": 0.03174089091717484
+                    "east": 0.0,
+                    "north": 0.011837746521805978,
+                    "south": 0.014047914445603953,
+                    "stay": 0.973668589591829,
+                    "west": 0.00044574944076106074
                 },
                 "room_010": {
-                    "east": 0.12618907387017345,
-                    "north": 0.0,
-                    "south": 0.035406895184163255,
-                    "stay": 0.7195278787533886,
-                    "west": 0.11887615219227465
+                    "east": 0.0,
+                    "north": 0.04175976254857083,
+                    "south": 0.007797312636206096,
+                    "stay": 0.9504429248152231,
+                    "west": 0.0
                 },
                 "room_011": {
-                    "east": 0.0016595988214839737,
-                    "north": 0.02703227286034294,
-                    "south": 0.08629618789154063,
-                    "stay": 0.873997347709346,
-                    "west": 0.011014592717286453
+                    "east": 0.041091107794848876,
+                    "north": 0.040244269342505905,
+                    "south": 0.03958036680351956,
+                    "stay": 0.8790842560591257,
+                    "west": 0.0
                 },
                 "room_012": {
                     "east": 0.0,
-                    "north": 0.16265265815247898,
-                    "south": 0.0,
-                    "stay": 0.8281537164225139,
-                    "west": 0.009193625425007144
+                    "north": 0.00750228384849157,
+                    "south": 0.026125118935679405,
+                    "stay": 0.9468644008956227,
+                    "west": 0.019508196320206287
                 },
                 "room_013": {
-                    "east": 0.0005191705001948781,
-                    "north": 0.03919306739576651,
-                    "south": 0.05105927089002556,
-                    "stay": 0.9092284912140131,
+                    "east": 0.15079440449671042,
+                    "north": 0.0,
+                    "south": 0.21012008707411456,
+                    "stay": 0.639085508429175,
                     "west": 0.0
                 },
                 "room_014": {
-                    "east": 0.1263983480573867,
-                    "north": 0.02980177405929648,
-                    "south": 0.0,
-                    "stay": 0.6624149661027058,
-                    "west": 0.18138491178061103
+                    "east": 0.08435778535970131,
+                    "north": 0.06922514137846585,
+                    "south": 0.00028996264626217496,
+                    "stay": 0.8454863140030078,
+                    "west": 0.0006407966125628855
                 },
                 "room_015": {
-                    "east": 0.10142023242762359,
-                    "north": 0.023254326910557947,
-                    "south": 0.06413700652313778,
-                    "stay": 0.7153431056118613,
-                    "west": 0.09584532852681937
+                    "east": 0.0007865281397351017,
+                    "north": 0.0,
+                    "south": 0.1807480815011716,
+                    "stay": 0.7685842256872143,
+                    "west": 0.04988116467187902
                 },
                 "room_016": {
-                    "east": 0.1104994376315663,
-                    "north": 0.0011234514087996423,
-                    "south": 0.01264905861070162,
-                    "stay": 0.733654001818407,
-                    "west": 0.14207405053052544
+                    "east": 0.16223383061897192,
+                    "north": 0.15286849483203763,
+                    "south": 0.0,
+                    "stay": 0.6548323392969023,
+                    "west": 0.030065335252088116
                 },
                 "room_017": {
                     "east": 0.0,
-                    "north": 0.0072401138682319545,
-                    "south": 0.0020675949033213195,
-                    "stay": 0.9902238026686302,
-                    "west": 0.0004684885598165328
+                    "north": 0.09851414625409917,
+                    "south": 0.11253620692876617,
+                    "stay": 0.7666389675229383,
+                    "west": 0.022310679294196358
                 },
                 "room_018": {
-                    "east": 0.0,
-                    "north": 0.13756695349935166,
-                    "south": 0.10691358414387302,
-                    "stay": 0.7555194623567754,
+                    "east": 0.09673800085528399,
+                    "north": 0.068193788769698,
+                    "south": 0.00014433516455794395,
+                    "stay": 0.8349238752104601,
                     "west": 0.0
                 },
                 "room_019": {
-                    "east": 0.1259801769455579,
-                    "north": 0.0009939686852583943,
-                    "south": 0.028507514074165654,
-                    "stay": 0.844518340295018,
-                    "west": 0.0
+                    "east": 0.009834751776916985,
+                    "north": 0.039625242396077474,
+                    "south": 0.1095531478473609,
+                    "stay": 0.6664343792077626,
+                    "west": 0.17455247877188204
                 },
                 "room_020": {
-                    "east": 0.07290552855699772,
-                    "north": 0.0013555321209536824,
-                    "south": 0.007676670160278599,
-                    "stay": 0.8533229146572787,
-                    "west": 0.0647393545044913
+                    "east": 0.0,
+                    "north": 0.01057197483178422,
+                    "south": 0.0025214498378517535,
+                    "stay": 0.9779642407904452,
+                    "west": 0.008942334539918835
                 },
                 "room_021": {
                     "east": 0.0,
-                    "north": 0.06908479257132609,
-                    "south": 0.042892889795048954,
-                    "stay": 0.8661863151308979,
-                    "west": 0.02183600250272701
+                    "north": 0.21363261405361697,
+                    "south": 0.11566321274709881,
+                    "stay": 0.6707041731992842,
+                    "west": 0.0
                 },
                 "room_022": {
-                    "east": 0.0,
-                    "north": 0.11636349091331345,
-                    "south": 0.0,
-                    "stay": 0.8836365090866866,
+                    "east": 0.08848718232026599,
+                    "north": 0.0,
+                    "south": 0.05122805713334321,
+                    "stay": 0.8602847605463908,
                     "west": 0.0
                 },
                 "room_023": {
-                    "east": 0.0005789517061779247,
-                    "north": 0.025743358194128683,
-                    "south": 0.11666058256103283,
-                    "stay": 0.8570171075386606,
-                    "west": 0.0
+                    "east": 0.14391973410002099,
+                    "north": 0.034685342294207666,
+                    "south": 0.14375290053453527,
+                    "stay": 0.6676232208623161,
+                    "west": 0.010018802208919939
                 },
                 "room_024": {
-                    "east": 0.07787578738438988,
-                    "north": 0.16471578322734123,
+                    "east": 0.10411854616090052,
+                    "north": 0.09612333055614343,
                     "south": 0.0,
-                    "stay": 0.6692071954210719,
-                    "west": 0.088201233967197
+                    "stay": 0.7907161145499128,
+                    "west": 0.009042008733043307
                 },
                 "room_025": {
-                    "east": 0.03082874913606461,
-                    "north": 0.06148018283033746,
-                    "south": 0.053514597919743785,
-                    "stay": 0.7829165676001337,
-                    "west": 0.07125990251372043
+                    "east": 0.007998520816063632,
+                    "north": 0.058793495513509125,
+                    "south": 0.0,
+                    "stay": 0.8802909371451262,
+                    "west": 0.05291704652530105
                 },
                 "room_026": {
-                    "east": 0.009152510458780787,
+                    "east": 0.20954639560190544,
                     "north": 0.0,
-                    "south": 0.10432761146993372,
-                    "stay": 0.8018156048679614,
-                    "west": 0.08470427320332403
+                    "south": 0.0045475444556574264,
+                    "stay": 0.656828137157385,
+                    "west": 0.12907792278505217
                 },
                 "room_027": {
                     "east": 0.0,
-                    "north": 0.0,
-                    "south": 0.1153213133865039,
-                    "stay": 0.6650943539260569,
-                    "west": 0.21958433268743924
+                    "north": 0.12171508505160514,
+                    "south": 0.0,
+                    "stay": 0.6075098015883909,
+                    "west": 0.270775113360004
                 },
                 "room_028": {
-                    "east": 0.0,
-                    "north": 0.30840572397057897,
+                    "east": 0.3891633948136807,
+                    "north": 0.0,
                     "south": 0.0,
-                    "stay": 0.691594276029421,
+                    "stay": 0.6108366051863193,
                     "west": 0.0
                 },
                 "room_029": {
-                    "east": 0.18184366770981455,
-                    "north": 0.19595749991051134,
+                    "east": 0.18744846478589808,
+                    "north": 0.1296299564613901,
                     "south": 0.0,
-                    "stay": 0.6221988323796741,
-                    "west": 0.0
+                    "stay": 0.6583260569974295,
+                    "west": 0.024595521755282315
                 },
                 "room_030": {
-                    "east": 0.10450513829231227,
-                    "north": 0.01449752675018537,
+                    "east": 0.0,
+                    "north": 0.0651151909659152,
                     "south": 0.0,
-                    "stay": 0.8433889822712541,
-                    "west": 0.03760835268624821
+                    "stay": 0.8720898173680036,
+                    "west": 0.06279499166608118
                 },
                 "room_031": {
                     "east": 0.0,
-                    "north": 0.1808393864489815,
+                    "north": 0.30426425566897963,
                     "south": 0.0,
-                    "stay": 0.6363912158688317,
-                    "west": 0.18276939768218678
+                    "stay": 0.6957357443310204,
+                    "west": 0.0
                 }
             },
             "ind_003": {
                 "room_000": {
-                    "east": 0.31253477622616743,
+                    "east": 0.26599431165754817,
                     "north": 0.0,
-                    "south": 0.0,
-                    "stay": 0.6874652237738326,
+                    "south": 3.2766334935674144e-05,
+                    "stay": 0.7339729220075162,
                     "west": 0.0
                 },
                 "room_001": {
                     "east": 0.0,
                     "north": 0.0,
-                    "south": 0.009496166695189523,
-                    "stay": 0.9272628581596706,
-                    "west": 0.0632409751451399
+                    "south": 0.045838621605230015,
+                    "stay": 0.7646938471365714,
+                    "west": 0.18946753125819862
                 },
                 "room_002": {
-                    "east": 0.1458029234606397,
+                    "east": 0.35559013837097553,
                     "north": 0.0,
-                    "south": 0.06725844699987794,
-                    "stay": 0.7869386295394823,
+                    "south": 0.007477802104742793,
+                    "stay": 0.6369320595242817,
                     "west": 0.0
                 },
                 "room_003": {
                     "east": 0.0,
                     "north": 0.0,
-                    "south": 0.12879366775248038,
-                    "stay": 0.8709693376238504,
-                    "west": 0.0002369946236691926
+                    "south": 0.19795840172312587,
+                    "stay": 0.7189915053898367,
+                    "west": 0.08305009288703742
                 },
                 "room_004": {
-                    "east": 0.0,
-                    "north": 0.007774014375707066,
-                    "south": 0.13857140156669706,
-                    "stay": 0.8536545840575959,
+                    "east": 0.16673348333306348,
+                    "north": 0.011698658145066891,
+                    "south": 0.0,
+                    "stay": 0.8215678585218696,
                     "west": 0.0
                 },
                 "room_005": {
-                    "east": 0.018370147290963566,
-                    "north": 0.027782491020670323,
-                    "south": 0.09316844326218872,
-                    "stay": 0.8606789184261774,
-                    "west": 0.0
+                    "east": 0.06087550912249636,
+                    "north": 0.05032500623139809,
+                    "south": 0.0,
+                    "stay": 0.8612435315525793,
+                    "west": 0.0275559530935263
                 },
                 "room_006": {
-                    "east": 0.0,
-                    "north": 0.11408363369736278,
-                    "south": 0.10395242758642659,
-                    "stay": 0.7779395933696194,
-                    "west": 0.004024345346591274
+                    "east": 0.11960750412171436,
+                    "north": 0.0,
+                    "south": 0.0934316030817129,
+                    "stay": 0.6648168436994488,
+                    "west": 0.12214404909712392
                 },
                 "room_007": {
-                    "east": 0.10113141861173121,
+                    "east": 0.09549070539000737,
                     "north": 0.0,
-                    "south": 0.0022101672150611025,
-                    "stay": 0.8966584141732077,
-                    "west": 0.0
+                    "south": 0.0,
+                    "stay": 0.6320923053310158,
+                    "west": 0.2724169892789768
                 },
                 "room_008": {
-                    "east": 0.10003862430921559,
-                    "north": 0.0,
-                    "south": 0.08324551396735126,
-                    "stay": 0.7306311784281432,
-                    "west": 0.08608468329528998
+                    "east": 0.04335522051891871,
+                    "north": 0.06232696995154694,
+                    "south": 0.006383612550628184,
+                    "stay": 0.8865879132123511,
+                    "west": 0.0013462837665550826
                 },
                 "room_009": {
-                    "east": 0.0024714075932596256,
-                    "north": 0.0022524715413623736,
-                    "south": 0.07306351769251758,
-                    "stay": 0.921923275812619,
-                    "west": 0.0002893273602414176
+                    "east": 0.0,
+                    "north": 0.020270760753359516,
+                    "south": 0.2406497813895527,
+                    "stay": 0.7271988207660379,
+                    "west": 0.011880637091049834
                 },
                 "room_010": {
-                    "east": 0.0008033996088002984,
-                    "north": 0.0,
-                    "south": 0.07294328756026766,
-                    "stay": 0.8633997100349691,
-                    "west": 0.06285360279596296
+                    "east": 0.0,
+                    "north": 0.16568515010952056,
+                    "south": 0.06206302496319093,
+                    "stay": 0.7722518249272885,
+                    "west": 0.0
                 },
                 "room_011": {
-                    "east": 0.07225349319447158,
-                    "north": 0.0688085068788914,
-                    "south": 0.07790334762134572,
-                    "stay": 0.7649304743517112,
-                    "west": 0.01610417795358006
+                    "east": 0.0007867830333346354,
+                    "north": 0.0807981207957649,
+                    "south": 0.13241878999716894,
+                    "stay": 0.7859963061737315,
+                    "west": 0.0
                 },
                 "room_012": {
                     "east": 0.0,
-                    "north": 0.19044378162727238,
-                    "south": 0.0,
-                    "stay": 0.8090720487916772,
-                    "west": 0.00048416958105045174
+                    "north": 0.16232615821232335,
+                    "south": 0.04639830529756018,
+                    "stay": 0.6164660757139667,
+                    "west": 0.17480946077614976
                 },
                 "room_013": {
-                    "east": 0.008461586408412823,
-                    "north": 0.0025383362194470235,
-                    "south": 0.0058849038713572315,
-                    "stay": 0.9831151735007829,
+                    "east": 0.033636034783446206,
+                    "north": 0.0,
+                    "south": 0.011633326516305907,
+                    "stay": 0.9547306387002479,
                     "west": 0.0
                 },
                 "room_014": {
-                    "east": 0.025454361133600157,
-                    "north": 2.8868717024264905e-05,
-                    "south": 0.0,
-                    "stay": 0.9418244140249384,
-                    "west": 0.03269235612443715
+                    "east": 0.04864598513006432,
+                    "north": 0.0752939453731428,
+                    "south": 0.11607559831595848,
+                    "stay": 0.7555166505880717,
+                    "west": 0.004467820592762718
                 },
                 "room_015": {
-                    "east": 7.022878763364552e-06,
-                    "north": 0.01889428995543724,
-                    "south": 0.08393221177348809,
-                    "stay": 0.8688684040720122,
-                    "west": 0.02829807132029912
+                    "east": 0.032694363164584815,
+                    "north": 0.0,
+                    "south": 0.010550462419860804,
+                    "stay": 0.956572071543136,
+                    "west": 0.00018310287241843232
                 },
                 "room_016": {
-                    "east": 0.09075700044802985,
-                    "north": 0.01572845288712532,
-                    "south": 0.09279740621633403,
-                    "stay": 0.8007167406734272,
-                    "west": 3.9977508355687853e-07
+                    "east": 0.15788305099579097,
+                    "north": 0.0002736458682472341,
+                    "south": 0.0,
+                    "stay": 0.6628863520906781,
+                    "west": 0.1789569510452836
                 },
                 "room_017": {
                     "east": 0.0,
-                    "north": 0.07819462369153782,
-                    "south": 0.032012536328882776,
-                    "stay": 0.837420761513862,
-                    "west": 0.0523720784657174
+                    "north": 0.004973755276945984,
+                    "south": 0.00022675149474711217,
+                    "stay": 0.9877760234984306,
+                    "west": 0.00702346972987627
                 },
                 "room_018": {
-                    "east": 0.0,
-                    "north": 0.07648234986628184,
-                    "south": 0.07798704520255867,
-                    "stay": 0.8455306049311595,
+                    "east": 0.00030457239462518905,
+                    "north": 0.06746396914325295,
+                    "south": 0.12245584318477311,
+                    "stay": 0.8097756152773488,
                     "west": 0.0
                 },
                 "room_019": {
-                    "east": 0.16865052221217802,
-                    "north": 0.06946256448640228,
-                    "south": 3.2712586703832775e-05,
-                    "stay": 0.7618542007147159,
-                    "west": 0.0
+                    "east": 0.01973847026526648,
+                    "north": 0.07448216358608883,
+                    "south": 0.16520630381583018,
+                    "stay": 0.6167065572651304,
+                    "west": 0.12386650506768414
                 },
                 "room_020": {
-                    "east": 2.2061890456825013e-05,
-                    "north": 0.06712920700704028,
-                    "south": 0.1241134491507886,
-                    "stay": 0.6604591423128605,
-                    "west": 0.14827613963885383
+                    "east": 0.0,
+                    "north": 0.0038330659880738,
+                    "south": 0.02996288239891027,
+                    "stay": 0.9659240583470629,
+                    "west": 0.0002799932659530779
                 },
                 "room_021": {
                     "east": 0.0,
-                    "north": 0.07484924301481997,
-                    "south": 0.11231446184819911,
-                    "stay": 0.7724373122693053,
-                    "west": 0.040398982867675584
+                    "north": 0.1176369674671672,
+                    "south": 0.035757738892559864,
+                    "stay": 0.8466052936402729,
+                    "west": 0.0
                 },
                 "room_022": {
-                    "east": 0.0,
-                    "north": 0.26299538861993244,
-                    "south": 0.0,
-                    "stay": 0.7370046113800676,
+                    "east": 0.18314812135538278,
+                    "north": 0.0,
+                    "south": 0.17954219085199227,
+                    "stay": 0.637309687792625,
                     "west": 0.0
                 },
                 "room_023": {
-                    "east": 0.045345642232936315,
-                    "north": 0.032396041411704275,
-                    "south": 0.04602241129998309,
-                    "stay": 0.8762359050553763,
-                    "west": 0.0
+                    "east": 0.00013769072904662495,
+                    "north": 0.06422416090161763,
+                    "south": 0.044577649691599455,
+                    "stay": 0.82634997330336,
+                    "west": 0.06471052537437628
                 },
                 "room_024": {
-                    "east": 0.0984376765139546,
-                    "north": 0.05889494633893904,
+                    "east": 0.007832162223803521,
+                    "north": 0.0009332559985363144,
                     "south": 0.0,
-                    "stay": 0.7186289310641658,
-                    "west": 0.12403844608294054
+                    "stay": 0.9836267273609115,
+                    "west": 0.0076078544167486615
                 },
                 "room_025": {
-                    "east": 0.03253901476195979,
-                    "north": 0.04798713669700652,
-                    "south": 0.03908572412952197,
-                    "stay": 0.8187086908973178,
-                    "west": 0.061679433514193895
+                    "east": 0.005486320679917367,
+                    "north": 0.09679179542466805,
+                    "south": 0.0,
+                    "stay": 0.8177617641058236,
+                    "west": 0.07996011978959101
                 },
                 "room_026": {
-                    "east": 0.06257858997556752,
+                    "east": 0.03323486117520845,
                     "north": 0.0,
-                    "south": 0.10356194320666026,
-                    "stay": 0.7523711066115111,
-                    "west": 0.08148836020626113
+                    "south": 0.12775317009320428,
+                    "stay": 0.6994546772033337,
+                    "west": 0.13955729152825364
                 },
                 "room_027": {
                     "east": 0.0,
-                    "north": 0.0,
-                    "south": 0.24258102826877487,
-                    "stay": 0.7117037153396456,
-                    "west": 0.04571525639157952
+                    "north": 0.17695495497871835,
+                    "south": 0.0,
+                    "stay": 0.6261183697615792,
+                    "west": 0.19692667525970248
                 },
                 "room_028": {
-                    "east": 0.0,
-                    "north": 0.11684745876169321,
+                    "east": 0.2364221529854594,
+                    "north": 0.0,
                     "south": 0.0,
-                    "stay": 0.8831525412383068,
+                    "stay": 0.7635778470145406,
                     "west": 0.0
                 },
                 "room_029": {
-                    "east": 0.07039143427366018,
-                    "north": 0.13968494851922134,
+                    "east": 0.005132100178204227,
+                    "north": 0.06268244660500862,
                     "south": 0.0,
-                    "stay": 0.7899236172071185,
-                    "west": 0.0
+                    "stay": 0.9239869068929001,
+                    "west": 0.008198546323887071
                 },
                 "room_030": {
-                    "east": 0.22765550699765483,
-                    "north": 0.056221264909350754,
+                    "east": 0.0,
+                    "north": 0.12295175999676872,
                     "south": 0.0,
-                    "stay": 0.6470014366299216,
-                    "west": 0.06912179146307278
+                    "stay": 0.6222194090608869,
+                    "west": 0.2548288309423443
                 },
                 "room_031": {
                     "east": 0.0,
-                    "north": 0.14539845872379206,
+                    "north": 0.31099054896764355,
                     "south": 0.0,
-                    "stay": 0.6679774228649336,
-                    "west": 0.18662411841127444
+                    "stay": 0.6890094510323564,
+                    "west": 0.0
                 }
             },
             "ind_004": {
                 "room_000": {
-                    "east": 0.057159609843084436,
+                    "east": 0.05488406035980181,
                     "north": 0.0,
-                    "south": 0.0,
-                    "stay": 0.9428403901569156,
+                    "south": 0.305691452234971,
+                    "stay": 0.6394244874052272,
                     "west": 0.0
                 },
                 "room_001": {
                     "east": 0.0,
                     "north": 0.0,
-                    "south": 0.2663398236233663,
-                    "stay": 0.6115745638159064,
-                    "west": 0.12208561256072735
+                    "south": 0.05209094388676617,
+                    "stay": 0.9204655981056437,
+                    "west": 0.02744345800759018
                 },
                 "room_002": {
-                    "east": 0.006507984884807525,
+                    "east": 0.05191606486814843,
                     "north": 0.0,
-                    "south": 0.33257325430226314,
-                    "stay": 0.6609187608129293,
+                    "south": 0.1081632168100319,
+                    "stay": 0.8399207183218197,
                     "west": 0.0
                 },
                 "room_003": {
                     "east": 0.0,
                     "north": 0.0,
-                    "south": 0.01242574674643735,
-                    "stay": 0.9807302758887392,
-                    "west": 0.006843977364823472
+                    "south": 0.10713703926241487,
+                    "stay": 0.8527991906941372,
+                    "west": 0.04006377004344789
                 },
                 "room_004": {
-                    "east": 0.0,
-                    "north": 0.0511625944720129,
-                    "south": 0.05982316949402698,
-                    "stay": 0.8890142360339601,
+                    "east": 0.013367742500467593,
+                    "north": 0.013579637262002155,
+                    "south": 0.0,
+                    "stay": 0.9730526202375303,
                     "west": 0.0
                 },
                 "room_005": {
-                    "east": 0.12386721104586645,
-                    "north": 0.1046802635591333,
-                    "south": 0.09862797310565165,
-                    "stay": 0.6728245522893486,
-                    "west": 0.0
+                    "east": 0.15675875805258582,
+                    "north": 0.10212796420821396,
+                    "south": 0.0,
+                    "stay": 0.7247070843245217,
+                    "west": 0.016406193414678482
                 },
                 "room_006": {
-                    "east": 0.0,
-                    "north": 0.1776416597866782,
-                    "south": 0.007049963784566354,
-                    "stay": 0.6814135820169009,
-                    "west": 0.1338947944118545
+                    "east": 0.025255999072739784,
+                    "north": 0.0,
+                    "south": 0.0375552125268873,
+                    "stay": 0.9225181618273558,
+                    "west": 0.014670626573017103
                 },
                 "room_007": {
-                    "east": 0.28424353817701137,
+                    "east": 0.039450454000942506,
                     "north": 0.0,
-                    "south": 0.03171753494725599,
-                    "stay": 0.6840389268757326,
-                    "west": 0.0
+                    "south": 0.0,
+                    "stay": 0.9160887832772412,
+                    "west": 0.04446076272181629
                 },
                 "room_008": {
-                    "east": 0.1586030140518792,
-                    "north": 0.0,
-                    "south": 0.16086123020640686,
-                    "stay": 0.6803468375372593,
-                    "west": 0.00018891820445460914
+                    "east": 0.05140979498210408,
+                    "north": 0.028078133087126797,
+                    "south": 0.160816998543073,
+                    "stay": 0.7536192229150298,
+                    "west": 0.006075850472666334
                 },
                 "room_009": {
-                    "east": 0.0038819142568219354,
-                    "north": 1.1354304722297975e-07,
-                    "south": 0.08179468770598979,
-                    "stay": 0.83452815081074,
-                    "west": 0.07979513368340102
+                    "east": 0.0,
+                    "north": 0.030987607617313874,
+                    "south": 0.033305614913523615,
+                    "stay": 0.8969184823221151,
+                    "west": 0.03878829514704736
                 },
                 "room_010": {
-                    "east": 0.07660318255023614,
-                    "north": 0.0,
-                    "south": 0.14889375470984043,
-                    "stay": 0.620498232566917,
-                    "west": 0.1540048301730064
+                    "east": 0.0,
+                    "north": 0.012873464838012574,
+                    "south": 0.06550880093384856,
+                    "stay": 0.9216177342281389,
+                    "west": 0.0
                 },
                 "room_011": {
-                    "east": 0.08178829102557492,
-                    "north": 0.044052822206041606,
-                    "south": 0.08105210791613426,
-                    "stay": 0.7898097495097077,
-                    "west": 0.00329702934254149
+                    "east": 0.27272714610441745,
+                    "north": 0.1259597492426689,
+                    "south": 2.7021069133812618e-05,
+                    "stay": 0.6012860835837799,
+                    "west": 0.0
                 },
                 "room_012": {
                     "east": 0.0,
-                    "north": 0.25497683889111294,
-                    "south": 0.0,
-                    "stay": 0.728881465758089,
-                    "west": 0.016141695350798044
+                    "north": 0.010946024863076232,
+                    "south": 0.013993463624743945,
+                    "stay": 0.9505279188080396,
+                    "west": 0.02453259270414028
                 },
                 "room_013": {
-                    "east": 7.275500154365861e-05,
-                    "north": 0.017998770540615456,
-                    "south": 0.018831781003955727,
-                    "stay": 0.9630966934538852,
+                    "east": 0.0007863463769663239,
+                    "north": 0.0,
+                    "south": 0.26895608870588317,
+                    "stay": 0.7302575649171505,
                     "west": 0.0
                 },
                 "room_014": {
-                    "east": 0.005664881151944765,
-                    "north": 0.01755893501034543,
-                    "south": 0.0,
-                    "stay": 0.9754848878273581,
-                    "west": 0.0012912960103517112
+                    "east": 0.02983495443492757,
+                    "north": 0.00969338875775379,
+                    "south": 0.0007657725231978138,
+                    "stay": 0.930234228651613,
+                    "west": 0.02947165563250784
                 },
                 "room_015": {
-                    "east": 0.0819526445543473,
-                    "north": 0.027857944837265506,
-                    "south": 0.06920087296873864,
-                    "stay": 0.7795054426181861,
-                    "west": 0.041483095021462434
+                    "east": 0.0315342015009498,
+                    "north": 0.0,
+                    "south": 0.15960861773570276,
+                    "stay": 0.6713757392348269,
+                    "west": 0.13748144152852057
                 },
                 "room_016": {
-                    "east": 0.10402893466392527,
-                    "north": 0.02431038324011887,
-                    "south": 0.09962629246554995,
-                    "stay": 0.7719819757620563,
-                    "west": 5.241386834963274e-05
+                    "east": 0.026111233668397505,
+                    "north": 0.022616032658327963,
+                    "south": 0.0,
+                    "stay": 0.9440464387323838,
+                    "west": 0.007226294940890716
                 },
                 "room_017": {
                     "east": 0.0,
-                    "north": 0.021032073758024794,
-                    "south": 0.01741605721267018,
-                    "stay": 0.9334225362655989,
-                    "west": 0.028129332763706126
+                    "north": 0.01778484974527216,
+                    "south": 0.02970932789714717,
+                    "stay": 0.9140902547981943,
+                    "west": 0.03841556755938639
                 },
                 "room_018": {
-                    "east": 0.0,
-                    "north": 0.0011044803402713683,
-                    "south": 0.09672127326506194,
-                    "stay": 0.9021742463946667,
+                    "east": 0.036158475642291736,
+                    "north": 0.0025133266562278552,
+                    "south": 0.03474791028319883,
+                    "stay": 0.9265802874182816,
                     "west": 0.0
                 },
                 "room_019": {
-                    "east": 0.004332926104713381,
-                    "north": 0.010227389885016645,
-                    "south": 0.0200951018319178,
-                    "stay": 0.9653445821783522,
-                    "west": 0.0
+                    "east": 0.08182827991859784,
+                    "north": 0.09958127376676187,
+                    "south": 0.0763280242907424,
+                    "stay": 0.7336756405228543,
+                    "west": 0.00858678150104361
                 },
                 "room_020": {
-                    "east": 0.12687997945263801,
-                    "north": 7.343377344747082e-05,
-                    "south": 0.061035586910374626,
-                    "stay": 0.7194961273604069,
-                    "west": 0.09251487250313298
+                    "east": 0.0,
+                    "north": 0.10621655410771216,
+                    "south": 0.26098241264731953,
+                    "stay": 0.6138414616114878,
+                    "west": 0.018959571633480565
                 },
                 "room_021": {
                     "east": 0.0,
-                    "north": 0.0012601262673170625,
-                    "south": 0.020366594145805286,
-                    "stay": 0.9385158135181935,
-                    "west": 0.03985746606868419
+                    "north": 0.2052649597237895,
+                    "south": 0.040833496960960516,
+                    "stay": 0.75390154331525,
+                    "west": 0.0
                 },
                 "room_022": {
-                    "east": 0.0,
-                    "north": 0.03040109198598318,
-                    "south": 0.0,
-                    "stay": 0.9695989080140168,
+                    "east": 0.011604854345534765,
+                    "north": 0.0,
+                    "south": 0.008175393112755782,
+                    "stay": 0.9802197525417095,
                     "west": 0.0
                 },
                 "room_023": {
-                    "east": 0.015142308342062247,
-                    "north": 0.014798498212133155,
-                    "south": 4.616646065423235e-09,
-                    "stay": 0.9700591888291585,
-                    "west": 0.0
+                    "east": 0.0016927700043706867,
+                    "north": 0.05045201701800212,
+                    "south": 0.01145298269068941,
+                    "stay": 0.8956146568300034,
+                    "west": 0.04078757345693437
                 },
                 "room_024": {
-                    "east": 0.010822011125882665,
-                    "north": 0.10334163695165748,
+                    "east": 0.05280033962780401,
+                    "north": 0.13318866121705147,
                     "south": 0.0,
-                    "stay": 0.7267907879831349,
-                    "west": 0.15904556393932498
+                    "stay": 0.7378900791505585,
+                    "west": 0.076120920004586
                 },
                 "room_025": {
-                    "east": 0.02767387336482968,
-                    "north": 0.10822179025309935,
-                    "south": 0.02051654822630568,
-                    "stay": 0.7441857606351892,
-                    "west": 0.09940202752057617
+                    "east": 0.16218427553510872,
+                    "north": 0.0478147355190967,
+                    "south": 0.0,
+                    "stay": 0.7594750482599548,
+                    "west": 0.03052594068583978
                 },
                 "room_026": {
-                    "east": 0.03418344629895008,
+                    "east": 0.025430259613037062,
                     "north": 0.0,
-                    "south": 0.050120173221657925,
-                    "stay": 0.8934444967654505,
-                    "west": 0.022251883713941528
+                    "south": 0.04442966704142935,
+                    "stay": 0.780416482782582,
+                    "west": 0.14972359056295156
                 },
                 "room_027": {
                     "east": 0.0,
-                    "north": 0.0,
-                    "south": 0.04840478482472564,
-                    "stay": 0.6845682086349367,
-                    "west": 0.2670270065403376
+                    "north": 0.03813509523115016,
+                    "south": 0.0,
+                    "stay": 0.9540485864876636,
+                    "west": 0.007816318281186282
                 },
                 "room_028": {
-                    "east": 0.0,
-                    "north": 0.2614319479017344,
+                    "east": 0.3378403106880109,
+                    "north": 0.0,
                     "south": 0.0,
-                    "stay": 0.7385680520982656,
+                    "stay": 0.6621596893119891,
                     "west": 0.0
                 },
                 "room_029": {
-                    "east": 0.23701609284308012,
-                    "north": 0.07143167410502169,
+                    "east": 0.055148865407103294,
+                    "north": 0.14201747649079888,
                     "south": 0.0,
-                    "stay": 0.6915522330518982,
-                    "west": 0.0
+                    "stay": 0.6623350616885918,
+                    "west": 0.14049859641350604
                 },
                 "room_030": {
-                    "east": 0.05567897100057954,
-                    "north": 0.12769045291256295,
+                    "east": 0.0,
+                    "north": 0.014887990707277097,
                     "south": 0.0,
-                    "stay": 0.8134034491940177,
-                    "west": 0.003227126892839768
+                    "stay": 0.9717242404174432,
+                    "west": 0.013387768875279692
                 },
                 "room_031": {
                     "east": 0.0,
-                    "north": 0.13408281253006873,
+                    "north": 0.24000436341362144,
                     "south": 0.0,
-                    "stay": 0.8309747789843949,
-                    "west": 0.0349424084855364
+                    "stay": 0.7599956365863786,
+                    "west": 0.0
                 }
             },
             "ind_005": {
                 "room_000": {
-                    "east": 0.20368116778329373,
+                    "east": 0.1640604660340343,
                     "north": 0.0,
-                    "south": 0.0,
-                    "stay": 0.7963188322167063,
+                    "south": 0.23367537859729332,
+                    "stay": 0.6022641553686724,
                     "west": 0.0
                 },
                 "room_001": {
                     "east": 0.0,
                     "north": 0.0,
-                    "south": 0.06692411213023867,
-                    "stay": 0.93205555440921,
-                    "west": 0.0010203334605513718
+                    "south": 0.3136505568446029,
+                    "stay": 0.6473939333817026,
+                    "west": 0.0389555097736945
                 },
                 "room_002": {
-                    "east": 0.11942666956385894,
+                    "east": 0.02439753939778097,
                     "north": 0.0,
-                    "south": 0.1783971199045311,
-                    "stay": 0.70217621053161,
+                    "south": 0.011215805816659959,
+                    "stay": 0.9643866547855591,
                     "west": 0.0
                 },
                 "room_003": {
                     "east": 0.0,
                     "north": 0.0,
-                    "south": 0.18646102128086955,
-                    "stay": 0.7845615801541032,
-                    "west": 0.02897739856502731
+                    "south": 0.04062126979629241,
+                    "stay": 0.9590822155352243,
+                    "west": 0.00029651466848326316
                 },
                 "room_004": {
-                    "east": 0.0,
-                    "north": 0.027621126829490566,
-                    "south": 0.1455088777181548,
-                    "stay": 0.8268699954523546,
+                    "east": 0.03987516583501759,
+                    "north": 0.18749659260256438,
+                    "south": 0.0,
+                    "stay": 0.772628241562418,
                     "west": 0.0
                 },
                 "room_005": {
-                    "east": 0.08055732830807985,
-                    "north": 0.14813396015789954,
-                    "south": 0.14587125268604895,
-                    "stay": 0.6254374588479716,
-                    "west": 0.0
+                    "east": 0.03599523753216843,
+                    "north": 0.033255217062715635,
+                    "south": 0.0,
+                    "stay": 0.9070531187301334,
+                    "west": 0.02369642667498255
                 },
                 "room_006": {
-                    "east": 0.0,
-                    "north": 0.10523629066316807,
-                    "south": 0.053130429377025196,
-                    "stay": 0.7583900928184815,
-                    "west": 0.08324318714132524
+                    "east": 0.047044846268022314,
+                    "north": 0.0,
+                    "south": 0.011269855859823477,
+                    "stay": 0.8309697144949864,
+                    "west": 0.11071558337716784
                 },
                 "room_007": {
-                    "east": 0.14146853063867895,
+                    "east": 0.11864144718564534,
                     "north": 0.0,
-                    "south": 0.13034538340817442,
-                    "stay": 0.7281860859531466,
-                    "west": 0.0
+                    "south": 0.0,
+                    "stay": 0.7529393030511768,
+                    "west": 0.12841924976317784
                 },
                 "room_008": {
-                    "east": 0.05434265784818251,
-                    "north": 0.0,
-                    "south": 0.0018809712771851283,
-                    "stay": 0.8925785972651942,
-                    "west": 0.051197773609438176
+                    "east": 0.0029330508144257855,
+                    "north": 0.0008804941092247062,
+                    "south": 0.0006926049170837877,
+                    "stay": 0.9949964097393565,
+                    "west": 0.0004974404199091741
                 },
                 "room_009": {
-                    "east": 0.016821963379984765,
-                    "north": 0.2009575731329775,
-                    "south": 0.000648321517329903,
-                    "stay": 0.7412345243596574,
-                    "west": 0.04033761761005041
+                    "east": 0.0,
+                    "north": 0.020747037161586008,
+                    "south": 0.021939855938059163,
+                    "stay": 0.9350311669231288,
+                    "west": 0.022281939977226013
                 },
                 "room_010": {
-                    "east": 0.023128979039900414,
-                    "north": 0.0,
-                    "south": 0.05428770271336365,
-                    "stay": 0.8235033343203486,
-                    "west": 0.09907998392638731
+                    "east": 0.0,
+                    "north": 0.05286843592928553,
+                    "south": 0.07726303813709007,
+                    "stay": 0.8698685259336244,
+                    "west": 0.0
                 },
                 "room_011": {
-                    "east": 0.06468247834343091,
-                    "north": 0.05398926508641262,
-                    "south": 0.0509294014124122,
-                    "stay": 0.7590271003138473,
-                    "west": 0.07137175484389696
+                    "east": 0.015455979660954819,
+                    "north": 0.021934619916818852,
+                    "south": 0.23274463632285183,
+                    "stay": 0.7298647640993745,
+                    "west": 0.0
                 },
                 "room_012": {
                     "east": 0.0,
-                    "north": 0.07996951291035204,
-                    "south": 0.0,
-                    "stay": 0.7131847991652944,
-                    "west": 0.20684568792435354
+                    "north": 0.11407090047200594,
+                    "south": 0.010913239569346157,
+                    "stay": 0.8514232008796181,
+                    "west": 0.0235926590790298
                 },
                 "room_013": {
-                    "east": 0.0029064173825604825,
-                    "north": 0.0003108522222635509,
-                    "south": 0.002963988491374927,
-                    "stay": 0.993818741903801,
+                    "east": 0.03737588252953442,
+                    "north": 0.0,
+                    "south": 0.02971317511346969,
+                    "stay": 0.9329109423569959,
                     "west": 0.0
                 },
                 "room_014": {
-                    "east": 0.000592945464548427,
-                    "north": 0.23677767448065215,
-                    "south": 0.0,
-                    "stay": 0.6082850347338684,
-                    "west": 0.15434434532093105
+                    "east": 0.0036029308480480613,
+                    "north": 0.07434612630757338,
+                    "south": 0.014603621746908168,
+                    "stay": 0.8048417686698949,
+                    "west": 0.1026055524275755
                 },
                 "room_015": {
-                    "east": 0.00869877205812875,
-                    "north": 0.04031596984922987,
-                    "south": 0.07320412159672073,
-                    "stay": 0.751106098449802,
-                    "west": 0.1266750380461186
+                    "east": 0.21860698395250314,
+                    "north": 0.0,
+                    "south": 0.00573293671531427,
+                    "stay": 0.7696145699257437,
+                    "west": 0.006045509406438862
                 },
                 "room_016": {
-                    "east": 0.0001089145900943369,
-                    "north": 0.00017332724360708592,
-                    "south": 7.341051391140238e-05,
-                    "stay": 0.9996254473752044,
-                    "west": 1.8900277182751437e-05
+                    "east": 0.0010979287407730477,
+                    "north": 0.11015648501966112,
+                    "south": 0.0,
+                    "stay": 0.8641385825829908,
+                    "west": 0.024607003656575043
                 },
                 "room_017": {
                     "east": 0.0,
-                    "north": 0.09179829722211331,
-                    "south": 0.037350554484411186,
-                    "stay": 0.8693068462994955,
-                    "west": 0.0015443019939799974
+                    "north": 0.00012142057739891594,
+                    "south": 0.02681257675067879,
+                    "stay": 0.9571003067101835,
+                    "west": 0.015965695961738753
                 },
                 "room_018": {
-                    "east": 0.0,
-                    "north": 0.057291149371985095,
-                    "south": 0.04409226189187033,
-                    "stay": 0.8986165887361446,
+                    "east": 0.012822315133411633,
+                    "north": 0.1965268720307919,
+                    "south": 0.08615121250098184,
+                    "stay": 0.7044996003348146,
                     "west": 0.0
                 },
                 "room_019": {
-                    "east": 0.052944548921863434,
-                    "north": 0.05573654632401958,
-                    "south": 0.28820295835105897,
-                    "stay": 0.603115946403058,
-                    "west": 0.0
+                    "east": 0.004743117663177773,
+                    "north": 0.004209740646663897,
+                    "south": 0.000995055840662006,
+                    "stay": 0.9858540569757234,
+                    "west": 0.004198028873772956
                 },
                 "room_020": {
-                    "east": 0.07537092731922423,
-                    "north": 0.15169393595925895,
-                    "south": 0.00040867992379733443,
-                    "stay": 0.6845053179483053,
-                    "west": 0.0880211388494142
+                    "east": 0.0,
+                    "north": 0.071698310859633,
+                    "south": 0.10953861967891347,
+                    "stay": 0.7974059045847027,
+                    "west": 0.021357164876750802
                 },
                 "room_021": {
                     "east": 0.0,
-                    "north": 0.012707534140359043,
-                    "south": 0.007385528794527633,
-                    "stay": 0.9795687628085449,
-                    "west": 0.00033817425656844304
+                    "north": 0.05511994398359725,
+                    "south": 0.17379202811837932,
+                    "stay": 0.7710880278980234,
+                    "west": 0.0
                 },
                 "room_022": {
-                    "east": 0.0,
-                    "north": 0.339987081017072,
-                    "south": 0.0,
-                    "stay": 0.660012918982928,
+                    "east": 0.017797925733196586,
+                    "north": 0.0,
+                    "south": 0.036877053901502,
+                    "stay": 0.9453250203653014,
                     "west": 0.0
                 },
                 "room_023": {
-                    "east": 0.028974773369148357,
-                    "north": 0.03566316981843465,
-                    "south": 0.043798694656143805,
-                    "stay": 0.8915633621562732,
-                    "west": 0.0
+                    "east": 0.13707107828149642,
+                    "north": 0.00051552834963075,
+                    "south": 0.08359906211832877,
+                    "stay": 0.7784752267894168,
+                    "west": 0.00033910446112726193
                 },
                 "room_024": {
-                    "east": 1.1678471436793053e-05,
-                    "north": 0.027620511803649363,
+                    "east": 0.044875213186838514,
+                    "north": 0.04188359794726213,
                     "south": 0.0,
-                    "stay": 0.9407434502473051,
-                    "west": 0.03162435947760874
+                    "stay": 0.9131607828046386,
+                    "west": 8.040606126071004e-05
                 },
                 "room_025": {
-                    "east": 0.1160667322446257,
-                    "north": 0.07972747978875519,
-                    "south": 0.02320680511396648,
-                    "stay": 0.7737775960031121,
-                    "west": 0.007221386849540483
+                    "east": 0.009370354350210336,
+                    "north": 0.04601556165593803,
+                    "south": 0.0,
+                    "stay": 0.8084977226345106,
+                    "west": 0.13611636135934105
                 },
                 "room_026": {
-                    "east": 0.011768773377040622,
+                    "east": 0.1910048204117419,
                     "north": 0.0,
-                    "south": 0.20338623188562552,
-                    "stay": 0.6503579961212417,
-                    "west": 0.13448699861609217
+                    "south": 0.04322026899377093,
+                    "stay": 0.6024340983123666,
+                    "west": 0.16334081228212055
                 },
                 "room_027": {
                     "east": 0.0,
-                    "north": 0.0,
-                    "south": 0.08589697733557293,
-                    "stay": 0.9138141634300287,
-                    "west": 0.00028885923439832484
+                    "north": 0.10967143560819198,
+                    "south": 0.0,
+                    "stay": 0.6545900656465817,
+                    "west": 0.23573849874522632
                 },
                 "room_028": {
-                    "east": 0.0,
-                    "north": 0.30216394958427273,
+                    "east": 0.096677425637552,
+                    "north": 0.0,
                     "south": 0.0,
-                    "stay": 0.6978360504157273,
+                    "stay": 0.903322574362448,
                     "west": 0.0
                 },
                 "room_029": {
-                    "east": 0.18225627885660622,
-                    "north": 0.023243727785772033,
+                    "east": 0.016377017935260234,
+                    "north": 0.03538932080852833,
                     "south": 0.0,
-                    "stay": 0.7944999933576218,
-                    "west": 0.0
+                    "stay": 0.8650417000844075,
+                    "west": 0.08319196117180394
                 },
                 "room_030": {
-                    "east": 0.08053860712597424,
-                    "north": 0.019800829548653667,
+                    "east": 0.0,
+                    "north": 0.06334611648658248,
                     "south": 0.0,
-                    "stay": 0.8841624953888441,
-                    "west": 0.01549806793652802
+                    "stay": 0.8539132347761993,
+                    "west": 0.08274064873721824
                 },
                 "room_031": {
                     "east": 0.0,
-                    "north": 0.045560680357182436,
+                    "north": 0.02760465181459215,
                     "south": 0.0,
-                    "stay": 0.8437782868461493,
-                    "west": 0.11066103279666825
+                    "stay": 0.9723953481854078,
+                    "west": 0.0
                 }
             },
             "ind_006": {
                 "room_000": {
-                    "east": 0.3389511564571096,
+                    "east": 0.020445190873799916,
                     "north": 0.0,
-                    "south": 0.0,
-                    "stay": 0.6610488435428904,
+                    "south": 0.17993905627730156,
+                    "stay": 0.7996157528488985,
                     "west": 0.0
                 },
                 "room_001": {
                     "east": 0.0,
                     "north": 0.0,
-                    "south": 0.09342330882898131,
-                    "stay": 0.8455835794790653,
-                    "west": 0.06099311169195344
+                    "south": 0.28773693819974044,
+                    "stay": 0.6220950930323575,
+                    "west": 0.09016796876790202
                 },
                 "room_002": {
-                    "east": 0.10907356140014045,
+                    "east": 0.013121898727513556,
                     "north": 0.0,
-                    "south": 0.07672154072380456,
-                    "stay": 0.814204897876055,
+                    "south": 0.3366011127963607,
+                    "stay": 0.6502769884761258,
                     "west": 0.0
                 },
                 "room_003": {
                     "east": 0.0,
                     "north": 0.0,
-                    "south": 0.35923268848881157,
-                    "stay": 0.6356761875268759,
-                    "west": 0.005091123984312496
+                    "south": 0.12466399042736892,
+                    "stay": 0.8120694106097524,
+                    "west": 0.06326659896287873
                 },
                 "room_004": {
-                    "east": 0.0,
-                    "north": 0.15905796247275847,
-                    "south": 0.15192117496990032,
-                    "stay": 0.6890208625573412,
+                    "east": 0.020896244462395963,
+                    "north": 0.006505605919485409,
+                    "south": 0.0,
+                    "stay": 0.9725981496181186,
                     "west": 0.0
                 },
                 "room_005": {
-                    "east": 0.0007419626305470929,
-                    "north": 0.019779445519493635,
-                    "south": 0.006407501417594874,
-                    "stay": 0.9730710904323644,
-                    "west": 0.0
+                    "east": 0.1274677422866127,
+                    "north": 1.7590139243802946e-06,
+                    "south": 0.0,
+                    "stay": 0.785838955540947,
+                    "west": 0.08669154315851593
                 },
                 "room_006": {
-                    "east": 0.0,
-                    "north": 0.04452351764266054,
-                    "south": 0.0005369079329021762,
-                    "stay": 0.9188539868483679,
-                    "west": 0.03608558757606934
+                    "east": 0.01570596752363419,
+                    "north": 0.0,
+                    "south": 0.00020348280560827679,
+                    "stay": 0.8070926863755892,
+                    "west": 0.1769978632951684
                 },
                 "room_007": {
-                    "east": 0.0038711959550369944,
+                    "east": 0.10266328812858141,
                     "north": 0.0,
-                    "south": 7.399107250576856e-05,
-                    "stay": 0.9960548129724572,
-                    "west": 0.0
+                    "south": 0.0,
+                    "stay": 0.8708162452979016,
+                    "west": 0.02652046657351701
                 },
                 "room_008": {
-                    "east": 0.14506922282534546,
-                    "north": 0.0,
-                    "south": 0.018145532016365554,
-                    "stay": 0.7733254094423072,
-                    "west": 0.06345983571598177
+                    "east": 0.10644068804901666,
+                    "north": 0.0017703713911680536,
+                    "south": 0.14837708144938025,
+                    "stay": 0.6493822771370904,
+                    "west": 0.09402958197334461
                 },
                 "room_009": {
-                    "east": 0.01572516951343086,
-                    "north": 0.011453998668606915,
-                    "south": 0.019695654302848076,
-                    "stay": 0.8008094400324812,
-                    "west": 0.1523157374826329
+                    "east": 0.0,
+                    "north": 0.03568051145427663,
+                    "south": 0.06694637116717918,
+                    "stay": 0.8118937055180324,
+                    "west": 0.08547941186051179
                 },
                 "room_010": {
-                    "east": 0.18335296879583787,
-                    "north": 0.0,
-                    "south": 9.97815586112688e-06,
-                    "stay": 0.6658607377077083,
-                    "west": 0.15077631534059271
+                    "east": 0.0,
+                    "north": 0.12468293954933034,
+                    "south": 0.030641243413926437,
+                    "stay": 0.8446758170367432,
+                    "west": 0.0
                 },
                 "room_011": {
-                    "east": 0.08704127918663229,
-                    "north": 0.06352885207107116,
-                    "south": 0.04116962444152835,
-                    "stay": 0.7467928891510605,
-                    "west": 0.061467355149707734
+                    "east": 0.015064366354645356,
+                    "north": 0.05374594288569371,
+                    "south": 0.10738057158569178,
+                    "stay": 0.8238091191739692,
+                    "west": 0.0
                 },
                 "room_012": {
                     "east": 0.0,
-                    "north": 0.09477574110190938,
-                    "south": 0.0,
-                    "stay": 0.7148512478188975,
-                    "west": 0.19037301107919305
+                    "north": 0.0626194736544935,
+                    "south": 0.060033966449179695,
+                    "stay": 0.7620544295796595,
+                    "west": 0.1152921303166673
                 },
                 "room_013": {
-                    "east": 0.0020719855770042943,
-                    "north": 0.0027667384611700877,
-                    "south": 0.0008675181142577126,
-                    "stay": 0.9942937578475679,
+                    "east": 0.008448884033369903,
+                    "north": 0.0,
+                    "south": 0.04271049884721285,
+                    "stay": 0.9488406171194173,
                     "west": 0.0
                 },
                 "room_014": {
-                    "east": 0.04112663777224137,
-                    "north": 0.02267901840156162,
-                    "south": 0.0,
-                    "stay": 0.7863230790955021,
-                    "west": 0.14987126473069487
+                    "east": 0.1378337287338904,
+                    "north": 0.04347069400375089,
+                    "south": 0.10329354950756059,
+                    "stay": 0.7039202501859514,
+                    "west": 0.011481777568846708
                 },
                 "room_015": {
-                    "east": 0.20479637250664226,
-                    "north": 0.0043067930535009066,
-                    "south": 0.05974243690468571,
-                    "stay": 0.7215497805958736,
-                    "west": 0.009604616939297532
+                    "east": 0.008910206062380176,
+                    "north": 0.0,
+                    "south": 8.200585649932689e-05,
+                    "stay": 0.6564948858029618,
+                    "west": 0.33451290227815866
                 },
                 "room_016": {
-                    "east": 0.0004730788007310666,
-                    "north": 7.203389718436633e-05,
-                    "south": 0.002643655094839134,
-                    "stay": 0.7591058776530375,
-                    "west": 0.23770535455420794
+                    "east": 0.09582659290412691,
+                    "north": 0.05808795503896166,
+                    "south": 0.0,
+                    "stay": 0.8067832950947429,
+                    "west": 0.039302156962168565
                 },
                 "room_017": {
                     "east": 0.0,
-                    "north": 0.09374174896192995,
-                    "south": 0.019009316283090584,
-                    "stay": 0.871190232920114,
-                    "west": 0.016058701834865477
+                    "north": 0.09072054997915686,
+                    "south": 0.023475539270278522,
+                    "stay": 0.7882859480051605,
+                    "west": 0.09751796274540413
                 },
                 "room_018": {
-                    "east": 0.0,
-                    "north": 0.062434146870902346,
-                    "south": 0.20936311885427214,
-                    "stay": 0.7282027342748255,
+                    "east": 0.07290983168626401,
+                    "north": 0.07553282130515121,
+                    "south": 0.09618305738219578,
+                    "stay": 0.755374289626389,
                     "west": 0.0
                 },
                 "room_019": {
-                    "east": 0.02376178010896702,
-                    "north": 0.25042366091464463,
-                    "south": 0.0024336220312245714,
-                    "stay": 0.7233809369451638,
-                    "west": 0.0
+                    "east": 0.025066633038950927,
+                    "north": 0.015142263859492069,
+                    "south": 0.026266330665256125,
+                    "stay": 0.919458974873274,
+                    "west": 0.014065797563026889
                 },
                 "room_020": {
-                    "east": 0.035669917767392804,
-                    "north": 0.024757243763645975,
-                    "south": 0.0005426584165006495,
-                    "stay": 0.9077267894656059,
-                    "west": 0.031303390586854656
+                    "east": 0.0,
+                    "north": 0.064543696563494,
+                    "south": 0.019221407082181435,
+                    "stay": 0.8680583863489224,
+                    "west": 0.04817651000540218
                 },
                 "room_021": {
                     "east": 0.0,
-                    "north": 0.10651941397683515,
-                    "south": 0.036232982157777,
-                    "stay": 0.8357595412956369,
-                    "west": 0.021488062569750964
+                    "north": 0.04867004941868224,
+                    "south": 0.03982227445787879,
+                    "stay": 0.911507676123439,
+                    "west": 0.0
                 },
                 "room_022": {
-                    "east": 0.0,
-                    "north": 0.35339646302372063,
-                    "south": 0.0,
-                    "stay": 0.6466035369762794,
+                    "east": 0.049726284531069746,
+                    "north": 0.0,
+                    "south": 0.0445114551210929,
+                    "stay": 0.9057622603478374,
                     "west": 0.0
                 },
                 "room_023": {
-                    "east": 0.10741491574153998,
-                    "north": 0.1729052439983711,
-                    "south": 0.026051605394615863,
-                    "stay": 0.6936282348654731,
-                    "west": 0.0
+                    "east": 0.10997556711371187,
+                    "north": 0.00036672812479690255,
+                    "south": 0.02175150304570326,
+                    "stay": 0.8675091002843013,
+                    "west": 0.0003971014314866895
                 },
                 "room_024": {
-                    "east": 0.0007340307779803703,
-                    "north": 0.1072351025804932,
+                    "east": 0.032444605940237764,
+                    "north": 0.2482735365936068,
                     "south": 0.0,
-                    "stay": 0.8628029955156444,
-                    "west": 0.029227871125882
+                    "stay": 0.6958994774453034,
+                    "west": 0.023382380020851988
                 },
                 "room_025": {
-                    "east": 0.007136306881790247,
-                    "north": 0.057913801237797796,
-                    "south": 0.08506580602750831,
-                    "stay": 0.7610184715834805,
-                    "west": 0.08886561426942317
+                    "east": 0.07295333959432435,
+                    "north": 0.04761884773417916,
+                    "south": 0.0,
+                    "stay": 0.8304294294310153,
+                    "west": 0.04899838324048124
                 },
                 "room_026": {
-                    "east": 0.23592696474113553,
+                    "east": 0.051164010300056746,
                     "north": 0.0,
-                    "south": 0.022459272627462928,
-                    "stay": 0.691762357171735,
-                    "west": 0.04985140545966654
+                    "south": 0.0009193712791453737,
+                    "stay": 0.8068835532964617,
+                    "west": 0.14103306512433622
                 },
                 "room_027": {
                     "east": 0.0,
-                    "north": 0.0,
-                    "south": 0.27155764521716313,
-                    "stay": 0.6114638228902759,
-                    "west": 0.11697853189256095
+                    "north": 0.008612368682383536,
+                    "south": 0.0,
+                    "stay": 0.8048178967058374,
+                    "west": 0.18656973461177911
                 },
                 "room_028": {
-                    "east": 0.0,
-                    "north": 0.04985682335871645,
+                    "east": 0.22540755086243658,
+                    "north": 0.0,
                     "south": 0.0,
-                    "stay": 0.9501431766412836,
+                    "stay": 0.7745924491375634,
                     "west": 0.0
                 },
                 "room_029": {
-                    "east": 0.07915016754802179,
-                    "north": 0.08947028087723669,
+                    "east": 0.03563015927336475,
+                    "north": 0.09679477290653084,
                     "south": 0.0,
-                    "stay": 0.8313795515747415,
-                    "west": 0.0
+                    "stay": 0.7735667464468479,
+                    "west": 0.09400832137325657
                 },
                 "room_030": {
-                    "east": 0.0008214439928311991,
-                    "north": 0.1409486417045254,
+                    "east": 0.0,
+                    "north": 0.14670167314407884,
                     "south": 0.0,
-                    "stay": 0.7043877578982292,
-                    "west": 0.1538421564044142
+                    "stay": 0.8387636841747492,
+                    "west": 0.014534642681171914
                 },
                 "room_031": {
                     "east": 0.0,
-                    "north": 0.10999268631135534,
+                    "north": 0.07562732799005778,
                     "south": 0.0,
-                    "stay": 0.6957410740545973,
-                    "west": 0.1942662396340474
+                    "stay": 0.9243726720099422,
+                    "west": 0.0
                 }
             },
             "ind_007": {
                 "room_000": {
-                    "east": 0.24504399157966272,
+                    "east": 0.18706863058391054,
                     "north": 0.0,
-                    "south": 0.0,
-                    "stay": 0.7549560084203373,
+                    "south": 0.17110135492515047,
+                    "stay": 0.641830014490939,
                     "west": 0.0
                 },
                 "room_001": {
                     "east": 0.0,
                     "north": 0.0,
-                    "south": 0.3877530023502038,
-                    "stay": 0.6109438580642171,
-                    "west": 0.00130313958557906
+                    "south": 0.005600296325695863,
+                    "stay": 0.9601281170709074,
+                    "west": 0.03427158660339674
                 },
                 "room_002": {
-                    "east": 0.09216808152366861,
+                    "east": 0.11759698941366607,
                     "north": 0.0,
-                    "south": 0.13429669957888313,
-                    "stay": 0.7735352188974483,
+                    "south": 0.003720934774488931,
+                    "stay": 0.878682075811845,
                     "west": 0.0
                 },
                 "room_003": {
                     "east": 0.0,
                     "north": 0.0,
-                    "south": 0.2141697646906713,
-                    "stay": 0.7794581042509863,
-                    "west": 0.006372131058342423
+                    "south": 0.26415448534788555,
+                    "stay": 0.6144196878714677,
+                    "west": 0.12142582678064671
                 },
                 "room_004": {
-                    "east": 0.0,
-                    "north": 0.03321647337424716,
-                    "south": 0.030650279214358922,
-                    "stay": 0.9361332474113939,
+                    "east": 0.18889026322852998,
+                    "north": 0.003640780959570989,
+                    "south": 0.0,
+                    "stay": 0.807468955811899,
                     "west": 0.0
                 },
                 "room_005": {
-                    "east": 0.014271119943372313,
-                    "north": 0.0036787074814443937,
-                    "south": 0.06603182237285815,
-                    "stay": 0.9160183502023251,
-                    "west": 0.0
+                    "east": 0.10995853089906947,
+                    "north": 0.1015170830957302,
+                    "south": 0.0,
+                    "stay": 0.6510451499859401,
+                    "west": 0.13747923601926024
                 },
                 "room_006": {
-                    "east": 0.0,
-                    "north": 0.0034577896200464644,
-                    "south": 0.13882119784272098,
-                    "stay": 0.8435283729127672,
-                    "west": 0.014192639624465396
+                    "east": 0.07491248435236021,
+                    "north": 0.0,
+                    "south": 0.15780785864323285,
+                    "stay": 0.7233469206812836,
+                    "west": 0.04393273632312339
                 },
                 "room_007": {
-                    "east": 0.2401459646340289,
+                    "east": 0.13495590259778836,
                     "north": 0.0,
-                    "south": 0.06152029939352758,
-                    "stay": 0.6983337359724435,
-                    "west": 0.0
+                    "south": 0.0,
+                    "stay": 0.8641655766566338,
+                    "west": 0.0008785207455777776
                 },
                 "room_008": {
-                    "east": 0.0010383514086363737,
-                    "north": 0.0,
-                    "south": 0.011794909958802075,
-                    "stay": 0.9754199340743143,
-                    "west": 0.01174680455824729
+                    "east": 0.006700299540768872,
+                    "north": 0.22164346460250026,
+                    "south": 0.03366500698983027,
+                    "stay": 0.7128301827639806,
+                    "west": 0.025161046102920033
                 },
                 "room_009": {
-                    "east": 0.14519399488644508,
-                    "north": 0.2018842659131493,
-                    "south": 0.0023647840177271977,
-                    "stay": 0.6126822921390119,
-                    "west": 0.03787466304366652
+                    "east": 0.0,
+                    "north": 0.11841801767252096,
+                    "south": 0.01195862410929922,
+                    "stay": 0.781243657313894,
+                    "west": 0.08837970090428583
                 },
                 "room_010": {
-                    "east": 0.010193052770766466,
-                    "north": 0.0,
-                    "south": 0.024229971540334752,
-                    "stay": 0.9408343148149285,
-                    "west": 0.024742660873970257
+                    "east": 0.0,
+                    "north": 0.12271723078320555,
+                    "south": 0.006521619008238293,
+                    "stay": 0.8707611502085562,
+                    "west": 0.0
                 },
                 "room_011": {
-                    "east": 0.03861040581071763,
-                    "north": 0.09341392475799692,
-                    "south": 0.024163596150402877,
-                    "stay": 0.8398456211881661,
-                    "west": 0.00396645209271649
+                    "east": 0.17236995096961172,
+                    "north": 0.07788347330322762,
+                    "south": 0.0032451722025426868,
+                    "stay": 0.746501403524618,
+                    "west": 0.0
                 },
                 "room_012": {
                     "east": 0.0,
-                    "north": 0.19524726734695255,
-                    "south": 0.0,
-                    "stay": 0.6445632047757404,
-                    "west": 0.16018952787730711
+                    "north": 0.0009332103157549679,
+                    "south": 0.0009347706229970919,
+                    "stay": 0.939825274071073,
+                    "west": 0.05830674499017497
                 },
                 "room_013": {
-                    "east": 0.07535334303195125,
-                    "north": 0.14587279977370488,
-                    "south": 0.06419659983571557,
-                    "stay": 0.7145772573586283,
+                    "east": 0.00474620274208224,
+                    "north": 0.0,
+                    "south": 0.26864617437301563,
+                    "stay": 0.7266076228849021,
                     "west": 0.0
                 },
                 "room_014": {
-                    "east": 0.0005103166890932016,
-                    "north": 0.0011142180309484308,
-                    "south": 0.0,
-                    "stay": 0.9978338107732505,
-                    "west": 0.0005416545067078607
+                    "east": 0.0683004853571894,
+                    "north": 0.10082691769616253,
+                    "south": 0.1698728373324,
+                    "stay": 0.6530736798613866,
+                    "west": 0.007926079752861352
                 },
                 "room_015": {
-                    "east": 0.02667123283758036,
-                    "north": 0.14225228628495581,
-                    "south": 0.02940828918642661,
-                    "stay": 0.7063038024497721,
-                    "west": 0.0953643892412652
+                    "east": 0.13415975796949764,
+                    "north": 0.0,
+                    "south": 0.02863382447466749,
+                    "stay": 0.6705012783316853,
+                    "west": 0.1667051392241496
                 },
                 "room_016": {
-                    "east": 0.051690430729119594,
-                    "north": 0.05081963377383654,
-                    "south": 0.03727698109555825,
-                    "stay": 0.8566998562535215,
-                    "west": 0.003513098147964088
+                    "east": 0.1343128749900236,
+                    "north": 0.025604347885737382,
+                    "south": 0.0,
+                    "stay": 0.7778435882804617,
+                    "west": 0.06223918884377726
                 },
                 "room_017": {
                     "east": 0.0,
-                    "north": 0.0038861885562618314,
-                    "south": 0.01627282761562993,
-                    "stay": 0.9792079530614525,
-                    "west": 0.0006330307666557686
+                    "north": 0.01976085863124919,
+                    "south": 0.020166049879218467,
+                    "stay": 0.956096142422813,
+                    "west": 0.003976949066719303
                 },
                 "room_018": {
-                    "east": 0.0,
-                    "north": 0.15573545022864355,
-                    "south": 0.1432887400176829,
-                    "stay": 0.7009758097536736,
+                    "east": 0.013236312467350799,
+                    "north": 0.0053841686812985175,
+                    "south": 0.010675982439917764,
+                    "stay": 0.9707035364114329,
                     "west": 0.0
                 },
                 "room_019": {
-                    "east": 0.04021162686741479,
-                    "north": 0.0005784939990171467,
-                    "south": 0.0535961774408217,
-                    "stay": 0.9056137016927464,
-                    "west": 0.0
+                    "east": 0.04642288285709927,
+                    "north": 0.08645486066477404,
+                    "south": 0.045987134544249256,
+                    "stay": 0.6684804283085454,
+                    "west": 0.15265469362533204
                 },
                 "room_020": {
-                    "east": 0.0848449895426118,
-                    "north": 7.595949814498966e-06,
-                    "south": 0.047644773263666854,
-                    "stay": 0.7765147145125548,
-                    "west": 0.09098792673135203
+                    "east": 0.0,
+                    "north": 0.007952917181445062,
+                    "south": 0.017542042074949093,
+                    "stay": 0.9464395359351416,
+                    "west": 0.02806550480846422
                 },
                 "room_021": {
                     "east": 0.0,
-                    "north": 0.20778486749031705,
-                    "south": 0.012399847076449337,
-                    "stay": 0.7786326301611127,
-                    "west": 0.0011826552721209084
+                    "north": 0.05937148435368321,
+                    "south": 0.10515441019433146,
+                    "stay": 0.8354741054519853,
+                    "west": 0.0
                 },
                 "room_022": {
-                    "east": 0.0,
-                    "north": 0.3889523520350794,
-                    "south": 0.0,
-                    "stay": 0.6110476479649206,
+                    "east": 0.26307247058423916,
+                    "north": 0.0,
+                    "south": 0.05525969148052286,
+                    "stay": 0.681667837935238,
                     "west": 0.0
                 },
                 "room_023": {
-                    "east": 0.04223939444884659,
-                    "north": 0.006427423052484418,
-                    "south": 0.03163386505447647,
-                    "stay": 0.9196993174441925,
-                    "west": 0.0
+                    "east": 0.021479979673536622,
+                    "north": 0.012692297711007583,
+                    "south": 0.013487841160471496,
+                    "stay": 0.9434150304137956,
+                    "west": 0.008924851041188706
                 },
                 "room_024": {
-                    "east": 0.0011483993281621314,
-                    "north": 0.019408476019286868,
+                    "east": 0.03607411209872183,
+                    "north": 0.046402571962571755,
                     "south": 0.0,
-                    "stay": 0.9691088018791635,
-                    "west": 0.010334322773387512
+                    "stay": 0.9168548132548076,
+                    "west": 0.0006685026838988584
                 },
                 "room_025": {
-                    "east": 0.03496536252877691,
-                    "north": 0.026021978815380868,
-                    "south": 0.03754504256168828,
-                    "stay": 0.8650201680768778,
-                    "west": 0.03644744801727618
+                    "east": 0.0001398530713362388,
+                    "north": 0.01932463858105757,
+                    "south": 0.0,
+                    "stay": 0.835744398278465,
+                    "west": 0.14479111006914117
                 },
                 "room_026": {
-                    "east": 0.07174589524707702,
+                    "east": 0.13427747418018918,
                     "north": 0.0,
-                    "south": 0.1625749868423789,
-                    "stay": 0.722242214901226,
-                    "west": 0.04343690300931811
+                    "south": 0.0881978513294412,
+                    "stay": 0.777033114606813,
+                    "west": 0.0004915598835566196
                 },
                 "room_027": {
                     "east": 0.0,
-                    "north": 0.0,
-                    "south": 0.09577127169026915,
-                    "stay": 0.7957672627427326,
-                    "west": 0.10846146556699827
+                    "north": 0.11529275811782003,
+                    "south": 0.0,
+                    "stay": 0.6700965588901202,
+                    "west": 0.21461068299205976
                 },
                 "room_028": {
-                    "east": 0.0,
-                    "north": 0.2023226326537739,
+                    "east": 0.049524299676397376,
+                    "north": 0.0,
                     "south": 0.0,
-                    "stay": 0.7976773673462261,
+                    "stay": 0.9504757003236026,
                     "west": 0.0
                 },
                 "room_029": {
-                    "east": 0.024667213585113618,
-                    "north": 0.007250391411754512,
+                    "east": 0.0360495313543177,
+                    "north": 0.020314341282586048,
                     "south": 0.0,
-                    "stay": 0.9680823950031319,
-                    "west": 0.0
+                    "stay": 0.9264352900176407,
+                    "west": 0.017200837345455557
                 },
                 "room_030": {
-                    "east": 0.03146163817842545,
-                    "north": 0.1925472057715087,
+                    "east": 0.0,
+                    "north": 0.15465924492751112,
                     "south": 0.0,
-                    "stay": 0.6189008784145803,
-                    "west": 0.1570902776354856
+                    "stay": 0.6357780715159181,
+                    "west": 0.20956268355657073
                 },
                 "room_031": {
                     "east": 0.0,
-                    "north": 0.12398729807943432,
+                    "north": 0.03796896536669525,
                     "south": 0.0,
-                    "stay": 0.6790382495246609,
-                    "west": 0.19697445239590483
+                    "stay": 0.9620310346333047,
+                    "west": 0.0
                 }
             }
         },
         "static": {
             "sta_000": null,
             "sta_001": null,
             "sta_002": null,
@@ -2932,296 +2932,296 @@
             "sta_007": null
         }
     },
     "room_config": {
         "room_000": {
             "east": "room_001",
             "north": "wall",
-            "south": "wall",
+            "south": "room_004",
             "west": "wall"
         },
         "room_001": {
             "east": "wall",
             "north": "wall",
-            "south": "room_004",
+            "south": "room_005",
             "west": "room_000"
         },
         "room_002": {
             "east": "room_003",
             "north": "wall",
-            "south": "room_005",
+            "south": "room_008",
             "west": "wall"
         },
         "room_003": {
             "east": "wall",
             "north": "wall",
-            "south": "room_006",
+            "south": "room_009",
             "west": "room_002"
         },
         "room_004": {
-            "east": "wall",
-            "north": "room_001",
-            "south": "room_009",
+            "east": "room_005",
+            "north": "room_000",
+            "south": "wall",
             "west": "wall"
         },
         "room_005": {
             "east": "room_006",
-            "north": "room_002",
-            "south": "room_011",
-            "west": "wall"
+            "north": "room_001",
+            "south": "wall",
+            "west": "room_004"
         },
         "room_006": {
-            "east": "wall",
-            "north": "room_003",
-            "south": "room_012",
+            "east": "room_007",
+            "north": "wall",
+            "south": "room_010",
             "west": "room_005"
         },
         "room_007": {
             "east": "room_008",
             "north": "wall",
-            "south": "room_013",
-            "west": "wall"
+            "south": "wall",
+            "west": "room_006"
         },
         "room_008": {
             "east": "room_009",
-            "north": "wall",
-            "south": "room_014",
+            "north": "room_002",
+            "south": "room_011",
             "west": "room_007"
         },
         "room_009": {
-            "east": "room_010",
-            "north": "room_004",
-            "south": "room_015",
+            "east": "wall",
+            "north": "room_003",
+            "south": "room_012",
             "west": "room_008"
         },
         "room_010": {
-            "east": "room_011",
-            "north": "wall",
-            "south": "room_016",
-            "west": "room_009"
+            "east": "wall",
+            "north": "room_006",
+            "south": "room_014",
+            "west": "wall"
         },
         "room_011": {
             "east": "room_012",
-            "north": "room_005",
-            "south": "room_017",
-            "west": "room_010"
+            "north": "room_008",
+            "south": "room_016",
+            "west": "wall"
         },
         "room_012": {
             "east": "wall",
-            "north": "room_006",
-            "south": "wall",
+            "north": "room_009",
+            "south": "room_017",
             "west": "room_011"
         },
         "room_013": {
             "east": "room_014",
-            "north": "room_007",
+            "north": "wall",
             "south": "room_018",
             "west": "wall"
         },
         "room_014": {
             "east": "room_015",
-            "north": "room_008",
-            "south": "wall",
+            "north": "room_010",
+            "south": "room_019",
             "west": "room_013"
         },
         "room_015": {
             "east": "room_016",
-            "north": "room_009",
-            "south": "room_019",
+            "north": "wall",
+            "south": "room_020",
             "west": "room_014"
         },
         "room_016": {
             "east": "room_017",
-            "north": "room_010",
-            "south": "room_020",
+            "north": "room_011",
+            "south": "wall",
             "west": "room_015"
         },
         "room_017": {
             "east": "wall",
-            "north": "room_011",
+            "north": "room_012",
             "south": "room_021",
             "west": "room_016"
         },
         "room_018": {
-            "east": "wall",
+            "east": "room_019",
             "north": "room_013",
-            "south": "room_022",
+            "south": "room_023",
             "west": "wall"
         },
         "room_019": {
             "east": "room_020",
-            "north": "room_015",
-            "south": "room_023",
-            "west": "wall"
+            "north": "room_014",
+            "south": "room_024",
+            "west": "room_018"
         },
         "room_020": {
-            "east": "room_021",
-            "north": "room_016",
-            "south": "room_024",
+            "east": "wall",
+            "north": "room_015",
+            "south": "room_025",
             "west": "room_019"
         },
         "room_021": {
             "east": "wall",
             "north": "room_017",
-            "south": "room_025",
-            "west": "room_020"
+            "south": "room_027",
+            "west": "wall"
         },
         "room_022": {
-            "east": "wall",
-            "north": "room_018",
-            "south": "wall",
+            "east": "room_023",
+            "north": "wall",
+            "south": "room_029",
             "west": "wall"
         },
         "room_023": {
             "east": "room_024",
-            "north": "room_019",
-            "south": "room_028",
-            "west": "wall"
+            "north": "room_018",
+            "south": "room_030",
+            "west": "room_022"
         },
         "room_024": {
             "east": "room_025",
-            "north": "room_020",
+            "north": "room_019",
             "south": "wall",
             "west": "room_023"
         },
         "room_025": {
             "east": "room_026",
-            "north": "room_021",
-            "south": "room_029",
+            "north": "room_020",
+            "south": "wall",
             "west": "room_024"
         },
         "room_026": {
             "east": "room_027",
             "north": "wall",
-            "south": "room_030",
+            "south": "room_031",
             "west": "room_025"
         },
         "room_027": {
             "east": "wall",
-            "north": "wall",
-            "south": "room_031",
+            "north": "room_021",
+            "south": "wall",
             "west": "room_026"
         },
         "room_028": {
-            "east": "wall",
-            "north": "room_023",
+            "east": "room_029",
+            "north": "wall",
             "south": "wall",
             "west": "wall"
         },
         "room_029": {
             "east": "room_030",
-            "north": "room_025",
+            "north": "room_022",
             "south": "wall",
-            "west": "wall"
+            "west": "room_028"
         },
         "room_030": {
-            "east": "room_031",
-            "north": "room_026",
+            "east": "wall",
+            "north": "room_023",
             "south": "wall",
             "west": "room_029"
         },
         "room_031": {
             "east": "wall",
-            "north": "room_027",
+            "north": "room_026",
             "south": "wall",
-            "west": "room_030"
+            "west": "wall"
         }
     },
     "room_indexes": [
         [
             0,
             1
         ],
         [
             0,
             2
         ],
         [
             0,
-            4
+            5
         ],
         [
             0,
-            5
+            6
         ],
         [
             1,
-            2
+            1
         ],
         [
             1,
-            4
+            2
         ],
         [
             1,
-            5
+            3
         ],
         [
-            2,
-            0
+            1,
+            4
         ],
         [
-            2,
-            1
+            1,
+            5
         ],
         [
-            2,
-            2
+            1,
+            6
         ],
         [
             2,
             3
         ],
         [
             2,
-            4
+            5
         ],
         [
             2,
-            5
+            6
         ],
         [
             3,
-            0
+            2
         ],
         [
             3,
-            1
+            3
         ],
         [
             3,
-            2
+            4
         ],
         [
             3,
-            3
+            5
         ],
         [
             3,
-            4
-        ],
-        [
-            4,
-            0
+            6
         ],
         [
             4,
             2
         ],
         [
             4,
             3
         ],
         [
             4,
             4
         ],
         [
+            4,
+            6
+        ],
+        [
             5,
-            0
+            1
         ],
         [
             5,
             2
         ],
         [
             5,
@@ -3237,23 +3237,23 @@
         ],
         [
             5,
             6
         ],
         [
             6,
-            2
+            0
         ],
         [
             6,
-            4
+            1
         ],
         [
             6,
-            5
+            2
         ],
         [
             6,
-            6
+            5
         ]
     ]
 }
```

### Comparing `room_env-1.0.3/room_env/data/room-config-xs-v2.json` & `room_env-2.0.0/room_env/data/room-config-xs-v2.json`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/data/room-config-xxs-v2.json` & `room_env-2.0.0/room_env/data/room-config-xxs-v2.json`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/data/semantic-knowledge-small.json` & `room_env-2.0.0/room_env/data/semantic-knowledge-small.json`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/data/semantic-knowledge.json` & `room_env-2.0.0/room_env/data/semantic-knowledge.json`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/des.py` & `room_env-2.0.0/room_env/des.py`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/envs/room0.py` & `room_env-2.0.0/room_env/envs/room0.py`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/envs/room1.py` & `room_env-2.0.0/room_env/envs/room1.py`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env/envs/room2.py` & `room_env-2.0.0/room_env/envs/room2.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,17 +68,15 @@
 
         assert (
             self.question_prob >= 0 and self.question_prob <= 1
         ), f"question_prob must be between 0 and 1, but it's {self.question_prob}"
 
         # place an object in one of the rooms when it is created.
         if self.deterministic:
-            self.location = sample_max_value_key(
-                self.init_probs, keys_to_exclude=["stay"]
-            )
+            self.location = sample_max_value_key(self.init_probs)
 
         else:
             self.location = random.choices(
                 list(self.init_probs.keys()),
                 weights=list(self.init_probs.values()),
                 k=1,
             )[0]
@@ -146,33 +144,35 @@
 class StaticObject(Object):
     def __init__(
         self,
         name: str,
         init_probs: dict,
         transition_probs: dict,
         question_prob: float,
+        deterministic: bool,
     ) -> None:
         """Static object does not move. Once they are initialized, they stay forever.
 
 
         Args:
             name: e.g., bed
             init_probs: initial probabilities of being in a room
             transition_probs: just a place holder. It's not gonna be used anyway.
             question_prob: the probability of a question being asked at every
                 observation
+            deterministic: whether the object is deterministic.
 
         """
         super().__init__(
             name,
             "static",
             init_probs,
             transition_probs,
             question_prob,
-            deterministic=True,
+            deterministic=deterministic,
         )
         assert self.transition_probs is None, "Static objects do not move."
 
     def __repr__(self) -> str:
         return super().__repr__() + ")"
 
 
@@ -569,14 +569,15 @@
         for name, init_probs in self.object_init_config["static"].items():
             self.objects["static"].append(
                 StaticObject(
                     name,
                     init_probs,
                     self.object_transition_config["static"][name],
                     self.object_question_probs["static"][name],
+                    self.deterministic_objects,
                 )
             )
 
         for name, init_probs in self.object_init_config["independent"].items():
             self.objects["independent"].append(
                 IndepdentObject(
                     name,
```

### Comparing `room_env-1.0.3/room_env/utils.py` & `room_env-2.0.0/room_env/utils.py`

 * *Files identical despite different names*

### Comparing `room_env-1.0.3/room_env.egg-info/PKG-INFO` & `room_env-2.0.0/room_env.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: room-env
-Version: 1.0.3
+Version: 2.0.0
 Summary: The Room environment
 Home-page: https://github.com/humemai/room-env
 Author: Taewoon Kim
 Author-email: info@humem.ai
 Project-URL: Bug Tracker, https://github.com/humemai/room-env/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `room_env-1.0.3/room_env.egg-info/SOURCES.txt` & `room_env-2.0.0/room_env.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 room_env/data/human-locations
 room_env/data/human-names
 room_env/data/ms-coco-80-categories
 room_env/data/names-v2.json
 room_env/data/room-config-dev-v2.json
 room_env/data/room-config-foo-v2.json
 room_env/data/room-config-l-v2.json
-room_env/data/room-config-l2-v2.json
 room_env/data/room-config-m-v2.json
 room_env/data/room-config-s-v2.json
 room_env/data/room-config-xl-v2.json
 room_env/data/room-config-xs-v2.json
 room_env/data/room-config-xxl-v2.json
 room_env/data/room-config-xxs-v2.json
 room_env/data/semantic-knowledge-small.json
```

### Comparing `room_env-1.0.3/setup.cfg` & `room_env-2.0.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = room_env
-version = 1.0.3
+version = 2.0.0
 author = Taewoon Kim
 author_email = info@humem.ai
 description = The Room environment
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/humemai/room-env
 project_urls =
```

### Comparing `room_env-1.0.3/test/test_utils.py` & `room_env-2.0.0/test/test_utils.py`

 * *Files identical despite different names*

