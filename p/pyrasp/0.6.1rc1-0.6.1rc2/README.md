# Comparing `tmp/pyrasp-0.6.1rc1.tar.gz` & `tmp/pyrasp-0.6.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrasp-0.6.1rc1.tar", last modified: Wed Apr 17 06:31:01 2024, max compression
+gzip compressed data, was "pyrasp-0.6.1rc2.tar", last modified: Wed Apr 17 06:44:32 2024, max compression
```

## Comparing `pyrasp-0.6.1rc1.tar` & `pyrasp-0.6.1rc2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 06:31:01.094898 pyrasp-0.6.1rc1/
--rw-rw-rw-   0        0        0    35823 2024-04-17 06:30:52.000000 pyrasp-0.6.1rc1/LICENSE
--rw-rw-rw-   0        0        0    43607 2024-04-17 06:31:01.092698 pyrasp-0.6.1rc1/PKG-INFO
--rw-rw-rw-   0        0        0     1666 2024-04-17 06:30:52.000000 pyrasp-0.6.1rc1/README.md
--rw-rw-rw-   0        0        0      780 2024-04-17 06:30:52.000000 pyrasp-0.6.1rc1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-17 06:31:01.076408 pyrasp-0.6.1rc1/pyrasp/
--rw-rw-rw-   0        0        0        0 2024-04-17 06:30:52.000000 pyrasp-0.6.1rc1/pyrasp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:31:01.088034 pyrasp-0.6.1rc1/pyrasp/data/
--rw-rw-rw-   0        0        0   486969 2024-04-17 06:30:52.000000 pyrasp-0.6.1rc1/pyrasp/data/sqli_model-1.1.0
--rw-rw-rw-   0        0        0  1111448 2024-04-17 06:30:52.000000 pyrasp-0.6.1rc1/pyrasp/data/xss_model-1.2.0
--rw-rw-rw-   0        0        0    86378 2024-04-17 06:30:52.000000 pyrasp-0.6.1rc1/pyrasp/pyrasp.py
--rw-rw-rw-   0        0        0     6372 2024-04-17 06:30:52.000000 pyrasp-0.6.1rc1/pyrasp/pyrasp_data.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:31:01.090298 pyrasp-0.6.1rc1/pyrasp.egg-info/
--rw-rw-rw-   0        0        0    43607 2024-04-17 06:31:01.000000 pyrasp-0.6.1rc1/pyrasp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2024-04-17 06:31:01.000000 pyrasp-0.6.1rc1/pyrasp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 06:31:01.000000 pyrasp-0.6.1rc1/pyrasp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-17 06:31:01.000000 pyrasp-0.6.1rc1/pyrasp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-17 06:31:01.000000 pyrasp-0.6.1rc1/pyrasp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 06:31:01.094898 pyrasp-0.6.1rc1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 06:44:32.217777 pyrasp-0.6.1rc2/
+-rw-rw-rw-   0        0        0    35823 2024-04-17 06:44:24.000000 pyrasp-0.6.1rc2/LICENSE
+-rw-rw-rw-   0        0        0    43607 2024-04-17 06:44:32.215633 pyrasp-0.6.1rc2/PKG-INFO
+-rw-rw-rw-   0        0        0     1666 2024-04-17 06:44:24.000000 pyrasp-0.6.1rc2/README.md
+-rw-rw-rw-   0        0        0      780 2024-04-17 06:44:24.000000 pyrasp-0.6.1rc2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-17 06:44:32.195483 pyrasp-0.6.1rc2/pyrasp/
+-rw-rw-rw-   0        0        0        0 2024-04-17 06:44:24.000000 pyrasp-0.6.1rc2/pyrasp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:44:32.209278 pyrasp-0.6.1rc2/pyrasp/data/
+-rw-rw-rw-   0        0        0   486969 2024-04-17 06:44:24.000000 pyrasp-0.6.1rc2/pyrasp/data/sqli_model-1.1.0
+-rw-rw-rw-   0        0        0  1111448 2024-04-17 06:44:24.000000 pyrasp-0.6.1rc2/pyrasp/data/xss_model-1.2.0
+-rw-rw-rw-   0        0        0    87941 2024-04-17 06:44:24.000000 pyrasp-0.6.1rc2/pyrasp/pyrasp.py
+-rw-rw-rw-   0        0        0     6372 2024-04-17 06:44:24.000000 pyrasp-0.6.1rc2/pyrasp/pyrasp_data.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:44:32.213535 pyrasp-0.6.1rc2/pyrasp.egg-info/
+-rw-rw-rw-   0        0        0    43607 2024-04-17 06:44:32.000000 pyrasp-0.6.1rc2/pyrasp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2024-04-17 06:44:32.000000 pyrasp-0.6.1rc2/pyrasp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 06:44:32.000000 pyrasp-0.6.1rc2/pyrasp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-17 06:44:32.000000 pyrasp-0.6.1rc2/pyrasp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-17 06:44:32.000000 pyrasp-0.6.1rc2/pyrasp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 06:44:32.217777 pyrasp-0.6.1rc2/setup.cfg
```

### Comparing `pyrasp-0.6.1rc1/LICENSE` & `pyrasp-0.6.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrasp-0.6.1rc1/PKG-INFO` & `pyrasp-0.6.1rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrasp
-Version: 0.6.1rc1
+Version: 0.6.1rc2
 Summary: Python RASP
 Author-email: Renaud Bidou <renaud@paracyberbellum.io>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pyrasp-0.6.1rc1/README.md` & `pyrasp-0.6.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `pyrasp-0.6.1rc1/pyproject.toml` & `pyrasp-0.6.1rc2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyrasp"
-version = "0.6.1rc1"
+version = "0.6.1rc2"
 authors = [
     { name = "Renaud Bidou", email = "renaud@paracyberbellum.io" }
 ]
 description = "Python RASP"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `pyrasp-0.6.1rc1/pyrasp/data/sqli_model-1.1.0` & `pyrasp-0.6.1rc2/pyrasp/data/sqli_model-1.1.0`

 * *Files identical despite different names*

### Comparing `pyrasp-0.6.1rc1/pyrasp/data/xss_model-1.2.0` & `pyrasp-0.6.1rc2/pyrasp/data/xss_model-1.2.0`

 * *Files identical despite different names*

### Comparing `pyrasp-0.6.1rc1/pyrasp/pyrasp.py` & `pyrasp-0.6.1rc2/pyrasp/pyrasp.py`

 * *Files 1% similar despite different names*

```diff
@@ -2698,9 +2698,52 @@
 
         else:
             content = response
             status_code = 200
 
         return (content, status_code)
     
