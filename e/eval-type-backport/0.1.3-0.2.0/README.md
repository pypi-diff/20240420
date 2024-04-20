# Comparing `tmp/eval_type_backport-0.1.3.tar.gz` & `tmp/eval_type_backport-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eval_type_backport-0.1.3.tar", last modified: Sun Dec 17 18:03:39 2023, max compression
+gzip compressed data, was "eval_type_backport-0.2.0.tar", last modified: Sat Apr 20 13:04:00 2024, max compression
```

## Comparing `eval_type_backport-0.1.3.tar` & `eval_type_backport-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-12-17 18:03:39.406530 eval_type_backport-0.1.3/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-12-17 18:03:39.402530 eval_type_backport-0.1.3/.github/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-12-17 18:03:39.402530 eval_type_backport-0.1.3/.github/workflows/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1405 2023-11-24 14:31:04.000000 eval_type_backport-0.1.3/.github/workflows/test.yml
--rw-rw-r--   0 alex      (1000) alex      (1000)      727 2023-11-10 14:34:35.000000 eval_type_backport-0.1.3/.gitignore
--rw-rw-r--   0 alex      (1000) alex      (1000)      441 2023-11-10 14:11:59.000000 eval_type_backport-0.1.3/.pre-commit-config.yaml
--rw-rw-r--   0 alex      (1000) alex      (1000)     1066 2023-11-10 14:29:58.000000 eval_type_backport-0.1.3/LICENSE.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       20 2020-08-14 19:28:33.000000 eval_type_backport-0.1.3/MANIFEST.in
--rw-r--r--   0 alex      (1000) alex      (1000)     1937 2023-12-17 18:03:39.406530 eval_type_backport-0.1.3/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1058 2023-12-16 18:35:44.000000 eval_type_backport-0.1.3/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-12-17 18:03:39.402530 eval_type_backport-0.1.3/eval_type_backport/
--rw-rw-r--   0 alex      (1000) alex      (1000)      273 2023-11-18 13:08:15.000000 eval_type_backport-0.1.3/eval_type_backport/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6992 2023-12-17 18:03:28.000000 eval_type_backport-0.1.3/eval_type_backport/eval_type_backport.py
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-16 19:09:43.000000 eval_type_backport-0.1.3/eval_type_backport/py.typed
--rw-rw-r--   0 alex      (1000) alex      (1000)       21 2023-12-17 18:03:39.000000 eval_type_backport-0.1.3/eval_type_backport/version.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-12-17 18:03:39.406530 eval_type_backport-0.1.3/eval_type_backport.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)     1937 2023-12-17 18:03:39.000000 eval_type_backport-0.1.3/eval_type_backport.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      561 2023-12-17 18:03:39.000000 eval_type_backport-0.1.3/eval_type_backport.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-12-17 18:03:39.000000 eval_type_backport-0.1.3/eval_type_backport.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-11-10 14:32:41.000000 eval_type_backport-0.1.3/eval_type_backport.egg-info/not-zip-safe
--rw-rw-r--   0 alex      (1000) alex      (1000)       16 2023-12-17 18:03:39.000000 eval_type_backport-0.1.3/eval_type_backport.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       19 2023-12-17 18:03:39.000000 eval_type_backport-0.1.3/eval_type_backport.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      476 2023-11-10 14:25:58.000000 eval_type_backport-0.1.3/pyproject.toml
--rwxrwxr-x   0 alex      (1000) alex      (1000)      586 2023-11-22 18:55:43.000000 eval_type_backport-0.1.3/release.sh
--rw-rw-r--   0 alex      (1000) alex      (1000)     1050 2023-12-17 18:03:39.406530 eval_type_backport-0.1.3/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)       63 2023-11-10 14:35:07.000000 eval_type_backport-0.1.3/setup.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-12-17 18:03:39.406530 eval_type_backport-0.1.3/tests/
--rw-rw-r--   0 alex      (1000) alex      (1000)     9045 2023-12-17 16:23:58.000000 eval_type_backport-0.1.3/tests/test_eval_type_backport.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      113 2023-11-10 14:32:26.000000 eval_type_backport-0.1.3/tox.ini
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-20 13:04:00.818619 eval_type_backport-0.2.0/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-20 13:04:00.814619 eval_type_backport-0.2.0/.github/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-20 13:04:00.814619 eval_type_backport-0.2.0/.github/workflows/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1387 2024-04-20 13:01:47.000000 eval_type_backport-0.2.0/.github/workflows/test.yml
+-rw-rw-r--   0 alex      (1000) alex      (1000)      727 2023-11-10 14:34:35.000000 eval_type_backport-0.2.0/.gitignore
+-rw-rw-r--   0 alex      (1000) alex      (1000)      441 2023-11-10 14:11:59.000000 eval_type_backport-0.2.0/.pre-commit-config.yaml
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1066 2023-11-10 14:29:58.000000 eval_type_backport-0.2.0/LICENSE.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       20 2020-08-14 19:28:33.000000 eval_type_backport-0.2.0/MANIFEST.in
+-rw-r--r--   0 alex      (1000) alex      (1000)     2195 2024-04-20 13:04:00.818619 eval_type_backport-0.2.0/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1366 2024-04-20 13:01:47.000000 eval_type_backport-0.2.0/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-20 13:04:00.818619 eval_type_backport-0.2.0/eval_type_backport/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      299 2024-04-20 13:01:47.000000 eval_type_backport-0.2.0/eval_type_backport/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8198 2024-04-20 13:01:47.000000 eval_type_backport-0.2.0/eval_type_backport/eval_type_backport.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-16 19:09:43.000000 eval_type_backport-0.2.0/eval_type_backport/py.typed
+-rw-rw-r--   0 alex      (1000) alex      (1000)       21 2024-04-20 13:04:00.000000 eval_type_backport-0.2.0/eval_type_backport/version.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-20 13:04:00.818619 eval_type_backport-0.2.0/eval_type_backport.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)     2195 2024-04-20 13:04:00.000000 eval_type_backport-0.2.0/eval_type_backport.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      561 2024-04-20 13:04:00.000000 eval_type_backport-0.2.0/eval_type_backport.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2024-04-20 13:04:00.000000 eval_type_backport-0.2.0/eval_type_backport.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-11-10 14:32:41.000000 eval_type_backport-0.2.0/eval_type_backport.egg-info/not-zip-safe
+-rw-rw-r--   0 alex      (1000) alex      (1000)       16 2024-04-20 13:04:00.000000 eval_type_backport-0.2.0/eval_type_backport.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       19 2024-04-20 13:04:00.000000 eval_type_backport-0.2.0/eval_type_backport.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      475 2024-04-20 13:01:47.000000 eval_type_backport-0.2.0/pyproject.toml
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      586 2023-11-22 18:55:43.000000 eval_type_backport-0.2.0/release.sh
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1011 2024-04-20 13:04:00.818619 eval_type_backport-0.2.0/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)       63 2023-11-10 14:35:07.000000 eval_type_backport-0.2.0/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-20 13:04:00.818619 eval_type_backport-0.2.0/tests/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9802 2024-04-20 13:01:47.000000 eval_type_backport-0.2.0/tests/test_eval_type_backport.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      108 2024-04-20 13:01:47.000000 eval_type_backport-0.2.0/tox.ini
```

### Comparing `eval_type_backport-0.1.3/.github/workflows/test.yml` & `eval_type_backport-0.2.0/.github/workflows/test.yml`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 jobs:
   test:
     name: test ${{ matrix.os }} / ${{ matrix.python-version }}
     strategy:
       fail-fast: false
       matrix:
         os: [ ubuntu, macos, windows ]
-        python-version: [ '3.7', '3.8', '3.9', '3.10', '3.11', '3.12', 'pypy3.7', 'pypy3.8', 'pypy3.9', 'pypy3.10' ]
+        python-version: [ '3.8', '3.9', '3.10', '3.11', '3.12', 'pypy3.8', 'pypy3.9', 'pypy3.10' ]
 
     runs-on: ${{ matrix.os }}-latest
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python --version
         pip install --upgrade pip
         pip install --upgrade coveralls .[tests]
```

