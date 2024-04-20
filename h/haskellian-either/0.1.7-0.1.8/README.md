# Comparing `tmp/haskellian_either-0.1.7.tar.gz` & `tmp/haskellian_either-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haskellian_either-0.1.7.tar", last modified: Fri Apr 12 17:46:53 2024, max compression
+gzip compressed data, was "haskellian_either-0.1.8.tar", last modified: Fri Apr 19 10:23:05 2024, max compression
```

## Comparing `haskellian_either-0.1.7.tar` & `haskellian_either-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-12 17:46:53.787777 haskellian_either-0.1.7/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      319 2024-04-12 17:46:53.777776 haskellian_either-0.1.7/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       41 2024-04-02 05:31:14.000000 haskellian_either-0.1.7/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      514 2024-04-12 17:46:51.000000 haskellian_either-0.1.7/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-12 17:46:53.787777 haskellian_either-0.1.7/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-12 17:46:53.777776 haskellian_either-0.1.7/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-12 17:46:53.777776 haskellian_either-0.1.7/src/haskellian/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-12 17:46:53.777776 haskellian_either-0.1.7/src/haskellian/either/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      286 2024-04-12 17:17:47.000000 haskellian_either-0.1.7/src/haskellian/either/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-12 17:46:53.777776 haskellian_either-0.1.7/src/haskellian/either/extras/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-04-05 16:46:47.000000 haskellian_either-0.1.7/src/haskellian/either/extras/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      464 2024-04-05 16:46:28.000000 haskellian_either-0.1.7/src/haskellian/either/extras/pydantic.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1283 2024-04-12 17:17:42.000000 haskellian_either-0.1.7/src/haskellian/either/funcs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      300 2024-04-08 13:18:48.000000 haskellian_either-0.1.7/src/haskellian/either/narrowing.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2082 2024-04-09 09:12:43.000000 haskellian_either-0.1.7/src/haskellian/either/type.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-12 17:46:53.777776 haskellian_either-0.1.7/src/haskellian_either.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      319 2024-04-12 17:46:53.000000 haskellian_either-0.1.7/src/haskellian_either.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      460 2024-04-12 17:46:53.000000 haskellian_either-0.1.7/src/haskellian_either.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-12 17:46:53.000000 haskellian_either-0.1.7/src/haskellian_either.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       21 2024-04-12 17:46:53.000000 haskellian_either-0.1.7/src/haskellian_either.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-12 17:46:53.000000 haskellian_either-0.1.7/src/haskellian_either.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-19 10:23:05.362170 haskellian_either-0.1.8/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      319 2024-04-19 10:23:05.362170 haskellian_either-0.1.8/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       41 2024-04-02 05:31:14.000000 haskellian_either-0.1.8/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      514 2024-04-19 10:23:02.000000 haskellian_either-0.1.8/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-19 10:23:05.362170 haskellian_either-0.1.8/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-19 10:23:05.362170 haskellian_either-0.1.8/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-19 10:23:05.362170 haskellian_either-0.1.8/src/haskellian/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-19 10:23:05.362170 haskellian_either-0.1.8/src/haskellian/either/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      286 2024-04-12 17:17:47.000000 haskellian_either-0.1.8/src/haskellian/either/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-19 10:23:05.362170 haskellian_either-0.1.8/src/haskellian/either/extras/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-04-05 16:46:47.000000 haskellian_either-0.1.8/src/haskellian/either/extras/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      464 2024-04-05 16:46:28.000000 haskellian_either-0.1.8/src/haskellian/either/extras/pydantic.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1283 2024-04-12 17:17:42.000000 haskellian_either-0.1.8/src/haskellian/either/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      300 2024-04-08 13:18:48.000000 haskellian_either-0.1.8/src/haskellian/either/narrowing.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2198 2024-04-19 10:22:58.000000 haskellian_either-0.1.8/src/haskellian/either/type.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-19 10:23:05.362170 haskellian_either-0.1.8/src/haskellian_either.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      319 2024-04-19 10:23:05.000000 haskellian_either-0.1.8/src/haskellian_either.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      460 2024-04-19 10:23:05.000000 haskellian_either-0.1.8/src/haskellian_either.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-19 10:23:05.000000 haskellian_either-0.1.8/src/haskellian_either.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       21 2024-04-19 10:23:05.000000 haskellian_either-0.1.8/src/haskellian_either.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-19 10:23:05.000000 haskellian_either-0.1.8/src/haskellian_either.egg-info/top_level.txt
```

### Comparing `haskellian_either-0.1.7/pyproject.toml` & `haskellian_either-0.1.8/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "haskellian-either"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Simple Either type"
 dependencies = []
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
```

### Comparing `haskellian_either-0.1.7/src/haskellian/either/funcs.py` & `haskellian_either-0.1.8/src/haskellian/either/funcs.py`

 * *Files identical despite different names*

### Comparing `haskellian_either-0.1.7/src/haskellian/either/type.py` & `haskellian_either-0.1.8/src/haskellian/either/type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,75 @@
 from typing import Generic, TypeVar, Literal, Callable, Any, TypeGuard
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 
-A = TypeVar('A', covariant=True)
+A = TypeVar('A')
 L = TypeVar('L', covariant=True)
 R = TypeVar('R', covariant=True)
 L2 = TypeVar('L2')
 R2 = TypeVar('R2')
 
 @dataclass(eq=False)
 class IsLeft(BaseException, Generic[L]):
   value: L
 
 class EitherBase(ABC, Generic[L, R]):
 
   @abstractmethod