+    ####################################################
+    # LOGGING
+    ####################################################
+
+    def log_security_event(self, event_type, source_ip, user = None, details = {}):
+
+        log_data = make_security_log(self.APP_NAME, event_type, source_ip, self.LOG_FORMAT, user, details, False)
+        
+        webhook = False
+        syslog_udp = False
+        syslog_tcp = False
+
+        if self.LOG_FORMAT.lower() in ['json', 'pcb']:
+            path = self.LOG_PATH
+            if not path.startswith('/'):
+                path = '/'+path
+            server_url = f'{self.LOG_PROTOCOL.lower()}://{self.LOG_SERVER}:{self.LOG_PORT}{path}'
+            webhook = True
+
+        elif self.LOG_FORMAT.lower() == 'syslog':
+            if self.LOG_PROTOCOL.lower() == 'udp':
+                syslog_udp = True
+                sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+            elif self.LOG_PROTOCOL.lower() == 'tcp':
+                syslog_tcp = True
+                sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+
+        try:
+            if webhook:
+                requests.post(server_url, json=log_data, timeout=1) 
+            elif syslog_udp:
+                sock.sendto(log_data.encode(), (self.LOG_SERVER, self.LOG_PORT))
+            elif syslog_tcp:
+                sock.connect((self.LOG_SERVER, self.LOG_PORT))
+                sock.settimeout(1)
+                sock.send(log_data)
+                sock.close()
+
+        except:
+            pass
+
+
+
```

### Comparing `pyrasp-0.6.1rc1/pyrasp/pyrasp_data.py` & `pyrasp-0.6.1rc2/pyrasp/pyrasp_data.py`

 * *Files identical despite different names*

### Comparing `pyrasp-0.6.1rc1/pyrasp.egg-info/PKG-INFO` & `pyrasp-0.6.1rc2/pyrasp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrasp
-Version: 0.6.1rc1
+Version: 0.6.1rc2
 Summary: Python RASP
 Author-email: Renaud Bidou <renaud@paracyberbellum.io>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

