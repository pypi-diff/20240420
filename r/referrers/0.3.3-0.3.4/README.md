# Comparing `tmp/referrers-0.3.3.tar.gz` & `tmp/referrers-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "referrers-0.3.3.tar", max compression
+gzip compressed data, was "referrers-0.3.4.tar", max compression
```

## Comparing `referrers-0.3.3.tar` & `referrers-0.3.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2024-04-19 17:05:14.757568 referrers-0.3.3/LICENSE
--rw-r--r--   0        0        0     6887 2024-04-19 17:05:14.757568 referrers-0.3.3/README.md
--rw-r--r--   0        0        0      372 2024-04-19 17:05:14.761568 referrers-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      130 2024-04-19 17:05:14.761568 referrers-0.3.3/src/referrers/__init__.py
--rw-r--r--   0        0        0    37144 2024-04-19 17:05:14.761568 referrers-0.3.3/src/referrers/impl.py
--rw-r--r--   0        0        0     7420 1970-01-01 00:00:00.000000 referrers-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-19 17:07:28.050418 referrers-0.3.4/LICENSE
+-rw-r--r--   0        0        0     7266 2024-04-19 17:07:28.050418 referrers-0.3.4/README.md
+-rw-r--r--   0        0        0      372 2024-04-19 17:07:28.050418 referrers-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-04-19 17:07:28.050418 referrers-0.3.4/src/referrers/__init__.py
+-rw-r--r--   0        0        0    37144 2024-04-19 17:07:28.050418 referrers-0.3.4/src/referrers/impl.py
+-rw-r--r--   0        0        0     7799 1970-01-01 00:00:00.000000 referrers-0.3.4/PKG-INFO
```

### Comparing `referrers-0.3.3/LICENSE` & `referrers-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `referrers-0.3.3/README.md` & `referrers-0.3.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -93,26 +93,39 @@
 is in turn referenced by a local variable in the `my_func` function.
 
 ## Integration with memory analysis tools
 
 This library can be used with other memory analysis tools to help identify the source
 of memory leaks.
 
-For example, to print the referrers of all lists using
-[Pympler](https://pympler.readthedocs.io/en/latest/) (warning: this may produce a lot of output!):
+For example, to print the referrers of the top 10 largest objects using 
+[Pympler](https://pympler.readthedocs.io/en/latest/):
 
 ```python
-import referrers
 from pympler import muppy
+import referrers
+
+top_10_objects = (muppy.sort(muppy.get_objects()))[-10:]
+top_10_objects.reverse()
+
+for obj in top_10_objects:
+    print(
+        referrers.get_referrer_graph(
+            obj,
+            search_for_untracked_objects=True,
+            exclude_object_ids=[id(top_10_objects)],
+        )
+    )
 
-all_dicts = [obj for obj in muppy.get_objects() if isinstance(obj, list)]
-for obj in all_dicts:
-    print(referrers.get_referrer_graph(obj))
 ```
 
+Note that this example sets the `search_for_untracked_objects` flag to `True` to try to find
+referrers for objects that are not tracked by the garbage collector. It also sets
+`exclude_object_ids` to exclude the `top_10_objects` variable from the graph.
+
 ## Integration with NetworkX
 
 The graph produced by `get_referrer_graph` can be converted to a NetworkX graph using
 its `to_networkx` method. This can be useful for visualizing the graph, or for
 performing more complex analysis.
 
 The resulting NetworkX graph consists of nodes of type `ReferrerGraphNode`, with edges
```

### Comparing `referrers-0.3.3/src/referrers/impl.py` & `referrers-0.3.4/src/referrers/impl.py`

 * *Files identical despite different names*

### Comparing `referrers-0.3.3/PKG-INFO` & `referrers-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: referrers
-Version: 0.3.3
+Version: 0.3.4
 Summary: Finds the graph of referrers for a Python object
 Author: Neil Ferguson
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -108,26 +108,39 @@
 is in turn referenced by a local variable in the `my_func` function.
 
 ## Integration with memory analysis tools
 
 This library can be used with other memory analysis tools to help identify the source
 of memory leaks.
 
-For example, to print the referrers of all lists using
-[Pympler](https://pympler.readthedocs.io/en/latest/) (warning: this may produce a lot of output!):
+For example, to print the referrers of the top 10 largest objects using 
+[Pympler](https://pympler.readthedocs.io/en/latest/):
 
 ```python
-import referrers
 from pympler import muppy
+import referrers
+
+top_10_objects = (muppy.sort(muppy.get_objects()))[-10:]
+top_10_objects.reverse()
+
+for obj in top_10_objects:
+    print(
+        referrers.get_referrer_graph(
+            obj,
+            search_for_untracked_objects=True,
+            exclude_object_ids=[id(top_10_objects)],
+        )
+    )
 
-all_dicts = [obj for obj in muppy.get_objects() if isinstance(obj, list)]
-for obj in all_dicts:
-    print(referrers.get_referrer_graph(obj))
 ```
 
+Note that this example sets the `search_for_untracked_objects` flag to `True` to try to find
+referrers for objects that are not tracked by the garbage collector. It also sets
+`exclude_object_ids` to exclude the `top_10_objects` variable from the graph.
+
 ## Integration with NetworkX
 
 The graph produced by `get_referrer_graph` can be converted to a NetworkX graph using
 its `to_networkx` method. This can be useful for visualizing the graph, or for
 performing more complex analysis.
 
 The resulting NetworkX graph consists of nodes of type `ReferrerGraphNode`, with edges
```

