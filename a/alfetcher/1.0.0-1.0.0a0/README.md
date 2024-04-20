# Comparing `tmp/alfetcher-1.0.0.tar.gz` & `tmp/alfetcher-1.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfetcher-1.0.0.tar", last modified: Sat Apr 20 07:46:32 2024, max compression
+gzip compressed data, was "alfetcher-1.0.0a0.tar", last modified: Sat Apr 20 08:30:18 2024, max compression
```

## Comparing `alfetcher-1.0.0.tar` & `alfetcher-1.0.0a0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:46:32.626436 alfetcher-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-20 07:46:28.000000 alfetcher-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-20 07:46:32.626436 alfetcher-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-20 07:46:28.000000 alfetcher-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:46:32.626436 alfetcher-1.0.0/alfetcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-20 07:46:32.000000 alfetcher-1.0.0/alfetcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-20 07:46:32.000000 alfetcher-1.0.0/alfetcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 07:46:32.000000 alfetcher-1.0.0/alfetcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 07:46:32.000000 alfetcher-1.0.0/alfetcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 07:46:32.000000 alfetcher-1.0.0/alfetcher.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:46:32.626436 alfetcher-1.0.0/alhelper/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-20 07:46:28.000000 alfetcher-1.0.0/alhelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-20 07:46:28.000000 alfetcher-1.0.0/alhelper/al_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23029 2024-04-20 07:46:28.000000 alfetcher-1.0.0/alhelper/al_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-20 07:46:28.000000 alfetcher-1.0.0/alhelper/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-20 07:46:28.000000 alfetcher-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 07:46:32.626436 alfetcher-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 07:46:28.000000 alfetcher-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:30:18.458609 alfetcher-1.0.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-20 08:30:08.000000 alfetcher-1.0.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-20 08:30:18.458609 alfetcher-1.0.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-20 08:30:08.000000 alfetcher-1.0.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:30:18.458609 alfetcher-1.0.0a0/alfetcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-20 08:30:08.000000 alfetcher-1.0.0a0/alfetcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-20 08:30:08.000000 alfetcher-1.0.0a0/alfetcher/al_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23029 2024-04-20 08:30:08.000000 alfetcher-1.0.0a0/alfetcher/al_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-20 08:30:08.000000 alfetcher-1.0.0a0/alfetcher/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:30:18.458609 alfetcher-1.0.0a0/alfetcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-20 08:30:18.000000 alfetcher-1.0.0a0/alfetcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-20 08:30:18.000000 alfetcher-1.0.0a0/alfetcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 08:30:18.000000 alfetcher-1.0.0a0/alfetcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 08:30:18.000000 alfetcher-1.0.0a0/alfetcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 08:30:18.000000 alfetcher-1.0.0a0/alfetcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-20 08:30:08.000000 alfetcher-1.0.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 08:30:18.458609 alfetcher-1.0.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-20 08:30:08.000000 alfetcher-1.0.0a0/setup.py
```

### Comparing `alfetcher-1.0.0/LICENSE` & `alfetcher-1.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `alfetcher-1.0.0/PKG-INFO` & `alfetcher-1.0.0a0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: alfetcher
-Version: 1.0.0
+Version: 1.0.0a0
 Summary: A simple library to help you fetch data from AniList.
 Author: Dominik Procházka
 Maintainer: Dominik Procházka
-Project-URL: Homepage, https://github.com/prochy-exe/al-helper
-Project-URL: Documentation, https://github.com/prochy-exe/al-helper/wiki
-Project-URL: Source, https://github.com/prochy-exe/al-helper
+Project-URL: Homepage, https://github.com/prochy-exe/alfetcher
+Project-URL: Documentation, https://github.com/prochy-exe/alfetcher/wiki
+Project-URL: Source, https://github.com/prochy-exe/alfetcher
 Keywords: python,anilist,al
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flask
 Classifier: Topic :: Database
 Classifier: Topic :: Games/Entertainment
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.8
@@ -21,15 +21,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: flask
 Requires-Dist: gevent
 
-# al-helper
+# alfetcher
 
 A simple library to help you fetch data from AniList
 
 ## Description
 
 Welcome to my first python project!
 This library is aimed at people who might be interested in automatizing their anime library.
@@ -43,19 +43,19 @@
 * An AniList developer app
 * Javascript enabled during the set-up process (for sending the access token back to Python)
 
 ### Installing
 
 * Clone this repo
 ```
