# Comparing `tmp/beepy_web-0.9.6.tar.gz` & `tmp/beepy_web-0.9.7.tar.gz`

## Comparing `beepy_web-0.9.6.tar` & `beepy_web-0.9.7.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 beepy_web-0.9.6/.env.template
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 beepy_web-0.9.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 beepy_web-0.9.6/.python-version
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 beepy_web-0.9.6/requirements.txt
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/__init__.py
--rw-r--r--   0        0        0    14723 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/attrs.py
--rw-r--r--   0        0        0     7310 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/children.py
--rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/components.py
--rw-r--r--   0        0        0     8540 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/context.py
--rw-r--r--   0        0        0    21151 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/framework.py
--rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/listeners.py
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/router.py
--rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/style.py
--rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/tags.py
--rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/trackable.py
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/types.py
--rwxr-xr-x   0        0        0     5127 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/dev/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/dev/__main__.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/dev/example.html
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/dev/example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/modules/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/modules/actions.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/modules/context_menu.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/modules/local_storage.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/modules/modal.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/modules/plot.py
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/modules/table.py
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/modules/tabs.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/utils/__init__.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/utils/api.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/utils/asyncio.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/utils/common.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/utils/dev.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/utils/import_hooks.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/utils/internal.py
--rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/utils/js.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 beepy_web-0.9.6/beepy/utils/js_py.py
--rwxr-xr-x   0        0        0      691 2020-02-02 00:00:00.000000 beepy_web-0.9.6/scripts/publish.sh
--rw-r--r--   0        0        0   179387 2020-02-02 00:00:00.000000 beepy_web-0.9.6/web/package-lock.json
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 beepy_web-0.9.6/web/package.json
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 beepy_web-0.9.6/web/webpack.dev.js
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 beepy_web-0.9.6/web/webpack.prod.js
--rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 beepy_web-0.9.6/web/src/beepy.js
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 beepy_web-0.9.6/web/src/dev-server.js
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 beepy_web-0.9.6/web/src/files.js
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 beepy_web-0.9.6/web/src/index.js
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 beepy_web-0.9.6/web/src/main.css
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 beepy_web-0.9.6/web/src/python.js
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 beepy_web-0.9.6/web/src/utils.js
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 beepy_web-0.9.6/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 beepy_web-0.9.6/LICENSE
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 beepy_web-0.9.6/README.md
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 beepy_web-0.9.6/pyproject.toml
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 beepy_web-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 beepy_web-0.9.7/.env.template
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 beepy_web-0.9.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 beepy_web-0.9.7/.python-version
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 beepy_web-0.9.7/.readthedocs.yml
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 beepy_web-0.9.7/requirements.txt
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/__init__.py
+-rw-r--r--   0        0        0    14791 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/attrs.py
+-rw-r--r--   0        0        0     7310 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/children.py
+-rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/components.py
+-rw-r--r--   0        0        0     8540 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/context.py
+-rw-r--r--   0        0        0    21163 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/framework.py
+-rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/listeners.py
+-rw-r--r--   0        0        0     4641 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/router.py
+-rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/style.py
+-rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/tags.py
+-rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/trackable.py
+-rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/types.py
+-rwxr-xr-x   0        0        0     5181 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/dev/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/dev/__main__.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/dev/example.html
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/dev/example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/modules/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/modules/actions.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/modules/context_menu.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/modules/local_storage.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/modules/modal.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/modules/plot.py
+-rw-r--r--   0        0        0     5149 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/modules/table.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/modules/tabs.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/utils/__init__.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/utils/api.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/utils/asyncio.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/utils/common.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/utils/dev.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/utils/import_hooks.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/utils/internal.py
+-rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/utils/js.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/utils/js_py.py
+-rwxr-xr-x   0        0        0      691 2020-02-02 00:00:00.000000 beepy_web-0.9.7/scripts/publish.sh
+-rw-r--r--   0        0        0   179387 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/package-lock.json
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/package.json
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/webpack.dev.js
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/webpack.prod.js
+-rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/src/beepy.js
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/src/dev-server.js
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/src/files.js
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/src/index.js
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/src/main.css
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/src/python.js
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/src/utils.js
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 beepy_web-0.9.7/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 beepy_web-0.9.7/LICENSE
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 beepy_web-0.9.7/README.md
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 beepy_web-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 beepy_web-0.9.7/PKG-INFO
```

### Comparing `beepy_web-0.9.6/.pre-commit-config.yaml` & `beepy_web-0.9.7/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,30 @@
+exclude: '^(backend/users/migrations/|docs/)'
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.5.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: double-quote-string-fixer
       - id: check-toml
   - repo: https://github.com/pycqa/isort
     rev: 5.13.2
     hooks:
       - id: isort
   - repo: https://github.com/dosisod/refurb
