# Comparing `tmp/pyiter-0.8.5.tar.gz` & `tmp/pyiter-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiter-0.8.5.tar", last modified: Tue Apr 16 13:46:13 2024, max compression
+gzip compressed data, was "pyiter-0.8.7.tar", last modified: Fri Apr 19 06:42:18 2024, max compression
```

## Comparing `pyiter-0.8.5.tar` & `pyiter-0.8.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-16 13:46:13.239461 pyiter-0.8.5/
--rw-r--r--   0 yish      (1000) yish      (1000)    11357 2023-09-09 01:32:37.000000 pyiter-0.8.5/LICENSE-APACHE
--rw-r--r--   0 yish      (1000) yish      (1000)     1062 2023-09-08 13:21:33.000000 pyiter-0.8.5/LICENSE-MIT
--rw-r--r--   0 yish      (1000) yish      (1000)     2900 2024-04-16 13:46:13.239461 pyiter-0.8.5/PKG-INFO
--rw-r--r--   0 yish      (1000) yish      (1000)     2346 2024-04-13 12:58:27.000000 pyiter-0.8.5/README.md
--rw-r--r--   0 yish      (1000) yish      (1000)       84 2023-10-12 09:06:56.000000 pyiter-0.8.5/pyproject.toml
--rw-r--r--   0 yish      (1000) yish      (1000)       38 2024-04-16 13:46:13.239461 pyiter-0.8.5/setup.cfg
--rw-r--r--   0 yish      (1000) yish      (1000)      846 2024-04-16 13:45:54.000000 pyiter-0.8.5/setup.py
-drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-16 13:46:13.239461 pyiter-0.8.5/src/
-drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-16 13:46:13.239461 pyiter-0.8.5/src/pyiter/
--rw-r--r--   0 yish      (1000) yish      (1000)      624 2024-03-26 03:31:01.000000 pyiter-0.8.5/src/pyiter/__init__.py
--rw-r--r--   0 yish      (1000) yish      (1000)    95789 2024-04-16 08:53:27.000000 pyiter-0.8.5/src/pyiter/sequence.py
-drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-16 13:46:13.239461 pyiter-0.8.5/src/pyiter.egg-info/
--rw-r--r--   0 yish      (1000) yish      (1000)     2900 2024-04-16 13:46:13.000000 pyiter-0.8.5/src/pyiter.egg-info/PKG-INFO
--rw-r--r--   0 yish      (1000) yish      (1000)      275 2024-04-16 13:46:13.000000 pyiter-0.8.5/src/pyiter.egg-info/SOURCES.txt
--rw-r--r--   0 yish      (1000) yish      (1000)        1 2024-04-16 13:46:13.000000 pyiter-0.8.5/src/pyiter.egg-info/dependency_links.txt
--rw-r--r--   0 yish      (1000) yish      (1000)       11 2024-04-16 13:46:13.000000 pyiter-0.8.5/src/pyiter.egg-info/requires.txt
--rw-r--r--   0 yish      (1000) yish      (1000)        7 2024-04-16 13:46:13.000000 pyiter-0.8.5/src/pyiter.egg-info/top_level.txt
+drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-19 06:42:18.982126 pyiter-0.8.7/
+-rw-r--r--   0 yish      (1000) yish      (1000)    11357 2023-09-09 01:32:37.000000 pyiter-0.8.7/LICENSE-APACHE
+-rw-r--r--   0 yish      (1000) yish      (1000)     1062 2023-09-08 13:21:33.000000 pyiter-0.8.7/LICENSE-MIT
+-rw-r--r--   0 yish      (1000) yish      (1000)     2900 2024-04-19 06:42:18.982126 pyiter-0.8.7/PKG-INFO
+-rw-r--r--   0 yish      (1000) yish      (1000)     2346 2024-04-13 12:58:27.000000 pyiter-0.8.7/README.md
+-rw-r--r--   0 yish      (1000) yish      (1000)       84 2023-10-12 09:06:56.000000 pyiter-0.8.7/pyproject.toml
+-rw-r--r--   0 yish      (1000) yish      (1000)       38 2024-04-19 06:42:18.982126 pyiter-0.8.7/setup.cfg
+-rw-r--r--   0 yish      (1000) yish      (1000)      846 2024-04-19 06:42:07.000000 pyiter-0.8.7/setup.py
+drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-19 06:42:18.972126 pyiter-0.8.7/src/
+drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-19 06:42:18.982126 pyiter-0.8.7/src/pyiter/
+-rw-r--r--   0 yish      (1000) yish      (1000)      624 2024-03-26 03:31:01.000000 pyiter-0.8.7/src/pyiter/__init__.py
+-rw-r--r--   0 yish      (1000) yish      (1000)    96689 2024-04-19 06:40:44.000000 pyiter-0.8.7/src/pyiter/sequence.py
+drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-19 06:42:18.982126 pyiter-0.8.7/src/pyiter.egg-info/
+-rw-r--r--   0 yish      (1000) yish      (1000)     2900 2024-04-19 06:42:18.000000 pyiter-0.8.7/src/pyiter.egg-info/PKG-INFO
+-rw-r--r--   0 yish      (1000) yish      (1000)      275 2024-04-19 06:42:18.000000 pyiter-0.8.7/src/pyiter.egg-info/SOURCES.txt
+-rw-r--r--   0 yish      (1000) yish      (1000)        1 2024-04-19 06:42:18.000000 pyiter-0.8.7/src/pyiter.egg-info/dependency_links.txt
+-rw-r--r--   0 yish      (1000) yish      (1000)       11 2024-04-19 06:42:18.000000 pyiter-0.8.7/src/pyiter.egg-info/requires.txt
+-rw-r--r--   0 yish      (1000) yish      (1000)        7 2024-04-19 06:42:18.000000 pyiter-0.8.7/src/pyiter.egg-info/top_level.txt
```

### Comparing `pyiter-0.8.5/LICENSE-APACHE` & `pyiter-0.8.7/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `pyiter-0.8.5/LICENSE-MIT` & `pyiter-0.8.7/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `pyiter-0.8.5/PKG-INFO` & `pyiter-0.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiter
-Version: 0.8.5
+Version: 0.8.7
 Summary: PyIter is a Python package for iterative operations inspired by the Kotlin、CSharp(linq)、TypeSrcipt and Rust . Enables strong typing and type inference for iterative operations.
 Home-page: https://github.com/mokeyish/pyiter
 Author: YISH
 Author-email: mokeyish@hotmail.com
 License: MIT
 Keywords: linq,iterator,typing,lazy evaluation,type inference
 Requires-Python: >=3.8
