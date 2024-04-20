# Comparing `tmp/autonomous_app-0.2.5.tar.gz` & `tmp/autonomous_app-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomous_app-0.2.5.tar", last modified: Fri Apr 19 20:02:57 2024, max compression
+gzip compressed data, was "autonomous_app-0.2.6.tar", last modified: Sat Apr 20 17:25:24 2024, max compression
```

## Comparing `autonomous_app-0.2.5.tar` & `autonomous_app-0.2.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.982425 autonomous_app-0.2.5/
--rw-r--r--   0 root         (0) root         (0)     1076 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4227 2024-04-19 20:02:57.982425 autonomous_app-0.2.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2008 2024-02-28 15:34:22.000000 autonomous_app-0.2.5/README.md
--rw-r--r--   0 root         (0) root         (0)     1321 2024-04-16 15:28:50.000000 autonomous_app-0.2.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      521 2024-04-17 20:37:08.000000 autonomous_app-0.2.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 20:02:57.982425 autonomous_app-0.2.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.974424 autonomous_app-0.2.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.978424 autonomous_app-0.2.5/src/autonomous/
--rw-r--r--   0 root         (0) root         (0)       86 2024-04-19 20:02:41.000000 autonomous_app-0.2.5/src/autonomous/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.978424 autonomous_app-0.2.5/src/autonomous/ai/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 19:48:34.000000 autonomous_app-0.2.5/src/autonomous/ai/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7128 2024-04-19 19:59:58.000000 autonomous_app-0.2.5/src/autonomous/ai/oaiagent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.978424 autonomous_app-0.2.5/src/autonomous/auth/
--rw-r--r--   0 root         (0) root         (0)      161 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3574 2024-02-20 18:09:54.000000 autonomous_app-0.2.5/src/autonomous/auth/autoauth.py
--rw-r--r--   0 root         (0) root         (0)      886 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/auth/github.py
--rw-r--r--   0 root         (0) root         (0)     1049 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/auth/google.py
--rw-r--r--   0 root         (0) root         (0)     2174 2024-03-30 04:51:47.000000 autonomous_app-0.2.5/src/autonomous/auth/user.py
--rw-r--r--   0 root         (0) root         (0)       42 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.978424 autonomous_app-0.2.5/src/autonomous/db/
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2376 2024-03-20 18:44:15.000000 autonomous_app-0.2.5/src/autonomous/db/autodb.py
--rw-r--r--   0 root         (0) root         (0)     4581 2024-02-26 19:40:28.000000 autonomous_app-0.2.5/src/autonomous/db/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.978424 autonomous_app-0.2.5/src/autonomous/errors/
--rw-r--r--   0 root         (0) root         (0)       59 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/errors/__init__.py
--rw-r--r--   0 root         (0) root         (0)      321 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/errors/danglingreferenceerror.py
--rw-r--r--   0 root         (0) root         (0)     1844 2024-04-18 14:33:06.000000 autonomous_app-0.2.5/src/autonomous/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.978424 autonomous_app-0.2.5/src/autonomous/model/
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)      588 2024-02-20 20:56:13.000000 autonomous_app-0.2.5/src/autonomous/model/autoattribute.py
--rw-r--r--   0 root         (0) root         (0)    11214 2024-04-11 16:19:39.000000 autonomous_app-0.2.5/src/autonomous/model/automodel.py
--rw-r--r--   0 root         (0) root         (0)     2521 2024-03-30 05:04:37.000000 autonomous_app-0.2.5/src/autonomous/model/orm.py
--rw-r--r--   0 root         (0) root         (0)     2939 2024-03-24 18:25:01.000000 autonomous_app-0.2.5/src/autonomous/model/serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.978424 autonomous_app-0.2.5/src/autonomous/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 19:48:54.000000 autonomous_app-0.2.5/src/autonomous/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3966 2024-04-17 14:41:12.000000 autonomous_app-0.2.5/src/autonomous/storage/imagestorage.py
--rw-r--r--   0 root         (0) root         (0)     2286 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/storage/localstorage.py
--rw-r--r--   0 root         (0) root         (0)     2153 2024-04-17 21:07:33.000000 autonomous_app-0.2.5/src/autonomous/storage/markdown.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.982425 autonomous_app-0.2.5/src/autonomous/storage/version_control/
--rw-r--r--   0 root         (0) root         (0)     1069 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/storage/version_control/GHCallbacks.py
--rw-r--r--   0 root         (0) root         (0)     1155 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/storage/version_control/GHOrganization.py
--rw-r--r--   0 root         (0) root         (0)     4622 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/storage/version_control/GHRepo.py
--rw-r--r--   0 root         (0) root         (0)      196 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/storage/version_control/GHVersionControl.py
--rw-r--r--   0 root         (0) root         (0)      117 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/storage/version_control/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.982425 autonomous_app-0.2.5/src/autonomous/tasks/
--rw-r--r--   0 root         (0) root         (0)       32 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4910 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/tasks/autotask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.982425 autonomous_app-0.2.5/src/autonomous_app.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4227 2024-04-19 20:02:57.000000 autonomous_app-0.2.5/src/autonomous_app.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1372 2024-04-19 20:02:57.000000 autonomous_app-0.2.5/src/autonomous_app.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 20:02:57.000000 autonomous_app-0.2.5/src/autonomous_app.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      166 2024-04-19 20:02:57.000000 autonomous_app-0.2.5/src/autonomous_app.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-19 20:02:57.000000 autonomous_app-0.2.5/src/autonomous_app.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 17:25:24.014603 autonomous_app-0.2.6/
+-rw-r--r--   0 root         (0) root         (0)     1076 2024-02-14 21:26:11.000000 autonomous_app-0.2.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4227 2024-04-20 17:25:24.014603 autonomous_app-0.2.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-02-28 15:34:22.000000 autonomous_app-0.2.6/README.md
+-rw-r--r--   0 root         (0) root         (0)     1321 2024-04-16 15:28:50.000000 autonomous_app-0.2.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      521 2024-04-17 20:37:08.000000 autonomous_app-0.2.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 17:25:24.014603 autonomous_app-0.2.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-02-14 21:26:11.000000 autonomous_app-0.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 17:25:24.010602 autonomous_app-0.2.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 17:25:24.010602 autonomous_app-0.2.6/src/autonomous/
+-rw-r--r--   0 root         (0) root         (0)       86 2024-04-20 17:25:06.000000 autonomous_app-0.2.6/src/autonomous/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 17:25:24.010602 autonomous_app-0.2.6/src/autonomous/ai/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 19:48:34.000000 autonomous_app-0.2.6/src/autonomous/ai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7128 2024-04-19 19:59:58.000000 autonomous_app-0.2.6/src/autonomous/ai/oaiagent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 17:25:24.010602 autonomous_app-0.2.6/src/autonomous/auth/
+-rw-r--r--   0 root         (0) root         (0)      161 2024-02-14 21:26:11.000000 autonomous_app-0.2.6/src/autonomous/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3574 2024-02-20 18:09:54.000000 autonomous_app-0.2.6/src/autonomous/auth/autoauth.py
+-rw-r--r--   0 root         (0) root         (0)      886 2024-02-14 21:26:11.000000 autonomous_app-0.2.6/src/autonomous/auth/github.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2024-02-14 21:26:11.000000 autonomous_app-0.2.6/src/autonomous/auth/google.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2024-03-30 04:51:47.000000 autonomous_app-0.2.6/src/autonomous/auth/user.py
+-rw-r--r--   0 root         (0) root         (0)       42 2024-02-14 21:26:11.000000 autonomous_app-0.2.6/src/autonomous/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 17:25:24.010602 autonomous_app-0.2.6/src/autonomous/db/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 21:26:11.000000 autonomous_app-0.2.6/src/autonomous/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2024-03-20 18:44:15.000000 autonomous_app-0.2.6/src/autonomous/db/autodb.py
+-rw-r--r--   0 root         (0) root         (0)     4633 2024-04-20 17:24:06.000000 autonomous_app-0.2.6/src/autonomous/db/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 17:25:24.010602 autonomous_app-0.2.6/src/autonomous/errors/
+-rw-r--r--   0 root         (0) root         (0)       59 2024-02-14 21:26:11.000000 autonomous_app-0.2.6/src/autonomous/errors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      321 2024-02-14 21:26:11.000000 autonomous_app-0.2.6/src/autonomous/errors/danglingreferenceerror.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2024-04-18 14:33:06.000000 autonomous_app-0.2.6/src/autonomous/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 17:25:24.014603 autonomous_app-0.2.6/src/autonomous/model/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 21:26:11.000000 autonomous_app-0.2.6/src/autonomous/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      588 2024-02-20 20:56:13.000000 autonomous_app-0.2.6/src/autonomous/model/autoattribute.py
+-rw-r--r--   0 root         (0) root         (0)    11296 2024-04-20 17:24:46.000000 autonomous_app-0.2.6/src/autonomous/model/automodel.py
+-rw-r--r--   0 root         (0) root         (0)     2521 2024-03-30 05:04:37.000000 autonomous_app-0.2.6/src/autonomous/model/orm.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2024-03-24 18:25:01.000000 autonomous_app-0.2.6/src/autonomous/model/serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 17:25:24.014603 autonomous_app-0.2.6/src/autonomous/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 19:48:54.000000 autonomous_app-0.2.6/src/autonomous/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3966 2024-04-17 14:41:12.000000 autonomous_app-0.2.6/src/autonomous/storage/imagestorage.py
+-rw-r--r--   0 root         (0) root         (0)     2286 2024-02-14 21:26:11.000000 autonomous_app-0.2.6/src/autonomous/storage/localstorage.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2024-04-17 21:07:33.000000 autonomous_app-0.2.6/src/autonomous/storage/markdown.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 17:25:24.014603 autonomous_app-0.2.6/src/autonomous/storage/version_control/
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-02-14 21:26:11.000000 autonomous_app-0.2.6/src/autonomous/storage/version_control/GHCallbacks.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-02-14 21:26:11.000000 autonomous_app-0.2.6/src/autonomous/storage/version_control/GHOrganization.py
+-rw-r--r--   0 root         (0) root         (0)     4622 2024-02-14 21:26:11.000000 autonomous_app-0.2.6/src/autonomous/storage/version_control/GHRepo.py
+-rw-r--r--   0 root         (0) root         (0)      196 2024-02-14 21:26:11.000000 autonomous_app-0.2.6/src/autonomous/storage/version_control/GHVersionControl.py
+-rw-r--r--   0 root         (0) root         (0)      117 2024-02-14 21:26:11.000000 autonomous_app-0.2.6/src/autonomous/storage/version_control/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 17:25:24.014603 autonomous_app-0.2.6/src/autonomous/tasks/
+-rw-r--r--   0 root         (0) root         (0)       32 2024-02-14 21:26:11.000000 autonomous_app-0.2.6/src/autonomous/tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4910 2024-02-14 21:26:11.000000 autonomous_app-0.2.6/src/autonomous/tasks/autotask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 17:25:24.014603 autonomous_app-0.2.6/src/autonomous_app.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4227 2024-04-20 17:25:23.000000 autonomous_app-0.2.6/src/autonomous_app.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1372 2024-04-20 17:25:24.000000 autonomous_app-0.2.6/src/autonomous_app.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 17:25:23.000000 autonomous_app-0.2.6/src/autonomous_app.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2024-04-20 17:25:23.000000 autonomous_app-0.2.6/src/autonomous_app.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-20 17:25:23.000000 autonomous_app-0.2.6/src/autonomous_app.egg-info/top_level.txt
```

### Comparing `autonomous_app-0.2.5/LICENSE` & `autonomous_app-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.5/PKG-INFO` & `autonomous_app-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.2.5
+Version: 0.2.6
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autonomous_app-0.2.5/README.md` & `autonomous_app-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.5/pyproject.toml` & `autonomous_app-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.5/requirements.txt` & `autonomous_app-0.2.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.5/src/autonomous/ai/oaiagent.py` & `autonomous_app-0.2.6/src/autonomous/ai/oaiagent.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.5/src/autonomous/auth/autoauth.py` & `autonomous_app-0.2.6/src/autonomous/auth/autoauth.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.5/src/autonomous/auth/github.py` & `autonomous_app-0.2.6/src/autonomous/auth/github.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.5/src/autonomous/auth/google.py` & `autonomous_app-0.2.6/src/autonomous/auth/google.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.5/src/autonomous/auth/user.py` & `autonomous_app-0.2.6/src/autonomous/auth/user.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.5/src/autonomous/db/autodb.py` & `autonomous_app-0.2.6/src/autonomous/db/autodb.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.5/src/autonomous/db/table.py` & `autonomous_app-0.2.6/src/autonomous/db/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,24 +98,26 @@
                     dot_notation[f"{prefix}{key}"] = {"$regex": value, "$options": "i"}
                 else:
                     dot_notation[f"{prefix}{key}"] = value
         return dot_notation
 
     def find(self, **search_terms):
         search_terms = self._convert_to_dot_notation(search_terms)