-  def _match(self, on_left: Callable[[L], A], on_right: Callable[[R], A]) -> int:
+  def _match(self, on_left: Callable[[L], A], on_right: Callable[[R], A]) -> A:
     """Unwrap an `Either` by matching both branches"""
   
   def match(self, on_left: Callable[[L], A], on_right: Callable[[R], A]) -> A:
     """Unwrap an `Either` by matching both branches"""
     return self._match(on_left, on_right)
 
   @abstractmethod
   def unsafe(self) -> R:
     """Unwraps the value or throws an `IsLeft` exception
     
     (`IsLeft.value` will contain the wrapped value)"""
     
 
-  def bind(self, f: 'Callable[[R], Either[L, R2]]') -> 'Either[L, R2]':
+  def bind(self, f: 'Callable[[R], Either[L2, R2]]') -> 'Either[L|L2, R2]':
     return self.match(lambda x: Left(x), f)
 
   def fmap(self, f: Callable[[R], R2]) -> 'Either[L, R2]':
     return self.match(lambda x: Left(x), lambda x: Right(f(x)))
 
   def mapl(self, f: Callable[[L], L2]) -> 'Either[L2, R]':
     """Map the left branch"""
     return self.match(lambda x: Left(f(x)), lambda x: Right(x))
+  
+  def get_or(self, fallback: A) -> A | R:
+    return self.match(lambda _: fallback, lambda x: x)
 
   __or__ = fmap
   """Alias of `fmap`"""
   
   __and__ = bind
   """Alias of `bind`"""
   
   def match_(self, on_left: Callable[[], A], on_right: Callable[[], A]) -> A:
     """Like `match`, but handlers don't get the wrapped value"""
     return self.match(lambda _: on_left(), lambda _: on_right())
   
 @dataclass
 class Left(EitherBase[L, R], Generic[L, R]):
-  value: L = None
+  value: L = None # type: ignore
   tag: Literal['left'] = 'left'
 
   def _match(self, on_left, on_right):
     return on_left(self.value)
   
   def unsafe(self):
     raise IsLeft(self.value)
 
 @dataclass
 class Right(EitherBase[L, R], Generic[L, R]):
-  value: R = None
+  value: R = None # type: ignore
   tag: Literal['right'] = 'right'
 
   def _match(self, on_left, on_right):
     return on_right(self.value)
   
   def unsafe(self) -> R:
     return self.value
```