### Comparing `eval_type_backport-0.1.3/.gitignore` & `eval_type_backport-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `eval_type_backport-0.1.3/LICENSE.txt` & `eval_type_backport-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eval_type_backport-0.1.3/PKG-INFO` & `eval_type_backport-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,47 @@
 Metadata-Version: 2.1
 Name: eval_type_backport
-Version: 0.1.3
+Version: 0.2.0
 Summary: Like `typing._eval_type`, but lets older Python versions use newer typing features.
 Home-page: https://github.com/alexmojaki/eval_type_backport
 Author: Alex Hall
 Author-email: alex.mojaki@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 
 # eval_type_backport
 
-[![Build Status](https://github.com/alexmojaki/eval_type_backport/workflows/Tests/badge.svg)](https://github.com/alexmojaki/eval_type_backport/actions) [![Coverage Status](https://coveralls.io/repos/github/alexmojaki/eval_type_backport/badge.svg)](https://coveralls.io/github/alexmojaki/eval_type_backport) [![Supports Python versions 3.7+, including PyPy](https://img.shields.io/pypi/pyversions/eval_type_backport.svg)](https://pypi.python.org/pypi/eval_type_backport)
+[![Build Status](https://github.com/alexmojaki/eval_type_backport/workflows/Tests/badge.svg)](https://github.com/alexmojaki/eval_type_backport/actions) [![Coverage Status](https://coveralls.io/repos/github/alexmojaki/eval_type_backport/badge.svg)](https://coveralls.io/github/alexmojaki/eval_type_backport) [![Supports Python versions 3.8+, including PyPy](https://img.shields.io/pypi/pyversions/eval_type_backport.svg)](https://pypi.python.org/pypi/eval_type_backport) [![Anaconda's conda-forge channel](https://anaconda.org/conda-forge/eval-type-backport/badges/version.svg)](https://anaconda.org/conda-forge/eval-type-backport)
 
 This is a tiny package providing a replacement for `typing._eval_type` to support newer typing features in older Python versions.
 
 Yes, that's very specific, and yes, `typing._eval_type` is a protected function that you shouldn't normally be using. Really this package is specifically made for https://github.com/pydantic/pydantic/issues/7873.
 
 Specifically, this transforms `X | Y` into `typing.Union[X, Y]`
 and `list[X]` into `typing.List[X]` etc. (for all the types made generic in PEP 585)
 if the original syntax is not supported in the current Python version.
+
+## Install
+
+From PyPI:
+
+```shell
+pip install eval-type-backport
+```
+
+or with Conda:
+
+```shell
+conda install -c conda-forge eval-type-backport
+```
```

### Comparing `eval_type_backport-0.1.3/README.md` & `eval_type_backport-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 # eval_type_backport
 
-[![Build Status](https://github.com/alexmojaki/eval_type_backport/workflows/Tests/badge.svg)](https://github.com/alexmojaki/eval_type_backport/actions) [![Coverage Status](https://coveralls.io/repos/github/alexmojaki/eval_type_backport/badge.svg)](https://coveralls.io/github/alexmojaki/eval_type_backport) [![Supports Python versions 3.7+, including PyPy](https://img.shields.io/pypi/pyversions/eval_type_backport.svg)](https://pypi.python.org/pypi/eval_type_backport)
+[![Build Status](https://github.com/alexmojaki/eval_type_backport/workflows/Tests/badge.svg)](https://github.com/alexmojaki/eval_type_backport/actions) [![Coverage Status](https://coveralls.io/repos/github/alexmojaki/eval_type_backport/badge.svg)](https://coveralls.io/github/alexmojaki/eval_type_backport) [![Supports Python versions 3.8+, including PyPy](https://img.shields.io/pypi/pyversions/eval_type_backport.svg)](https://pypi.python.org/pypi/eval_type_backport) [![Anaconda's conda-forge channel](https://anaconda.org/conda-forge/eval-type-backport/badges/version.svg)](https://anaconda.org/conda-forge/eval-type-backport)
 
 This is a tiny package providing a replacement for `typing._eval_type` to support newer typing features in older Python versions.
 
 Yes, that's very specific, and yes, `typing._eval_type` is a protected function that you shouldn't normally be using. Really this package is specifically made for https://github.com/pydantic/pydantic/issues/7873.
 
 Specifically, this transforms `X | Y` into `typing.Union[X, Y]`
 and `list[X]` into `typing.List[X]` etc. (for all the types made generic in PEP 585)
 if the original syntax is not supported in the current Python version.
+
+## Install
+
+From PyPI:
+
+```shell
+pip install eval-type-backport
+```
+
+or with Conda:
+
+```shell
+conda install -c conda-forge eval-type-backport
+```
```

### Comparing `eval_type_backport-0.1.3/eval_type_backport/eval_type_backport.py` & `eval_type_backport-0.2.0/eval_type_backport/eval_type_backport.py`

 * *Files 21% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     collections.deque: 'Deque',
     collections.defaultdict: 'DefaultDict',
     collections.abc.Set: 'AbstractSet',
     contextlib.AbstractContextManager: 'ContextManager',
     contextlib.AbstractAsyncContextManager: 'AsyncContextManager',
     **{
         k: k.__name__
-        for k in [
+        for k in (
             collections.OrderedDict,
             collections.Counter,
             collections.ChainMap,
             collections.abc.Awaitable,
             collections.abc.Coroutine,
             collections.abc.AsyncIterable,
             collections.abc.AsyncIterator,
@@ -60,15 +60,15 @@
             collections.abc.MutableSequence,
             collections.abc.MappingView,
             collections.abc.KeysView,
             collections.abc.ItemsView,
             collections.abc.ValuesView,
             re.Pattern,
             re.Match,
-        ]
+        )
     },
 }
 
 
 class BackportTransformer(ast.NodeTransformer):
     """
     Transforms `X | Y` into `typing.Union[X, Y]`
@@ -89,15 +89,20 @@
             assert globalns is not None
             localns = globalns
 
         self.typing_name = f'typing_{uuid.uuid4().hex}'
         self.globalns = globalns
         self.localns = {**localns, self.typing_name: typing}
 
-    def eval_type(self, node: ast.Expression | ast.expr, *, original_ref: typing.ForwardRef | None = None) -> Any:
+    def eval_type(
+        self,
+        node: ast.Expression | ast.expr,
+        *,
+        original_ref: typing.ForwardRef | None = None,
+    ) -> Any:
         if not isinstance(node, ast.Expression):
             node = ast.copy_location(ast.Expression(node), node)
         ref = typing.ForwardRef(ast.dump(node))
         if original_ref:
             for attr in 'is_argument is_class module'.split():
                 attr = f'__forward_{attr}__'
                 if hasattr(original_ref, attr):
@@ -121,15 +126,17 @@
                 # Replace `left | right` with `typing.Union[left, right]`
                 replacement = ast.Subscript(
                     value=ast.Attribute(
                         value=ast.Name(id=self.typing_name, ctx=ast.Load()),
                         attr='Union',
                         ctx=ast.Load(),
                     ),
-                    slice=ast.Index(value=ast.Tuple(elts=[node.left, node.right], ctx=ast.Load())),
+                    slice=ast.Index(
+                        value=ast.Tuple(elts=[node.left, node.right], ctx=ast.Load())
+                    ),
                     ctx=ast.Load(),
                 )
                 return ast.fix_missing_locations(replacement)
 
         return node
 
     if sys.version_info[:2] < (3, 9):
@@ -138,15 +145,16 @@
             node = self.generic_visit(node)
             assert isinstance(node, ast.Subscript)
             try:
                 value_val = self.eval_type(node.value)
             except TypeError:
                 # Likely typing._type_check complaining that the result isn't a type,
                 # e.g. that it's a plain `Literal`.
-                # Either way, this probably isn't one of the new generic types that needs replacing.
+                # Either way, this probably isn't one of the new generic types
+                # that needs replacing.
                 return node
             if value_val not in new_generic_types:
                 return node
             replacement = ast.Subscript(
                 value=ast.Attribute(
                     value=ast.Name(id=self.typing_name, ctx=ast.Load()),
                     attr=new_generic_types[value_val],
@@ -154,14 +162,42 @@
                 ),
                 slice=node.slice,
                 ctx=ast.Load(),
             )
             return ast.fix_missing_locations(replacement)
 
 
+class ForwardRef(typing.ForwardRef, _root=True):  # type: ignore[call-arg,misc]
+    """
+    Like `typing.ForwardRef`, but lets older Python versions use newer typing features.
+    Specifically, when evaluated, this transforms `X | Y` into `typing.Union[X, Y]`
+    and `list[X]` into `typing.List[X]` etc. (for all the types made generic in PEP 585)
+    if the original syntax is not supported in the current Python version.
+    """
+
+    def _evaluate(
+        self,
+        globalns: dict[str, Any] | None,
+        localns: dict[str, Any] | None,
+        recursive_guard: frozenset[str] | None = None,
+    ) -> Any:
+        try:
+            return super()._evaluate(
+                globalns,
+                localns,
+                # assume `recursive_guard` is provided by typing,
+                # so if it's not None, it is supported in typing.ForwardRef
+                *() if recursive_guard is None else (recursive_guard,),
+            )
+        except TypeError as e:
+            if not is_backport_fixable_error(e):
+                raise
+        return _eval_direct(self, globalns, localns)
+
+
 def _eval_direct(
     value: typing.ForwardRef,
     globalns: dict[str, Any] | None = None,
     localns: dict[str, Any] | None = None,
 ):
     tree = ast.parse(value.__forward_arg__, mode='eval')
     transformer = BackportTransformer(globalns, localns)
```

### Comparing `eval_type_backport-0.1.3/eval_type_backport.egg-info/PKG-INFO` & `eval_type_backport-0.2.0/eval_type_backport.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,47 @@
 Metadata-Version: 2.1
-Name: eval-type-backport
-Version: 0.1.3
+Name: eval_type_backport
+Version: 0.2.0
 Summary: Like `typing._eval_type`, but lets older Python versions use newer typing features.
 Home-page: https://github.com/alexmojaki/eval_type_backport
 Author: Alex Hall
 Author-email: alex.mojaki@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 
 # eval_type_backport
 
-[![Build Status](https://github.com/alexmojaki/eval_type_backport/workflows/Tests/badge.svg)](https://github.com/alexmojaki/eval_type_backport/actions) [![Coverage Status](https://coveralls.io/repos/github/alexmojaki/eval_type_backport/badge.svg)](https://coveralls.io/github/alexmojaki/eval_type_backport) [![Supports Python versions 3.7+, including PyPy](https://img.shields.io/pypi/pyversions/eval_type_backport.svg)](https://pypi.python.org/pypi/eval_type_backport)
+[![Build Status](https://github.com/alexmojaki/eval_type_backport/workflows/Tests/badge.svg)](https://github.com/alexmojaki/eval_type_backport/actions) [![Coverage Status](https://coveralls.io/repos/github/alexmojaki/eval_type_backport/badge.svg)](https://coveralls.io/github/alexmojaki/eval_type_backport) [![Supports Python versions 3.8+, including PyPy](https://img.shields.io/pypi/pyversions/eval_type_backport.svg)](https://pypi.python.org/pypi/eval_type_backport) [![Anaconda's conda-forge channel](https://anaconda.org/conda-forge/eval-type-backport/badges/version.svg)](https://anaconda.org/conda-forge/eval-type-backport)
 
 This is a tiny package providing a replacement for `typing._eval_type` to support newer typing features in older Python versions.
 
 Yes, that's very specific, and yes, `typing._eval_type` is a protected function that you shouldn't normally be using. Really this package is specifically made for https://github.com/pydantic/pydantic/issues/7873.
 
 Specifically, this transforms `X | Y` into `typing.Union[X, Y]`
 and `list[X]` into `typing.List[X]` etc. (for all the types made generic in PEP 585)
 if the original syntax is not supported in the current Python version.
+
+## Install
+
+From PyPI:
+
+```shell
+pip install eval-type-backport
+```
+
+or with Conda:
+
+```shell
+conda install -c conda-forge eval-type-backport
+```
```

### Comparing `eval_type_backport-0.1.3/eval_type_backport.egg-info/SOURCES.txt` & `eval_type_backport-0.2.0/eval_type_backport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eval_type_backport-0.1.3/release.sh` & `eval_type_backport-0.2.0/release.sh`

 * *Files identical despite different names*

### Comparing `eval_type_backport-0.1.3/setup.cfg` & `eval_type_backport-0.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -7,27 +7,26 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/alexmojaki/eval_type_backport
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 
 [options]
 packages = eval_type_backport
 zip_safe = False
 include_package_data = True
 setup_requires = setuptools; setuptools_scm[toml]
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.extras_require]
 tests = 
 	pytest
 
 [options.package_data]
 eval_type_backport = py.typed
```

### Comparing `eval_type_backport-0.1.3/tests/test_eval_type_backport.py` & `eval_type_backport-0.2.0/tests/test_eval_type_backport.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,26 @@
+from __future__ import annotations
+
 import collections
 import contextlib
 import re
 import sys
 import typing as t
 
 import pytest
 
-from eval_type_backport import eval_type_backport
+from eval_type_backport import ForwardRef, eval_type_backport
 from eval_type_backport.eval_type_backport import new_generic_types
 
 str((collections, contextlib, re))  # mark these as used (by eval calls)
 
 
+eval_type = t._eval_type  # type: ignore[attr-defined]
+
+
 def eval_kwargs(code: str):
     result = []
     for globalns in (None, globals(), {'t': t}, {}):
         for localns in (None, locals(), {'t': t}, {}):
             for try_default in (True, False):
                 kwargs = t.cast(
                     t.Dict[str, t.Any],
@@ -33,27 +38,29 @@
 
 
 def check_eval(code: str, expected: t.Any):
     if sys.version_info[:2] < (3, 9):
         code_with_list = code.replace('t.List', 'list')
         if code_with_list != code:
             check_eval(code_with_list, expected)
-    ref = t.ForwardRef(code)
+    typing_ref = t.ForwardRef(code)
+    backport_ref = ForwardRef(code)
     for kwargs in eval_kwargs(code):
-        assert eval_type_backport(ref, **kwargs) == expected
-        if sys.version_info >= (3, 10):
-            assert eval(code) == expected
-            assert (
-                t._eval_type(  # type: ignore
-                    ref,
-                    globalns=kwargs['globalns'],
-                    localns=kwargs['localns'],
+        for ref in typing_ref, backport_ref:
+            assert eval_type_backport(ref, **kwargs) == expected
+            if sys.version_info >= (3, 10):
+                assert eval(code) == expected
+                assert (
+                    eval_type(
+                        ref,
+                        globalns=kwargs['globalns'],
+                        localns=kwargs['localns'],
+                    )
+                    == expected
                 )
-                == expected
-            )
 
 
 def test_eval_type_backport():
     check_eval('int', int)
     check_eval('int | str', t.Union[int, str])
     check_eval('int | str | float', t.Union[int, str, float])
     check_eval('int | None', t.Optional[int])
@@ -112,14 +119,16 @@
         '(int + str) | float',
         'int + (str | float)',
         '(int | str) + (float | None)',
         '(int + str) | (float + None)',
     ]:
         with pytest.raises(TypeError):
             check_eval(code, None)
+        with pytest.raises(TypeError):
+            eval_type(ForwardRef(code), None, None)
 
 
 class FooMeta(type):
     def __or__(self, other):
         raise TypeError('foo')
 
 
@@ -147,33 +156,39 @@
 class Bar(metaclass=BarMeta):
     pass
 
 
 def test_working_or():
     check_eval(
         't.List[(Bar | t.List[int]) | (str | Bar)] | float | t.List[Bar]',
-        t.Union[t.List[t.Union[t.Dict[Bar, t.List[int]], t.Dict[str, Bar]]], float, t.List[Bar]],
+        t.Union[
+            t.List[t.Union[t.Dict[Bar, t.List[int]], t.Dict[str, Bar]]],
+            float,
+            t.List[Bar],
+        ],
     )
 
 
 def check_subscript(code: str, expected_old: t.Any):
-    ref = t.ForwardRef(code)
+    typing_ref = t.ForwardRef(code)
+    backport_ref = ForwardRef(code)
     for kwargs in eval_kwargs(code):
-        if sys.version_info >= (3, 9):
-            expected_new = eval(code)
-            assert str(expected_new) == code
-            assert eval_type_backport(ref, **kwargs) == expected_new
-            args = t.get_args(expected_old)
-            origin = t.get_origin(expected_old)
-            assert args == t.get_args(expected_new)
-            assert origin == t.get_origin(expected_new)
-            assert origin[args] == expected_new != expected_old
-            assert t.get_origin(getattr(t, new_generic_types[origin])) == origin
-        else:
-            assert eval_type_backport(ref, **kwargs) == expected_old
+        for ref in typing_ref, backport_ref:
+            if sys.version_info >= (3, 9):
+                expected_new = eval(code)
+                assert str(expected_new) == code
+                assert eval_type_backport(ref, **kwargs) == expected_new
+                args = t.get_args(expected_old)
+                origin = t.get_origin(expected_old)
+                assert args == t.get_args(expected_new)
+                assert origin == t.get_origin(expected_new)
+                assert origin[args] == expected_new != expected_old
+                assert t.get_origin(getattr(t, new_generic_types[origin])) == origin
+            else:
+                assert eval_type_backport(ref, **kwargs) == expected_old
 
 
 def test_subscript():
     check_subscript(
         'tuple[int]',
         t.Tuple[int],
     )
@@ -329,7 +344,16 @@
         're.Pattern[str]',
         t.Pattern[str],
     )
     check_subscript(
         're.Match[str]',
         t.Match[str],
     )
+
+
+def test_copy_forward_ref_attrs():
+    ref = t.ForwardRef(
+        't.ClassVar[int | str]',
+        is_argument=False,
+        **({} if sys.version_info < (3, 9, 8) else {'is_class': True}),
+    )
+    eval_type_backport(ref, globalns=globals(), localns=locals())
```

