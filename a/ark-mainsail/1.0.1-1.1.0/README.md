# Comparing `tmp/ark-mainsail-1.0.1.tar.gz` & `tmp/ark-mainsail-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ark-mainsail-1.0.1.tar", last modified: Mon Apr  8 20:57:11 2024, max compression
+gzip compressed data, was "ark-mainsail-1.1.0.tar", last modified: Sat Apr 20 18:00:45 2024, max compression
```

## Comparing `ark-mainsail-1.0.1.tar` & `ark-mainsail-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 20:57:11.449917 ark-mainsail-1.0.1/
--rw-rw-rw-   0        0        0     1063 2024-03-31 14:12:30.000000 ark-mainsail-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     3136 2024-04-08 20:57:11.447924 ark-mainsail-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-08 20:57:11.419639 ark-mainsail-1.0.1/ark_mainsail.egg-info/
--rw-rw-rw-   0        0        0     3136 2024-04-08 20:57:10.000000 ark-mainsail-1.0.1/ark_mainsail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      784 2024-04-08 20:57:10.000000 ark-mainsail-1.0.1/ark_mainsail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 20:57:10.000000 ark-mainsail-1.0.1/ark_mainsail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-08 20:57:10.000000 ark-mainsail-1.0.1/ark_mainsail.egg-info/requires.txt
--rw-rw-rw-   0        0        0       35 2024-04-08 20:57:10.000000 ark-mainsail-1.0.1/ark_mainsail.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 20:57:11.398697 ark-mainsail-1.0.1/mainsail/
--rw-rw-rw-   0        0        0     1848 2024-04-01 07:41:04.000000 ark-mainsail-1.0.1/mainsail/__init__.py
--rw-rw-rw-   0        0        0      961 2024-04-07 19:01:11.000000 ark-mainsail-1.0.1/mainsail/config.py
--rw-rw-rw-   0        0        0     1585 2024-03-31 14:12:31.000000 ark-mainsail-1.0.1/mainsail/deserializer.py
--rw-rw-rw-   0        0        0     9663 2024-04-07 05:49:52.000000 ark-mainsail-1.0.1/mainsail/identity.py
--rw-rw-rw-   0        0        0     4092 2024-04-07 13:54:09.000000 ark-mainsail-1.0.1/mainsail/rest.py
--rw-rw-rw-   0        0        0     1884 2024-03-31 14:12:31.000000 ark-mainsail-1.0.1/mainsail/serializer.py
--rw-rw-rw-   0        0        0     9253 2024-04-07 12:56:22.000000 ark-mainsail-1.0.1/mainsail/transaction.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:57:11.405677 ark-mainsail-1.0.1/mainsail/tx/
--rw-rw-rw-   0        0        0     1424 2024-04-07 15:25:42.000000 ark-mainsail-1.0.1/mainsail/tx/__init__.py
--rw-rw-rw-   0        0        0     7078 2024-04-07 12:42:08.000000 ark-mainsail-1.0.1/mainsail/tx/v1.py
--rw-rw-rw-   0        0        0     5057 2024-04-06 14:46:17.000000 ark-mainsail-1.0.1/mainsail/webhook.py
--rw-rw-rw-   0        0        0       42 2024-04-08 20:57:11.450915 ark-mainsail-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1569 2024-04-08 20:57:04.000000 ark-mainsail-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:57:11.416648 ark-mainsail-1.0.1/test/
--rw-rw-rw-   0        0        0       25 2024-04-01 18:54:30.000000 ark-mainsail-1.0.1/test/__init__.py
--rw-rw-rw-   0        0        0     1765 2024-04-06 14:10:01.000000 ark-mainsail-1.0.1/test/test_identity.py
--rw-rw-rw-   0        0        0     3331 2024-04-07 12:59:32.000000 ark-mainsail-1.0.1/test/test_v1_builders.py
+drwxrwxrwx   0        0        0        0 2024-04-20 18:00:45.478827 ark-mainsail-1.1.0/
+-rw-rw-rw-   0        0        0     1063 2024-03-31 14:12:30.000000 ark-mainsail-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4132 2024-04-20 18:00:45.475835 ark-mainsail-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-20 18:00:45.471845 ark-mainsail-1.1.0/ark_mainsail.egg-info/
+-rw-rw-rw-   0        0        0     4132 2024-04-20 18:00:45.000000 ark-mainsail-1.1.0/ark_mainsail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      936 2024-04-20 18:00:45.000000 ark-mainsail-1.1.0/ark_mainsail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 18:00:45.000000 ark-mainsail-1.1.0/ark_mainsail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-20 18:00:45.000000 ark-mainsail-1.1.0/ark_mainsail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       40 2024-04-20 18:00:45.000000 ark-mainsail-1.1.0/ark_mainsail.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 18:00:45.416992 ark-mainsail-1.1.0/mainsail/
+-rw-rw-rw-   0        0        0     1924 2024-04-13 21:52:02.000000 ark-mainsail-1.1.0/mainsail/__init__.py
+-rw-rw-rw-   0        0        0      961 2024-04-07 19:01:11.000000 ark-mainsail-1.1.0/mainsail/config.py
+-rw-rw-rw-   0        0        0     1585 2024-03-31 14:12:31.000000 ark-mainsail-1.1.0/mainsail/deserializer.py
+-rw-rw-rw-   0        0        0     9663 2024-04-07 05:49:52.000000 ark-mainsail-1.1.0/mainsail/identity.py
+-rw-rw-rw-   0        0        0     4742 2024-04-20 16:22:13.000000 ark-mainsail-1.1.0/mainsail/rest.py
+-rw-rw-rw-   0        0        0     1884 2024-03-31 14:12:31.000000 ark-mainsail-1.1.0/mainsail/serializer.py
+-rw-rw-rw-   0        0        0     9371 2024-04-13 16:38:37.000000 ark-mainsail-1.1.0/mainsail/transaction.py
+drwxrwxrwx   0        0        0        0 2024-04-20 18:00:45.424969 ark-mainsail-1.1.0/mainsail/tx/
+-rw-rw-rw-   0        0        0     1424 2024-04-07 15:25:42.000000 ark-mainsail-1.1.0/mainsail/tx/__init__.py
+-rw-rw-rw-   0        0        0     7080 2024-04-13 15:44:25.000000 ark-mainsail-1.1.0/mainsail/tx/v1.py
+-rw-rw-rw-   0        0        0     5013 2024-04-20 16:26:40.000000 ark-mainsail-1.1.0/mainsail/webhook.py
+drwxrwxrwx   0        0        0        0 2024-04-20 18:00:45.441924 ark-mainsail-1.1.0/pool/
+-rw-rw-rw-   0        0        0     5166 2024-04-20 12:54:07.000000 ark-mainsail-1.1.0/pool/__init__.py
+-rw-rw-rw-   0        0        0     5060 2024-04-20 11:32:24.000000 ark-mainsail-1.1.0/pool/__main__.py
+-rw-rw-rw-   0        0        0     1268 2024-04-20 12:49:05.000000 ark-mainsail-1.1.0/pool/api.py
+-rw-rw-rw-   0        0        0     6222 2024-04-20 16:45:21.000000 ark-mainsail-1.1.0/pool/biom.py
+-rw-rw-rw-   0        0        0     9370 2024-04-20 13:43:34.000000 ark-mainsail-1.1.0/pool/tbw.py
+-rw-rw-rw-   0        0        0       42 2024-04-20 18:00:45.479822 ark-mainsail-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1615 2024-04-20 18:00:42.000000 ark-mainsail-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 18:00:45.468852 ark-mainsail-1.1.0/test/
+-rw-rw-rw-   0        0        0       25 2024-04-01 18:54:30.000000 ark-mainsail-1.1.0/test/__init__.py
+-rw-rw-rw-   0        0        0     1765 2024-04-06 14:10:01.000000 ark-mainsail-1.1.0/test/test_identity.py
+-rw-rw-rw-   0        0        0     3635 2024-04-20 11:21:27.000000 ark-mainsail-1.1.0/test/test_v1_builders.py
```

### Comparing `ark-mainsail-1.0.1/LICENSE` & `ark-mainsail-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.0.1/PKG-INFO` & `ark-mainsail-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ark-mainsail
-Version: 1.0.1
+Version: 1.1.0
 Summary: Interact with ARK blockchain and forks
 Home-page: https://github.com/Moustikitos/python-mainsail
 Author: Toons
 Author-email: moustikitos@gmail.com
 Maintainer: Toons
 Maintainer-email: moustikitos@gmail.com
 License: Copyright 2024, MIT licence