-    rev: v1.27.0
+    rev: v2.0.0
     hooks:
       - id: refurb
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.1.11
+    rev: v0.4.1
     hooks:
       - id: ruff
         args: ['--unsafe-fixes']
   - repo: https://github.com/psf/black
-    rev: 23.12.1
+    rev: 24.4.0
     hooks:
       - id: black
 
 default_language_version:
   python: python3.11
```

### Comparing `beepy_web-0.9.6/beepy/__init__.py` & `beepy_web-0.9.7/beepy/__init__.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/beepy/attrs.py` & `beepy_web-0.9.7/beepy/attrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     from beepy.context import Context
 
     T = TypeVar('T')
 
 SPECIAL_CONVERT_ATTRIBUTES = {
     'contenteditable': lambda tag, val: (
         convert_boolean_attribute_value(val) if val == tag.mount_element.isContentEditable else val
-    )
+    ),
 }
 
 
 def convert_boolean_attribute_value(value):
     return '' if value else None
 
 
@@ -103,15 +103,16 @@
         enum=None,
         **kwargs,
     ):
         _type = kwargs.get('type')
 
         self.name = None
         self.const = const
-        assert not const or default is None, f'Const {type(self).__name__} cannot have initial value'
+        if const and default is not None:  # TODO: Add example for usage of const
+            raise ValueError(f'Const {type(self).__name__} cannot have initial value')
         self._initial_value = default
         self.required = required or const  # const attr must be also required
         self.notify = notify
         self.static = static
         self.move_on = move_on
         self.model = 'change' if model is True else model
         self.model_options = {'attribute': None} | (model_options or {})
```

### Comparing `beepy_web-0.9.6/beepy/children.py` & `beepy_web-0.9.7/beepy/children.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/beepy/components.py` & `beepy_web-0.9.7/beepy/components.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/beepy/context.py` & `beepy_web-0.9.7/beepy/context.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/beepy/framework.py` & `beepy_web-0.9.7/beepy/framework.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 from beepy.context import SpecialChild
 from beepy.types import AttrType, ContentType, Mounter, Renderer
 from beepy.utils import __CONFIG__, js, log
 from beepy.utils.common import NONE_TYPE, get_random_name, to_kebab_case
 from beepy.utils.dev import _debugger
 from beepy.utils.internal import _PY_TAG_ATTRIBUTE
 
-__version__ = '0.9.6'  # For internal development set to 0.0a0
+__version__ = '0.9.7'  # For internal development set to 0.0a0
 __CONFIG__['version'] = __version__
 
 
 _TAG_INITIALIZED = False
 
 
 class _MetaTag(_MetaComponent):
     _tag_classes: list[type[Tag]] = []
     __clean_class_attribute_names = ('_content_tag', '_static_children_tag')
 
-    def __new__(mcs, _name: str, bases: tuple, namespace: dict, **kwargs):  # noqa: PLR0912, PLR0915
+    def __new__(mcs, _name: str, bases: tuple, namespace: dict, **kwargs):  # noqa: PLR0912, PLR0915, C901
         namespace = namespace.copy()
         namespace.setdefault('__slots__', ())
         if '_content' in namespace:
             namespace['_static_content'] = namespace.pop('_content')
 
         # used for checking inheritance: attributes, methods, etc.
         # for example: extending classes Tag and WithRouter must produce correct state 'router'
@@ -273,15 +273,15 @@
 
         yield from super().__render__.original_fn(self, *args, **kwargs)
 
     def __init__(self, *args, **kwargs: AttrType):
         kwargs.setdefault('_load_children', False)
         super().__init__(*args, **kwargs)
 
