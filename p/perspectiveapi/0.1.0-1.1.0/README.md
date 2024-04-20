# Comparing `tmp/perspectiveapi-0.1.0.tar.gz` & `tmp/perspectiveapi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perspectiveapi-0.1.0.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `perspectiveapi-0.1.0.tar` & `perspectiveapi-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,14 @@
--rw-r--r--   0        0        0     1062 2023-02-24 02:46:03.000000 perspectiveapi-0.1.0/LICENSE
--rw-r--r--   0        0        0      405 2023-02-24 15:38:31.580253 perspectiveapi-0.1.0/README.md
--rw-r--r--   0        0        0       50 2023-02-24 15:33:57.308475 perspectiveapi-0.1.0/perspective/__init__.py
--rw-r--r--   0        0        0     2219 2023-02-24 15:37:46.224295 perspectiveapi-0.1.0/perspective/models.py
--rw-r--r--   0        0        0      467 2023-02-24 16:00:55.475048 perspectiveapi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1089 1970-01-01 00:00:00.000000 perspectiveapi-0.1.0/setup.py
--rw-r--r--   0        0        0     1029 1970-01-01 00:00:00.000000 perspectiveapi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 perspectiveapi-1.1.0/requirements-dev.lock
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 perspectiveapi-1.1.0/requirements.lock
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 perspectiveapi-1.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 perspectiveapi-1.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 perspectiveapi-1.1.0/perspective/__init__.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 perspectiveapi-1.1.0/perspective/blocking.py
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 perspectiveapi-1.1.0/perspective/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 perspectiveapi-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 perspectiveapi-1.1.0/tests/test_perspective.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 perspectiveapi-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 perspectiveapi-1.1.0/LICENSE
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 perspectiveapi-1.1.0/README.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 perspectiveapi-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 perspectiveapi-1.1.0/PKG-INFO
```

### Comparing `perspectiveapi-0.1.0/LICENSE` & `perspectiveapi-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `perspectiveapi-0.1.0/perspective/models.py` & `perspectiveapi-1.1.0/perspective/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,102 @@
-from __future__ import annotations
+# from __future__ import annotations
 from typing import List
-from aiohttp import ClientSession
-from orjson import dumps
 from enum import Enum
+from typing import Dict
+from httpx import AsyncClient
 
-
-class Attribute(Enum):
-    __slots__ = (
-        "toxicity",
-        "severe_toxicity",
-        "insult",
-        "threat",
-        "sexually_explicit",
-        "flirtation",
-    )
-    toxicity = "TOXICITY"
-    severe_toxicity = "SEVERE_TOXICITY"
-    insult = "INSULT"
-    threat = "THREAT"
-    sexually_explicit = "SEXUALLY_EXPLICIT"
-    flirtation = "FLIRTATION"
-
-
-class Perspective:
-    __slots__ = ("__key", "session", "attributes")
-
-    def __init__(self, key: str):
-        self.__key: str = key
-
-    async def score(
-        self, message: str, attributes: List[Attribute] = [Attribute.toxicity]
-    ) -> Score:
-        if isinstance(attributes, Attribute):
-            attributes = [attributes]
-
-        if not all(isinstance(attribute, Attribute) for attribute in attributes):
-            raise ValueError("Attributes are invalid!")
-
-        requested_attributes = {attribute.value: {} for attribute in attributes}
-
-        payload = dumps(
-            dict(
-                languages=["en"],
-                comment={"text": message},
-                requestedAttributes=requested_attributes,
-            )
-        )
-        async with ClientSession() as session:
-            res = await session.post(
-                f"https://commentanalyzer.googleapis.com/v1alpha1/comments:analyze",
-                data=payload,
-                params={"key": self.__key},
-            )
-        return Score(await res.json())
+Attribute = Enum(
+    "Attribute",
+    [
+        "TOXICITY",
+        "SEVERE_TOXICITY",
+        "INSULT",
+        "THREAT",
+        "SEXUALLY_EXPLICIT",
+        "FLIRTATION",
+    ],
+)
+"""An Enum containing the attributes to scan text for. This controls the requestedAttributes field of the request.
+
+Raises:
+    AttributeError: If the attributes are invalid.
+"""
 
 
 class Score:
+    """The attribute score of the scanned message. You should never have to intialize this class yourself."""
+
     __slots__ = (
         "toxicity",
         "severe_toxicity",
         "insult",
         "threat",
         "sexually_explicit",
         "flirtation",
     )
 
-    def __init__(self, res: dict):
+    def __init__(self, res: Dict[str, dict]):
         self.toxicity: float
         self.severe_toxicity: float
         self.insult: float
         self.sexually_explicit: float
         self.flirtation: float
 
-        for i in Attribute.__members__:
+        for attribute in Attribute:
             setattr(
                 self,
-                i.lower(),
+                attribute.name.lower(),
                 res["attributeScores"]
-                .get(str(i).upper(), {})
+                .get(attribute.name.upper(), {})
                 .get("summaryScore", {})
-                .get("value", None),
+                .get("value"),
             )
+
+
+class Perspective:
+    """The Perspective API client.
+
+    Args:
+        key (str): Your Perspective API key.
+    """
+
+    __slots__ = ("__key", "session", "attributes", "__client")
+
+    def __init__(self, key: str):
+        self.__key: str = key
+        self.__client = AsyncClient()
+
+    async def score(
+        self, message: str, attributes: List[Attribute] = [Attribute.TOXICITY]
+    ) -> Score:
+        """Makes a request to the Perspective API.
+
+        Args:
+            message (str): The message to scan.
+            attributes (List[Attribute], optional): The attributes to scan the messages for. Defaults to [Attribute.TOXICITY].
+
+        Raises:
+            ValueError: If the attributes are invalid.
+
+        Returns:
+            Score: The attribute scores of the scanned message.
+        """
+        attributes = list(attributes)
+
+        if not all(isinstance(attribute, Attribute) for attribute in attributes):
+            raise ValueError("Attributes are invalid!")
+
+        requested_attributes: Dict[str, dict] = {
+            attribute.name: {} for attribute in attributes
+        }
+
+        payload = dict(
+            languages=["en"],
+            comment={"text": message},
+            requestedAttributes=requested_attributes,
+        )
+        res = await self.__client.post(
+            "https://commentanalyzer.googleapis.com/v1alpha1/comments:analyze",
+            json=payload,
+            params={"key": self.__key},
+        )
+        return Score(res.json())
```

