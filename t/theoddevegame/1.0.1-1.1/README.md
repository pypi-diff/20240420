# Comparing `tmp/theoddevegame-1.0.1.tar.gz` & `tmp/theoddevegame-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theoddevegame-1.0.1.tar", last modified: Thu Apr 18 19:36:21 2024, max compression
+gzip compressed data, was "theoddevegame-1.1.tar", last modified: Sat Apr 20 17:02:23 2024, max compression
```

## Comparing `theoddevegame-1.0.1.tar` & `theoddevegame-1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 19:36:21.508056 theoddevegame-1.0.1/
--rw-rw-rw-   0        0        0     1916 2024-04-18 19:36:21.506623 theoddevegame-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-18 19:36:21.508056 theoddevegame-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-18 19:36:21.297426 theoddevegame-1.0.1/theoddevegame/
-drwxrwxrwx   0        0        0        0 2024-04-18 19:36:21.298029 theoddevegame-1.0.1/theoddevegame/src/
-drwxrwxrwx   0        0        0        0 2024-04-18 19:36:21.505221 theoddevegame-1.0.1/theoddevegame/src/theoddevegame.egg-info/
--rw-rw-rw-   0        0        0     1916 2024-04-18 19:36:20.000000 theoddevegame-1.0.1/theoddevegame/src/theoddevegame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-04-18 19:36:20.000000 theoddevegame-1.0.1/theoddevegame/src/theoddevegame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 19:36:20.000000 theoddevegame-1.0.1/theoddevegame/src/theoddevegame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-18 19:36:20.000000 theoddevegame-1.0.1/theoddevegame/src/theoddevegame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8941 2024-04-18 19:24:28.000000 theoddevegame-1.0.1/theoddevegame/src/theoddevegame.py
+drwxrwxrwx   0        0        0        0 2024-04-20 17:02:23.806910 theoddevegame-1.1/
+-rw-rw-rw-   0        0        0     1976 2024-04-20 17:02:23.806230 theoddevegame-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-20 17:02:23.806910 theoddevegame-1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-20 17:02:23.718566 theoddevegame-1.1/theoddevegame/
+drwxrwxrwx   0        0        0        0 2024-04-20 17:02:23.719111 theoddevegame-1.1/theoddevegame/src/
+drwxrwxrwx   0        0        0        0 2024-04-20 17:02:23.805215 theoddevegame-1.1/theoddevegame/src/theoddevegame.egg-info/
+-rw-rw-rw-   0        0        0     1976 2024-04-20 17:02:22.000000 theoddevegame-1.1/theoddevegame/src/theoddevegame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-04-20 17:02:22.000000 theoddevegame-1.1/theoddevegame/src/theoddevegame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 17:02:22.000000 theoddevegame-1.1/theoddevegame/src/theoddevegame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-20 17:02:22.000000 theoddevegame-1.1/theoddevegame/src/theoddevegame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13919 2024-04-20 12:42:25.000000 theoddevegame-1.1/theoddevegame/src/theoddevegame.py
```

### Comparing `theoddevegame-1.0.1/PKG-INFO` & `theoddevegame-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: theoddevegame
-Version: 1.0.1
-Summary: The digitised odd eve game (The hand cricket version). 
+Version: 1.1
+Summary: The digitised odd eve game (The hand cricket version). The version 1.1 offers fixes some bugs and minor improvements.
 Author: Prashant Bhatt
 Author-email: pb3924924@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `theoddevegame-1.0.1/theoddevegame/src/theoddevegame.egg-info/PKG-INFO` & `theoddevegame-1.1/theoddevegame/src/theoddevegame.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: theoddevegame
-Version: 1.0.1
-Summary: The digitised odd eve game (The hand cricket version). 
+Version: 1.1
+Summary: The digitised odd eve game (The hand cricket version). The version 1.1 offers fixes some bugs and minor improvements.
 Author: Prashant Bhatt
 Author-email: pb3924924@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

