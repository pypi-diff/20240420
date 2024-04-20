# Comparing `tmp/showroom-0.2.tar.gz` & `tmp/showroom-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "showroom-0.2.tar", last modified: Sat Apr 20 19:14:10 2024, max compression
+gzip compressed data, was "showroom-0.3.tar", last modified: Sat Apr 20 19:26:33 2024, max compression
```

## Comparing `showroom-0.2.tar` & `showroom-0.3.tar`

### file list

```diff
@@ -1,11 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 19:14:10.184832 showroom-0.2/
--rw-rw-rw-   0        0        0      461 2024-04-20 19:14:10.181832 showroom-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-20 19:14:10.186834 showroom-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1485 2024-04-20 19:14:08.000000 showroom-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 19:14:10.151074 showroom-0.2/showroom/
-drwxrwxrwx   0        0        0        0 2024-04-20 19:14:10.173089 showroom-0.2/showroom/showroom.egg-info/
--rw-rw-rw-   0        0        0      461 2024-04-20 19:14:10.000000 showroom-0.2/showroom/showroom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-04-20 19:14:10.000000 showroom-0.2/showroom/showroom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 19:14:10.000000 showroom-0.2/showroom/showroom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-04-20 19:14:10.000000 showroom-0.2/showroom/showroom.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 19:14:10.000000 showroom-0.2/showroom/showroom.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 19:26:33.053245 showroom-0.3/
+-rw-rw-rw-   0        0        0      461 2024-04-20 19:26:33.049230 showroom-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-20 19:26:33.054240 showroom-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1485 2024-04-20 19:25:46.000000 showroom-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 19:26:33.008357 showroom-0.3/showroom/
+drwxrwxrwx   0        0        0        0 2024-04-20 19:26:33.018021 showroom-0.3/showroom/models/
+-rw-rw-rw-   0        0        0      206 2024-04-20 19:26:09.000000 showroom-0.3/showroom/models/__init__.py
+-rw-rw-rw-   0        0        0     5272 2024-04-20 12:56:49.000000 showroom-0.3/showroom/models/models.py
+drwxrwxrwx   0        0        0        0 2024-04-20 19:26:33.040056 showroom-0.3/showroom/showroom.egg-info/
+-rw-rw-rw-   0        0        0      461 2024-04-20 19:26:32.000000 showroom-0.3/showroom/showroom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2024-04-20 19:26:32.000000 showroom-0.3/showroom/showroom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 19:26:32.000000 showroom-0.3/showroom/showroom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-04-20 19:26:32.000000 showroom-0.3/showroom/showroom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-20 19:26:32.000000 showroom-0.3/showroom/showroom.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 19:26:33.043076 showroom-0.3/showroom/sql/
+-rw-rw-rw-   0        0        0        0 2024-04-20 19:26:15.000000 showroom-0.3/showroom/sql/__init__.py
```

### Comparing `showroom-0.2/setup.py` & `showroom-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             if len(files) != 0:
                 sql_files.append((directory, files))
         return sql_files
 
 
 setup(
     name="showroom",
-    version="0.2",
+    version="0.3",
     description="Ntt Showroom models and schemas",
     data_files=FilePicker().sql_file_picker(),
     package_dir={"": "showroom"},
     packages=find_packages(where="showroom"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
```