-git clone https://github.com/ProchyGaming/al-helper /path/to/desired/folder
+git clone https://github.com/ProchyGaming/alfetcher /path/to/desired/folder
 ```
 * Install it using pip
 ```
-pip install al-helper
+pip install alfetcher
 ```
 * Install it using pip locally
 ```
 cd /path/to/desired/folder
 pip install .
 ```
 * If you want to make modifications to the library install it in the edit mode:
@@ -85,15 +85,15 @@
 * After that the library is successfully set-up and ready for use.
 
 ## Help
 
 If you encounter any issues, feel free to open a new issue. If you have any new ideas or fixes, please open a pull request, they are more than welcome!
 
 ## Version History
-* [1.0.0](https://github.com/prochy-exe/al-helper/releases/tag/v1.0.0)
-    * [Initial Release](https://github.com/prochy-exe/al-helper/commit/8abffc852728cecb580282a0749c8051b95e3d10)
+* [1.0.0](https://github.com/prochy-exe/alfetcher/releases/tag/v1.0.0)
+    * [Initial Release](https://github.com/prochy-exe/alfetcher/commit/4b67b1d8719d183012446a065c5b6c941ec6518e)
 
 ## Acknowledgments
 
 Huge thanks to AniList team for their great page and database:
 * [AniList](https://anilist.co/home)
 * [AniList GraphQL](https://anilist.co/graphiql)
```

### Comparing `alfetcher-1.0.0/README.md` & `alfetcher-1.0.0a0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# al-helper
+# alfetcher
 
 A simple library to help you fetch data from AniList
 
 ## Description
 
 Welcome to my first python project!
 This library is aimed at people who might be interested in automatizing their anime library.
@@ -16,19 +16,19 @@
 * An AniList developer app
 * Javascript enabled during the set-up process (for sending the access token back to Python)
 
 ### Installing
 
 * Clone this repo
 ```
-git clone https://github.com/ProchyGaming/al-helper /path/to/desired/folder
+git clone https://github.com/ProchyGaming/alfetcher /path/to/desired/folder
 ```
 * Install it using pip
 ```
-pip install al-helper
+pip install alfetcher
 ```
 * Install it using pip locally
 ```
 cd /path/to/desired/folder
 pip install .
 ```
 * If you want to make modifications to the library install it in the edit mode:
@@ -58,15 +58,15 @@
 * After that the library is successfully set-up and ready for use.
 
 ## Help
 
 If you encounter any issues, feel free to open a new issue. If you have any new ideas or fixes, please open a pull request, they are more than welcome!
 
 ## Version History
