# Comparing `tmp/ParendumLib-0.2.2.tar.gz` & `tmp/ParendumLib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ParendumLib-0.2.2.tar", last modified: Sat Apr 20 11:46:47 2024, max compression
+gzip compressed data, was "ParendumLib-0.2.3.tar", last modified: Sat Apr 20 13:21:37 2024, max compression
```

## Comparing `ParendumLib-0.2.2.tar` & `ParendumLib-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 11:46:47.402623 ParendumLib-0.2.2/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      220 2024-04-20 11:46:47.402623 ParendumLib-0.2.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 11:46:47.400622 ParendumLib-0.2.2/ParendumLib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      220 2024-04-20 11:46:47.000000 ParendumLib-0.2.2/ParendumLib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2024-04-20 11:46:47.000000 ParendumLib-0.2.2/ParendumLib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 11:46:47.000000 ParendumLib-0.2.2/ParendumLib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-20 11:46:47.000000 ParendumLib-0.2.2/ParendumLib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-20 11:46:47.000000 ParendumLib-0.2.2/ParendumLib.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1272 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 11:46:47.401622 ParendumLib-0.2.2/parendumlib/
--rw-rw-rw-   0 root         (0) root         (0)      215 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/parendumlib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 11:46:47.401622 ParendumLib-0.2.2/parendumlib/database/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/parendumlib/database/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3375 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/parendumlib/database/mongodb.py
--rw-rw-rw-   0 root         (0) root         (0)       53 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/parendumlib/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6063 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/parendumlib/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     4773 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/parendumlib/mailer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 11:46:47.402623 ParendumLib-0.2.2/parendumlib/permissions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/parendumlib/permissions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3179 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/parendumlib/permissions/mongodb.py
--rw-rw-rw-   0 root         (0) root         (0)     1447 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/parendumlib/responses.py
--rw-rw-rw-   0 root         (0) root         (0)     2133 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/parendumlib/utils.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 11:46:47.402623 ParendumLib-0.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-04-20 11:46:32.000000 ParendumLib-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 13:21:37.994555 ParendumLib-0.2.3/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-20 13:21:22.000000 ParendumLib-0.2.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      220 2024-04-20 13:21:37.994555 ParendumLib-0.2.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 13:21:37.992555 ParendumLib-0.2.3/ParendumLib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      220 2024-04-20 13:21:37.000000 ParendumLib-0.2.3/ParendumLib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2024-04-20 13:21:37.000000 ParendumLib-0.2.3/ParendumLib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 13:21:37.000000 ParendumLib-0.2.3/ParendumLib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-20 13:21:37.000000 ParendumLib-0.2.3/ParendumLib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-20 13:21:37.000000 ParendumLib-0.2.3/ParendumLib.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2024-04-20 13:21:22.000000 ParendumLib-0.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 13:21:37.993555 ParendumLib-0.2.3/parendumlib/
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-04-20 13:21:22.000000 ParendumLib-0.2.3/parendumlib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 13:21:37.993555 ParendumLib-0.2.3/parendumlib/database/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-20 13:21:22.000000 ParendumLib-0.2.3/parendumlib/database/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3375 2024-04-20 13:21:22.000000 ParendumLib-0.2.3/parendumlib/database/mongodb.py
+-rw-rw-rw-   0 root         (0) root         (0)       53 2024-04-20 13:21:22.000000 ParendumLib-0.2.3/parendumlib/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6493 2024-04-20 13:21:22.000000 ParendumLib-0.2.3/parendumlib/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     4773 2024-04-20 13:21:22.000000 ParendumLib-0.2.3/parendumlib/mailer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 13:21:37.993555 ParendumLib-0.2.3/parendumlib/permissions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-20 13:21:22.000000 ParendumLib-0.2.3/parendumlib/permissions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3179 2024-04-20 13:21:22.000000 ParendumLib-0.2.3/parendumlib/permissions/mongodb.py
+-rw-rw-rw-   0 root         (0) root         (0)     1447 2024-04-20 13:21:22.000000 ParendumLib-0.2.3/parendumlib/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)     2133 2024-04-20 13:21:22.000000 ParendumLib-0.2.3/parendumlib/utils.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 13:21:37.994555 ParendumLib-0.2.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-04-20 13:21:22.000000 ParendumLib-0.2.3/setup.py
```

### Comparing `ParendumLib-0.2.2/README.md` & `ParendumLib-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ParendumLib-0.2.2/parendumlib/database/mongodb.py` & `ParendumLib-0.2.3/parendumlib/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `ParendumLib-0.2.2/parendumlib/logger.py` & `ParendumLib-0.2.3/parendumlib/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 class Logger:
 
     def __init__(self, domain: str, api_key: str, api_secret: str, port: int = 443, log_file: str = None):
         self.protocol = "https" if port == 443 else "http"
         self.endpoint = f"{self.protocol}://{domain}:{port}"
         self.api_key = api_key
         self.api_secret = api_secret.encode()
+        self.pending = list()
+        self._start_thread()
 
         self.logger = logging.getLogger()
         self.logger.setLevel(logging.INFO)
 
         self.formatter = logging.Formatter('[%(asctime)s] [%(levelname)s] %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
 
         if log_file:
@@ -25,14 +27,29 @@
             self.file_handler.setFormatter(self.formatter)
             self.logger.addHandler(self.file_handler)
 
         self.console_handler = logging.StreamHandler()
         self.console_handler.setFormatter(self.formatter)
         self.logger.addHandler(self.console_handler)
 
+    def _start_thread(self):
+        thread = threading.Thread(target=self._send_pending)
+        thread.start()
+
+    def _send_pending(self):
+        while True:
+            if self.pending:
+                _pending = self.pending.pop()
+                try:
+                    self._log(*_pending)
+                    time.sleep(100)
+                except:
+                    time.sleep(500)
+            time.sleep(500)
+
     def _generate_signature(self, timestamp: str) -> str:
         """
         Generate HMAC signature using the provided timestamp.
 
         Args:
             timestamp (str): The timestamp to be used in signature generation.
 
@@ -84,27 +101,25 @@
             status_code=status_code or 0,
             elapsed_time=elapsed_time
         )
         if arguments:
             _new_log["arguments"] = arguments
         if content:
             _new_log["content"] = content
-        if hasattr(self.logger, level):
-            getattr(self.logger, level)(f"[{function}] {message}")
-        else:
-            self.logger.info(f"[{level}:{function}] {message}")
         if save:
             self._do_post(f"{self.endpoint}/api/logs/new", _new_log)
 
     def _do_log(self, level: str, function: str, message: str, status_code: int, elapsed_time: int = 1,
                 arguments: list = None, content: dict = None, save: bool = False):
-        thread = threading.Thread(target=self._log, args=(
-            level, function, message, status_code, elapsed_time, arguments, content, save,
-        ))
-        thread.start()
+        if save:
+            self.pending.append([level, function, message, status_code, elapsed_time, arguments, content, save])
+        if hasattr(self.logger, level):
+            getattr(self.logger, level)(f"[{function}] {message}")
+        else:
+            self.logger.info(f"[{level}:{function}] {message}")
 
     def log(self, level: str, message: str, status_code: int = 0, save: bool = False):
         stack = inspect.stack()
         caller_info = stack[1]
         caller_name = caller_info.function
         caller_line_no = caller_info.lineno
         self._do_log(level, f"{caller_name}():{caller_line_no}", message, status_code, save=save)
```

### Comparing `ParendumLib-0.2.2/parendumlib/mailer.py` & `ParendumLib-0.2.3/parendumlib/mailer.py`

 * *Files identical despite different names*

### Comparing `ParendumLib-0.2.2/parendumlib/permissions/mongodb.py` & `ParendumLib-0.2.3/parendumlib/permissions/mongodb.py`

 * *Files identical despite different names*

### Comparing `ParendumLib-0.2.2/parendumlib/responses.py` & `ParendumLib-0.2.3/parendumlib/responses.py`

 * *Files identical despite different names*

### Comparing `ParendumLib-0.2.2/parendumlib/utils.py` & `ParendumLib-0.2.3/parendumlib/utils.py`

 * *Files identical despite different names*