@@ -51,27 +51,70 @@
 >>> t = Transfer(1, 'D5Ha4o3UTuTd59vjDw1F26mYhaRdXh7YPv', 'message \U0001f919')
 >>> t.sign()
 Type or paste your passphrase >
 >>> t.send()
 {'data': {'accept': [0], 'broadcast': [0], 'excess': [], 'invalid': []}}
 ```
 
+## Validator pool managment tool
+
+Installation:
+
+```bash
+~$ wget https://raw.githubusercontent.com/Moustikitos/python-mainsail/master/pool-install.sh
+~$ bash pool-install.sh
+~$ add_delegate 02968e862011738ac185e87f47dec61b32c842fd8e24fab625c02a15ad7e2d0f65
+Type or paste your passphrase>
+enter pin code to secure secret>
+provide a valid network peer> http://127.0.0.1:4003
+provide a valid webhook peer> http://127.0.0.1:4004
+provide a valid target endpoint> http://127.0.0.1:5000/block/forged
+```
+
+## [RIPEMD160 issue with OpenSSL v>=3](https://github.com/openssl/openssl/issues/16994) on ubuntu
+
+Get the installation folder:
+
+```bash
+openssl version -d
+```
+
+Make sure that the openssl config file contains following lines:
+
+```conf
+openssl_conf = openssl_init
+
+[openssl_init]
+providers = provider_sect
+
+[provider_sect]
+default = default_sect
+legacy = legacy_sect
+
+[default_sect]
+activate = 1
+
+[legacy_sect]
+activate = 1
+```
+
 ## Available transactions
 
 * [x] Transfer
 * [x] ValidatorRegistration
 * [x] Vote
 * [x] MultiSignature
 * [x] MultiPayment
 * [x] ValidatorResignation
 * [x] UsernameRegistration
 * [x] UsernameResignation
 
 ## Features
 
+* [x] pool managment tools
 * [x] secured private keys storage
 * [x] secured webhook subscriptions storage
 * [x] offline network configuration available
 
 ## Support this project
 
 <!-- [![Liberapay receiving](https://img.shields.io/liberapay/goal/Toons?logo=liberapay)](https://liberapay.com/Toons/donate) -->
```

