# Comparing `tmp/ofnodes-1.6.0.tar.gz` & `tmp/ofnodes-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofnodes-1.6.0.tar", max compression
+gzip compressed data, was "ofnodes-1.6.1.tar", max compression
```

## Comparing `ofnodes-1.6.0.tar` & `ofnodes-1.6.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-1.6.0/LICENSE
--rw-r--r--   0        0        0     2606 2024-04-05 21:55:30.417310 ofnodes-1.6.0/README.md
--rw-r--r--   0        0        0      590 2024-04-18 20:15:49.132482 ofnodes-1.6.0/pyproject.toml
--rw-r--r--   0        0        0      953 2024-04-05 16:17:48.873936 ofnodes-1.6.0/src/ofnodes/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.6.0/src/ofnodes/nodes/__init__.py
--rw-r--r--   0        0        0     2479 2024-04-17 16:06:36.566198 ofnodes-1.6.0/src/ofnodes/nodes/singlynode.py
--rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.6.0/src/ofnodes/py.typed
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.6.0/src/ofnodes/structures/__init__.py
--rw-r--r--   0        0        0    26514 2024-04-18 20:15:49.132482 ofnodes-1.6.0/src/ofnodes/structures/singlylinkedlist.py
--rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 ofnodes-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-1.6.1/LICENSE
+-rw-r--r--   0        0        0     2606 2024-04-05 21:55:30.417310 ofnodes-1.6.1/README.md
+-rw-r--r--   0        0        0      590 2024-04-20 03:24:00.640697 ofnodes-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0      953 2024-04-05 16:17:48.873936 ofnodes-1.6.1/src/ofnodes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.6.1/src/ofnodes/nodes/__init__.py
+-rw-r--r--   0        0        0     2820 2024-04-20 03:24:00.640697 ofnodes-1.6.1/src/ofnodes/nodes/singlynode.py
+-rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.6.1/src/ofnodes/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.6.1/src/ofnodes/structures/__init__.py
+-rw-r--r--   0        0        0    28576 2024-04-20 03:24:00.640697 ofnodes-1.6.1/src/ofnodes/structures/singlylinkedlist.py
+-rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 ofnodes-1.6.1/PKG-INFO
```

### Comparing `ofnodes-1.6.0/LICENSE` & `ofnodes-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ofnodes-1.6.0/README.md` & `ofnodes-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ofnodes-1.6.0/pyproject.toml` & `ofnodes-1.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofnodes"
-version = "1.6.0"
+version = "1.6.1"
 description = "A library of Data Structures and Algorithms written in Python"
 authors = ["Robert Portelli <github@robertportelli.com>"]
 readme = "README.md"
 packages = [{include = "ofnodes", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `ofnodes-1.6.0/src/ofnodes/__init__.py` & `ofnodes-1.6.1/src/ofnodes/__init__.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.6.0/src/ofnodes/nodes/singlynode.py` & `ofnodes-1.6.1/src/ofnodes/nodes/singlynode.py`

 * *Files 20% similar despite different names*

```diff
@@ -54,14 +54,21 @@
         """
         raise AttributeError(
             f"{type(self).__name__}'s `data` attribute " "cannot be deleted."
         )
 
     @property
     def next(self):
+        """Getter property for the next node in the singly linked list.
+
+        Note:
+            This property allows access to the next node in the linked list. Modifying
+            the next node should be done using linked list methods for consistency and
+            to maintain the integrity of the linked list structure.
+        """
         return self._next
 
     @next.setter
     def next(self, value):
         raise AttributeError("Cannot set 'next' attribute directly. Use linked list methods for modification.")
 
     @next.deleter
```

### Comparing `ofnodes-1.6.0/src/ofnodes/structures/singlylinkedlist.py` & `ofnodes-1.6.1/src/ofnodes/structures/singlylinkedlist.py`

 * *Files 4% similar despite different names*

```diff
@@ -350,62 +350,120 @@
             (SinglyNode(data='1 node'), SinglyNode(data='2 node'), SinglyNode(data='4 node'))
             >>> llist.tail = "is passed to setter to become SinglyNode()"
             >>> llist.head, llist.head.next, llist.tail
             (SinglyNode(data='1 node'), SinglyNode(data='2 node'), SinglyNode(data='is passed to setter to become SinglyNode()'))
         """
         self.tail = data  # trigger the tail setter
 
-    def insert_after_target(self, target_data: Any, data_to_insert: Any) -> None:
+    def insert_after_target(self, target_data: Any, data_to_insert: Any) -> bool:
         """
-        steps:
-        1) the target data is validated
-        2) the head data is checked for the target
-            - if True, the linked list is checked if it's a one node list
-                - if True, simply use the tail property to insert after the head
-                - if False, the list contains more than one node
-        3) the tail data is checked for the target
-            - if True, simply use
+        Inserts a new node containing the specified data after the first occurrence
+        of the target data in the linked list.
+
+        Args:
+            target_data (Any): The data value to search for in the linked list.
+            data_to_insert (Any): The data value to insert after the target data.
+
+        Returns:
+            bool: True if the insertion was successful, False otherwise.
+
+        Raises:
+            ValueError: If the target data is not found in the linked list.
+
+        Note:
+            This method triggers the setter for the target data attribute.
+            If the target data is found at the head of the linked list and the list
+            contains only one node, the new node becomes the new tail of the list.
+            Otherwise, the method traverses the list to find the target data and inserts
+            the new node immediately after it. If the target data is found at the tail,
+            the new node becomes the new tail of the list.
         """
-        self.target = target_data  # trigger the setter
-        # insert after the first encounter
-        if getattr(self._head, 'data') == self._target:
+        try:
+            self.target = target_data  # trigger the setter
+        except ValueError:
+            return False
+        # check head and if it's a one node list
+        if self._head and self._head.data == self._target:
             if self._head is self._tail:  # it's a one node list
                 self.tail = data_to_insert  # trigger the setter, tail property will validate input
-                return
-        current_node = getattr(self, '_head')  # traversal
-        while current_node is not self._tail:  # traversal
+                return True
+
+        # check each node in the list from head until, but not including, the tail
+        current_node = self._head
+        while current_node and current_node is not self._tail:  # traversal
             if current_node.data == self._target:
                 new_node = SinglyNode(data_to_insert)  # SinglyNode() will validate input
                 setattr(new_node, '_next', current_node.next)  # insert after()
                 setattr(current_node, '_next', new_node)  # insert after()
-                return
+                return True
             current_node = current_node.next  # traversal
+        # check tail
         if getattr(self._tail, 'data') == self.target:
             self.tail = data_to_insert  # # trigger the setter, tail property will validate input
+            return True
+        # no target match
+        return False
+
+    def insert_before_target(self, target_data: Any, data_to_insert: Any) -> bool:
+        """
+        Inserts a new node containing the specified data before the first occurrence
+        of the target data in the linked list.
+
+        Args:
+            target_data: The data value to search for in the linked list or the reference to the node.
+            data_to_insert: The data value to insert before the target data.
 
-    def insert_before_target(self, target_data, data_to_insert):
-        """The traversal doesn't have to account for head or tail because
-        each is explicitly checked before traversal.
-
-        using current_node.next for traversal accounts for a one node list
-        as .next is not set on the head of a one node list."""
-        self.target = target_data  # trigger setter
-        # insert before first occurence
-        if getattr(self._head, 'data') == self._target:
-            self.head = data_to_insert  # trigger the setter, head property will validate input
-            return
-        current_node = getattr(self, '_head')  # traversal
-        while current_node: # traversal
+        Returns:
+            bool: True if the insertion was successful, False otherwise.
+
+        Raises:
+            ValueError: If the target data is not found in the linked list.
+
+        Note:
+            This method assumes that the linked list has already been instantiated.
+            If the target data is found at the head of the linked list, the new node
+            will become the new head of the list.
+
+        Examples:
+            >>> sllist = SinglyLinkedList(['foo', 'bar'])
+            >>> sllist.insert_before_target('foo', 'before_head')
+            True
+            >>> sllist
+            SinglyLinkedList(['before_head', 'foo', 'bar'])
+
+            >>> sllist.insert_before_target('baz', 'new node')
+            False
+            >>> sllist
+            SinglyLinkedList(['before_head', 'foo', 'bar'])
+
+            >>> sllist.insert_before_target(sllist.head, 'new node')
+            True
+            >>> sllist
+            SinglyLinkedList(['new node', 'before_head', 'foo', 'bar'])
+        """
+        try:
+            self.target = target_data  # trigger the setter
+        except ValueError:
+            return False
+        current_node = getattr(self, '_head')
+        while current_node and current_node.next: # traversal
+            # check head
+            if current_node.data == self._target:
+                self.head = data_to_insert  # trigger the setter, head property will validate input
+                return True
+            # check after head through tail
             if current_node.next.data == self._target:  # peek
-                #node = current_node.next  # the node containing the target
-                new_node = SinglyNode(data_to_insert)
+                new_node = SinglyNode(data_to_insert)  # SinglyNode() will validate data_to_insert
                 setattr(new_node, '_next', current_node.next)  # insert_before()
                 setattr(current_node, '_next', new_node)  # insert before()
-                return #node
-            current_node = current_node.next  # traversal
+                return True
+            current_node = getattr(current_node, 'next')  # traversal
+        return False
+
+
 
     def search(self, target_data):
         """Searches each node's data in a linked list until the first occurrence of
         the target is found.
 
         Args:
             target_data (Any): The value to search for in the linked list.
```

### Comparing `ofnodes-1.6.0/PKG-INFO` & `ofnodes-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofnodes
-Version: 1.6.0
+Version: 1.6.1
 Summary: A library of Data Structures and Algorithms written in Python
 Author: Robert Portelli
 Author-email: github@robertportelli.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

