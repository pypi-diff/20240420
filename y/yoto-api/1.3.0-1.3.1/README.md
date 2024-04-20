# Comparing `tmp/yoto_api-1.3.0.tar.gz` & `tmp/yoto_api-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoto_api-1.3.0.tar", last modified: Sat Apr 20 01:09:26 2024, max compression
+gzip compressed data, was "yoto_api-1.3.1.tar", last modified: Sat Apr 20 02:01:36 2024, max compression
```

## Comparing `yoto_api-1.3.0.tar` & `yoto_api-1.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:09:26.520253 yoto_api-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-20 01:09:04.000000 yoto_api-1.3.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-20 01:09:04.000000 yoto_api-1.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 01:09:04.000000 yoto_api-1.3.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-20 01:09:04.000000 yoto_api-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-20 01:09:04.000000 yoto_api-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-20 01:09:26.520253 yoto_api-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-20 01:09:04.000000 yoto_api-1.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-20 01:09:04.000000 yoto_api-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 01:09:26.524253 yoto_api-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-20 01:09:20.000000 yoto_api-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:09:26.520253 yoto_api-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:09:04.000000 yoto_api-1.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-20 01:09:04.000000 yoto_api-1.3.0/tests/login_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:09:26.520253 yoto_api-1.3.0/yoto_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-20 01:09:04.000000 yoto_api-1.3.0/yoto_api/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-20 01:09:04.000000 yoto_api-1.3.0/yoto_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)    20950 2024-04-20 01:09:04.000000 yoto_api-1.3.0/yoto_api/YotoAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-20 01:09:04.000000 yoto_api-1.3.0/yoto_api/YotoManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-20 01:09:04.000000 yoto_api-1.3.0/yoto_api/YotoPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-20 01:09:04.000000 yoto_api-1.3.0/yoto_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 01:09:04.000000 yoto_api-1.3.0/yoto_api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:09:26.520253 yoto_api-1.3.0/yoto_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-20 01:09:26.000000 yoto_api-1.3.0/yoto_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-20 01:09:26.000000 yoto_api-1.3.0/yoto_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:09:26.000000 yoto_api-1.3.0/yoto_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:09:26.000000 yoto_api-1.3.0/yoto_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-20 01:09:26.000000 yoto_api-1.3.0/yoto_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 01:09:26.000000 yoto_api-1.3.0/yoto_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:01:36.466202 yoto_api-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-20 02:01:09.000000 yoto_api-1.3.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-20 02:01:09.000000 yoto_api-1.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 02:01:09.000000 yoto_api-1.3.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-20 02:01:09.000000 yoto_api-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-20 02:01:09.000000 yoto_api-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-20 02:01:36.466202 yoto_api-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-20 02:01:09.000000 yoto_api-1.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-20 02:01:09.000000 yoto_api-1.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 02:01:36.466202 yoto_api-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-20 02:01:28.000000 yoto_api-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:01:36.462202 yoto_api-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 02:01:09.000000 yoto_api-1.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-20 02:01:09.000000 yoto_api-1.3.1/tests/login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:01:36.462202 yoto_api-1.3.1/yoto_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-20 02:01:09.000000 yoto_api-1.3.1/yoto_api/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-20 02:01:09.000000 yoto_api-1.3.1/yoto_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21095 2024-04-20 02:01:09.000000 yoto_api-1.3.1/yoto_api/YotoAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-20 02:01:09.000000 yoto_api-1.3.1/yoto_api/YotoManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-20 02:01:09.000000 yoto_api-1.3.1/yoto_api/YotoPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-20 02:01:09.000000 yoto_api-1.3.1/yoto_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 02:01:09.000000 yoto_api-1.3.1/yoto_api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:01:36.466202 yoto_api-1.3.1/yoto_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-20 02:01:36.000000 yoto_api-1.3.1/yoto_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-20 02:01:36.000000 yoto_api-1.3.1/yoto_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 02:01:36.000000 yoto_api-1.3.1/yoto_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 02:01:36.000000 yoto_api-1.3.1/yoto_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-20 02:01:36.000000 yoto_api-1.3.1/yoto_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 02:01:36.000000 yoto_api-1.3.1/yoto_api.egg-info/top_level.txt
```

### Comparing `yoto_api-1.3.0/CONTRIBUTING.rst` & `yoto_api-1.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.3.0/LICENSE` & `yoto_api-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yoto_api-1.3.0/PKG-INFO` & `yoto_api-1.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `yoto_api-1.3.0/README.rst` & `yoto_api-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.3.0/setup.py` & `yoto_api-1.3.1/setup.py`

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
-    version="1.3.0",
+    version="1.3.1",
     zip_safe=False,
 )
```

### Comparing `yoto_api-1.3.0/yoto_api/Card.py` & `yoto_api-1.3.1/yoto_api/Card.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.3.0/yoto_api/YotoAPI.py` & `yoto_api-1.3.1/yoto_api/YotoAPI.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,59 +64,56 @@
         # Requests to endpoints below use contents of "access_token" in the header ->
         # Authorization: Bearer access_token
         # User-Agent: Yoto/2.73 (com.yotoplay.Yoto; build:10405; iOS 17.4.0) Alamofire/5.6.4
 
     # pass='audience=https%3A//api.yotoplay.com&client_id=FILL_THIS_IN&grant_type=password&password=FILL_THIS_IN&scope=openid%20email%20profile%20offline_access&username=FILL_THIS_IN%40gmail.com'
     # curl -d "$pass" https://api.yotoplay.com/auth/token | jq '.access_token'
 