### Comparing `ark-mainsail-1.0.1/ark_mainsail.egg-info/PKG-INFO` & `ark-mainsail-1.1.0/ark_mainsail.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ark-mainsail
-Version: 1.0.1
+Version: 1.1.0
 Summary: Interact with ARK blockchain and forks
 Home-page: https://github.com/Moustikitos/python-mainsail
 Author: Toons
 Author-email: moustikitos@gmail.com
 Maintainer: Toons
 Maintainer-email: moustikitos@gmail.com
 License: Copyright 2024, MIT licence
@@ -51,27 +51,70 @@
 >>> t = Transfer(1, 'D5Ha4o3UTuTd59vjDw1F26mYhaRdXh7YPv', 'message \U0001f919')
 >>> t.sign()
 Type or paste your passphrase >
 >>> t.send()
 {'data': {'accept': [0], 'broadcast': [0], 'excess': [], 'invalid': []}}
 ```
 
+## Validator pool managment tool
+
+Installation:
+
+```bash
+~$ wget https://raw.githubusercontent.com/Moustikitos/python-mainsail/master/pool-install.sh
+~$ bash pool-install.sh
+~$ add_delegate 02968e862011738ac185e87f47dec61b32c842fd8e24fab625c02a15ad7e2d0f65
+Type or paste your passphrase>
+enter pin code to secure secret>
+provide a valid network peer> http://127.0.0.1:4003
+provide a valid webhook peer> http://127.0.0.1:4004
+provide a valid target endpoint> http://127.0.0.1:5000/block/forged
+```
+
+## [RIPEMD160 issue with OpenSSL v>=3](https://github.com/openssl/openssl/issues/16994) on ubuntu
+
+Get the installation folder:
+
+```bash
+openssl version -d
+```
+
+Make sure that the openssl config file contains following lines:
+
+```conf
+openssl_conf = openssl_init
+
+[openssl_init]
+providers = provider_sect
+
+[provider_sect]
+default = default_sect
+legacy = legacy_sect
+
+[default_sect]
+activate = 1
+
+[legacy_sect]
+activate = 1
+```
+
 ## Available transactions
 
 * [x] Transfer
 * [x] ValidatorRegistration
 * [x] Vote
 * [x] MultiSignature
 * [x] MultiPayment
 * [x] ValidatorResignation
 * [x] UsernameRegistration
 * [x] UsernameResignation
 
 ## Features
 
+* [x] pool managment tools
 * [x] secured private keys storage
 * [x] secured webhook subscriptions storage
 * [x] offline network configuration available
 
 ## Support this project
 
 <!-- [![Liberapay receiving](https://img.shields.io/liberapay/goal/Toons?logo=liberapay)](https://liberapay.com/Toons/donate) -->
```

