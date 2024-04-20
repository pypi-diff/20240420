# Comparing `tmp/yoto_api-1.2.4.tar.gz` & `tmp/yoto_api-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoto_api-1.2.4.tar", last modified: Fri Apr 19 20:53:32 2024, max compression
+gzip compressed data, was "yoto_api-1.2.5.tar", last modified: Sat Apr 20 00:17:19 2024, max compression
```

## Comparing `yoto_api-1.2.4.tar` & `yoto_api-1.2.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:53:32.520410 yoto_api-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-19 20:53:08.000000 yoto_api-1.2.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-19 20:53:08.000000 yoto_api-1.2.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 20:53:08.000000 yoto_api-1.2.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 20:53:08.000000 yoto_api-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 20:53:08.000000 yoto_api-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-19 20:53:32.520410 yoto_api-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-19 20:53:08.000000 yoto_api-1.2.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 20:53:08.000000 yoto_api-1.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 20:53:32.520410 yoto_api-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-19 20:53:26.000000 yoto_api-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:53:32.516410 yoto_api-1.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 20:53:08.000000 yoto_api-1.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-19 20:53:08.000000 yoto_api-1.2.4/tests/login_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:53:32.516410 yoto_api-1.2.4/yoto_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-19 20:53:08.000000 yoto_api-1.2.4/yoto_api/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-19 20:53:08.000000 yoto_api-1.2.4/yoto_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)    20012 2024-04-19 20:53:08.000000 yoto_api-1.2.4/yoto_api/YotoAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-19 20:53:08.000000 yoto_api-1.2.4/yoto_api/YotoManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-19 20:53:08.000000 yoto_api-1.2.4/yoto_api/YotoPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-19 20:53:08.000000 yoto_api-1.2.4/yoto_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 20:53:08.000000 yoto_api-1.2.4/yoto_api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:53:32.520410 yoto_api-1.2.4/yoto_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-19 20:53:32.000000 yoto_api-1.2.4/yoto_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-19 20:53:32.000000 yoto_api-1.2.4/yoto_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 20:53:32.000000 yoto_api-1.2.4/yoto_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 20:53:32.000000 yoto_api-1.2.4/yoto_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 20:53:32.000000 yoto_api-1.2.4/yoto_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 20:53:32.000000 yoto_api-1.2.4/yoto_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:17:19.046597 yoto_api-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-20 00:16:54.000000 yoto_api-1.2.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-20 00:16:54.000000 yoto_api-1.2.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 00:16:54.000000 yoto_api-1.2.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-20 00:16:54.000000 yoto_api-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-20 00:16:54.000000 yoto_api-1.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-20 00:17:19.046597 yoto_api-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-20 00:16:54.000000 yoto_api-1.2.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-20 00:16:54.000000 yoto_api-1.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 00:17:19.046597 yoto_api-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-20 00:17:12.000000 yoto_api-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:17:19.046597 yoto_api-1.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:16:54.000000 yoto_api-1.2.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-20 00:16:54.000000 yoto_api-1.2.5/tests/login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:17:19.046597 yoto_api-1.2.5/yoto_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-20 00:16:54.000000 yoto_api-1.2.5/yoto_api/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-20 00:16:54.000000 yoto_api-1.2.5/yoto_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20118 2024-04-20 00:16:54.000000 yoto_api-1.2.5/yoto_api/YotoAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-20 00:16:54.000000 yoto_api-1.2.5/yoto_api/YotoManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-20 00:16:54.000000 yoto_api-1.2.5/yoto_api/YotoPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-20 00:16:54.000000 yoto_api-1.2.5/yoto_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 00:16:54.000000 yoto_api-1.2.5/yoto_api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:17:19.046597 yoto_api-1.2.5/yoto_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-20 00:17:19.000000 yoto_api-1.2.5/yoto_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-20 00:17:19.000000 yoto_api-1.2.5/yoto_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 00:17:19.000000 yoto_api-1.2.5/yoto_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 00:17:18.000000 yoto_api-1.2.5/yoto_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-20 00:17:19.000000 yoto_api-1.2.5/yoto_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 00:17:19.000000 yoto_api-1.2.5/yoto_api.egg-info/top_level.txt
```

### Comparing `yoto_api-1.2.4/CONTRIBUTING.rst` & `yoto_api-1.2.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.2.4/LICENSE` & `yoto_api-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yoto_api-1.2.4/PKG-INFO` & `yoto_api-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.2.4
+Version: 1.2.5
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `yoto_api-1.2.4/README.rst` & `yoto_api-1.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.2.4/setup.py` & `yoto_api-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="yoto_api",
     name="yoto_api",
     packages=find_packages(include=["yoto_api", "yoto_api.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/cdnninja/yoto_api",
-    version="1.2.4",
+    version="1.2.5",
     zip_safe=False,
 )
```

### Comparing `yoto_api-1.2.4/yoto_api/Card.py` & `yoto_api-1.2.5/yoto_api/Card.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.2.4/yoto_api/YotoAPI.py` & `yoto_api-1.2.5/yoto_api/YotoAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,20 +61,22 @@
                 online=device["online"],
                 last_updated_at=datetime.datetime.now(pytz.utc)
             )
             result[player.id] = player
 
         return result
     
-    def update_devices(self, token, players) -> None:
+    def update_devices(self, token, players: list[YotoPlayer]) -> None:
         response = self._get_devices(token)
-        for device in response["devices"]:
-            players[device["deviceId"]].online=device["online"]
-            players[device["deviceId"]].last_update_at=datetime.datetime.now(pytz.utc)
-
+        for player in players.values():
+            print(player)
+            player.last_updated_at=datetime.datetime.now(pytz.utc)
+            for device in response["devices"]:
+                if device["deviceId"] == player.id:
+                    player.online=device["online"]
 
     def get_library(self, token) -> list[Card]:
         cards = self._get_cards(token)
         return cards
         # TODO: parse the data and return a list of cards.
 
     def refresh_token(self, token: Token) -> Token:
```

### Comparing `yoto_api-1.2.4/yoto_api/YotoManager.py` & `yoto_api-1.2.5/yoto_api/YotoManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def initialize(self) -> None:
         self.token: Token = self.api.login(self.username, self.password)
         self.players = self.api.get_devices(self.token)
         # self.library = 
 
     def update_player_status(self) -> None:
         # Updates the data with current player data.
-        self.players = self.api.update_devices(self.token, self.players)
+        self.api.update_devices(self.token, self.players)
 
     def update_cards(self) -> None:
         # Updates library and all card data.  Typically only required on startup.
         # TODO: Should update the self.library object with a current dict of players. Should it do details for all cards too or separate?
         self.library = self.api.update_library(self.token)
 
     def check_and_refresh_token(self) -> bool:
```

### Comparing `yoto_api-1.2.4/yoto_api.egg-info/PKG-INFO` & `yoto_api-1.2.5/yoto_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.2.4
+Version: 1.2.5
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