-    def __new__(cls, *args, **kwargs):  # noqa: PLR0915, PLR0912 - Statements (60 > 50)  +  Branches (23 > 12)
+    def __new__(cls, *args, **kwargs):  # noqa: PLR0915, PLR0912, C901 - Statements (60 > 50)  +  Branches (23 > 12)
         if hasattr(getattr(cls, 'mount_element', None), _PY_TAG_ATTRIBUTE):
             return getattr(cls.mount_element, _PY_TAG_ATTRIBUTE)
 
         self: Tag = super().__new__(cls, *args, **kwargs)
 
         self._children = self._static_children.copy()
         self._content = self._static_content
```

### Comparing `beepy_web-0.9.6/beepy/listeners.py` & `beepy_web-0.9.7/beepy/listeners.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/beepy/router.py` & `beepy_web-0.9.7/beepy/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 
     @classmethod
     def parse(cls, path: str):
         result = cls()
 
         if path:
             if '#' in path:
-                path, hash = path.split('#', 1)
-                result.hash = '#' + hash
+                path, hash_ = path.split('#', 1)
+                result.hash = '#' + hash_
 
             if '?' in path:
                 path, search = path.split('?', 1)
                 result.search = '?' + search
 
             if path:
                 result.pathname = path
```

### Comparing `beepy_web-0.9.6/beepy/style.py` & `beepy_web-0.9.7/beepy/style.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/beepy/tags.py` & `beepy_web-0.9.7/beepy/tags.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/beepy/trackable.py` & `beepy_web-0.9.7/beepy/trackable.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/beepy/types.py` & `beepy_web-0.9.7/beepy/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 
     @abstractmethod
     def __view_value__(self):
         """This method will be called on render, must return serializable value"""
 
 
 class safe_html(str):
+    __slots__ = ()
+
     def __html__(self) -> str:
         return self
 
 
 def safe_html_content(function):
     @wraps(function)
     def content_wrapper(*args, **kwargs):
```

### Comparing `beepy_web-0.9.6/beepy/dev/__init__.py` & `beepy_web-0.9.7/beepy/dev/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import asyncio
 import functools
 import http.server
 import os
 import re
 import shutil
 import socketserver
+import subprocess
 import time
 from pathlib import Path
 from threading import Thread
 
 import dotenv
 from watchdog.events import FileSystemEventHandler
 from watchdog.observers import Observer
@@ -85,17 +86,17 @@
 
     def _handle_file_event(self, event):
         path: str = event.src_path.removeprefix(str(self.root_path)).removeprefix('/')
 
         print(f'[BeePy] Found file change: {path}')
         if self.developer_mode:
             if path.endswith('.py'):
-                os.system('hatch build')
+                subprocess.call('hatch build', shell=True)
             elif path.endswith('.js'):
-                os.system(f'cd {self.root_path}/web; npm run build; cd -')  # rebuild dist
+                subprocess.call(f'cd {self.root_path}/web; npm run build; cd -', shell=True)  # rebuild dist
             asyncio.run(self.ws_send('__'))
         else:
             asyncio.run(self.ws_send(path))
 
     def _watcher_start(self):
         event_handler = MonitorFolder(self)
         observer = Observer()
```

### Comparing `beepy_web-0.9.6/beepy/modules/context_menu.py` & `beepy_web-0.9.7/beepy/modules/context_menu.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             'cursor': 'pointer',
             'display': 'flex',
             'align-items': 'center',
             '&:hover': {
                 'background-color': '#2d2d2d',
                 'border-left': '4px solid #333',
             },
-        }
+        },
     )
 
 
 class ContextMenu(ul):
     visible = attr(default=False)
 
     pos_x = state(0)
@@ -57,15 +57,15 @@
             'box-shadow': '0 0 20px 0 #222',
             'opacity': 0,
             'transition': '0.2s',
             '&[visible]': {
                 'opacity': 1,
                 'visibility': 'visible',
             },
-        }
+        },
     )
 
     def show(self):
         self.visible = True
 
     def hide(self):
         self.visible = False
