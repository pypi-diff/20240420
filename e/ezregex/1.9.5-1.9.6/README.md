# Comparing `tmp/ezregex-1.9.5.tar.gz` & `tmp/ezregex-1.9.6.tar.gz`

## Comparing `ezregex-1.9.5.tar` & `ezregex-1.9.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ezregex-1.9.5/.coveragerc
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ezregex-1.9.5/MANIFEST.in
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 ezregex-1.9.5/requirements.txt
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 ezregex-1.9.5/setup.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 ezregex-1.9.5/tox.ini
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ezregex-1.9.5/.github/FUNDING.yml
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 ezregex-1.9.5/.github/workflows/unit-tests.yml
--rw-r--r--   0        0        0    19179 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/EZRegex.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/__init__.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/_dialects.py
--rw-r--r--   0        0        0     7509 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/_docs.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/api.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/api.pyi
--rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/generate.py
--rw-r--r--   0        0        0    24619 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/invert.py
--rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/invert_old.py
--rw-r--r--   0        0        0  4975177 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/assets/sorted_words.json
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/base/__init__.py
--rw-r--r--   0        0        0     9832 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/base/elements.py
--rw-r--r--   0        0        0    12964 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/base/interface.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/javascript/__init__.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/javascript/elements.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/javascript/elements.pyi
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/javascript/psuedonymns.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/perl/__init__.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/perl/elements.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/perl/elements.pyi
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/perl/psuedonymns.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/python/__init__.py
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/python/elements.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/python/elements.pyi
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.5/ezregex/python/psuedonymns.py
--rw-r--r--   0        0        0    13484 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/groups.py
--rw-r--r--   0        0        0    17584 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/regexs.jsonc
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/replacements.jsonc
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/test_EZRegex.py
--rw-r--r--   0        0        0    17019 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/test_elements.py
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/test_generate.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/test_invert.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/test_javascript.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/test_operators.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/test_python.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/test_replacement.py
--rw-r--r--   0        0        0    37422 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/testing_color_algorithm.ipynb
--rw-r--r--   0        0        0    15201 2020-02-02 00:00:00.000000 ezregex-1.9.5/tests/tests.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 ezregex-1.9.5/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ezregex-1.9.5/LICENSE
--rw-r--r--   0        0        0    52510 2020-02-02 00:00:00.000000 ezregex-1.9.5/README.md
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 ezregex-1.9.5/pyproject.toml
--rw-r--r--   0        0        0    53450 2020-02-02 00:00:00.000000 ezregex-1.9.5/PKG-INFO
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ezregex-1.9.6/.coveragerc
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ezregex-1.9.6/MANIFEST.in
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 ezregex-1.9.6/requirements.txt
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 ezregex-1.9.6/setup.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 ezregex-1.9.6/tox.ini
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ezregex-1.9.6/.github/FUNDING.yml
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 ezregex-1.9.6/.github/workflows/unit-tests.yml
+-rw-r--r--   0        0        0    19097 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/EZRegex.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/__init__.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/_dialects.py
+-rw-r--r--   0        0        0     7509 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/_docs.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/api.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/api.pyi
+-rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/generate.py
+-rw-r--r--   0        0        0    24626 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/invert.py
+-rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/invert_old.py
+-rw-r--r--   0        0        0   337000 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/assets/common_sorted_words.json
+-rw-r--r--   0        0        0  4975177 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/assets/sorted_words.json
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/base/__init__.py
+-rw-r--r--   0        0        0     9831 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/base/elements.py
+-rw-r--r--   0        0        0    12964 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/base/interface.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/javascript/__init__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/javascript/elements.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/javascript/elements.pyi
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/javascript/psuedonymns.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/perl/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/perl/elements.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/perl/elements.pyi
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/perl/psuedonymns.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/python/__init__.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/python/elements.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/python/elements.pyi
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.6/ezregex/python/psuedonymns.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/test_EZRegex.py
+-rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/test_generate.py
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/test_invert.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/test_javascript.py
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/test_operators.py
+-rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/test_python.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/test_replacement.py
+-rw-r--r--   0        0        0    37422 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/testing_color_algorithm.ipynb
+-rw-r--r--   0        0        0    13448 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/data/groups.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/data/python_regexs.jsonc
+-rw-r--r--   0        0        0    18074 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/data/regexs.jsonc
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 ezregex-1.9.6/tests/data/replacements.jsonc
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 ezregex-1.9.6/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ezregex-1.9.6/LICENSE
+-rw-r--r--   0        0        0    53707 2020-02-02 00:00:00.000000 ezregex-1.9.6/README.md
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 ezregex-1.9.6/pyproject.toml
+-rw-r--r--   0        0        0    54647 2020-02-02 00:00:00.000000 ezregex-1.9.6/PKG-INFO
```

### Comparing `ezregex-1.9.5/setup.py` & `ezregex-1.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.5/.github/FUNDING.yml` & `ezregex-1.9.6/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.5/.github/workflows/unit-tests.yml` & `ezregex-1.9.6/.github/workflows/unit-tests.yml`

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
+        python -m pip install --upgrade pytest jstyleson py_js_runner rich Cope
     - name: Run Tests
       run: |
-        cd tests/
-        python tests.py
+        pytest .
```

### Comparing `ezregex-1.9.5/ezregex/EZRegex.py` & `ezregex-1.9.6/ezregex/EZRegex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # pyright: reportArgumentType = false
-import colorsys
 import logging
 import re
 from copy import deepcopy
 from functools import partial
-from typing import Callable, List, Literal, LiteralString
-from warnings import warn
+from typing import Callable, List, Literal
 
 from .api import api
 from .generate import *
 from .invert import invert
 from ._dialects import dialects
 
 # TODO: consider changing addFlags to "outer" or "end" or something
 # TODO: Seriously consider removing the debug functions
 # TODO: in all the magic functions assert that we're not mixing dialects