+        log(search_terms)
         result = self._db.find_one(search_terms)
         if result:
             result["_id"] = str(result["_id"])
             return result
 
     def search(self, **search_terms):
         fuzzy_search = search_terms.pop("_FUZZY_SEARCH", False)
         search_terms = self._convert_to_dot_notation(
             search_terms, fuzzy_search=fuzzy_search
         )
+        log(search_terms)
         result = self._db.find(search_terms) or []
 
         objs = []
         for o in result:
             o["_id"] = str(o["_id"])
             objs.append(o)
         # log(search_terms, fuzzy_search, objs)
```

### Comparing `autonomous_app-0.2.5/src/autonomous/logger.py` & `autonomous_app-0.2.6/src/autonomous/logger.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.5/src/autonomous/model/autoattribute.py` & `autonomous_app-0.2.6/src/autonomous/model/autoattribute.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.5/src/autonomous/model/automodel.py` & `autonomous_app-0.2.6/src/autonomous/model/automodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,14 +332,16 @@
 
         Args:
             **kwargs: Keyword arguments to search for (dict).
 
         Returns:
             AutoModel or None: The first matching AutoModel instance, or None if not found.
         """
+        for k, v in kwargs.items():
+            kwargs[k] = AutoEncoder.encode(v)
         attribs = cls.table().find(**kwargs)
         return cls(**attribs) if attribs else None
 
     def delete(self):
         """
         Delete this model from the database.
         """
```

### Comparing `autonomous_app-0.2.5/src/autonomous/model/orm.py` & `autonomous_app-0.2.6/src/autonomous/model/orm.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.5/src/autonomous/model/serializer.py` & `autonomous_app-0.2.6/src/autonomous/model/serializer.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.5/src/autonomous/storage/imagestorage.py` & `autonomous_app-0.2.6/src/autonomous/storage/imagestorage.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.5/src/autonomous/storage/localstorage.py` & `autonomous_app-0.2.6/src/autonomous/storage/localstorage.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.5/src/autonomous/storage/markdown.py` & `autonomous_app-0.2.6/src/autonomous/storage/markdown.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.5/src/autonomous/storage/version_control/GHCallbacks.py` & `autonomous_app-0.2.6/src/autonomous/storage/version_control/GHCallbacks.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.5/src/autonomous/storage/version_control/GHOrganization.py` & `autonomous_app-0.2.6/src/autonomous/storage/version_control/GHOrganization.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.5/src/autonomous/storage/version_control/GHRepo.py` & `autonomous_app-0.2.6/src/autonomous/storage/version_control/GHRepo.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.5/src/autonomous/tasks/autotask.py` & `autonomous_app-0.2.6/src/autonomous/tasks/autotask.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.5/src/autonomous_app.egg-info/PKG-INFO` & `autonomous_app-0.2.6/src/autonomous_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.2.5
+Version: 0.2.6
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autonomous_app-0.2.5/src/autonomous_app.egg-info/SOURCES.txt` & `autonomous_app-0.2.6/src/autonomous_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

