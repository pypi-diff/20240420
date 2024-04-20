# Comparing `tmp/ezregex-1.9.6.tar.gz` & `tmp/ezregex-2.0.0.tar.gz`

## Comparing `ezregex-1.9.6.tar` & `ezregex-2.0.0.tar`

### file list

```diff
@@ -1,50 +1,52 @@
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ezregex-1.9.6/.coveragerc
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ezregex-1.9.6/MANIFEST.in
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 ezregex-1.9.6/requirements.txt
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 ezregex-1.9.6/setup.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 ezregex-1.9.6/tox.ini
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ezregex-1.9.6/.github/FUNDING.yml
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 ezregex-1.9.6/.github/workflows/unit-tests.yml
--rw-r--r--   0        0        0    19097 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/EZRegex.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/__init__.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/_dialects.py
--rw-r--r--   0        0        0     7509 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/_docs.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/api.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/api.pyi
--rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/generate.py
--rw-r--r--   0        0        0    24626 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/invert.py
--rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/invert_old.py
--rw-r--r--   0        0        0   337000 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/assets/common_sorted_words.json
--rw-r--r--   0        0        0  4975177 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/assets/sorted_words.json
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/base/__init__.py
--rw-r--r--   0        0        0     9831 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/base/elements.py
--rw-r--r--   0        0        0    12964 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/base/interface.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/javascript/__init__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/javascript/elements.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/javascript/elements.pyi
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/javascript/psuedonymns.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/perl/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/perl/elements.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/perl/elements.pyi
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/perl/psuedonymns.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/python/__init__.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/python/elements.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/python/elements.pyi
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/python/psuedonymns.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/test_EZRegex.py
--rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/test_generate.py
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/test_invert.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/test_javascript.py
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/test_operators.py
--rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/test_python.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/test_replacement.py
--rw-r--r--   0        0        0    37422 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/testing_color_algorithm.ipynb
--rw-r--r--   0        0        0    13448 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/data/groups.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/data/python_regexs.jsonc
--rw-r--r--   0        0        0    18074 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/data/regexs.jsonc
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/data/replacements.jsonc
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 ezregex-1.9.6/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ezregex-1.9.6/LICENSE
--rw-r--r--   0        0        0    53707 2020-02-02 00:00:00.000000 ezregex-1.9.6/README.md
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 ezregex-1.9.6/pyproject.toml
--rw-r--r--   0        0        0    54647 2020-02-02 00:00:00.000000 ezregex-1.9.6/PKG-INFO
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ezregex-2.0.0/.coveragerc
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ezregex-2.0.0/MANIFEST.in
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 ezregex-2.0.0/requirements.txt
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 ezregex-2.0.0/setup.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 ezregex-2.0.0/tox.ini
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ezregex-2.0.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 ezregex-2.0.0/.github/workflows/unit-tests.yml
+-rw-r--r--   0        0        0    17111 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/EZRegex.py
+-rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/EZRegex.pyi
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/__init__.py
+-rw-r--r--   0        0        0     7510 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/_docs.py
+-rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/api.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/api.pyi
+-rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/generate.py
+-rw-r--r--   0        0        0    24721 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/invert.py
+-rw-r--r--   0        0        0    10150 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/invert_old.py
+-rw-r--r--   0        0        0   337000 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/assets/common_sorted_words.json
+-rw-r--r--   0        0        0  4975177 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/assets/sorted_words.json
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/base/__init__.py
+-rw-r--r--   0        0        0    14693 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/base/elements.py
+-rw-r--r--   0        0        0    12964 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/base/interface.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/javascript/JavaScriptEZRegex.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/javascript/__init__.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/javascript/elements.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/javascript/elements.pyi
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/perl/PerlEZRegex.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/perl/__init__.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/perl/elements.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/perl/elements.pyi
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/python/PythonEZRegex.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/python/PythonEZRegex.pyi
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/python/__init__.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/python/elements.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ezregex-2.0.0/ezregex/python/elements.pyi
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 ezregex-2.0.0/tests/test_EZRegex.py
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 ezregex-2.0.0/tests/test_api.py
+-rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 ezregex-2.0.0/tests/test_generate.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 ezregex-2.0.0/tests/test_invert.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 ezregex-2.0.0/tests/test_javascript.py
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 ezregex-2.0.0/tests/test_operators.py
+-rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 ezregex-2.0.0/tests/test_python.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 ezregex-2.0.0/tests/test_replacement.py
+-rw-r--r--   0        0        0    37422 2020-02-02 00:00:00.000000 ezregex-2.0.0/tests/testing_color_algorithm.ipynb
+-rw-r--r--   0        0        0    13448 2020-02-02 00:00:00.000000 ezregex-2.0.0/tests/data/groups.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 ezregex-2.0.0/tests/data/python_regexs.jsonc
+-rw-r--r--   0        0        0    22727 2020-02-02 00:00:00.000000 ezregex-2.0.0/tests/data/regexs.jsonc
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 ezregex-2.0.0/tests/data/replacements.jsonc
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 ezregex-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ezregex-2.0.0/LICENSE
+-rw-r--r--   0        0        0    53562 2020-02-02 00:00:00.000000 ezregex-2.0.0/README.md
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 ezregex-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    54502 2020-02-02 00:00:00.000000 ezregex-2.0.0/PKG-INFO
```

### Comparing `ezregex-1.9.6/setup.py` & `ezregex-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.6/.github/FUNDING.yml` & `ezregex-2.0.0/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.6/.github/workflows/unit-tests.yml` & `ezregex-2.0.0/.github/workflows/unit-tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -24,11 +24,11 @@
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
-        python -m pip install --upgrade pytest jstyleson py_js_runner rich Cope
+        python -m pip install --upgrade pytest jstyleson py_js_runner rich Cope pydantic
     - name: Run Tests
       run: |
         pytest .
```

### Comparing `ezregex-1.9.6/ezregex/EZRegex.py` & `ezregex-2.0.0/ezregex/EZRegex.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,97 +1,61 @@
-# pyright: reportArgumentType = false
 import logging
 import re
-from copy import deepcopy
+from abc import ABC
 from functools import partial
-from typing import Callable, List, Literal
 
 from .api import api
 from .generate import *
 from .invert import invert
-from ._dialects import dialects
 
-# TODO: consider changing addFlags to "outer" or "end" or something
+# TODO: Seperate EZRegex into a "bytes" mode vs "string" mode
+# TODO: consider changing add_flags to "outer" or "end" or something
 # TODO: Seriously consider removing the debug functions
 # TODO: in all the magic functions assert that we're not mixing dialects
-# TODO: delete induvidual deepcopy statements and rerun all the tests to see what ones I can remove
+# TODO: figure out if theres a way to make a "change dialect" function
 
-class EZRegex:
+class EZRegex(ABC):
     """ Represent parts of the Regex syntax. Should not be instantiated by the user directly."""
 
-    def __init__(self,
-                 definition:List[partial[str]]|str|"EZRegex"|partial[str]|list[str],
-                 dialect: str,
-                 sanatize:bool=True,
-                 init:bool=True,
-                 replacement:bool=False,
-                 flags:str='',
-        ):
+    def __init__(self, definition, *, sanatize=True, replacement=False, flags=''):
         """
         The workhorse of the EZRegex library. This represents a regex pattern that can be combined
         with other EZRegexs and strings. Ideally, this should only be called internally, but it should
         still work from the user's end
         """
-
-        if dialect not in dialects.keys():
-            raise ValueError(f'Unsupported dialect `{dialect}` given. Supported dialects are: {list(dialects.keys())}')
-
         # Set attributes like this so the class can remain "immutable", while still being usable
         self.__setattr__('flags', flags, True)
-        # Parse params
-        # Add flags if it's another EZRegex
-        if isinstance(definition, EZRegex):
-            self.__setattr__('flags', definition.flags, True)
-            if definition.dialect != dialect:
-                raise ValueError('Cannot mix regex dialects')
-
-        if isinstance(definition, (str, EZRegex)):
-            definition = [str(definition)]
-        elif not isinstance(definition, (list, tuple)):
-            definition = [definition]
-
         self.__setattr__('_sanatize', sanatize, True)
         self.__setattr__('replacement', replacement, True)
-        # This allows strings in the list now, but they get converted later in this function
-        # self._funcList: list[str|partial[str]|Callable] = list(definition)
-        self.__setattr__('_funcList', list(definition), True)
-        self.__setattr__('dialect', dialect, True)
-        # The dict that has the values
-        self.__setattr__('_dialect_attr', dialects[dialect], True)
-
-
-        # The init parameter is not actually required, but it will make it more
-        # efficient, so we don't have to check that the whole chain is callable
-        if init:
-            # Go through the chain (most likely of length 1) and parse any strings
-            # This is for simplicity when defining all the members
-            for i in range(len(self._funcList)):
-                if isinstance(self._funcList[i], str):
-                    # I *hate* how Python handles lambdas
-                    stringBecauseHatred = deepcopy(self._funcList[i])
-                    self._funcList[i] = lambda cur=...: cur + stringBecauseHatred
-                elif not callable(self._funcList[i]) and self._funcList[i] is not None:
-                    raise ValueError(f"Invalid type {type(self._funcList[i])} passed to EZRegex constructor")
+
+        if isinstance(definition, str):
+            self.__setattr__('_funcList', [lambda cur=...: cur + definition], True)
+        elif callable(definition):
+            self.__setattr__('_funcList', [definition], True)
+        elif isinstance(definition, list):
+            self.__setattr__('_funcList', definition, True)
+
+    # Private functions
+    def _flag_func(self, final:str) -> str:
+        raise NotImplementedError('Subclasses need to implement _flag_func(final)')
 
     def _escape(self, pattern:str):
         """ This function was modified from the one in /usr/lib64/python3.12/re/__init__.py line 255 """
-        _special_chars_map = {i: '\\' + chr(i) for i in self._dialect_attr['escape_chars']}
+        _special_chars_map = {i: '\\' + chr(i) for i in self._escape_chars}
         return pattern.translate(_special_chars_map)
 
-    def _sanitizeInput(self, i, addFlags=False):
+    def _sanitizeInput(self, i, add_flags=False):
         """ Instead of rasising an error if passed a strange datatype, it now trys to cast it to a string """
-        i = deepcopy(i)
-
         # Don't sanatize anything if this is a replacement string
         if self.replacement:
             return str(i)
 
         # If it's another chain, compile it
         if isinstance(i, EZRegex):
-            return i._compile(addFlags=addFlags)
+            return i._compile(add_flags=add_flags)
         # It's a string (so we need to escape it)
         elif isinstance(i, str):
             return self._escape(i)
         # A couple of singletons use bools and None as kwargs, just ignore them and move on
         elif i is None or isinstance(i, bool):
             return i
         # A couple singletons use ints as input, just cast it to a string and don't throw a warning
@@ -101,54 +65,175 @@
         else:
             try:
                 logging.warning(f"Type {type(i)} passed to EZRegex, auto-casting to a string. Special characters will will not be escaped.")
                 return str(i)
             except:
                 raise ValueError(f'Incorrect type {type(i)} given to EZRegex parameter: Must be string or another EZRegex chain.')
 
+    def _compile(self, add_flags=True):
+        regex = ''
+        for func in self._funcList:
+            regex = func(cur=regex) # type: ignore
+
+        # Add the flags
+        if add_flags:
+            regex = self._beginning + regex + self._end
+
+            if len(self.flags):
+                regex = self._flag_func(regex)
+        return regex
+
+    def _copy(self, definition=..., sanatize=..., replacement=..., flags=...):
+        if definition is Ellipsis:
+            definition = self._compile()
+        if sanatize is Ellipsis:
+            sanatize = self._sanatize
+        if replacement is Ellipsis:
+            replacement = self.replacement
+        if flags is Ellipsis:
+            flags = self.flags
+
+        return type(self)(definition, sanatize=sanatize, replacement=replacement, flags=flags)
+
+
+    # Regular functions
+    def str(self):
+        return self.__str__()
+
+    def debug(self):
+        try:
+            from Cope import debug
+        except ImportError:
+            print(f"Compiled ezregex string = {self}")
+        else:
+            debug(self, name='Compiled ezregex string', calls=2)
+        return self
+
+    def copy(self, add_flags=True):
+        try:
+            from clipboard import copy  # type: ignore
+        except ImportError as err:
+            raise ImportError(
+                'Please install the clipboard module in order to auto copy ezregex expressions (i.e. pip install clipboard)'
+            ) from err
+        else:
+            copy(self._compile(add_flags=add_flags))
+
+    def test(self, testString=None, show=True, context=True) -> bool:
+        """ Tests the current regex expression to see if it's in @param testString.
+            Returns the match objects (None if there was no match)
+        """
+        try:
+            from rich import print as rprint
+            from rich.panel import Panel
+            from rich.text import Text
+        except ImportError:
+            raise ImportError("The rich library is required to use the EZRegex.test() method. Try running `pip install rich`")
+
+        # json = self._matchJSON(testString=testString)
+        json = api(self, test_string=testString)
+        if not show:
+            return bool(len(json['matches']))
+
+        st = Text()  # String
+        gt = Text()  # Groups (all the group-related text)
+        defaultColor = 'bold'
+        textColor = ''
+
+        st.append("Testing expression", style=defaultColor)
+        # Add the context line
+        # st.append(f' (from {get_context(get_metadata(2), False, True, True).strip()})', style=defaultColor)
+        st.append(':\n', style=defaultColor)
+
+        # The expression we're testing
+        st.append(f'\t{json["regex"]}\n', style=textColor)
+        st.append("for matches in:\n\t", style=defaultColor)
+
+        # Add the main string
+        for color, background, part in json['parts']:
+            st.append(part, style=color if background is None else f'{color} on {background}')
+        st.append('\n')
+
+        # Add all the matches and groups
+        for m in json['matches']:
+            gt.append('Match = "')
+            for color, background, part in m['match']['parts']:
+                gt.append(part, style=color if background is None else f'{color} on {background}')
+            gt.append('" ')
+            gt.append(f"({m['match']['start']}:{m['match']['end']})", style='italic bright_black')
+            gt.append('\n')
+            if len(m['unnamed groups']):
+                gt.append('Unnamed Groups:\n')
+            for id, group in m['unnamed groups'].items():
+                gt.append(f'\t{id}: "')
+                gt.append(['string'], style=group['color'])
+                gt.append('" ')
+                gt.append(f"({group['start']}:{group['end']})", style='italic bright_black')
+                gt.append('\n')
+            if len(m['named groups']):
+                gt.append('Named Groups:\n')
+            for name, group in m['named groups'].items():
+                gt.append(f'\t{name}: "')
+                gt.append(group['string'], style=group['color'])
+                gt.append('" ')
+                gt.append(f"({group['start']}:{group['end']})", style='italic bright_black')
+                gt.append('\n')
+            gt.append('\n')
+
+        # Assemble everything into a panel
+        rprint(Panel(Text.assemble(*st, '\n', *gt),
+            title='Testing Regex',
+            subtitle=Text('Found\n', style='blue') if len(json['matches'])
+                else Text('Not Found\n', style='red')))  #, border_style='dim green')
+
+        return bool(len(json['matches']))
+
+    def inverse(self, amt=1, **kwargs):
+        """ "Inverts" the current Regex expression to give an example of a string it would match.
+            Useful for debugging purposes. """
+        return '\n'.join([invert(self._compile(), **kwargs) for _ in range(amt)])
+
+    def invert(self, amt=1, **kwargs):
+        return self.inverse(amt, **kwargs)
+
+    # Magic Functions
     def __call__(self, *args, **kwargs):
         """ This should be called by the user to specify the specific parameters of this instance i.e. anyof('a', 'b') """
         # If this is being called without parameters, just compile the chain.
         # If it's being called *with* parameters, then it better be a fundemental
         # member, otherwise that doesn't make any sense.
         if len(self._funcList) > 1:
             if not len(args) and not len(kwargs):
                 return self._compile()
             else:
                 raise TypeError("You're trying to pass parameters to a chain of expressions. That doesn't make any sense. Stop that.")
 
         # Sanatize the arguments
-        args = list(map(self._sanitizeInput if self._sanatize else deepcopy, args))
+        if self._sanatize:
+            args = list(map(self._sanitizeInput, args))
 
         _kwargs = {}
         for key, val in kwargs.items():
-            _kwargs[key] = self._sanitizeInput(val) if self._sanatize else deepcopy(val)
+            _kwargs[key] = self._sanitizeInput(val) if self._sanatize else val
 
