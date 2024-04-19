# Comparing `tmp/py_madvr2-1.5.4.tar.gz` & `tmp/py_madvr2-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr2-1.5.4.tar", last modified: Sun Apr  7 23:30:55 2024, max compression
+gzip compressed data, was "py_madvr2-1.5.5.tar", last modified: Fri Apr 19 22:52:35 2024, max compression
```

## Comparing `py_madvr2-1.5.4.tar` & `py_madvr2-1.5.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-07 23:30:55.655390 py_madvr2-1.5.4/
--rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-01-10 23:29:29.000000 py_madvr2-1.5.4/LICENSE
--rw-r--r--   0 ilan       (501) staff       (20)      870 2024-04-07 23:30:55.655198 py_madvr2-1.5.4/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)      472 2023-05-14 18:58:32.000000 py_madvr2-1.5.4/README.md
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-07 23:30:55.653784 py_madvr2-1.5.4/madvr/
--rw-r--r--   0 ilan       (501) staff       (20)      230 2023-01-10 23:29:29.000000 py_madvr2-1.5.4/madvr/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)     3566 2023-07-02 16:13:13.000000 py_madvr2-1.5.4/madvr/commands.py
--rw-r--r--   0 ilan       (501) staff       (20)      242 2023-01-14 01:34:27.000000 py_madvr2-1.5.4/madvr/errors.py
--rw-r--r--   0 ilan       (501) staff       (20)    18430 2024-04-07 23:25:31.000000 py_madvr2-1.5.4/madvr/madvr.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-07 23:30:55.655002 py_madvr2-1.5.4/py_madvr2.egg-info/
--rw-r--r--   0 ilan       (501) staff       (20)      870 2024-04-07 23:30:55.000000 py_madvr2-1.5.4/py_madvr2.egg-info/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)      262 2024-04-07 23:30:55.000000 py_madvr2-1.5.4/py_madvr2.egg-info/SOURCES.txt
--rw-r--r--   0 ilan       (501) staff       (20)        1 2024-04-07 23:30:55.000000 py_madvr2-1.5.4/py_madvr2.egg-info/dependency_links.txt
--rw-r--r--   0 ilan       (501) staff       (20)       12 2024-04-07 23:30:55.000000 py_madvr2-1.5.4/py_madvr2.egg-info/top_level.txt
--rw-r--r--   0 ilan       (501) staff       (20)       38 2024-04-07 23:30:55.655432 py_madvr2-1.5.4/setup.cfg
--rw-r--r--   0 ilan       (501) staff       (20)      601 2024-04-07 22:48:41.000000 py_madvr2-1.5.4/setup.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-07 23:30:55.654742 py_madvr2-1.5.4/tests/
--rw-r--r--   0 ilan       (501) staff       (20)        0 2023-01-10 23:29:29.000000 py_madvr2-1.5.4/tests/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)     2159 2024-03-09 17:25:48.000000 py_madvr2-1.5.4/tests/testMadVR.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 22:52:35.400186 py_madvr2-1.5.5/
+-rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-01-10 23:29:29.000000 py_madvr2-1.5.5/LICENSE
+-rw-r--r--   0 ilan       (501) staff       (20)      870 2024-04-19 22:52:35.399969 py_madvr2-1.5.5/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)      472 2023-05-14 18:58:32.000000 py_madvr2-1.5.5/README.md
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 22:52:35.398364 py_madvr2-1.5.5/madvr/
+-rw-r--r--   0 ilan       (501) staff       (20)      230 2023-01-10 23:29:29.000000 py_madvr2-1.5.5/madvr/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)     3566 2023-07-02 16:13:13.000000 py_madvr2-1.5.5/madvr/commands.py
+-rw-r--r--   0 ilan       (501) staff       (20)      242 2023-01-14 01:34:27.000000 py_madvr2-1.5.5/madvr/errors.py
+-rw-r--r--   0 ilan       (501) staff       (20)    17055 2024-04-19 22:47:27.000000 py_madvr2-1.5.5/madvr/madvr.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 22:52:35.399750 py_madvr2-1.5.5/py_madvr2.egg-info/
+-rw-r--r--   0 ilan       (501) staff       (20)      870 2024-04-19 22:52:35.000000 py_madvr2-1.5.5/py_madvr2.egg-info/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)      262 2024-04-19 22:52:35.000000 py_madvr2-1.5.5/py_madvr2.egg-info/SOURCES.txt
+-rw-r--r--   0 ilan       (501) staff       (20)        1 2024-04-19 22:52:35.000000 py_madvr2-1.5.5/py_madvr2.egg-info/dependency_links.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       12 2024-04-19 22:52:35.000000 py_madvr2-1.5.5/py_madvr2.egg-info/top_level.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       38 2024-04-19 22:52:35.400242 py_madvr2-1.5.5/setup.cfg
+-rw-r--r--   0 ilan       (501) staff       (20)      601 2024-04-19 22:52:30.000000 py_madvr2-1.5.5/setup.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 22:52:35.399466 py_madvr2-1.5.5/tests/
+-rw-r--r--   0 ilan       (501) staff       (20)        0 2023-01-10 23:29:29.000000 py_madvr2-1.5.5/tests/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)     2159 2024-03-09 17:25:48.000000 py_madvr2-1.5.5/tests/testMadVR.py
```

### Comparing `py_madvr2-1.5.4/LICENSE` & `py_madvr2-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr2-1.5.4/PKG-INFO` & `py_madvr2-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr2
-Version: 1.5.4
+Version: 1.5.5
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr2-1.5.4/madvr/commands.py` & `py_madvr2-1.5.5/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr2-1.5.4/madvr/madvr.py` & `py_madvr2-1.5.5/madvr/madvr.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,17 +37,15 @@
         # stores all attributes
         self.msg_dict = {}
 
         # Sockets
         self.reader = None
         self.writer = None
 