+# TODO: delete induvidual deepcopy statements and rerun all the tests to see what ones I can remove
 
 class EZRegex:
     """ Represent parts of the Regex syntax. Should not be instantiated by the user directly."""
 
     def __init__(self,
                  definition:List[partial[str]]|str|"EZRegex"|partial[str]|list[str],
                  dialect: str,
@@ -32,35 +31,34 @@
         with other EZRegexs and strings. Ideally, this should only be called internally, but it should
         still work from the user's end
         """
 
         if dialect not in dialects.keys():
             raise ValueError(f'Unsupported dialect `{dialect}` given. Supported dialects are: {list(dialects.keys())}')
 
+        # Set attributes like this so the class can remain "immutable", while still being usable
         self.__setattr__('flags', flags, True)
         # Parse params
         # Add flags if it's another EZRegex
         if isinstance(definition, EZRegex):
             self.__setattr__('flags', definition.flags, True)
-            if definition._dialect != dialect:
+            if definition.dialect != dialect:
                 raise ValueError('Cannot mix regex dialects')
 
         if isinstance(definition, (str, EZRegex)):
             definition = [str(definition)]
         elif not isinstance(definition, (list, tuple)):
             definition = [definition]
 
         self.__setattr__('_sanatize', sanatize, True)
         self.__setattr__('replacement', replacement, True)
         # This allows strings in the list now, but they get converted later in this function
         # self._funcList: list[str|partial[str]|Callable] = list(definition)
         self.__setattr__('_funcList', list(definition), True)
-        # Just some psuedonymns
-        # self.example = self.invert = self.inverse
-        self.__setattr__('_dialect', dialect, True)
+        self.__setattr__('dialect', dialect, True)
         # The dict that has the values
         self.__setattr__('_dialect_attr', dialects[dialect], True)
 
 
         # The init parameter is not actually required, but it will make it more
         # efficient, so we don't have to check that the whole chain is callable
         if init:
@@ -112,26 +110,26 @@
         # If this is being called without parameters, just compile the chain.
         # If it's being called *with* parameters, then it better be a fundemental
         # member, otherwise that doesn't make any sense.
         if len(self._funcList) > 1:
             if not len(args) and not len(kwargs):
                 return self._compile()
             else:
-                raise ValueError("You're trying to pass parameters to a chain of expressions. That doesn't make any sense. Stop that.")
+                raise TypeError("You're trying to pass parameters to a chain of expressions. That doesn't make any sense. Stop that.")
 
         # Sanatize the arguments
         args = list(map(self._sanitizeInput if self._sanatize else deepcopy, args))
 
         _kwargs = {}
         for key, val in kwargs.items():
             _kwargs[key] = self._sanitizeInput(val) if self._sanatize else deepcopy(val)
 
         return EZRegex(
             [partial(self._funcList[0], *args, **_kwargs)],
-            dialect=self._dialect,
+            dialect=self.dialect,
             init=False,
             sanatize=self._sanatize,
             replacement=self.replacement,
             flags=self.flags
         )
 
     # Magic Functions
@@ -142,15 +140,15 @@
         return 'EZRegex("' + self._compile() + '")'
 
     def __eq__(self, thing):
         return self._sanitizeInput(thing, addFlags=True) == self._compile()
 
     def __mul__(self, amt):
         if amt is Ellipsis:
-            return EZRegex(f'(?{self})*', self._dialect, sanatize=False)
+            return EZRegex(f'(?{self})*', self.dialect, sanatize=False)
         rtn = self
         # This isn't optimal, but it's unlikely anyone will use this with large numbers
         for i in range(amt-1):
             # This doesn't work
             # rtn += self
             # But this does??
             rtn = rtn + self
@@ -160,41 +158,41 @@
         return self * amt
 
     def __imul__(self, amt):
         return self * amt
 
     def __add__(self, thing):
         return EZRegex(self._funcList + [partial(lambda cur=...: cur + self._sanitizeInput(thing))],
-            dialect=self._dialect,
+            dialect=self.dialect,
             init=False,
             sanatize=self._sanatize or thing._sanatize if isinstance(thing, EZRegex) else self._sanatize,
             replacement=self.replacement or thing.replacement if isinstance(thing, EZRegex) else self.replacement,
             flags=(self.flags + thing.flags) if isinstance(thing, EZRegex) else self.flags
         )
 
     def __radd__(self, thing):
         return EZRegex([partial(lambda cur=...: self._sanitizeInput(thing) + cur)] + self._funcList,
-            dialect=self._dialect,
+            dialect=self.dialect,
             init=False,
             sanatize=self._sanatize or thing._sanatize if isinstance(thing, EZRegex) else self._sanatize,
             replacement=self.replacement or thing.replacement if isinstance(thing, EZRegex) else self.replacement,
             flags=(self.flags + thing.flags) if isinstance(thing, EZRegex) else self.flags
         )
 
     def __iadd__(self, thing):
         # return self + self._sanitizeInput(thing)
         return self + thing
 
     def __and__(self, thing):
-        warn('The & operator is unstable still. Use each() instead.')
-        return EZRegex(fr'(?={self}){thing}', self._dialect, sanatize=False)
+        logging.warning('The & operator is unstable still. Use each() instead.')
+        return EZRegex(fr'(?={self}){thing}', self.dialect, sanatize=False)
 
     def __rand__(self, thing):
-        warn('The & operator is unstable still. Use each() instead.')
-        return EZRegex(fr'(?={thing}){self}', self._dialect, sanatize=False)
+        logging.warning('The & operator is unstable still. Use each() instead.')
+        return EZRegex(fr'(?={thing}){self}', self.dialect, sanatize=False)
 
     # The shift operators just shadow the add operators
     def __lshift__(self, thing):
         return self.__add__(thing)
 
     def __rlshift__(self, thing):
         return self.__radd__(thing)
@@ -214,25 +212,27 @@
 
     def __invert__(self):
         return self.invert()
 
     def __not__(self):
         raise NotImplementedError('The not operator is not implemented. What you probably want is one of anyExcept(), anyCharExcept(), ifNotProceededBy(), or ifNotPreceededBy()')
 
+    def __rnot__(self):
+        raise NotImplementedError('The not operator is not implemented. What you probably want is one of anyExcept(), anyCharExcept(), ifNotProceededBy(), or ifNotPreceededBy()')
+
     def __pos__(self):
         comp = self._compile()
-        return EZRegex(('' if not len(comp) else r'(?:' + comp + r')') + r'+', self._dialect, sanatize=False)
+        return EZRegex(('' if not len(comp) else r'(?:' + comp + r')') + r'+', self.dialect, sanatize=False)
 
     def __ror__(self, thing):
-        print('ror called')
-        return EZRegex(f'(?:{self._sanitizeInput(thing)}|{self._compile()})', self._dialect, sanatize=False)
+        return EZRegex(f'(?:{self._sanitizeInput(thing)}|{self._compile()})', self.dialect, sanatize=False)
 
     def __or__(self, thing):
-        warn('The or operator is unstable and likely to fail, if used more than twice. Use anyof() instead, for now.')
-        return EZRegex(f'(?:{self._compile()}|{self._sanitizeInput(thing)})', self._dialect, sanatize=False)
+        logging.warning('The or operator is unstable and likely to fail, if used more than twice. Use anyof() instead, for now.')
+        return EZRegex(f'(?:{self._compile()}|{self._sanitizeInput(thing)})', self.dialect, sanatize=False)
 
     def __xor__(self, thing):
         return NotImplemented
 
     def __rxor__(self, thing):
         return NotImplemented
 
@@ -286,49 +286,58 @@
             # assert digit[...:'foo'] == digit[None:'foo'] == digit[,'foo'] ==
             pass
         elif type(args) is not tuple or len(args) == 1:
             if type(args) is tuple:
                 args = args[0]
             if args is None or args is Ellipsis or args == 0:
                 # at_least_0(self)
-                return EZRegex(fr'(?:{self._compile()})*', self._dialect, sanatize=False)
+                return EZRegex(fr'(?:{self._compile()})*', self.dialect, sanatize=False)
             elif args == 1:
                 # at_least_1(self)
-                return EZRegex(fr'(?:{self._compile()})+', self._dialect, sanatize=False)
+                return EZRegex(fr'(?:{self._compile()})+', self.dialect, sanatize=False)
             else:
                 # match_at_least(args, self)
-                return EZRegex(fr'(?:{self._compile()}){{{args},}}', self._dialect, sanatize=False)
+                return EZRegex(fr'(?:{self._compile()}){{{args},}}', self.dialect, sanatize=False)
         else:
             start, end = args
             if start is None or start is Ellipsis:
                 # match_at_most(2, self)
-                return EZRegex(fr'(?:{self._compile()}){{0,{end}}}', self._dialect, sanatize=False)
+                return EZRegex(fr'(?:{self._compile()}){{0,{end}}}', self.dialect, sanatize=False)
             elif end is None or end is Ellipsis:
                 if start == 0:
                     # at_least_0(self)
-                    return EZRegex(fr'(?:{self._compile()})*', self._dialect, sanatize=False)
+                    return EZRegex(fr'(?:{self._compile()})*', self.dialect, sanatize=False)
                 elif start == 1:
                     # at_least_1(self)
-                    return EZRegex(fr'(?:{self._compile()})+', self._dialect, sanatize=False)
+                    return EZRegex(fr'(?:{self._compile()})+', self.dialect, sanatize=False)
                 else:
                     # match_at_least(start, self)
-                    return EZRegex(fr'(?:{self._compile()}){{{start},}}', self._dialect, sanatize=False)
+                    return EZRegex(fr'(?:{self._compile()}){{{start},}}', self.dialect, sanatize=False)
             else:
                 # match_range(start, end, self)
-                return EZRegex(fr'(?:{self._compile()}){{{start},{end}}}', self._dialect, sanatize=False)
+                return EZRegex(fr'(?:{self._compile()}){{{start},{end}}}', self.dialect, sanatize=False)
 
     def __reversed__(self):
         return self.inverse()
 
     def __rich__(self):
         return self._compile()
 
     def __pretty__(self):
         return self._compile()
 
+    def __setattr__(self, name, value, ignore=False):
+        if ignore:
+            self.__dict__[name] = value
+        else:
+            raise TypeError('EZRegex objects are immutable')
+
+    def __delattr__(self, *args):
+        raise TypeError('EZRegex objects are immutable')
+
     # Regular functions
     def _compile(self, addFlags=True):
         regex = ''
         for func in self._funcList:
             regex = func(cur=regex) # type: ignore
 
         # Add the flags
@@ -373,30 +382,22 @@
         from rich.text import Text
 
         # json = self._matchJSON(testString=testString)
         json = api(self, test_string=testString)
         if not show:
             return bool(len(json['matches']))
 
-        _cope = False
-        if context:
-            # Use the nice context function in the Cope library
-            try:   from Cope import get_context, get_metadata
-            except ImportError: pass
-            else:  _cope = True
-
         st = Text()  # String
         gt = Text()  # Groups (all the group-related text)
         defaultColor = 'bold'
         textColor = ''
 
         st.append("Testing expression", style=defaultColor)
         # Add the context line
-        if _cope:
-            st.append(f' (from {get_context(get_metadata(2), False, True, True).strip()})', style=defaultColor)
+        # st.append(f' (from {get_context(get_metadata(2), False, True, True).strip()})', style=defaultColor)
         st.append(':\n', style=defaultColor)
 
         # The expression we're testing
         st.append(f'\t{json["regex"]}\n', style=textColor)
         st.append("for matches in:\n\t", style=defaultColor)
 
         # Add the main string
@@ -441,22 +442,7 @@
     def inverse(self, amt=1, **kwargs):
         """ "Inverts" the current Regex expression to give an example of a string it would match.
             Useful for debugging purposes. """
         return '\n'.join([invert(self._compile(), **kwargs) for _ in range(amt)])
 
     def invert(self, amt=1, **kwargs):
         return self.inverse(amt, **kwargs)
-
-
-    @property
-    def dialect(self):
-        return self._dialect
-
-    def __setattr__(self, name, value, ignore=False):
-        if ignore:
-            self.__dict__[name] = value
-        else:
-            raise TypeError('EZRegex objects are immutable')
-
-
-    def __delattr__(self, *args):
-        raise TypeError('EZRegex objects are immutable')
```

### Comparing `ezregex-1.9.5/ezregex/_dialects.py` & `ezregex-1.9.6/ezregex/_dialects.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.5/ezregex/_docs.py` & `ezregex-1.9.6/ezregex/_docs.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.5/ezregex/api.py` & `ezregex-1.9.6/ezregex/api.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.5/ezregex/api.pyi` & `ezregex-1.9.6/ezregex/api.pyi`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.5/ezregex/generate.py` & `ezregex-1.9.6/ezregex/generate.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.5/ezregex/invert.py` & `ezregex-1.9.6/ezregex/invert.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 else:
     from re import _parser as sre  # type: ignore
 
 # So I can debug this function directly
 if __name__ != '__main__':
     from .invert_old import invertRegex
 
-with open(Path(__file__).parent / 'assets' / 'sorted_words.json') as f:
+with open(Path(__file__).parent / 'assets' / 'common_sorted_words.json') as f:
     words = json.load(f)
 
 # Don't use string.whitespace, because we don't want to use weird difficult to print characters.
 # We want the replacement to be readable.
 _whitespace   = ' '
 _everything   = string.digits + string.ascii_letters + string.punctuation + _whitespace + '_'
```

### Comparing `ezregex-1.9.5/ezregex/invert_old.py` & `ezregex-1.9.6/ezregex/invert_old.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from copy import copy
 from dataclasses import dataclass
 from random import choice, choices, randint
 from warnings import warn
 
 
 def unsanitize(string):
-    return re.sub(r'\\([' + re.escape(')([]{}+*$^-\\?| ,') + r'])', '\g<1>', string)
+    return re.sub(r'\\([' + re.escape(')([]{}+*$^-\\?| ,') + r'])', r'\g<1>', string)
 
 def randbool():
     return bool(randint(0, 1))
 
 def _randWord(randomlyGenerate=False):
     if randomlyGenerate:
         return ''.join(choices(_letters + '_', k=randint(1, _alot)))
```

### Comparing `ezregex-1.9.5/ezregex/assets/sorted_words.json` & `ezregex-1.9.6/ezregex/assets/sorted_words.json`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.5/ezregex/base/elements.py` & `ezregex-1.9.6/ezregex/base/elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
     # Grouping
     'group':              {'definition': lambda input, name=None, cur=...: f'{cur}({input})' if name is None else f'{cur}(?P<{name}>{input})'},
     'passive_group':      {'definition': lambda input, cur=...: f'{cur}(?:{input})'},
     'earlier_group':      {'definition': lambda num_or_name, cur=...: f'{cur}\\{num_or_name}' if isinstance(num_or_name, int) or num_or_name in digits else f'{cur}(?P={num_or_name})'},
     'if_exists':          {'definition': lambda num_or_name, does, doesnt, cur=...: f'{cur}(?({num_or_name}){does}{"|" + str(doesnt) if doesnt is not None else ""})'},
 
     # Premade
-    'literally_anything':  {'definition': r'(?:.|\n)'},
+    'literally_anything': {'definition': r'(?:.|\n)'},
     'signed':             {'definition': r'(?:(?:\-|\+))?\d+'},
     'unsigned':           {'definition': r'\d+'},
     'plain_float':        {'definition': r'(?:(?:\-|\+))?\d+\.(?:\d+)?'},
     'full_float':         {'definition': r'(?:(?:\-|\+))?\d+\.(?:\d+)?(?:e(?:(?:\-|\+))?\d+)?'},
     'int_or_float':       {'definition': r'(?:(?:\-|\+))?\d+\.(?:\d+)?(?:e(?:(?:\-|\+))?\d+)?(?:\-)?\d+(?:\.(?:\d+)?)?'},
     'ow':                 {'definition': r'(?:\s+)?'},
```

### Comparing `ezregex-1.9.5/ezregex/base/interface.py` & `ezregex-1.9.6/ezregex/base/interface.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.5/ezregex/javascript/psuedonymns.py` & `ezregex-1.9.6/ezregex/javascript/psuedonymns.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.5/ezregex/perl/psuedonymns.py` & `ezregex-1.9.6/ezregex/perl/psuedonymns.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.5/ezregex/python/psuedonymns.py` & `ezregex-1.9.6/ezregex/python/psuedonymns.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.5/tests/groups.py` & `ezregex-1.9.6/tests/data/groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import random
 
-# from builtins import __builtin__
-
 Set = frozenset # Data will be frozensets, so they can't be mutated.
 
 def words(text):
     "All space-separated words in text."
     return Set(text.split())
 
 def phrases(text, sep='/'):
```

### Comparing `ezregex-1.9.5/tests/regexs.jsonc` & `ezregex-1.9.6/tests/data/regexs.jsonc`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-// This goes [regex, [things it should match], [things it shouldnt match]]
+// This goes ["regex", [things it should match], [things it shouldnt match]]
+// IMPORTANT NOTE: Because this is a JSON file, and the the regexs get compiled, escaped characters like \n and \t need to
+// be double escaped in the regex patterns (i.e. \\n, \\t), but NOT in the strings they should and shouldn't match
 [
     [
         "'------------------FIRST REGEX---------------------'",
         ["------------------FIRST REGEX---------------------"],
         ["asdk"]
     ],
     [
@@ -163,35 +165,35 @@
     [
         "raw(r'.')",
         ["s", "a", "h", "r", "d", "h", "c", "f", "G", "S", "G", "D", "8", "7", "w", "3", "u", "e", "8", "4", "1", "2", "5", "a", "s", "d", "_", ";", ".", ",", "?", ".", "1", "3", "4", "*", "&", "^", "`"],
         []
     ],
     [
         "raw(r'\\n')",
-        ["\\n"],
+        ["\n"],
         []
     ],
     [
         "raw(r'\\r')",
-        ["\\r"],
+        ["\r"],
         []
     ],
     [
         "raw(r'\\t')",
-        ["\\t"],
-        []
-    ],
-    [
-        "raw(r'\\v')",
-        ["\\v"],
+        ["\t"],
         []
     ],
+    // [
+    //     "raw(r'\\v')",
+    //     ["\\v"],
+    //     []
+    // ],
     [
         "raw(r'\\f')",
-        ["\\f"],
+        ["\f"],
         []
     ],
     [
         "raw(r'\\S')",
         ["s", "d", "g", "S", "G", "H", "R", "5", "1", "2", "2", "$", "%", "^", "&", "*", "Z", "`"],
         []
     ],
@@ -329,46 +331,46 @@
     [
         "stringStartsWith('a')",
         ["asdfs", "a 89sdf a", "a"],
         [" asdf", "sdfa", "sdf"]
     ],
     [
         "lineStartsWith('a')",
-        ["asdfs", "a 89sdf a", "a", "sdfs\\nasdfd"],
-        [" asdf", "sdf\\nsdf", "sdf\\n a", "sdfa", "sdf"]
+        ["asdfs", "a 89sdf a", "a", "sdfs\nasdfd"],
+        [" asdf", "sdf\nsdf", "sdf\n a", "sdfa", "sdf"]
     ],
     [
         "stringEndsWith('a')",
         ["lklkjfda", "sdf 8 a", "a"],
         ["asdfds", "sd fd"]
     ],
     [
         "lineEndsWith('a')",
-        ["lklkjfda", "sdf 8 a", "a", "sdf\\na", "sdfse\\nsdafsda", "sdfa\\nsdf"],
+        ["lklkjfda", "sdf 8 a", "a", "sdf\na", "sdfse\nsdafsda", "sdfa\nsdf"],
         ["asdfds", "sd fd"]
     ],
     [
         "literal('test')",
         ["test", " sdfstestsdfs",],
         ["te st",]
     ],
     [
         "underscore",
         ["_",],
-        ["a test", "test ", "\\ntest\\n", "\\ntest", "test\\n"]
+        ["a test", "test ", "\ntest\n", "\ntest", "test\n"]
     ],
     [
         "quote",
         ["\"", "'", "`"],
-        ["a test", "test ", "\\ntest\\n", "\\ntest", "test\\n"]
+        ["a test", "test ", "\ntest\n", "\ntest", "test\n"]
     ],
     [
         "isExactly('test')",
         ["test",],
-        ["a test", "test ", "\\ntest\\n", "\\ntest", "test\\n"]
+        ["a test", "test ", "\ntest\n", "\ntest", "test\n"]
     ],
     [
         "matchMax('a')",
         ["aaa", "a"],
         ["b",]
     ],
     [
@@ -394,25 +396,25 @@
     [
         "either('aa', 'ba')",
         ["aa", "ba",],
         ["bb", "a"]
     ],
     [
         "whitespace",
-        [" ", "\\t", "\\t  ", "\\n"],
+        [" ", "\t", "\t  ", "\n"],
         ["dfsd",]
     ],
     [
         "whitechunk",
-        [" ", "\\t", "\\t  ", "\\n"],
+        [" ", "\t", "\t  ", "\n"],
         ["dfsd",]
     ],
     [
         "white",
-        [" ", "\\t", "\\t  ", "\\n"],
+        [" ", "\t", "\t  ", "\n"],
         ["dfsd",]
     ],
     [
         "digit",
         ["6",],
         ["_", "-", "a"]
     ],
@@ -439,41 +441,41 @@
     [
         "octDigit",
         ["7",],
         ["9", "a", "A", "8"]
     ],
     [
         "chunk",
-        ["wordssdf   asdf\\n",],
-        ["\\n",]
+        ["wordssdf   asdf\n",],
+        ["\n",]
     ],
     [
         "spaceOrTab",
-        [" ", "\\t", " \\t  "],
-        ["\\n",]
+        [" ", "\t", " \t  "],
+        ["\n",]
     ],
     [
         "newLine",
-        ["\\n",],
+        ["\n",],
         ["\r",]
     ],
     [
         "carriageReturn",
         ["\r",],
-        ["\\n",]
+        ["\n",]
     ],
     [
         "tab",
-        ["\\t",],
+        ["\t",],
         [" ",]
     ],
     [
         "space",
         [" ",],
-        ["\\t",]
+        ["\t",]
     ],
     [
         "quote",
         ["'", "\""],
         ["wer",]
     ],
     [
@@ -524,41 +526,41 @@
     [
         "(optional('a') + 'b') * 3",
         ["abbb", "bbb", "ababab", "bbab"],
         ["", "aaa", "aa", "a"]
     ],
     [
         "word + whitechunk + group('func') + ':' + '()' + group(either('|', '7'), name='test')",
-        ["wo  func:[]|", "wo  func:[]7"],
-        []
+        ["wo  func:()|", "wo  func:()7"],
+        ["wo  func:[]|", "wo  func:(]7"],
     ],
     [
         "word + whitechunk + group('func') + ':' + group(anyof('8', '7'), 'test')",
         ["wo  func:8", "wo  func:7"],
         []
     ],
     [
         "7 + anyof('abc') + lineEnd",
-        ["7a", "sdfsd7b", "sdf\\nsdf7b", "sdf\\nsdf7b\\n"],
+        ["7a", "sdfsd7b", "sdf\nsdf7b", "sdf\nsdf7b\n"],
         ["7asdfsd", "7v"]
     ],
     [
         "7 + anyof('abc') + stringEnd",
         ["7a", "sdfsd7b"],
-        ["7asdfsd", "7v", "sdf\\nsdf7bds", "sdf\\nsdf7bf\\n"]
+        ["7asdfsd", "7v", "sdf\nsdf7bds", "sdf\nsdf7bf\n"]
     ],
     [
         "lineStart + 7 + anyof('abc')",
-        ["7a", "7bsdfsd", "\\n7a", "\\n7bsdfsd"],
+        ["7a", "7bsdfsd", "\n7a", "\n7bsdfsd"],
         ["ds7asdfsd", "7v"]
     ],
     [
         "stringStart + 7 + anyof('abc')",
         ["7a", "7bsdfsd"],
-        ["ds7asdfsd", "7v", "\\n7a", "\\n7bsdfsd"]
+        ["ds7asdfsd", "7v", "\n7a", "\n7bsdfsd"]
     ],
     [
         "+alpha",
         ["a", "asd"],
         ["89", "._78"]
     ],
     [
@@ -587,14 +589,24 @@
         []
     ],
     [
         "(match_range(3, 5, word_char) + ' ') + (match_range(3, 5, word_char) + ' ') + (match_range(3, 5, word_char) + ' ') + (match_range(3, 5, word_char) + ' ') + (match_range(3, 5, word_char) + ' ') + (match_range(3, 5, word_char) + ' ')",
         [],
         []
     ],
+    [
+        "group('pattern', name='i') + optional(digit) + match_max(group('me')) + amt(2, 'mhmm')",
+        [],
+        []
+    ],
+    [
+        "group('', name='i') + optional(digit) + match_max(group('')) + amt(2, '')",
+        [],
+        []
+    ],
     // ('foo' + ((chunk + 'here' + chunk) & (chunk + anyOf('this', 'that') + chunk)) + 'bar',  ('fooum here there that bar', 'foo that there here bar'),               None),
     // ('foo' + ((chunk + 'here' + chunk) & (chunk + anyOf('this', 'that') + chunk) & (chunk + 'the' + chunk)) + 'bar',  ('fooum the here there that bar', 'foo that there thehere bar'), ('fooum here there that bar', 'foo that there here bar')),
     // (,                                                                                    (,),                                                                    (,)),
     // (word_boundary + word_char[...,3] + wordBoundary,                                       ('yes', 'hey', 'sup', 'thi'),                                           ('none', 'no', 'foo3', '333', 'jar_')), // This does what it's supposed to do, but doesn't search correctly, as far as I understand it
     //TODO ('foo ' + anyExcept('bar') + ' baz',                                               ('foo thing baz', 'foo bax baz'),                                       ('foo bar baz',)),
     //TODO: (exactly('foo' + anyExcept('boo') + 'bar'),                                             ('foonotbar', 'foobar'),                                                ('fooboobar', 'boobar', 'fooboo')), // not sure where 'foo boo bar' goes
     //TODO: (exactly('foo' + anyExcept('boo', number) + 'bar'),                                     ('foo999bar', 'foo8bar'),                                               ('fooboobar','foonotbar', 'foo boo bar', 'foobar', 'boobar')),
@@ -621,9 +633,9 @@
     // anyBetween,                                                                           ('',),                                                                  ('',),
     // (unicode,                                                                             ('',),                                                                  ('',),
     // (word,                                                                                ('word',),                                                              ('33a',)), // Is this *supposed* to work?
     [
         "'------------------LAST REGEX---------------------'",
         ["------------------LAST REGEX---------------------"],
         ["asdk"]
-    ],
+    ]
 ]
```

### Comparing `ezregex-1.9.5/tests/replacements.jsonc` & `ezregex-1.9.6/tests/data/replacements.jsonc`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [ // This goes ["regex pattern", "replacement regex", "base string", "what the base string should look like after substitution"]
     [
         "'------------------FIRST REPLACEMENT---------------------'",
-        "-",
+        "'-'",
         "asdk",
         "asdk"
     ],
     [ // Replace digits with *
         "digit",
-        "*",
+        "'*'",
         "123abc",
         "***abc"
     ],
     [ // Replace vowels with _
         "anyof('aeiou')",
-        "_",
+        "'_'",
         "hello",
         "h_ll_"
     ],
     [ // Replace digits with #
         "digit",
-        "#",
+        "'#'",
         "a1b2c3",
         "a#b#c#"
     ],
     [ // Swap the first two digits
         "group(digit) + group(digit)",
         "rgroup(2) + rgroup(1)",
         "12345",
@@ -51,15 +51,15 @@
         "group(+uppercase)",
         "rgroup(1) * 2",
         "HelloWorld",
         "HHelloWWorld"
     ],
     [ // Replace non-word characters with space
         "group(+not_word)",
-        " ",
+        "' '",
         "a@b#c",
         "a b c"
     ],
     [ // Add underscore between digits and lowercase letters
         "group(digit) + group(lowercase)",
         "rgroup(1) + '_' + rgroup(2)",
         "1a2b3c",
@@ -75,21 +75,21 @@
         "group(digit, 'digit') + group(lowercase, 'letter')",
         "rgroup('letter') + rgroup('digit')",
         "1a2b3c",
         "a1b2c3"
     ],
     [ // Enclose vowels in square brackets with named group
         "group(anyof('aeiou'), 'vowel')",
-        "f'[{rgroup('vowel')}]'",
+        "f\"[{rgroup('vowel')}]\"",
         "hello",
         "h[e]ll[o]"
     ],
     [
         "'foo' + group(number, 'num') + 'bar'",
-        "f'foo-{rgroup('num')}-bar'",
+        "f\"foo-{rgroup('num')}-bar\"",
         "foo87bar",
         "foo-87-bar"
     ],
     [
         "group(word + number) + ':' + ow + group(word)",
         "replace_group(1) + ' - ' + replace_group(2)",
         "test1:    thing",
@@ -105,15 +105,15 @@
         "stringStart + '(' + group(chunk + optional(',' + chunk)) + ')' + chunk",
         "'(' + '${' + rgroup(1) + '})'",
         "(name, input) -> ezregex.EZRegex.EZRegex",
         "(${name, input})"
     ],
     [
         "'------------------LAST REPLACEMENT---------------------'",
-        "-",
+        "'-'",
         "asdk",
         "asdk"
     ],
 ]
 
 // ("(\\b\\w{3}\\b)", "[\\1]", "The cat sat on the mat", "The [cat] [sat] on the [mat]"),  // Enclose 3-letter words in square brackets
 // ("(\\b\\w+\\b)", "\\U\\1", "python is fun", "PYTHON IS FUN"),  // Convert words to uppercase
```

### Comparing `ezregex-1.9.5/tests/test_EZRegex.py` & `ezregex-1.9.6/tests/test_EZRegex.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,7 +38,27 @@
 
     # This is actually accurate, if you think about it.
     # ifFollowedBy(word).test("literal(hllow) + isExactly('thing')")# fails in _matchJSON()
 
     ('(' + +(anything + optional(group(comma))) + ')').test()# -- empty groups print as None
 
     group(+group(number) + group(anyof('98'))).test('999')
+
+def test_no_parameters_to_chains():
+    # This is sort of conceptually impossible, ish
+    # with pytest.raises(TypeError):
+    #     digit(6)
+    # with pytest.raises(TypeError):
+    #     digit(input=6)
+    with pytest.raises(TypeError):
+        (digit + word)(6)
+    with pytest.raises(TypeError):
+        (digit + word)(input=6)
+    # This is also conceptually impossible without a moderate refactor
+    # with pytest.raises(TypeError):
+    #     match_amt(6, digit)(6)
+    # with pytest.raises(TypeError):
+    #     match_amt(6, digit)(input=6)
+
+    assert match_amt(6, digit)()
+    assert (digit + word)()
+    assert digit()
```

### Comparing `ezregex-1.9.5/tests/test_generate.py` & `ezregex-1.9.6/tests/test_generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import re
-from groups import *
-from groups import _losers, _winners
-
+from tests.data.groups import *
+from tests.data.groups import _losers, _winners
 
 from ezregex.generate import *
 
 
 def words(text):
     "All space-separated words in text."
     return Set(text.split())
```

### Comparing `ezregex-1.9.5/tests/test_invert.py` & `ezregex-1.9.6/tests/test_invert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from multiprocessing import Value
 from rich import print as rprint
 from rich.table import Table
 import time
 import threading
 from rich.text import Text
 from ezregex import invert
 from ezregex.python import literal
@@ -15,18 +14,18 @@
 import jstyleson
 
 
 def test_invert():
     offset = 2
 
     # The structure is ["regex pattern", "replacement regex", "base string", "what the base string should look like after substitution"]
-    with open('tests/replacements.jsonc') as f:
+    with open('tests/data/replacements.jsonc') as f:
         replacements = jstyleson.load(f)
 
-    with open('tests/regexs.jsonc') as f:
+    with open('tests/data/regexs.jsonc') as f:
         regexs = jstyleson.load(f)
 
     # with open('deleteme.txt', 'w') as f:
     #     rprint(regexs + replacements, file=f)
 
     table = Table(title="invert tests", expand=False)
     table.add_column("Line", justify="center", style="grey37")#, max_width=2)
```

### Comparing `ezregex-1.9.5/tests/test_javascript.py` & `ezregex-1.9.6/tests/test_javascript.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     #     py_js_runner.javascript().run(js)
 
 
 def test_javascript():
     return # This should be written in the javascript branch
     offset = 2
 
-    with open('tests/regexs.jsonc') as f:
+    with open('tests/data/regexs.jsonc') as f:
         regexs = jstyleson.load(f)
 
     for cnt, r in enumerate(regexs):
         regex_str, match, dontMatch = r
         regex = eval(regex_str, javascript.__dict__)
         try:
             if match:
```

### Comparing `ezregex-1.9.5/tests/test_operators.py` & `ezregex-1.9.6/tests/test_operators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,24 @@
-strictness=20
-dontIncludePassed=True
-invertBackend='re_parser'
-invert_tries=1
-import random
 import re
 
 import pytest
 from ezregex import *
-import jstyleson
-import ezregex as er
+
+strictness=20
+dontIncludePassed=True
+invertBackend='re_parser'
+invert_tries=1
 offset = 2
 
 
 def test_invert():
     import ezregex as er
     regex = (er.digit + er.word)
     assert re.search(regex.str(), ~regex)
 
-def test_not():
-    # Not sure why this doesn't work?...
-    with pytest.raises(NotImplementedError):
-        not anything
-
 # TODO: Finish this
 # assert digit * ... == matchMax(digit)
 
 # TODO: Debug this
 # assert digit | word == anyof(digit, word), f"{digit | word} != {anyof(digit, word)}"
 # assert 7 | digit == anyof(7, digit), f"{7 | digit} != {anyof(digit, 7)}"
 # assert re.search(str(digit | word | '1'), '1') == re.search(anyof(digit, word, 1).str(), '1')
```

### Comparing `ezregex-1.9.5/tests/testing_color_algorithm.ipynb` & `ezregex-1.9.6/tests/testing_color_algorithm.ipynb`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.5/.gitignore` & `ezregex-1.9.6/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 # Created by https://www.toptal.com/developers/gitignore/api/python,venv,visualstudiocode
 # Edit at https://www.toptal.com/developers/gitignore?templates=python,venv,visualstudiocode
 
 ### Python ###
 # Byte-compiled / optimized / DLL files
+__pycache__/**
+__pycache__/*
 __pycache__/
+__pycache__
 *.py[cod]
 *$py.class
-
+*.pyc
 # C extensions
 *.so
+**.pyc
+invert*.pyc
+__init__*.pyc
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
```

### Comparing `ezregex-1.9.5/LICENSE` & `ezregex-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.5/README.md` & `ezregex-1.9.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1029,14 +1029,24 @@
 
 ### Typing & Linting
 The updated method of doing this is to define all the EZRegex elements of a dialect in `elements.py`, and then add type hints and doc strings in the `elements.pyi` file. EZRegex elements that accept parameters are typed as functions (even though they're not), for both convenience for the user when using linter, and to give documentation in an easier way. EZRegex elements that don't accept parameters should be typed as EZRegex, and given documentation as a string on the line below it. This is *slightly* non-standard, but linters support it, as well as my documentation generator script, which parses the .pyi files. The elements can also be seperated into groups in the .pyi files by using `"Group: \<group name\>\n\<group description\>"`, which also gets parsed by the documentation script. The groups aren't used in the actual library, but are helpful in seperating the documentation, as well as used in [ezregex.org](http://ezregex.org)
 
 ### Dialects
 Because most regex dialects *are* 90% identical, a hidden "base" dialect is implemented, but it works a bit differently. It has an `elements.py` file, but it defines all the elements as a dict in the form of {"element_name": {"keyword": "arguements"}}. It then has a `load_dialect()` function, which is the only thing importable from it. The reason it's done this way is because `dialect` is a required parameter of the EZRegex constructor, so `load_dialect()` takes a `dialect` parameter, and constructs the base elements from it's dict and returns a new dict of initialized elements to be dumped into the global scope of the dialect. The `elements.py` file of a specific dialect can then remove any elements that it doesn't support (using the `del` keyword) and add/overwrite any it does support.
 
+There's also a _dialects.py file that has a dict for each dialect to describe the dialect-specific behavior of the EZRegex class, for example, in the JavaScript dialect, /'s are added to the beginning and end of the pattern, and flags are handled differently in each dialect. This has to be implemented directly into the EZRegex class. The dicts *would* be in the dialect folders themselves, but that causes all sorts of circular dependancies, so they're all just in the _dialects.py file.
+
+There's 4 parts to the dicts in the _dialects.py file:
+- `beginning` and `end`
+    - Plain strings which describe what to tack onto the beginning and end of the compiled pattern (but *before* flags are added)
+- `flag_func`
+    - A function that gets called with `final`, which is the final compiled pattern *with* `beginning` and `end` attached, and `flags`, which is a string of all the flags applied to the pattern. Internally, the flags are single digits, because flags usually are. They get passed to this function as a single string, which can be parsed and modified if necissary (it usually isn't)
+- `escape_chars`
+    - The characters that need to be escaped. Should be a byte string (i.e. b'...')
+
 ### Inverting
 There's actually 2 algorithms implemented for "inverting" regexs. The old algorithm regexs the regexs in a specific order to replace parts one at a time. This is just as nasty and horrifying as it sounds. Dispite it being a terrible, *terrible* solution, I actually got it to work decently well.
 
 Later, when I was reading up on abstract syntax trees, and scrolling around on PyPi, I realized that Python has one built in, and that it's available to use. I reimplemented the whole algorithm to instead parse the AST given by the built-in re lexer, and wrote my own parser on top of it, which works *much* better.
 
 Along the way, I also discovered, deep in the corners of the internet, 2 other Python libraries which do almost the same thing: `xeger` (regex backwards), and `sre_yield`. `xeger` technically works, however it tends to include unprintable characters, so it's output isn't very readable. `sre_yeild` is better, but it can be very slow, and is not quite the use case I'm going for. My invert algorithm is meant to be a debugging tool (though it doubles well for a testing tool), so it does things like detecting words (as opposed to seperate word characters) and inserts actual words, and doing the same for numbers and inserting `12345...`, as well as a couple other enhancements.
```

#### html2text {}

```diff
@@ -567,37 +567,52 @@
 "arguements"}}. It then has a `load_dialect()` function, which is the only
 thing importable from it. The reason it's done this way is because `dialect` is
 a required parameter of the EZRegex constructor, so `load_dialect()` takes a
 `dialect` parameter, and constructs the base elements from it's dict and
 returns a new dict of initialized elements to be dumped into the global scope
 of the dialect. The `elements.py` file of a specific dialect can then remove
 any elements that it doesn't support (using the `del` keyword) and add/
-overwrite any it does support. ### Inverting There's actually 2 algorithms
-implemented for "inverting" regexs. The old algorithm regexs the regexs in a
-specific order to replace parts one at a time. This is just as nasty and
-horrifying as it sounds. Dispite it being a terrible, *terrible* solution, I
-actually got it to work decently well. Later, when I was reading up on abstract
-syntax trees, and scrolling around on PyPi, I realized that Python has one
-built in, and that it's available to use. I reimplemented the whole algorithm
-to instead parse the AST given by the built-in re lexer, and wrote my own
-parser on top of it, which works *much* better. Along the way, I also
-discovered, deep in the corners of the internet, 2 other Python libraries which
-do almost the same thing: `xeger` (regex backwards), and `sre_yield`. `xeger`
-technically works, however it tends to include unprintable characters, so it's
-output isn't very readable. `sre_yeild` is better, but it can be very slow, and
-is not quite the use case I'm going for. My invert algorithm is meant to be a
-debugging tool (though it doubles well for a testing tool), so it does things
-like detecting words (as opposed to seperate word characters) and inserts
-actual words, and doing the same for numbers and inserting `12345...`, as well
-as a couple other enhancements. ### Tests Tests for a while now have just been
-in a single `tests.py` file, which was a giant pile of all the tests. I'm
-currently moving to use pytest. There's a `regexs.json` file (and a
-`replacements.json` file) that have a bunch of regexs, along with things
-they're supposed to match, and things they're not supposed to match, for
-testing. ## Installation EZRegex is distributed on [PyPI](https://pypi.org) as
-a universal wheel and is available on Linux, macOS and Windows and supports
-Python 3.10+ and PyPy. ```bash pip install ezregex ``` The import name is the
-same as the package name: ```python import ezregex as er ``` ## Todo See [the
-todo](todo.txt). I'm slowly moving these to [GitHub issues](https://github.com/
-smartycope/ezregex/issues), but for now, they're mostly still there ## License
-EZRegex is distributed under the [MIT License](https://choosealicense.com/
-licenses/mit)
+overwrite any it does support. There's also a _dialects.py file that has a dict
+for each dialect to describe the dialect-specific behavior of the EZRegex
+class, for example, in the JavaScript dialect, /'s are added to the beginning
+and end of the pattern, and flags are handled differently in each dialect. This
+has to be implemented directly into the EZRegex class. The dicts *would* be in
+the dialect folders themselves, but that causes all sorts of circular
+dependancies, so they're all just in the _dialects.py file. There's 4 parts to
+the dicts in the _dialects.py file: - `beginning` and `end` - Plain strings
+which describe what to tack onto the beginning and end of the compiled pattern
+(but *before* flags are added) - `flag_func` - A function that gets called with
+`final`, which is the final compiled pattern *with* `beginning` and `end`
+attached, and `flags`, which is a string of all the flags applied to the
+pattern. Internally, the flags are single digits, because flags usually are.
+They get passed to this function as a single string, which can be parsed and
+modified if necissary (it usually isn't) - `escape_chars` - The characters that
+need to be escaped. Should be a byte string (i.e. b'...') ### Inverting There's
+actually 2 algorithms implemented for "inverting" regexs. The old algorithm
+regexs the regexs in a specific order to replace parts one at a time. This is
+just as nasty and horrifying as it sounds. Dispite it being a terrible,
+*terrible* solution, I actually got it to work decently well. Later, when I was
+reading up on abstract syntax trees, and scrolling around on PyPi, I realized
+that Python has one built in, and that it's available to use. I reimplemented
+the whole algorithm to instead parse the AST given by the built-in re lexer,
+and wrote my own parser on top of it, which works *much* better. Along the way,
+I also discovered, deep in the corners of the internet, 2 other Python
+libraries which do almost the same thing: `xeger` (regex backwards), and
+`sre_yield`. `xeger` technically works, however it tends to include unprintable
+characters, so it's output isn't very readable. `sre_yeild` is better, but it
+can be very slow, and is not quite the use case I'm going for. My invert
+algorithm is meant to be a debugging tool (though it doubles well for a testing
+tool), so it does things like detecting words (as opposed to seperate word
+characters) and inserts actual words, and doing the same for numbers and
+inserting `12345...`, as well as a couple other enhancements. ### Tests Tests
+for a while now have just been in a single `tests.py` file, which was a giant
+pile of all the tests. I'm currently moving to use pytest. There's a
+`regexs.json` file (and a `replacements.json` file) that have a bunch of
+regexs, along with things they're supposed to match, and things they're not
+supposed to match, for testing. ## Installation EZRegex is distributed on
+[PyPI](https://pypi.org) as a universal wheel and is available on Linux, macOS
+and Windows and supports Python 3.10+ and PyPy. ```bash pip install ezregex ```
+The import name is the same as the package name: ```python import ezregex as er
+``` ## Todo See [the todo](todo.txt). I'm slowly moving these to [GitHub
+issues](https://github.com/smartycope/ezregex/issues), but for now, they're
+mostly still there ## License EZRegex is distributed under the [MIT License]
+(https://choosealicense.com/licenses/mit)
```

### Comparing `ezregex-1.9.5/pyproject.toml` & `ezregex-1.9.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.5/PKG-INFO` & `ezregex-1.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ezregex
-Version: 1.9.5
+Version: 1.9.6
 Summary: A readable and intuitive way to generate Regular Expressions
 Project-URL: Documentation, https://github.com/smartycope/ezregex?tab=readme-ov-file#documentation
 Project-URL: Issues, https://github.com/smartycope/ezregex/issues
 Project-URL: Source, https://github.com/smartycope/ezregex
 Project-URL: Official Website, https://ezregex.org
 Author-email: Copeland Carter <smartycope@gmail.com>
 License-Expression: MIT
@@ -1050,14 +1050,24 @@
 
 ### Typing & Linting
 The updated method of doing this is to define all the EZRegex elements of a dialect in `elements.py`, and then add type hints and doc strings in the `elements.pyi` file. EZRegex elements that accept parameters are typed as functions (even though they're not), for both convenience for the user when using linter, and to give documentation in an easier way. EZRegex elements that don't accept parameters should be typed as EZRegex, and given documentation as a string on the line below it. This is *slightly* non-standard, but linters support it, as well as my documentation generator script, which parses the .pyi files. The elements can also be seperated into groups in the .pyi files by using `"Group: \<group name\>\n\<group description\>"`, which also gets parsed by the documentation script. The groups aren't used in the actual library, but are helpful in seperating the documentation, as well as used in [ezregex.org](http://ezregex.org)
 
 ### Dialects
 Because most regex dialects *are* 90% identical, a hidden "base" dialect is implemented, but it works a bit differently. It has an `elements.py` file, but it defines all the elements as a dict in the form of {"element_name": {"keyword": "arguements"}}. It then has a `load_dialect()` function, which is the only thing importable from it. The reason it's done this way is because `dialect` is a required parameter of the EZRegex constructor, so `load_dialect()` takes a `dialect` parameter, and constructs the base elements from it's dict and returns a new dict of initialized elements to be dumped into the global scope of the dialect. The `elements.py` file of a specific dialect can then remove any elements that it doesn't support (using the `del` keyword) and add/overwrite any it does support.
 
+There's also a _dialects.py file that has a dict for each dialect to describe the dialect-specific behavior of the EZRegex class, for example, in the JavaScript dialect, /'s are added to the beginning and end of the pattern, and flags are handled differently in each dialect. This has to be implemented directly into the EZRegex class. The dicts *would* be in the dialect folders themselves, but that causes all sorts of circular dependancies, so they're all just in the _dialects.py file.
+
+There's 4 parts to the dicts in the _dialects.py file:
+- `beginning` and `end`
+    - Plain strings which describe what to tack onto the beginning and end of the compiled pattern (but *before* flags are added)
+- `flag_func`
+    - A function that gets called with `final`, which is the final compiled pattern *with* `beginning` and `end` attached, and `flags`, which is a string of all the flags applied to the pattern. Internally, the flags are single digits, because flags usually are. They get passed to this function as a single string, which can be parsed and modified if necissary (it usually isn't)
+- `escape_chars`
+    - The characters that need to be escaped. Should be a byte string (i.e. b'...')
+
 ### Inverting
 There's actually 2 algorithms implemented for "inverting" regexs. The old algorithm regexs the regexs in a specific order to replace parts one at a time. This is just as nasty and horrifying as it sounds. Dispite it being a terrible, *terrible* solution, I actually got it to work decently well.
 
 Later, when I was reading up on abstract syntax trees, and scrolling around on PyPi, I realized that Python has one built in, and that it's available to use. I reimplemented the whole algorithm to instead parse the AST given by the built-in re lexer, and wrote my own parser on top of it, which works *much* better.
 
 Along the way, I also discovered, deep in the corners of the internet, 2 other Python libraries which do almost the same thing: `xeger` (regex backwards), and `sre_yield`. `xeger` technically works, however it tends to include unprintable characters, so it's output isn't very readable. `sre_yeild` is better, but it can be very slow, and is not quite the use case I'm going for. My invert algorithm is meant to be a debugging tool (though it doubles well for a testing tool), so it does things like detecting words (as opposed to seperate word characters) and inserts actual words, and doing the same for numbers and inserting `12345...`, as well as a couple other enhancements.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: ezregex Version: 1.9.5 Summary: A readable and
+Metadata-Version: 2.3 Name: ezregex Version: 1.9.6 Summary: A readable and
 intuitive way to generate Regular Expressions Project-URL: Documentation,
 https://github.com/smartycope/ezregex?tab=readme-ov-file#documentation Project-
 URL: Issues, https://github.com/smartycope/ezregex/issues Project-URL: Source,
 https://github.com/smartycope/ezregex Project-URL: Official Website, https://
 ezregex.org Author-email: Copeland Carter
 gmail.com> License-Expression: MIT License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
@@ -580,37 +580,52 @@
 "arguements"}}. It then has a `load_dialect()` function, which is the only
 thing importable from it. The reason it's done this way is because `dialect` is
 a required parameter of the EZRegex constructor, so `load_dialect()` takes a
 `dialect` parameter, and constructs the base elements from it's dict and
 returns a new dict of initialized elements to be dumped into the global scope
 of the dialect. The `elements.py` file of a specific dialect can then remove
 any elements that it doesn't support (using the `del` keyword) and add/
-overwrite any it does support. ### Inverting There's actually 2 algorithms
-implemented for "inverting" regexs. The old algorithm regexs the regexs in a
-specific order to replace parts one at a time. This is just as nasty and
-horrifying as it sounds. Dispite it being a terrible, *terrible* solution, I
-actually got it to work decently well. Later, when I was reading up on abstract
-syntax trees, and scrolling around on PyPi, I realized that Python has one
-built in, and that it's available to use. I reimplemented the whole algorithm
-to instead parse the AST given by the built-in re lexer, and wrote my own
-parser on top of it, which works *much* better. Along the way, I also
-discovered, deep in the corners of the internet, 2 other Python libraries which
-do almost the same thing: `xeger` (regex backwards), and `sre_yield`. `xeger`
-technically works, however it tends to include unprintable characters, so it's
-output isn't very readable. `sre_yeild` is better, but it can be very slow, and
-is not quite the use case I'm going for. My invert algorithm is meant to be a
-debugging tool (though it doubles well for a testing tool), so it does things
-like detecting words (as opposed to seperate word characters) and inserts
-actual words, and doing the same for numbers and inserting `12345...`, as well
-as a couple other enhancements. ### Tests Tests for a while now have just been
-in a single `tests.py` file, which was a giant pile of all the tests. I'm
-currently moving to use pytest. There's a `regexs.json` file (and a
-`replacements.json` file) that have a bunch of regexs, along with things
-they're supposed to match, and things they're not supposed to match, for
-testing. ## Installation EZRegex is distributed on [PyPI](https://pypi.org) as
-a universal wheel and is available on Linux, macOS and Windows and supports
-Python 3.10+ and PyPy. ```bash pip install ezregex ``` The import name is the
-same as the package name: ```python import ezregex as er ``` ## Todo See [the
-todo](todo.txt). I'm slowly moving these to [GitHub issues](https://github.com/
-smartycope/ezregex/issues), but for now, they're mostly still there ## License
-EZRegex is distributed under the [MIT License](https://choosealicense.com/
-licenses/mit)
+overwrite any it does support. There's also a _dialects.py file that has a dict
+for each dialect to describe the dialect-specific behavior of the EZRegex
+class, for example, in the JavaScript dialect, /'s are added to the beginning
+and end of the pattern, and flags are handled differently in each dialect. This
+has to be implemented directly into the EZRegex class. The dicts *would* be in
+the dialect folders themselves, but that causes all sorts of circular
+dependancies, so they're all just in the _dialects.py file. There's 4 parts to
+the dicts in the _dialects.py file: - `beginning` and `end` - Plain strings
+which describe what to tack onto the beginning and end of the compiled pattern
+(but *before* flags are added) - `flag_func` - A function that gets called with
+`final`, which is the final compiled pattern *with* `beginning` and `end`
+attached, and `flags`, which is a string of all the flags applied to the
+pattern. Internally, the flags are single digits, because flags usually are.
+They get passed to this function as a single string, which can be parsed and
+modified if necissary (it usually isn't) - `escape_chars` - The characters that
+need to be escaped. Should be a byte string (i.e. b'...') ### Inverting There's
+actually 2 algorithms implemented for "inverting" regexs. The old algorithm
+regexs the regexs in a specific order to replace parts one at a time. This is
+just as nasty and horrifying as it sounds. Dispite it being a terrible,
+*terrible* solution, I actually got it to work decently well. Later, when I was
+reading up on abstract syntax trees, and scrolling around on PyPi, I realized
+that Python has one built in, and that it's available to use. I reimplemented
+the whole algorithm to instead parse the AST given by the built-in re lexer,
+and wrote my own parser on top of it, which works *much* better. Along the way,
+I also discovered, deep in the corners of the internet, 2 other Python
+libraries which do almost the same thing: `xeger` (regex backwards), and
+`sre_yield`. `xeger` technically works, however it tends to include unprintable
+characters, so it's output isn't very readable. `sre_yeild` is better, but it
+can be very slow, and is not quite the use case I'm going for. My invert
+algorithm is meant to be a debugging tool (though it doubles well for a testing
+tool), so it does things like detecting words (as opposed to seperate word
+characters) and inserts actual words, and doing the same for numbers and
+inserting `12345...`, as well as a couple other enhancements. ### Tests Tests
+for a while now have just been in a single `tests.py` file, which was a giant
+pile of all the tests. I'm currently moving to use pytest. There's a
+`regexs.json` file (and a `replacements.json` file) that have a bunch of
+regexs, along with things they're supposed to match, and things they're not
+supposed to match, for testing. ## Installation EZRegex is distributed on
+[PyPI](https://pypi.org) as a universal wheel and is available on Linux, macOS
+and Windows and supports Python 3.10+ and PyPy. ```bash pip install ezregex ```
+The import name is the same as the package name: ```python import ezregex as er
+``` ## Todo See [the todo](todo.txt). I'm slowly moving these to [GitHub
+issues](https://github.com/smartycope/ezregex/issues), but for now, they're
+mostly still there ## License EZRegex is distributed under the [MIT License]
+(https://choosealicense.com/licenses/mit)
```