-* [1.0.0](https://github.com/prochy-exe/al-helper/releases/tag/v1.0.0)
-    * [Initial Release](https://github.com/prochy-exe/al-helper/commit/8abffc852728cecb580282a0749c8051b95e3d10)
+* [1.0.0](https://github.com/prochy-exe/alfetcher/releases/tag/v1.0.0)
+    * [Initial Release](https://github.com/prochy-exe/alfetcher/commit/4b67b1d8719d183012446a065c5b6c941ec6518e)
 
 ## Acknowledgments
 
 Huge thanks to AniList team for their great page and database:
 * [AniList](https://anilist.co/home)
 * [AniList GraphQL](https://anilist.co/graphiql)
```

### Comparing `alfetcher-1.0.0/alfetcher.egg-info/PKG-INFO` & `alfetcher-1.0.0a0/alfetcher.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: alfetcher
-Version: 1.0.0
+Version: 1.0.0a0
 Summary: A simple library to help you fetch data from AniList.
 Author: Dominik Procházka
 Maintainer: Dominik Procházka
-Project-URL: Homepage, https://github.com/prochy-exe/al-helper
-Project-URL: Documentation, https://github.com/prochy-exe/al-helper/wiki
-Project-URL: Source, https://github.com/prochy-exe/al-helper
+Project-URL: Homepage, https://github.com/prochy-exe/alfetcher
+Project-URL: Documentation, https://github.com/prochy-exe/alfetcher/wiki
+Project-URL: Source, https://github.com/prochy-exe/alfetcher
 Keywords: python,anilist,al
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flask
 Classifier: Topic :: Database
 Classifier: Topic :: Games/Entertainment
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.8
@@ -21,15 +21,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: flask
 Requires-Dist: gevent
 
-# al-helper
+# alfetcher
 
 A simple library to help you fetch data from AniList
 
 ## Description
 
 Welcome to my first python project!
 This library is aimed at people who might be interested in automatizing their anime library.
@@ -43,19 +43,19 @@
 * An AniList developer app
 * Javascript enabled during the set-up process (for sending the access token back to Python)
 
 ### Installing
 
 * Clone this repo
 ```
-git clone https://github.com/ProchyGaming/al-helper /path/to/desired/folder
+git clone https://github.com/ProchyGaming/alfetcher /path/to/desired/folder
 ```
 * Install it using pip
 ```
-pip install al-helper
+pip install alfetcher
 ```
 * Install it using pip locally
 ```
 cd /path/to/desired/folder
 pip install .
 ```
 * If you want to make modifications to the library install it in the edit mode:
@@ -85,15 +85,15 @@
 * After that the library is successfully set-up and ready for use.
 
 ## Help
 
 If you encounter any issues, feel free to open a new issue. If you have any new ideas or fixes, please open a pull request, they are more than welcome!
 
 ## Version History
-* [1.0.0](https://github.com/prochy-exe/al-helper/releases/tag/v1.0.0)
-    * [Initial Release](https://github.com/prochy-exe/al-helper/commit/8abffc852728cecb580282a0749c8051b95e3d10)
+* [1.0.0](https://github.com/prochy-exe/alfetcher/releases/tag/v1.0.0)
+    * [Initial Release](https://github.com/prochy-exe/alfetcher/commit/4b67b1d8719d183012446a065c5b6c941ec6518e)
 
 ## Acknowledgments
 
 Huge thanks to AniList team for their great page and database:
 * [AniList](https://anilist.co/home)
 * [AniList GraphQL](https://anilist.co/graphiql)
```

### Comparing `alfetcher-1.0.0/alhelper/al_config_utils.py` & `alfetcher-1.0.0a0/alfetcher/al_config_utils.py`

 * *Files identical despite different names*

### Comparing `alfetcher-1.0.0/alhelper/al_helper.py` & `alfetcher-1.0.0a0/alfetcher/al_fetcher.py`

 * *Files identical despite different names*

### Comparing `alfetcher-1.0.0/alhelper/utils.py` & `alfetcher-1.0.0a0/alfetcher/utils.py`

 * *Files identical despite different names*

### Comparing `alfetcher-1.0.0/pyproject.toml` & `alfetcher-1.0.0a0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -26,10 +26,10 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/prochy-exe/al-helper"
-"Documentation" = "https://github.com/prochy-exe/al-helper/wiki"
-"Source" = "https://github.com/prochy-exe/al-helper"
+"Homepage" = "https://github.com/prochy-exe/alfetcher"
+"Documentation" = "https://github.com/prochy-exe/alfetcher/wiki"
+"Source" = "https://github.com/prochy-exe/alfetcher"
```