```

### Comparing `beepy_web-0.9.6/beepy/modules/local_storage.py` & `beepy_web-0.9.7/beepy/modules/local_storage.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/beepy/modules/modal.py` & `beepy_web-0.9.7/beepy/modules/modal.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                 ('width', 'height'): 'fit-content',
                 'display': 'flex',
                 'flex-direction': 'column',
                 ('justify-content', 'justify-items', 'align-items'): 'center',
                 'background-color': '#333',
                 'box-shadow': '0 0 1.5rem rgb(255 255 255 / 33%)',  # TODO: create beepy.style.rgb function
             },
-        }
+        },
     )
 
     children = [
         button_close := button('Close'),
     ]
 
     def show(self):
```

### Comparing `beepy_web-0.9.6/beepy/modules/table.py` & `beepy_web-0.9.7/beepy/modules/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
             TR(
                 data=[
                     *(
                         {'value': cell, 'view': col['view'](cell).__view_value__() if 'view' in col else cell}
                         for col, cell in self.parent._zip_column_row(row)
                     ),
                     [TableCellAction.components[action]() for action in self.parent.actions],
-                ]
+                ],
             )
             for row in self.rows
         ]
 
     def delete_row(self, index):
         self.rows.pop(index)
         self._rows.pop(index)
@@ -146,15 +146,15 @@
                 '&, th, td': {
                     'border': '1px solid #333',
                 },
                 'th, td': {
                     'padding': '8px',
                 },
             },
-        }
+        },
     )
 
     def _zip_column_row(self, row):
         if isinstance(row, dict):
             for col in self.head.columns:
                 yield col, row[col['id']]
         else:
```

### Comparing `beepy_web-0.9.6/beepy/modules/tabs.py` & `beepy_web-0.9.7/beepy/modules/tabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         styles={
             'padding': '6px 12px',
             'animation': 'fadeEffect 1s',
             'display': 'none',
             '&[visible]': {
                 'display': 'block',
             },
-        }
+        },
     )
 
     @attr()
     def id(self) -> str:
         return f'tab-{self.parent.name}/{self.tab_id}'
 
     parent: tabs
@@ -89,15 +89,15 @@
                         'background-color': '#222222',
                     },
                     '&[selected]': {
                         'background-color': '#3e3e3e',
                     },
                 },
             },
-        }
+        },
     )
 
     children = [
         tabs_titles := ul(),
     ]
 
     @property
@@ -107,15 +107,15 @@
 
     @classmethod
     def __class_declared__(cls):
         for tab_id, _tab_title in cls.tabs_titles.child.ref_children.items():
             _tab_title.on('click')(lambda _ul, _tab_id=tab_id: _ul.parent.select_tab(_tab_id))
 
     def mount(self):
-        for tab_id, _tab in self.tabs_list.items():
+        for tab_id in self.tabs_list:
             getattr(self.tabs_titles, tab_id)._link_parent_attrs(self)
 
         url = js.URL.new(js.location.href)
 
         selected = None
         if url.hash and url.hash.startswith(f'#tab-{self.name}/'):
             selected = self.select_tab(url.hash[len(f'#tab-{self.name}/') :])
```

### Comparing `beepy_web-0.9.6/beepy/utils/api.py` & `beepy_web-0.9.7/beepy/utils/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
         headers.update(
             {
                 'mode': 'no-cors',
                 'Content-Type': 'application/json',
                 'Access-Control-Allow-Headers': '*',
                 'Access-Control-Allow-Origin': '*',
-            }
+            },
         )
 
         response = await pyfetch(__CONFIG__['api_url'] + url, method=method, body=body, headers=headers, **opts)
 
         try:
             response.raise_for_status()
         except OSError as err:
```

### Comparing `beepy_web-0.9.6/beepy/utils/asyncio.py` & `beepy_web-0.9.7/beepy/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/beepy/utils/common.py` & `beepy_web-0.9.7/beepy/utils/common.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/beepy/utils/dev.py` & `beepy_web-0.9.7/beepy/utils/dev.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/beepy/utils/import_hooks.py` & `beepy_web-0.9.7/beepy/utils/import_hooks.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/beepy/utils/internal.py` & `beepy_web-0.9.7/beepy/utils/internal.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/beepy/utils/js.py` & `beepy_web-0.9.7/beepy/utils/js.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/beepy/utils/js_py.py` & `beepy_web-0.9.7/beepy/utils/js_py.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/scripts/publish.sh` & `beepy_web-0.9.7/scripts/publish.sh`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/web/package-lock.json` & `beepy_web-0.9.7/web/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.899982970027248%*

 * *Differences: {"'packages'": "{'': {'version': '0.9.7'}}", "'version'": "'0.9.7'"}*

```diff
@@ -12,15 +12,15 @@
                 "webpack": "^5.89.0",
                 "webpack-cli": "^5.1.4",
                 "webpack-dev-server": "^4.15.1",
                 "webpack-merge": "^5.10.0"
             },
             "license": "MIT",
             "name": "@kor0p/beepy",
-            "version": "0.9.6"
+            "version": "0.9.7"
         },
         "node_modules/@discoveryjs/json-ext": {
             "dev": true,
             "engines": {
                 "node": ">=10.0.0"
             },
             "integrity": "sha512-dBVuXR082gk3jsFp7Rd/JI4kytwGHecnCoTtXFb7DB6CNHp4rg5k1bhg0nWdLGLnOV71lmDzGQaLMy8iPLY0pw==",
@@ -4174,9 +4174,9 @@
             "dev": true,
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         }
     },
     "requires": true,
-    "version": "0.9.6"
+    "version": "0.9.7"
 }
```

### Comparing `beepy_web-0.9.6/web/package.json` & `beepy_web-0.9.7/web/package.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.9.7'"}*

```diff
@@ -31,9 +31,9 @@
     "name": "@kor0p/beepy",
     "scripts": {
         "build": "webpack --config webpack.prod.js",
         "start": "webpack serve --config webpack.dev.js",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch"
     },
-    "version": "0.9.6"
+    "version": "0.9.7"
 }
```

