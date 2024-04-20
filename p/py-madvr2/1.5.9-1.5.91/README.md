# Comparing `tmp/py_madvr2-1.5.9.tar.gz` & `tmp/py_madvr2-1.5.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr2-1.5.9.tar", last modified: Fri Apr 19 23:46:17 2024, max compression
+gzip compressed data, was "py_madvr2-1.5.91.tar", last modified: Sat Apr 20 00:11:02 2024, max compression
```

## Comparing `py_madvr2-1.5.9.tar` & `py_madvr2-1.5.91.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 23:46:17.220145 py_madvr2-1.5.9/
--rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-01-10 23:29:29.000000 py_madvr2-1.5.9/LICENSE
--rw-r--r--   0 ilan       (501) staff       (20)      870 2024-04-19 23:46:17.219953 py_madvr2-1.5.9/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)      472 2023-05-14 18:58:32.000000 py_madvr2-1.5.9/README.md
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 23:46:17.218399 py_madvr2-1.5.9/madvr/
--rw-r--r--   0 ilan       (501) staff       (20)      230 2023-01-10 23:29:29.000000 py_madvr2-1.5.9/madvr/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)     3566 2023-07-02 16:13:13.000000 py_madvr2-1.5.9/madvr/commands.py
--rw-r--r--   0 ilan       (501) staff       (20)      242 2023-01-14 01:34:27.000000 py_madvr2-1.5.9/madvr/errors.py
--rw-r--r--   0 ilan       (501) staff       (20)    17191 2024-04-19 23:45:45.000000 py_madvr2-1.5.9/madvr/madvr.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 23:46:17.219762 py_madvr2-1.5.9/py_madvr2.egg-info/
--rw-r--r--   0 ilan       (501) staff       (20)      870 2024-04-19 23:46:17.000000 py_madvr2-1.5.9/py_madvr2.egg-info/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)      262 2024-04-19 23:46:17.000000 py_madvr2-1.5.9/py_madvr2.egg-info/SOURCES.txt
--rw-r--r--   0 ilan       (501) staff       (20)        1 2024-04-19 23:46:17.000000 py_madvr2-1.5.9/py_madvr2.egg-info/dependency_links.txt
--rw-r--r--   0 ilan       (501) staff       (20)       12 2024-04-19 23:46:17.000000 py_madvr2-1.5.9/py_madvr2.egg-info/top_level.txt
--rw-r--r--   0 ilan       (501) staff       (20)       38 2024-04-19 23:46:17.220188 py_madvr2-1.5.9/setup.cfg
--rw-r--r--   0 ilan       (501) staff       (20)      601 2024-04-19 23:46:10.000000 py_madvr2-1.5.9/setup.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 23:46:17.219505 py_madvr2-1.5.9/tests/
--rw-r--r--   0 ilan       (501) staff       (20)        0 2023-01-10 23:29:29.000000 py_madvr2-1.5.9/tests/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)     2159 2024-03-09 17:25:48.000000 py_madvr2-1.5.9/tests/testMadVR.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-20 00:11:02.454814 py_madvr2-1.5.91/
+-rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-01-10 23:29:29.000000 py_madvr2-1.5.91/LICENSE
+-rw-r--r--   0 ilan       (501) staff       (20)      871 2024-04-20 00:11:02.454599 py_madvr2-1.5.91/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)      472 2023-05-14 18:58:32.000000 py_madvr2-1.5.91/README.md
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-20 00:11:02.452931 py_madvr2-1.5.91/madvr/
+-rw-r--r--   0 ilan       (501) staff       (20)      230 2023-01-10 23:29:29.000000 py_madvr2-1.5.91/madvr/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)     3566 2023-07-02 16:13:13.000000 py_madvr2-1.5.91/madvr/commands.py
+-rw-r--r--   0 ilan       (501) staff       (20)      242 2023-01-14 01:34:27.000000 py_madvr2-1.5.91/madvr/errors.py
+-rw-r--r--   0 ilan       (501) staff       (20)    17237 2024-04-20 00:10:38.000000 py_madvr2-1.5.91/madvr/madvr.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-20 00:11:02.454391 py_madvr2-1.5.91/py_madvr2.egg-info/
+-rw-r--r--   0 ilan       (501) staff       (20)      871 2024-04-20 00:11:02.000000 py_madvr2-1.5.91/py_madvr2.egg-info/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)      262 2024-04-20 00:11:02.000000 py_madvr2-1.5.91/py_madvr2.egg-info/SOURCES.txt
+-rw-r--r--   0 ilan       (501) staff       (20)        1 2024-04-20 00:11:02.000000 py_madvr2-1.5.91/py_madvr2.egg-info/dependency_links.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       12 2024-04-20 00:11:02.000000 py_madvr2-1.5.91/py_madvr2.egg-info/top_level.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       38 2024-04-20 00:11:02.454867 py_madvr2-1.5.91/setup.cfg
+-rw-r--r--   0 ilan       (501) staff       (20)      602 2024-04-20 00:10:55.000000 py_madvr2-1.5.91/setup.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-20 00:11:02.454115 py_madvr2-1.5.91/tests/
+-rw-r--r--   0 ilan       (501) staff       (20)        0 2023-01-10 23:29:29.000000 py_madvr2-1.5.91/tests/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)     2159 2024-03-09 17:25:48.000000 py_madvr2-1.5.91/tests/testMadVR.py
```

### Comparing `py_madvr2-1.5.9/LICENSE` & `py_madvr2-1.5.91/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr2-1.5.9/PKG-INFO` & `py_madvr2-1.5.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr2
-Version: 1.5.9
+Version: 1.5.91
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr2-1.5.9/madvr/commands.py` & `py_madvr2-1.5.91/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr2-1.5.9/madvr/madvr.py` & `py_madvr2-1.5.91/madvr/madvr.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,14 +328,15 @@
                 msg = await asyncio.wait_for(
                     self.reader.read(self.read_limit),
                     timeout=self.command_read_timeout,
                 )
                 await self._process_notifications(msg.decode("utf-8"))
             except ConnectionResetError:
                 self.logger.debug("Connection reset by peer. Probably off")
+                await self.close_connection()
             except asyncio.TimeoutError as err:
                 # if no new notifications, just keep going
                 self.logger.debug("No new notifications to read: %s", err)
             except AttributeError as err:
                 self.logger.error("Attribute error with notifications: %s", err)
                 await self._reconnect()
                 continue
```

### Comparing `py_madvr2-1.5.9/py_madvr2.egg-info/PKG-INFO` & `py_madvr2-1.5.91/py_madvr2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr2
-Version: 1.5.9
+Version: 1.5.91
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr2-1.5.9/setup.py` & `py_madvr2-1.5.91/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr2",
-    version="1.5.9",
+    version="1.5.91",
     author="iloveicedgreentea2",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr2-1.5.9/tests/testMadVR.py` & `py_madvr2-1.5.91/tests/testMadVR.py`

 * *Files identical despite different names*

