# Comparing `tmp/showroom-0.0.1.tar.gz` & `tmp/showroom-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "showroom-0.0.1.tar", last modified: Sat Apr 20 18:59:18 2024, max compression
+gzip compressed data, was "showroom-0.2.tar", last modified: Sat Apr 20 19:14:10 2024, max compression
```

## Comparing `showroom-0.0.1.tar` & `showroom-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 18:59:18.946801 showroom-0.0.1/
--rw-rw-rw-   0        0        0      463 2024-04-20 18:59:18.944783 showroom-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-20 18:59:18.948783 showroom-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1487 2024-04-20 18:52:29.000000 showroom-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 18:59:18.913259 showroom-0.0.1/showroom/
-drwxrwxrwx   0        0        0        0 2024-04-20 18:59:18.939789 showroom-0.0.1/showroom/showroom.egg-info/
--rw-rw-rw-   0        0        0      463 2024-04-20 18:59:18.000000 showroom-0.0.1/showroom/showroom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-04-20 18:59:18.000000 showroom-0.0.1/showroom/showroom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 18:59:18.000000 showroom-0.0.1/showroom/showroom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-04-20 18:59:18.000000 showroom-0.0.1/showroom/showroom.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 18:59:18.000000 showroom-0.0.1/showroom/showroom.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 19:14:10.184832 showroom-0.2/
+-rw-rw-rw-   0        0        0      461 2024-04-20 19:14:10.181832 showroom-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-20 19:14:10.186834 showroom-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1485 2024-04-20 19:14:08.000000 showroom-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 19:14:10.151074 showroom-0.2/showroom/
+drwxrwxrwx   0        0        0        0 2024-04-20 19:14:10.173089 showroom-0.2/showroom/showroom.egg-info/
+-rw-rw-rw-   0        0        0      461 2024-04-20 19:14:10.000000 showroom-0.2/showroom/showroom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-04-20 19:14:10.000000 showroom-0.2/showroom/showroom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 19:14:10.000000 showroom-0.2/showroom/showroom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-04-20 19:14:10.000000 showroom-0.2/showroom/showroom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 19:14:10.000000 showroom-0.2/showroom/showroom.egg-info/top_level.txt
```

### Comparing `showroom-0.0.1/setup.py` & `showroom-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             if len(files) != 0:
                 sql_files.append((directory, files))
         return sql_files
 
 
 setup(
     name="showroom",
-    version="0.0.1",
+    version="0.2",
     description="Ntt Showroom models and schemas",
     data_files=FilePicker().sql_file_picker(),
     package_dir={"": "showroom"},
     packages=find_packages(where="showroom"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
```