### Comparing `beepy_web-0.9.6/web/webpack.prod.js` & `beepy_web-0.9.7/web/webpack.prod.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/web/src/beepy.js` & `beepy_web-0.9.7/web/src/beepy.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -21,15 +21,15 @@
 const _script = document.currentScript
 let localConfig = {}
 if (!!window.beepy) {
     localConfig = window.beepy
 }
 
 class BeePy {
-    __version__ = '0.9.6'
+    __version__ = '0.9.7'
 
     pyodideIndexURL = null
     globals = null
     dev_server = dev_server
     dev_path = ''
     python_api = python
```

### Comparing `beepy_web-0.9.6/web/src/dev-server.js` & `beepy_web-0.9.7/web/src/dev-server.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/web/src/files.js` & `beepy_web-0.9.7/web/src/files.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/web/src/main.css` & `beepy_web-0.9.7/web/src/main.css`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/web/src/python.js` & `beepy_web-0.9.7/web/src/python.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/web/src/utils.js` & `beepy_web-0.9.7/web/src/utils.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/.gitignore` & `beepy_web-0.9.7/.gitignore`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/LICENSE` & `beepy_web-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.6/README.md` & `beepy_web-0.9.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # 🐝 BeePy
 
 [![NPM Package](https://img.shields.io/npm/v/@kor0p/beepy)](https://www.npmjs.com/package/@kor0p/beepy)
 [![PyPI Package](https://img.shields.io/pypi/v/beepy-web.svg)](https://pypi.org/project/beepy-web/)
-[![Documentation](https://cdn.jsdelivr.net/gh/Andre601/devins-badges@v3.x-mkdocs-material/assets/compact-minimal/built-with/mkdocs-material_vector.svg)](https://kor0p.github.io/BeePy/)
+[![Documentation](https://cdn.jsdelivr.net/gh/Andre601/devins-badges@v3.x-mkdocs-material/assets/compact-minimal/built-with/mkdocs-material_vector.svg)](https://bee-py.readthedocs.io/en/latest/)
 
 ## The _frontend_ web framework for python
 ### Thanks for [Pyodide](https://pyodide.org/) - port of Python to [Emscripten](https://emscripten.org/), based on [WASM](https://webassembly.org/).
 ### Use Python in browser to build modern frontend via BeePy!
 
 ## Try it out! [CodeSandBox](https://codesandbox.io/s/beepy-two-synced-counters-k5sm9j) and [BeePy Sandbox](https://kor0p.github.io/BeePy-examples/sandbox)
 
 ## Join our community at [Telegram chat](https://t.me/bee_py/)
+## [Documentation](https://kor0p.github.io/BeePy-examples/sandbox) | [PyPI](https://pypi.org/project/beepy-web/) | [NPM](https://www.npmjs.com/package/@kor0p/beepy)
 
 ## Local development:
 ### Install BeePy
 ### `pip install -U beepy-web[dev]`
 ### Then just start local server
 ### `python -m beepy.dev --create`
 ### And that's it!
```

### Comparing `beepy_web-0.9.6/PKG-INFO` & `beepy_web-0.9.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: beepy-web
-Version: 0.9.6
+Version: 0.9.7
 Summary: The modern frontend web framework for Python
-Project-URL: Homepage, https://bit.ly/beepy
+Project-URL: Homepage, https://beepy-web-ba63e5a12994.herokuapp.com/e/
 Project-URL: Repository, https://github.com/kor0p/BeePy
-Project-URL: Docs, https://kor0p.github.io/BeePy/
+Project-URL: Docs, https://bee-py.readthedocs.io/en/latest/
+Project-URL: Community, https://t.me/bee_py/
+Project-URL: Sandbox, https://kor0p.github.io/BeePy-examples/sandbox
+Project-URL: NPM, https://www.npmjs.com/package/@kor0p/beepy
 Author-email: kor0p <3.kor0p@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10.10
 Requires-Dist: boltons==23.1.1
 Requires-Dist: python-dotenv==1.0.0
@@ -16,29 +19,32 @@
 Requires-Dist: pre-commit; extra == 'contributing'
 Provides-Extra: dev
 Requires-Dist: micropip==0.3.0; extra == 'dev'
 Requires-Dist: pyodide-py==0.25.1; extra == 'dev'
 Requires-Dist: requests==2.31.0; extra == 'dev'
 Requires-Dist: watchdog==3.0.0; extra == 'dev'
 Requires-Dist: websockets==11.0.3; extra == 'dev'
+Provides-Extra: docs
+Requires-Dist: mkdocs-material==9.5.17; extra == 'docs'
 Description-Content-Type: text/markdown
 
 # 🐝 BeePy
 
 [![NPM Package](https://img.shields.io/npm/v/@kor0p/beepy)](https://www.npmjs.com/package/@kor0p/beepy)
 [![PyPI Package](https://img.shields.io/pypi/v/beepy-web.svg)](https://pypi.org/project/beepy-web/)
-[![Documentation](https://cdn.jsdelivr.net/gh/Andre601/devins-badges@v3.x-mkdocs-material/assets/compact-minimal/built-with/mkdocs-material_vector.svg)](https://kor0p.github.io/BeePy/)
+[![Documentation](https://cdn.jsdelivr.net/gh/Andre601/devins-badges@v3.x-mkdocs-material/assets/compact-minimal/built-with/mkdocs-material_vector.svg)](https://bee-py.readthedocs.io/en/latest/)
 
 ## The _frontend_ web framework for python
 ### Thanks for [Pyodide](https://pyodide.org/) - port of Python to [Emscripten](https://emscripten.org/), based on [WASM](https://webassembly.org/).
 ### Use Python in browser to build modern frontend via BeePy!
 
 ## Try it out! [CodeSandBox](https://codesandbox.io/s/beepy-two-synced-counters-k5sm9j) and [BeePy Sandbox](https://kor0p.github.io/BeePy-examples/sandbox)
 
 ## Join our community at [Telegram chat](https://t.me/bee_py/)
+## [Documentation](https://kor0p.github.io/BeePy-examples/sandbox) | [PyPI](https://pypi.org/project/beepy-web/) | [NPM](https://www.npmjs.com/package/@kor0p/beepy)
 
 ## Local development:
 ### Install BeePy
 ### `pip install -U beepy-web[dev]`
 ### Then just start local server
 ### `python -m beepy.dev --create`
 ### And that's it!
```

