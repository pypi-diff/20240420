# Comparing `tmp/py_madvr2-1.5.7.tar.gz` & `tmp/py_madvr2-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr2-1.5.7.tar", last modified: Fri Apr 19 23:26:22 2024, max compression
+gzip compressed data, was "py_madvr2-1.5.8.tar", last modified: Fri Apr 19 23:35:27 2024, max compression
```

## Comparing `py_madvr2-1.5.7.tar` & `py_madvr2-1.5.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 23:26:22.507079 py_madvr2-1.5.7/
--rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-01-10 23:29:29.000000 py_madvr2-1.5.7/LICENSE
--rw-r--r--   0 ilan       (501) staff       (20)      870 2024-04-19 23:26:22.506877 py_madvr2-1.5.7/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)      472 2023-05-14 18:58:32.000000 py_madvr2-1.5.7/README.md
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 23:26:22.505232 py_madvr2-1.5.7/madvr/
--rw-r--r--   0 ilan       (501) staff       (20)      230 2023-01-10 23:29:29.000000 py_madvr2-1.5.7/madvr/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)     3566 2023-07-02 16:13:13.000000 py_madvr2-1.5.7/madvr/commands.py
--rw-r--r--   0 ilan       (501) staff       (20)      242 2023-01-14 01:34:27.000000 py_madvr2-1.5.7/madvr/errors.py
--rw-r--r--   0 ilan       (501) staff       (20)    17150 2024-04-19 23:23:02.000000 py_madvr2-1.5.7/madvr/madvr.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 23:26:22.506646 py_madvr2-1.5.7/py_madvr2.egg-info/
--rw-r--r--   0 ilan       (501) staff       (20)      870 2024-04-19 23:26:22.000000 py_madvr2-1.5.7/py_madvr2.egg-info/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)      262 2024-04-19 23:26:22.000000 py_madvr2-1.5.7/py_madvr2.egg-info/SOURCES.txt
--rw-r--r--   0 ilan       (501) staff       (20)        1 2024-04-19 23:26:22.000000 py_madvr2-1.5.7/py_madvr2.egg-info/dependency_links.txt
--rw-r--r--   0 ilan       (501) staff       (20)       12 2024-04-19 23:26:22.000000 py_madvr2-1.5.7/py_madvr2.egg-info/top_level.txt
--rw-r--r--   0 ilan       (501) staff       (20)       38 2024-04-19 23:26:22.507125 py_madvr2-1.5.7/setup.cfg
--rw-r--r--   0 ilan       (501) staff       (20)      601 2024-04-19 23:26:17.000000 py_madvr2-1.5.7/setup.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 23:26:22.506359 py_madvr2-1.5.7/tests/
--rw-r--r--   0 ilan       (501) staff       (20)        0 2023-01-10 23:29:29.000000 py_madvr2-1.5.7/tests/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)     2159 2024-03-09 17:25:48.000000 py_madvr2-1.5.7/tests/testMadVR.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 23:35:27.183840 py_madvr2-1.5.8/
+-rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-01-10 23:29:29.000000 py_madvr2-1.5.8/LICENSE
+-rw-r--r--   0 ilan       (501) staff       (20)      870 2024-04-19 23:35:27.183671 py_madvr2-1.5.8/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)      472 2023-05-14 18:58:32.000000 py_madvr2-1.5.8/README.md
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 23:35:27.182224 py_madvr2-1.5.8/madvr/
+-rw-r--r--   0 ilan       (501) staff       (20)      230 2023-01-10 23:29:29.000000 py_madvr2-1.5.8/madvr/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)     3566 2023-07-02 16:13:13.000000 py_madvr2-1.5.8/madvr/commands.py
+-rw-r--r--   0 ilan       (501) staff       (20)      242 2023-01-14 01:34:27.000000 py_madvr2-1.5.8/madvr/errors.py
+-rw-r--r--   0 ilan       (501) staff       (20)    17121 2024-04-19 23:34:54.000000 py_madvr2-1.5.8/madvr/madvr.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 23:35:27.183498 py_madvr2-1.5.8/py_madvr2.egg-info/
+-rw-r--r--   0 ilan       (501) staff       (20)      870 2024-04-19 23:35:27.000000 py_madvr2-1.5.8/py_madvr2.egg-info/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)      262 2024-04-19 23:35:27.000000 py_madvr2-1.5.8/py_madvr2.egg-info/SOURCES.txt
+-rw-r--r--   0 ilan       (501) staff       (20)        1 2024-04-19 23:35:27.000000 py_madvr2-1.5.8/py_madvr2.egg-info/dependency_links.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       12 2024-04-19 23:35:27.000000 py_madvr2-1.5.8/py_madvr2.egg-info/top_level.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       38 2024-04-19 23:35:27.183882 py_madvr2-1.5.8/setup.cfg
+-rw-r--r--   0 ilan       (501) staff       (20)      601 2024-04-19 23:35:21.000000 py_madvr2-1.5.8/setup.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 23:35:27.183184 py_madvr2-1.5.8/tests/
+-rw-r--r--   0 ilan       (501) staff       (20)        0 2023-01-10 23:29:29.000000 py_madvr2-1.5.8/tests/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)     2159 2024-03-09 17:25:48.000000 py_madvr2-1.5.8/tests/testMadVR.py
```

### Comparing `py_madvr2-1.5.7/LICENSE` & `py_madvr2-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr2-1.5.7/PKG-INFO` & `py_madvr2-1.5.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr2
-Version: 1.5.7
+Version: 1.5.8
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr2-1.5.7/madvr/commands.py` & `py_madvr2-1.5.8/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr2-1.5.7/madvr/madvr.py` & `py_madvr2-1.5.8/madvr/madvr.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,15 +298,17 @@
         while retry_count < 5:
             try:
                 self.writer.write(cmd)
                 await self.writer.drain()
                 return "ok"  # if success, break the loop
             except ConnectionResetError as err:
                 # for now just assuming the envy was turned off
