# Comparing `tmp/rtrie-0.1.3.tar.gz` & `tmp/rtrie-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtrie-0.1.3.tar", max compression
+gzip compressed data, was "rtrie-1.0.0.tar", max compression
```

## Comparing `rtrie-0.1.3.tar` & `rtrie-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rw-r--r--   0        0        0       65 2023-06-26 02:07:13.317162 rtrie-0.1.3/README.md
--rw-r--r--   0        0        0      886 2023-07-01 03:53:18.595569 rtrie-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      193 2023-07-04 04:23:45.805946 rtrie-0.1.3/src/rtrie/__init__.py
--rw-r--r--   0        0        0      158 2023-07-01 06:07:54.375569 rtrie-0.1.3/src/rtrie/__main__.py
--rw-r--r--   0        0        0     1136 2023-07-04 04:45:34.425946 rtrie-0.1.3/src/rtrie/array_trie.py
--rw-r--r--   0        0        0     1029 2023-06-26 02:21:05.787162 rtrie-0.1.3/src/rtrie/stats.py
--rw-r--r--   0        0        0      929 2023-07-04 04:45:40.315946 rtrie-0.1.3/src/rtrie/string_trie.py
--rw-r--r--   0        0        0    27026 2023-07-04 03:28:25.925946 rtrie-0.1.3/src/rtrie/trie.py
--rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 rtrie-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1256 2024-04-20 17:06:19.923309 rtrie-1.0.0/README.md
+-rw-r--r--   0        0        0      937 2024-04-20 17:06:19.933309 rtrie-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      359 2024-04-20 17:06:19.933309 rtrie-1.0.0/rtrie/__init__.py
+-rw-r--r--   0        0        0     1564 2024-04-20 17:06:19.933309 rtrie-1.0.0/rtrie/__main__.py
+-rw-r--r--   0        0        0     1132 2024-04-20 17:06:19.933309 rtrie-1.0.0/rtrie/array_trie.py
+-rw-r--r--   0        0        0     3184 2024-04-20 17:06:19.933309 rtrie-1.0.0/rtrie/naive_trie.py
+-rw-r--r--   0        0        0     6301 2024-04-20 17:06:19.933309 rtrie-1.0.0/rtrie/node.py
+-rw-r--r--   0        0        0     1029 2024-04-20 17:06:19.933309 rtrie-1.0.0/rtrie/stats.py
+-rw-r--r--   0        0        0     2048 2024-04-20 17:06:19.933309 rtrie-1.0.0/rtrie/stored_trie.py
+-rw-r--r--   0        0        0      275 2024-04-20 17:06:19.933309 rtrie-1.0.0/rtrie/string_trie.py
+-rw-r--r--   0        0        0    28995 2024-04-20 17:06:19.933309 rtrie-1.0.0/rtrie/trie.py
+-rw-r--r--   0        0        0      258 2024-04-20 17:06:19.933309 rtrie-1.0.0/rtrie/types.py
+-rw-r--r--   0        0        0     1733 1970-01-01 00:00:00.000000 rtrie-1.0.0/PKG-INFO
```

### Comparing `rtrie-0.1.3/pyproject.toml` & `rtrie-1.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 [tool.poetry]
 name = "rtrie"
-version = "0.1.3"
+version = "1.0.0"
 description = ""
 authors = ["alexgagnon <alex@monad.media>"]
 readme = "README.md"
 license = "MIT"