### Comparing `ark-mainsail-1.0.1/ark_mainsail.egg-info/SOURCES.txt` & `ark-mainsail-1.1.0/ark_mainsail.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 ./mainsail/identity.py
 ./mainsail/rest.py
 ./mainsail/serializer.py
 ./mainsail/transaction.py
 ./mainsail/webhook.py
 ./mainsail/tx/__init__.py
 ./mainsail/tx/v1.py
+./pool/__init__.py
+./pool/__main__.py
+./pool/api.py
+./pool/biom.py
+./pool/tbw.py
 ./test/__init__.py
 ./test/test_identity.py
 ./test/test_v1_builders.py
 ark_mainsail.egg-info/PKG-INFO
 ark_mainsail.egg-info/SOURCES.txt
 ark_mainsail.egg-info/dependency_links.txt
 ark_mainsail.egg-info/requires.txt
@@ -25,10 +30,15 @@
 mainsail/identity.py
 mainsail/rest.py
 mainsail/serializer.py
 mainsail/transaction.py
 mainsail/webhook.py
 mainsail/tx/__init__.py
 mainsail/tx/v1.py
+pool/__init__.py
+pool/__main__.py
+pool/api.py
+pool/biom.py
+pool/tbw.py
 test/__init__.py
 test/test_identity.py
 test/test_v1_builders.py
```

### Comparing `ark-mainsail-1.0.1/mainsail/__init__.py` & `ark-mainsail-1.1.0/mainsail/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import os
 import json
 import struct
 
 from typing import TextIO, Union
 from enum import IntEnum
 
+XTOSHI = 1e8
+
 
 class TYPES(IntEnum):
     TRANSFER = 0
     VALIDATOR_REGISTRATION = 2
     VOTE = 3
     MULTI_SIGNATURE = 4
     MULTI_PAYMENT = 6
@@ -42,22 +44,24 @@
         in_.close()
         del in_
     except Exception:
         pass
     return data
 
 
-def dumpJson(data: Union[dict, list], path: str) -> None:
+def dumpJson(data: Union[dict, list], path: str, **opt) -> None:
     "Dump JSON data to path"
+    if "indent" not in opt:
+        opt["indent"] = 4
     try:
         os.makedirs(os.path.dirname(path))
     except Exception:
         pass
     with io.open(path, "w", encoding="utf-8") as out:
-        json.dump(data, out, indent=4)
+        json.dump(data, out, **opt)
     try:
         out.close()
         del out
     except Exception:
         pass
```

### Comparing `ark-mainsail-1.0.1/mainsail/config.py` & `ark-mainsail-1.1.0/mainsail/config.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.0.1/mainsail/deserializer.py` & `ark-mainsail-1.1.0/mainsail/deserializer.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.0.1/mainsail/identity.py` & `ark-mainsail-1.1.0/mainsail/identity.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.0.1/mainsail/rest.py` & `ark-mainsail-1.1.0/mainsail/rest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 Network endpoint managment module.
 """
 
-import random
 import requests
 
 from typing import Union
 from mainsail import config
 from urllib.parse import urlencode
 
 
@@ -35,37 +34,57 @@
                     self.path, attr, headers=self.headers, func=self.func,
                     ports=self.ports
                 )
         else:
             return object.__getattribute__(self, attr)
 
     def __call__(self, *path, **data) -> Union[list, dict, requests.Response]:
-        peer, n = data.pop("peer", False), 10
-        # n tries to fetch a valid peer
+        peer, n = data.pop("peer", False), len(getattr(config, "peers", []))
+        ports = {}  # void set
+        # tries to fetch a valid peer
         while peer is False and n >= 0:
             # get a random peer from available network peers
-            peer = random.choice(config.peers)
+            peer = config.peers.pop(0)
+            config.peers.append(peer)
             # match attended ports and enabled ports
-            peer = \
-                False if not len(set(self.ports) & set(peer["ports"].keys())) \
-                else peer
+            ports = set(self.ports) & set(peer.get("ports", {}).keys())
+            peer = False if not len(ports) else peer
             n -= 1
-        # if n unsuccessful tries
+        # if unsuccessful
         if peer is False:
             raise ApiError(
                 f"no peer available with '{self.ports}' port enabled"
             )
         # else do HTTP request call
-        ports = list(set(self.ports) & set(peer["ports"].keys()))
-        resp = self.func(
-            f"http://{peer['ip']}:{peer['ports'][ports[0]]}/{self.path}/"
-            f"{'/'.join(path)}" + (f"?{urlencode(data)}" if len(data) else ""),
-            headers=self.headers,
-            json=data
-        )
+        if "url" in peer:
+            base_url = peer["url"]
+        else:
+            ports = list(
+                ports or set(self.ports) & set(peer.get("ports", {}).keys())
+            ) or ["requests"]
+            base_url = \
+                f"http://{peer.get('ip', '127.0.0.1')}:" \
+                f"{peer.get('ports', {}).get(ports[0], 5000)}"
+
+        path = '/'.join((self.path,) + path)
+        if base_url[-1] == "/":
+            base_url = base_url[:-1]
+        if path[0] != "/":
+            path = f"/{path}"
+
+        if self.func is requests.post:
+            resp = self.func(
+                f"{base_url}{path}", headers=self.headers, json=data
+            )
+        else:
+            resp = self.func(
+                f"{base_url}{path}"
+                f"{f'?{urlencode(data)}' if len(data) else ''}",
+                headers=self.headers,
+            )
         try:
             return resp.json()
         except requests.exceptions.JSONDecodeError:
             return resp
 
 
 def use_network(peer: str) -> None:
@@ -92,15 +111,15 @@
         config._dump(nethash)
 
 
 def load_network(name: str) -> bool:
     return config._load(name)
 
 
-def get_peers(peer: str, latency: int = 200) -> None:
+def get_peers(peer: str, latency: int = 500) -> None:
     resp = sorted(
         requests.get(
             f"{peer}/api/peers", headers={'Content-type': 'application/json'}
         ).json().get("data", {}),
         key=lambda p: p["latency"]
     )
     setattr(config, "peers", [
@@ -114,14 +133,14 @@
         for peer in resp if peer["latency"] <= latency
     ])
     if "peers" not in config._track:
         config._track.append("peers")
 
 
 # api root endpoints
-GET = EndPoint(ports=["api-development", "api-http", "core-api"])
+GET = EndPoint(ports=["api-http", "api-development", "core-api"])
 # transaction pool root endpoint
 POST = EndPoint(ports=["api-transaction-pool", "core-api"], func=requests.post)
 # webhook root endpoints
 WHK = EndPoint(ports=["api-webhook", "core-webhooks"])
 WHKP = EndPoint(ports=["api-webhook", "core-webhooks"], func=requests.post)
 WHKD = EndPoint(ports=["api-webhook", "core-webhooks"], func=requests.delete)
```

### Comparing `ark-mainsail-1.0.1/mainsail/serializer.py` & `ark-mainsail-1.1.0/mainsail/serializer.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.0.1/mainsail/transaction.py` & `ark-mainsail-1.1.0/mainsail/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import binascii
 
 from io import BytesIO
 from typing import Union, TextIO
 from mainsail import config, serializer, deserializer, identity, rest
-from mainsail import pack, pack_bytes, unpack, unpack_bytes
+from mainsail import pack, pack_bytes, unpack, unpack_bytes, XTOSHI
 
 # bit masks for serialization options
 SKIP_SIG1 = 0b100  # skip signature
 SKIP_SIG2 = 0b010  # skip second signature
 SKIP_MSIG = 0b001  # skip multiple signatures
 
 # list of attributes to be exported
@@ -25,15 +25,14 @@
     """
     Generic transaction class.
     """
     APB_MODE: int = 0  # TODO: continue APB_MODE dev
 
     amount: int = 0
     asset: dict = None
-    id: str = None
     blockId: str = None
     network: int = None
     recipientId: str = None
     secondSignature: str = None
     signature: str = None
     signatures: list = None
     signSignature: str = None
@@ -43,14 +42,19 @@
     vendorField: Union[str, bytes] = None
     version: int = 1
     lockTransactionId: str = None
     lockSecret: str = None
     expiration: int = 0
 
     @property
+    def id(self):
+        return \
+            identity.cSecp256k1.hash_sha256(self.serialize()).decode("utf-8")
+
+    @property
     def vendorFieldHex(self):
         return self.vendorField
 
     @vendorFieldHex.setter
     def vendorFieldHex(self, value: str):
         self.vendorField = binascii.unhexlify(value)
 
@@ -60,15 +64,15 @@
 
     @fee.setter
     def fee(self, value: Union[float, str]) -> None:
         # if value is float it is converted into arktoshi
         # if value is str it should starts with either 'min', 'avg' or 'max'
         # TODO: isinstance int -> arktoshi/bytes mode (APB_MODE)
         if isinstance(value, float):
-            self._fee = int(value * 100000000)
+            self._fee = int(value * XTOSHI)
         elif isinstance(value, str):
             value = value[:3]
             # to match tx name in cfg.fees, lowercase the first char of class
             # name: 'ClassName' -> 'className'
             name = self.__class__.__name__
             name = f"{name[0].lower()}{name[1:]}"
             if value in "minavgmax":
```

### Comparing `ark-mainsail-1.0.1/mainsail/tx/__init__.py` & `ark-mainsail-1.1.0/mainsail/tx/__init__.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.0.1/mainsail/tx/v1.py` & `ark-mainsail-1.1.0/mainsail/tx/v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import base58
 import getpass
 import binascii
 import cSecp256k1
 
 from typing import Union
 from mainsail.transaction import Transaction, SKIP_SIG1, SKIP_SIG2
-from mainsail import config, rest, identity, TYPE_GROUPS, TYPES
+from mainsail import config, rest, identity, TYPE_GROUPS, TYPES, XTOSHI
 
 __all__ = [
     "Transfer", "ValidatorRegistration", "ValidatorResignation",
     "UsernameRegistration", "UsernameResignation", "Vote", "MultiPayment",
     "MultiSignature"
 ]
 
@@ -35,15 +35,15 @@
         Transaction.__init__(self)
         self.version = \
             getattr(config, "consants", {}).get("block", {}).get("version", 1)
         self.typeGroup = TYPE_GROUPS.CORE.value
         self.type = TYPES.TRANSFER.value
         self.fee = "avg"
 
-        self.amount = int(amount * 100000000)
+        self.amount = int(amount * XTOSHI)
         self.recipientId = recipientId
         if vendorField is not None:
             self.vendorField = vendorField
 
 
 class ValidatorRegistration(Transaction):
 
@@ -159,15 +159,15 @@
         self.asset = {"payments": []}
         if vendorField is not None:
             self.vendorField = vendorField
         for address, amount in payments.items():
             self.addPayment(amount, address)
 
     def addPayment(self, amount: float, address: str):
-        amount = int(amount * 100000000)
+        amount = int(amount * XTOSHI)
         self.asset["payments"].append(
             {"recipientId": address, "amount": amount}
         )
         self.amount += amount
 
 
 class ValidatorResignation(Transaction):
```

### Comparing `ark-mainsail-1.0.1/mainsail/webhook.py` & `ark-mainsail-1.1.0/mainsail/webhook.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 # -*- coding: utf-8 -*-
 
 import io
 import os
 import re
 import pickle
+import logging
 import hashlib
 
 from mainsail import rest, dumpJson, loadJson
 
 DATA = os.path.join(os.getenv("HOME"), ".mainsail", ".webhooks")
 REGEXP = re.compile(r'^([\w\.]*)\s*([^\w\s\^]*)\s*(.*)\s*$')
 OPERATORS = {
     "<": "lt", "<=": "lte",
     ">": "gt", ">=": "gte",
     "==": "eq", "!=": "ne",
     "?": "truthy", "!?": "falsy",
     "\\": "regexp", "$": "contains",
     "<>": "between", "!<>": "not-between"
 }
+# set basic logging
+logging.basicConfig()
+LOGGER = logging.getLogger(__name__)
+LOGGER.setLevel(logging.INFO)
 
 
 def condition(expr: str) -> dict:
     """
     Webhook condition builder from `str` expression.
 
     <style>td,th{border:none!important;text-align:left;}</style>
