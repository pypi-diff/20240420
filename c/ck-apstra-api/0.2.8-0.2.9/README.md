# Comparing `tmp/ck_apstra_api-0.2.8.tar.gz` & `tmp/ck_apstra_api-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ck_apstra_api-0.2.8.tar", max compression
+gzip compressed data, was "ck_apstra_api-0.2.9.tar", max compression
```

## Comparing `ck_apstra_api-0.2.8.tar` & `ck_apstra_api-0.2.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-09-28 00:59:26.688335 ck_apstra_api-0.2.8/LICENSE
--rw-r--r--   0        0        0     1226 2023-11-24 23:30:58.367886 ck_apstra_api-0.2.8/README.md
--rw-r--r--   0        0        0     1158 2023-12-08 00:57:36.904475 ck_apstra_api-0.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-09-28 01:27:34.624568 ck_apstra_api-0.2.8/src/ck_apstra_api/__init__.py
--rwxr-xr-x   0        0        0    29965 2023-11-29 15:31:31.415103 ck_apstra_api-0.2.8/src/ck_apstra_api/apstra_blueprint.py
--rwxr-xr-x   0        0        0     7582 2023-12-08 00:56:05.725552 ck_apstra_api-0.2.8/src/ck_apstra_api/apstra_session.py
--rw-r--r--   0        0        0     9265 2023-11-29 15:30:29.638239 ck_apstra_api-0.2.8/src/ck_apstra_api/cli.py
--rw-r--r--   0        0        0    24400 2023-10-08 05:14:40.501949 ck_apstra_api-0.2.8/src/ck_apstra_api/generic_system.py
--rw-r--r--   0        0        0    11866 2023-10-23 01:37:34.339126 ck_apstra_api-0.2.8/src/ck_apstra_api/ip_endpoint.py
--rw-r--r--   0        0        0     2346 2023-11-17 18:23:57.618869 ck_apstra_api-0.2.8/src/ck_apstra_api/pull_device_configuration.py
--rw-r--r--   0        0        0     1961 1970-01-01 00:00:00.000000 ck_apstra_api-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-09-28 00:59:26.688335 ck_apstra_api-0.2.9/LICENSE
+-rw-r--r--   0        0        0     1226 2023-11-24 23:30:58.367886 ck_apstra_api-0.2.9/README.md
+-rw-r--r--   0        0        0     1158 2023-12-09 00:15:06.151366 ck_apstra_api-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-09-28 01:27:34.624568 ck_apstra_api-0.2.9/src/ck_apstra_api/__init__.py
+-rwxr-xr-x   0        0        0    29965 2023-11-29 15:31:31.415103 ck_apstra_api-0.2.9/src/ck_apstra_api/apstra_blueprint.py
+-rwxr-xr-x   0        0        0     7944 2023-12-09 00:16:53.341642 ck_apstra_api-0.2.9/src/ck_apstra_api/apstra_session.py
+-rw-r--r--   0        0        0     9265 2023-11-29 15:30:29.638239 ck_apstra_api-0.2.9/src/ck_apstra_api/cli.py
+-rw-r--r--   0        0        0    24400 2023-10-08 05:14:40.501949 ck_apstra_api-0.2.9/src/ck_apstra_api/generic_system.py
+-rw-r--r--   0        0        0    11866 2023-10-23 01:37:34.339126 ck_apstra_api-0.2.9/src/ck_apstra_api/ip_endpoint.py
+-rw-r--r--   0        0        0     2346 2023-11-17 18:23:57.618869 ck_apstra_api-0.2.9/src/ck_apstra_api/pull_device_configuration.py
+-rw-r--r--   0        0        0     1961 1970-01-01 00:00:00.000000 ck_apstra_api-0.2.9/PKG-INFO
```

### Comparing `ck_apstra_api-0.2.8/LICENSE` & `ck_apstra_api-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ck_apstra_api-0.2.8/README.md` & `ck_apstra_api-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ck_apstra_api-0.2.8/pyproject.toml` & `ck_apstra_api-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ck-apstra-api"
-version = "0.2.8"
+version = "0.2.9"
 description = "An implementation to use Apstra API"
 authors = [ "Charlie Kim <ckim@juniper.net>" ]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "<3.13,>=3.9"
```

### Comparing `ck_apstra_api-0.2.8/src/ck_apstra_api/apstra_blueprint.py` & `ck_apstra_api-0.2.9/src/ck_apstra_api/apstra_blueprint.py`

 * *Files identical despite different names*

### Comparing `ck_apstra_api-0.2.8/src/ck_apstra_api/apstra_session.py` & `ck_apstra_api-0.2.9/src/ck_apstra_api/apstra_session.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,18 +91,28 @@
             return
         else:
             self.last_error = response.content
             self.logger.error(f"login failed: {self.last_error}")
             return
 
     def logout(self) -> None:
+        self.token = None
         url = f"{self.url_prefix}/aaa/logout"
         response = self.post(url, None)
         # the status code is 404 (not found) if the logout is successful
         return response
+    
+    def is_online(self) -> bool:
+        """
+        Check if the Apstra controller is online.
+
+        Returns:
+            True if the Apstra controller is online, False otherwise.
+        """
+        return self.token is not None
 
     def get_device_profile(self, device_profile_name: str = None) -> dict:
         """
         Get the device profile with the specified name.
 
         Args:
             name: The name of the device profile.
@@ -229,9 +239,13 @@
     apstra_server_port = os.getenv('apstra_server_port')
     apstra_server_username = os.getenv('apstra_server_username')
     apstra_server_password = os.getenv('apstra_server_password')
 
     apstra = CkApstraSession(apstra_server_host, apstra_server_port, apstra_server_username, apstra_server_password)
     apstra.print_token()
 
+    logging.info(f"Done {apstra.is_online()=}")
+
     logouted = apstra.logout()
     logging.info(f"Done {logouted=}")
+
+    logging.info(f"Done {apstra.is_online()=}")
```

### Comparing `ck_apstra_api-0.2.8/src/ck_apstra_api/cli.py` & `ck_apstra_api-0.2.9/src/ck_apstra_api/cli.py`

 * *Files identical despite different names*

### Comparing `ck_apstra_api-0.2.8/src/ck_apstra_api/generic_system.py` & `ck_apstra_api-0.2.9/src/ck_apstra_api/generic_system.py`

 * *Files identical despite different names*

### Comparing `ck_apstra_api-0.2.8/src/ck_apstra_api/ip_endpoint.py` & `ck_apstra_api-0.2.9/src/ck_apstra_api/ip_endpoint.py`

 * *Files identical despite different names*

### Comparing `ck_apstra_api-0.2.8/src/ck_apstra_api/pull_device_configuration.py` & `ck_apstra_api-0.2.9/src/ck_apstra_api/pull_device_configuration.py`

 * *Files identical despite different names*

### Comparing `ck_apstra_api-0.2.8/PKG-INFO` & `ck_apstra_api-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ck-apstra-api
-Version: 0.2.8
+Version: 0.2.9
 Summary: An implementation to use Apstra API
 License: MIT
 Author: Charlie Kim
 Author-email: ckim@juniper.net
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

