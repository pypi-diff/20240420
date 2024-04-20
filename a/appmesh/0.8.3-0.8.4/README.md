# Comparing `tmp/appmesh-0.8.3-py3-none-any.whl.zip` & `tmp/appmesh-0.8.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 15203 bytes, number of entries: 6
--rw-r--r--  2.0 unx       11 b- defN 24-Mar-24 23:25 appmesh/__init__.py
--rw-r--r--  2.0 unx    54470 b- defN 24-Mar-24 23:25 appmesh/appmesh_client.py
--rw-r--r--  2.0 unx    10746 b- defN 24-Mar-24 23:25 appmesh-0.8.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-24 23:25 appmesh-0.8.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Mar-24 23:25 appmesh-0.8.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      455 b- defN 24-Mar-24 23:25 appmesh-0.8.3.dist-info/RECORD
-6 files, 65782 bytes uncompressed, 14381 bytes compressed:  78.1%
+Zip file size: 15369 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-19 12:19 appmesh/__init__.py
+-rw-r--r--  2.0 unx    55928 b- defN 24-Apr-19 12:19 appmesh/appmesh_client.py
+-rw-r--r--  2.0 unx    10786 b- defN 24-Apr-19 12:19 appmesh-0.8.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 12:19 appmesh-0.8.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-19 12:19 appmesh-0.8.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      455 b- defN 24-Apr-19 12:19 appmesh-0.8.4.dist-info/RECORD
+6 files, 67280 bytes uncompressed, 14547 bytes compressed:  78.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: appmesh/__init__.py
 Comment: 
 
 Filename: appmesh/appmesh_client.py
 Comment: 
 
-Filename: appmesh-0.8.3.dist-info/METADATA
+Filename: appmesh-0.8.4.dist-info/METADATA
 Comment: 
 
-Filename: appmesh-0.8.3.dist-info/WHEEL
+Filename: appmesh-0.8.4.dist-info/WHEEL
 Comment: 
 
-Filename: appmesh-0.8.3.dist-info/top_level.txt
+Filename: appmesh-0.8.4.dist-info/top_level.txt
 Comment: 
 
-Filename: appmesh-0.8.3.dist-info/RECORD
+Filename: appmesh-0.8.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## appmesh/appmesh_client.py

```diff
@@ -316,43 +316,59 @@
             token (str): _description_
         """
         self.__jwt_token = token
 
     ########################################
     # Security
     ########################################
-    def login(self, user_name: str, user_pwd: str, timeout_seconds=DEFAULT_TOKEN_EXPIRE_SECONDS) -> str:
+    def login(self, user_name: str, user_pwd: str, totp_key="", timeout_seconds=DEFAULT_TOKEN_EXPIRE_SECONDS) -> str:
         """Login with user name and password
 
         Args:
             user_name (str): the name of the user.
             user_pwd (str): the password of the user.
+            totp_key (str, optional): the TOTP key if enabled for the user.
             timeout_seconds (int | str, optional): token expire timeout of seconds. support ISO 8601 durations (e.g., 'P1Y2M3DT4H5M6S' 'P1W').
 
         Returns:
             str: JWT token if verify success, otherwise return None.
         """
         self.jwt_token = None
         resp = self._request_http(
             AppMeshClient.Method.POST,
             path="/appmesh/login",
             header={
                 "Username": base64.b64encode(user_name.encode()),
                 "Password": base64.b64encode(user_pwd.encode()),
+                "Totp": base64.b64encode(totp_key.encode()),
                 "Expire-Seconds": self._parse_duration(timeout_seconds),
             },
         )
         if resp.status_code == HTTPStatus.OK:
             if "Access-Token" in resp.json():
                 self.jwt_token = resp.json()["Access-Token"]
         else:
             print(resp.text)
             # resp.raise_for_status()
         return self.jwt_token
 
+    def logoff(self) -> bool:
+        """Logoff current session from server
+
+        Returns:
+            bool: logoff success or failure.
+        """
+        resp = self._request_http(AppMeshClient.Method.POST, path="/appmesh/self/logoff")
+        if resp.status_code == HTTPStatus.OK:
+            return True
+        else:
+            # resp.raise_for_status()
+            print(resp.text)
+            return False
+
     def authentication(self, token: str, permission=None) -> bool:
         """Login with token and verify permission when specified
 
         Args:
             token (str): JWT token returned from login().
             permission (str, optional): the permission ID used to verify the token user
                 permission ID can be:
@@ -370,14 +386,39 @@
         if resp.status_code == HTTPStatus.OK:
             return True
         else:
             # resp.raise_for_status()
             print(resp.text)
             return False
 
+    def renew(self, timeout_seconds=DEFAULT_TOKEN_EXPIRE_SECONDS) -> str:
+        """Renew current token
+
+        Args:
+            timeout_seconds (int | str, optional): token expire timeout of seconds. support ISO 8601 durations (e.g., 'P1Y2M3DT4H5M6S' 'P1W').
+
+        Returns:
+            str: The new JWT token if renew success, otherwise return None.
+        """
+        assert self.jwt_token
+        resp = self._request_http(
+            AppMeshClient.Method.POST,
+            path="/appmesh/token/renew",
+            header={
+                "Expire-Seconds": self._parse_duration(timeout_seconds),
+            },
+        )
+        if resp.status_code == HTTPStatus.OK:
+            if "Access-Token" in resp.json():
+                self.jwt_token = resp.json()["Access-Token"]
+        else:
+            print(resp.text)
+            # resp.raise_for_status()
+        return self.jwt_token
+
     ########################################
     # Application view
     ########################################
     def app_view(self, app_name: str) -> App:
         """Get one application information
 
         Args:
@@ -1034,17 +1075,15 @@
         """
         exit_code = None
         if run:
             output_position = 0
             start = datetime.now()
             interval = 1 if self.__class__.__name__ == "AppMeshClient" else 1000
             while len(run.proc_uid) > 0:
-                success, output, position, exit_code = self.app_output(
-                    app_name=run.app_name, stdout_position=output_position, stdout_index=0, process_uuid=run.proc_uid, timeout=interval
-                )
+                success, output, position, exit_code = self.app_output(app_name=run.app_name, stdout_position=output_position, stdout_index=0, process_uuid=run.proc_uid, timeout=interval)
                 if output and stdout_print:
                     print(output, end="")
                 if position is not None:
                     output_position = position
                 if exit_code is not None:
                     # success
                     self.app_delete(run.app_name)
@@ -1110,15 +1149,17 @@
         if self.jwt_token:
             header["Authorization"] = "Bearer " + self.jwt_token
         header[HTTP_USER_AGENT_HEADER_NAME] = HTTP_USER_AGENT
 
         if method is AppMeshClient.Method.GET:
             return requests.get(url=rest_url, params=query, headers=header, cert=self.ssl_client_cert, verify=self.ssl_verify, timeout=self.rest_timeout)
         elif method is AppMeshClient.Method.POST:
-            return requests.post(url=rest_url, params=query, headers=header, data=json.dumps(body) if type(body) in (dict, list) else body, cert=self.ssl_client_cert, verify=self.ssl_verify, timeout=self.rest_timeout)
+            return requests.post(
+                url=rest_url, params=query, headers=header, data=json.dumps(body) if type(body) in (dict, list) else body, cert=self.ssl_client_cert, verify=self.ssl_verify, timeout=self.rest_timeout
+            )
         elif method is AppMeshClient.Method.POST_STREAM:
             return requests.post(
                 url=rest_url,
                 params=query,
                 headers=header,
                 data=body,
                 cert=self.ssl_client_cert,
```

