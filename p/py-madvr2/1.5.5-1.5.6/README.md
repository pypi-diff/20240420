# Comparing `tmp/py_madvr2-1.5.5.tar.gz` & `tmp/py_madvr2-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr2-1.5.5.tar", last modified: Fri Apr 19 22:52:35 2024, max compression
+gzip compressed data, was "py_madvr2-1.5.6.tar", last modified: Fri Apr 19 23:16:33 2024, max compression
```

## Comparing `py_madvr2-1.5.5.tar` & `py_madvr2-1.5.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 22:52:35.400186 py_madvr2-1.5.5/
--rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-01-10 23:29:29.000000 py_madvr2-1.5.5/LICENSE
--rw-r--r--   0 ilan       (501) staff       (20)      870 2024-04-19 22:52:35.399969 py_madvr2-1.5.5/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)      472 2023-05-14 18:58:32.000000 py_madvr2-1.5.5/README.md
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 22:52:35.398364 py_madvr2-1.5.5/madvr/
--rw-r--r--   0 ilan       (501) staff       (20)      230 2023-01-10 23:29:29.000000 py_madvr2-1.5.5/madvr/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)     3566 2023-07-02 16:13:13.000000 py_madvr2-1.5.5/madvr/commands.py
--rw-r--r--   0 ilan       (501) staff       (20)      242 2023-01-14 01:34:27.000000 py_madvr2-1.5.5/madvr/errors.py
--rw-r--r--   0 ilan       (501) staff       (20)    17055 2024-04-19 22:47:27.000000 py_madvr2-1.5.5/madvr/madvr.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 22:52:35.399750 py_madvr2-1.5.5/py_madvr2.egg-info/
--rw-r--r--   0 ilan       (501) staff       (20)      870 2024-04-19 22:52:35.000000 py_madvr2-1.5.5/py_madvr2.egg-info/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)      262 2024-04-19 22:52:35.000000 py_madvr2-1.5.5/py_madvr2.egg-info/SOURCES.txt
--rw-r--r--   0 ilan       (501) staff       (20)        1 2024-04-19 22:52:35.000000 py_madvr2-1.5.5/py_madvr2.egg-info/dependency_links.txt
--rw-r--r--   0 ilan       (501) staff       (20)       12 2024-04-19 22:52:35.000000 py_madvr2-1.5.5/py_madvr2.egg-info/top_level.txt
--rw-r--r--   0 ilan       (501) staff       (20)       38 2024-04-19 22:52:35.400242 py_madvr2-1.5.5/setup.cfg
--rw-r--r--   0 ilan       (501) staff       (20)      601 2024-04-19 22:52:30.000000 py_madvr2-1.5.5/setup.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 22:52:35.399466 py_madvr2-1.5.5/tests/
--rw-r--r--   0 ilan       (501) staff       (20)        0 2023-01-10 23:29:29.000000 py_madvr2-1.5.5/tests/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)     2159 2024-03-09 17:25:48.000000 py_madvr2-1.5.5/tests/testMadVR.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 23:16:33.514521 py_madvr2-1.5.6/
+-rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-01-10 23:29:29.000000 py_madvr2-1.5.6/LICENSE
+-rw-r--r--   0 ilan       (501) staff       (20)      870 2024-04-19 23:16:33.514257 py_madvr2-1.5.6/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)      472 2023-05-14 18:58:32.000000 py_madvr2-1.5.6/README.md
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 23:16:33.512537 py_madvr2-1.5.6/madvr/
+-rw-r--r--   0 ilan       (501) staff       (20)      230 2023-01-10 23:29:29.000000 py_madvr2-1.5.6/madvr/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)     3566 2023-07-02 16:13:13.000000 py_madvr2-1.5.6/madvr/commands.py
+-rw-r--r--   0 ilan       (501) staff       (20)      242 2023-01-14 01:34:27.000000 py_madvr2-1.5.6/madvr/errors.py
+-rw-r--r--   0 ilan       (501) staff       (20)    17188 2024-04-19 23:12:49.000000 py_madvr2-1.5.6/madvr/madvr.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 23:16:33.514039 py_madvr2-1.5.6/py_madvr2.egg-info/
+-rw-r--r--   0 ilan       (501) staff       (20)      870 2024-04-19 23:16:33.000000 py_madvr2-1.5.6/py_madvr2.egg-info/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)      262 2024-04-19 23:16:33.000000 py_madvr2-1.5.6/py_madvr2.egg-info/SOURCES.txt
+-rw-r--r--   0 ilan       (501) staff       (20)        1 2024-04-19 23:16:33.000000 py_madvr2-1.5.6/py_madvr2.egg-info/dependency_links.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       12 2024-04-19 23:16:33.000000 py_madvr2-1.5.6/py_madvr2.egg-info/top_level.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       38 2024-04-19 23:16:33.514578 py_madvr2-1.5.6/setup.cfg
+-rw-r--r--   0 ilan       (501) staff       (20)      601 2024-04-19 23:16:28.000000 py_madvr2-1.5.6/setup.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 23:16:33.513764 py_madvr2-1.5.6/tests/
+-rw-r--r--   0 ilan       (501) staff       (20)        0 2023-01-10 23:29:29.000000 py_madvr2-1.5.6/tests/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)     2159 2024-03-09 17:25:48.000000 py_madvr2-1.5.6/tests/testMadVR.py
```

### Comparing `py_madvr2-1.5.5/LICENSE` & `py_madvr2-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr2-1.5.5/PKG-INFO` & `py_madvr2-1.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr2
-Version: 1.5.5
+Version: 1.5.6
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr2-1.5.5/madvr/commands.py` & `py_madvr2-1.5.6/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr2-1.5.5/madvr/madvr.py` & `py_madvr2-1.5.6/madvr/madvr.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,18 +81,14 @@
         except AckError as err:
             self.logger.error(err)
 
     def connected(self) -> bool:
         """Check if the client is connected"""
         return self.reader is not None and self.writer is not None
 
-    def is_on(self) -> bool:
-        """Check if the client is on"""
-        return self.connected()  # its impossible to be connected and off
-
     def stop(self):
         """Stop reconnecting"""
         self.stop_reconnect.set()
 
     async def _reconnect(self) -> None:
         """
         Initiate keep-alive connection. This should handle any error and reconnect eventually.
@@ -300,14 +296,18 @@
         retry_count = 0
 
         while retry_count < 5:
             try:
                 self.writer.write(cmd)
                 await self.writer.drain()
                 return "ok"  # if success, break the loop
+            except ConnectionResetError:
+                # for now just assuming the envy was turned off
+                self.logger.warning("Connection reset by peer. Assuming envy was turned off manually")
+                raise RetryExceededError("Connection reset by peer")
             except (asyncio.TimeoutError, OSError) as err:
                 self.logger.debug(
                     "OK receipt timed out or connection failed when reading OK, retrying - %s",
                     err,
                 )
                 retry_count += 1
                 await asyncio.sleep(0.2)  # sleep before retrying
```

### Comparing `py_madvr2-1.5.5/py_madvr2.egg-info/PKG-INFO` & `py_madvr2-1.5.6/py_madvr2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr2
-Version: 1.5.5
+Version: 1.5.6
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr2-1.5.5/setup.py` & `py_madvr2-1.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr2",
-    version="1.5.5",
+    version="1.5.6",
     author="iloveicedgreentea2",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr2-1.5.5/tests/testMadVR.py` & `py_madvr2-1.5.6/tests/testMadVR.py`

 * *Files identical despite different names*

