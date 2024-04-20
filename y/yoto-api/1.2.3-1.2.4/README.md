# Comparing `tmp/yoto_api-1.2.3.tar.gz` & `tmp/yoto_api-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoto_api-1.2.3.tar", last modified: Fri Apr 19 19:12:07 2024, max compression
+gzip compressed data, was "yoto_api-1.2.4.tar", last modified: Fri Apr 19 20:53:32 2024, max compression
```

## Comparing `yoto_api-1.2.3.tar` & `yoto_api-1.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:12:07.463125 yoto_api-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-19 19:11:43.000000 yoto_api-1.2.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-19 19:11:43.000000 yoto_api-1.2.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 19:11:43.000000 yoto_api-1.2.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 19:11:43.000000 yoto_api-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 19:11:43.000000 yoto_api-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-19 19:12:07.463125 yoto_api-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-19 19:11:43.000000 yoto_api-1.2.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 19:11:43.000000 yoto_api-1.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:12:07.463125 yoto_api-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-19 19:12:01.000000 yoto_api-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:12:07.459125 yoto_api-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:11:43.000000 yoto_api-1.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-19 19:11:43.000000 yoto_api-1.2.3/tests/login_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:12:07.459125 yoto_api-1.2.3/yoto_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-19 19:11:43.000000 yoto_api-1.2.3/yoto_api/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-19 19:11:43.000000 yoto_api-1.2.3/yoto_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)    19768 2024-04-19 19:11:43.000000 yoto_api-1.2.3/yoto_api/YotoAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-19 19:11:43.000000 yoto_api-1.2.3/yoto_api/YotoManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-19 19:11:43.000000 yoto_api-1.2.3/yoto_api/YotoPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-19 19:11:43.000000 yoto_api-1.2.3/yoto_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 19:11:43.000000 yoto_api-1.2.3/yoto_api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:12:07.463125 yoto_api-1.2.3/yoto_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-19 19:12:07.000000 yoto_api-1.2.3/yoto_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-19 19:12:07.000000 yoto_api-1.2.3/yoto_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:12:07.000000 yoto_api-1.2.3/yoto_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:12:07.000000 yoto_api-1.2.3/yoto_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 19:12:07.000000 yoto_api-1.2.3/yoto_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 19:12:07.000000 yoto_api-1.2.3/yoto_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:53:32.520410 yoto_api-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-19 20:53:08.000000 yoto_api-1.2.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-19 20:53:08.000000 yoto_api-1.2.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 20:53:08.000000 yoto_api-1.2.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 20:53:08.000000 yoto_api-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 20:53:08.000000 yoto_api-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-19 20:53:32.520410 yoto_api-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-19 20:53:08.000000 yoto_api-1.2.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 20:53:08.000000 yoto_api-1.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 20:53:32.520410 yoto_api-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-19 20:53:26.000000 yoto_api-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:53:32.516410 yoto_api-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 20:53:08.000000 yoto_api-1.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-19 20:53:08.000000 yoto_api-1.2.4/tests/login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:53:32.516410 yoto_api-1.2.4/yoto_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-19 20:53:08.000000 yoto_api-1.2.4/yoto_api/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-19 20:53:08.000000 yoto_api-1.2.4/yoto_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20012 2024-04-19 20:53:08.000000 yoto_api-1.2.4/yoto_api/YotoAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-19 20:53:08.000000 yoto_api-1.2.4/yoto_api/YotoManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-19 20:53:08.000000 yoto_api-1.2.4/yoto_api/YotoPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-19 20:53:08.000000 yoto_api-1.2.4/yoto_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 20:53:08.000000 yoto_api-1.2.4/yoto_api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:53:32.520410 yoto_api-1.2.4/yoto_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-19 20:53:32.000000 yoto_api-1.2.4/yoto_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-19 20:53:32.000000 yoto_api-1.2.4/yoto_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 20:53:32.000000 yoto_api-1.2.4/yoto_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 20:53:32.000000 yoto_api-1.2.4/yoto_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 20:53:32.000000 yoto_api-1.2.4/yoto_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 20:53:32.000000 yoto_api-1.2.4/yoto_api.egg-info/top_level.txt
```

### Comparing `yoto_api-1.2.3/CONTRIBUTING.rst` & `yoto_api-1.2.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.2.3/LICENSE` & `yoto_api-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yoto_api-1.2.3/PKG-INFO` & `yoto_api-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `yoto_api-1.2.3/README.rst` & `yoto_api-1.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.2.3/setup.py` & `yoto_api-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="yoto_api",
     name="yoto_api",
     packages=find_packages(include=["yoto_api", "yoto_api.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/cdnninja/yoto_api",
-    version="1.2.3",
+    version="1.2.4",
     zip_safe=False,
 )
```

