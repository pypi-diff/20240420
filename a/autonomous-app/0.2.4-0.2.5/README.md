# Comparing `tmp/autonomous_app-0.2.4.tar.gz` & `tmp/autonomous_app-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomous_app-0.2.4.tar", last modified: Fri Apr 19 19:25:47 2024, max compression
+gzip compressed data, was "autonomous_app-0.2.5.tar", last modified: Fri Apr 19 20:02:57 2024, max compression
```

## Comparing `autonomous_app-0.2.4.tar` & `autonomous_app-0.2.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 19:25:47.231950 autonomous_app-0.2.4/
--rw-r--r--   0 root         (0) root         (0)     1076 2024-02-14 21:26:11.000000 autonomous_app-0.2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4227 2024-04-19 19:25:47.231950 autonomous_app-0.2.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2008 2024-02-28 15:34:22.000000 autonomous_app-0.2.4/README.md
--rw-r--r--   0 root         (0) root         (0)     1321 2024-04-16 15:28:50.000000 autonomous_app-0.2.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      521 2024-04-17 20:37:08.000000 autonomous_app-0.2.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 19:25:47.231950 autonomous_app-0.2.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-14 21:26:11.000000 autonomous_app-0.2.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 19:25:47.223950 autonomous_app-0.2.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 19:25:47.227950 autonomous_app-0.2.4/src/autonomous/
--rw-r--r--   0 root         (0) root         (0)       86 2024-04-19 19:25:27.000000 autonomous_app-0.2.4/src/autonomous/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 19:25:47.227950 autonomous_app-0.2.4/src/autonomous/ai/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 19:48:34.000000 autonomous_app-0.2.4/src/autonomous/ai/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7194 2024-04-19 19:23:59.000000 autonomous_app-0.2.4/src/autonomous/ai/oaiagent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 19:25:47.227950 autonomous_app-0.2.4/src/autonomous/auth/
--rw-r--r--   0 root         (0) root         (0)      161 2024-02-14 21:26:11.000000 autonomous_app-0.2.4/src/autonomous/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3574 2024-02-20 18:09:54.000000 autonomous_app-0.2.4/src/autonomous/auth/autoauth.py
--rw-r--r--   0 root         (0) root         (0)      886 2024-02-14 21:26:11.000000 autonomous_app-0.2.4/src/autonomous/auth/github.py
--rw-r--r--   0 root         (0) root         (0)     1049 2024-02-14 21:26:11.000000 autonomous_app-0.2.4/src/autonomous/auth/google.py
--rw-r--r--   0 root         (0) root         (0)     2174 2024-03-30 04:51:47.000000 autonomous_app-0.2.4/src/autonomous/auth/user.py
--rw-r--r--   0 root         (0) root         (0)       42 2024-02-14 21:26:11.000000 autonomous_app-0.2.4/src/autonomous/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 19:25:47.227950 autonomous_app-0.2.4/src/autonomous/db/
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 21:26:11.000000 autonomous_app-0.2.4/src/autonomous/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2376 2024-03-20 18:44:15.000000 autonomous_app-0.2.4/src/autonomous/db/autodb.py
--rw-r--r--   0 root         (0) root         (0)     4581 2024-02-26 19:40:28.000000 autonomous_app-0.2.4/src/autonomous/db/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 19:25:47.227950 autonomous_app-0.2.4/src/autonomous/errors/
--rw-r--r--   0 root         (0) root         (0)       59 2024-02-14 21:26:11.000000 autonomous_app-0.2.4/src/autonomous/errors/__init__.py
--rw-r--r--   0 root         (0) root         (0)      321 2024-02-14 21:26:11.000000 autonomous_app-0.2.4/src/autonomous/errors/danglingreferenceerror.py
--rw-r--r--   0 root         (0) root         (0)     1844 2024-04-18 14:33:06.000000 autonomous_app-0.2.4/src/autonomous/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 19:25:47.227950 autonomous_app-0.2.4/src/autonomous/model/
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 21:26:11.000000 autonomous_app-0.2.4/src/autonomous/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)      588 2024-02-20 20:56:13.000000 autonomous_app-0.2.4/src/autonomous/model/autoattribute.py
--rw-r--r--   0 root         (0) root         (0)    11214 2024-04-11 16:19:39.000000 autonomous_app-0.2.4/src/autonomous/model/automodel.py
--rw-r--r--   0 root         (0) root         (0)     2521 2024-03-30 05:04:37.000000 autonomous_app-0.2.4/src/autonomous/model/orm.py
--rw-r--r--   0 root         (0) root         (0)     2939 2024-03-24 18:25:01.000000 autonomous_app-0.2.4/src/autonomous/model/serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 19:25:47.227950 autonomous_app-0.2.4/src/autonomous/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 19:48:54.000000 autonomous_app-0.2.4/src/autonomous/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3966 2024-04-17 14:41:12.000000 autonomous_app-0.2.4/src/autonomous/storage/imagestorage.py
--rw-r--r--   0 root         (0) root         (0)     2286 2024-02-14 21:26:11.000000 autonomous_app-0.2.4/src/autonomous/storage/localstorage.py
--rw-r--r--   0 root         (0) root         (0)     2153 2024-04-17 21:07:33.000000 autonomous_app-0.2.4/src/autonomous/storage/markdown.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 19:25:47.227950 autonomous_app-0.2.4/src/autonomous/storage/version_control/
--rw-r--r--   0 root         (0) root         (0)     1069 2024-02-14 21:26:11.000000 autonomous_app-0.2.4/src/autonomous/storage/version_control/GHCallbacks.py
--rw-r--r--   0 root         (0) root         (0)     1155 2024-02-14 21:26:11.000000 autonomous_app-0.2.4/src/autonomous/storage/version_control/GHOrganization.py
--rw-r--r--   0 root         (0) root         (0)     4622 2024-02-14 21:26:11.000000 autonomous_app-0.2.4/src/autonomous/storage/version_control/GHRepo.py
--rw-r--r--   0 root         (0) root         (0)      196 2024-02-14 21:26:11.000000 autonomous_app-0.2.4/src/autonomous/storage/version_control/GHVersionControl.py
--rw-r--r--   0 root         (0) root         (0)      117 2024-02-14 21:26:11.000000 autonomous_app-0.2.4/src/autonomous/storage/version_control/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 19:25:47.231950 autonomous_app-0.2.4/src/autonomous/tasks/
--rw-r--r--   0 root         (0) root         (0)       32 2024-02-14 21:26:11.000000 autonomous_app-0.2.4/src/autonomous/tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4910 2024-02-14 21:26:11.000000 autonomous_app-0.2.4/src/autonomous/tasks/autotask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 19:25:47.231950 autonomous_app-0.2.4/src/autonomous_app.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4227 2024-04-19 19:25:47.000000 autonomous_app-0.2.4/src/autonomous_app.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1372 2024-04-19 19:25:47.000000 autonomous_app-0.2.4/src/autonomous_app.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 19:25:47.000000 autonomous_app-0.2.4/src/autonomous_app.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      166 2024-04-19 19:25:47.000000 autonomous_app-0.2.4/src/autonomous_app.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-19 19:25:47.000000 autonomous_app-0.2.4/src/autonomous_app.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.982425 autonomous_app-0.2.5/
+-rw-r--r--   0 root         (0) root         (0)     1076 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4227 2024-04-19 20:02:57.982425 autonomous_app-0.2.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-02-28 15:34:22.000000 autonomous_app-0.2.5/README.md
+-rw-r--r--   0 root         (0) root         (0)     1321 2024-04-16 15:28:50.000000 autonomous_app-0.2.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      521 2024-04-17 20:37:08.000000 autonomous_app-0.2.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 20:02:57.982425 autonomous_app-0.2.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.974424 autonomous_app-0.2.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.978424 autonomous_app-0.2.5/src/autonomous/
+-rw-r--r--   0 root         (0) root         (0)       86 2024-04-19 20:02:41.000000 autonomous_app-0.2.5/src/autonomous/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.978424 autonomous_app-0.2.5/src/autonomous/ai/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 19:48:34.000000 autonomous_app-0.2.5/src/autonomous/ai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7128 2024-04-19 19:59:58.000000 autonomous_app-0.2.5/src/autonomous/ai/oaiagent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.978424 autonomous_app-0.2.5/src/autonomous/auth/
+-rw-r--r--   0 root         (0) root         (0)      161 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3574 2024-02-20 18:09:54.000000 autonomous_app-0.2.5/src/autonomous/auth/autoauth.py
+-rw-r--r--   0 root         (0) root         (0)      886 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/auth/github.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/auth/google.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2024-03-30 04:51:47.000000 autonomous_app-0.2.5/src/autonomous/auth/user.py
+-rw-r--r--   0 root         (0) root         (0)       42 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.978424 autonomous_app-0.2.5/src/autonomous/db/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2024-03-20 18:44:15.000000 autonomous_app-0.2.5/src/autonomous/db/autodb.py
+-rw-r--r--   0 root         (0) root         (0)     4581 2024-02-26 19:40:28.000000 autonomous_app-0.2.5/src/autonomous/db/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.978424 autonomous_app-0.2.5/src/autonomous/errors/
+-rw-r--r--   0 root         (0) root         (0)       59 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/errors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      321 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/errors/danglingreferenceerror.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2024-04-18 14:33:06.000000 autonomous_app-0.2.5/src/autonomous/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.978424 autonomous_app-0.2.5/src/autonomous/model/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      588 2024-02-20 20:56:13.000000 autonomous_app-0.2.5/src/autonomous/model/autoattribute.py
+-rw-r--r--   0 root         (0) root         (0)    11214 2024-04-11 16:19:39.000000 autonomous_app-0.2.5/src/autonomous/model/automodel.py
+-rw-r--r--   0 root         (0) root         (0)     2521 2024-03-30 05:04:37.000000 autonomous_app-0.2.5/src/autonomous/model/orm.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2024-03-24 18:25:01.000000 autonomous_app-0.2.5/src/autonomous/model/serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.978424 autonomous_app-0.2.5/src/autonomous/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 19:48:54.000000 autonomous_app-0.2.5/src/autonomous/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3966 2024-04-17 14:41:12.000000 autonomous_app-0.2.5/src/autonomous/storage/imagestorage.py
+-rw-r--r--   0 root         (0) root         (0)     2286 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/storage/localstorage.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2024-04-17 21:07:33.000000 autonomous_app-0.2.5/src/autonomous/storage/markdown.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.982425 autonomous_app-0.2.5/src/autonomous/storage/version_control/
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/storage/version_control/GHCallbacks.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/storage/version_control/GHOrganization.py
+-rw-r--r--   0 root         (0) root         (0)     4622 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/storage/version_control/GHRepo.py
+-rw-r--r--   0 root         (0) root         (0)      196 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/storage/version_control/GHVersionControl.py
+-rw-r--r--   0 root         (0) root         (0)      117 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/storage/version_control/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.982425 autonomous_app-0.2.5/src/autonomous/tasks/
+-rw-r--r--   0 root         (0) root         (0)       32 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4910 2024-02-14 21:26:11.000000 autonomous_app-0.2.5/src/autonomous/tasks/autotask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 20:02:57.982425 autonomous_app-0.2.5/src/autonomous_app.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4227 2024-04-19 20:02:57.000000 autonomous_app-0.2.5/src/autonomous_app.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1372 2024-04-19 20:02:57.000000 autonomous_app-0.2.5/src/autonomous_app.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 20:02:57.000000 autonomous_app-0.2.5/src/autonomous_app.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2024-04-19 20:02:57.000000 autonomous_app-0.2.5/src/autonomous_app.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-19 20:02:57.000000 autonomous_app-0.2.5/src/autonomous_app.egg-info/top_level.txt
```

### Comparing `autonomous_app-0.2.4/LICENSE` & `autonomous_app-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/PKG-INFO` & `autonomous_app-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.2.4
+Version: 0.2.5
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autonomous_app-0.2.4/README.md` & `autonomous_app-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/pyproject.toml` & `autonomous_app-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/requirements.txt` & `autonomous_app-0.2.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/src/autonomous/ai/oaiagent.py` & `autonomous_app-0.2.5/src/autonomous/ai/oaiagent.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,15 @@
         self._agent_id = value
 
     def clear_agent(self):
         self.client.beta.assistants.delete(self.agent_id)
         self.agent_id = ""
 
     def get_agent(self):