-                self.logger.warning("Connection reset by peer. Assuming envy was turned off manually")
+                self.logger.warning(
+                    "Connection reset by peer. Assuming envy was turned off manually"
+                )
                 raise ConnectionResetError("Connection reset by peer") from err
             except (asyncio.TimeoutError, OSError) as err:
                 self.logger.debug(
                     "OK receipt timed out or connection failed when reading OK, retrying - %s",
                     err,
                 )
                 retry_count += 1
@@ -323,34 +325,30 @@
             # wait until the connection is established
             await self.connection_event.wait()
             try:
                 msg = await asyncio.wait_for(
                     self.reader.read(self.read_limit),
                     timeout=self.command_read_timeout,
                 )
+                await self._process_notifications(msg.decode("utf-8"))
             except ConnectionResetError:
-                self.logger.debug(
-                    "Connection reset by peer. Probably off"
-                )
+                self.logger.debug("Connection reset by peer. Probably off")
             except asyncio.TimeoutError as err:
                 # if no new notifications, just keep going
                 self.logger.debug("No new notifications to read: %s", err)
             except AttributeError as err:
                 self.logger.error("Attribute error with notifications: %s", err)
                 await self._reconnect()
                 continue
             except OSError as err:
                 self.logger.error("Reading notifications failed or timed out: %s", err)
                 continue
 
-            if not msg:
-                await asyncio.sleep(0.1)
-                continue
-
-            await self._process_notifications(msg.decode("utf-8"))
+            await asyncio.sleep(0.1)
+            continue
 
     async def _process_notifications(self, msg: str) -> None:
         """Parse a message and store the attributes and values in a dictionary"""
         self.logger.debug("Processing notifications: %s", msg)
         notifications = msg.split("\r\n")
         # for each /r/n split it by title, then the rest are values
         for notification in notifications:
```

### Comparing `py_madvr2-1.5.7/py_madvr2.egg-info/PKG-INFO` & `py_madvr2-1.5.8/py_madvr2.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr2
-Version: 1.5.7
+Version: 1.5.8
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr2-1.5.7/setup.py` & `py_madvr2-1.5.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr2",
-    version="1.5.7",
+    version="1.5.8",
     author="iloveicedgreentea2",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr2-1.5.7/tests/testMadVR.py` & `py_madvr2-1.5.8/tests/testMadVR.py`

 * *Files identical despite different names*

