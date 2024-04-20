# Comparing `tmp/dailytasks-2.1.3.tar.gz` & `tmp/dailytasks-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dailytasks-2.1.3.tar", last modified: Tue Apr 16 17:53:50 2024, max compression
+gzip compressed data, was "dailytasks-2.2.0.tar", last modified: Sat Apr 20 01:53:01 2024, max compression
```

## Comparing `dailytasks-2.1.3.tar` & `dailytasks-2.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:53:50.183582 dailytasks-2.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:53:50.175582 dailytasks-2.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:53:50.179582 dailytasks-2.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-16 17:53:46.000000 dailytasks-2.1.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-16 17:53:46.000000 dailytasks-2.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-16 17:53:46.000000 dailytasks-2.1.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 17:53:46.000000 dailytasks-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 17:53:46.000000 dailytasks-2.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15478 2024-04-16 17:53:50.183582 dailytasks-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-16 17:53:46.000000 dailytasks-2.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:53:50.179582 dailytasks-2.1.3/daily_tasks/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:53:50.179582 dailytasks-2.1.3/daily_tasks/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/commands/filter_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/commands/info_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/commands/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/commands/main_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/commands/modification_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/commands/removal_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/commands/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:53:50.179582 dailytasks-2.1.3/daily_tasks/data_files/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/data_files/tasks.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:53:50.179582 dailytasks-2.1.3/daily_tasks/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/tests/test_main_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/tests/test_sub_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:53:50.183582 dailytasks-2.1.3/dailytasks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15478 2024-04-16 17:53:50.000000 dailytasks-2.1.3/dailytasks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-16 17:53:50.000000 dailytasks-2.1.3/dailytasks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:53:50.000000 dailytasks-2.1.3/dailytasks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 17:53:50.000000 dailytasks-2.1.3/dailytasks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-16 17:53:50.000000 dailytasks-2.1.3/dailytasks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 17:53:50.000000 dailytasks-2.1.3/dailytasks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-16 17:53:46.000000 dailytasks-2.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-16 17:53:46.000000 dailytasks-2.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 17:53:50.183582 dailytasks-2.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:53:01.929000 dailytasks-2.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:53:01.924999 dailytasks-2.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:53:01.924999 dailytasks-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-20 01:52:57.000000 dailytasks-2.2.0/.github/workflows/build_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-20 01:52:57.000000 dailytasks-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-20 01:52:57.000000 dailytasks-2.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-20 01:52:57.000000 dailytasks-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-20 01:52:57.000000 dailytasks-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16119 2024-04-20 01:53:01.929000 dailytasks-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-20 01:52:57.000000 dailytasks-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:53:01.924999 dailytasks-2.2.0/daily_tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-20 01:52:57.000000 dailytasks-2.2.0/daily_tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:53:01.929000 dailytasks-2.2.0/daily_tasks/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-20 01:52:57.000000 dailytasks-2.2.0/daily_tasks/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-20 01:52:57.000000 dailytasks-2.2.0/daily_tasks/commands/filter_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-20 01:52:57.000000 dailytasks-2.2.0/daily_tasks/commands/info_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-20 01:52:57.000000 dailytasks-2.2.0/daily_tasks/commands/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-20 01:52:57.000000 dailytasks-2.2.0/daily_tasks/commands/main_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-20 01:52:57.000000 dailytasks-2.2.0/daily_tasks/commands/modification_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-20 01:52:57.000000 dailytasks-2.2.0/daily_tasks/commands/removal_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-20 01:52:57.000000 dailytasks-2.2.0/daily_tasks/commands/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:53:01.929000 dailytasks-2.2.0/daily_tasks/data_files/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-20 01:52:57.000000 dailytasks-2.2.0/daily_tasks/data_files/tasks.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:53:01.929000 dailytasks-2.2.0/daily_tasks/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:52:57.000000 dailytasks-2.2.0/daily_tasks/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-20 01:52:57.000000 dailytasks-2.2.0/daily_tasks/tests/test_main_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-20 01:52:57.000000 dailytasks-2.2.0/daily_tasks/tests/test_sub_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:53:01.929000 dailytasks-2.2.0/dailytasks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16119 2024-04-20 01:53:01.000000 dailytasks-2.2.0/dailytasks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-20 01:53:01.000000 dailytasks-2.2.0/dailytasks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:53:01.000000 dailytasks-2.2.0/dailytasks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-20 01:53:01.000000 dailytasks-2.2.0/dailytasks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-20 01:53:01.000000 dailytasks-2.2.0/dailytasks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-20 01:53:01.000000 dailytasks-2.2.0/dailytasks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-20 01:52:57.000000 dailytasks-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-20 01:52:57.000000 dailytasks-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 01:53:01.929000 dailytasks-2.2.0/setup.cfg
```

### Comparing `dailytasks-2.1.3/.github/workflows/publish.yml` & `dailytasks-2.2.0/.github/workflows/build_and_publish.yml`

 * *Files identical despite different names*

### Comparing `dailytasks-2.1.3/CONTRIBUTING.md` & `dailytasks-2.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dailytasks-2.1.3/LICENSE` & `dailytasks-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dailytasks-2.1.3/PKG-INFO` & `dailytasks-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dailytasks
-Version: 2.1.3
+Version: 2.2.0
 Summary: A tasks manager for those who like work from shell.
 Author-email: LuisanaMTDev <luisanamartineztorres25@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -218,14 +218,16 @@
 
 # DailyTasks #
 A tasks manager for those who like work from shell.
 
 ![PyPI - Version](https://img.shields.io/pypi/v/dailytasks?style=for-the-badge&label=Lastest%20version&color=008B8B&link=https%3A%2F%2Fpypi.org%2Fproject%2Fdailytasks%2F)
 ![GitHub issue custom search in repo](https://img.shields.io/github/issues-search/LuisanaMTDev/dailytasks?query=is%3Aopen&style=for-the-badge&label=Open%20issues&color=008B8B&link=https%3A%2F%2Fgithub.com%2FLuisanaMTDev%2Fdailytasks%2Fissues%3Fq%3Dis%253Aissue%2Bis%253Aopen)
 
+
+
 ## Installation ##
 **Requirements:**
 - Python >= 3.11
 
 **How install it:**
 
 `pip install dailytasks`
@@ -239,14 +241,28 @@
 
 2. After update execute `dailytasks import` command to restore all your data.
 
     2.1. Provide the path provided before (with `-p` option) and all your data will be restore.
 
    **This is because when you update the CLI, data folder ([data_files](./daily_tasks/data_files/)) is overwritten and all your data deleted.**
    
+## How to add tasks from a json file ##
+Execute `dailytasks import --help` to get information about import cmd options.
+
+import options:
+- Normal:
+    `dailytasks import -p C:\where\you\export\tasks\are`
+- Personalized (A better name is welcome):
+    `dailytasks import -a -f your_json_file_name -d key_that_contains_the_descriptions -p C:\where\you\json\file\is`
+
+    - `-a`: Activate this option.
+    - `-f`: To pass name of your json file.
+    - `-d`: The text you want as description should be in a object, in a key-value pair, to this option you will pass key of that key-value pair.
+    - `-p`: To pass path where you json file is.
+
 ## Testing ##
 
 Running tests locally:
 
 1. Clone this repository.
 
 1. cd into your clone.
```

### Comparing `dailytasks-2.1.3/README.md` & `dailytasks-2.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # DailyTasks #
 A tasks manager for those who like work from shell.
 
 ![PyPI - Version](https://img.shields.io/pypi/v/dailytasks?style=for-the-badge&label=Lastest%20version&color=008B8B&link=https%3A%2F%2Fpypi.org%2Fproject%2Fdailytasks%2F)
 ![GitHub issue custom search in repo](https://img.shields.io/github/issues-search/LuisanaMTDev/dailytasks?query=is%3Aopen&style=for-the-badge&label=Open%20issues&color=008B8B&link=https%3A%2F%2Fgithub.com%2FLuisanaMTDev%2Fdailytasks%2Fissues%3Fq%3Dis%253Aissue%2Bis%253Aopen)
 
+
+
 ## Installation ##
 **Requirements:**
 - Python >= 3.11
 
 **How install it:**
 
 `pip install dailytasks`
@@ -21,14 +23,28 @@
 
 2. After update execute `dailytasks import` command to restore all your data.
 
     2.1. Provide the path provided before (with `-p` option) and all your data will be restore.
 
    **This is because when you update the CLI, data folder ([data_files](./daily_tasks/data_files/)) is overwritten and all your data deleted.**
    
+## How to add tasks from a json file ##
+Execute `dailytasks import --help` to get information about import cmd options.
+
+import options:
+- Normal:
+    `dailytasks import -p C:\where\you\export\tasks\are`
+- Personalized (A better name is welcome):
+    `dailytasks import -a -f your_json_file_name -d key_that_contains_the_descriptions -p C:\where\you\json\file\is`
+
+    - `-a`: Activate this option.
+    - `-f`: To pass name of your json file.
+    - `-d`: The text you want as description should be in a object, in a key-value pair, to this option you will pass key of that key-value pair.
+    - `-p`: To pass path where you json file is.
+
 ## Testing ##
 
 Running tests locally:
 
 1. Clone this repository.
 
 1. cd into your clone.
```

### Comparing `dailytasks-2.1.3/daily_tasks/commands/filter_commands.py` & `dailytasks-2.2.0/daily_tasks/commands/filter_commands.py`

 * *Files identical despite different names*

### Comparing `dailytasks-2.1.3/daily_tasks/commands/main.py` & `dailytasks-2.2.0/daily_tasks/commands/main.py`

 * *Files identical despite different names*

### Comparing `dailytasks-2.1.3/daily_tasks/commands/main_commands.py` & `dailytasks-2.2.0/daily_tasks/commands/main_commands.py`

 * *Files identical despite different names*

### Comparing `dailytasks-2.1.3/daily_tasks/commands/modification_commands.py` & `dailytasks-2.2.0/daily_tasks/commands/modification_commands.py`

 * *Files identical despite different names*

### Comparing `dailytasks-2.1.3/daily_tasks/commands/removal_commands.py` & `dailytasks-2.2.0/daily_tasks/commands/removal_commands.py`

 * *Files identical despite different names*

### Comparing `dailytasks-2.1.3/daily_tasks/commands/utilities.py` & `dailytasks-2.2.0/daily_tasks/commands/utilities.py`

 * *Files identical despite different names*

### Comparing `dailytasks-2.1.3/daily_tasks/tests/test_main_commands.py` & `dailytasks-2.2.0/daily_tasks/tests/test_main_commands.py`

 * *Files identical despite different names*

### Comparing `dailytasks-2.1.3/daily_tasks/tests/test_sub_commands.py` & `dailytasks-2.2.0/daily_tasks/tests/test_sub_commands.py`

 * *Files identical despite different names*

### Comparing `dailytasks-2.1.3/dailytasks.egg-info/PKG-INFO` & `dailytasks-2.2.0/dailytasks.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dailytasks
-Version: 2.1.3
+Version: 2.2.0
 Summary: A tasks manager for those who like work from shell.
 Author-email: LuisanaMTDev <luisanamartineztorres25@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -218,14 +218,16 @@
 
 # DailyTasks #
 A tasks manager for those who like work from shell.
 
 ![PyPI - Version](https://img.shields.io/pypi/v/dailytasks?style=for-the-badge&label=Lastest%20version&color=008B8B&link=https%3A%2F%2Fpypi.org%2Fproject%2Fdailytasks%2F)
 ![GitHub issue custom search in repo](https://img.shields.io/github/issues-search/LuisanaMTDev/dailytasks?query=is%3Aopen&style=for-the-badge&label=Open%20issues&color=008B8B&link=https%3A%2F%2Fgithub.com%2FLuisanaMTDev%2Fdailytasks%2Fissues%3Fq%3Dis%253Aissue%2Bis%253Aopen)
 
+
+
 ## Installation ##
 **Requirements:**
 - Python >= 3.11
 
 **How install it:**
 
 `pip install dailytasks`
@@ -239,14 +241,28 @@
 
 2. After update execute `dailytasks import` command to restore all your data.
 
     2.1. Provide the path provided before (with `-p` option) and all your data will be restore.
 
    **This is because when you update the CLI, data folder ([data_files](./daily_tasks/data_files/)) is overwritten and all your data deleted.**
    
+## How to add tasks from a json file ##
+Execute `dailytasks import --help` to get information about import cmd options.
+
+import options:
+- Normal:
+    `dailytasks import -p C:\where\you\export\tasks\are`
+- Personalized (A better name is welcome):
+    `dailytasks import -a -f your_json_file_name -d key_that_contains_the_descriptions -p C:\where\you\json\file\is`
+
+    - `-a`: Activate this option.
+    - `-f`: To pass name of your json file.
+    - `-d`: The text you want as description should be in a object, in a key-value pair, to this option you will pass key of that key-value pair.
+    - `-p`: To pass path where you json file is.
+
 ## Testing ##
 
 Running tests locally:
 
 1. Clone this repository.
 
 1. cd into your clone.
```

### Comparing `dailytasks-2.1.3/dailytasks.egg-info/SOURCES.txt` & `dailytasks-2.2.0/dailytasks.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .gitignore
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
-.github/workflows/publish.yml
+.github/workflows/build_and_publish.yml
 daily_tasks/__init__.py
 daily_tasks/commands/__init__.py
 daily_tasks/commands/filter_commands.py
 daily_tasks/commands/info_commands.py
 daily_tasks/commands/main.py
 daily_tasks/commands/main_commands.py
 daily_tasks/commands/modification_commands.py
```

### Comparing `dailytasks-2.1.3/pyproject.toml` & `dailytasks-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dailytasks"
-version = "2.1.3"
+version = "2.2.0"
 authors = [{name = "LuisanaMTDev", email = "luisanamartineztorres25@gmail.com"}]
 description = "A tasks manager for those who like work from shell."
 readme = "README.md"
 license = { file = "LICENSE"}
 classifiers = [
     "Environment :: Console",
     "Intended Audience :: Developers",
```