-        result = self.client.beta.assistants.retrieve(self.agent_id)
-        log(f"==== Agent: {result} ====")
-        return result
+        return self.client.beta.assistants.retrieve(self.agent_id)
 
     def clear_files(self, file_id=None):
         if self.vector_store:
             if not file_id:
                 vector_store_files = self.client.beta.vector_stores.files.list(
                     vector_store_id=self.vector_store
                 ).data
```

### Comparing `autonomous_app-0.2.4/src/autonomous/auth/autoauth.py` & `autonomous_app-0.2.5/src/autonomous/auth/autoauth.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/src/autonomous/auth/github.py` & `autonomous_app-0.2.5/src/autonomous/auth/github.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/src/autonomous/auth/google.py` & `autonomous_app-0.2.5/src/autonomous/auth/google.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/src/autonomous/auth/user.py` & `autonomous_app-0.2.5/src/autonomous/auth/user.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/src/autonomous/db/autodb.py` & `autonomous_app-0.2.5/src/autonomous/db/autodb.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/src/autonomous/db/table.py` & `autonomous_app-0.2.5/src/autonomous/db/table.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/src/autonomous/logger.py` & `autonomous_app-0.2.5/src/autonomous/logger.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/src/autonomous/model/autoattribute.py` & `autonomous_app-0.2.5/src/autonomous/model/autoattribute.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/src/autonomous/model/automodel.py` & `autonomous_app-0.2.5/src/autonomous/model/automodel.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/src/autonomous/model/orm.py` & `autonomous_app-0.2.5/src/autonomous/model/orm.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/src/autonomous/model/serializer.py` & `autonomous_app-0.2.5/src/autonomous/model/serializer.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/src/autonomous/storage/imagestorage.py` & `autonomous_app-0.2.5/src/autonomous/storage/imagestorage.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/src/autonomous/storage/localstorage.py` & `autonomous_app-0.2.5/src/autonomous/storage/localstorage.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/src/autonomous/storage/markdown.py` & `autonomous_app-0.2.5/src/autonomous/storage/markdown.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/src/autonomous/storage/version_control/GHCallbacks.py` & `autonomous_app-0.2.5/src/autonomous/storage/version_control/GHCallbacks.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/src/autonomous/storage/version_control/GHOrganization.py` & `autonomous_app-0.2.5/src/autonomous/storage/version_control/GHOrganization.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/src/autonomous/storage/version_control/GHRepo.py` & `autonomous_app-0.2.5/src/autonomous/storage/version_control/GHRepo.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/src/autonomous/tasks/autotask.py` & `autonomous_app-0.2.5/src/autonomous/tasks/autotask.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.4/src/autonomous_app.egg-info/PKG-INFO` & `autonomous_app-0.2.5/src/autonomous_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.2.4
+Version: 0.2.5
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autonomous_app-0.2.4/src/autonomous_app.egg-info/SOURCES.txt` & `autonomous_app-0.2.5/src/autonomous_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