@@ -50,15 +55,15 @@
         dict: webhook conditions
     """
     condition = {}
     try:
         key, _operator, value = REGEXP.match(expr).groups()
         operator = OPERATORS[_operator]
     except Exception as error:
-        print(">>> %r" % error)
+        LOGGER.info("%r", error)
     else:
         if "between" in operator:
             _min, _max = value.split(":")
             condition["value"] = {"min": _min, "max": _max}
         elif value != "":
             condition["value"] = value
         condition["key"] = key
@@ -67,16 +72,15 @@
 
 
 def dump(token: str) -> str:
     # "0c8e74e1cbfe36404386d33a5bbd8b66fe944e318edb02b979d6bf0c87978b64"
     authorization = token[:32]  # "0c8e74e1cbfe36404386d33a5bbd8b66"
     verification = token[32:]   # "fe944e318edb02b979d6bf0c87978b64"
     filename = os.path.join(
-        DATA, rest.config.nethash,
-        hashlib.md5(authorization.encode("utf-8")).hexdigest()
+        DATA, hashlib.md5(authorization.encode("utf-8")).hexdigest()
     )
     os.makedirs(os.path.dirname(filename), exist_ok=True)
     with io.open(filename, "wb") as out:
         pickle.dump(
             {
                 "verification": verification,
                 "hash": hashlib.sha256(token.encode("utf-8")).hexdigest()
@@ -96,56 +100,50 @@
         for cond in conditions
     ]
     data = rest.WHKP.api.webhooks(
         peer=peer, event=event, target=target,
         conditions=[cond for cond in conditions if cond],
     ).get("data", {})
     if "token" in data:
-        print("security token :", data["token"])
         # build the security hash and keep only second token part and
         # save the used peer to be able to delete it later
+        data["nethash"] = getattr(rest.config, "nethash")
         data["dump"] = dump(data.pop("token"))
         data["peer"] = peer
-        dumpJson(
-            data, os.path.join(DATA, rest.config.nethash, data["id"] + ".json")
-        )
+        dumpJson(data, os.path.join(DATA, data["id"] + ".json"))
+        return data["id"]
     else:
         raise Exception("webhook not created")
 
 
 def verify(authorization: str) -> bool:
-    filename = os.path.join(
-        DATA, rest.config.nethash,
-        hashlib.md5(authorization.encode("utf-8")).hexdigest()
-    )
     try:
+        filename = os.path.join(
+            DATA, hashlib.md5(authorization.encode("utf-8")).hexdigest()
+        )
         with io.open(filename, "rb") as in_:
             data = pickle.load(in_)
     except Exception:
         return False
     else:
         token = authorization + data["verification"]
         return \
             hashlib.sha256(token.encode("utf-8")).hexdigest() == data["hash"]
 
 
 def list() -> list:
-    return [
-        name for name in next(
-            os.walk(os.path.join(DATA, rest.config.nethash))
-        )[-1] if name.endswith(".json")
-    ]
+    return [name for name in next(os.walk(DATA))[-1] if name.endswith(".json")]
 
 
 def open(whk_id: str) -> dict:
-    return loadJson(os.path.join(DATA, rest.config.nethash, whk_id + ".json"))
+    return loadJson(os.path.join(DATA, whk_id + ".json"))
 
 
 def unsubscribe(whk_id: str) -> dict:
-    whk_path = os.path.join(DATA, rest.config.nethash, whk_id + ".json")
+    whk_path = os.path.join(DATA, whk_id + ".json")
     if os.path.exists(whk_path):
         data = loadJson(whk_path)
         resp = rest.WHKD.api.webhooks(
             "%s" % whk_id, peer=data.get("peer", None)
         )
         if resp.status_code == 204:
             try:
```

### Comparing `ark-mainsail-1.0.1/setup.py` & `ark-mainsail-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # -*- coding:utf-8 -*-
 
-from setuptools import setup
+from setuptools import setup, find_packages
 
 
 with open("README.md") as f2:
     LONG_DESCRIPTION = f2.read()
 
 kw = {
-    "version": "1.0.1",
+    "version": "1.1.0",
     "name": "ark-mainsail",
     "keywords": ["api", "ark", "blockchain"],
     "author": "Toons",
     "author_email": "moustikitos@gmail.com",
     "maintainer": "Toons",
     "maintainer_email": "moustikitos@gmail.com",
     "url": "https://github.com/Moustikitos/python-mainsail",
     "project_urls": {  # Optional
         "Bug Reports": "https://github.com/Moustikitos/python-mainsail/issues",
-        "Funding": "https://github.com/Moustikitos/python-mainsail?tab=readme-ov-file#support-this-project",
+        "Funding":
+            "https://github.com/Moustikitos/python-mainsail?tab=readme-ov-file"
+            "#support-this-project",
         "Source": "https://github.com/Moustikitos/python-mainsail/",
     },
-    "include_package_data": True,
+    "include_package_data": False,
     "description": "Interact with ARK blockchain and forks",
     "long_description": LONG_DESCRIPTION,
     "long_description_content_type": "text/markdown",
     "install_requires": ["requests", "base58", "pyaes", "blspy", "cSecp256k1"],
     "license": "Copyright 2024, MIT licence",
     "classifiers": [
         "Development Status :: 5 - Production/Stable",
@@ -33,11 +35,11 @@
         "Intended Audience :: Developers",
         "Intended Audience :: End Users/Desktop",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
-    "package_dir": {"": "."}
+    "package_dir": {"": "."},
 }
 
 setup(**kw)
```

### Comparing `ark-mainsail-1.0.1/test/test_identity.py` & `ark-mainsail-1.1.0/test/test_identity.py`

 * *Files identical despite different names*

