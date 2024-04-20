# Comparing `tmp/async_VKsher-1.7.0.tar.gz` & `tmp/async_VKsher-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_VKsher-1.7.0.tar", last modified: Sat Apr 20 15:26:54 2024, max compression
+gzip compressed data, was "async_VKsher-1.7.1.tar", last modified: Sat Apr 20 15:46:57 2024, max compression
```

## Comparing `async_VKsher-1.7.0.tar` & `async_VKsher-1.7.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 15:26:54.922201 async_VKsher-1.7.0/
--rw-rw-rw-   0        0        0    35149 2022-07-25 16:43:52.000000 async_VKsher-1.7.0/LICENSE
--rw-rw-rw-   0        0        0    28089 2024-04-20 15:26:54.921204 async_VKsher-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0    27096 2024-04-20 15:22:35.000000 async_VKsher-1.7.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 15:26:54.909237 async_VKsher-1.7.0/asyncVK/
--rw-rw-rw-   0        0        0     4177 2024-04-20 14:40:33.000000 async_VKsher-1.7.0/asyncVK/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:26:54.910258 async_VKsher-1.7.0/asyncVK/asyncDB/
--rw-rw-rw-   0        0        0     1199 2021-12-13 13:50:31.000000 async_VKsher-1.7.0/asyncVK/asyncDB/__init__.py
--rw-rw-rw-   0        0        0     1557 2022-07-26 07:13:15.000000 async_VKsher-1.7.0/asyncVK/chain.py
--rw-rw-rw-   0        0        0     1912 2021-12-13 12:57:10.000000 async_VKsher-1.7.0/asyncVK/condition.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:26:54.911231 async_VKsher-1.7.0/asyncVK/core/
--rw-rw-rw-   0        0        0     2364 2024-04-20 15:15:28.000000 async_VKsher-1.7.0/asyncVK/core/__init__.py
--rw-rw-rw-   0        0        0     3639 2024-04-20 14:56:50.000000 async_VKsher-1.7.0/asyncVK/dispatcher.py
--rw-rw-rw-   0        0        0     2690 2024-04-20 15:13:40.000000 async_VKsher-1.7.0/asyncVK/handlers.py
--rw-rw-rw-   0        0        0      731 2021-02-02 06:00:48.000000 async_VKsher-1.7.0/asyncVK/keyboard.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:26:54.913252 async_VKsher-1.7.0/asyncVK/upload/
--rw-rw-rw-   0        0        0       91 2022-07-26 07:31:37.000000 async_VKsher-1.7.0/asyncVK/upload/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:26:54.920207 async_VKsher-1.7.0/async_VKsher.egg-info/
--rw-rw-rw-   0        0        0    28089 2024-04-20 15:26:54.000000 async_VKsher-1.7.0/async_VKsher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2024-04-20 15:26:54.000000 async_VKsher-1.7.0/async_VKsher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 15:26:54.000000 async_VKsher-1.7.0/async_VKsher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-20 15:26:54.000000 async_VKsher-1.7.0/async_VKsher.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-20 15:26:54.000000 async_VKsher-1.7.0/async_VKsher.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 15:26:54.922201 async_VKsher-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0      805 2024-04-20 15:26:19.000000 async_VKsher-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:46:57.621492 async_VKsher-1.7.1/
+-rw-rw-rw-   0        0        0    35149 2022-07-25 16:43:52.000000 async_VKsher-1.7.1/LICENSE
+-rw-rw-rw-   0        0        0    28089 2024-04-20 15:46:57.620494 async_VKsher-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0    27096 2024-04-20 15:22:35.000000 async_VKsher-1.7.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 15:46:57.609523 async_VKsher-1.7.1/asyncVK/
+-rw-rw-rw-   0        0        0     4177 2024-04-20 14:40:33.000000 async_VKsher-1.7.1/asyncVK/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:46:57.610520 async_VKsher-1.7.1/asyncVK/asyncDB/
+-rw-rw-rw-   0        0        0     1199 2021-12-13 13:50:31.000000 async_VKsher-1.7.1/asyncVK/asyncDB/__init__.py
+-rw-rw-rw-   0        0        0     1557 2022-07-26 07:13:15.000000 async_VKsher-1.7.1/asyncVK/chain.py
+-rw-rw-rw-   0        0        0     1912 2021-12-13 12:57:10.000000 async_VKsher-1.7.1/asyncVK/condition.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:46:57.612515 async_VKsher-1.7.1/asyncVK/core/
+-rw-rw-rw-   0        0        0     2364 2024-04-20 15:15:28.000000 async_VKsher-1.7.1/asyncVK/core/__init__.py
+-rw-rw-rw-   0        0        0     3639 2024-04-20 14:56:50.000000 async_VKsher-1.7.1/asyncVK/dispatcher.py
+-rw-rw-rw-   0        0        0     2690 2024-04-20 15:13:40.000000 async_VKsher-1.7.1/asyncVK/handlers.py
+-rw-rw-rw-   0        0        0      731 2021-02-02 06:00:48.000000 async_VKsher-1.7.1/asyncVK/keyboard.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:46:57.612515 async_VKsher-1.7.1/asyncVK/upload/
+-rw-rw-rw-   0        0        0       91 2022-07-26 07:31:37.000000 async_VKsher-1.7.1/asyncVK/upload/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:46:57.619496 async_VKsher-1.7.1/async_VKsher.egg-info/
+-rw-rw-rw-   0        0        0    28089 2024-04-20 15:46:57.000000 async_VKsher-1.7.1/async_VKsher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2024-04-20 15:46:57.000000 async_VKsher-1.7.1/async_VKsher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 15:46:57.000000 async_VKsher-1.7.1/async_VKsher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-20 15:46:57.000000 async_VKsher-1.7.1/async_VKsher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-20 15:46:57.000000 async_VKsher-1.7.1/async_VKsher.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 15:46:57.622489 async_VKsher-1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      805 2024-04-20 15:46:50.000000 async_VKsher-1.7.1/setup.py
```

### Comparing `async_VKsher-1.7.0/LICENSE` & `async_VKsher-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.0/PKG-INFO` & `async_VKsher-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async_VKsher
-Version: 1.7.0
+Version: 1.7.1
 Summary: asyncVK is asynchronous library for creating a bot in VK
 Home-page: https://github.com/Ekventor/asyncVK
 Author: Kulenov Islam
 Author-email: kit.werr34@gmail.com
 Keywords: vk vkontakte вк вконтакте бот bot
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `async_VKsher-1.7.0/README.md` & `async_VKsher-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.0/asyncVK/__init__.py` & `async_VKsher-1.7.1/asyncVK/__init__.py`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.0/asyncVK/asyncDB/__init__.py` & `async_VKsher-1.7.1/asyncVK/asyncDB/__init__.py`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.0/asyncVK/chain.py` & `async_VKsher-1.7.1/asyncVK/chain.py`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.0/asyncVK/condition.py` & `async_VKsher-1.7.1/asyncVK/condition.py`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.0/asyncVK/core/__init__.py` & `async_VKsher-1.7.1/asyncVK/core/__init__.py`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.0/asyncVK/dispatcher.py` & `async_VKsher-1.7.1/asyncVK/dispatcher.py`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.0/asyncVK/handlers.py` & `async_VKsher-1.7.1/asyncVK/handlers.py`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.0/asyncVK/keyboard.py` & `async_VKsher-1.7.1/asyncVK/keyboard.py`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.0/async_VKsher.egg-info/PKG-INFO` & `async_VKsher-1.7.1/async_VKsher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async_VKsher
-Version: 1.7.0
+Version: 1.7.1
 Summary: asyncVK is asynchronous library for creating a bot in VK
 Home-page: https://github.com/Ekventor/asyncVK
 Author: Kulenov Islam
 Author-email: kit.werr34@gmail.com
 Keywords: vk vkontakte вк вконтакте бот bot
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `async_VKsher-1.7.0/setup.py` & `async_VKsher-1.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 requirements = ["asyncio>=3", "aiohttp>=3"]
 
 
 setup(
     name="async_VKsher",
-    version="1.7.0",
+    version="1.7.1",
     author="Kulenov Islam",
     author_email="kit.werr34@gmail.com",
     description="asyncVK is asynchronous library for creating a bot in VK",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/Ekventor/asyncVK",
     packages=find_packages(),
```