```

### Comparing `pyiter-0.8.5/README.md` & `pyiter-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `pyiter-0.8.5/setup.py` & `pyiter-0.8.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='pyiter',
-    version='0.8.5',
+    version='0.8.7',
     keywords=['linq', 'iterator', 'typing', 'lazy evaluation', 'type inference'],
     description='PyIter is a Python package for iterative operations inspired by the Kotlin、CSharp(linq)、TypeSrcipt '
                 'and Rust . Enables strong typing and type inference for iterative operations.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='YISH',
     author_email="mokeyish@hotmail.com",
```

### Comparing `pyiter-0.8.5/src/pyiter/__init__.py` & `pyiter-0.8.7/src/pyiter/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiter-0.8.5/src/pyiter/sequence.py` & `pyiter-0.8.7/src/pyiter/sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,15 @@
     
     The values are evaluated lazily, and the sequence is potentially infinite.
     """
     _iter: SequenceTransform[Iterable[T], T]
 
     def __init__(self, iterable: Iterable[T]) -> None:
         super().__init__()
-        if not isinstance(isinstance, SequenceTransform):
-            iterable = SequenceTransform(iterable)
-        self._iter = iterable
+        self._iter = SequenceTransform(iterable)
 
     @overload
     def filter(self, predicate: Callable[[T], bool]) -> Sequence[T]:
         ...
     @overload
     def filter(self, predicate: Callable[[T, int], bool]) -> Sequence[T]:
         ...
@@ -530,15 +528,15 @@
         1
 
         Example 2:
         >>> lst = ['a', 'b', 'c']
         >>> it(lst).index_of('d')
         -1
         """
-        return self.index_of_or_none(element) or -1
+        return none_or(self.index_of_or_none(element), -1)
     
     def last_index_of_or_none(self, element: T) -> Optional[int]:
         """
          Returns last index of [element], or None if the collection does not contain element.
 
         Example 1:
         >>> lst = ['a', 'b', 'c', 'b']
@@ -546,15 +544,15 @@
         3
 
         Example 2:
         >>> lst = ['a', 'b', 'c']
         >>> it(lst).last_index_of_or_none('d')
         """
         seq = self.reversed()
-        last_idx = len(seq) - 1;
+        last_idx = len(seq) - 1
         for i, x in enumerate(seq):
             if x == element:
                 return last_idx - i
         return None
 
     def last_index_of(self, element: T) -> int:
         """
@@ -566,15 +564,15 @@
         3
 
         Example 2:
         >>> lst = ['a', 'b', 'c']
         >>> it(lst).last_index_of('d')
         -1
         """
-        return self.last_index_of_or_none(element) or -1
+        return none_or(self.last_index_of_or_none(element), -1)
 
     @overload
     def index_of_first_or_none(self, predicate: Callable[[T], bool]) -> Optional[int]:
         ...
     @overload
     def index_of_first_or_none(self, predicate: Callable[[T, int], bool]) -> Optional[int]:
         ...
