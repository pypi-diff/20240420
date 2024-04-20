# Comparing `tmp/humemai-1.0.0.tar.gz` & `tmp/humemai-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humemai-1.0.0.tar", last modified: Fri Apr  5 15:12:11 2024, max compression
+gzip compressed data, was "humemai-1.0.1.tar", last modified: Sat Apr 20 09:34:57 2024, max compression
```

## Comparing `humemai-1.0.0.tar` & `humemai-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:11.207245 humemai-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 15:11:59.000000 humemai-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-05 15:12:11.207245 humemai-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-05 15:11:59.000000 humemai-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:11.207245 humemai-1.0.0/humemai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:11:59.000000 humemai-1.0.0/humemai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29982 2024-04-05 15:11:59.000000 humemai-1.0.0/humemai/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    14656 2024-04-05 15:11:59.000000 humemai-1.0.0/humemai/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-04-05 15:11:59.000000 humemai-1.0.0/humemai/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:11.207245 humemai-1.0.0/humemai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-05 15:12:11.000000 humemai-1.0.0/humemai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-05 15:12:11.000000 humemai-1.0.0/humemai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:12:11.000000 humemai-1.0.0/humemai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-05 15:12:11.000000 humemai-1.0.0/humemai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 15:12:11.000000 humemai-1.0.0/humemai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-05 15:12:11.211245 humemai-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 15:11:59.000000 humemai-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:11.207245 humemai-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)    42568 2024-04-05 15:11:59.000000 humemai-1.0.0/test/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    29843 2024-04-05 15:11:59.000000 humemai-1.0.0/test/test_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-05 15:11:59.000000 humemai-1.0.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:34:57.011994 humemai-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-20 09:34:47.000000 humemai-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-20 09:34:57.011994 humemai-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-20 09:34:47.000000 humemai-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:34:57.011994 humemai-1.0.1/humemai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 09:34:47.000000 humemai-1.0.1/humemai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32182 2024-04-20 09:34:47.000000 humemai-1.0.1/humemai/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-04-20 09:34:47.000000 humemai-1.0.1/humemai/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-04-20 09:34:47.000000 humemai-1.0.1/humemai/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:34:57.011994 humemai-1.0.1/humemai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-20 09:34:56.000000 humemai-1.0.1/humemai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-20 09:34:56.000000 humemai-1.0.1/humemai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 09:34:56.000000 humemai-1.0.1/humemai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-20 09:34:56.000000 humemai-1.0.1/humemai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 09:34:56.000000 humemai-1.0.1/humemai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-20 09:34:57.011994 humemai-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-20 09:34:47.000000 humemai-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:34:57.011994 humemai-1.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    42246 2024-04-20 09:34:47.000000 humemai-1.0.1/test/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29843 2024-04-20 09:34:47.000000 humemai-1.0.1/test/test_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-20 09:34:47.000000 humemai-1.0.1/test/test_utils.py
```

### Comparing `humemai-1.0.0/LICENSE` & `humemai-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `humemai-1.0.0/PKG-INFO` & `humemai-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: humemai
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Machine With Human-Like Memory Systems.
 Home-page: https://github.com/humemai/humemai
 Author: Taewoon Kim
 Author-email: info@humem.ai
 Project-URL: Bug Tracker, https://github.com/humemai/humemai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,19 +12,21 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # humemai
 
 [![DOI](https://zenodo.org/badge/614376180.svg)](https://zenodo.org/doi/10.5281/zenodo.10876440)
+[![PyPI
+version](https://badge.fury.io/py/humemai.svg)](https://badge.fury.io/py/humemai)
 
 This repo hosts a package `humemai`, a human-like memory systems that are modeled with
 knowledge knoweldge graphs (KGs). At the moment they are nothing but a Python list of
 quadruples, but soon it'll be a better object type so that they can be compatible with
-graph databases, e.g., GraphDB, Neo4j, etc. There have been both [academic
+graph databases, e.g., RDFLib, GraphDB, Neo4j, etc. There have been both [academic
 papers](#list-of-academic-papers-that-use-humemai) and
 [applications](#list-of-applications-that-use-humemai) that have used this package.
 
 ## List of academic papers that use HumemAI
 
 - ["A Machine With Human-Like Memory Systems"](https://arxiv.org/abs/2204.01611).
 - ["A Machine with Short-Term, Episodic, and Semantic Memory
```