### Comparing `yoto_api-1.2.3/yoto_api/Card.py` & `yoto_api-1.2.4/yoto_api/Card.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.2.3/yoto_api/YotoAPI.py` & `yoto_api-1.2.4/yoto_api/YotoAPI.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,28 +46,37 @@
             scope=response["scope"],
             valid_until=valid_until,
         )
 
     # pass='audience=https%3A//api.yotoplay.com&client_id=FILL_THIS_IN&grant_type=password&password=FILL_THIS_IN&scope=openid%20email%20profile%20offline_access&username=FILL_THIS_IN%40gmail.com'
     # curl -d "$pass" https://api.yotoplay.com/auth/token | jq '.access_token'
 
-    def update_devices(self, token, devices) -> dict[YotoPlayer]:
-        response = self._get_devices(token)      
-        if devices is None:
-            devices = {}
-        else: 
-            for player in response["devices"]:
-                devices[player.id].id = player["deviceId"]
-                devices[player.id].name = player["name"]
-                devices[player.id].deviceType = player["deviceType"]
-                devices[player.id].last_update_at = datetime.datetime.now(pytz.utc)
-                devices[player.id].online = player["online"],
+    def get_devices(self, token) -> dict[YotoPlayer]:
+        response = self._get_devices(token)
+        result = {}
+        for device in response["devices"]:
+            player: YotoPlayer = YotoPlayer(
+                id=device["deviceId"],
+                name=device["name"],
+                deviceType=device["deviceType"],
+                online=device["online"],
+                last_updated_at=datetime.datetime.now(pytz.utc)
+            )
+            result[player.id] = player
 
+        return result
+    
+    def update_devices(self, token, players) -> None:
+        response = self._get_devices(token)
+        for device in response["devices"]:
+            players[device["deviceId"]].online=device["online"]
+            players[device["deviceId"]].last_update_at=datetime.datetime.now(pytz.utc)
 
-    def update_library(self, token) -> list[Card]:
+
+    def get_library(self, token) -> list[Card]:
         cards = self._get_cards(token)
         return cards
         # TODO: parse the data and return a list of cards.
 
     def refresh_token(self, token: Token) -> Token:
         # audience=https%3A//api.yotoplay.com&client_id=FILL_THIS_IN&grant_type=refresh_token&refresh_token=FILL_THIS_IN&scope=openid%20email%20profile%20offline_access
         url = self.TOKEN_URL
```

### Comparing `yoto_api-1.2.3/yoto_api/YotoManager.py` & `yoto_api-1.2.4/yoto_api/YotoManager.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,16 +18,16 @@
         self.players: dict = {}
         self.token: Token = None
         self.players: list = None
         self.library: list = None
 
     def initialize(self) -> None:
         self.token: Token = self.api.login(self.username, self.password)
-        self.update_player_status()
-        self.update_cards()
+        self.players = self.api.get_devices(self.token)
+        # self.library = 
 
     def update_player_status(self) -> None:
         # Updates the data with current player data.
         self.players = self.api.update_devices(self.token, self.players)
 
     def update_cards(self) -> None:
         # Updates library and all card data.  Typically only required on startup.
```

### Comparing `yoto_api-1.2.3/yoto_api.egg-info/PKG-INFO` & `yoto_api-1.2.4/yoto_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