-        self.is_closed = False
         # Envy does not have an are you on cmd, just assuming its on based on active connection
-        self.is_on = False
         self.read_limit = 8000
         self.command_read_timeout = 3
         # self.async_write_ha_state from HA
         self.update_callback = None
 
         self.logger.debug("Running in debug mode")
 
@@ -59,40 +57,42 @@
         Clear instance attr so HA doesn't report stale values
         """
         # Incoming attrs
         self.msg_dict = {}
 
     async def close_connection(self) -> None:
         """close the connection"""
+        self.logger.debug("closing connection")
         try:
             self.writer.close()
             await self.writer.wait_closed()
         except AttributeError:
             # means its already closed
             pass
-        self.logger.debug("self.writer is closed")
+        self.writer = None
         self.reader = None
-        self.is_closed = True
-        self.logger.debug("clearing connection event")
         self.connection_event.clear()
 
-        # Clear attr
-        self.logger.debug("clearing attr")
-        await self._clear_attr()
-        self.logger.debug("connection is closed")
-
     async def open_connection(self) -> None:
         """Open a connection"""
         self.logger.debug("Starting open connection")
         try:
             self.stop_reconnect.clear()
             await self._reconnect()
         except AckError as err:
             self.logger.error(err)
 
+    def connected(self) -> bool:
+        """Check if the client is connected"""
+        return self.reader is not None and self.writer is not None
+
+    def is_on(self) -> bool:
+        """Check if the client is on"""
+        return self.connected()  # its impossible to be connected and off
+
     def stop(self):
         """Stop reconnecting"""
         self.stop_reconnect.set()
 
     async def _reconnect(self) -> None:
         """
         Initiate keep-alive connection. This should handle any error and reconnect eventually.
@@ -102,47 +102,28 @@
         while not self.stop_reconnect.is_set():
             try:
                 self.logger.info("Connecting to Envy: %s:%s", self.host, self.port)
 
                 # Command client
                 self.reader, self.writer = await asyncio.wait_for(
                     asyncio.open_connection(self.host, self.port),
-                    timeout=2,
+                    timeout=5,
                 )
 
                 # Test heartbeat
                 self.logger.debug("Handshaking")
 