-        return EZRegex(
-            [partial(self._funcList[0], *args, **_kwargs)],
-            dialect=self.dialect,
-            init=False,
-            sanatize=self._sanatize,
-            replacement=self.replacement,
-            flags=self.flags
-        )
+        return self._copy([partial(self._funcList[0], *args, **_kwargs)])
 
-    # Magic Functions
-    def __str__(self, addFlags=True):
-        return self._compile(addFlags)
+    def __str__(self, add_flags=True):
+        return self._compile(add_flags)
 
     def __repr__(self):
-        return 'EZRegex("' + self._compile() + '")'
+        return f'{type(self).__name__}("{self}")'
 
     def __eq__(self, thing):
-        return self._sanitizeInput(thing, addFlags=True) == self._compile()
+        """ NOTE: This will return True for equivelent EZRegex expressions of different dialects """
+        return self._sanitizeInput(thing, add_flags=True) == self._compile()
 
     def __mul__(self, amt):
         if amt is Ellipsis:
-            return EZRegex(f'(?{self})*', self.dialect, sanatize=False)
+            return self._copy(f'(?{self})*', sanatize=False)
         rtn = self
         # This isn't optimal, but it's unlikely anyone will use this with large numbers
         for i in range(amt-1):
             # This doesn't work
             # rtn += self
             # But this does??
             rtn = rtn + self
@@ -157,88 +242,78 @@
     def __rmul__(self, amt):
         return self * amt
 
     def __imul__(self, amt):
         return self * amt
 
     def __add__(self, thing):