### Comparing `humemai-1.0.0/README.md` & `humemai-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # humemai
 
 [![DOI](https://zenodo.org/badge/614376180.svg)](https://zenodo.org/doi/10.5281/zenodo.10876440)
+[![PyPI
+version](https://badge.fury.io/py/humemai.svg)](https://badge.fury.io/py/humemai)
 
 This repo hosts a package `humemai`, a human-like memory systems that are modeled with
 knowledge knoweldge graphs (KGs). At the moment they are nothing but a Python list of
 quadruples, but soon it'll be a better object type so that they can be compatible with
-graph databases, e.g., GraphDB, Neo4j, etc. There have been both [academic
+graph databases, e.g., RDFLib, GraphDB, Neo4j, etc. There have been both [academic
 papers](#list-of-academic-papers-that-use-humemai) and
 [applications](#list-of-applications-that-use-humemai) that have used this package.
 
 ## List of academic papers that use HumemAI
 
 - ["A Machine With Human-Like Memory Systems"](https://arxiv.org/abs/2204.01611).
 - ["A Machine with Short-Term, Episodic, and Semantic Memory
```

### Comparing `humemai-1.0.0/humemai/memory.py` & `humemai-1.0.1/humemai/memory.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,36 +13,49 @@
     level=os.environ.get("LOGLEVEL", "INFO").upper(),
     format="%(asctime)s.%(msecs)03d %(levelname)s %(module)s - %(funcName)s: %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
 )
 
 
 class Memory:
-    """Memory (episodic, semantic, or short) class"""
+    """Memory class.
 
-    def __init__(self, memory_type: str, capacity: int) -> None:
+    At the moment, the memory system is a simple Python list of memories. In the future,
+    a more suitable python object will be used to represent the graph structure of the
+    memories.
+
+    Attributes:
+        type: episodic, semantic, short, or working
+        entries: list of memories
+        capacity: memory capacity
+        _frozen: whether the memory system is frozen or not
+
+    """
+
+    def __init__(self, capacity: int, memories: list | None = None) -> None:
         """
 
         Args:
-            memory_type: episodic, semantic, or short
             capacity: memory capacity
+            memories: memories that can already be added from the beginning, if None,
+                then it's an empty memory system.
 
         """
-        logging.debug(
-            f"instantiating a {memory_type} memory object with size {capacity} ..."
-        )
+        logging.debug(f"instantiating a memory object with size {capacity} ...")
 
-        assert memory_type in ["episodic", "semantic", "short"]
-        self.type = memory_type
         self.entries = []
         self.capacity = capacity
         assert self.capacity >= 0
         self._frozen = False
 
-        logging.debug(f"{memory_type} memory object with size {capacity} instantiated!")
+        logging.debug(f"Memory systrem with size {capacity} instantiated!")
+
+        if memories is not None:
+            for mem in memories:
+                self.add(mem)
 
     def __repr__(self):
         return pformat(vars(self), indent=4, width=1)
 
     def can_be_added(self, mem: list[str]) -> tuple[bool, str]:
         """Check if a memory can be added to the system or not.
 
@@ -61,14 +74,18 @@
             return False, "The memory system is frozen!"
 
         if self.is_full:
             return False, "The memory system is full!"
 
         return True, ""
 
+    def __add__(self, other):
+        entries = self.entries + other.entries
+        return Memory(self.capacity + other.capacity, entries)
+
     def add(self, mem: list[str]) -> None:
         """Add memory to the memory system.
 
         Args:
            mem: A memory as a quadraple: [head, relation, tail, num]
 
         """
@@ -349,24 +366,32 @@
 
         return mems_found
 
 
 class EpisodicMemory(Memory):
     """Episodic memory class."""
 
-    def __init__(self, capacity: int, remove_duplicates: bool = False) -> None:
+    def __init__(
+        self,
+        capacity: int,
+        memories: list | None = None,
+        remove_duplicates: bool = False,
+    ) -> None:
         """Init an episodic memory system.
 
         Args:
             capacity: capacity of the memory system (i.e., number of entries)
+            memories: memories that can already be added from the beginning, if None,
+                then it's an empty memory system.
             remove_duplicates: if True, it'll remove the same memories with the older
                 timestamps.
 
         """
-        super().__init__("episodic", capacity)
+        super().__init__(capacity, memories)
+        self.type = "episodic"
         self.remove_duplicates = remove_duplicates
 
     def add(self, mem: list[str]) -> None:
         """Append a memory to the episodic memory system.
 
         Args:
             mem: An episodic memory as a quadraple: [head, relation, tail, timestamp]
@@ -553,16 +578,17 @@
         else:
             raise ValueError("Something is wrong!")
 
 
 class ShortMemory(Memory):
     """Short-term memory class."""
 
-    def __init__(self, capacity: int) -> None:
-        super().__init__("short", capacity)
+    def __init__(self, capacity: int, memories: list | None = None) -> None:
+        super().__init__(capacity, memories)
+        self.type = "short"
 
     def get_oldest_memory(self) -> list:
         return self.get_first_memory()
 
     def get_latest_memory(self) -> list:
         return self.get_last_memory()
 
@@ -631,15 +657,16 @@
         """Turn a short memory into a semantic memory.
 
         Args:
             short: A short memory as a quadruple: [head, relation, tail, timestamp]
             split_possessive: whether to split the possessive, i.e., 's, or not.
 
         Returns:
-            sem: A semantic memory as a quadruple: [head, relation, tail, NUM_GENERALIZED]
+            sem: A semantic memory as a quadruple: [head, relation, tail,
+                NUM_GENERALIZED]
 
         """
         sem = short[:-1]
 
         if split_possessive:
             sem = [remove_posession(elem) for elem in sem]
 
@@ -647,31 +674,32 @@
 
         return sem
 
 
 class SemanticMemory(Memory):
     """Semantic memory class."""
 
-    def __init__(
-        self,
-        capacity: int,
-    ) -> None:
+    def __init__(self, capacity: int, memories: list | None = None) -> None:
         """Init a semantic memory system.
 
         Args:
             capacity: capacity of the memory system (i.e., number of entries)
+            memories: memories that can already be added from the beginning, if None,
+                then it's an empty memory system.
 
         """
-        super().__init__("semantic", capacity)
+        super().__init__(capacity, memories)
+        self.type = "semantic"
 
     def can_be_added(self, mem: list[str]) -> bool:
         """Checks if a memory can be added to the system or not.
 
         Args:
-            mem: A semantic memory as a quadraple: [head, relation, tail, num_generalized]
+            mem: A semantic memory as a quadraple: [head, relation, tail,
+                num_generalized]
 
         Returns:
             True or False
 
         """
         if self.capacity == 0:
             return False, "The memory system capacity is 0!"
@@ -872,14 +900,22 @@
             entries_cleaned.append(mem)
 
         self.entries = entries_cleaned
         self.entries.sort(key=lambda x: x[-1])
         logging.debug(f"There are {len(self.entries)} episodic memories after cleaning")
 
 
+class WorkingMemory(Memory):
+    """Working memory class."""
+
+    def __init__(self, capacity: int, memories: list | None = None) -> None:
+        super().__init__(capacity)
+        self.type = "working"
+
+
 class MemorySystems:
     """Multiple memory systems class."""
 
     def __init__(
         self,
         episodic: EpisodicMemory = None,
         episodic_agent: EpisodicMemory = None,
@@ -904,20 +940,44 @@
         if semantic is not None and semantic.capacity > 0:
             self.semantic = semantic
         if semantic_map is not None and semantic_map.capacity > 0:
             self.semantic_map = semantic_map
         if short is not None and short.capacity > 0:
             self.short = short
 
+    def get_working_memory(self, num_hops: int | str = "all") -> Memory:
+        """Get the working memory system.
+
+        The working memory system is defined as short-term memory + partial long-term
+            memory (episodic and semantic).
+
+        Args:
+            num_hops: number of hops to consider when fetching long-term memories
+            (episodic and semantic). If "all", then basically it's infinity, which
+            means all long-term memories will be considered.
+
+        Returns:
+            working_memory: the working memory system
+
+        """
+        if num_hops == "all":
+            return self.short + self.episodic + self.semantic
+        else:
+            raise NotImplementedError("Not implemented yet!")
+
     def return_as_a_dict_list(self) -> dict[str, list[list[str]]]:
         """Return memory systems as a dictionary of lists.
 
         Returns:
-            to_return: a dictionary of lists. This is a  state is a list, which is a
-                mutable object. So, deepcopy it, if you want to keep the original state.
+            to_return: a dictionary of lists. At the moment, memories are nothing but
+                python lists (lists of quadruples), which is a mutable object. So,
+                deepcopy it, if you want to keep the original state. In the future, a
+                more suitable python object will be used to represent the graph
+                structure of the memories.
+
         """
         to_return = {}
         if hasattr(self, "episodic"):
             to_return["episodic"] = self.episodic.return_as_list()
         if hasattr(self, "episodic_agent"):
             to_return["episodic_agent"] = self.episodic_agent.return_as_list()
         if hasattr(self, "semantic"):
```

### Comparing `humemai-1.0.0/humemai/policy.py` & `humemai-1.0.1/humemai/policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,30 +9,45 @@
 import numpy as np
 import torch
 
 from .memory import EpisodicMemory, MemorySystems, SemanticMemory, ShortMemory
 from .utils import argmax
 
 
-def encode_observation(memory_systems: MemorySystems, obs: list[list]) -> None:
+def encode_observation(memory_systems: MemorySystems, obs: list[str | int]) -> None:
     """Non RL policy of encoding an observation into a short-term memory.
 
     At the moment, observation is the same as short-term memory. However, in the future
     we may want to encode the observation into a different format, e.g., when
-    observatio is in the pixel space.
+    observation is in the pixel space.
 
     Args:
         MemorySystems
         obs: observation as a quadruple: [head, relation, tail, num]
 
     """
     mem_short = ShortMemory.ob2short(obs)
     memory_systems.short.add(mem_short)
 
 
+def encode_all_observations(
+    memory_systems: MemorySystems, obs_multiple: list[list[str | int]]
+) -> None:
+    """Non RL policy of encoding all observations into short-term memories.
+
+    Args:
+        MemorySystems
+        obs_multiple: a list of observations
+
+    """
+    for obs in obs_multiple:
+        mem_short = ShortMemory.ob2short(obs)
+        memory_systems.short.add(mem_short)
+
+
 def find_agent_current_location(memory_systems: MemorySystems) -> str:
     """Find the current location of the agent.
 
     If memory_systems has episodic_agent, then it is used to find the current location
     if not, it looks up the episodic. If fails, it looks up the semantic.
     If all fails, it returns None.
```

### Comparing `humemai-1.0.0/humemai/utils.py` & `humemai-1.0.1/humemai/utils.py`

 * *Files identical despite different names*

### Comparing `humemai-1.0.0/humemai.egg-info/PKG-INFO` & `humemai-1.0.1/humemai.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: humemai
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Machine With Human-Like Memory Systems.
 Home-page: https://github.com/humemai/humemai
 Author: Taewoon Kim
 Author-email: info@humem.ai
 Project-URL: Bug Tracker, https://github.com/humemai/humemai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,19 +12,21 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # humemai
 
 [![DOI](https://zenodo.org/badge/614376180.svg)](https://zenodo.org/doi/10.5281/zenodo.10876440)
+[![PyPI
+version](https://badge.fury.io/py/humemai.svg)](https://badge.fury.io/py/humemai)
 
 This repo hosts a package `humemai`, a human-like memory systems that are modeled with
 knowledge knoweldge graphs (KGs). At the moment they are nothing but a Python list of
 quadruples, but soon it'll be a better object type so that they can be compatible with
-graph databases, e.g., GraphDB, Neo4j, etc. There have been both [academic
+graph databases, e.g., RDFLib, GraphDB, Neo4j, etc. There have been both [academic
 papers](#list-of-academic-papers-that-use-humemai) and
 [applications](#list-of-applications-that-use-humemai) that have used this package.
 
 ## List of academic papers that use HumemAI
 
 - ["A Machine With Human-Like Memory Systems"](https://arxiv.org/abs/2204.01611).
 - ["A Machine with Short-Term, Episodic, and Semantic Memory
```

### Comparing `humemai-1.0.0/setup.cfg` & `humemai-1.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = humemai
-version = 1.0.0
+version = 1.0.1
 author = Taewoon Kim
 author_email = info@humem.ai
 description = A Machine With Human-Like Memory Systems.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/humemai/humemai
 project_urls =
```

### Comparing `humemai-1.0.0/test/test_memory.py` & `humemai-1.0.1/test/test_memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,30 +3,26 @@
 import unittest
 
 from humemai.memory import *
 
 
 class MemoryTest(unittest.TestCase):
     def setUp(self) -> None:
-        self.memory = Memory(memory_type="episodic", capacity=8)
-
-    def test_init(self):
-        with self.assertRaises(AssertionError):
-            foo = Memory(memory_type="foo", capacity=0)
+        self.memory = Memory(capacity=8)
 
     def test_can_be_added(self):
-        memory = Memory(memory_type="episodic", capacity=0)
+        memory = Memory(capacity=0)
         self.assertFalse(memory.can_be_added(["foo", "bar", "baz", 1])[0])
 
-        memory = Memory(memory_type="semantic", capacity=4)
+        memory = Memory(capacity=4)
         memory.freeze()
         self.assertFalse(memory.can_be_added(["foo", "bar", "baz", 1])[0])
 
         memory.unfreeze()
-        memory = Memory(memory_type="short", capacity=1)
+        memory = Memory(capacity=1)
         memory.add(["foo", "bar", "baz", 1])
         self.assertFalse(memory.can_be_added(["foo", "bar", "baz", 1])[0])
 
     def test_add(self):
         self.memory.add(["foo", "bar", "baz", 1])
         self.assertEqual(self.memory.size, 1)
 
@@ -50,28 +46,28 @@
         timestamps = [mem[-1] for mem in self.memory.entries]
         self.assertEqual(sorted(timestamps), timestamps)
 
         with self.assertRaises(ValueError):
             self.memory.add(["foo", "bar", "baz", 9])
 
     def test_can_be_forgotten(self):
-        memory = Memory(memory_type="short", capacity=0)
+        memory = Memory(capacity=0)
         check, error_msg = memory.can_be_forgotten(["foo", "bar", "baz", 1])
         self.assertFalse(check)
 
-        memory = Memory(memory_type="semantic", capacity=4)
+        memory = Memory(capacity=4)
         check, error_msg = memory.can_be_forgotten(["foo", "bar", "baz", 1])
         self.assertFalse(check)
 
-        memory = Memory(memory_type="episodic", capacity=4)
+        memory = Memory(capacity=4)
         memory.freeze()
         check, error_msg = memory.can_be_forgotten(["foo", "bar", "baz", 1])
         self.assertFalse(check)
 
-        memory = Memory(memory_type="short", capacity=2)
+        memory = Memory(capacity=2)
         memory.add(["foo", "bar", "baz", 1])
         check, error_msg = memory.can_be_forgotten(["foo", "bar", "qux", 1])
         self.assertFalse(check)
 
     def test_forget(self):
         with self.assertRaises(ValueError):
             self.memory.forget(["foo", "bar", "baz", 2])
@@ -98,15 +94,15 @@
         self.memory.add(["foo", "bar", "baz", 2])
         self.memory.add(["foo", "bar", "baz", 3])
 
         self.memory.forget_all()
         self.assertEqual(self.memory.size, 0)
         self.assertTrue(self.memory.is_empty)
 
-        memory = Memory("short", 0)
+        memory = Memory(0)
         with self.assertRaises(ValueError):
             memory.forget_all()
 
     def test_forget_random(self):
         self.memory.add(["foo", "bar", "baz", 1])
         self.memory.add(["foo", "bar", "baz", 2])
         self.memory.add(["foo", "bar", "baz", 3])
```

### Comparing `humemai-1.0.0/test/test_policy.py` & `humemai-1.0.1/test/test_policy.py`

 * *Files identical despite different names*

### Comparing `humemai-1.0.0/test/test_utils.py` & `humemai-1.0.1/test/test_utils.py`

 * *Files identical despite different names*