-                # its possible for the envy to output something while we connect, so this isnt reliable
-                # Make sure first message says WELCOME
-                # async with self.reader_lock:
-                #     msg_envy = await asyncio.wait_for(
-                #         self.reader.readline(),
-                #         timeout=10,
-                #     )
-
-                # Check if first 7 char match
-                # if self.MADVR_OK != msg_envy[:7]:
-                #     # This is fatal, and should not retry. If it doesn't respond as expected something is wrong
-                #     raise AckError(
-                #         f"Notification did not reply with correct greeting: {msg_envy}"
-                #     )
-
                 self.logger.info("Waiting for envy to be available")
                 # envy needs some time to setup new connections
                 await asyncio.sleep(3)
 
                 # handshake func
-                await self.send_heartbeat(True)
+                await self.send_heartbeat(once=True)
 
                 self.logger.info("Connection established")
-
-                self.is_on = True
-                self.is_closed = False
-
                 self.connection_event.set()
 
                 return
 
             except HeartBeatError:
                 self.logger.warning(
                     "Error sending heartbeat, retrying in %s seconds", 2
@@ -156,15 +137,17 @@
                 self.logger.debug("Connecting timeout, retrying in %s seconds", 2)
                 await asyncio.sleep(2)
                 continue
 
             # includes conn refused
             # backoff to not spam HA
             except OSError as err:
-                self.logger.warning("Connecting failed, retrying in %s seconds: %s", 2, err)
+                self.logger.warning(
+                    "Connecting failed, retrying in %s seconds: %s", 2, err
+                )
                 self.logger.debug(err)
                 await asyncio.sleep(2)
                 continue
 
     async def send_heartbeat(self, once=False) -> None:
         """
         Send a heartbeat to keep connection open
@@ -183,28 +166,29 @@
                 self.logger.error("timeout when sending heartbeat")
             except OSError:
                 self.logger.error("error when sending heartbeat")
                 await self._reconnect()
 
             return
 
-        while True:
+        # wait until connection is established
+        while not self.stop_reconnect.is_set():
             await self.connection_event.wait()
             # confirm can send heartbeat, ready for commands
             self.logger.debug("Sending heartbeats")
             try:
                 self.writer.write(self.HEARTBEAT)
                 await self.writer.drain()
 
                 self.logger.debug("heartbeat complete")
-            except asyncio.TimeoutError:
-                self.logger.error("timeout when sending heartbeat")
-            except OSError:
-                self.logger.error("error when sending heartbeat")
-                await self._reconnect()
+            except asyncio.TimeoutError as err:
+                self.logger.error("timeout when sending heartbeat %s", err)
+            except OSError as err:
+                self.logger.error("error when sending heartbeat %s", err)
+                # await self._reconnect()
             finally:
                 # Wait some time before the next heartbeat
                 await asyncio.sleep(15)
 
     async def _construct_command(self, raw_command: list[str]) -> tuple[bytes, str]:
         """
         Transform commands into their byte values from the string value
@@ -233,23 +217,20 @@
                 command, *raw_value = raw_command[0].split(",")
                 # remove space
                 values = [val.strip() for val in raw_value]
                 self.logger.debug("using command %s and values %s", command, values)
             # if valuerror it means theres just one command like PowerOff, so use that directly
             except ValueError as err:
                 self.logger.debug(err)
-                self.logger.debug("Using raw_command directly")
                 command = raw_command[0]
                 skip_val = True
         # if there are more than three values, this is incorrect, error
         elif len(raw_command) > 3:
-            self.logger.error("More than three command values provided.")
             raise NotImplementedError(f"Too many values provided {raw_command}")
         else:
-            self.logger.debug("command is a list")
             # else a command was provided as a proper list ['keypress', 'menu']
             # raw command will be a list of 2+
             command, *values = raw_command
 
         self.logger.debug("checking command %s", command)
 
         # Check if command is implemented
@@ -297,48 +278,46 @@
         Raises RetryExceededError
         """
 
         # Verify the command is supported
         try:
             cmd, enum_type = await self._construct_command(command)
         except NotImplementedError as err:
-            self.logger.error("command not implemented: %s -- %s", command, err)
+            self.logger.warning("command not implemented: %s -- %s", command, err)
             return f"Command not found: {command}"
 
         self.logger.debug("using values: %s %s", cmd, enum_type)
 
         # reconnect if client is not init or its off
-        if self.reader is None or self.is_on is False:
-            # Don't reconnect if poweroff or standby because HA will complain
-            if "PowerOff" in command or "Standby" in command:
-                return ""
-            self.logger.debug("Connection lost - restarting connection")
-            await self._reconnect()
+        # should not be necessary because of ping_until_alive
+        # if self.reader is None or self.is_on is False:
+        #     # Don't reconnect if poweroff or standby because HA will complain
+        #     if "PowerOff" in command or "Standby" in command:
+        #         return ""
+        #     self.logger.debug("Connection lost - restarting connection")
+        #     await self._reconnect()
 
         # simple retry logic
         retry_count = 0
 
         while retry_count < 5:
             try:
                 self.writer.write(cmd)
                 await self.writer.drain()
-                break  # if success, break the loop
-            except (asyncio.TimeoutError, OSError):
+                return "ok"  # if success, break the loop
+            except (asyncio.TimeoutError, OSError) as err:
                 self.logger.debug(
-                    "OK receipt timed out or connection failed when reading OK, retrying"
+                    "OK receipt timed out or connection failed when reading OK, retrying - %s",
+                    err,
                 )
                 retry_count += 1
-                await asyncio.sleep(1)  # sleep before retrying
+                await asyncio.sleep(0.2)  # sleep before retrying
                 continue
 
-        if retry_count == 5:  # if we got here something went wrong
-            await self.close_connection()
-            await self._reconnect()
-
-        return ""
+        raise RetryExceededError("Retry exceeded")
 
     async def read_notifications(self) -> None:
         """
         Read notifications from the server and update attributes
         """
         while True:
             # wait until the connection is established
@@ -427,32 +406,23 @@
                     self.update_callback()
                 # catch every possible error because python is a mess why can't you guarantee runtime behavior?
                 except Exception as err:
                     self.logger.error("Error updating HA: %s", err)
 
     async def power_off(self, standby=False) -> str:
         """
-        turn off madvr it must have a render thread active at the moment
-        once it is off, you can't turn it back on unless standby=True
-        It uses about 30w idle on standby. I use IR via harmony to turn it on
+        turn off madvr
 
         standby: bool -> standby instead of poweroff if true
         """
-        # dont do anything if its off besides mark it off
-        # sending command will open connection
         try:
             # stop trying to reconnect
-            self.logger.debug("setting stop reconnect")
             self.stop()
-            self.logger.debug("sending power off command")
             res = await self.send_command(["Standby"] if standby else ["PowerOff"])
-            self.logger.debug("closing connection")
             await self.close_connection()
-            self.is_on = False
-            self.logger.debug("finished power_off")
             return res
 
         except RetryExceededError:
             return "Retries Exceeded"
 
     def print_commands(self) -> str:
         """
```

### Comparing `py_madvr2-1.5.4/py_madvr2.egg-info/PKG-INFO` & `py_madvr2-1.5.5/py_madvr2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr2
-Version: 1.5.4
+Version: 1.5.5
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr2-1.5.4/setup.py` & `py_madvr2-1.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr2",
-    version="1.5.4",
+    version="1.5.5",
     author="iloveicedgreentea2",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr2-1.5.4/tests/testMadVR.py` & `py_madvr2-1.5.5/tests/testMadVR.py`

 * *Files identical despite different names*