-        return EZRegex(self._funcList + [partial(lambda cur=...: cur + self._sanitizeInput(thing))],
-            dialect=self.dialect,
-            init=False,
+        return self._copy(
+            self._funcList + [partial(lambda cur=...: cur + self._sanitizeInput(thing))],
             sanatize=self._sanatize or thing._sanatize if isinstance(thing, EZRegex) else self._sanatize,
             replacement=self.replacement or thing.replacement if isinstance(thing, EZRegex) else self.replacement,
             flags=(self.flags + thing.flags) if isinstance(thing, EZRegex) else self.flags
         )
 
     def __radd__(self, thing):
-        return EZRegex([partial(lambda cur=...: self._sanitizeInput(thing) + cur)] + self._funcList,
-            dialect=self.dialect,
-            init=False,
+        return self._copy([partial(lambda cur=...: self._sanitizeInput(thing) + cur)] + self._funcList,
             sanatize=self._sanatize or thing._sanatize if isinstance(thing, EZRegex) else self._sanatize,
             replacement=self.replacement or thing.replacement if isinstance(thing, EZRegex) else self.replacement,
             flags=(self.flags + thing.flags) if isinstance(thing, EZRegex) else self.flags
         )
 
     def __iadd__(self, thing):
-        # return self + self._sanitizeInput(thing)
         return self + thing
 
     def __and__(self, thing):
+        raise NotImplementedError
         logging.warning('The & operator is unstable still. Use each() instead.')
         return EZRegex(fr'(?={self}){thing}', self.dialect, sanatize=False)
 
     def __rand__(self, thing):
+        raise NotImplementedError
         logging.warning('The & operator is unstable still. Use each() instead.')
         return EZRegex(fr'(?={thing}){self}', self.dialect, sanatize=False)
-
     # The shift operators just shadow the add operators
     def __lshift__(self, thing):
         return self.__add__(thing)
 
     def __rlshift__(self, thing):
         return self.__radd__(thing)
 
     def __ilshift__(self, thing):
         return self.__iadd__(thing)
-
     # I don't think right and left shifts should be any different, right?
     def __rshift__(self, thing):
         return self.__add__(thing)
 
     def __rrshift__(self, thing):
         return self.__radd__(thing)
 
     def __irshift__(self, thing):
         return self.__iadd__(thing)
 
     def __invert__(self):
         return self.invert()
 
-    def __not__(self):
-        raise NotImplementedError('The not operator is not implemented. What you probably want is one of anyExcept(), anyCharExcept(), ifNotProceededBy(), or ifNotPreceededBy()')
-
-    def __rnot__(self):
-        raise NotImplementedError('The not operator is not implemented. What you probably want is one of anyExcept(), anyCharExcept(), ifNotProceededBy(), or ifNotPreceededBy()')
-
     def __pos__(self):
         comp = self._compile()
-        return EZRegex(('' if not len(comp) else r'(?:' + comp + r')') + r'+', self.dialect, sanatize=False)
+        return self._copy(('' if not len(comp) else r'(?:' + comp + r')') + r'+', sanatize=False)
 
     def __ror__(self, thing):
-        return EZRegex(f'(?:{self._sanitizeInput(thing)}|{self._compile()})', self.dialect, sanatize=False)
+        return self._copy(f'(?:{self._sanitizeInput(thing)}|{self._compile()})', sanatize=False)
 
     def __or__(self, thing):
         logging.warning('The or operator is unstable and likely to fail, if used more than twice. Use anyof() instead, for now.')
-        return EZRegex(f'(?:{self._compile()}|{self._sanitizeInput(thing)})', self.dialect, sanatize=False)
+        return self._copy(f'(?:{self._compile()}|{self._sanitizeInput(thing)})', sanatize=False)
 
     def __xor__(self, thing):
-        return NotImplemented
+        return NotImplementedError
 
     def __rxor__(self, thing):
-        return NotImplemented
+        return NotImplementedError
 
     def __mod__(self, other):
         """ I would prefer __rmod__(), but it doesn't work on strings, since __mod__() is already specified for string formmating. """
         # I don't need to check this, re will do it for me
         # if not isisntance(other, str):
             # raise TypeError(f"Can't search type {type(other)} ")
         return re.search(other, self._compile())
@@ -250,19 +325,19 @@
         # been called at all. And that means we're one of the basic singletons,
         # because users aren't supposed to instantiate this class directly.
         # THAT means we can use this instance's pointer as a unique identifier.
         else:
             return hash(id(self))
 
     def __contains__(self, thing):
-        assert isinstance(thing, str), "`in` statement can only be used with a string"
+        # assert isinstance(thing, str), "`in` statement can only be used with a string"
         return re.search(self._compile(), thing) is not None
 
-    # I guess this isn't a thing? But it really should be.
     def __rcontains__(self, thing):
+        """ I guess this isn't a thing? But it really should be. """
         assert isinstance(thing, str), "`in` statement can only be used with a string"
         return re.search(self._compile(), thing) is not None
 
     def __getitem__(self, args):
         # digit[2, 3]    # (2, 3)
         # digit[2, ...]  # (2, Ellipsis)
         # digit[2, None] # (2, None)
@@ -286,39 +361,39 @@
             # assert digit[...:'foo'] == digit[None:'foo'] == digit[,'foo'] ==
             pass
         elif type(args) is not tuple or len(args) == 1:
             if type(args) is tuple:
                 args = args[0]
             if args is None or args is Ellipsis or args == 0:
                 # at_least_0(self)
-                return EZRegex(fr'(?:{self._compile()})*', self.dialect, sanatize=False)
+                return self._copy(fr'(?:{self._compile()})*', sanatize=False)
             elif args == 1:
                 # at_least_1(self)
-                return EZRegex(fr'(?:{self._compile()})+', self.dialect, sanatize=False)
+                return self._copy(fr'(?:{self._compile()})+', sanatize=False)
             else:
                 # match_at_least(args, self)
-                return EZRegex(fr'(?:{self._compile()}){{{args},}}', self.dialect, sanatize=False)
+                return self._copy(fr'(?:{self._compile()}){{{args},}}', sanatize=False)
         else:
             start, end = args
             if start is None or start is Ellipsis:
                 # match_at_most(2, self)
-                return EZRegex(fr'(?:{self._compile()}){{0,{end}}}', self.dialect, sanatize=False)
+                return self._copy(fr'(?:{self._compile()}){{0,{end}}}', sanatize=False)
             elif end is None or end is Ellipsis:
                 if start == 0:
                     # at_least_0(self)
-                    return EZRegex(fr'(?:{self._compile()})*', self.dialect, sanatize=False)
+                    return self._copy(fr'(?:{self._compile()})*', sanatize=False)
                 elif start == 1:
                     # at_least_1(self)
-                    return EZRegex(fr'(?:{self._compile()})+', self.dialect, sanatize=False)
+                    return self._copy(fr'(?:{self._compile()})+', sanatize=False)
                 else:
                     # match_at_least(start, self)
-                    return EZRegex(fr'(?:{self._compile()}){{{start},}}', self.dialect, sanatize=False)
+                    return self._copy(fr'(?:{self._compile()}){{{start},}}', sanatize=False)
             else:
                 # match_range(start, end, self)
-                return EZRegex(fr'(?:{self._compile()}){{{start},{end}}}', self.dialect, sanatize=False)
+                return self._copy(fr'(?:{self._compile()}){{{start},{end}}}', sanatize=False)
 
     def __reversed__(self):
         return self.inverse()
 
     def __rich__(self):
         return self._compile()
 
@@ -329,120 +404,7 @@
         if ignore:
             self.__dict__[name] = value
         else:
             raise TypeError('EZRegex objects are immutable')
 
     def __delattr__(self, *args):
         raise TypeError('EZRegex objects are immutable')
-
-    # Regular functions
-    def _compile(self, addFlags=True):
-        regex = ''
-        for func in self._funcList:
-            regex = func(cur=regex) # type: ignore
-
-        # Add the flags
-        if addFlags:
-            regex = self._dialect_attr['beginning'] + regex + self._dialect_attr['end']
-            if len(self.flags):
-                regex = self._dialect_attr['flag_func'](regex, self.flags)
-        return regex
-
-    def compile(self, addFlags=True):
-        return re.compile(self._compile(addFlags))
-
-    def str(self):
-        return self.__str__()
-
-    def debug(self):
-        try:
-            from Cope import debug
-        except ModuleNotFoundError:
-            print(f"Compiled ezregex string = {self}")
-        else:
-            debug(self, name='Compiled ezregex string', calls=2)
-        return self
-
-    def debugStr(self):
-        return self.debug().str()
-
-    def copy(self, addFlags=True):
-        try:
-            from clipboard import copy  # type: ignore
-        except ImportError as err:
-            raise ModuleNotFoundError('Please install the clipboard module in order to auto copy '
-                                      'ezregex expressions (i.e. pip install clipboard)') from err
-        else:
-            copy(self._compile(addFlags=addFlags))
-
-    def test(self, testString=None, show=True, context=True) -> bool:
-        """ Tests the current regex expression to see if it's in @param testString.
-            Returns the match objects (None if there was no match)"""
-        from rich import print as rprint
-        from rich.panel import Panel
-        from rich.text import Text
-
-        # json = self._matchJSON(testString=testString)
-        json = api(self, test_string=testString)
-        if not show:
-            return bool(len(json['matches']))
-
-        st = Text()  # String
-        gt = Text()  # Groups (all the group-related text)
-        defaultColor = 'bold'
-        textColor = ''
-
-        st.append("Testing expression", style=defaultColor)
-        # Add the context line
-        # st.append(f' (from {get_context(get_metadata(2), False, True, True).strip()})', style=defaultColor)
-        st.append(':\n', style=defaultColor)
-
-        # The expression we're testing
-        st.append(f'\t{json["regex"]}\n', style=textColor)
-        st.append("for matches in:\n\t", style=defaultColor)
-
-        # Add the main string
-        for color, background, part in json['parts']:
-            st.append(part, style=color if background is None else f'{color} on {background}')
-        st.append('\n')
-
-        # Add all the matches and groups
-        for m in json['matches']:
-            gt.append('Match = "')
-            for color, background, part in m['match']['parts']:
-                gt.append(part, style=color if background is None else f'{color} on {background}')
-            gt.append('" ')
-            gt.append(f"({m['match']['start']}:{m['match']['end']})", style='italic bright_black')
-            gt.append('\n')
-            if len(m['unnamed groups']):
-                gt.append('Unnamed Groups:\n')
-            for id, group in m['unnamed groups'].items():
-                gt.append(f'\t{id}: "')
-                gt.append(['string'], style=group['color'])
-                gt.append('" ')
-                gt.append(f"({group['start']}:{group['end']})", style='italic bright_black')
-                gt.append('\n')
-            if len(m['named groups']):
-                gt.append('Named Groups:\n')
-            for name, group in m['named groups'].items():
-                gt.append(f'\t{name}: "')
-                gt.append(group['string'], style=group['color'])
-                gt.append('" ')
-                gt.append(f"({group['start']}:{group['end']})", style='italic bright_black')
-                gt.append('\n')
-            gt.append('\n')
-
-        # Assemble everything into a panel
-        rprint(Panel(Text.assemble(*st, '\n', *gt),
-            title='Testing Regex',
-            subtitle=Text('Found\n', style='blue') if len(json['matches'])
-                else Text('Not Found\n', style='red')))  #, border_style='dim green')
-
-        return bool(len(json['matches']))
-
-    def inverse(self, amt=1, **kwargs):
-        """ "Inverts" the current Regex expression to give an example of a string it would match.
-            Useful for debugging purposes. """
-        return '\n'.join([invert(self._compile(), **kwargs) for _ in range(amt)])
-
-    def invert(self, amt=1, **kwargs):
-        return self.inverse(amt, **kwargs)
```

### Comparing `ezregex-1.9.6/ezregex/_docs.py` & `ezregex-2.0.0/ezregex/_docs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import ast
 import os
 from copy import deepcopy
 from pathlib import Path
+
 # from clipboard import copy
 from rich import print
 
 # ASSUMPTION: Groups are designated using the form "Group: <name>\n<optional description>"
 # ASSUMPTION: strings below variables act as the descriptions for those variables
 # ASSUMPTION: There aren't any extraneous variables or functions in the .pyi dialect files
```

### Comparing `ezregex-1.9.6/ezregex/api.py` & `ezregex-2.0.0/ezregex/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,17 @@
     amt += 1
     h, s, v = colorsys.rgb_to_hsv(*map(lambda c: c/255, toRgb(html)))
 
     return [toHtml(*map(lambda c: round(c*255), colorsys.hsv_to_rgb(*((h + ((1/amt) * (i + 1))) % 1.001, (s+s_bias) % 1.001, (v+v_bias) % 1.001)))) for i in range(amt-1)]
 
 
 def api(pattern, replacement_pattern=None, test_string=None, *, replacement_count=0, split_count=0):
+    if type(pattern) is str:
+        raise ValueError(f'The api `pattern` parameter must be of type EZRegex, recieved {type(pattern)}')
+
     # Get an inverse, if nessicary
     if test_string is None:
         test_string = pattern.inverse()
     matches = list(re.finditer(pattern._compile(), test_string))
     found = bool(len(matches))
 
     json = {
```

### Comparing `ezregex-1.9.6/ezregex/api.pyi` & `ezregex-2.0.0/ezregex/api.pyi`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.6/ezregex/generate.py` & `ezregex-2.0.0/ezregex/generate.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.6/ezregex/invert.py` & `ezregex-2.0.0/ezregex/invert.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,416 +1,471 @@
 import json
 import string
 import traceback
+from pathlib import Path
 from random import choice, choices, randint
 from re import search
 from sys import version_info
 from typing import Literal, Union
-from pathlib import Path
+
 from ezregex import *
 
 if version_info.minor <= 10:
     from re import sre_parse as sre  # type: ignore
 else:
     from re import _parser as sre  # type: ignore
 
 # So I can debug this function directly
 if __name__ != '__main__':
     from .invert_old import invertRegex
+else:
+    from ezregex.invert_old import invertRegex
+
 
 with open(Path(__file__).parent / 'assets' / 'common_sorted_words.json') as f:
     words = json.load(f)
 
-# Don't use string.whitespace, because we don't want to use weird difficult to print characters.
-# We want the replacement to be readable.
-_whitespace   = ' '
-_everything   = string.digits + string.ascii_letters + string.punctuation + _whitespace + '_'
-
-def _randWord(length=None, word='lookup'):
-    if length is None:
-        length = randint(3, 9)
-
-    if word == 'random':
-        return ''.join(choices(string.ascii_letters, k=length))
-
-    elif word == 'lookup':
-        try:
-            # The keys are strings, not ints, and I don't feel like fixing it
-            return choice(words[str(length)])
-        except KeyError:
-            return _randWord(length, word='random')
-
-    elif word is None:
-        return 'word'
-
-    else:
-        raise ValueError(f"invalid parameter given for word {word}. Accepted values are either random, lookup, or None")
-
-def _randNumber(length:int, random=False) -> str:
-    if random:
-        return str(randint(0, 10**length))
-    else:
-        return ''.join(map(lambda i: str(i)[-1], range(1, length+1)))
 
 def invert(
     expr:Union[str, 'EZRegex'],
-    words:Literal['lookup', 'random']='lookup',
+    tries:int=10,
+    backend:Literal['re_parser', 'regex', 'xeger', 'sre_yield']=...,
+    words:Literal['lookup', 'random']|None='lookup',
     randomNumbers=False,
     alot=8,
-    tries:int=10,
-    backend:Literal['re_parser', 'regex', 'xeger', 'sre_yield']='re_parser',
-    _verbose=False,
-    # Here for recursion; not to be used
-    _untried=['re_parser', 'regex', 'xeger', 'sre_yield'],
-    _tried=...,
+    verbose=False,
 ) -> str:
+    return Inverter(
+        expr,tries, backend, words, randomNumbers, alot, verbose
+    ).invert()
+
+
+class Inverter:
     """ "Inverts" a regular expression by returning an example of something which is guaruanteed to
         match the passed expression.
         NOTE: This only works on valid Python regular expressions (it will probably mostly work for
             other dialects, but is not guarenteed.)
         expr: The regular expression to invert. Can be a string, or a EZRegex expression
         words: Controls how works are handled. If `random`, words are made of random letters. If `lookup`,
             it looks up valid english words and inserts them to make it more readable.
         randomNumbers: controls whether all numbers are 12345... to a desired length, or if they're
             just random numbers (again, for readability)
-        alot: When given a choice of how many characters to put someone, it inserts a random integer
+        self.alot: When given a choice of how many characters to put someone, it inserts a random integer
             between 1 and `alot`.
         tries: Controls how many times to try to invert the expression before giving up. This is effective,
             because there is an element of randomness involved in inverting the regex given.
         backend: One of ('re_parser', 'regex', 'xeger', 'sre_yield').
             `re_parser` is the default, it uses the build-in parser in the re package to create an AST
                 of the regex
             `regex` uses regular expressions to parse regular expressions, which is as gross as it sounds.
                 It's slightly buggy, but mostly works.
             `xeger` imports the `xeger` pacakge and uses it instead. Xeger inverts work, but are less
                 readable. Must have the `xeger` package installed.
             `sre_yield` imports the `sre_yield` package and uses it instead. I don't think this works
                 right now, and may be significantly slower.
     """
-    expr = str(expr)
-    if _tried is Ellipsis:
-        _tried = tries
-
-    # If we get an error in the actual inversion part, just handle it as though
-    # we generated a bad string that doesn't match, and continue recusing
-    try:
-        match backend:
-            case 'xeger':
-                from xeger import Xeger  # type: ignore
-                rtn = Xeger().xeger(expr)
-            case 'regex':
-                # Tries already gets implemented in this function
-                try:
-                    rtn = invertRegex(expr, 1)
-                except NotImplementedError:
-                    # Handle the error ourselves
-                    rtn = None
-            case 'sre_yield':
-                import sre_yield  # type: ignore
-                for i in sre_yield.AllStrings(expr):
-                    rtn = i
-            case 're_parser':
-                groups = {}
-                def handle(pattern, amt=1, opposite=False):
-                    if _verbose:
-                        print(f'Handling {pattern} * {amt}')
-                    s = ''
-                    for op, args in pattern:
-                        if not opposite:
-                            match op:
-                                case sre.LITERAL:
-                                    s += chr(args) * amt
-                                case sre.NOT_LITERAL:
-                                    almost_everything = list(_everything)
-                                    if chr(args) in almost_everything:
-                                        almost_everything.remove(chr(args))
-                                    # If it's not in there, great!
-                                    s += choice(almost_everything) * amt
-                                case sre.RANGE:
-                                    start, end = args
-                                    s += chr(randint(start, end))
-                                case sre.MAX_REPEAT | sre.MIN_REPEAT:
-                                    min, max, sub = args
-                                    if max is None or max is sre.MAXREPEAT:
-                                        max = randint(min, alot)
-                                    try:
-                                        # If we know we're getting word chars, make a word of it
-                                        if type(sub[0][1][0]) is not int and sub[0][1][0][1] in (sre.CATEGORY_WORD, sre.CATEGORY_UNI_WORD, sre.CATEGORY_LOC_WORD):
-                                            if _verbose: print('Getting a random word')
-                                            s += _randWord(word=words)
-                                        elif type(sub[0][1][0]) is not int and sub[0][1][0][1] in (sre.CATEGORY_DIGIT, sre.CATEGORY_UNI_DIGIT):
-                                            if _verbose: print('Getting whole number')
-                                            s += _randNumber(randint(1, alot), random=randomNumbers)
-                                        else:
-                                            s += handle(sub, randint(min, max) * amt)
-                                    except Exception as err:
-                                        if _verbose:
-                                            print(err)
-                                            print(traceback.format_exc())
-
-                                        s += handle(sub, randint(min, max) * amt)
-                                case sre.ANY:
-                                    for _ in range(amt):
-                                        s += choice(_everything)
-                                case sre.ASSERT:
-                                    type_, sub = args
-                                    if type_ == 1: # ifProcededBy
-                                        s = s + handle(sub, amt)
-                                    elif type_ == -1: # ifPrecededBy
-                                        s += handle(sub, amt)
-                                    else:
-                                        s += handle(sub, amt)
-                                case sre.ASSERT_NOT:
-                                    type_, sub = args
-                                    if type_ == 1: # ifNotProcededBy
-                                        # almost_everything = list(_everything)
-                                        # if chr(args) in almost_everything:
-                                        #     almost_everything.remove(chr(args))
-                                        # # If it's not in there, great!
-                                        # s += choice(almost_everything) * amt
-                                        s += handle(sub, amt, opposite=True)
-                                    if type_ == -1: # ifNotPrecededBy
-                                        s = s + handle(sub, amt, opposite=True)
-                                    # If it needs to be followed by that sequence, simply add that sequence
-                                    else:
-                                        s += handle(sub, amt, opposite=True)
-                                        # s += handle(sub, amt)
-                                case sre.CATEGORY:
-                                    for _ in range(amt):
-                                        match args:
-                                            case sre.CATEGORY_DIGIT | sre.CATEGORY_UNI_DIGIT:
-                                                s += str(randint(0, 10))
-                                            case sre.CATEGORY_LINEBREAK | sre.CATEGORY_UNI_LINEBREAK:
-                                                s += '\n'
-                                            case sre.CATEGORY_NOT_DIGIT | sre.CATEGORY_UNI_NOT_DIGIT:
-                                                s += choice(string.ascii_letters + string.punctuation + _whitespace)
-                                            case sre.CATEGORY_NOT_LINEBREAK | sre.CATEGORY_UNI_NOT_LINEBREAK:
-                                                s += choice(_everything)
-                                            case sre.CATEGORY_NOT_SPACE | sre.CATEGORY_UNI_NOT_SPACE:
-                                                s += choice(string.punctuation + string.ascii_letters + string.digits)
-                                            case sre.CATEGORY_NOT_WORD | sre.CATEGORY_UNI_NOT_WORD | sre.CATEGORY_LOC_NOT_WORD:
-                                                s += choice(string.punctuation + _whitespace)
-                                            case sre.CATEGORY_SPACE | sre.CATEGORY_UNI_SPACE:
-                                                s += ' '
-                                            case sre.CATEGORY_WORD | sre.CATEGORY_UNI_WORD | sre.CATEGORY_LOC_WORD:
-                                                s += choice(string.ascii_letters + '_')
-                                            case _:
-                                                raise NotImplementedError(f'Unknown category given: {args}')
-                                case sre.IN:
-                                    # If this is a pattern like [^abc]
-                                    if args[0][0] is sre.NEGATE:
-                                        # Handle all the args except the negate flag and remove it from the options
-                                        otherthan = handle(args[1:])
-                                        almost_everything = list(_everything)
-                                        for i in otherthan:
-                                            if i in almost_everything:
-                                                almost_everything.remove(i)
-                                        s += choice(almost_everything)
-                                    else:
-                                        s += handle([choice(args)], amt)
-                                case sre.SUBPATTERN: # This handles groups
-                                    group, num, num2, sub = args
-                                    sub_pattern = handle(sub) * amt
-                                    groups[group] = sub_pattern
-                                    s += sub_pattern
-                                case sre.AT:
-                                    if args is sre.AT_BEGINNING_STRING:
-                                        # Whatever comes next better be first
-                                        s = ''
-                                    elif args is sre.AT_END_STRING:
-                                        # Whatever comes next better be last
-                                        return s
-                                    elif args is sre.AT_BEGINNING:
+    def __init__(self,
+        expr:Union[str, 'EZRegex'],
+        tries:int=10,
+        backend:Literal['re_parser', 'regex', 'xeger', 'sre_yield']=...,
+        words:Literal['lookup', 'random']|None='lookup',
+        randomNumbers=False,
+        alot=8,
+        verbose=False,
+    ):
+        self.expr = str(expr)
+        self.words = words
+        self.randomNumbers = randomNumbers
+        self.alot = alot
+        self.tries = tries
+        self.backend = backend
+        self._verbose = verbose
+        self._attempts = {
+            're_parser': 0,
+            'regex': 0,
+            'xeger': 0,
+            'sre_yield': 0,
+        }
+        # Don't use string.whitespace, because we don't want to use weird difficult to print characters.
+        # We want the replacement to be readable.
+        self._whitespace = ' '
+        self._everything = string.digits + string.ascii_letters + string.punctuation + self._whitespace + '_'
+
+        try: from xeger import Xeger  # type: ignore
+        except ImportError: self._xeger = False
+        else: self._xeger = True
+
+        try: import sre_yield  # type: ignore
+        except ImportError: self._sre_yield = False
+        else: self._sre_yield = True
+
+        if backend == 'xeger' and not self._xeger:
+            raise ImportError(f'Requested backend `xeger` not available. Try installing it by running `pip install xeger`')
+
+        if backend == 'sre_yield' and not self._sre_yield:
+            raise ImportError(f'Requested backend `sre_yield` not available. Try installing it by running `pip install sre_yield`')
+
+    def _log(self, s, **kwargs):
+        if self._verbose:
+            print(s, **kwargs)
+
+    def _randWord(self, length=..., word=...) -> str:
+        if word is Ellipsis:
+            word = self.words
+        if length is Ellipsis:
+            length = randint(3, self.alot)
+
+        if word == 'random':
+            return ''.join(choices(string.ascii_letters, k=length))
+
+        elif word == 'lookup':
+            try:
+                # The keys are strings, not ints, and I don't feel like fixing it
+                return choice(words[str(length)])
+            except KeyError:
+                return self._randWord(length, word='random')
+
+        elif word is None:
+            return 'word'
+
+        else:
+            raise ValueError(f"invalid parameter given for word {word}. Accepted values are either random, lookup, or None")
+
+    def _randNumber(self, length=...) -> str:
+        if length is Ellipsis:
+            length = randint(2, self.alot)
+
+        if self.randomNumbers:
+            return str(randint(0, 10**length))
+        else:
+            return ''.join(map(lambda i: str(i)[-1], range(1, length+1)))
+
+    def invert_re_parser(self) -> str | None:
+        self._attempts['re_parser'] += 1
+        self._log(f're_parser attempt #{self._attempts["re_parser"]}...')
+        groups = {}
+        def handle(pattern, amt=1, opposite=False):
+            self._log(f'Handling {pattern} * {amt}')
+            s = ''
+            for op, args in pattern:
+                if not opposite:
+                    match op:
+                        case sre.LITERAL:
+                            s += chr(args) * amt
+                        case sre.NOT_LITERAL:
+                            almost_everything = list(self._everything)
+                            if chr(args) in almost_everything:
+                                almost_everything.remove(chr(args))
+                            # If it's not in there, great!
+                            s += choice(almost_everything) * amt
+                        case sre.RANGE:
+                            start, end = args
+                            s += chr(randint(start, end))
+                        case sre.MAX_REPEAT | sre.MIN_REPEAT:
+                            min, max, sub = args
+                            if max is None or max is sre.MAXREPEAT:
+                                max = randint(min, self.alot)
+                            try:
+                                # If we know we're getting word chars, make a word of it
+                                if type(sub[0][1][0]) is not int and sub[0][1][0][1] in (sre.CATEGORY_WORD, sre.CATEGORY_UNI_WORD, sre.CATEGORY_LOC_WORD):
+                                    self._log('Getting a random word')
+                                    s += self._randWord()
+                                elif type(sub[0][1][0]) is not int and sub[0][1][0][1] in (sre.CATEGORY_DIGIT, sre.CATEGORY_UNI_DIGIT):
+                                    self._log('Getting whole number')
+                                    s += self._randNumber()
+                                else:
+                                    s += handle(sub, randint(min, max) * amt)
+                            except Exception as err:
+                                self._log(err)
+                                self._log(traceback.format_exc())
+
+                                s += handle(sub, randint(min, max) * amt)
+                        case sre.ANY:
+                            for _ in range(amt):
+                                s += choice(self._everything)
+                        case sre.ASSERT:
+                            type_, sub = args
+                            if type_ == 1: # ifProcededBy
+                                s = s + handle(sub, amt)
+                            elif type_ == -1: # ifPrecededBy
+                                s += handle(sub, amt)
+                            else:
+                                s += handle(sub, amt)
+                        case sre.ASSERT_NOT:
+                            type_, sub = args
+                            if type_ == 1: # ifNotProcededBy
+                                # almost_everything = list(self._everything)
+                                # if chr(args) in almost_everything:
+                                #     almost_everything.remove(chr(args))
+                                # # If it's not in there, great!
+                                # s += choice(almost_everything) * amt
+                                s += handle(sub, amt, opposite=True)
+                            if type_ == -1: # ifNotPrecededBy
+                                s = s + handle(sub, amt, opposite=True)
+                            # If it needs to be followed by that sequence, simply add that sequence
+                            else:
+                                s += handle(sub, amt, opposite=True)
+                                # s += handle(sub, amt)
+                        case sre.CATEGORY:
+                            for _ in range(amt):
+                                match args:
+                                    case sre.CATEGORY_DIGIT | sre.CATEGORY_UNI_DIGIT:
+                                        s += str(randint(0, 10))
+                                    case sre.CATEGORY_LINEBREAK | sre.CATEGORY_UNI_LINEBREAK:
                                         s += '\n'
-                                    elif args is sre.AT_END:
+                                    case sre.CATEGORY_NOT_DIGIT | sre.CATEGORY_UNI_NOT_DIGIT:
+                                        s += choice(string.ascii_letters + string.punctuation + self._whitespace)
+                                    case sre.CATEGORY_NOT_LINEBREAK | sre.CATEGORY_UNI_NOT_LINEBREAK:
+                                        s += choice(self._everything)
+                                    case sre.CATEGORY_NOT_SPACE | sre.CATEGORY_UNI_NOT_SPACE:
+                                        s += choice(string.punctuation + string.ascii_letters + string.digits)
+                                    case sre.CATEGORY_NOT_WORD | sre.CATEGORY_UNI_NOT_WORD | sre.CATEGORY_LOC_NOT_WORD:
+                                        s += choice(string.punctuation + self._whitespace)
+                                    case sre.CATEGORY_SPACE | sre.CATEGORY_UNI_SPACE:
+                                        s += ' '
+                                    case sre.CATEGORY_WORD | sre.CATEGORY_UNI_WORD | sre.CATEGORY_LOC_WORD:
+                                        s += choice(string.ascii_letters + '_')
+                                    case _:
+                                        raise NotImplementedError(f'Unknown category given: {args}')
+                        case sre.IN:
+                            # If this is a pattern like [^abc]
+                            if args[0][0] is sre.NEGATE:
+                                # Handle all the args except the negate flag and remove it from the options
+                                otherthan = handle(args[1:])
+                                almost_everything = list(self._everything)
+                                for i in otherthan:
+                                    if i in almost_everything:
+                                        almost_everything.remove(i)
+                                s += choice(almost_everything)
+                            else:
+                                s += handle([choice(args)], amt)
+                        case sre.SUBPATTERN: # This handles groups
+                            group, num, num2, sub = args
+                            sub_pattern = handle(sub) * amt
+                            groups[group] = sub_pattern
+                            s += sub_pattern
+                        case sre.AT:
+                            if args is sre.AT_BEGINNING_STRING:
+                                # Whatever comes next better be first
+                                s = ''
+                            elif args is sre.AT_END_STRING:
+                                # Whatever comes next better be last
+                                return s
+                            elif args is sre.AT_BEGINNING:
+                                s += '\n'
+                            elif args is sre.AT_END:
+                                s += '\n'
+                            elif args is sre.AT_BOUNDARY:
+                                if len(s) and s[-1] in string.digits + string.ascii_letters + '_':
+                                    s += choice(string.punctuation + self._whitespace)
+                                else:
+                                    s += choice(string.digits + string.ascii_letters + '_')
+                            else:
+                                raise NotImplementedError(f'Unknown parameter[s] given for AT op: {args}')
+                        case sre.BRANCH:
+                            something, branches = args
+                            s += handle(choice(branches), amt)
+                        case sre.NEGATE:
+                            s += handle(args, amt, opposite=True)
+                        case sre.GROUPREF:
+                            s += groups[args]
+                        case sre.GROUPREF_EXISTS:
+                            # TODO: This often requires multiple tries to get right
+                            group, trueSub, falseSub = args
+                            s += handle(trueSub if group in groups else falseSub, amt)
+                        case _:
+                            raise NotImplementedError(f'Unknown op {op} given with args {args}')
+                else:
+                    match op:
+                        case sre.LITERAL:
+                            almost_everything = list(self._everything)
+                            if chr(args) in almost_everything:
+                                almost_everything.remove(chr(args))
+                            # If it's not in there, great!
+                            s += choice(almost_everything) * amt
+                        case sre.NOT_LITERAL:
+                            s += chr(args) * amt
+                        case sre.RANGE:
+                            start, end = args
+                            almost_everything = set(self._everything)
+                            almost_everything.difference(map(chr, range(start, end)))
+                            s += choice(list(almost_everything))
+                        case sre.MAX_REPEAT | sre.MIN_REPEAT:
+                            min, max, sub = args
+                            # Adding something that wouldn't match at all is always an option
+                            options = [handle(sub, amt, opposite=True)]
+                            # If a max is specified, then it can't match more than that many
+                            if max is not None and max is not sre.MAXREPEAT:
+                                options.append(handle(sub, amt * (max + randint(1, self.alot))))
+                            # If there's a min (meaning its more than 0), then it can't match
+                            # less than that many
+                            if min >= 1:
+                                # TODO: Potential Error: This doesn't take into account the current amt.
+                                options.append(handle(sub, randint(0, min-1)))
+                            s += choice(options)
+                        case sre.ANY:
+                            # TODO: I think this will fail if given [^.\\n] (or anyExcept(literallyAnything)),
+                            # but also, how DO you handle that?
+                            for _ in range(amt):
+                                # I guess?
+                                s += '\n'
+                        case sre.ASSERT:
+                            # I don't think conditionals are allowed inside a not assert (I think)
+                            type_, sub = args
+                            s += handle(sub, amt, opposite=True)
+                        case sre.ASSERT_NOT:
+                            type_, sub = args
+                            # I *think* this will work?...
+                            s += handle(sub)
+                        case sre.CATEGORY:
+                            for _ in range(amt):
+                                match args:
+                                    case sre.CATEGORY_DIGIT | sre.CATEGORY_UNI_DIGIT:
+                                        s += choice(string.ascii_letters + string.punctuation + self._whitespace)
+                                    case sre.CATEGORY_LINEBREAK | sre.CATEGORY_UNI_LINEBREAK:
+                                        s += choice(self._everything)
+                                    case sre.CATEGORY_NOT_DIGIT | sre.CATEGORY_UNI_NOT_DIGIT:
+                                        s += choice(string.digits)
+                                    case sre.CATEGORY_NOT_LINEBREAK | sre.CATEGORY_UNI_NOT_LINEBREAK:
                                         s += '\n'
-                                    elif args is sre.AT_BOUNDARY:
-                                        if len(s) and s[-1] in string.digits + string.ascii_letters + '_':
-                                            s += choice(string.punctuation + _whitespace)
-                                        else:
-                                            s += choice(string.digits + string.ascii_letters + '_')
-                                    else:
-                                        raise NotImplementedError(f'Unknown parameter[s] given for AT op: {args}')
-                                case sre.BRANCH:
-                                    something, branches = args
-                                    s += handle(choice(branches), amt)
-                                case sre.NEGATE:
-                                    s += handle(args, amt, opposite=True)
-                                case sre.GROUPREF:
-                                    s += groups[args]
-                                case sre.GROUPREF_EXISTS:
-                                    # TODO: This often requires multiple tries to get right
-                                    group, trueSub, falseSub = args
-                                    s += handle(trueSub if group in groups else falseSub, amt)
-                                case _:
-                                    raise NotImplementedError(f'Unknown op {op} given with args {args}')
+                                    case sre.CATEGORY_NOT_SPACE | sre.CATEGORY_UNI_NOT_SPACE:
+                                        s += ' '
+                                    case sre.CATEGORY_NOT_WORD | sre.CATEGORY_UNI_NOT_WORD | sre.CATEGORY_LOC_NOT_WORD:
+                                        s += choice(string.ascii_letters + '_')
+                                    case sre.CATEGORY_SPACE | sre.CATEGORY_UNI_SPACE:
+                                        s += choice(string.punctuation + string.ascii_letters + string.digits)
+                                    case sre.CATEGORY_WORD | sre.CATEGORY_UNI_WORD | sre.CATEGORY_LOC_WORD:
+                                        s += choice(string.punctuation + self._whitespace)
+                                    case _:
+                                        raise NotImplementedError(f'Unknown category given: {args}')
+                        case sre.IN:
+                            # If this is a pattern like [^abc]
+                            if args[0][0] is not sre.NEGATE:
+                                # Handle all the args except the negate flag and remove it from the options
+                                otherthan = handle(args[1:])
+                                almost_everything = list(self._everything)
+                                for i in otherthan:
+                                    if i in almost_everything:
+                                        almost_everything.remove(i)
+                                s += choice(almost_everything)
+                            else:
+                                s += handle([choice(args)], amt)
+                        case sre.SUBPATTERN:
+                            idk, num, num2, sub = args
+                            s += handle(sub, opposite=True) * randint(0, amt)
+                        case None: #sre.AT: # I don't know how to handle this
+                            if args is sre.AT_BEGINNING_STRING:
+                                # Whatever comes next better be first
+                                s = ''
+                            elif args is sre.AT_END_STRING:
+                                # Whatever comes next better be last
+                                return s
+                            elif args is sre.AT_BEGINNING:
+                                s += '\n'
+                            elif args is sre.AT_END:
+                                s += '\n'
+                            elif args is sre.AT_BOUNDARY:
+                                if len(s) and s[-1] in string.digits + string.ascii_letters + '_':
+                                    s += choice(string.punctuation + self._whitespace)
+                                else:
+                                    s += choice(string.digits + string.ascii_letters + '_')
+                            else:
+                                raise NotImplementedError(f'Unknown parameter[s] given for AT op: {args}')
+                        case sre.BRANCH:
+                            something, branches = args
+                            s += handle(choice(branches), amt, opposite=True)
+                        case sre.NEGATE:
+                            s += handle(args, amt)
+                        case sre.GROUPREF:
+                            add = groups[args]
+                            while add == groups[args]:
+                                add = self._randWord()
+                            s += add
+                        case sre.GROUPREF_EXISTS:
+                            group, trueSub, falseSub = args
+                            s += handle(trueSub if group in groups else falseSub, amt, opposite=True)
+                        case _:
+                            raise NotImplementedError(f'Unknown opposite op {op} given with args {args}')
+            return s
+
+        return handle(sre.parse(self.expr))
+
+    def invert_regex(self) -> str | None:
+        self._attempts['regex'] += 1
+        self._log(f'regex attempt #{self._attempts["regex"]}', end='... ')
+        try:
+            rtn = invertRegex(self.expr, 1)
+        except NotImplementedError:
+            pass
+
+    def invert_xeger(self) -> str | None:
+        self._attempts['xeger'] += 1
+        self._log(f'xeger attempt #{self._attempts["xeger"]}', end='... ')
+        if self._xeger:
+            from xeger import Xeger  # type: ignore
+            return Xeger().xeger(self.expr)
+
+    def invert_sre_yield(self) -> str | None:
+        self._attempts['sre_yield'] += 1
+        self._log(f'sre_yield attempt #{self._attempts["sre_yield"]}', end='... ')
+        if self._sre_yield:
+            import sre_yield  # type: ignore
+            for i in sre_yield.AllStrings(self.expr):
+                return i
+
+    def invert(self) -> str:
+        if self.backend is Ellipsis:
+            order = ('re_parser', 'regex', 'sre_yield', 'xeger')
+            for backend in order:
+                while self._attempts[backend] <= self.tries:
+                    rtn = getattr(self, 'invert_' + backend)()
+                    if rtn is not None and search(self.expr, rtn):
+                        self._log(f'Found using {backend}')
+                        return rtn
+                    else:
+                        if rtn is not None:
+                            self._log(f'Successfully inverted pattern, but it was invalid: `{rtn}`')
                         else:
-                            match op:
-                                case sre.LITERAL:
-                                    almost_everything = list(_everything)
-                                    if chr(args) in almost_everything:
-                                        almost_everything.remove(chr(args))
-                                    # If it's not in there, great!
-                                    s += choice(almost_everything) * amt
-                                case sre.NOT_LITERAL:
-                                    s += chr(args) * amt
-                                case sre.RANGE:
-                                    start, end = args
-                                    almost_everything = set(_everything)
-                                    almost_everything.difference(map(chr, range(start, end)))
-                                    s += choice(list(almost_everything))
-                                case sre.MAX_REPEAT | sre.MIN_REPEAT:
-                                    min, max, sub = args
-                                    # Adding something that wouldn't match at all is always an option
-                                    options = [handle(sub, amt, opposite=True)]
-                                    # If a max is specified, then it can't match more than that many
-                                    if max is not None and max is not sre.MAXREPEAT:
-                                        options.append(handle(sub, amt * (max + randint(1, alot))))
-                                    # If there's a min (meaning its more than 0), then it can't match
-                                    # less than that many
-                                    if min >= 1:
-                                        # TODO: Potential Error: This doesn't take into account the current amt.
-                                        options.append(handle(sub, randint(0, min-1)))
-                                    s += choice(options)
-                                case sre.ANY:
-                                    # TODO: I think this will fail if given [^.\\n] (or anyExcept(literallyAnything)),
-                                    # but also, how DO you handle that?
-                                    for _ in range(amt):
-                                        # I guess?
-                                        s += '\n'
-                                case sre.ASSERT:
-                                    # I don't think conditionals are allowed inside a not assert (I think)
-                                    type_, sub = args
-                                    s += handle(sub, amt, opposite=True)
-                                case sre.ASSERT_NOT:
-                                    type_, sub = args
-                                    # I *think* this will work?...
-                                    s += handle(sub)
-                                case sre.CATEGORY:
-                                    for _ in range(amt):
-                                        match args:
-                                            case sre.CATEGORY_DIGIT | sre.CATEGORY_UNI_DIGIT:
-                                                s += choice(string.ascii_letters + string.punctuation + _whitespace)
-                                            case sre.CATEGORY_LINEBREAK | sre.CATEGORY_UNI_LINEBREAK:
-                                                s += choice(_everything)
-                                            case sre.CATEGORY_NOT_DIGIT | sre.CATEGORY_UNI_NOT_DIGIT:
-                                                s += choice(string.digits)
-                                            case sre.CATEGORY_NOT_LINEBREAK | sre.CATEGORY_UNI_NOT_LINEBREAK:
-                                                s += '\n'
-                                            case sre.CATEGORY_NOT_SPACE | sre.CATEGORY_UNI_NOT_SPACE:
-                                                s += ' '
-                                            case sre.CATEGORY_NOT_WORD | sre.CATEGORY_UNI_NOT_WORD | sre.CATEGORY_LOC_NOT_WORD:
-                                                s += choice(string.ascii_letters + '_')
-                                            case sre.CATEGORY_SPACE | sre.CATEGORY_UNI_SPACE:
-                                                s += choice(string.punctuation + string.ascii_letters + string.digits)
-                                            case sre.CATEGORY_WORD | sre.CATEGORY_UNI_WORD | sre.CATEGORY_LOC_WORD:
-                                                s += choice(string.punctuation + _whitespace)
-                                            case _:
-                                                raise NotImplementedError(f'Unknown category given: {args}')
-                                case sre.IN:
-                                    # If this is a pattern like [^abc]
-                                    if args[0][0] is not sre.NEGATE:
-                                        # Handle all the args except the negate flag and remove it from the options
-                                        otherthan = handle(args[1:])
-                                        almost_everything = list(_everything)
-                                        for i in otherthan:
-                                            if i in almost_everything:
-                                                almost_everything.remove(i)
-                                        s += choice(almost_everything)
-                                    else:
-                                        s += handle([choice(args)], amt)
-                                case sre.SUBPATTERN:
-                                    idk, num, num2, sub = args
-                                    s += handle(sub, opposite=True) * randint(0, amt)
-                                case None: #sre.AT: # I don't know how to handle this
-                                    if args is sre.AT_BEGINNING_STRING:
-                                        # Whatever comes next better be first
-                                        s = ''
-                                    elif args is sre.AT_END_STRING:
-                                        # Whatever comes next better be last
-                                        return s
-                                    elif args is sre.AT_BEGINNING:
-                                        s += '\n'
-                                    elif args is sre.AT_END:
-                                        s += '\n'
-                                    elif args is sre.AT_BOUNDARY:
-                                        if len(s) and s[-1] in string.digits + string.ascii_letters + '_':
-                                            s += choice(string.punctuation + _whitespace)
-                                        else:
-                                            s += choice(string.digits + string.ascii_letters + '_')
-                                    else:
-                                        raise NotImplementedError(f'Unknown parameter[s] given for AT op: {args}')
-                                case sre.BRANCH:
-                                    something, branches = args
-                                    s += handle(choice(branches), amt, opposite=True)
-                                case sre.NEGATE:
-                                    s += handle(args, amt)
-                                case sre.GROUPREF:
-                                    add = groups[args]
-                                    while add == groups[args]:
-                                        add = _randWord(word=words)
-                                    s += add
-                                case sre.GROUPREF_EXISTS:
-                                    group, trueSub, falseSub = args
-                                    s += handle(trueSub if group in groups else falseSub, amt, opposite=True)
-                                case _:
-                                    raise NotImplementedError(f'Unknown opposite op {op} given with args {args}')
-                    return s
-
-                rtn = handle(sre.parse(expr))
-    except:
-        rtn = None
-    # I don't know why copying here is necissary. Do parameters act like globals?
-    _untried = _untried.copy()
-    try:
-        _untried.remove(backend)
-    # If we get a ValueError here, it just means that we're retrying the current backend
-    # We can't just remove the _untried parameter in the recuse call in the else
-    # statement below, because then it causes an infinite loop, instead of trying all
-    # the options. This is better.
-    except ValueError: pass
-
-    # Try the current backend `tries` times
-    if rtn is not None and search(expr, rtn):
-        return rtn
-    # If we're out of tries, switch backends
-    elif tries < 0:
-        # If we have options we haven't tried yet
-        if len(_untried):
-            # # tryNext = _untried.pop(0)
-            # The next recursion will remove it for us
-            tryNext = _untried[0]
-            if _verbose:
-                print(f'Not found using {backend}, trying {tryNext}')
-            return invert(expr, words, randomNumbers, alot, _tried, tryNext, _verbose, _untried) # type: ignore
-        # If we've tried everything, go to the error outside the if statement
-    # If we're here, we generated a bad string, but we have more tries
-    else:
-        if _verbose:
-            print(f'Not found using {backend}, retrying')
-
-        return invert(expr, words, randomNumbers, alot, tries, backend, _verbose, _untried, _tried-1) # type: ignore
-
-    raise NotImplementedError(f"Failed to invert pattern `{expr}`. Likely, bad regex was given. "
-        "Otherwise, there\'s a bug in the invert function. You can submit a bug report to "
-        "smartycope@gmail.com, and include the regex you used to get this error. (Failed expr: "
-        f"was `{rtn}`)")
-    return rtn
+                            self._log('Failed to invert pattern')
+
+            self._log(f'Not found using {backend}')
+            msg = (
+                f"Failed to invert pattern `{self.expr}`. Likely, bad regex was given. "
+                "If you think that's not the case, please submit a bug report to "
+                "https://github.com/smartycope/ezregex/issues, and include the regex you used to get this error. "
+            )
+            if not self._xeger or not self._sre_yield:
+                msg += "You can also try installing the extra backends to see if those work:\n"
+            if not self._xeger:
+                msg += "xeger (`pip install xeger`)\n"
+            if not self._sre_yield:
+                msg += "sre_yield (`pip install sre-yield`)"
+
+            raise NotImplementedError(msg)
+        else:
+            while self._attempts[self.backend] <= self.tries:
+                rtn = getattr(self, 'invert_' + self.backend)()
+                if rtn is not None and search(self.expr, rtn):
+                    return rtn
+            raise NotImplementedError(f"Failed to invert pattern `{self.expr}` using the `{self.backend}` backend")
 
 
 if __name__ == '__main__':
     pass
-    # print(invert(r'D(?=AB)C'))  # ASSERT,      1, ifProcededBy
+    # inv = Inverter(r'\w+\d+', verbose=False)
+    # print(inv.invert())
+    # print(invert(r'D(?=AB)C', verbose=True))  # ASSERT,      1, ifProcededBy
     # print(invert(r'D(?!AB)C'))  # ASSERT_NOT,  1, ifNotProcededBy
     # print(invert(r'C(?<=AB)D', _verbose=True)) # ASSERT,     -1, ifPrecededBy
     # print(invert(r'C(?<!AB)D'))   # ASSERT_NOT, -1, ifNotPrecededBy
 
     # print(invert(r'C(?=AB)'))  # ASSERT,      1, ifProcededBy
     # print(invert(r'C(?!AB)'))  # ASSERT_NOT,  1, ifNotProcededBy
     # print(invert(r'(?<=AB)C')) # ASSERT,     -1, ifPrecededBye
     # print(invert(r'(?<!AB)C'))   # ASSERT_NOT, -1, ifNotPrecededBy
 
     # print(invert(r'(?=AB)(?!CD)DC AB(?<=CD) AB(?<!CD)'))
 
     # print(invert(r'[ABC]+(?=D).*$ <.*?>'))
 
     # print(invert(r'\w+test\d+', _verbose=True))
+    # TODO: I think this will fail if given [^.\\n] (or anyExcept(literallyAnything)),
```

### Comparing `ezregex-1.9.6/ezregex/invert_old.py` & `ezregex-2.0.0/ezregex/invert_old.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 def invertRegex(regex:str, tries=10) -> str:
     """ 'Inverts' a regex expression.
         Gives an example of something that would match the given regex
         If tries is positive, it's guarenteed to return an expression that
         correctly matches the given expression, or raise an Error
     """
-    warn('This backend only works most of the time. The default backend is prefered.')
+    # warn('This backend only works most of the time. The default backend is prefered.')
     # So we can compare later and make sure it works
     original = copy(regex)
 
     # So you can pass in an EasyRegex chain
     regex = str(regex)
 
     # Because I hate everyone and this is a stupid bug and it makes NO sense
```

### Comparing `ezregex-1.9.6/ezregex/assets/common_sorted_words.json` & `ezregex-2.0.0/ezregex/assets/common_sorted_words.json`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.6/ezregex/assets/sorted_words.json` & `ezregex-2.0.0/ezregex/assets/sorted_words.json`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.6/ezregex/base/interface.py` & `ezregex-2.0.0/ezregex/base/interface.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.6/ezregex/python/elements.py` & `ezregex-2.0.0/ezregex/python/elements.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # pyright: reportArgumentType = false
 # pyright: reportUndefinedVariable = false
 from ..base import load_base
 from ..EZRegex import EZRegex
+from .PythonEZRegex import PythonEZRegex
 
-globals().update(load_base('python', lambda num_or_name, cur=...: fr'{cur}\g<{num_or_name}>'))
+globals().update(load_base(PythonEZRegex, lambda num_or_name, cur=...: fr'{cur}\g<{num_or_name}>'))
 
 del UNICODE
 
 # Source: http://stackoverflow.com/questions/201323/ddg#201378
 email = raw(r"(?:[a-z0-9!#$%&'*+/=?^_`{|}~-]+(?:\.[a-z0-9!#$%&'*+/=?^_`{|}~-]+)*|\"(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21\x23-\x5b\x5d-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])*\")@(?:(?:[a-z0-9](?:[a-z0-9-]*[a-z0-9])?\.)+[a-z0-9](?:[a-z0-9-]*[a-z0-9])?|\[(?:(?:(2(5[0-5]|[0-4][0-9])|1[0-9][0-9]|[1-9]?[0-9]))\.){3}(?:(2(5[0-5]|[0-4][0-9])|1[0-9][0-9]|[1-9]?[0-9])|[a-z0-9-]*[a-z0-9]:(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21-\x5a\x53-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])+)\])")
 # Source: https://semver.org/ (at the bottom)
 version = raw(r"(?P<major>0|[1-9]\d*)\.(?P<minor>0|[1-9]\d*)\.(?P<patch>0|[1-9]\d*)(?:-(?P<prerelease>(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*)(?:\.(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*))*))?(?:\+(?P<buildmetadata>[0-9a-zA-Z-]+(?:\.[0-9a-zA-Z-]+)*))?")
```

### Comparing `ezregex-1.9.6/tests/test_generate.py` & `ezregex-2.0.0/tests/test_generate.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
-from tests.data.groups import *
-from tests.data.groups import _losers, _winners
 
 from ezregex.generate import *
+from tests.data.groups import *
+from tests.data.groups import _losers, _winners
 
 
 def words(text):
     "All space-separated words in text."
     return Set(text.split())
 
 def phrases(text, sep='/'):
```

### Comparing `ezregex-1.9.6/tests/test_invert.py` & `ezregex-2.0.0/tests/test_invert.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+import threading
+import time
+
 from rich import print as rprint
 from rich.table import Table
-import time
-import threading
 from rich.text import Text
-from ezregex import invert
+
+from ezregex import invert, python
 from ezregex.python import literal
-from ezregex import python
 
 strictness=20
 dontIncludePassed=True
-invertBackend='re_parser'
+invertBackend=...
 invert_tries=5
 import jstyleson
 
 
 def test_invert():
     offset = 2
 
@@ -47,25 +48,15 @@
                     inv = invert(regex, backend=invertBackend, tries=invert_tries)
                     if inv not in regex or not dontIncludePassed:
                         table.add_row(str(offset+(cnt*5)), Text(regex.str()), '`' + inv + '`', Text('passed', style='blue') if inv in regex else Text('failed', style='red'))
             except (Exception, AssertionError) as err:
                 raise ValueError(f'Error @ approx. {__file__}, line {offset+(cnt*4)}: \nregex = `{r[0]}`') #from err#, inv = `{inv}`')
         thread = threading.Thread(target=do_test)
         thread.start()
-        limit = 15
+        limit = 5
         thread.join(timeout=limit)
         assert not thread.is_alive(), f"Invert took too long (>{limit} seconds): `{r[0]}`'"
 
     if len(table.rows):
         with open('summary.txt', 'w') as f:
             rprint(table, file=f)
     assert not len(table.rows)
-
-
-def test_function():
-    start_time = time.time()
-    for i in range(10):  # Change 10 to whatever your loop range is
-        if time.time() - start_time > 5:
-            raise AssertionError("Iteration took too long!")
-        # Your loop code here
-
-test_function()
```

### Comparing `ezregex-1.9.6/tests/test_javascript.py` & `ezregex-2.0.0/tests/test_javascript.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # import jsonc
-from ezregex import javascript
+# from ezregex import javascript
 # import js2py
-import py_js_runner
 import jstyleson
+import py_js_runner
 from Cope import RedirectStd
 
+
 def runjs(js):
     pass
     # with RedirectStd(stdout=):
     #     py_js_runner.javascript().run(js)
 
 
 def test_javascript():
```

### Comparing `ezregex-1.9.6/tests/test_operators.py` & `ezregex-2.0.0/tests/test_operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 
 import pytest
+
 from ezregex import *
 
 strictness=20
 dontIncludePassed=True
 invertBackend='re_parser'
 invert_tries=1
 offset = 2
```

### Comparing `ezregex-1.9.6/tests/test_python.py` & `ezregex-2.0.0/tests/test_python.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,46 @@
-from ezregex import python
 import jstyleson
+import pytest
+
 import ezregex as er
-from ezregex import EZRegex
 from ezregex import *
+from ezregex import EZRegex, python
+
 
 def test_python():
-    offset = 2
+    try:
+        with open('tests/data/regexs.jsonc') as f:
+            regexs = jstyleson.load(f)
+
+        for cnt, r in enumerate(regexs):
+            regex_str, match, dontMatch = r
+            regex = eval(regex_str, python.__dict__)
+            # try:
+            if match:
+                for m in match:
+                    assert m in regex, f"{r[0]} does not match '{m}'"
+            if dontMatch:
+                for m in dontMatch:
+                    assert m not in regex, f"{r[0]} DOES match '{m}'"
+    except Exception as err:
+        raise AssertionError(f'pattern = `{regex_str}`, match = `{match}`, dontMatch = `{dontMatch}`') from err
+
+
+def test_no_empty_strings():
+    with pytest.raises(ValueError):
+        str(group('', name='i') + optional(digit))
+
+    with pytest.raises(ValueError):
+        str(match_max(group('')))
 
-    with open('tests/data/regexs.jsonc') as f:
-        regexs = jstyleson.load(f)
+    with pytest.raises(ValueError):
+        str(amt(2, ''))
 
-    for cnt, r in enumerate(regexs):
-        regex_str, match, dontMatch = r
-        regex = eval(regex_str, python.__dict__)
-        # try:
-        if match:
-            for m in match:
-                assert m in regex, f"{r[0]} does not match '{m}'"
-        if dontMatch:
-            for m in dontMatch:
-                assert m not in regex, f"{r[0]} DOES match '{m}'"
-        # except Exception as err:
-            # raise ValueError(f'pattern = `{r[0]}`, match = `{match}`, dontMatch = `{dontMatch}`') from err
+    with pytest.raises(ValueError):
+        str(group('abc', name=''))
 
 
 def test_any_of():
     # """ _any_of_func """
     assert er.anyof('aiLmsux', split=True, chars=True)._compile(False) == "[aiLmsux]", \
         f"Was supposed to be '[aiLmsux]', was actually '{er.anyof('aiLmsux', split=True, chars=True)._compile(False)}'"
     # assert er.anyof('aiLmsux', split=False, chars=True)._compile(False) == Error, \
@@ -73,29 +88,30 @@
 
 
 def test_misc():
     """ Just threw a bunch of stuff in here for now, I need to move it elsewhere eventually """
     a = word + ow
     # b = stuff + UNICODE
     c = IGNORECASE + '9'
-    assert a + c == word + ow + IGNORECASE + '9', f"{a + b + c} != {word + ow + IGNORECASE + '9'}"
+    assert a + c == word + ow + IGNORECASE + '9', f"{a + c} != {word + ow + IGNORECASE + '9'}"
 
-    a = str(EZRegex(r'\s+', 'python'))
-    b = str(EZRegex(raw(r'\s+'), 'python'))
+    a = str(PythonEZRegex(r'\s+'))
+    with pytest.raises(TypeError):
+        b = str(PythonEZRegex(raw(r'\s+')))
     c = r'\s+'
     d = str(raw(r'\s+'))
     # e = str(whitespace + matchMax)
-    assert a == b == c == d, f'\na: {a}\n b: {b}\n c: {c}\n d: {d}\n e: {e}'
+    assert a == c == d, f'\na: {a}\n c: {c}\n d: {d}\n e: {e}'
     # assert (word + ow + anything + ':').test('word    d:', show=False)
     # assert not (word + ow + anything + ':').test('word', show=False)
     assert 'word    d:' in (word + ow + anything + ':')
 
     test = word + chunk
     test += word
     assert str(test) == str(word + chunk + word), f"{str(test)} != {str(word + chunk + word)}"
     assert test == word + chunk + word
     assert either('(' + word + ')', '.') == either(er.literal('(') + word() + er.literal(')'), '.'), f"{either('(' + word + ')', '.')} != {either(er.literal('(') + word() + er.literal(')'), '.')}"
-    assert str(ifFollowedBy(word)) == r'(?=\w+)'
+    assert str(er.ifFollowedBy(word)) == r'(?=\w+)'
 
     #TODO: assert (word + ow + anything + ':') in 'word    d:'
     #TODO: assert (word + ow + anything + ':') not in 'word'
     assert str(word) == r'\w+', f'{word}'
```

### Comparing `ezregex-1.9.6/tests/test_replacement.py` & `ezregex-2.0.0/tests/test_replacement.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 
-from ezregex import python
-from ezregex import *
-
 import jstyleson
 
+from ezregex import *
+from ezregex import python
+
 
 def test_replacement():
     offset = 2
     with open('tests/data/replacements.jsonc') as f:
         replacements = jstyleson.load(f)
 
     for pattern_str, repl_str, s, ans in replacements:
```

### Comparing `ezregex-1.9.6/tests/testing_color_algorithm.ipynb` & `ezregex-2.0.0/tests/testing_color_algorithm.ipynb`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.6/tests/data/groups.py` & `ezregex-2.0.0/tests/data/groups.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.6/tests/data/regexs.jsonc` & `ezregex-2.0.0/tests/data/regexs.jsonc`

 * *Files 21% similar despite different names*

```diff
@@ -346,15 +346,15 @@
     [
         "lineEndsWith('a')",
         ["lklkjfda", "sdf 8 a", "a", "sdf\na", "sdfse\nsdafsda", "sdfa\nsdf"],
         ["asdfds", "sd fd"]
     ],
     [
         "literal('test')",
-        ["test", " sdfstestsdfs",],
+        ["test", " sdfstestsdfs"],
         ["te st",]
     ],
     [
         "underscore",
         ["_",],
         ["a test", "test ", "\ntest\n", "\ntest", "test\n"]
     ],
@@ -595,15 +595,389 @@
     ],
     [
         "group('pattern', name='i') + optional(digit) + match_max(group('me')) + amt(2, 'mhmm')",
         [],
         []
     ],
     [
-        "group('', name='i') + optional(digit) + match_max(group('')) + amt(2, '')",
+        "string_starts_with",
+        [],
+        []
+    ],
+    [
+        "string_ends_with",
+        [],
+        []
+    ],
+    [
+        "line_starts_with",
+        [],
+        []
+    ],
+    [
+        "line_ends_with",
+        [],
+        []
+    ],
+    [
+        "word_boundary",
+        [],
+        []
+    ],
+    [
+        "not_word_boundary",
+        [],
+        []
+    ],
+    [
+        "tab",
+        [],
+        []
+    ],
+    [
+        "space",
+        [],
+        []
+    ],
+    [
+        "space_or_tab",
+        [],
+        []
+    ],
+    [
+        "new_line",
+        [],
+        []
+    ],
+    [
+        "carriage_return",
+        [],
+        []
+    ],
+    [
+        "quote",
+        [],
+        []
+    ],
+    [
+        "vertical_tab",
+        [],
+        []
+    ],
+    [
+        "form_feed",
+        [],
+        []
+    ],
+    [
+        "comma",
+        [],
+        []
+    ],
+    [
+        "period",
+        [],
+        []
+    ],
+    [
+        "underscore",
+        [],
+        []
+    ],
+    [
+        "any_between('a', 'b')",
+        [],
+        []
+    ],
+    [
+        "not_whitespace",
+        [],
+        []
+    ],
+    [
+        "not_digit",
+        [],
+        []
+    ],
+    [
+        "not_word",
+        [],
+        []
+    ],
+    [
+        "whitespace",
+        [],
+        []
+    ],
+    [
+        "whitechunk",
+        [],
+        []
+    ],
+    [
+        "digit",
+        [],
+        []
+    ],
+    [
+        "number",
+        [],
+        []
+    ],
+    [
+        "word",
+        [],
+        []
+    ],
+    [
+        "word_char",
+        [],
+        []
+    ],
+    [
+        "anything",
+        [],
+        []
+    ],
+    [
+        "chunk",
+        [],
+        []
+    ],
+    [
+        "uppercase",
+        [],
+        []
+    ],
+    [
+        "lowercase",
+        [],
+        []
+    ],
+    [
+        "letter",
+        [],
+        []
+    ],
+    [
+        "hex_digit",
+        [],
+        []
+    ],
+    [
+        "oct_digit",
+        [],
+        []
+    ],
+    [
+        "punctuation",
+        [],
+        []
+    ],
+    [
+        "controller",
+        [],
+        []
+    ],
+    [
+        "printable",
+        [],
+        []
+    ],
+    [
+        "printable_and_space",
+        [],
+        []
+    ],
+    [
+        "alpha_num",
+        [],
+        []
+    ],
+    // TODO
+    // [
+    //     "unicode('pi')",
+    //     [],
+    //     []
+    // ],
+    [
+        "match_max(digit)",
+        [],
+        []
+    ],
+    [
+        "match_num(2, digit)",
+        [],
+        []
+    ],
+    [
+        "match_more_than(2, digit)",
+        [],
+        []
+    ],
+    [
+        "match_at_least(2, digit)",
+        [],
+        []
+    ],
+    [
+        "match_at_most(2, digit)",
+        [],
+        []
+    ],
+    [
+        "match_range(2, 4, digit)",
+        [],
+        []
+    ],
+    [
+        "at_least_one(digit)",
+        [],
+        []
+    ],
+    [
+        "at_least_none(digit)",
+        [],
+        []
+    ],
+    [
+        "optional(digit)",
+        [],
+        []
+    ],
+    [
+        "either(digit, word)",
+        [],
+        []
+    ],
+    [
+        "any_of(digit, word, 'a', 'b')",
+        [],
+        []
+    ],
+    [
+        "any_char_except('abcd')",
+        [],
+        []
+    ],
+    [
+        "if_proceded_by(digit)",
+        [],
+        []
+    ],
+    [
+        "if_not_proceded_by(digit)",
+        [],
+        []
+    ],
+    [
+        "if_preceded_by(digit)",
+        [],
+        []
+    ],
+    [
+        "if_not_preceded_by(digit)",
+        [],
+        []
+    ],
+    [
+        "if_enclosed_with('|', digit)",
+        [],
+        []
+    ],
+    [
+        "group(digit)",
+        [],
+        []
+    ],
+    [
+        "passive_group(digit)",
+        [],
+        []
+    ],
+    // TODO
+    // [
+    //     "'earlier_group(''",
+    //     [],
+    //     []
+    // ],
+    // TODO
+    // [
+    //     "'if_exists'",
+    //     [],
+    //     []
+    // ],
+    [
+        "literally_anything",
+        [],
+        []
+    ],
+    [
+        "signed",
+        [],
+        []
+    ],
+    [
+        "unsigned",
+        [],
+        []
+    ],
+    [
+        "plain_float",
+        [],
+        []
+    ],
+    [
+        "full_float",
+        [],
+        []
+    ],
+    [
+        "int_or_float",
+        [],
+        []
+    ],
+    [
+        "ow",
+        [],
+        []
+    ],
+    [
+        "is_exactly(digit)",
+        [],
+        []
+    ],
+    [
+        "literal('this')",
+        [],
+        []
+    ],
+    [
+        "digit + ASCII",
+        [],
+        []
+    ],
+    [
+        "digit + DOTALL",
+        [],
+        []
+    ],
+    [
+        "digit + IGNORECASE",
+        [],
+        []
+    ],
+    // TODO: This is for bytes only programs or something?...
+    // [
+    //     "digit + LOCALE",
+    //     [],
+    //     []
+    // ],
+    [
+        "digit + MULTILINE",
         [],
         []
     ],
     // ('foo' + ((chunk + 'here' + chunk) & (chunk + anyOf('this', 'that') + chunk)) + 'bar',  ('fooum here there that bar', 'foo that there here bar'),               None),
     // ('foo' + ((chunk + 'here' + chunk) & (chunk + anyOf('this', 'that') + chunk) & (chunk + 'the' + chunk)) + 'bar',  ('fooum the here there that bar', 'foo that there thehere bar'), ('fooum here there that bar', 'foo that there here bar')),
     // (,                                                                                    (,),                                                                    (,)),
     // (word_boundary + word_char[...,3] + wordBoundary,                                       ('yes', 'hey', 'sup', 'thi'),                                           ('none', 'no', 'foo3', '333', 'jar_')), // This does what it's supposed to do, but doesn't search correctly, as far as I understand it
```

### Comparing `ezregex-1.9.6/tests/data/replacements.jsonc` & `ezregex-2.0.0/tests/data/replacements.jsonc`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.6/.gitignore` & `ezregex-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.6/LICENSE` & `ezregex-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.6/README.md` & `ezregex-2.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,16 @@
     - Next on the roadmap, technically importable, but not implemented yet
 
 If you know a particular flavor of regex and would like to contribute, feel free to read the [developer documentation](#developer-documentation) and make a pull request! If you would like one that's not implemented yet, you can also add a [github issue](https://github.com/smartycope/ezregex/issues).
 
 ## Documentation
 ### Notes and Gotchas
 - The different Regular Expression dialects don't all have the same features, and those features don't all work the same way. I've tried to standardize these as best I can and use reasonable names for all the elements. If you're confused by something not working as expected, be sure to understand how your language specifically handles regular expressions.
-- When using the Python `re` library, functions like re.search() and re.sub() don't accept EZRegex patterns as valid regex. Be sure to either call .str() (or cast it to a string) or .compile() (to compile to an re.Pattern) when passing to those. Also, be careful to call the function on the entire pattern: chunk + whitespace.str() is not the same as (chunk + whitespace).str().
+- All the functions in the Python `re` library (`search`, `match`, `sub`, etc.) are implemented in the Python EZRegex dialect, and act identically to their equivalents. If you still want to use the Python `re` library, note that functions like `search` and `sub` don't accept EZRegex patterns as valid regex. Be sure to either call .str() (or cast it to a string) or .compile() (to compile to an re.Pattern) when passing to those. Using the member functions however, will be more efficient, as EZRegex caches the compiled re.Pattern internally.
+- Be careful to call functions on the entire pattern: chunk + whitespace.str() is not the same as (chunk + whitespace).str().
 - In regular regex, a lot of random things capture groups for no apparent reason. All regexes in EZRegex intentionally capture passively, so to capture any groups, use group(), with the optional `name` parameter.
 - All EZRegexs (except for `raw`) auto-sanitize strings given to them, so there's no need to escape characters or use r strings. This *does* mean, however, that you cannot pass actual regex strings to any of them, as they'll think you're talking about it literally (unless you want that, of course). To include already written regex strings, use `raw`
 - Note that I have camelCase and snake_case versions of each of the functions, because I waver back and forth between which I like better. Both versions function identically.
 - The `InputType` can accept strings, other EZRegexs, or entire sequences of EZRegex patterns. It can also accept things that can be cast to a string, but it will warn you when it does, so it's better to cast to a string yourself.
 - The `invert` function can accept any regular expression, not just EZRegex expressions, if you want to use it independently of the rest of the library.
 
 <!-- Start of generated docs -->
@@ -1017,57 +1018,54 @@
     - This automatically calls re.search() for you and returns the match object (or None). Use like this: `(digit * 2) % '99 beers on the wall'`
 - `~`
     - This inverts the expression, equivalent to calling the .invert() method
 </details>
 
 ## Developer Documentation
 ### The EZRegex class
-Everything relies on the EZRegex class. EZRegex shouldn't be instantiated by the user, as each dialect defines their own EZRegex elements specific to that dialect (more on that later). Each element represents a fundamental part of the Regular Expression syntax for that language, as well as less-fundemental common combinations for convenience (like email and float).
+Everything relies on the EZRegex class. EZRegex shouldn't be instantiated by the user, as each dialect subclasses the EZRegex class and defines their own elements specific to that dialect (more on that later). Each element represents a fundamental part of the Regular Expression syntax for that language, as well as less-fundemental common combinations for convenience (like email and float).
 
 EZRegex can accept a string or a function to define how it's supposed to interact with the current "chain" of elements. If it's a string, it just adds it to the end. If it's a function, it can accept any positional or named parameters, but has to accept `cur=...` as the last parameter (it's complicated). The `cur` parameter is the current regular expression chain, as a string. What's returned becomes the new `cur` parameter of the next element, or, if there is no next element, the final regex. That way you can add to the front or back of an expression, and you can change what exactly gets added to the current expression based on other parameters.
 
 The EZRegex class has operators overloaded so you can combine them in intuitive ways and call them by intuitive names.
 
 ### Typing & Linting
 The updated method of doing this is to define all the EZRegex elements of a dialect in `elements.py`, and then add type hints and doc strings in the `elements.pyi` file. EZRegex elements that accept parameters are typed as functions (even though they're not), for both convenience for the user when using linter, and to give documentation in an easier way. EZRegex elements that don't accept parameters should be typed as EZRegex, and given documentation as a string on the line below it. This is *slightly* non-standard, but linters support it, as well as my documentation generator script, which parses the .pyi files. The elements can also be seperated into groups in the .pyi files by using `"Group: \<group name\>\n\<group description\>"`, which also gets parsed by the documentation script. The groups aren't used in the actual library, but are helpful in seperating the documentation, as well as used in [ezregex.org](http://ezregex.org)
 
 ### Dialects
-Because most regex dialects *are* 90% identical, a hidden "base" dialect is implemented, but it works a bit differently. It has an `elements.py` file, but it defines all the elements as a dict in the form of {"element_name": {"keyword": "arguements"}}. It then has a `load_dialect()` function, which is the only thing importable from it. The reason it's done this way is because `dialect` is a required parameter of the EZRegex constructor, so `load_dialect()` takes a `dialect` parameter, and constructs the base elements from it's dict and returns a new dict of initialized elements to be dumped into the global scope of the dialect. The `elements.py` file of a specific dialect can then remove any elements that it doesn't support (using the `del` keyword) and add/overwrite any it does support.
+Because most regex dialects *are* 90% identical, a parent EZRegex class implements most of the applicable logic, and a hidden "base" dialect is implemented, but works a bit differently. It has an `elements.py` file, but it defines all the elements as a dict in the form of {"element_name": {"keyword": "arguements"}}. It then has a `load_dialect()` function, which is the only thing importable from it. The reason it's done this way is because most elements, though identical in different dialects, have to be the appropriate dialect subclass. `load_dialect()` takes the dialect type as a parameter, and instantiates the base elements from it's dict and returns a new dict of initialized elements to be dumped into the global scope of the dialect. The `elements.py` file of a specific dialect can then remove any elements that it doesn't support (using the `del` keyword) and add/overwrite any it does support, or that work differently.
 
-There's also a _dialects.py file that has a dict for each dialect to describe the dialect-specific behavior of the EZRegex class, for example, in the JavaScript dialect, /'s are added to the beginning and end of the pattern, and flags are handled differently in each dialect. This has to be implemented directly into the EZRegex class. The dicts *would* be in the dialect folders themselves, but that causes all sorts of circular dependancies, so they're all just in the _dialects.py file.
+Each subclass of EZRegex must implement a few options to describe the dialect-specific behavior of the EZRegex class, for example, in the JavaScript dialect, /'s are added to the beginning and end of the pattern, and flags are handled differently in each dialect. This has to be implemented directly into the EZRegex subclass.
 
-There's 4 parts to the dicts in the _dialects.py file:
+There's 4 parts that are required:
 - `beginning` and `end`
     - Plain strings which describe what to tack onto the beginning and end of the compiled pattern (but *before* flags are added)
 - `flag_func`
-    - A function that gets called with `final`, which is the final compiled pattern *with* `beginning` and `end` attached, and `flags`, which is a string of all the flags applied to the pattern. Internally, the flags are single digits, because flags usually are. They get passed to this function as a single string, which can be parsed and modified if necissary (it usually isn't)
+    - An abstract function that gets called with `final`, which is the final compiled pattern *with* `beginning` and `end` attached, and `flags`, which is a string of all the flags applied to the pattern. Internally, the flags are single digits, because flags usually are. They get passed to this function as a single string, which can be parsed and modified if necissary (it usually isn't)
 - `escape_chars`
     - The characters that need to be escaped. Should be a byte string (i.e. b'...')
 
 ### Inverting
 There's actually 2 algorithms implemented for "inverting" regexs. The old algorithm regexs the regexs in a specific order to replace parts one at a time. This is just as nasty and horrifying as it sounds. Dispite it being a terrible, *terrible* solution, I actually got it to work decently well.
 
 Later, when I was reading up on abstract syntax trees, and scrolling around on PyPi, I realized that Python has one built in, and that it's available to use. I reimplemented the whole algorithm to instead parse the AST given by the built-in re lexer, and wrote my own parser on top of it, which works *much* better.
 
 Along the way, I also discovered, deep in the corners of the internet, 2 other Python libraries which do almost the same thing: `xeger` (regex backwards), and `sre_yield`. `xeger` technically works, however it tends to include unprintable characters, so it's output isn't very readable. `sre_yeild` is better, but it can be very slow, and is not quite the use case I'm going for. My invert algorithm is meant to be a debugging tool (though it doubles well for a testing tool), so it does things like detecting words (as opposed to seperate word characters) and inserts actual words, and doing the same for numbers and inserting `12345...`, as well as a couple other enhancements.
 
-### Tests
-Tests for a while now have just been in a single `tests.py` file, which was a giant pile of all the tests. I'm currently moving to use pytest. There's a `regexs.json` file (and a `replacements.json` file) that have a bunch of regexs, along with things they're supposed to match, and things they're not supposed to match, for testing.
-
 ## Installation
 EZRegex is distributed on [PyPI](https://pypi.org) as a universal wheel and is available on Linux, macOS and Windows and supports Python 3.10+ and PyPy.
 
 ```bash
 pip install ezregex
 ```
 
 The import name is the same as the package name:
 ```python
 import ezregex as er
 ```
 
 ## Todo
-See [the todo](todo.txt). I'm slowly moving these to [GitHub issues](https://github.com/smartycope/ezregex/issues), but for now, they're mostly still there
+See the [GitHub Issue Page](https://github.com/smartycope/ezregex/issues)
 
 
 ## License
 EZRegex is distributed under the [MIT License](https://choosealicense.com/licenses/mit)
```

#### html2text {}

```diff
@@ -64,19 +64,23 @@
 [developer documentation](#developer-documentation) and make a pull request! If
 you would like one that's not implemented yet, you can also add a [github
 issue](https://github.com/smartycope/ezregex/issues). ## Documentation ###
 Notes and Gotchas - The different Regular Expression dialects don't all have
 the same features, and those features don't all work the same way. I've tried
 to standardize these as best I can and use reasonable names for all the
 elements. If you're confused by something not working as expected, be sure to
-understand how your language specifically handles regular expressions. - When
-using the Python `re` library, functions like re.search() and re.sub() don't
-accept EZRegex patterns as valid regex. Be sure to either call .str() (or cast
-it to a string) or .compile() (to compile to an re.Pattern) when passing to
-those. Also, be careful to call the function on the entire pattern: chunk +
+understand how your language specifically handles regular expressions. - All
+the functions in the Python `re` library (`search`, `match`, `sub`, etc.) are
+implemented in the Python EZRegex dialect, and act identically to their
+equivalents. If you still want to use the Python `re` library, note that
+functions like `search` and `sub` don't accept EZRegex patterns as valid regex.
+Be sure to either call .str() (or cast it to a string) or .compile() (to
+compile to an re.Pattern) when passing to those. Using the member functions
+however, will be more efficient, as EZRegex caches the compiled re.Pattern
+internally. - Be careful to call functions on the entire pattern: chunk +
 whitespace.str() is not the same as (chunk + whitespace).str(). - In regular
 regex, a lot of random things capture groups for no apparent reason. All
 regexes in EZRegex intentionally capture passively, so to capture any groups,
 use group(), with the optional `name` parameter. - All EZRegexs (except for
 `raw`) auto-sanitize strings given to them, so there's no need to escape
 characters or use r strings. This *does* mean, however, that you cannot pass
 actual regex strings to any of them, as they'll think you're talking about it
@@ -531,88 +535,83 @@
 This will work like the + operator, but they can be out of order. Like an and
 operation. - `|` - Coming soon! This will work like an or operation, which will
 work just like any_of() - `%` - This automatically calls re.search() for you
 and returns the match object (or None). Use like this: `(digit * 2) % '99 beers
 on the wall'` - `~` - This inverts the expression, equivalent to calling the
 .invert() method ## Developer Documentation ### The EZRegex class Everything
 relies on the EZRegex class. EZRegex shouldn't be instantiated by the user, as
-each dialect defines their own EZRegex elements specific to that dialect (more
-on that later). Each element represents a fundamental part of the Regular
-Expression syntax for that language, as well as less-fundemental common
-combinations for convenience (like email and float). EZRegex can accept a
-string or a function to define how it's supposed to interact with the current
-"chain" of elements. If it's a string, it just adds it to the end. If it's a
-function, it can accept any positional or named parameters, but has to accept
-`cur=...` as the last parameter (it's complicated). The `cur` parameter is the
-current regular expression chain, as a string. What's returned becomes the new
-`cur` parameter of the next element, or, if there is no next element, the final
-regex. That way you can add to the front or back of an expression, and you can
-change what exactly gets added to the current expression based on other
-parameters. The EZRegex class has operators overloaded so you can combine them
-in intuitive ways and call them by intuitive names. ### Typing & Linting The
-updated method of doing this is to define all the EZRegex elements of a dialect
-in `elements.py`, and then add type hints and doc strings in the `elements.pyi`
-file. EZRegex elements that accept parameters are typed as functions (even
-though they're not), for both convenience for the user when using linter, and
-to give documentation in an easier way. EZRegex elements that don't accept
-parameters should be typed as EZRegex, and given documentation as a string on
-the line below it. This is *slightly* non-standard, but linters support it, as
-well as my documentation generator script, which parses the .pyi files. The
-elements can also be seperated into groups in the .pyi files by using `"Group:
-\\n\"`, which also gets parsed by the documentation script. The groups aren't
-used in the actual library, but are helpful in seperating the documentation, as
-well as used in [ezregex.org](http://ezregex.org) ### Dialects Because most
-regex dialects *are* 90% identical, a hidden "base" dialect is implemented, but
-it works a bit differently. It has an `elements.py` file, but it defines all
-the elements as a dict in the form of {"element_name": {"keyword":
-"arguements"}}. It then has a `load_dialect()` function, which is the only
-thing importable from it. The reason it's done this way is because `dialect` is
-a required parameter of the EZRegex constructor, so `load_dialect()` takes a
-`dialect` parameter, and constructs the base elements from it's dict and
-returns a new dict of initialized elements to be dumped into the global scope
-of the dialect. The `elements.py` file of a specific dialect can then remove
-any elements that it doesn't support (using the `del` keyword) and add/
-overwrite any it does support. There's also a _dialects.py file that has a dict
-for each dialect to describe the dialect-specific behavior of the EZRegex
-class, for example, in the JavaScript dialect, /'s are added to the beginning
-and end of the pattern, and flags are handled differently in each dialect. This
-has to be implemented directly into the EZRegex class. The dicts *would* be in
-the dialect folders themselves, but that causes all sorts of circular
-dependancies, so they're all just in the _dialects.py file. There's 4 parts to
-the dicts in the _dialects.py file: - `beginning` and `end` - Plain strings
-which describe what to tack onto the beginning and end of the compiled pattern
-(but *before* flags are added) - `flag_func` - A function that gets called with
-`final`, which is the final compiled pattern *with* `beginning` and `end`
-attached, and `flags`, which is a string of all the flags applied to the
-pattern. Internally, the flags are single digits, because flags usually are.
-They get passed to this function as a single string, which can be parsed and
-modified if necissary (it usually isn't) - `escape_chars` - The characters that
-need to be escaped. Should be a byte string (i.e. b'...') ### Inverting There's
-actually 2 algorithms implemented for "inverting" regexs. The old algorithm
-regexs the regexs in a specific order to replace parts one at a time. This is
-just as nasty and horrifying as it sounds. Dispite it being a terrible,
-*terrible* solution, I actually got it to work decently well. Later, when I was
-reading up on abstract syntax trees, and scrolling around on PyPi, I realized
-that Python has one built in, and that it's available to use. I reimplemented
-the whole algorithm to instead parse the AST given by the built-in re lexer,
-and wrote my own parser on top of it, which works *much* better. Along the way,
-I also discovered, deep in the corners of the internet, 2 other Python
-libraries which do almost the same thing: `xeger` (regex backwards), and
-`sre_yield`. `xeger` technically works, however it tends to include unprintable
-characters, so it's output isn't very readable. `sre_yeild` is better, but it
-can be very slow, and is not quite the use case I'm going for. My invert
-algorithm is meant to be a debugging tool (though it doubles well for a testing
-tool), so it does things like detecting words (as opposed to seperate word
-characters) and inserts actual words, and doing the same for numbers and
-inserting `12345...`, as well as a couple other enhancements. ### Tests Tests
-for a while now have just been in a single `tests.py` file, which was a giant
-pile of all the tests. I'm currently moving to use pytest. There's a
-`regexs.json` file (and a `replacements.json` file) that have a bunch of
-regexs, along with things they're supposed to match, and things they're not
-supposed to match, for testing. ## Installation EZRegex is distributed on
-[PyPI](https://pypi.org) as a universal wheel and is available on Linux, macOS
-and Windows and supports Python 3.10+ and PyPy. ```bash pip install ezregex ```
-The import name is the same as the package name: ```python import ezregex as er
-``` ## Todo See [the todo](todo.txt). I'm slowly moving these to [GitHub
-issues](https://github.com/smartycope/ezregex/issues), but for now, they're
-mostly still there ## License EZRegex is distributed under the [MIT License]
-(https://choosealicense.com/licenses/mit)
+each dialect subclasses the EZRegex class and defines their own elements
+specific to that dialect (more on that later). Each element represents a
+fundamental part of the Regular Expression syntax for that language, as well as
+less-fundemental common combinations for convenience (like email and float).
+EZRegex can accept a string or a function to define how it's supposed to
+interact with the current "chain" of elements. If it's a string, it just adds
+it to the end. If it's a function, it can accept any positional or named
+parameters, but has to accept `cur=...` as the last parameter (it's
+complicated). The `cur` parameter is the current regular expression chain, as a
+string. What's returned becomes the new `cur` parameter of the next element,
+or, if there is no next element, the final regex. That way you can add to the
+front or back of an expression, and you can change what exactly gets added to
+the current expression based on other parameters. The EZRegex class has
+operators overloaded so you can combine them in intuitive ways and call them by
+intuitive names. ### Typing & Linting The updated method of doing this is to
+define all the EZRegex elements of a dialect in `elements.py`, and then add
+type hints and doc strings in the `elements.pyi` file. EZRegex elements that
+accept parameters are typed as functions (even though they're not), for both
+convenience for the user when using linter, and to give documentation in an
+easier way. EZRegex elements that don't accept parameters should be typed as
+EZRegex, and given documentation as a string on the line below it. This is
+*slightly* non-standard, but linters support it, as well as my documentation
+generator script, which parses the .pyi files. The elements can also be
+seperated into groups in the .pyi files by using `"Group: \\n\"`, which also
+gets parsed by the documentation script. The groups aren't used in the actual
+library, but are helpful in seperating the documentation, as well as used in
+[ezregex.org](http://ezregex.org) ### Dialects Because most regex dialects
+*are* 90% identical, a parent EZRegex class implements most of the applicable
+logic, and a hidden "base" dialect is implemented, but works a bit differently.
+It has an `elements.py` file, but it defines all the elements as a dict in the
+form of {"element_name": {"keyword": "arguements"}}. It then has a
+`load_dialect()` function, which is the only thing importable from it. The
+reason it's done this way is because most elements, though identical in
+different dialects, have to be the appropriate dialect subclass. `load_dialect
+()` takes the dialect type as a parameter, and instantiates the base elements
+from it's dict and returns a new dict of initialized elements to be dumped into
+the global scope of the dialect. The `elements.py` file of a specific dialect
+can then remove any elements that it doesn't support (using the `del` keyword)
+and add/overwrite any it does support, or that work differently. Each subclass
+of EZRegex must implement a few options to describe the dialect-specific
+behavior of the EZRegex class, for example, in the JavaScript dialect, /'s are
+added to the beginning and end of the pattern, and flags are handled
+differently in each dialect. This has to be implemented directly into the
+EZRegex subclass. There's 4 parts that are required: - `beginning` and `end` -
+Plain strings which describe what to tack onto the beginning and end of the
+compiled pattern (but *before* flags are added) - `flag_func` - An abstract
+function that gets called with `final`, which is the final compiled pattern
+*with* `beginning` and `end` attached, and `flags`, which is a string of all
+the flags applied to the pattern. Internally, the flags are single digits,
+because flags usually are. They get passed to this function as a single string,
+which can be parsed and modified if necissary (it usually isn't) -
+`escape_chars` - The characters that need to be escaped. Should be a byte
+string (i.e. b'...') ### Inverting There's actually 2 algorithms implemented
+for "inverting" regexs. The old algorithm regexs the regexs in a specific order
+to replace parts one at a time. This is just as nasty and horrifying as it
+sounds. Dispite it being a terrible, *terrible* solution, I actually got it to
+work decently well. Later, when I was reading up on abstract syntax trees, and
+scrolling around on PyPi, I realized that Python has one built in, and that
+it's available to use. I reimplemented the whole algorithm to instead parse the
+AST given by the built-in re lexer, and wrote my own parser on top of it, which
+works *much* better. Along the way, I also discovered, deep in the corners of
+the internet, 2 other Python libraries which do almost the same thing: `xeger`
+(regex backwards), and `sre_yield`. `xeger` technically works, however it tends
+to include unprintable characters, so it's output isn't very readable.
+`sre_yeild` is better, but it can be very slow, and is not quite the use case
+I'm going for. My invert algorithm is meant to be a debugging tool (though it
+doubles well for a testing tool), so it does things like detecting words (as
+opposed to seperate word characters) and inserts actual words, and doing the
+same for numbers and inserting `12345...`, as well as a couple other
+enhancements. ## Installation EZRegex is distributed on [PyPI](https://
+pypi.org) as a universal wheel and is available on Linux, macOS and Windows and
+supports Python 3.10+ and PyPy. ```bash pip install ezregex ``` The import name
+is the same as the package name: ```python import ezregex as er ``` ## Todo See
+the [GitHub Issue Page](https://github.com/smartycope/ezregex/issues) ##
+License EZRegex is distributed under the [MIT License](https://
+choosealicense.com/licenses/mit)
```

### Comparing `ezregex-1.9.6/pyproject.toml` & `ezregex-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.6/PKG-INFO` & `ezregex-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: ezregex
-Version: 1.9.6
+Version: 2.0.0
 Summary: A readable and intuitive way to generate Regular Expressions
 Project-URL: Documentation, https://github.com/smartycope/ezregex?tab=readme-ov-file#documentation
 Project-URL: Issues, https://github.com/smartycope/ezregex/issues
 Project-URL: Source, https://github.com/smartycope/ezregex
 Project-URL: Official Website, https://ezregex.org
 Author-email: Copeland Carter <smartycope@gmail.com>
 License-Expression: MIT
@@ -170,15 +170,16 @@
     - Next on the roadmap, technically importable, but not implemented yet
 
 If you know a particular flavor of regex and would like to contribute, feel free to read the [developer documentation](#developer-documentation) and make a pull request! If you would like one that's not implemented yet, you can also add a [github issue](https://github.com/smartycope/ezregex/issues).
 
 ## Documentation
 ### Notes and Gotchas
 - The different Regular Expression dialects don't all have the same features, and those features don't all work the same way. I've tried to standardize these as best I can and use reasonable names for all the elements. If you're confused by something not working as expected, be sure to understand how your language specifically handles regular expressions.
-- When using the Python `re` library, functions like re.search() and re.sub() don't accept EZRegex patterns as valid regex. Be sure to either call .str() (or cast it to a string) or .compile() (to compile to an re.Pattern) when passing to those. Also, be careful to call the function on the entire pattern: chunk + whitespace.str() is not the same as (chunk + whitespace).str().
+- All the functions in the Python `re` library (`search`, `match`, `sub`, etc.) are implemented in the Python EZRegex dialect, and act identically to their equivalents. If you still want to use the Python `re` library, note that functions like `search` and `sub` don't accept EZRegex patterns as valid regex. Be sure to either call .str() (or cast it to a string) or .compile() (to compile to an re.Pattern) when passing to those. Using the member functions however, will be more efficient, as EZRegex caches the compiled re.Pattern internally.
+- Be careful to call functions on the entire pattern: chunk + whitespace.str() is not the same as (chunk + whitespace).str().
 - In regular regex, a lot of random things capture groups for no apparent reason. All regexes in EZRegex intentionally capture passively, so to capture any groups, use group(), with the optional `name` parameter.
 - All EZRegexs (except for `raw`) auto-sanitize strings given to them, so there's no need to escape characters or use r strings. This *does* mean, however, that you cannot pass actual regex strings to any of them, as they'll think you're talking about it literally (unless you want that, of course). To include already written regex strings, use `raw`
 - Note that I have camelCase and snake_case versions of each of the functions, because I waver back and forth between which I like better. Both versions function identically.
 - The `InputType` can accept strings, other EZRegexs, or entire sequences of EZRegex patterns. It can also accept things that can be cast to a string, but it will warn you when it does, so it's better to cast to a string yourself.
 - The `invert` function can accept any regular expression, not just EZRegex expressions, if you want to use it independently of the rest of the library.
 
 <!-- Start of generated docs -->
@@ -1038,57 +1039,54 @@
     - This automatically calls re.search() for you and returns the match object (or None). Use like this: `(digit * 2) % '99 beers on the wall'`
 - `~`
     - This inverts the expression, equivalent to calling the .invert() method
 </details>
 
 ## Developer Documentation
 ### The EZRegex class
-Everything relies on the EZRegex class. EZRegex shouldn't be instantiated by the user, as each dialect defines their own EZRegex elements specific to that dialect (more on that later). Each element represents a fundamental part of the Regular Expression syntax for that language, as well as less-fundemental common combinations for convenience (like email and float).
+Everything relies on the EZRegex class. EZRegex shouldn't be instantiated by the user, as each dialect subclasses the EZRegex class and defines their own elements specific to that dialect (more on that later). Each element represents a fundamental part of the Regular Expression syntax for that language, as well as less-fundemental common combinations for convenience (like email and float).
 
 EZRegex can accept a string or a function to define how it's supposed to interact with the current "chain" of elements. If it's a string, it just adds it to the end. If it's a function, it can accept any positional or named parameters, but has to accept `cur=...` as the last parameter (it's complicated). The `cur` parameter is the current regular expression chain, as a string. What's returned becomes the new `cur` parameter of the next element, or, if there is no next element, the final regex. That way you can add to the front or back of an expression, and you can change what exactly gets added to the current expression based on other parameters.
 
 The EZRegex class has operators overloaded so you can combine them in intuitive ways and call them by intuitive names.
 
 ### Typing & Linting
 The updated method of doing this is to define all the EZRegex elements of a dialect in `elements.py`, and then add type hints and doc strings in the `elements.pyi` file. EZRegex elements that accept parameters are typed as functions (even though they're not), for both convenience for the user when using linter, and to give documentation in an easier way. EZRegex elements that don't accept parameters should be typed as EZRegex, and given documentation as a string on the line below it. This is *slightly* non-standard, but linters support it, as well as my documentation generator script, which parses the .pyi files. The elements can also be seperated into groups in the .pyi files by using `"Group: \<group name\>\n\<group description\>"`, which also gets parsed by the documentation script. The groups aren't used in the actual library, but are helpful in seperating the documentation, as well as used in [ezregex.org](http://ezregex.org)
 
 ### Dialects
-Because most regex dialects *are* 90% identical, a hidden "base" dialect is implemented, but it works a bit differently. It has an `elements.py` file, but it defines all the elements as a dict in the form of {"element_name": {"keyword": "arguements"}}. It then has a `load_dialect()` function, which is the only thing importable from it. The reason it's done this way is because `dialect` is a required parameter of the EZRegex constructor, so `load_dialect()` takes a `dialect` parameter, and constructs the base elements from it's dict and returns a new dict of initialized elements to be dumped into the global scope of the dialect. The `elements.py` file of a specific dialect can then remove any elements that it doesn't support (using the `del` keyword) and add/overwrite any it does support.
+Because most regex dialects *are* 90% identical, a parent EZRegex class implements most of the applicable logic, and a hidden "base" dialect is implemented, but works a bit differently. It has an `elements.py` file, but it defines all the elements as a dict in the form of {"element_name": {"keyword": "arguements"}}. It then has a `load_dialect()` function, which is the only thing importable from it. The reason it's done this way is because most elements, though identical in different dialects, have to be the appropriate dialect subclass. `load_dialect()` takes the dialect type as a parameter, and instantiates the base elements from it's dict and returns a new dict of initialized elements to be dumped into the global scope of the dialect. The `elements.py` file of a specific dialect can then remove any elements that it doesn't support (using the `del` keyword) and add/overwrite any it does support, or that work differently.
 
-There's also a _dialects.py file that has a dict for each dialect to describe the dialect-specific behavior of the EZRegex class, for example, in the JavaScript dialect, /'s are added to the beginning and end of the pattern, and flags are handled differently in each dialect. This has to be implemented directly into the EZRegex class. The dicts *would* be in the dialect folders themselves, but that causes all sorts of circular dependancies, so they're all just in the _dialects.py file.
+Each subclass of EZRegex must implement a few options to describe the dialect-specific behavior of the EZRegex class, for example, in the JavaScript dialect, /'s are added to the beginning and end of the pattern, and flags are handled differently in each dialect. This has to be implemented directly into the EZRegex subclass.
 
-There's 4 parts to the dicts in the _dialects.py file:
+There's 4 parts that are required:
 - `beginning` and `end`
     - Plain strings which describe what to tack onto the beginning and end of the compiled pattern (but *before* flags are added)
 - `flag_func`
-    - A function that gets called with `final`, which is the final compiled pattern *with* `beginning` and `end` attached, and `flags`, which is a string of all the flags applied to the pattern. Internally, the flags are single digits, because flags usually are. They get passed to this function as a single string, which can be parsed and modified if necissary (it usually isn't)
+    - An abstract function that gets called with `final`, which is the final compiled pattern *with* `beginning` and `end` attached, and `flags`, which is a string of all the flags applied to the pattern. Internally, the flags are single digits, because flags usually are. They get passed to this function as a single string, which can be parsed and modified if necissary (it usually isn't)
 - `escape_chars`
     - The characters that need to be escaped. Should be a byte string (i.e. b'...')
 
 ### Inverting
 There's actually 2 algorithms implemented for "inverting" regexs. The old algorithm regexs the regexs in a specific order to replace parts one at a time. This is just as nasty and horrifying as it sounds. Dispite it being a terrible, *terrible* solution, I actually got it to work decently well.
 
 Later, when I was reading up on abstract syntax trees, and scrolling around on PyPi, I realized that Python has one built in, and that it's available to use. I reimplemented the whole algorithm to instead parse the AST given by the built-in re lexer, and wrote my own parser on top of it, which works *much* better.
 
 Along the way, I also discovered, deep in the corners of the internet, 2 other Python libraries which do almost the same thing: `xeger` (regex backwards), and `sre_yield`. `xeger` technically works, however it tends to include unprintable characters, so it's output isn't very readable. `sre_yeild` is better, but it can be very slow, and is not quite the use case I'm going for. My invert algorithm is meant to be a debugging tool (though it doubles well for a testing tool), so it does things like detecting words (as opposed to seperate word characters) and inserts actual words, and doing the same for numbers and inserting `12345...`, as well as a couple other enhancements.
 
-### Tests
-Tests for a while now have just been in a single `tests.py` file, which was a giant pile of all the tests. I'm currently moving to use pytest. There's a `regexs.json` file (and a `replacements.json` file) that have a bunch of regexs, along with things they're supposed to match, and things they're not supposed to match, for testing.
-
 ## Installation
 EZRegex is distributed on [PyPI](https://pypi.org) as a universal wheel and is available on Linux, macOS and Windows and supports Python 3.10+ and PyPy.
 
 ```bash
 pip install ezregex
 ```
 
 The import name is the same as the package name:
 ```python
 import ezregex as er
 ```
 
 ## Todo
-See [the todo](todo.txt). I'm slowly moving these to [GitHub issues](https://github.com/smartycope/ezregex/issues), but for now, they're mostly still there
+See the [GitHub Issue Page](https://github.com/smartycope/ezregex/issues)
 
 
 ## License
 EZRegex is distributed under the [MIT License](https://choosealicense.com/licenses/mit)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: ezregex Version: 1.9.6 Summary: A readable and
+Metadata-Version: 2.1 Name: ezregex Version: 2.0.0 Summary: A readable and
 intuitive way to generate Regular Expressions Project-URL: Documentation,
 https://github.com/smartycope/ezregex?tab=readme-ov-file#documentation Project-
 URL: Issues, https://github.com/smartycope/ezregex/issues Project-URL: Source,
 https://github.com/smartycope/ezregex Project-URL: Official Website, https://
 ezregex.org Author-email: Copeland Carter
 gmail.com> License-Expression: MIT License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
@@ -77,19 +77,23 @@
 [developer documentation](#developer-documentation) and make a pull request! If
 you would like one that's not implemented yet, you can also add a [github
 issue](https://github.com/smartycope/ezregex/issues). ## Documentation ###
 Notes and Gotchas - The different Regular Expression dialects don't all have
 the same features, and those features don't all work the same way. I've tried
 to standardize these as best I can and use reasonable names for all the
 elements. If you're confused by something not working as expected, be sure to
-understand how your language specifically handles regular expressions. - When
-using the Python `re` library, functions like re.search() and re.sub() don't
-accept EZRegex patterns as valid regex. Be sure to either call .str() (or cast
-it to a string) or .compile() (to compile to an re.Pattern) when passing to
-those. Also, be careful to call the function on the entire pattern: chunk +
+understand how your language specifically handles regular expressions. - All
+the functions in the Python `re` library (`search`, `match`, `sub`, etc.) are
+implemented in the Python EZRegex dialect, and act identically to their
+equivalents. If you still want to use the Python `re` library, note that
+functions like `search` and `sub` don't accept EZRegex patterns as valid regex.
+Be sure to either call .str() (or cast it to a string) or .compile() (to
+compile to an re.Pattern) when passing to those. Using the member functions
+however, will be more efficient, as EZRegex caches the compiled re.Pattern
+internally. - Be careful to call functions on the entire pattern: chunk +
 whitespace.str() is not the same as (chunk + whitespace).str(). - In regular
 regex, a lot of random things capture groups for no apparent reason. All
 regexes in EZRegex intentionally capture passively, so to capture any groups,
 use group(), with the optional `name` parameter. - All EZRegexs (except for
 `raw`) auto-sanitize strings given to them, so there's no need to escape
 characters or use r strings. This *does* mean, however, that you cannot pass
 actual regex strings to any of them, as they'll think you're talking about it
@@ -544,88 +548,83 @@
 This will work like the + operator, but they can be out of order. Like an and
 operation. - `|` - Coming soon! This will work like an or operation, which will
 work just like any_of() - `%` - This automatically calls re.search() for you
 and returns the match object (or None). Use like this: `(digit * 2) % '99 beers
 on the wall'` - `~` - This inverts the expression, equivalent to calling the
 .invert() method ## Developer Documentation ### The EZRegex class Everything
 relies on the EZRegex class. EZRegex shouldn't be instantiated by the user, as
-each dialect defines their own EZRegex elements specific to that dialect (more
-on that later). Each element represents a fundamental part of the Regular
-Expression syntax for that language, as well as less-fundemental common
-combinations for convenience (like email and float). EZRegex can accept a
-string or a function to define how it's supposed to interact with the current
-"chain" of elements. If it's a string, it just adds it to the end. If it's a
-function, it can accept any positional or named parameters, but has to accept
-`cur=...` as the last parameter (it's complicated). The `cur` parameter is the
-current regular expression chain, as a string. What's returned becomes the new
-`cur` parameter of the next element, or, if there is no next element, the final
-regex. That way you can add to the front or back of an expression, and you can
-change what exactly gets added to the current expression based on other
-parameters. The EZRegex class has operators overloaded so you can combine them
-in intuitive ways and call them by intuitive names. ### Typing & Linting The
-updated method of doing this is to define all the EZRegex elements of a dialect
-in `elements.py`, and then add type hints and doc strings in the `elements.pyi`
-file. EZRegex elements that accept parameters are typed as functions (even
-though they're not), for both convenience for the user when using linter, and
-to give documentation in an easier way. EZRegex elements that don't accept
-parameters should be typed as EZRegex, and given documentation as a string on
-the line below it. This is *slightly* non-standard, but linters support it, as
-well as my documentation generator script, which parses the .pyi files. The
-elements can also be seperated into groups in the .pyi files by using `"Group:
-\\n\"`, which also gets parsed by the documentation script. The groups aren't
-used in the actual library, but are helpful in seperating the documentation, as
-well as used in [ezregex.org](http://ezregex.org) ### Dialects Because most
-regex dialects *are* 90% identical, a hidden "base" dialect is implemented, but
-it works a bit differently. It has an `elements.py` file, but it defines all
-the elements as a dict in the form of {"element_name": {"keyword":
-"arguements"}}. It then has a `load_dialect()` function, which is the only
-thing importable from it. The reason it's done this way is because `dialect` is
-a required parameter of the EZRegex constructor, so `load_dialect()` takes a
-`dialect` parameter, and constructs the base elements from it's dict and
-returns a new dict of initialized elements to be dumped into the global scope
-of the dialect. The `elements.py` file of a specific dialect can then remove
-any elements that it doesn't support (using the `del` keyword) and add/
-overwrite any it does support. There's also a _dialects.py file that has a dict
-for each dialect to describe the dialect-specific behavior of the EZRegex
-class, for example, in the JavaScript dialect, /'s are added to the beginning
-and end of the pattern, and flags are handled differently in each dialect. This
-has to be implemented directly into the EZRegex class. The dicts *would* be in
-the dialect folders themselves, but that causes all sorts of circular
-dependancies, so they're all just in the _dialects.py file. There's 4 parts to
-the dicts in the _dialects.py file: - `beginning` and `end` - Plain strings
-which describe what to tack onto the beginning and end of the compiled pattern
-(but *before* flags are added) - `flag_func` - A function that gets called with
-`final`, which is the final compiled pattern *with* `beginning` and `end`
-attached, and `flags`, which is a string of all the flags applied to the
-pattern. Internally, the flags are single digits, because flags usually are.
-They get passed to this function as a single string, which can be parsed and
-modified if necissary (it usually isn't) - `escape_chars` - The characters that
-need to be escaped. Should be a byte string (i.e. b'...') ### Inverting There's
-actually 2 algorithms implemented for "inverting" regexs. The old algorithm
-regexs the regexs in a specific order to replace parts one at a time. This is
-just as nasty and horrifying as it sounds. Dispite it being a terrible,
-*terrible* solution, I actually got it to work decently well. Later, when I was
-reading up on abstract syntax trees, and scrolling around on PyPi, I realized
-that Python has one built in, and that it's available to use. I reimplemented
-the whole algorithm to instead parse the AST given by the built-in re lexer,
-and wrote my own parser on top of it, which works *much* better. Along the way,
-I also discovered, deep in the corners of the internet, 2 other Python
-libraries which do almost the same thing: `xeger` (regex backwards), and
-`sre_yield`. `xeger` technically works, however it tends to include unprintable
-characters, so it's output isn't very readable. `sre_yeild` is better, but it
-can be very slow, and is not quite the use case I'm going for. My invert
-algorithm is meant to be a debugging tool (though it doubles well for a testing
-tool), so it does things like detecting words (as opposed to seperate word
-characters) and inserts actual words, and doing the same for numbers and
-inserting `12345...`, as well as a couple other enhancements. ### Tests Tests
-for a while now have just been in a single `tests.py` file, which was a giant
-pile of all the tests. I'm currently moving to use pytest. There's a
-`regexs.json` file (and a `replacements.json` file) that have a bunch of
-regexs, along with things they're supposed to match, and things they're not
-supposed to match, for testing. ## Installation EZRegex is distributed on
-[PyPI](https://pypi.org) as a universal wheel and is available on Linux, macOS
-and Windows and supports Python 3.10+ and PyPy. ```bash pip install ezregex ```
-The import name is the same as the package name: ```python import ezregex as er
-``` ## Todo See [the todo](todo.txt). I'm slowly moving these to [GitHub
-issues](https://github.com/smartycope/ezregex/issues), but for now, they're
-mostly still there ## License EZRegex is distributed under the [MIT License]
-(https://choosealicense.com/licenses/mit)
+each dialect subclasses the EZRegex class and defines their own elements
+specific to that dialect (more on that later). Each element represents a
+fundamental part of the Regular Expression syntax for that language, as well as
+less-fundemental common combinations for convenience (like email and float).
+EZRegex can accept a string or a function to define how it's supposed to
+interact with the current "chain" of elements. If it's a string, it just adds
+it to the end. If it's a function, it can accept any positional or named
+parameters, but has to accept `cur=...` as the last parameter (it's
+complicated). The `cur` parameter is the current regular expression chain, as a
+string. What's returned becomes the new `cur` parameter of the next element,
+or, if there is no next element, the final regex. That way you can add to the
+front or back of an expression, and you can change what exactly gets added to
+the current expression based on other parameters. The EZRegex class has
+operators overloaded so you can combine them in intuitive ways and call them by
+intuitive names. ### Typing & Linting The updated method of doing this is to
+define all the EZRegex elements of a dialect in `elements.py`, and then add
+type hints and doc strings in the `elements.pyi` file. EZRegex elements that
+accept parameters are typed as functions (even though they're not), for both
+convenience for the user when using linter, and to give documentation in an
+easier way. EZRegex elements that don't accept parameters should be typed as
+EZRegex, and given documentation as a string on the line below it. This is
+*slightly* non-standard, but linters support it, as well as my documentation
+generator script, which parses the .pyi files. The elements can also be
+seperated into groups in the .pyi files by using `"Group: \\n\"`, which also
+gets parsed by the documentation script. The groups aren't used in the actual
+library, but are helpful in seperating the documentation, as well as used in
+[ezregex.org](http://ezregex.org) ### Dialects Because most regex dialects
+*are* 90% identical, a parent EZRegex class implements most of the applicable
+logic, and a hidden "base" dialect is implemented, but works a bit differently.
+It has an `elements.py` file, but it defines all the elements as a dict in the
+form of {"element_name": {"keyword": "arguements"}}. It then has a
+`load_dialect()` function, which is the only thing importable from it. The
+reason it's done this way is because most elements, though identical in
+different dialects, have to be the appropriate dialect subclass. `load_dialect
+()` takes the dialect type as a parameter, and instantiates the base elements
+from it's dict and returns a new dict of initialized elements to be dumped into
+the global scope of the dialect. The `elements.py` file of a specific dialect
+can then remove any elements that it doesn't support (using the `del` keyword)
+and add/overwrite any it does support, or that work differently. Each subclass
+of EZRegex must implement a few options to describe the dialect-specific
+behavior of the EZRegex class, for example, in the JavaScript dialect, /'s are
+added to the beginning and end of the pattern, and flags are handled
+differently in each dialect. This has to be implemented directly into the
+EZRegex subclass. There's 4 parts that are required: - `beginning` and `end` -
+Plain strings which describe what to tack onto the beginning and end of the
+compiled pattern (but *before* flags are added) - `flag_func` - An abstract
+function that gets called with `final`, which is the final compiled pattern
+*with* `beginning` and `end` attached, and `flags`, which is a string of all
+the flags applied to the pattern. Internally, the flags are single digits,
+because flags usually are. They get passed to this function as a single string,
+which can be parsed and modified if necissary (it usually isn't) -
+`escape_chars` - The characters that need to be escaped. Should be a byte
+string (i.e. b'...') ### Inverting There's actually 2 algorithms implemented
+for "inverting" regexs. The old algorithm regexs the regexs in a specific order
+to replace parts one at a time. This is just as nasty and horrifying as it
+sounds. Dispite it being a terrible, *terrible* solution, I actually got it to
+work decently well. Later, when I was reading up on abstract syntax trees, and
+scrolling around on PyPi, I realized that Python has one built in, and that
+it's available to use. I reimplemented the whole algorithm to instead parse the
+AST given by the built-in re lexer, and wrote my own parser on top of it, which
+works *much* better. Along the way, I also discovered, deep in the corners of
+the internet, 2 other Python libraries which do almost the same thing: `xeger`
+(regex backwards), and `sre_yield`. `xeger` technically works, however it tends
+to include unprintable characters, so it's output isn't very readable.
+`sre_yeild` is better, but it can be very slow, and is not quite the use case
+I'm going for. My invert algorithm is meant to be a debugging tool (though it
+doubles well for a testing tool), so it does things like detecting words (as
+opposed to seperate word characters) and inserts actual words, and doing the
+same for numbers and inserting `12345...`, as well as a couple other
+enhancements. ## Installation EZRegex is distributed on [PyPI](https://
+pypi.org) as a universal wheel and is available on Linux, macOS and Windows and
+supports Python 3.10+ and PyPy. ```bash pip install ezregex ``` The import name
+is the same as the package name: ```python import ezregex as er ``` ## Todo See
+the [GitHub Issue Page](https://github.com/smartycope/ezregex/issues) ##
+License EZRegex is distributed under the [MIT License](https://
+choosealicense.com/licenses/mit)
```

