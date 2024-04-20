# Comparing `tmp/malfetcher-1.0.0.tar.gz` & `tmp/malfetcher-1.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malfetcher-1.0.0.tar", last modified: Sat Apr 20 07:52:00 2024, max compression
+gzip compressed data, was "malfetcher-1.0.0a0.tar", last modified: Sat Apr 20 08:29:17 2024, max compression
```

## Comparing `malfetcher-1.0.0.tar` & `malfetcher-1.0.0a0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:52:00.013606 malfetcher-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-20 07:51:55.000000 malfetcher-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-20 07:52:00.013606 malfetcher-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-20 07:51:55.000000 malfetcher-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:52:00.013606 malfetcher-1.0.0/malfetcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-20 07:52:00.000000 malfetcher-1.0.0/malfetcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-20 07:52:00.000000 malfetcher-1.0.0/malfetcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 07:52:00.000000 malfetcher-1.0.0/malfetcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 07:52:00.000000 malfetcher-1.0.0/malfetcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 07:52:00.000000 malfetcher-1.0.0/malfetcher.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:52:00.013606 malfetcher-1.0.0/malhelper/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-20 07:51:55.000000 malfetcher-1.0.0/malhelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-20 07:51:55.000000 malfetcher-1.0.0/malhelper/mal_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18910 2024-04-20 07:51:55.000000 malfetcher-1.0.0/malhelper/mal_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-20 07:51:55.000000 malfetcher-1.0.0/malhelper/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-20 07:51:55.000000 malfetcher-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 07:52:00.013606 malfetcher-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-20 07:51:55.000000 malfetcher-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:29:17.409688 malfetcher-1.0.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-20 08:29:08.000000 malfetcher-1.0.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-20 08:29:17.409688 malfetcher-1.0.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-20 08:29:08.000000 malfetcher-1.0.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:29:17.409688 malfetcher-1.0.0a0/malfetcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-20 08:29:08.000000 malfetcher-1.0.0a0/malfetcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-20 08:29:08.000000 malfetcher-1.0.0a0/malfetcher/mal_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18910 2024-04-20 08:29:08.000000 malfetcher-1.0.0a0/malfetcher/mal_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-20 08:29:08.000000 malfetcher-1.0.0a0/malfetcher/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:29:17.409688 malfetcher-1.0.0a0/malfetcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-20 08:29:17.000000 malfetcher-1.0.0a0/malfetcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-20 08:29:17.000000 malfetcher-1.0.0a0/malfetcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 08:29:17.000000 malfetcher-1.0.0a0/malfetcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 08:29:17.000000 malfetcher-1.0.0a0/malfetcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 08:29:17.000000 malfetcher-1.0.0a0/malfetcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-20 08:29:08.000000 malfetcher-1.0.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 08:29:17.409688 malfetcher-1.0.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-20 08:29:08.000000 malfetcher-1.0.0a0/setup.py
```

### Comparing `malfetcher-1.0.0/LICENSE` & `malfetcher-1.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `malfetcher-1.0.0/PKG-INFO` & `malfetcher-1.0.0a0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: malfetcher
-Version: 1.0.0
+Version: 1.0.0a0
 Summary: A simple library to help you fetch data from MyAnimeList.
 Author: Dominik Procházka
 Maintainer: Dominik Procházka
-Project-URL: Homepage, https://github.com/prochy-exe/mal-helper
-Project-URL: Documentation, https://github.com/prochy-exe/mal-helper/wiki
-Project-URL: Source, https://github.com/prochy-exe/mal-helper
+Project-URL: Homepage, https://github.com/prochy-exe/malfetcher
+Project-URL: Documentation, https://github.com/prochy-exe/malfetcher/wiki
+Project-URL: Source, https://github.com/prochy-exe/malfetcher
 Keywords: python,mal,myanimelist
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
 
-# mal-helper
+# malfetcher
 
 A simple library to help you fetch data from MyAnimeList
 
 ## Description
 This library is aimed at people who might be interested in automatizing their anime library.
 
 ## Getting Started
@@ -40,15 +40,15 @@
 * A MyAnimeList account
 * A MyAnimeList developer app
 
 ### Installing
 
 * Clone this repo
 ```
-git clone https://github.com/prochy-exe/mal-helper /path/to/desired/folder
+git clone https://github.com/prochy-exe/malfetcher /path/to/desired/folder
 ```
 * Install it using pip
 ```
 pip install malfetcher
 ```
 * Install it using pip locally
 ```
@@ -82,12 +82,12 @@
 * After that the library is successfully set-up and ready for use.
 
 ## Help
 
 If you encounter any issues, feel free to open a new issue. If you have any new ideas or fixes, please open a pull request, they are more than welcome!
 
 ## Version History