-    def get_devices(self, token: Token) -> dict[YotoPlayer]:
+    def update_players(self, token: Token, players: list[YotoPlayer]) -> None:
         response = self._get_devices(token)
-        result = {}
-        for device in response["devices"]:
-            player: YotoPlayer = YotoPlayer(
-                id=device["deviceId"],
-                name=device["name"],
-                deviceType=device["deviceType"],
-                online=device["online"],
-                last_updated_at=datetime.datetime.now(pytz.utc),
-            )
-            result[player.id] = player
-
-        return result
+        for item in response["devices"]:
+            if self.get_child_value(item, "deviceId") not in players:
+                player: YotoPlayer = YotoPlayer(
+                    id=self.get_child_value(item, "deviceId"),
+                )
+                players[player.id] = player
+            deviceId = self.get_child_value(item, "deviceId")
+            players[deviceId].name = self.get_child_value(item, "name")
+            players[deviceId].deviceType = self.get_child_value(item, "deviceType")
+            players[deviceId].online = self.get_child_value(item, "online")
+            players[deviceId].last_updated_at = datetime.datetime.now(pytz.utc)
 
-    def update_devices(self, token: Token, players: list[YotoPlayer]) -> None:
-        response = self._get_devices(token)
-        for player in players.values():
-            print(player)
-            player.last_updated_at = datetime.datetime.now(pytz.utc)
-            for device in response["devices"]:
-                if device["deviceId"] == player.id:
-                    player.online = device["online"]
-
-    def get_library(self, token: Token) -> list[Card]:
+    def update_library(self, token: Token, library: dict[Card]) -> list[Card]:
         response = self._get_cards(token)
-        cards = {}
         for item in response["cards"]:
-            card: Card = Card(
-                id=self.get_child_value(item, "cardId"),
-                title=self.get_child_value(item, "card.title"),
-                description=self.get_child_value(item, "card.metadata.description"),
-                author=self.get_child_value(item, "card.metadata.author"),
-                category=self.get_child_value(item, "card.metadata.stories"),
-                coverImageL=self.get_child_value(item, "card.metadata.cover.imageL"),
-                seriesOrder=self.get_child_value(
-                    item, "card.metadata.cover.seriesorder"
-                ),
-                seriesTitle=self.get_child_value(
-                    item, "card.metadata.cover.seriestitle"
-                ),
-            )
-            cards[card.id] = card
-        return cards
-        # TODO: parse the data and return a list of cards.
+            if self.get_child_value(item, "cardId") not in library:
+                card: Card = Card(
+                    id=self.get_child_value(item, "cardId"),
+                )
+                library[card.id] = card
+            cardId = self.get_child_value(item, "cardId")
+            library[cardId].title = self.get_child_value(item, "card.title")
+            library[cardId].description = self.get_child_value(
+                item, "card.metadata.description"
+            )
+            library[self.get_child_value(item, "cardId")].author = self.get_child_value(
+                item, "card.metadata.author"
+            )
+            library[cardId].category = self.get_child_value(
+                item, "card.metadata.stories"
+            )
+            library[cardId].coverImageL = self.get_child_value(
+                item, "card.metadata.cover.imageL"
+            )
+            library[cardId].seriesOrder = self.get_child_value(
+                item, "card.metadata.cover.seriesorder"
+            )
+            library[cardId].seriesTitle = self.get_child_value(
+                item, "card.metadata.cover.seriestitle"
+            )
 
     def refresh_token(self, token: Token) -> Token:
         # audience=https%3A//api.yotoplay.com&client_id=FILL_THIS_IN&grant_type=refresh_token&refresh_token=FILL_THIS_IN&scope=openid%20email%20profile%20offline_access
         url = self.TOKEN_URL
         payload = {}
         payload["audience"] = self.BASE_URL
         payload["client_id"] = self.CLIENT_ID
```

### Comparing `yoto_api-1.3.0/yoto_api/YotoManager.py` & `yoto_api-1.3.1/yoto_api/YotoManager.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,30 +14,29 @@
 class YotoManager:
     def __init__(self, username: str, password: str) -> None:
         self.username: str = username
         self.password: str = password
         self.api: YotoAPI = YotoAPI()
         self.players: dict = {}
         self.token: Token = None
-        self.players: list = None
-        self.library: list = None
+        self.library: list = {}
 
     def initialize(self) -> None:
         self.token: Token = self.api.login(self.username, self.password)
-        self.players = self.api.get_devices(self.token)
-        self.library = self.api.get_library(self.token)
+        self.update_players_status()
+        self.update_cards()
 
-    def update_player_status(self) -> None:
+    def update_players_status(self) -> None:
         # Updates the data with current player data.
-        self.api.update_devices(self.token, self.players)
+        self.api.update_players(self.token, self.players)
 
     def update_cards(self) -> None:
         # Updates library and all card data.  Typically only required on startup.
         # TODO: Should update the self.library object with a current dict of players. Should it do details for all cards too or separate?
-        self.library = self.api.update_library(self.token)
+        self.api.update_library(self.token, self.library)
 
     def check_and_refresh_token(self) -> bool:
         if self.token is None:
             self.initialize()
             return True
         # Check if valid and correct if not
         if self.token.valid_until <= datetime.datetime.now(pytz.utc):
```

### Comparing `yoto_api-1.3.0/yoto_api.egg-info/PKG-INFO` & `yoto_api-1.3.1/yoto_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