@@ -618,16 +616,21 @@
         >>> it(lst).index_of_first(lambda x: x == 'b')
         1
 
         Example 2:
         >>> lst = ['a', 'b', 'c']
         >>> it(lst).index_of_first(lambda x: x == 'd')
         -1
+
+        Example 3:
+        >>> lst = ['a', 'b', 'c']
+        >>> it(lst).index_of_first(lambda x: x == 'a')
+        0
         """
-        return self.index_of_first_or_none(predicate) or -1
+        return none_or(self.index_of_first_or_none(predicate), -1)
 
     @overload
     def index_of_last_or_none(self, predicate: Callable[[T], bool]) -> Optional[int]:
         ...
     @overload
     def index_of_last_or_none(self, predicate: Callable[[T, int], bool]) -> Optional[int]:
         ...
@@ -673,16 +676,21 @@
         >>> it(lst).index_of_last(lambda x: x == 'b')
         3
 
         Example 2:
         >>> lst = ['a', 'b', 'c']
         >>> it(lst).index_of_last(lambda x: x == 'd')
         -1
+
+        Example 3:
+        >>> lst = ['a', 'b', 'c']
+        >>> it(lst).index_of_last(lambda x: x == 'a')
+        0
         """
-        return self.index_of_last_or_none(predicate) or -1
+        return none_or(self.index_of_last_or_none(predicate), -1)
 
     @overload
     def single(self) -> T:
         ...
     @overload
     def single(self, predicate: Callable[[T], bool]) -> T:
         ...
@@ -1252,14 +1260,16 @@
         >>> it(lst).element_at_or_else(4, lambda x: 'default')
         'default'
 
         """
         if (index < 0):
             return default(index) if callable(default) else default
         
+        if type(self._iter) == SequenceTransform and isinstance(self._iter._iter, list) and index < len(self._iter._iter): # type: ignore
+            return self._iter._iter[index] # type: ignore
         for i, e in enumerate(self):
             if i == index:
                 return e
         return default(index) if callable(default) else default
     
 
     def element_at_or_default(self, index: int, default: T) -> T:
@@ -2346,15 +2356,15 @@
         {1: '1', 2: '2', 3: '3'}
 
         Example 2:
         >>> lst = [(1, '1'), (2, '2'), (3, '3')]
         >>> it(lst).to_dict()
         {1: '1', 2: '2', 3: '3'}
         """
-        return self.associate(transform or (lambda x: x))
+        return self.associate(transform or (lambda x: x)) # type: ignore
 
     def to_list(self) -> List[T]:
         """
         Returns a list with elements of the given Sequence.
 
         Example 1:
         >>> it(['b', 'c', 'a']).to_list()
@@ -2421,14 +2431,32 @@
     
     def __do_iter(self) -> Iterator[T]:
         yield from self._iter
 
     def __len__(self):
         return len(self._iter)
 
+    def __getitem__(self, key: int):
+        """
+        Returns the element at the specified [index] in the Sequence.
+
+        Example 1:
+        >>> lst = [1, 2, 3]
+        >>> it(lst)[1]
+        2
+
+        Example 2:
+        >>> lst = [1, 2, 3]
+        >>> it(lst)[3]
+        Traceback (most recent call last):
+        ...
+        IndexError: Index 3 out of range
+        """
+        return self.element_at(key)
+
     @overload
     def _callback_overload_warpper(self, callback: Callable[[T], R]) -> Callable[[T], R]:
         ...
     @overload
     def _callback_overload_warpper(self, callback: Callable[[T, int], R]) -> Callable[[T], R]:
         ...
     @overload
@@ -2802,14 +2830,18 @@
     #     return ListLike(self._iter)
 
     
 def throw(exception: Exception) -> Any:
     raise exception
 
 
+def none_or(value: Optional[T], default: T) -> T:
+    return default if value is None else value
+
+
 class SequenceProducer:
     @overload
     def __call__(self, elements: List[T]) -> Sequence[T]:
         ...
     @overload
     def __call__(self, elements: Iterable[T]) -> Sequence[T]:
         ...
```

### Comparing `pyiter-0.8.5/src/pyiter.egg-info/PKG-INFO` & `pyiter-0.8.7/src/pyiter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiter
-Version: 0.8.5
+Version: 0.8.7
 Summary: PyIter is a Python package for iterative operations inspired by the Kotlin、CSharp(linq)、TypeSrcipt and Rust . Enables strong typing and type inference for iterative operations.
 Home-page: https://github.com/mokeyish/pyiter
 Author: YISH
 Author-email: mokeyish@hotmail.com
 License: MIT
 Keywords: linq,iterator,typing,lazy evaluation,type inference
 Requires-Python: >=3.8
```