-packages = [{include = "rtrie", from = "src"}]
-
-# [tool.poetry.scripts]
-# dev = "rtrie:main"
+packages = [{include = "rtrie"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 rapidfuzz = "^3.1.1"
+argparse = "^1.4.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.0"
-deepdiff = "^6.3.0"
+deepdiff = "^7.0.1"
 
 [tool.poetry.group.dev.dependencies]
 bumpver = "^2023.1124"
+pympler = "^1.0.1"
+sortedcontainers = "^2.4.0"
+pandas = "^2.2.2"
+objsize = "^0.7.0"
 
 [build-system]
-requires = ["poetry-core"]
+requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "0.1.3"
+current_version = "1.0.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `rtrie-0.1.3/src/rtrie/array_trie.py` & `rtrie-1.0.0/rtrie/array_trie.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import collections
 from typing import Any
-from .trie import Trie, Node
+from . import Trie, Node
 
 class ArrayTrie(Trie):
     def __init__(self, no_array_for_single_value: bool = False, **kwargs):
         self.no_array_for_single_value = no_array_for_single_value
         super().__init__(**kwargs)
         
     def add_attributes(self, node: Node, value: Any) -> int:
```

### Comparing `rtrie-0.1.3/src/rtrie/stats.py` & `rtrie-1.0.0/rtrie/stats.py`

 * *Files identical despite different names*

### Comparing `rtrie-0.1.3/src/rtrie/trie.py` & `rtrie-1.0.0/rtrie/trie.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-import logging
-import os
-import pickle
-import gc
-from itertools import chain, tee
+from array import array
 from collections import deque
 from collections.abc import MutableMapping
-from array import array
-from typing import Any, Callable, ItemsView, Iterator, Literal, Optional, TypeAlias, cast
-from rapidfuzz import fuzz
+from itertools import chain, tee
+import logging
+from logging import debug, error, info
+import os
+import sys
+from rapidfuzz.fuzz import ratio
 from rapidfuzz.distance.DamerauLevenshtein import distance
-# from rapidfuzz.distance.Levenshtein import distance
+from typing import ItemsView, Iterator, Literal, Optional, cast
+
+from .types import Attributes, Record, Word, Words
+from .node import AttributeNode, Candidates, Children, Node
 
-Word: TypeAlias = str | tuple[str, Any]
-Words: TypeAlias = Iterator[Word]
-Attributes: TypeAlias = Any
-Entry: TypeAlias = tuple[str, 'Node']
-Record: TypeAlias = tuple[str, Attributes]
-Children: TypeAlias = dict[str, 'Node']
-Candidates: TypeAlias = list[tuple[int, str, 'Node']]
+log_level = os.environ.get('LOG_LEVEL') if os.environ.get('LOG_LEVEL') != None else 'ERROR'
+logging.basicConfig(level=logging.getLevelName(log_level), format='%(message)s')
 
 def get_filename(string: str) -> str:
     return "".join([x if x.isalnum() else "_" for x in string])
 
-
 def get_longest_prefix_index(word1: str, word2: str):
     """
         Returns the length of the longest prefix between two words
     """
     if word1 == word2:
         return len(word1)
     max = min(len(word1), len(word2))
@@ -34,15 +30,15 @@
         if word1[i] != word2[i]:
             return i
     return max
 
 
 def get_longest_prefixes_index(words: list[str]):
     """
-        Returns the length of the longest prefix in a sorted list of words
+        Returns the index of the longest prefix in a sorted list of words
     """
     if len(words) == 0:
         return 0
     if len(words) == 1:
         return len(words[0])
 
     # find the first word with a different first character
@@ -57,561 +53,583 @@
     if index - 1 == 0:
         return 0
 
     return get_longest_prefix_index(words[0], words[index - 1])
 
 
 def _get_values(element: Word) -> Record:
+    """
+      Get the value stored in a Node
+    """
     try:
         return (element[0], element[1]) if isinstance(element, tuple) else (element, True)
     except IndexError:
-        print(element[0])
+        error(element[0])
         return ("null", -1)
 
-class Node:
-    # avoid storing class attributes in '__dict__' to save memory
-    __slots__ = ('attributes', 'children')
-
-    def __init__(self, attributes: Attributes = None, children: Optional[Children] = None):
-        self.attributes = attributes
-        self.children = children
-
-    def __str__(self):
-        return self.attributes
-
-    def print(self, depth: int):
-        if self.children == None:
-            return ""
-        offset = "\t"*depth
-        string = ""
-        for item in self.children.items():
-            key: str = item[0]
-            child: Node = item[1]
-            string += "\n" + offset + "\t" + \
-                f"{key}({child.attributes}): {child.print(depth+1)}"
-        return string
-
 class Trie(MutableMapping[str, Attributes]):
+    # It appears we need to use slots here... for some reason it will always have
+    # slots even if it's not defined in the class, so without it doing memory
+    # profiling will fail
+    __slots__ = ('root', 'num_words', 'node_factory')
+
     def __init__(self, 
-                 root: Node | None=None, 
-                 depth_to_store: Optional[int]=None, 
-                 words: Optional[Words] = None, 
-                 subtrie_path: str='./subtrie'):
+      root: AttributeNode | None=None, 
+      words: Optional[Words] = None,
+      node_type: AttributeNode = AttributeNode
+    ):
         """
             Initialize a Trie.
 
-            NOTE: `words` must be either a list of strings or a list of tuples of the form (word: str, attributes: Any). If `words` is a list of
+            NOTE: `words` must be either a iterable of strings or a iterable of tuples of the form (word: str, attributes: Any). If `words` is a iterable of
             strings, the `attributes` property will be set to `True` for each word.
 
             You can pass in a custom add function that is used to control how attributes are defined. This can be useful if you need
             special cases for when words conflict or requiring merging of attributes, i.e. if `attributes` is an object and you add
             a word that already exists with other attributes, you may want to overwrite, merge, etc. The default is to simply assign
             the value `True`, indicating it is a word, and adding the same word again will not affect the trie.
-
-            NOTE: if you supply custom add_word and delete_word functions, they MUST manage the `num_words` property if you want `len(trie)` to report the correct value.
         """
 
-        self.root = root if root != None else Node()
+        self.node_factory = node_type
         self.num_words: int = 0
-        self.depth_to_store = depth_to_store
-        self.subtrie_path = subtrie_path
-        if self.depth_to_store != None:
-            os.mkdir(self.subtrie_path)
+        self.root = root if root != None else self.node_factory()
+
         if words:
             self.add_words(words)
 
     def __delitem__(self, word: str):
-        return self.delete(word)
+        return self.remove(word)
 
     def __getitem__(self, word: str) -> Record | None:
-        result = self._get_node(word)
-        if result != None and result[0][1].attributes != None:
-            return (result[0][0], result[0][1].attributes)
-        return None
+        path, label = self._get_node(word)
+        node = path.pop()[0] if len(path) > 0 else None
+        if label == word and node != None and node.is_word():
+            return (label, node.attributes)
+        raise KeyError(word)
 
     def __setitem__(self, word: str, attributes: Attributes) -> None:
-        result = self._get_node(word)
-        if result != None:
-            result[0][1].attributes = attributes
+        self.add(word, attributes)
 
     def __str__(self):
         return self.root.print(0)
 
     def __len__(self):
         return self.num_words
 
     def __contains__(self, word: object) -> bool:
-        result = self._get_node(cast(str, word))
-        return result != None and result[0][1].attributes != None
+        path, label = self._get_node(cast(str, word))
+        return label == word and (path[-1][0].is_word() if path != None and len(path) > 0 else False)
 
     def __iter__(self):
         return self.words()
-
-    def add_attributes(self, node: Node, value: Attributes) -> int:
+    
+    def post_add_node(self, **kwargs):
         """
-          The default add method to use when one isn't provided. It uses True/None to indicate whether a node is a word or not
+        Used to hook into the add method to perform additional operations after a node is added.
+        By default it's a no-op.
         """
-        # if this is a new word, increment the number of words
-        # otherwise we are just overwriting attributes which isn't a new word
-        is_new = 1
-        if node.attributes != None:
-            is_new = 0
-        node.attributes = value
-        return is_new
-
-    def delete_attributes(self, node: Node) -> int:
-        node.attributes = None
-        return -1
-
-    def count_attributes(self, node: Node) -> int:
-        return 1
+        info(f"Post add node: {kwargs}")
 
     def add(self, word: str, attributes: Attributes=True):
         """
-          Adds a single word to an already constructed Trie. You should use `add_words` to initialize a Trie for performance reasons
+        Adds a single word. 
+        NOTE: You should use `add_words` to initialize a Trie for performance reasons
         """
-        current: Node = self.root
+        current: AttributeNode = self.root
+        word = sys.intern(word)
 
         while True:
-            logging.debug(f'Adding "{word}"')
+            debug(f'Adding "{word}"')
 
             if current.children == None:
-                logging.debug("No children, initializing")
+                debug("No children, initializing")
                 current.children = cast(Children, {})
 
-            logging.debug(str(current.children.keys()))
+            debug(str(current.children.keys()))
 
             if len(current.children.keys()) == 0:
-                logging.debug(
+                debug(
                     f'Empty children, adding "{word}" with `attributes = {attributes}')
-                current.children[word] = Node()
-                self.num_words += self.add_attributes(current.children[word], attributes)
+                current.children[word] = self.node_factory()
+                self.num_words += current.children[word].add_attributes(attributes)
                 break
 
             elif word in current.children.keys():
-                logging.debug(
+                debug(
                     f'"{word}" already exists, adding attributes {attributes}')
-                self.num_words += self.add_attributes(current.children[word], attributes)
+                self.num_words += current.children[word].add_attributes(attributes)
                 break
 
             else:
                 match_found = False
-                logging.debug("No exact match, checking remaining keys...")
+                debug("No exact match, checking remaining keys...")
                 for key in list(current.children.keys()):
-                    index: int = get_longest_prefix_index(key, word)
-                    logging.debug(f"Prefix location: {index}")
+                    key = sys.intern(key)
+                    index = get_longest_prefix_index(key, word)
+                    debug(f"Prefix location: {index}")
 
                     if index == 0:
-                        logging.debug(
+                        debug(
                             f'"{key}" has no overlapping prefix, continuing...')
                         continue
 
                     else:
                         match_found = True
                         prefix = word[:index]
+                        prefix = sys.intern(prefix)
                         word_suffix = word[index:]
                         key_suffix = key[index:]
+                        key_suffix = sys.intern(key_suffix)
 
-                        logging.debug(
+                        debug(
                             f"\nPrefix: {prefix}\nWord remainder: {word_suffix}\nKey remainder: {key_suffix}")
 
                         if len(key_suffix) == 0:
-                            logging.debug("Moving")
+                            debug("Moving")
                             current = current.children[prefix]
                             word = word[index:]
                             break
 
                         else:
-                            logging.debug(f'Creating new node "{key_suffix}"')
+                            debug(f'Creating new node "{key_suffix}"')
                             is_word = len(prefix) == len(word)
-                            logging.debug(
+                            debug(
                                 f'Creating new node "{prefix}", is it a word: {is_word}')
-                            current.children[prefix] = Node(None, Children())
-                            self.num_words += self.add_attributes(
-                                current.children[prefix], attributes if is_word else None)
+                            current.children[prefix] = self.node_factory(None, Children())
+                            if is_word:
+                                self.num_words += current.children[prefix].add_attributes(attributes)
                             
                             # we know this is set to empty dict from above
                             current.children[prefix].children[key_suffix] = current.children[key] # type: ignore
-                            logging.debug(f'Deleting old node "{key}"')
+                            debug(f'Deleting old node "{key}"')
                             del current.children[key]
 
                         if len(word_suffix) > 0:
-                            logging.debug("Iterate to add word remainder")
+                            debug("Iterate to add word remainder")
                             current = current.children[prefix]
                             word = word[index:]
 
                         break
 
                 if not match_found:
-                    logging.debug(
+                    debug(
                         f'No overlapping prefixes in any key, adding "{word}" with `attributes` = {attributes}')
                     if current.children != None:
-                        current.children[word] = Node()
-                        self.num_words += self.add_attributes(
-                            current.children[word], attributes)
+                        word = sys.intern(word)
+                        current.children[word] = self.node_factory()
+                        self.num_words += current.children[word].add_attributes(attributes)
                     break
 
-    def delete(self, word: str):
-        prev: Node | None = None
-        current = self.root
-
-        while current != None:
-            if word in current.children:
-                # handle node shifts
-
-                self.delete_attributes(node)
-                return
-
-            for i in range(0, len(word)):
-                w = word[:i]
-                if w in node.children:
-                    logging.debug(f"Prefix: {prefix}, Word: {word}")
-                    prev = current
-                    current = current.children[w]
-
-    def add_words(self, words: Words):
+    def _restructure(self, node: Node, parents: list[Node]) -> None:
+        """
+        Ascends the Trie to restructure it after a node is deleted.
+        This should NOT be called directly, but rather through `delete` or `delete_attributes`
         """
-            This function is to speed up initialzing a Trie by using a sorted collection of words.
-            It also allows for storing subtries to a file based on a desired depth while building, allowing you
-            to build very large tries without consuming too much memory. This is a trade-off for speed for lookups and number of files
-            (greater depth, more files, but faster loading of subtries on disk), however can create more files, so only use
-            if necessary.
+        children = node.children
+        (prev, key) = parents.pop() if len(parents) > 0 else (None, None)  
+        debug(f"Restructuring node: {node}, prev: {prev}, key: {key}")    
+
+        # if the node is None, is a word, or has multiple children, nothing to do
+        if node == None or node.attributes != None or (children != None and len(children) > 1):
+            debug('Node is None, a word, or has multiple children, returning')
+            return
+        else:
+            if children == None or len(children) == 0:
+                if prev != None:
+                    debug('Deleting node')
+                    debug(f"Prev: {prev}, key: {key}")
+                    prev.children.pop(key)
+                    debug(prev)
+            else: 
+                # len(children) == 1, so just pop the only item
+                child_key, child_node = children.popitem()
+                if prev != None:
+                    debug('Merging node with child')
+                    debug(key + child_key)
+                    new_key = key + child_key
+                    new_key = sys.intern(new_key)
+                    prev.children[new_key] = child_node
+                    prev.children.pop(key)
+
+        if prev != self.root:
+            self._restructure(prev, parents)
+
+    def remove(self, word: str) -> bool:
+        """
+        Deletes a word from the Trie
+        """
+        path, label = self._get_node(word)
+        node = path.pop()[0] if len(path) > 0 else None
+        if label == word and node != None and node.is_word():
+            self.num_words -= 1
+            node.attributes = None
+            self._restructure(node, path)
+        else:
+            return False
+        return True
 
-            NOTE: the words passed in MUST be in lexigraphically sorted order, or else the output will not be correct
+    def delete_attributes(self, word: str, attributes: Attributes) -> int:
         """
-        self._add_words_recursive(words, self.root, 0, 0)
+        Deletes a specific attribute from a word. Deleting an attribute does not necessarily 
+        delete the word from the Trie, but to keep the Trie correct, it will delete the node
+        if it has no remaining attributes
+        """
+        result = self._get_node(word)
+        deleted = False
+        if result != None and result.node != None:
+            deleted = result.node.delete_attributes(attributes)
+        if deleted:
+            self.num_words -= 1
+        self._restructure(result.node, result.parents) # will restructure Trie if needed
+        return deleted
 
     def get_matching_prefixes(self, words: Words, offset: int) -> tuple[list[Word], Optional[Word]]:
         """
             Returns a list of words that have at least their first character in 
             common, and the first non-matching one so we can add it back into the generator
         """
-        logging.debug(">> get_matching_prefixes")
-        logging.debug(f"Offset: {offset}")
-        if logging.getLogger().level == logging.DEBUG:
-            words_copy = tee(words)
-            logging.debug(f"Words: {list(words_copy)}")
+        debug(">> get_matching_prefixes")
+        debug(f"Offset: {offset}")
+        if logging.getLogger().level == debug:
+            words_copy = tee(words) # need to tee it since it's a iterator
+            debug(f"Words: {list(words_copy)}")
         matches: list[Word] = []
         first = next(words, None)
-        logging.debug(f"First: {first}")
+        debug(f"First: {first}")
         if first == None:
             return (matches, None)
 
         matches.append(first)
         first_label = _get_values(first)[0]
-        logging.debug(f"First label: {first_label}")
+        debug(f"First label: {first_label}")
         first_label = first_label[offset:]
 
         # TODO: compare with takewhile
         current = next(words, None)
         while current != None:
             current_label = _get_values(current)[0]
-            logging.debug(f"Current label: {current_label}")
+            debug(f"Current label: {current_label}")
             current_label = current_label[offset:]
-            logging.debug(first_label)
-            logging.debug(current_label)
+            debug(first_label)
+            debug(current_label)
             try:
                 if first_label[0] == current_label[0]:
-                    logging.debug("Matching prefix")
+                    debug("Matching prefix")
                     matches.append(current)
                     current = next(words, None)
                 else:
-                    logging.debug("No matching prefix")
+                    debug("No matching prefix")
                     break
             except IndexError:
-                # TODO: fix this, it seems to be when a following word is shorted than the first?
-                logging.warn(current)
+                # TODO: fix this, it seems to be when a following word is shorter than the first?
+                logging.warn(first_label, current)
                 current = next(words, None)
 
-        logging.debug(f"Matches: {matches}, last: {current}")
-        logging.debug("<< get_matching_prefixes")
+        debug(f"Matches: {matches}, last: {current}")
+        debug("<< get_matching_prefixes")
         # return it as a list so we can use len() on it
         return (matches, current)
+    
+    def add_words(self, words: Words):
+        """
+            This function is to speed up initialzing a Trie by using a sorted iterable of words.
+
+            NOTE: the words passed in MUST be in lexigraphically sorted order, or else the output will not be correct
+        """
+        self._add_words_recursive(words, self.root, 0, 0)
 
-    def _add_words_recursive(self, words: Words, current: Node, offset: int, depth: int):
+    def _add_words_recursive(self, words: Words, current: AttributeNode, offset: int, depth: int):
         """
-          Pure recursive method for adding list of sorted words.
+          Pure recursive method for adding sorted list of words.
 
           `words` must be an iterator so that `next` is available
 
-          TODO: could create subtries in parallel to speed it up
+          TODO: since it's in sorted order, potentially could create subtries in parallel to speed it up since each
+          prefix will not be visited again, but we'd need to be careful about num_words
         """
 
         while 1:
             # `matches` will contain all words with at least one matching prefix
             # `last` contains the first 'peeked' word which didn't match
             matches, last = self.get_matching_prefixes(words, offset)
 
             # base case
             if len(matches) == 0:
-                logging.debug("No matches - base case")
+                debug("No matches - base case")
                 return
 
-            # handle the matches, then continue where it left off
             words = cast(Words, chain([last], words))
+
             if (current.children == None):
                 current.children = {}
 
             first_label, first_attributes = _get_values(matches[0])
             first_label_copy = first_label
             first_label = first_label[offset:]
+            first_label = sys.intern(first_label)
 
             # matching case, add to Trie
             if len(matches) == 1:
-                logging.debug("Single match - normal case")
-                logging.debug(
+                debug("Single match - normal case")
+                debug(
                     f"Adding word {first_label} with attributes {first_attributes}")
-                current.children[first_label] = Node()
-                self.num_words += self.add_attributes(
-                    current.children[first_label], first_attributes)
+                current.children[first_label] = self.node_factory()
+                self.num_words += current.children[first_label].add_attributes(first_attributes)
+                self.post_add_node(node = current, label = first_label_copy, prefix = '', depth = depth)
                 if last == None:
                     return
                 continue
 
             # recursive case
             else:
-                logging.debug("Multiple matches")
+                debug("Multiple matches")
 
+                # test if they are all the same word
                 # since it's a sorted list, we can do this by comparing the first
                 # and last words
                 last_label = _get_values(matches[-1])[0]
                 last_label = last_label[offset:]
-                logging.debug(f"{first_label} vs {last_label}")
+                debug(f"{first_label} vs {last_label}")
                 prefix_length = get_longest_prefix_index(
                     first_label, last_label)
                 prefix = first_label[:prefix_length]
-                logging.debug(f"Prefix: {prefix} ({prefix_length})")
+                prefix = sys.intern(prefix)
+                debug(f"Prefix: {prefix} ({prefix_length})")
 
                 # create a node for the longest matching prefix...
                 # the next step decides if it's a word or not
-                current.children[prefix] = Node()
+                current.children[prefix] = self.node_factory()
 
                 matches = iter(matches)
 
                 # if the length of the longest prefix is the same as the first word, it's a word
                 if (prefix_length == len(first_label)):
-                    logging.debug("Prefix is the first word")
+                    debug("Prefix is the first word")
 
-                    # there could be multiple instances of the word, so keep adding all matching ones
+                    # there could be multiple instances of the word with different attributes, 
+                    # so keep adding them all
                     word = next(matches, None)
                     while word != None:
                         label, attributes = _get_values(word)
                         if label[offset:] != prefix:
                             break
-                        logging.debug(
+                        debug(
                             f"Adding word {label} with attributes {attributes}")
-                        self.num_words += self.add_attributes(
-                            current.children[prefix], attributes)
+                        self.num_words += current.children[prefix].add_attributes(attributes)
                         word = next(matches, None)
 
+                    # if it's the end of the iter we're done
                     if word != None:
                         matches = chain([word], matches)
 
                 # otherwise, it's just a node
                 else:
-                    logging.debug("Prefix is not a word, just recurse")
+                    debug("Prefix is not a word")
 
-                logging.debug("Recursing...")
+                debug("Recursing...")
                 self._add_words_recursive(
                     matches, current.children[prefix], offset + prefix_length, depth + 1)
-
-                # dump to storage if specified
-                if (self.depth_to_store != None and depth == self.depth_to_store):
-                    filename = get_filename(first_label_copy)
-                    logging.info(
-                        f"Moving trie at '{first_label}' as '{filename}' to file")
-                    # TODO: investigate mmap instead of pickling
-                    with open(f"{self.subtrie_path}/{filename}.pickle", 'wb') as file:
-                        pickle.dump(current, file)
-                    # cleanup memory
-                    del current.children[prefix]
-                    gc.collect()
-
+                self.post_add_node(node = current, label = first_label_copy[:offset + prefix_length], prefix = prefix, depth = depth)
+  
             if last == None:
                 break
+            
+        info(f"Finished adding words at depth {depth}")  
 
-        logging.debug("End")
 
-    def words(self, sort: bool =False) -> Iterator[str]:
+    def words(self, sort = False) -> Iterator[str]:
         """
         Returns all nodes that are words
         """
-        for prefix, node in self.nodes(sort):
+        for prefix, node in self.nodes(sort = sort):
             if (node.attributes != None):
                 yield prefix
 
-    def nodes(self, sort: bool = False) -> Iterator[Record]:
-        prefix = ""
-        stack: deque[Entry] = deque()
-        if self.root.children != None:
-            items = self.root.children.items()
-            if sort:
-                items = reversed(sorted(items))
-            for item in items:
-                stack.append(item)
-
-        while stack:
-            prefix, node = stack.pop()
-
-            yield (prefix, node)
-
-            if node.children != None:
-                items = node.children.items()
-                if sort:
-                    items = reversed(sorted(items))
-                for key, value in items:
-                    stack.append((prefix + key, value))
+    def nodes(self, sort=False) -> Iterator[Record]:
+        """
+        BF traversal of the Trie, optionally in sorted order
+        """
+        return self.root.nodes(sort = sort)
 
-    def _get_node(self, word: str) -> tuple[Record, Node | None] | None:
-        return self._get_node_recursive(self.root, None, word, "")
+    def _get_node(self, word: str) -> list[tuple[Node, str]]:
+        """
+        Returns the stack of Node/key pairs that leads to a node with a potentially matching label.
+        The top of the stack will either be a match or the closest node that matches the prefix.
+        """
+        return self._get_node_recursive(self.root, word, "", path=[])
 
-    def _get_node_recursive(self, node: Node, previous_node: Optional[Node], word: str, prefix: str) -> Optional[tuple[Entry, Optional[Node]]]:
+    def _get_node_recursive(self, node: Node, remainder: str, prefix: str, path: list[tuple[Node, str]]) -> list[tuple[Node, str]]:
         if node.children != None:
-            if (word in node.children):
-                return ((prefix + word, node.children[word]), previous_node)
+            if (remainder in node.children):
+                path.append((node, remainder))
+                path.append((node.children[remainder], None))
+                return (path, prefix + remainder)
 
             # try seeing if there's a node with a matching prefix starting from shortest to longest
-            for i in range(0, len(word)):
-                w = word[:i]
-                if w in node.children:
-                    logging.debug(f"Prefix: {prefix}, Word: {word}")
-                    return self._get_node_recursive(node.children[w], node, word[i:], prefix + w)
+            for i in range(0, len(remainder)):
+                key = remainder[:i]
+                if key in node.children:
+                    debug(f"Prefix: {prefix}, remainder: {remainder}, key: {key}")
+                    path.append((node, key))
+                    return self._get_node_recursive(node.children[key], remainder[i:], prefix + key, path)
 
-            return None
-        return None
+        return (path, prefix)
 
-    # TODO: this returns a generator which technically isn't correct
+    # TODO: this returns a generator which technically isn't correct for a MultipleMap, but works for most cases
     def items(self) -> ItemsView[str, Attributes]:
         """
-            Method to make it interoperable with dict, where keys are the words, and values are the attributes
+        Method to make it interoperable with dict, where keys are the words, and values are the attributes
         """
-        
-        for prefix, node in self.nodes():
-            if (node.attributes != None):
-                yield (prefix, node.attributes) # type: ignore
+        return self.root.items()
 
-    def search1(self, word, threshold):
-        candidates = []
-
-        stack = deque()
-        if self.root.children != None:
-            for key, node in self.root.children.items():
-                stack.append((key, node))
-
-        while stack:
-            prefix, node = stack.pop()
-            similarity = fuzz.ratio(word[:len(prefix)], prefix)
-            # logging.debug(f"{word[:len(prefix)]} <> {prefix}: {similarity}")
-            if similarity >= threshold:
-                if node.attributes != None:
-                    candidates.append((similarity, prefix, node))
-
-                if node.children != None:
-                    for key, value in reversed(sorted(node.children.items())):
-                        stack.append((prefix + key, value))
-
-        return candidates
-
-    def search(self, word, type: Literal['fuzzy', 'edit'] = 'edit', max_distance: int = 0) -> Candidates:
-
-        # Pruning phase
+    def starts_with(self, prefix: str) -> Iterator[str]:
+        """
+        Returns a generator consisting of all nodes that are longer than the nearest node matching `prefix`.
+        """
+        if prefix == "":
+            return self.root.items()
+        path, label = self._get_node(prefix)
+        node = path.pop()[0] if len(path) > 0 else None
+        if node == None:
+            return chain(*[child.items(prefix = key, include_root = True) for key, child in self.root.children.items() if key.startswith(prefix)])
+                
+        else:
+            return node.items(prefix = label, include_root = True)
+        
+    def prefixes_of(self, string: str) -> str:
+        """
+        Returns all words that are a prefix of a given string.
+        """
+        path, label = self._get_node(string)
+        prefixes = []
+        prefix = ""
+        for node, key in path:
+            if key != None:
+                prefix += key
+                child = node.children[key]
+                if child.is_word():
+                    prefixes.append((prefix, child.attributes))
+        return prefixes
+    
+    def similar_to(self, word, type = 'ratio', max_distance = None, threshold = None):
+        if type == 'ratio':
+            if threshold == None:
+                raise ValueError("threshold must be provided when type is 'ratio'")
+        elif type == 'distance':
+            if max_distance == None:
+                raise ValueError("max_distance must be provided when type is 'distance'")
+            self.edit_distance(word, max_distance)
+
+    def edit_distance(self, word: str, max_distance: int) -> Candidates:
+        """
+        Returns a list of words with an edit distance of at most `max_distance` from `word`.
+
+        NOTE: this is a somewhat naive approach. We still get to skip a lot of nodes, but
+        for the ones that are within the range of len(word) +- max_distance, we are computing 
+        the distance for each word. 
+        We could perhaps do a running distance approach and/or memoize the values we've already 
+        computed to speed this up (see commented out below for a nearly working example)
+        """
+        word_length = len(word)
+        queue = deque([("", self.root)])
         candidates = []
-        offset = 0
-        distance = 0
+        
+        while queue:
+            prefix, child = queue.popleft()
+            if len(prefix) > word_length + max_distance:
+                debug('too long, done')
+                continue
+            elif len(prefix) < word_length - max_distance:
+                debug('too short, next')
+            else:
+                if child.is_word():
+                    debug(f'Checking word: {prefix}')
+                    d = distance(word, prefix)
+                    if d <= max_distance:
+                        debug(f'Adding word: {prefix}, Distance: {d}')
+                        candidates.append((d, prefix, child.attributes))
 
-        if type == 'edit':
-          self._search_edit_recursive(self.root, word, "", offset, distance, max_distance, candidates)
-        else:
-          print('TODO: fuzzy')
+            for k, c in child.children.items() if child.children != None else {}:
+                queue.append((prefix + k, c))
 
         return candidates
 
+    # def edit_distance(self, word: str, max_distance: int) -> Candidates:
+    #     """
+    #     Returns a list of words with an edit distance of at most `max_distance` from `word`.
+    #     """
+    #     nodes = []
+    #     self._edit_distance_recursive(self.root, word, "", max_distance, 0, 0, nodes)
+    #     return nodes
+    
+    # def _edit_distance_recursive(self, node, word, prefix, max_distance, total_distance, length, candidates):
+    #     word_length = len(word)
+    #     print(total_distance, max_distance, node.children.keys() if node.children != None else {})
+    #     for key, child in node.children.items() if node.children != None else {}:
+    #         key_length = len(key)
+    #         p = word[:key_length]
+    #         s = word[key_length:]
+    #         d = total_distance + distance(p, key)
+    #         l = length + key_length
+    #         print(f'Word: {word}, Prefix: {p}, Key: {key}, Distance: {d}, Length: {l}')
+
+    #         # need to handle both when we can directly compare the word and key, and when we need
+    #         # to check deeper in the trie for deletions/swaps
+    #         if total_distance <= max_distance:
+    #             if child.is_word() and max_distance >= d + len(s):
+    #                 candidates.append((d, prefix + key, child.attributes))
+    #             self._edit_distance_recursive(child, s, prefix + key, max_distance, d, l, candidates)
+
+    #         # check deeper nodes without consuming the word
+    #         if l <= max_distance:
+    #             self._edit_distance_recursive(child, word, prefix + key, max_distance, d, l, candidates)
 
-        # stack = deque()
-        # if self.root.children != None:
-        #     for key, node in self.root.children.items():
-        #         stack.append((key, node))
-
-        # while stack:
-        #     prefix, node = stack.pop()
-        #     prefix_length = len(prefix)
-        #     word_fragment = word[offset:prefix_length]
-
-        #     logging.debug(f"Prefix: {prefix}, Word: {word_fragment}")
-        #     score = distance(word_fragment, prefix)
-        #     logging.debug(f"Distance: {score}")
-
-        #     if score < max_distance:
-                
-
-        #     # prefix = word[:prefix_length]
-        #     logging.debug(f"Comparing {prefix} to {word}")
-        #     previous_row = array('b', range(prefix_length + 1))
-        #     for i in range(len(prefix) - 1):
-        #         current_row = array('b', range(prefix_length + 1))
-        #         current_row[0] = i + 1
-        #         for j in range(prefix_length - 1):
-        #             deletion_cost = previous_row[j + 1] + 1
-        #             insertion_cost = current_row[j] + 1
-        #             substitution_cost = previous_row[j] if word[i] == prefix[j] else previous_row[j] + 1
-        #             current_row[j + 1] = min(deletion_cost,
-        #                                      insertion_cost, substitution_cost)
-
-        #         previous_row = current_row
-
-        #     distance = previous_row[prefix_length - 1]
-        #     logging.debug(f"Distance: {distance}")
-        #     if previous_row[prefix_length - 1] < max_distance:
-        #         if node.children != None:
-        #             for key, value in node.children.items():
-        #                 stack.append((prefix + key, value))
-
-        # return candidates
-
-    def _search_edit_recursive(self, node: Node, word: str, prefix: str, offset: int, current_distance: int, max_distance: int, candidates: Candidates) -> Candidates:
+    def _search_fuzzy_recursive(self, node: AttributeNode, word: str, prefix: str, offset: int, current_distance: int, threshold: float, candidates: Candidates) -> Candidates:
         if node == None or node.children == None or len(node.children) == 0:
-          return
-
-
-
+            return
+        
+        # TODO: investigate if doing a running similarity is faster than skipping early ones
+        
+        for child in node.children:
+            new_prefix = f"{prefix}{child}"
 
-        # TODO: see if we can improve on this, since right now we're doing a lookup for each word and we could be doing lookup
-        # of each fragment of the word that lines up with key
+            min_sim = abs((len(new_prefix) - len(word)) / len(word))
 
-        for child in node.children:
-            fragment = word[offset:offset+len(child)]
-            d = distance(fragment, child)
+            # if theres' too many letters difference, there will be no more matches
+            if min_sim > threshold:
+                return
+            
+            # if there's not enough letters, we still need to recurse to check them
+            elif min_sim < 0:
+                self._search_fuzzy_recursive(child_node, word, new_prefix, offset + len(child), None, threshold, candidates)  
 
-            # we want to be able to tell if the key has 0 difference
-            total = d + current_distance
-            logging.debug(f"Distance b/w {child} and {fragment}: {d}")
-            logging.debug(f"{current_distance} + {d} = {total}")
-            if total <= max_distance:
-                child_node = node.children[child]
-                new_prefix = prefix + child
-                logging.debug(f"{word}, {new_prefix}, {distance(word, prefix)}")
-                if child_node.attributes != None:
-                    total_distance = distance(word, new_prefix)
-                    if total_distance <= max_distance:
-                        candidates.append((total_distance, child_node))
-                self._search_edit_recursive(child_node, word, new_prefix, offset + len(child), total, max_distance, candidates)
+            # within the length range where you could have similarities, need to compare.
+            # NOTE: even if a word is too short, 
+            else:
+              r = ratio(word, new_prefix)
+              debug(f"Search word: {word}, Prefix: {new_prefix}, Ratio: {r}")
+              if r >= threshold:
+                  child_node = node.children[child]
+                  if child_node.attributes != None:
+                      candidates.append((r, new_prefix, child_node))
+                  self._search_fuzzy_recursive(child_node, word, new_prefix, offset + len(child), None, threshold, candidates)  
 
     def stats(self, unique: bool = True):
         average_length: int = 0
         word_lengths: dict[int, int] = {}
         letter_frequency: dict[str, int] = {}
         letter_distribution: dict[str, dict[int, int]] = {}
         num_nodes: int = 0
         node_distribution: dict[int, int] = {}
         lengths_at_node_depths: dict[int, dict[int, int]] = {}
         depth: int = 0
 
         # initialize the stack
         prefix = ""
-        stack: deque[tuple[str, Node, int]] = deque()
+        stack: deque[tuple[str, AttributeNode, int]] = deque()
         if self.root.children != None:
             items = self.root.children.items()
             node_distribution[1] = len(items)
             for key, value in self.root.children.items():
                 stack.append((key, value, 1))
 
         while stack:
@@ -641,16 +659,15 @@
                     letter_distribution[letter] = letter_distribution.get(
                         letter, {})
                     letter_distribution[letter][index] = letter_distribution[letter].get(
                         index, 0) + count
 
             if node.children != None:
                 items = node.children.items()
-                node_distribution[depth +
-                                  1] = node_distribution.get(depth + 1, 0) + len(items)
+                node_distribution[depth + 1] = node_distribution.get(depth + 1, 0) + len(items)
                 for key, value in items:
                     stack.append((prefix + key, value, depth + 1))
 
         return {
             'num_words': self.num_words,
             'average_length': average_length / self.num_words,
             'word_lengths': word_lengths,
@@ -671,8 +688,8 @@
             deletion_cost = previous_row[j + 1] + 1
             insertion_cost = current_row[j] + 1
             substitution_cost = previous_row[j] if word1[i] == word2[j] else previous_row[j] + 1
             current_row[j + 1] = min(deletion_cost,
                                      insertion_cost, substitution_cost)
 
         previous_row = current_row
-    return previous_row[length - 1]
+    return previous_row[length - 1]
```

