# Comparing `tmp/pyblu-0.1.0.tar.gz` & `tmp/pyblu-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyblu-0.1.0.tar", max compression
+gzip compressed data, was "pyblu-0.2.0.tar", max compression
```

## Comparing `pyblu-0.1.0.tar` & `pyblu-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1069 2024-03-09 09:45:55.409568 pyblu-0.1.0/LICENSE
--rw-r--r--   0        0        0      880 2024-04-12 15:42:11.404846 pyblu-0.1.0/README.md
--rw-r--r--   0        0        0      921 2024-04-12 15:42:38.186030 pyblu-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      147 2024-04-11 18:02:26.467648 pyblu-0.1.0/src/pyblu/__init__.py
--rw-r--r--   0        0        0     2554 2024-04-11 18:02:26.436648 pyblu-0.1.0/src/pyblu/_entities.py
--rw-r--r--   0        0        0    12244 2024-04-12 15:43:12.252253 pyblu-0.1.0/src/pyblu/_player.py
--rw-r--r--   0        0        0     1473 1970-01-01 00:00:00.000000 pyblu-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-09 09:45:55.409568 pyblu-0.2.0/LICENSE
+-rw-r--r--   0        0        0      873 2024-04-12 16:28:03.088001 pyblu-0.2.0/README.md
+-rw-r--r--   0        0        0      921 2024-04-20 09:48:42.226893 pyblu-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      277 2024-04-14 21:03:17.059292 pyblu-0.2.0/src/pyblu/__init__.py
+-rw-r--r--   0        0        0     3854 2024-04-14 21:19:56.510398 pyblu-0.2.0/src/pyblu/_entities.py
+-rw-r--r--   0        0        0     5285 2024-04-19 13:03:35.299226 pyblu-0.2.0/src/pyblu/_parse.py
+-rw-r--r--   0        0        0    14366 2024-04-19 12:59:59.733715 pyblu-0.2.0/src/pyblu/_player.py
+-rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 pyblu-0.2.0/PKG-INFO
```

### Comparing `pyblu-0.1.0/LICENSE` & `pyblu-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyblu-0.1.0/README.md` & `pyblu-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyblu
 
 [![PyPI](https://img.shields.io/pypi/v/pyblu)](https://pypi.org/project/pyblu/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyblu)](https://pypi.org/project/pyblu/)
-[![PyPI - License](https://img.shields.io/pypi/l/pyblu)](https://github.com/LouisChrist/python-pyblu/blob/main/LICENSE)
+[![PyPI - License](https://img.shields.io/pypi/l/pyblu)](https://github.com/LouisChrist/pyblu/blob/main/LICENSE)
 
 This is a Python library for interfacing with BluOS players. 
 It uses the 
 [BluOS API](https://bluesound-deutschland.de/wp-content/uploads/2022/01/Custom-Integration-API-v1.0_March-2021.pdf) 
 to control and query the status of BluOS players.
 Authentication is not required.
```

### Comparing `pyblu-0.1.0/pyproject.toml` & `pyblu-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyblu"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Louis Christ <mail@louischrist.de>"]
 repository = "https://github.com/LouisChrist/pyblu"
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "pyblu", from = "src" },
```

### Comparing `pyblu-0.1.0/src/pyblu/_player.py` & `pyblu-0.2.0/src/pyblu/_player.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,13 @@
-from typing import TypeVar, Union, Callable, TypeAlias
-
 import aiohttp
 import xmltodict
+from urllib.parse import unquote
 
-from pyblu._entities import Status, Volume, SyncStatus, PairedPlayer
-
-StringDict: TypeAlias = dict[str, Union[str, "StringDict"]]
-# pylint: disable=invalid-name
-T: TypeAlias = TypeVar("T")
-
-
-def chained_get(data: StringDict, *keys, _map: Callable[[str], T] = lambda x: x) -> T | None:
-    local_data = data
-    for key in keys:
-        local_data = local_data.get(key)
-        if not local_data:
-            return None
-    return _map(local_data)
+from pyblu._entities import Status, Volume, SyncStatus, PairedPlayer, PlayQueue, Preset, Input
+from pyblu._parse import parse_slave_list, parse_sync_status, parse_status, parse_volume, chained_get, parse_play_queue, parse_presets
 
 
 class Player:
     def __init__(self, host: str, port: int = 11000, session: aiohttp.ClientSession = None):
         """Client for a BluOS player. Uses the HTTP API of the BluOS players to control it.
 
         The passed sessions will not be closed when the player is closed and has to be closed by the caller.
@@ -68,26 +55,15 @@
             params["etag"] = etag
             params["timeout"] = timeout
         async with self._session.get(f"{self.base_url}/Status", params=params) as response:
             response.raise_for_status()
             response_data = await response.text()
             response_dict = xmltodict.parse(response_data)
 
-            status = Status(
-                etag=chained_get(response_dict, "status", "@etag"),
-                state=chained_get(response_dict, "status", "state"),
-                album=chained_get(response_dict, "status", "album"),
-                artist=chained_get(response_dict, "status", "artist"),
-                name=chained_get(response_dict, "status", "title1"),
-                image=chained_get(response_dict, "status", "image"),
-                volume=chained_get(response_dict, "status", "volume", _map=int),
-                mute=chained_get(response_dict, "status", "mute") == "1",
-                seconds=chained_get(response_dict, "status", "secs", _map=int),
-                total_seconds=chained_get(response_dict, "status", "totlen", _map=float),
-            )
+            status = parse_status(response_dict)
 
             return status
 
     async def sync_status(self, etag: str | None = None, timeout: int = 30) -> SyncStatus:
         """Get the SyncStatus of the player.
 
         This endpoint supports long polling. If **etag** is set, the server will wait until the status changes or the timeout is reached.
@@ -103,44 +79,15 @@
             params["etag"] = etag
             params["timeout"] = timeout
         async with self._session.get(f"{self.base_url}/SyncStatus", params=params) as response:
             response.raise_for_status()
             response_data = await response.text()
             response_dict = xmltodict.parse(response_data)
 
-            master_ip = chained_get(response_dict, "SyncStatus", "master", "#text")
-            master_port = chained_get(response_dict, "SyncStatus", "master", "@port")
-            master = PairedPlayer(ip=master_ip, port=int(master_port)) if master_ip and master_port else None
-
-            slaves_raw = chained_get(response_dict, "SyncStatus", "slave")
-            slaves = _parse_slave_list(slaves_raw)
-
-            sync_status = SyncStatus(
-                etag=chained_get(response_dict, "SyncStatus", "@etag"),
-                sync_stat=chained_get(response_dict, "SyncStatus", "@syncStat"),
-                id=chained_get(response_dict, "SyncStatus", "@id"),
-                mac=chained_get(response_dict, "SyncStatus", "@mac"),
-                name=chained_get(response_dict, "SyncStatus", "@name"),
-                icon_url=chained_get(response_dict, "SyncStatus", "@icon"),
-                initialized=chained_get(response_dict, "SyncStatus", "@initialized") == "true",
-                group=chained_get(response_dict, "SyncStatus", "@group"),
-                master=master,
-                slaves=slaves,
-                zone=chained_get(response_dict, "SyncStatus", "@zone"),
-                zone_master=chained_get(response_dict, "SyncStatus", "@zoneMaster") == "true",
-                zone_slave=chained_get(response_dict, "SyncStatus", "@zoneSlave") == "true",
-                brand=chained_get(response_dict, "SyncStatus", "@brand"),
-                model=chained_get(response_dict, "SyncStatus", "@model"),
-                model_name=chained_get(response_dict, "SyncStatus", "@modelName"),
-                mute_volume_db=chained_get(response_dict, "SyncStatus", "@muteDb", _map=int),
-                mute_volume=chained_get(response_dict, "SyncStatus", "@muteVolume", _map=int),
-                volume_db=chained_get(response_dict, "SyncStatus", "@db", _map=int),
-                volume=chained_get(response_dict, "SyncStatus", "@volume", _map=int),
-                schema_version=chained_get(response_dict, "SyncStatus", "@schemaVersion", _map=int),
-            )
+            sync_status = parse_sync_status(response_dict)
 
             return sync_status
 
     async def volume(self, level: int = None, mute: bool = None, tell_slaves: bool = None) -> Volume:
         """Get or set the volume of the player.
         Call without parameters to get the current volume. Call with parameters to set the volume.
 
@@ -159,19 +106,15 @@
             params["tell_slaves"] = "1" if tell_slaves else "0"
 
         async with self._session.get(f"{self.base_url}/Volume", params=params) as response:
             response.raise_for_status()
             response_data = await response.text()
             response_dict = xmltodict.parse(response_data)
 
-            volume = Volume(
-                volume=chained_get(response_dict, "volume", "#text", _map=int),
-                db=chained_get(response_dict, "volume", "@db", _map=float),
-                mute=chained_get(response_dict, "volume", "@mute") == "1",
-            )
+            volume = parse_volume(response_dict)
 
             return volume
 
     async def play(self, seek: int = None) -> str:
         """Start playing the current track. Can also be used to seek within the current track.
         Works only when paused, not when stopped.
 
@@ -186,14 +129,31 @@
         async with self._session.get(f"{self.base_url}/Play", params=params) as response:
             response.raise_for_status()
             response_data = await response.text()
             response_dict = xmltodict.parse(response_data)
 
             return chained_get(response_dict, "state")
 
+    async def play_url(self, url: str) -> str:
+        """Start playing a track from a URL. Can also be used to select inputs. See *inputs* for available inputs.
+
+        :param url: The URL of the track to play.
+
+        :return: The playback state after command execution.
+        """
+        params = {
+            "url": url,
+        }
+        async with self._session.get(f"{self.base_url}/Play", params=params) as response:
+            response.raise_for_status()
+            response_data = await response.text()
+            response_dict = xmltodict.parse(response_data)
+
+            return chained_get(response_dict, "state")
+
     async def pause(self, toggle: bool = None) -> str:
         """Pause the current track. **toggle** can be used to toggle between playing and pause.
 
         :param toggle: Toggle between playing and pause.
 
         :return: The playback state after command execution.
         """
@@ -245,15 +205,15 @@
         }
         async with self._session.get(f"{self.base_url}/AddSlave", params=params) as response:
             response.raise_for_status()
             response_data = await response.text()
             response_dict = xmltodict.parse(response_data)
 
             slaves_raw = chained_get(response_dict, "addSlave", "slave")
-            slaves = _parse_slave_list(slaves_raw)
+            slaves = parse_slave_list(slaves_raw)
 
             return slaves
 
     async def add_slaves(self, slaves: list[PairedPlayer]) -> list[PairedPlayer]:
         """Add a list of secondary players to the current player as slaves.
         If it fails the player won't be in the returned list.
 
@@ -269,20 +229,156 @@
         }
         async with self._session.get(f"{self.base_url}/AddSlave", params=params) as response:
             response.raise_for_status()
             response_data = await response.text()
             response_dict = xmltodict.parse(response_data)
 
             slaves_raw = chained_get(response_dict, "addSlave", "slave")
-            slaves = _parse_slave_list(slaves_raw)
+            slaves = parse_slave_list(slaves_raw)
 
             return slaves
 
+    async def remove_slave(self, ip: str, port: int = 11000) -> SyncStatus:
+        """Remove a secondary player from the group.
+
+        :param ip: The IP address of the player to remove.
+        :param port: The port of the player to remove. Default is 11000.
+
+        :return: The SyncStatus of the player.
+        """
+        params = {
+            "slave": ip,
+            "port": port,
+        }
+        async with self._session.get(f"{self.base_url}/RemoveSlave", params=params) as response:
+            response.raise_for_status()
+            response_data = await response.text()
+            response_dict = xmltodict.parse(response_data)
+
+            sync_status = parse_sync_status(response_dict)
+
+            return sync_status
+
+    async def remove_slaves(self, slaves: list[PairedPlayer]) -> SyncStatus:
+        """Remove a list of secondary players from the group.
+
+        Same as *remove_slave* but with a list of players. Makes only one request to player.
+
+        :param slaves: The list of players to remove.
+
+        :return: The SyncStatus of the player.
+        """
+        params = {
+            "slaves": ",".join(x.ip for x in slaves),
+            "ports": ",".join(str(x.port) for x in slaves),
+        }
+        async with self._session.get(f"{self.base_url}/RemoveSlave", params=params) as response:
+            response.raise_for_status()
+            response_data = await response.text()
+            response_dict = xmltodict.parse(response_data)
+
+            sync_status = parse_sync_status(response_dict)
+
+            return sync_status
+
+    async def shuffle(self, shuffle: bool) -> PlayQueue:
+        """Set shuffle on current play queue.
+
+        :param shuffle: Whether to shuffle the playlist.
+
+        :return: The current play queue.
+        """
+        params = {
+            "shuffle": "1" if shuffle else "0",
+        }
+        async with self._session.get(f"{self.base_url}/Shuffle", params=params) as response:
+            response.raise_for_status()
+            response_data = await response.text()
+            response_dict = xmltodict.parse(response_data)
+
+            play_queue = parse_play_queue(response_dict)
+
+            return play_queue
+
+    async def clear(self) -> PlayQueue:
+        """Clear the play queue.
+
+        :return: The current play queue.
+        """
+        async with self._session.get(f"{self.base_url}/Clear") as response:
+            response.raise_for_status()
+            response_data = await response.text()
+            response_dict = xmltodict.parse(response_data)
+
+            play_queue = parse_play_queue(response_dict)
+
+            return play_queue
+
+    async def sleep_timer(self) -> int:
+        """Set sleep timer. Time steps are 15, 30, 45, 60, 90 minutes. Each call goes to next step.
+        Resets to 0 if called when 90 minutes are set.
+
+        :return: The current sleep timer in minutes. 0 if no sleep timer is set.
+        """
+        async with self._session.get(f"{self.base_url}/Sleep") as response:
+            response.raise_for_status()
+            response_data = await response.text()
+            response_dict = xmltodict.parse(response_data)
+
+            sleep_timer = chained_get(response_dict, "sleep", _map=int)
+            if not sleep_timer:
+                sleep_timer = 0
+
+            return sleep_timer
+
+    async def presets(self) -> list[Preset]:
+        """Get the list of presets of the player.
+
+        :return: The list of presets of the player.
+        """
+        async with self._session.get(f"{self.base_url}/Presets") as response:
+            response.raise_for_status()
+            response_data = await response.text()
+            response_dict = xmltodict.parse(response_data)
+
+            presets = parse_presets(response_dict)
+
+            return presets
+
+    async def load_preset(self, preset_id: int) -> None:
+        """Load a preset by ID.
+
+        :param preset_id: The ID of the preset to load.
+        """
+        params = {
+            "id": preset_id,
+        }
+        async with self._session.get(f"{self.base_url}/Preset", params=params) as response:
+            response.raise_for_status()
+
+    async def inputs(self) -> list[Input]:
+        """List all available inputs.
+
+        :return: The list of inputss of the player.
+        """
+        params = {"service": "Capture"}
+        async with self._session.get(f"{self.base_url}/RadioBrowse", params=params) as response:
+            response.raise_for_status()
+            response_data = await response.text()
+            response_dict = xmltodict.parse(response_data)
+
+            inputs_raw = chained_get(response_dict, "radiotime", "item")
+
+            if not isinstance(inputs_raw, list):
+                inputs_raw = [inputs_raw]
+
+            inputs = [
+                Input(
+                    id=chained_get(x, "@id"),
+                    text=chained_get(x, "@text"),
+                    image=chained_get(x, "@image"),
+                    url=chained_get(x, "@URL", _map=unquote),
+                )
+                for x in inputs_raw
+            ]
 
-def _parse_slave_list(slaves_raw: list[dict[str, str]]) -> list[PairedPlayer] | None:
-    match slaves_raw:
-        case {"@id": ip, "@port": port}:
-            return [PairedPlayer(ip=ip, port=int(port))]
-        case [*slaves_raw]:
-            return [PairedPlayer(ip=slave["@id"], port=int(slave["@port"])) for slave in slaves_raw]
-        case _:
-            return None
+            return inputs
```

### Comparing `pyblu-0.1.0/PKG-INFO` & `pyblu-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyblu
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Home-page: https://github.com/LouisChrist/pyblu
 License: MIT
 Author: Louis Christ
 Author-email: mail@louischrist.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 Project-URL: Repository, https://github.com/LouisChrist/pyblu
 Description-Content-Type: text/markdown
 
 # pyblu
 
 [![PyPI](https://img.shields.io/pypi/v/pyblu)](https://pypi.org/project/pyblu/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyblu)](https://pypi.org/project/pyblu/)
-[![PyPI - License](https://img.shields.io/pypi/l/pyblu)](https://github.com/LouisChrist/python-pyblu/blob/main/LICENSE)
+[![PyPI - License](https://img.shields.io/pypi/l/pyblu)](https://github.com/LouisChrist/pyblu/blob/main/LICENSE)
 
 This is a Python library for interfacing with BluOS players. 
 It uses the 
 [BluOS API](https://bluesound-deutschland.de/wp-content/uploads/2022/01/Custom-Integration-API-v1.0_March-2021.pdf) 
 to control and query the status of BluOS players.
 Authentication is not required.
```