-* [1.0](https://github.com/prochy-exe/mal-helper/releases/tag/v1.0.0)
-    * [Initial Release](https://github.com/prochy-exe/mal-helper/commit/38fbdd36e88890a8339f94d6e193deab5867220e)
+* [1.0](https://github.com/prochy-exe/malfetcher/releases/tag/v1.0.0)
+    * [Initial Release](https://github.com/prochy-exe/malfetcher/commit/2d356310fbe00143c50ffe14596532a7cd30e8db)
 
 ## Acknowledgments
 * [MyAnimeList](https://myanimelist.net)
```

### Comparing `malfetcher-1.0.0/README.md` & `malfetcher-1.0.0a0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# mal-helper
+# malfetcher
 
 A simple library to help you fetch data from MyAnimeList
 
 ## Description
 This library is aimed at people who might be interested in automatizing their anime library.
 
 ## Getting Started
@@ -13,15 +13,15 @@
 * A MyAnimeList account
 * A MyAnimeList developer app
 
 ### Installing
 
 * Clone this repo
 ```
-git clone https://github.com/prochy-exe/mal-helper /path/to/desired/folder
+git clone https://github.com/prochy-exe/malfetcher /path/to/desired/folder
 ```
 * Install it using pip
 ```
 pip install malfetcher
 ```
 * Install it using pip locally
 ```
@@ -55,12 +55,12 @@
 * After that the library is successfully set-up and ready for use.
 
 ## Help
 
 If you encounter any issues, feel free to open a new issue. If you have any new ideas or fixes, please open a pull request, they are more than welcome!
 
 ## Version History
-* [1.0](https://github.com/prochy-exe/mal-helper/releases/tag/v1.0.0)
-    * [Initial Release](https://github.com/prochy-exe/mal-helper/commit/38fbdd36e88890a8339f94d6e193deab5867220e)
+* [1.0](https://github.com/prochy-exe/malfetcher/releases/tag/v1.0.0)
+    * [Initial Release](https://github.com/prochy-exe/malfetcher/commit/2d356310fbe00143c50ffe14596532a7cd30e8db)
 
 ## Acknowledgments
 * [MyAnimeList](https://myanimelist.net)
```

### Comparing `malfetcher-1.0.0/malfetcher.egg-info/PKG-INFO` & `malfetcher-1.0.0a0/malfetcher.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: malfetcher
-Version: 1.0.0
+Version: 1.0.0a0
 Summary: A simple library to help you fetch data from MyAnimeList.
 Author: Dominik Procházka
 Maintainer: Dominik Procházka
-Project-URL: Homepage, https://github.com/prochy-exe/mal-helper
-Project-URL: Documentation, https://github.com/prochy-exe/mal-helper/wiki
-Project-URL: Source, https://github.com/prochy-exe/mal-helper
+Project-URL: Homepage, https://github.com/prochy-exe/malfetcher
+Project-URL: Documentation, https://github.com/prochy-exe/malfetcher/wiki
+Project-URL: Source, https://github.com/prochy-exe/malfetcher
 Keywords: python,mal,myanimelist
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
 
-# mal-helper
+# malfetcher
 
 A simple library to help you fetch data from MyAnimeList
 
 ## Description
 This library is aimed at people who might be interested in automatizing their anime library.
 
 ## Getting Started
@@ -40,15 +40,15 @@
 * A MyAnimeList account
 * A MyAnimeList developer app
 
 ### Installing
 
 * Clone this repo
 ```
-git clone https://github.com/prochy-exe/mal-helper /path/to/desired/folder
+git clone https://github.com/prochy-exe/malfetcher /path/to/desired/folder
 ```
 * Install it using pip
 ```
 pip install malfetcher
 ```
 * Install it using pip locally
 ```
@@ -82,12 +82,12 @@
 * After that the library is successfully set-up and ready for use.
 
 ## Help
 
 If you encounter any issues, feel free to open a new issue. If you have any new ideas or fixes, please open a pull request, they are more than welcome!
 
 ## Version History
-* [1.0](https://github.com/prochy-exe/mal-helper/releases/tag/v1.0.0)
-    * [Initial Release](https://github.com/prochy-exe/mal-helper/commit/38fbdd36e88890a8339f94d6e193deab5867220e)
+* [1.0](https://github.com/prochy-exe/malfetcher/releases/tag/v1.0.0)
+    * [Initial Release](https://github.com/prochy-exe/malfetcher/commit/2d356310fbe00143c50ffe14596532a7cd30e8db)
 
 ## Acknowledgments
 * [MyAnimeList](https://myanimelist.net)
```

### Comparing `malfetcher-1.0.0/malhelper/mal_config_utils.py` & `malfetcher-1.0.0a0/malfetcher/mal_config_utils.py`

 * *Files identical despite different names*

### Comparing `malfetcher-1.0.0/malhelper/mal_helper.py` & `malfetcher-1.0.0a0/malfetcher/mal_fetcher.py`

 * *Files identical despite different names*

### Comparing `malfetcher-1.0.0/malhelper/utils.py` & `malfetcher-1.0.0a0/malfetcher/utils.py`

 * *Files identical despite different names*

### Comparing `malfetcher-1.0.0/pyproject.toml` & `malfetcher-1.0.0a0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -26,10 +26,10 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/prochy-exe/mal-helper"
-"Documentation" = "https://github.com/prochy-exe/mal-helper/wiki"
-"Source" = "https://github.com/prochy-exe/mal-helper"
+"Homepage" = "https://github.com/prochy-exe/malfetcher"
+"Documentation" = "https://github.com/prochy-exe/malfetcher/wiki"
+"Source" = "https://github.com/prochy-exe/malfetcher"
```