## Comparing `appmesh-0.8.3.dist-info/METADATA` & `appmesh-0.8.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appmesh
-Version: 0.8.3
+Version: 0.8.4
 Summary: Client SDK for App Mesh
 Home-page: https://github.com/laoshanxi/app-mesh
 Author: laoshanxi
 Author-email: 178029200@qq.com
 License: MIT
 Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3
@@ -116,18 +116,19 @@
 
 ---
 
 ## Library dependency
 
 - [MessagePack](https://msgpack.org/)
 - [boostorg/boost](https://github.com/boostorg/boost)
-- [DOCGroup/ACE_TAO/ACE](https://github.com/DOCGroup/ACE_TAO)
+- [ACE_TAO/ACE](https://github.com/DOCGroup/ACE_TAO)
 - [curlpp](https://github.com/jpbarrette/curlpp)
 - [Thalhammer/jwt-cpp](https://github.com/Thalhammer/jwt-cpp)
 - [nlohmann/json](https://json.nlohmann.me)
+- [yaml-cpp](https://github.com/jbeder/yaml-cpp)
 - [nfpm](https://github.com/goreleaser/nfpm)
 - [jupp0r/prometheus-cpp](https://github.com/jupp0r/prometheus-cpp)
 - [zemasoft/wildcards](https://github.com/zemasoft/wildcards)
 - [mariusbancila/croncpp](https://github.com/mariusbancila/croncpp)
 - [log4cpp](http://log4cpp.sourceforge.net)
 - [Crypto++](https://www.cryptopp.com)
 - [ldap-cpp](https://github.com/AndreyBarmaley/ldap-cpp)
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: appmesh Version: 0.8.3 Summary: Client SDK for App
+Metadata-Version: 2.1 Name: appmesh Version: 0.8.4 Summary: Client SDK for App
 Mesh Home-page: https://github.com/laoshanxi/app-mesh Author: laoshanxi Author-
 email: 178029200@qq.com License: MIT Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown Requires-Dist:
 requests Requires-Dist: msgpack Requires-Dist: requests-toolbelt Requires-Dist:
 aniso8601 ï»¿[![language.badge]][language.url] [![standard.badge]]
@@ -107,30 +107,30 @@
 secure_REST_file_server.html) - [Standalone JWT server](https://app-
 mesh.readthedocs.io/en/latest/success/standalone_JWT_server.html) - [Kubernetes
 run none-container applications](https://app-mesh.readthedocs.io/en/latest/
 success/kubernetes_run_native_application.html) - [Remote execute](https://app-
 mesh.readthedocs.io/en/latest/success/remote_run_cli_and_python.html) - [Python
 parallel run](https://app-mesh.readthedocs.io/en/latest/success/
 python_parallel_run.html) --- ## Library dependency - [MessagePack](https://
-msgpack.org/) - [boostorg/boost](https://github.com/boostorg/boost) -
-[DOCGroup/ACE_TAO/ACE](https://github.com/DOCGroup/ACE_TAO) - [curlpp](https://
-github.com/jpbarrette/curlpp) - [Thalhammer/jwt-cpp](https://github.com/
-Thalhammer/jwt-cpp) - [nlohmann/json](https://json.nlohmann.me) - [nfpm](https:
-//github.com/goreleaser/nfpm) - [jupp0r/prometheus-cpp](https://github.com/
-jupp0r/prometheus-cpp) - [zemasoft/wildcards](https://github.com/zemasoft/
-wildcards) - [mariusbancila/croncpp](https://github.com/mariusbancila/croncpp)
-- [log4cpp](http://log4cpp.sourceforge.net) - [Crypto++](https://
-www.cryptopp.com) - [ldap-cpp](https://github.com/AndreyBarmaley/ldap-cpp) -
-[OATH Toolkit](http://www.nongnu.org/oath-toolkit/liboath-api) [language.url]:
-https://isocpp.org/ [language.badge]: https://img.shields.io/badge/language-
-C++-blue.svg [standard.url]: https://en.wikipedia.org/wiki/
-C%2B%2B#Standardization [standard.badge]: https://img.shields.io/badge/C%2B%2B-
-11%2F14%2F17-blue.svg [release.url]: https://github.com/laoshanxi/app-mesh/
-releases [release.badge]: https://img.shields.io/github/v/release/laoshanxi/
-app-mesh.svg [docker.url]: https://hub.docker.com/repository/docker/laoshanxi/
-appmesh [docker.badge]: https://img.shields.io/docker/pulls/laoshanxi/
-appmesh.svg [cockpit.url]: https://github.com/laoshanxi/app-mesh-ui
-[cockpit.badge]: https://img.shields.io/badge/Cockpit-app--mesh--ui-
-blue?logo=appveyor [unittest.url]: https://github.com/catchorg/Catch2
-[unittest.badge]: https://img.shields.io/badge/UnitTest-Catch2-
-blue?logo=appveyor [pypi.badge]: https://img.shields.io/pypi/v/
+msgpack.org/) - [boostorg/boost](https://github.com/boostorg/boost) - [ACE_TAO/
+ACE](https://github.com/DOCGroup/ACE_TAO) - [curlpp](https://github.com/
+jpbarrette/curlpp) - [Thalhammer/jwt-cpp](https://github.com/Thalhammer/jwt-
+cpp) - [nlohmann/json](https://json.nlohmann.me) - [yaml-cpp](https://
+github.com/jbeder/yaml-cpp) - [nfpm](https://github.com/goreleaser/nfpm) -
+[jupp0r/prometheus-cpp](https://github.com/jupp0r/prometheus-cpp) - [zemasoft/
+wildcards](https://github.com/zemasoft/wildcards) - [mariusbancila/croncpp]
+(https://github.com/mariusbancila/croncpp) - [log4cpp](http://
+log4cpp.sourceforge.net) - [Crypto++](https://www.cryptopp.com) - [ldap-cpp]
+(https://github.com/AndreyBarmaley/ldap-cpp) - [OATH Toolkit](http://
+www.nongnu.org/oath-toolkit/liboath-api) [language.url]: https://isocpp.org/
+[language.badge]: https://img.shields.io/badge/language-C++-blue.svg
+[standard.url]: https://en.wikipedia.org/wiki/C%2B%2B#Standardization
+[standard.badge]: https://img.shields.io/badge/C%2B%2B-11%2F14%2F17-blue.svg
+[release.url]: https://github.com/laoshanxi/app-mesh/releases [release.badge]:
+https://img.shields.io/github/v/release/laoshanxi/app-mesh.svg [docker.url]:
+https://hub.docker.com/repository/docker/laoshanxi/appmesh [docker.badge]:
+https://img.shields.io/docker/pulls/laoshanxi/appmesh.svg [cockpit.url]: https:
+//github.com/laoshanxi/app-mesh-ui [cockpit.badge]: https://img.shields.io/
+badge/Cockpit-app--mesh--ui-blue?logo=appveyor [unittest.url]: https://
+github.com/catchorg/Catch2 [unittest.badge]: https://img.shields.io/badge/
+UnitTest-Catch2-blue?logo=appveyor [pypi.badge]: https://img.shields.io/pypi/v/
 appmesh?label=PyPI%3Aappmesh [pypi.url]: https://pypi.org/project/appmesh/
```

