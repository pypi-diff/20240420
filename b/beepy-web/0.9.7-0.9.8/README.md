# Comparing `tmp/beepy_web-0.9.7.tar.gz` & `tmp/beepy_web-0.9.8.tar.gz`

## Comparing `beepy_web-0.9.7.tar` & `beepy_web-0.9.8.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 beepy_web-0.9.7/.env.template
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 beepy_web-0.9.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 beepy_web-0.9.7/.python-version
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 beepy_web-0.9.7/.readthedocs.yml
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 beepy_web-0.9.7/requirements.txt
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/__init__.py
--rw-r--r--   0        0        0    14791 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/attrs.py
--rw-r--r--   0        0        0     7310 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/children.py
--rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/components.py
--rw-r--r--   0        0        0     8540 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/context.py
--rw-r--r--   0        0        0    21163 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/framework.py
--rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/listeners.py
--rw-r--r--   0        0        0     4641 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/router.py
--rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/style.py
--rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/tags.py
--rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/trackable.py
--rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/types.py
--rwxr-xr-x   0        0        0     5181 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/dev/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/dev/__main__.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/dev/example.html
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/dev/example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/modules/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/modules/actions.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/modules/context_menu.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/modules/local_storage.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/modules/modal.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/modules/plot.py
--rw-r--r--   0        0        0     5149 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/modules/table.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/modules/tabs.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/utils/__init__.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/utils/api.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/utils/asyncio.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/utils/common.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/utils/dev.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/utils/import_hooks.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/utils/internal.py
--rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/utils/js.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 beepy_web-0.9.7/beepy/utils/js_py.py
--rwxr-xr-x   0        0        0      691 2020-02-02 00:00:00.000000 beepy_web-0.9.7/scripts/publish.sh
--rw-r--r--   0        0        0   179387 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/package-lock.json
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/package.json
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/webpack.dev.js
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/webpack.prod.js
--rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/src/beepy.js
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/src/dev-server.js
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/src/files.js
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/src/index.js
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/src/main.css
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/src/python.js
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 beepy_web-0.9.7/web/src/utils.js
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 beepy_web-0.9.7/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 beepy_web-0.9.7/LICENSE
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 beepy_web-0.9.7/README.md
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 beepy_web-0.9.7/pyproject.toml
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 beepy_web-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 beepy_web-0.9.8/.env.template
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 beepy_web-0.9.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 beepy_web-0.9.8/.python-version
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 beepy_web-0.9.8/.readthedocs.yml
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 beepy_web-0.9.8/requirements.txt
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/__init__.py
+-rw-r--r--   0        0        0    14637 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/attrs.py
+-rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/children.py
+-rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/components.py
+-rw-r--r--   0        0        0     8577 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/context.py
+-rw-r--r--   0        0        0    21072 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/framework.py
+-rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/listeners.py
+-rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/router.py
+-rw-r--r--   0        0        0     8060 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/style.py
+-rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/tags.py
+-rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/trackable.py
+-rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/types.py
+-rwxr-xr-x   0        0        0     5190 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/dev/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/dev/__main__.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/dev/example.html
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/dev/example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/modules/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/modules/actions.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/modules/context_menu.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/modules/local_storage.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/modules/modal.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/modules/plot.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/modules/table.py
+-rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/modules/tabs.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/utils/__init__.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/utils/api.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/utils/asyncio.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/utils/common.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/utils/dev.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/utils/import_hooks.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/utils/internal.py
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/utils/js.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 beepy_web-0.9.8/beepy/utils/js_py.py
+-rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 beepy_web-0.9.8/scripts/dev.sh
+-rwxr-xr-x   0        0        0      691 2020-02-02 00:00:00.000000 beepy_web-0.9.8/scripts/publish.sh
+-rw-r--r--   0        0        0   179387 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/package-lock.json
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/package.json
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/webpack.dev.js
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/webpack.prod.js
+-rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/src/beepy.js
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/src/dev-server.js
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/src/files.js
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/src/index.js
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/src/main.css
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/src/python.js
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 beepy_web-0.9.8/web/src/utils.js
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 beepy_web-0.9.8/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 beepy_web-0.9.8/LICENSE
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 beepy_web-0.9.8/README.md
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 beepy_web-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 beepy_web-0.9.8/PKG-INFO
```

### Comparing `beepy_web-0.9.7/.pre-commit-config.yaml` & `beepy_web-0.9.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.7/beepy/__init__.py` & `beepy_web-0.9.8/beepy/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,36 +6,40 @@
     from beepy.utils import js
 
     sys.modules['js'] = js
     del sys, js
 
 import beepy.children  # must be loaded before .framework due to circular import
 import beepy.utils.import_hooks  # allows to use `import` for local files  # noqa: F401
-from beepy.attrs import attr, html_attr, state
+from beepy.attrs import attr, attr_prop, html_attr, state, state_move_on, state_static
 from beepy.components import Directive
 from beepy.context import SpecialChild
 from beepy.framework import Tag, __version__, empty_tag, mount
 from beepy.listeners import on
 from beepy.style import Style, import_css
 from beepy.tags import Body, Head
-from beepy.types import safe_html, safe_html_content
-from beepy.utils import __CONFIG__
+from beepy.types import Children, safe_html, safe_html_content
+from beepy.utils import __config__
 
 __all__ = [
     'Head',
     'Body',
     'Style',
     'import_css',
-    '__CONFIG__',
+    '__config__',
     'attr',
+    'attr_prop',
     'state',
+    'state_static',
+    'state_move_on',
     'html_attr',
     'on',
     'safe_html',
     'safe_html_content',
     'Directive',
     'SpecialChild',
     'Tag',
+    'Children',
     'empty_tag',
     'mount',
     '__version__',
 ]
```

### Comparing `beepy_web-0.9.7/beepy/attrs.py` & `beepy_web-0.9.8/beepy/attrs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from __future__ import annotations
 
+import builtins
 import keyword
 from collections import defaultdict
+from functools import partial
 from typing import TYPE_CHECKING, Any, get_type_hints
 
 from boltons.iterutils import first
 from boltons.typeutils import issubclass
 
 from beepy.types import AttrType, AttrValue
 from beepy.utils import log
 from beepy.utils.common import NONE_TYPE, call_handler_with_optional_arguments, to_kebab_case, wraps_with_name
 
 if TYPE_CHECKING:
-    import builtins
     from collections.abc import Callable, Sequence
     from typing import TypeVar
 
     from beepy.components import Component
     from beepy.context import Context
 
     T = TypeVar('T')
 
-SPECIAL_CONVERT_ATTRIBUTES = {
+_special_convert_attributes = {
     'contenteditable': lambda tag, val: (
         convert_boolean_attribute_value(val) if val == tag.mount_element.isContentEditable else val
     ),
 }
 
 
 def convert_boolean_attribute_value(value):
@@ -39,185 +40,107 @@
         el.setAttribute(name[:-1], value)
     elif not hasattr(el, name) or issubclass(type, bool):
         el.setAttribute(name, value)
     else:
         setattr(el, name, value)
 
 
-class attr:
+class state:
     __slots__ = (
         'name',
-        '_initial_value',
         'type',
-        'const',
         'required',
-        'notify',
-        'static',
-        'move_on',
         'model',
-        'model_options',
-        '_from_model_cache',
-        'fget',
-        'fset',
-        'fdel',
+        'model_opts',
         'handlers',
         'enum',
+        '_default',
+        '_from_model_cache',
         '_cache',
     )
 
-    _view = True
-    _set_on_render = False
-
     name: str | None
-    _initial_value: T
     type: builtins.type | None
-    const: bool
     required: bool
-    notify: bool
-    static: bool
-    move_on: bool
     model: str | None
-    model_options: dict[str, Any]
-    _from_model_cache: list[tuple[Component, attr, str | None]]
-    fget: Callable[[Component], T]
-    fset: Callable[[Component, T], None]
-    fdel: Callable[[Component], None]
+    model_opts: dict[str, Any]
     handlers: dict[str, list[Callable[[Component, T], None]]]
     enum: Sequence
 
+    _default: T
+    _from_model_cache: list[tuple[Component, state, str | None]]
     _cache: dict[Component, AttrType]
 
-    def __init__(  # noqa: PLR0913    # TODO: think about splitting logic
-        self,
-        default=None,
-        *,
-        const=False,
-        required=False,
-        notify=False,
-        static=False,
-        move_on=False,
-        model=None,
-        model_options=None,
-        fget=None,
-        fset=None,
-        fdel=None,
-        enum=None,
-        **kwargs,
-    ):
-        _type = kwargs.get('type')
+    def __init__(self, default=None, *, required=False, model=None, model_opts=None, enum=None, type=None):
+        # TO THINK: add `const` (removed feature)
 
         self.name = None
-        self.const = const
-        if const and default is not None:  # TODO: Add example for usage of const
-            raise ValueError(f'Const {type(self).__name__} cannot have initial value')
-        self._initial_value = default
-        self.required = required or const  # const attr must be also required
-        self.notify = notify
-        self.static = static
-        self.move_on = move_on
+        self._default = default
+        self.required = required
         self.model = 'change' if model is True else model
-        self.model_options = {'attribute': None} | (model_options or {})
+        self.model_opts = {'attribute': None} | (model_opts or {})
         self._from_model_cache = []
 
-        if default is None and _type is None:
+        if default is None and type is None:
             self.type = NONE_TYPE
         else:
-            if _type is None:
-                _type = default.type if self.model and isinstance(default, attr) else type(default)
-            self._set_type(_type)
-
-        # TODO: think on: is this needed?
-        # behaviour like @property
-        self.fget = fget
-        self.fset = fset
-        self.fdel = fdel
-        if fget:
-            self(fget)
+            if type is None:
+                type = default.type if self.model and isinstance(default, state) else builtins.type(default)
+            self._set_type(type)
 
         self.handlers = defaultdict(list)
         self.enum = enum
 
         self._cache = {}
 
     @property
     def _priority(self):
-        if self.move_on:
-            return 0
-        elif self.model:
-            return 2
-        else:
-            return 1
+        return 2 if self.model else 1
 
     @classmethod
     def _order_dict_by_priority(cls, dict_attrs):
         return dict(sorted(dict_attrs.items(), key=lambda item: item[1]._priority))
 
     def __get__(self, instance, owner=None):
         if instance is None:
             return self
-        return (self.fget or self._fget)(instance)
+        return self._fget(instance)
 
     def _fget(self, instance):
-        return self._cache.get(None if self.static else instance, self._initial_value)
-
-    def __call__(self, fget):
-        self.fget = fget
-        self.name = to_kebab_case(fget.__name__)
-        if self.type is NONE_TYPE:
-            type_hints = get_type_hints(fget)
-            if 'return' in type_hints:
-                self._set_type(type_hints['return'])
-        return self
+        return self._cache.get(instance, self._default)
 
     def __set__(self, instance, value, *, _prevent_model=False):
         current_value = self.__get__(instance)
-        if self.const and current_value is not None:
-            raise AttributeError
 
         if current_value == value:
             return
 
-        (self.fset or self._fset)(instance, value)
+        self._fset(instance, value)
 
         if instance._parent_ is not None:
             for handler in self.handlers['change']:
                 if _prevent_model and _prevent_model in (True, self) and handler.__name__.startswith('@attr'):
                     continue
                 call_handler_with_optional_arguments(handler, instance, {'value': value})
 
-        if self.notify:
-            instance.__notify__(self.name, self, value)
-
     def _set_first_value(self, instance, value, parent):  # noqa: ARG002 - unused `parent
         if self.model and (
-            isinstance(value, attr) and value.name is not None and (instance, self, None) not in value._from_model_cache
+            isinstance(value, state) and value.name and (instance, self, None) not in value._from_model_cache
         ):
             value._from_model_cache.append((instance, self, value.name))
             instance._kwargs.pop(self.name)
 
     def _fset(self, instance, value):
-        if self.fget is not None:
-            raise AttributeError
-
         if self.enum is not None and value not in self.enum:
             raise TypeError(f'Possible values: {self.enum}. Provided value: {value}')
 
-        self._cache[None if self.static else instance] = value
-
-    def setter(self, fset):
-        self.fset = fset
-        if self.type is NONE_TYPE:
-            self._set_type(first(get_type_hints(fset).values()))
-        return self
+        self._cache[instance] = value
 
     def __set_name__(self, owner, name):
-        if self._view:
-            self.name = to_kebab_case(name)
-        else:
-            self.name = name
+        self.name = name
 
     def _set_type(self, _type, *, raise_error=False):
         if hasattr(_type, '__origin__'):  # TODO: add support of strict check of type on change/etc
             _type = _type.__origin__
 
         if not isinstance(_type, type):
             error = f'Bad type for attribute: {_type!r}, {type(_type)}'
@@ -239,31 +162,31 @@
             setattr(component, name, self.__get__(component))
         return self
 
     def _get_type_instance(self):
         try:
             return self.type()
         except Exception as e:  # noqa: BLE001 - trying to call empty constructor
-            log.debug(
+            log.warn(
                 f'Got error when trying to empty-args constructor of {self.type}: {e}\n'
                 f'Will be better to set {self.name} not to None'
             )
 
     def _prepare_attribute_for_model(self, instance):
-        if attribute := self.model_options['attribute']:
+        if attribute := self.model_opts['attribute']:
             if callable(attribute):
                 return attribute(instance)
             return attribute
 
     def _set_model_value(self, instance, attr_, component: Component):
         initial_value = self.__get__(instance.parent if instance._parent_ is not None else component)
 
         if initial_value is None:
-            if self._initial_value is not None:
-                initial_value = self._initial_value
+            if self._default is not None:
+                initial_value = self._default
             elif self.type and (value_from_type := self._get_type_instance()) is not None:
                 initial_value = value_from_type
         if attribute_ := self._prepare_attribute_for_model(instance):
             initial_value = getattr(initial_value, attribute_)
         if initial_value is None:
             initial_value = ''
 
@@ -323,83 +246,149 @@
 
         if self.handlers['mount']:
             value = self.__get__(component)
             for handler in self.handlers['mount']:
                 call_handler_with_optional_arguments(handler, component, {'value': value})
 
     def __delete__(self, instance):
-        return (self.fdel or self._fdel)(instance)
+        return self._fdel(instance)
 
     def _fdel(self, instance):
-        if self.fget is not None:
-            raise AttributeError
-        if self.static:
-            return
-
         self._cache.pop(instance, None)
 
-    def deleter(self, fdel):
-        self.fdel = fdel
-        return self
-
     def __repr__(self):
-        return (
-            f'{self.name} = {type(self).__name__}'
-            f'(default={self._initial_value!r}, type={self.type}, static={self.static})'
-        )
+        return f'{self.name} = {type(self).__name__}(default={self._default!r}, type={self.type})'
 
     def __str__(self):
-        return f'{self.name}({self._initial_value!r})'
+        return f'{self.name}({self._default!r})'
 
-    def on(self, *triggers):
-        def wrapper(handler):
-            if self.static or self._from_model_cache:  # check if _from_model_cache is required
-                if not hasattr(handler, '_attrs_static_'):
-                    handler._attrs_static_ = defaultdict(list)
-                for trigger in triggers:
-                    handler._attrs_static_[trigger].append(self)
-
-            for trigger in triggers:
-                if handler in self.handlers[trigger]:
-                    raise AttributeError(f"This @on('{trigger}') handler is already set")
-            for trigger in triggers:
-                self.handlers[trigger].append(handler)
-            return handler
+    def _on_wrapper(self, handler, *, triggers):
+        for trigger in triggers:
+            if handler in self.handlers[trigger]:
+                raise AttributeError(f"This @on('{trigger}') handler is already set")
+        for trigger in triggers:
+            self.handlers[trigger].append(handler)
+        return handler
 
-        return wrapper
+    def on(self, *triggers):
+        return partial(self._on_wrapper, triggers=triggers)
 
     def _get_view_value(self, instance=None, value=None):
         if instance is not None:
             if value is not None:
                 raise ValueError('You cannot provide both instance and value arguments')
             value = self.__get__(instance)
 
-        if check_fn := SPECIAL_CONVERT_ATTRIBUTES.get(self.name):
+        if check_fn := _special_convert_attributes.get(self.name):
             return check_fn(instance, value)
 
         if issubclass(self.type, bool):
             return convert_boolean_attribute_value(value)
 
         # support for custom types for attr
         if isinstance(self.type, AttrValue):
             return value.__view_value__()
 
         return value
 
 
-class state(attr):
+class attr(state):
+    __slots__ = ()
+
+    def __set_name__(self, owner, name):
+        self.name = to_kebab_case(name)
+
+
+class state_move_on(state):
     __slots__ = ()
 
-    _view = False
+    _move_on = True
+    _priority = 0
 
 
-class html_attr(attr):
+class attr_prop(attr):
+    __slots__ = ('fget', 'fset', 'fdel')
+
+    fget: Callable[[Component], T]
+    fset: Callable[[Component, T], None]
+    fdel: Callable[[Component], None]
+
+    def __init__(self, *args, fget=None, fset=None, fdel=None, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.fget = fget
+        self.fset = fset
+        self.fdel = fdel
+        if fget:
+            self(fget)
+
+    def _fget(self, instance):
+        if self.fget is not None:
+            return self.fget(instance)
+        return super()._fget(instance)
+
+    def __call__(self, fget):
+        self.fget = fget
+        self.name = to_kebab_case(fget.__name__)
+        if self.type is NONE_TYPE:
+            type_hints = get_type_hints(fget)
+            if 'return' in type_hints:
+                self._set_type(type_hints['return'])
+        return self
+
+    def _fset(self, instance, value):
+        if self.fset is not None:
+            return self.fset(instance, value)
+        if self.fget is not None:
+            raise AttributeError('This attr have no setter')
+        return super()._fset(instance, value)
+
+    def setter(self, fset):
+        self.fset = fset
+        if self.type is NONE_TYPE:
+            self._set_type(first(get_type_hints(fset).values()))
+        return self
+
+    def _fdel(self, instance):
+        if self.fdel is not None:
+            return self.fdel(instance)
+        if self.fget is not None:
+            raise AttributeError('This attr have no deleter')
+        return super()._fdel(instance)
+
+    def deleter(self, fdel):
+        self.fdel = fdel
+        return self
+
+
+class state_static(state):
     __slots__ = ()
 
-    _set_on_render = True
+    def _fget(self, instance):  # noqa: ARG002 - unused `instance`
+        return super()._fget(None)
+
+    def _fset(self, instance, value):  # noqa: ARG002 - unused `instance`
+        super()._fset(None, value)
+
+    def _fdel(self, instance):  # noqa: ARG002 - unused `instance`
+        return  # Static state shouldn't be deleted by `__delete__`
+
+    def clear(self):
+        super()._fdel(None)
+
+    def _on_wrapper(self, handler, *, triggers):
+        if not hasattr(handler, '_attrs_static_'):
+            handler._attrs_static_ = defaultdict(list)
+        for trigger in triggers:
+            handler._attrs_static_[trigger].append(self)
+
+        return super()._on_wrapper(handler, triggers=triggers)
+
+
+class html_attr(attr):
+    __slots__ = ()
 
     def __init__(self, *args, name=None, **kwargs):
         super().__init__(*args, **kwargs)
         self.name = name
 
     def __set_name__(self, owner, name):
         if self.name is None:
@@ -445,8 +434,8 @@
     def __set__(self, instance, value, *, _prevent_model=False):
         super().__set__(instance, value, _prevent_model=_prevent_model)
         if instance is self.provider:
             for component in self.subscribers:
                 component.__notify__(self.name, self, value)
 
 
-__all__ = ['attr', 'state', 'html_attr']
+__all__ = ['state', 'attr', 'attr_prop', 'state_move_on', 'state_static', 'html_attr']
```

### Comparing `beepy_web-0.9.7/beepy/children.py` & `beepy_web-0.9.8/beepy/children.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from collections.abc import Callable, Iterable
-from typing import TYPE_CHECKING, Generic, TypeVar
+from typing import TYPE_CHECKING, Generic, Self, TypeVar, overload
 
 import beepy
 from beepy.components import Component
 from beepy.types import Children, ContentType, Renderer, WebBase
 from beepy.utils import js, log
-from beepy.utils.internal import _PY_TAG_ATTRIBUTE
+from beepy.utils.internal import _py_tag_attribute
 
 if TYPE_CHECKING:
     from beepy.context import Context
     from beepy.framework import Tag
 else:
     Tag = None
 
@@ -33,17 +33,14 @@
     def __repr__(self):
         return f'String({self.content})'
 
 
 class ContentWrapper(CustomWrapper):
     __slots__ = ('content', 'tag', 'mount_element', '_current_render', 'parent', 'mount_parent', 'children')
 
-    SHADOW_ROOTS = ('article', 'aside', 'blockquote', 'body', 'div', 'footer', 'h1', 'h2', 'h3', 'h4', 'h5', 'h6')
-    SHADOW_ROOTS += ('header', 'main', 'nav', 'p', 'section', 'span')
-
     content: Callable[[], ContentType | Tag]
     tag: Tag | None
     mount_element: js.HTMLElement | None
     _current_render: list[Renderer]
     parent: Tag | None
     mount_parent: js.HTMLElement | None
     children: list[Tag] | None
@@ -66,23 +63,23 @@
         self.mount_parent = element
         if self.tag:
             self.mount_element = self.tag._clone(parent).mount_element
             self.mount_parent.insertChild(self.mount_element, index)
         else:
             self.mount_element = js.document.createDocumentFragment()
             self.mount_parent.insertChild(self.mount_element, index)
-        setattr(self.mount_element, _PY_TAG_ATTRIBUTE, self)
+        setattr(self.mount_element, _py_tag_attribute, self)
 
     def _mount_children(self):
         content = self.content()
 
         if isinstance(content, beepy.framework.Tag):
             content = (content,)
         elif isinstance(content, Iterable) and not isinstance(content, str) and content:
-            content = tuple(content)
+            content = list(content)
             for _child in content[:]:
                 if not isinstance(_child, beepy.framework.Tag):
                     content = None
                     break
         else:
             content = None
 
@@ -114,15 +111,15 @@
                 self._current_render.pop()
             return
 
         result = self._render(self.content())
         if not isinstance(result, str):
             raise TypeError(f'Function {self.content} cannot return {result}!')
 
-        if self.tag or (self.parent and self.parent._shadow_root):
+        if self.tag:
             self.mount_element.innerHTML = result
         else:  # fragment can't be re-rendered
             self.mount_element.innerHTML = result
             current_html = self.mount_parent.innerHTML
             current_html_escaped = self._render(current_html)
             if result and result not in (current_html, current_html_escaped):
                 if current_html and not (self.parent and self.parent._raw_html):
@@ -155,15 +152,21 @@
         self.child = child
         self.inline_def = inline_def
         self._cache = {}
 
     def __repr__(self):
         return f'{type(self).__name__}(Tag.{self.name} = {self.child})'
 
-    def __get__(self, instance: Context | None, owner: type[Context] | None = None) -> ChildRef | C:
+    @overload
+    def __get__(self, instance: None, owner: type[Context]) -> Self: ...
+
+    @overload
+    def __get__(self, instance: Context | Tag, owner: type[Context] | None = None) -> C: ...
+
+    def __get__(self, instance: Context | Tag | None, owner: type[Context] | None = None) -> Self | C:
         if instance is None:
             return self
 
         if (result := self._cache.get(instance)) is not None:
             return result
 
         self._cache[instance] = self.child
@@ -221,14 +224,11 @@
         self.__set__(parent, copy)
         return copy
 
     def __set__(self, instance, value):
         if isinstance(value, Children):
             super().__set__(instance, value)
         else:
-            current_value = self.__get__(instance)
-            current_value[:] = value
-
+            self.__get__(instance)[:] = value
 
-from beepy.framework import Tag  # noqa: E402, isort: skip - circular import
 
 __all__ = ['CustomWrapper', 'StringWrapper', 'ContentWrapper', 'TagRef', 'ChildrenRef']
```

### Comparing `beepy_web-0.9.7/beepy/components.py` & `beepy_web-0.9.8/beepy/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,20 +85,20 @@
 
             if step in self.steps:
                 result = self.manager_fn(self.instance, step, args, kwargs)
             else:
                 raise ValueError(f'Invalid lifecycle step found: {step}. Available steps: {self.steps}')
 
 
-_COMPONENT_INITIALIZED = False
+_component_initialized = False
 
 
 class _MetaComponent(_MetaContext):
     def __new__(mcs, _name: str, bases: tuple, namespace: dict, **kwargs):
-        initialized = _COMPONENT_INITIALIZED  # As base classes is also declared here, we must be sure base class exists
+        initialized = _component_initialized  # As base classes is also declared here, we must be sure base class exists
 
         static_onchange_handlers = []
         _lifecycle_methods = []
 
         base_cls: type[Component] | type = type.__new__(mcs, _name, bases, {})
 
         for _attribute_name, child in tuple(mcs._clean_namespace(namespace)):
@@ -347,15 +347,15 @@
 
         if not isinstance(method, str):
             return wrapper(method)
 
         return wrapper
 
 
-_COMPONENT_INITIALIZED = True
+_component_initialized = True
 
 
 class Directive(Component, _root=True):
     _force_ref: bool = True
 
     element = state()
```

### Comparing `beepy_web-0.9.7/beepy/context.py` & `beepy_web-0.9.8/beepy/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from __future__ import annotations
 
 import enum
 from abc import ABCMeta
-from typing import TYPE_CHECKING, TypeVar
+from typing import TYPE_CHECKING, Self
 
 import beepy
-from beepy.attrs import attr
+from beepy.attrs import attr, html_attr, state, state_move_on
 from beepy.utils import js
 from beepy.utils.common import get_random_name, log10_ceil, to_kebab_case
 from beepy.utils.js_py import Interval, create_once_callable
 
 if TYPE_CHECKING:
     from beepy.types import AttrType
 
 _base_obj_dir = (*dir(object()), '__abstractmethods__')
-Self = TypeVar('Self', bound='Context')
-_CONTEXT_INITIALIZED = False
+_context_initialized = False
 
 
 class SpecialChild(enum.StrEnum):
     OVERWRITE = 'OVERWRITE'
     SUPER = 'SUPER'
     CONTENT = 'CONTENT'
 
@@ -29,15 +28,15 @@
     _wait_onload_interval: dict[Context, Interval] = {}
     _context_classes = []
     __clean_class_attribute_names = ()
     _current_render = {None: []}  # to prevent ValueError, for now
     _contexts: list[Context]
 
     def __new__(mcs, _name: str, bases: tuple, namespace: dict, **kwargs):
-        initialized = _CONTEXT_INITIALIZED  # if class Context is already defined
+        initialized = _context_initialized  # if class Context is already defined
 
         # used for checking inheritance: attributes, methods, etc.
         # for example: extending classes Tag and WithRouter must produce correct state 'router'
         # TODO: move this (or part of this) to _MetaContext.__init__
         base_cls: type[Context] | type = type.__new__(mcs, _name, bases, {})
 
         namespace = namespace.copy()
@@ -47,39 +46,39 @@
 
         if initialized and hasattr(beepy, 'children'):
             _children = beepy.children
 
             mcs._update_namespace_with_extra_attributes(namespace)
 
             for attribute_name, child in mcs._clean_namespace(namespace):
-                if isinstance(child, attr):
+                if isinstance(child, state):
                     static_attrs[attribute_name] = child
 
             for attribute_name, child in mcs._clean_cls_iter(base_cls):
                 new_attr = namespace.get(attribute_name)
-                if attribute_name not in static_attrs and isinstance(child, attr):
+                if attribute_name not in static_attrs and isinstance(child, state):
                     static_attrs[attribute_name] = child
 
                 if new_attr and (
-                    (isinstance(child, attr) and not isinstance(new_attr, attr))
+                    (isinstance(child, state) and not isinstance(new_attr, state))
                     or (isinstance(child, _children.ChildrenRef) and not isinstance(new_attr, _children.ChildrenRef))
                 ):
                     attrs_defaults[attribute_name] = namespace.pop(attribute_name)
 
         is_root = kwargs.get('_root')
         ctx_name = '' if is_root else kwargs.get('name')
         namespace['_meta_root'] = is_root
 
         if ctx_name or (initialized and not hasattr(base_cls, '_context_name_')):
             namespace['_context_name_'] = ctx_name or to_kebab_case(_name)
 
         cls: type[Context] | type = super().__new__(mcs, _name, bases, namespace)
 
         if initialized:
-            cls._static_attrs = attr._order_dict_by_priority(cls._static_attrs.copy() | static_attrs)
+            cls._static_attrs = state._order_dict_by_priority(cls._static_attrs.copy() | static_attrs)
             cls._attrs_defaults = cls._attrs_defaults.copy() | attrs_defaults
         else:
             cls._static_attrs = {}
             cls._attrs_defaults = {}
 
         cls._contexts = []
 
@@ -153,29 +152,29 @@
 
     _meta_root = False
 
     _id_: str
     _args: tuple[AttrType, ...]
     _kwargs: dict[str, AttrType]
 
-    _static_attrs: dict[str, attr]
+    _static_attrs: dict[str, state]
     _attrs_defaults: dict[str, AttrType]
-    attrs: dict[str, attr]
+    attrs: dict[str, state]
     _context_name_: str
 
     def __new__(cls, *args, **kwargs):
         self = super().__new__(cls)
         self.attrs = self._static_attrs.copy()
 
         # define some attributes here, not in __init__, because they are used for __hash__ method
         self._id_ = get_random_name(log10_ceil(len(self._contexts) * len(self.__class__._context_classes)))
         self._args = args
         self._kwargs = kwargs
 
-        if not _CONTEXT_INITIALIZED:
+        if not _context_initialized:
             return self
 
         for name, attribute in self.attrs.items():
             attribute._link_cmpt(name, self, force=False)
 
         return self
 
@@ -185,15 +184,15 @@
                 attribute._set_first_value(self, self._kwargs[name], parent)
         self._link_parent_attrs(parent)
 
     def _link_parent_attrs(self, parent):
         p_data = parent._attrs_defaults | parent._kwargs
 
         for name, attr_to_move_on in parent.attrs.items():
-            if attr_to_move_on.move_on:
+            if isinstance(attr_to_move_on, state_move_on):
                 attr_to_move_on._link_cmpt(name, self, force_cls_set=True)
                 if name in p_data:
                     self._attrs_defaults[name] = p_data[name]
 
     def __init__(self, *args, **kwargs: AttrType):
         self.__class__._contexts.append(self)
         data = self._attrs_defaults | kwargs
@@ -216,15 +215,15 @@
         pass
 
     @property
     def _attrs_values(self) -> dict[str, AttrType]:
         return {
             _attr.name: _attr._get_view_value(self)
             for _attr in self.attrs.values()
-            if _attr._view and not _attr._set_on_render
+            if isinstance(_attr, attr) and not isinstance(_attr, html_attr)
         }
 
     @property
     def _states(self) -> dict[str, AttrType]:
         return {_attr.name: _attr.__get__(self) for _attr in self.attrs.values()}
 
     @property
@@ -234,20 +233,20 @@
         # TODO: make self._kwargs as frozendict
         return self._args, self._kwargs
 
     def __hash__(self):
         # TODO: make force immutable this attributes
         return hash((self._context_name_, self._id_))
 
-    def __notify__(self, attr_name: str, attribute: attr, value: AttrType):
+    def __notify__(self, attr_name: str, attribute: state, value: AttrType):
         pass
 
     def _clone(self, parent=None) -> Self:
         clone = type(self)(*self._args, **self._kwargs)
         clone._clone_link_parent(parent)
         return clone
 
 
-_CONTEXT_INITIALIZED = True
+_context_initialized = True
 
 
 __all__ = ['SpecialChild', '_MetaContext', 'Context']
```

### Comparing `beepy_web-0.9.7/beepy/framework.py` & `beepy_web-0.9.8/beepy/framework.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 import traceback
 from collections.abc import Callable, Iterable
 from functools import cache
 from types import MethodType
 from typing import ClassVar
 
-from beepy.attrs import attr, state
+from beepy.attrs import state, state_move_on
 from beepy.children import ChildRef, Children, ContentWrapper, CustomWrapper, StringWrapper, TagRef
 from beepy.components import Component, _MetaComponent
 from beepy.context import SpecialChild
 from beepy.types import AttrType, ContentType, Mounter, Renderer
-from beepy.utils import __CONFIG__, js, log
+from beepy.utils import __config__, js, log
 from beepy.utils.common import NONE_TYPE, get_random_name, to_kebab_case
 from beepy.utils.dev import _debugger
-from beepy.utils.internal import _PY_TAG_ATTRIBUTE
+from beepy.utils.internal import _py_tag_attribute
 
-__version__ = '0.9.7'  # For internal development set to 0.0a0
-__CONFIG__['version'] = __version__
+__version__ = '0.9.8'  # For internal development set to 0.0a0
+__config__['version'] = __version__
 
 
-_TAG_INITIALIZED = False
+_tag_initialized = False
 
 
 class _MetaTag(_MetaComponent):
     _tag_classes: list[type[Tag]] = []
     __clean_class_attribute_names = ('_content_tag', '_static_children_tag')
 
     def __new__(mcs, _name: str, bases: tuple, namespace: dict, **kwargs):  # noqa: PLR0912, PLR0915, C901
@@ -33,15 +33,15 @@
         if '_content' in namespace:
             namespace['_static_content'] = namespace.pop('_content')
 
         # used for checking inheritance: attributes, methods, etc.
         # for example: extending classes Tag and WithRouter must produce correct state 'router'
         mock_cls: type[Tag] | type = type.__new__(mcs, _name, bases, {})
 
-        initialized = _TAG_INITIALIZED  # As base classes is also declared here, we must be sure base class exists
+        initialized = _tag_initialized  # As base classes is also declared here, we must be sure base class exists
 
         is_root = kwargs.get('_root')
         tag_name = '' if is_root else kwargs.get('name')
         namespace['_meta_root'] = is_root
 
         if tag_name or (initialized and not hasattr(mock_cls, '_tag_name_')):
             namespace['_tag_name_'] = to_kebab_case(tag_name or _name)
@@ -155,44 +155,42 @@
 
         cls._tags = []
 
         mcs._tag_classes.append(cls)
 
         if initialized and 'mount' in kwargs:
             cls._root_parent = None
-            setattr(cls.mount_element, _PY_TAG_ATTRIBUTE, cls())
+            setattr(cls.mount_element, _py_tag_attribute, cls())
 
         if cls._meta_root:
             cls.__root_declared__()
         else:
             cls.__class_declared__()
 
         return cls
 
 
 class Tag(Component, metaclass=_MetaTag, _root=True):
     # TODO: add docstrings
 
     __slots__ = (
         '_content',
-        '_shadow_root',
         'mount_parent',
         '_mount_finished_',
         'mount_element',
         '_children',
         '_children_element',
         '_children_tag',
     )
 
     _root_parent: Tag = None  # see function mount in the bottom
 
     _static_content: ContentType = ''
 
     _content: ContentType
-    _shadow_root: js.HTMLElement
     _ref: TagRef | None
     _force_ref: bool = False
 
     _tag_name_: str
     _tags: list[Tag]
     mount_element: js.HTMLElement
     mount_parent: js.HTMLElement
@@ -274,16 +272,16 @@
         yield from super().__render__.original_fn(self, *args, **kwargs)
 
     def __init__(self, *args, **kwargs: AttrType):
         kwargs.setdefault('_load_children', False)
         super().__init__(*args, **kwargs)
 
     def __new__(cls, *args, **kwargs):  # noqa: PLR0915, PLR0912, C901 - Statements (60 > 50)  +  Branches (23 > 12)
-        if hasattr(getattr(cls, 'mount_element', None), _PY_TAG_ATTRIBUTE):
-            return getattr(cls.mount_element, _PY_TAG_ATTRIBUTE)
+        if hasattr(getattr(cls, 'mount_element', None), _py_tag_attribute):
+            return getattr(cls.mount_element, _py_tag_attribute)
 
         self: Tag = super().__new__(cls, *args, **kwargs)
 
         self._children = self._static_children.copy()
         self._content = self._static_content
 
         children_argument: Callable | ContentType = kwargs.get('children') or args
@@ -330,28 +328,27 @@
                 continue
             value: Component | Children
             child = value._as_child(self, exists_ok=True)
             child.__set_name__(self, key)
             setattr(type(self), key, child)
             self._children.append(child)
 
-        self._shadow_root = None
         self.mount_parent = None
         self._mount_finished_ = False
 
         if not hasattr(self, 'mount_element'):
             self.mount_element = js.document.createElement(self._tag_name_)
-        if getattr(self.mount_element, _PY_TAG_ATTRIBUTE, None):
+        if getattr(self.mount_element, _py_tag_attribute, None):
             raise ValueError(f'Coping or using as child is not allowed for "{self._tag_name_}"')
         else:
-            setattr(self.mount_element, _PY_TAG_ATTRIBUTE, self)
+            setattr(self.mount_element, _py_tag_attribute, self)
         if self._static_children_tag:
             self._children_tag = self._static_children_tag._clone(self)
             self._children_element = self._children_tag.mount_element
-            setattr(self._children_element, _PY_TAG_ATTRIBUTE, self)
+            setattr(self._children_element, _py_tag_attribute, self)
         else:
             self._children_tag = None
             self._children_element = self.mount_element
 
         return self
 
     def __repr__(self):
@@ -371,15 +368,15 @@
                 return self._ref
             else:
                 raise TypeError(f'Tag {self._tag_name_} already is child')
         ref = TagRef(self, inline_def=inline_def)
         self._set_ref(parent, ref)
         return ref
 
-    def __notify__(self, attr_name: str, attribute: attr, value: AttrType):
+    def __notify__(self, attr_name: str, attribute: state, value: AttrType):
         super().__notify__(attr_name, attribute, value)
         self.__render__()
 
     def _set_ref(self, parent: Tag | None, ref: TagRef):
         super()._set_ref(parent, ref)
         if ref.inline_def:
             setattr(type(parent), ref.name, self)
@@ -473,15 +470,15 @@
                 child = child.content.__func__
                 if child.__name__ == 'content':
                     child = SpecialChild.CONTENT
 
             if child == SpecialChild.CONTENT:
                 child = self.content
 
-            if isinstance(child, attr):
+            if isinstance(child, state):
 
                 def child(s, _n=child.name):
                     return getattr(s, _n)
 
             if isinstance(child, Component) and child in self._children and child._ref is not None:
                 # using Component as descriptor/just child; this allows save reference from parent to new copy of child
                 child = child._ref._update_child(self, self._children.index(child))
@@ -508,15 +505,15 @@
         try:
             return _MetaTag._current_render[self._root_parent]
         except KeyError as e:
             _debugger(e)
             raise ValueError('It looks like element is not mounted correctly, please see the docs') from None
 
 
-_TAG_INITIALIZED = True
+_tag_initialized = True
 
 
 @cache
 def empty_tag(name):
     return _MetaTag(name, (Tag,), {}, name=name, content_tag=None)
 
 
@@ -531,16 +528,16 @@
 
     js.beepy.stopLoading()
     if clear or js.beepy.dev_server.started:
         root.innerHTML = ''
     js.beepy.startLoading(mountPoint=root)
 
     name = root.tagName.lower()
-    parent = _MetaTag(name, (Tag,), {'_root_parent': state(type=Tag, move_on=True)}, name=name, content_tag=None)()
-    parent._attrs_defaults['_root_parent'] = parent.__class__._root_parent._initial_value = parent
+    parent = _MetaTag(name, (Tag,), {'_root_parent': state_move_on(type=Tag)}, name=name, content_tag=None)()
+    parent._attrs_defaults['_root_parent'] = parent.__class__._root_parent._default = parent
     parent.mount_element = root
     element._link_parent_attrs(parent)
 
     _MetaTag._top_mount(element)
 
     if not js.document.title:
         js.document.title = 'BeePy'
```

### Comparing `beepy_web-0.9.7/beepy/listeners.py` & `beepy_web-0.9.8/beepy/listeners.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from collections import defaultdict
 from functools import partial, wraps
 from types import MethodType
 from typing import TYPE_CHECKING, Any
 
 from beepy.utils import js, to_js
 from beepy.utils.common import nested_copy
-from beepy.utils.internal import _PY_TAG_ATTRIBUTE
+from beepy.utils.internal import _py_tag_attribute
 from beepy.utils.js_py import create_proxy
 
 if TYPE_CHECKING:
     from collections.abc import Callable
 
     from beepy.components import Component
 
@@ -139,15 +139,15 @@
         return data
 
     def _after_call(self, cmpt, event):
         for dependent in cmpt._dependents:
             # TODO: move to other place
             dependent.__render__()
 
-        getattr(event.currentTarget, _PY_TAG_ATTRIBUTE, cmpt).__render__()
+        getattr(event.currentTarget, _py_tag_attribute, cmpt).__render__()
 
     def _make_listener(self, event_name: str, cmpt: Component):
         if inspect.iscoroutinefunction(self._callback):
 
             @wraps(self._callback)
             async def method(event):
                 return await self._a_call(cmpt, event)
```

### Comparing `beepy_web-0.9.7/beepy/router.py` & `beepy_web-0.9.8/beepy/router.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from __future__ import annotations
 
 import re
 from dataclasses import dataclass
 from re import Match
 
-from beepy import Tag
-from beepy.attrs import html_attr, state
-from beepy.listeners import on
+from beepy import Tag, html_attr, on, state, state_move_on
 from beepy.tags import a
 from beepy.types import Children
 from beepy.utils import js
 from beepy.utils.dev import _debugger
 from beepy.utils.internal import lazy_import_cls, reload_requirements
 from beepy.utils.js_py import push_url
 
 
 class WithRouter:
-    match: Match = state(move_on=True)
-    router: Router = state(move_on=True)
+    match: Match = state_move_on()
+    router: Router = state_move_on()
 
 
 @dataclass
 class Path:
     # TODO: move to utils?
     pathname: str = ''
     search: str = ''
```

### Comparing `beepy_web-0.9.7/beepy/style.py` & `beepy_web-0.9.8/beepy/style.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from collections.abc import Iterable
 from typing import Any, Protocol
 
 from beepy.context import Context
-from beepy.framework import __CONFIG__, Tag, attr, state
+from beepy.framework import Tag, __config__, attr, state
 from beepy.tags import Head
 from beepy.types import AttrValue, safe_html, safe_html_content
 from beepy.utils import js
 from beepy.utils.common import MISSING, get_random_name, log10_ceil, safe_issubclass, to_kebab_case
 
 
 def dict_of_properties_to_css(properties):
@@ -175,15 +175,15 @@
             'render_states': True,
             'render_children': True,
             'get_vars_callback': get_vars,
         } | options
 
     def _mount_(self, element, parent, index=None):
         self.real_parent = parent
-        if __CONFIG__['style_head']:
+        if __config__['style_head']:
             super()._mount_(Head.mount_element, Head)
         else:
             super()._mount_(element, parent, index)
 
     def _unmount_(self, element, parent, *, _unsafe=False):
         return super()._unmount_(element, parent, _unsafe=True)
 
@@ -233,21 +233,21 @@
     def var(self, name, new_value=MISSING):
         parent = self.real_parent
         if not parent:
             return
 
         if new_value is MISSING:
             return parent.style_id.vars[name]
+
+        if new_value is None:
+            del parent.style_id.vars[name]
         else:
-            if new_value is None:
-                del parent.style_id.vars[name]
-            else:
-                parent.style_id.vars[name] = new_value
-            if parent._mount_finished_:
-                parent.__render__()
+            parent.style_id.vars[name] = new_value
+        if parent._mount_finished_:
+            parent.__render__()
 
 
 def import_css(file_path):
     return js.beepy.addElement(
         js.document.head,
         'link',
         href=js.beepy.files.getPathWithCurrentPathAndOrigin(file_path),
```

### Comparing `beepy_web-0.9.7/beepy/tags.py` & `beepy_web-0.9.8/beepy/tags.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Any
 
 from boltons.typeutils import make_sentinel
 
 from beepy.attrs import attr, html_attr, state
-from beepy.children import Children
 from beepy.framework import Tag
-from beepy.utils import __CONFIG__, js
+from beepy.types import Children
+from beepy.utils import __config__, js
 from beepy.utils.common import AnyOfType, get_random_name
 
 AUTO_ID = make_sentinel(var_name='AUTO_ID')
 
 
 class html_tag(Tag, _root=True, content_tag=None):
     contenteditable = html_attr(type=bool)
     id = html_attr(type=str)
     class_ = html_attr(type=str)
 
     def _set_ref(self, parent, ref):
         super()._set_ref(parent, ref)
-        if type(self).id is html_tag.id and (self.id is AUTO_ID or (__CONFIG__['inputs_auto_id'] and self.id is None)):
+        if type(self).id is html_tag.id and (self.id is AUTO_ID or (__config__['inputs_auto_id'] and self.id is None)):
             # TODO: replace 5 and 2 with some log value
             self.id = f'{ref.name or get_random_name(5)}-{get_random_name(2)}'
 
 
 def by__input_id(input_tag):
     return input_tag.id.rsplit('-', 1)[0]
 
@@ -222,15 +222,16 @@
     def _as_child(self, parent: Tag | None, *, exists_ok=False, inline_def=False):  # noqa: ARG002 - args for overriding
         return super()._as_child(parent, exists_ok=True, inline_def=inline_def)
 
 
 class Head(StandaloneTag, name='head', mount=js.document.head):
     title = state()
 
-    def render(self):
+    @title.on('change')
+    def _upd_title(self):
         if self.title:
             js.document.title = self.title
 
 
 Head = Head()
```

### Comparing `beepy_web-0.9.7/beepy/trackable.py` & `beepy_web-0.9.8/beepy/trackable.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.7/beepy/types.py` & `beepy_web-0.9.8/beepy/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from abc import ABC, abstractmethod
 from collections.abc import Iterable
 from functools import wraps
 from typing import TYPE_CHECKING
 
 from beepy.trackable import TrackableList
-from beepy.utils import __CONFIG__, js
+from beepy.utils import __config__, js
 from beepy.utils.common import escape_html
 
 if TYPE_CHECKING:
     from beepy.children import ChildrenRef
     from beepy.framework import Tag
 
 
@@ -54,15 +54,15 @@
     __slots__ = ()
 
     def _render(self, value: str | Iterable[str]) -> str:
         if isinstance(value, safe_html):
             return value.__html__()
 
         if isinstance(value, str):
-            return escape_html(value, whitespace=__CONFIG__['html_replace_whitespaces'])
+            return escape_html(value, whitespace=__config__['html_replace_whitespaces'])
 
         if isinstance(value, Iterable):
             return ''.join(self._render(child) for child in value)
 
         return str(value)
 
     @abstractmethod
```

### Comparing `beepy_web-0.9.7/beepy/dev/__init__.py` & `beepy_web-0.9.8/beepy/dev/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 
 class DevServer:
     def __init__(self, *, root_path=None, parse_cmd=True):
         self.websockets = []
         self.root_path = root_path
         self.observer = None
-        self.developer_mode = 'DEVELOPMENT' in os.environ
+        self.developer_mode = os.environ.get('DEVELOPMENT') == '1'
         if parse_cmd:
             self._handle_cmd_args()
 
     def _handle_cmd_args(self):
         parser = argparse.ArgumentParser(prog='beepy.dev', description='Simple dev server for BeePy')
         parser.add_argument(
             '-d', '--root-dir', default=Path.cwd(), help='Root directory to start server and watch file changes'
```

### Comparing `beepy_web-0.9.7/beepy/modules/context_menu.py` & `beepy_web-0.9.8/beepy/modules/context_menu.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from __future__ import annotations
 
-from beepy.attrs import attr, state
-from beepy.listeners import on
-from beepy.style import Style
+from beepy import Style, attr, on, state
 from beepy.tags import Body, div, hr, li, ul
 from beepy.utils import js
 
 
 class MenuDivider(hr):
     default_style = Style(
         border_bottom='1px solid #eee',
```

### Comparing `beepy_web-0.9.7/beepy/modules/local_storage.py` & `beepy_web-0.9.8/beepy/modules/local_storage.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.7/beepy/modules/modal.py` & `beepy_web-0.9.8/beepy/modules/modal.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from collections.abc import Callable
 
-from beepy import Tag
-from beepy.attrs import attr, state
-from beepy.listeners import on
-from beepy.style import Style
+from beepy import Style, Tag, attr, on, state
 from beepy.tags import Body, button, div
 
 
 class Modal(Tag, name='modal', content_tag='h2', children_tag='modal-content'):
     visible = attr(default=False)
     on_close = state(type=Callable[[], None])  # TODO: add example
```

### Comparing `beepy_web-0.9.7/beepy/modules/table.py` & `beepy_web-0.9.8/beepy/modules/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from __future__ import annotations
 
 from typing import Literal, TypeVar
 
-from beepy.attrs import state
-from beepy.children import Children
-from beepy.listeners import on
+from beepy import Children, Style, on, state
 from beepy.modules.actions import Action
-from beepy.style import Style
 from beepy.tags import table, tbody, td, th, thead, tr
 from beepy.utils.asyncio import ensure_sync_many
 from beepy.utils.common import call_handler_with_optional_arguments
 
 T = TypeVar('T')
```

### Comparing `beepy_web-0.9.7/beepy/modules/tabs.py` & `beepy_web-0.9.8/beepy/modules/tabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from __future__ import annotations
 
 from boltons.iterutils import first
 
-from beepy import Tag
-from beepy.attrs import attr, html_attr, state
-from beepy.style import Style
+from beepy import Style, Tag, attr, attr_prop, html_attr, state
 from beepy.tags import div, ul
 from beepy.utils import js
 from beepy.utils.js_py import replace_url
 
 
 class tab(div, name='tab'):
     tab_id = state(type=str)
@@ -22,15 +20,15 @@
             'display': 'none',
             '&[visible]': {
                 'display': 'block',
             },
         },
     )
 
-    @attr()
+    @attr_prop()
     def id(self) -> str:
         return f'tab-{self.parent.name}/{self.tab_id}'
 
     parent: tabs
 
     def _set_ref(self, parent, ref):
         super()._set_ref(parent, ref)
```

### Comparing `beepy_web-0.9.7/beepy/utils/api.py` & `beepy_web-0.9.8/beepy/utils/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import dataclasses
 import json
 from datetime import datetime
 from http import HTTPStatus
 from http.client import HTTPException
 
-from beepy.utils.internal import __CONFIG__
+from beepy.utils.internal import __config__
 from beepy.utils.js_py import IN_BROWSER
 
 
 class UpgradedJSONEncoder(json.JSONEncoder):  # TODO: consider on rewriting json.JSONEncoder
     def default(self, o):
         if dataclasses.is_dataclass(o):
             return dataclasses.asdict(o)
         if isinstance(o, datetime):
-            return o.strftime(__CONFIG__['default_datetime_format'])
+            return o.strftime(__config__['default_datetime_format'])
         return super().default(o)
 
 
 if IN_BROWSER:
     from pyodide.http import pyfetch
 
     async def request(url, method='GET', body=None, headers=None, **opts):
@@ -32,15 +32,15 @@
                 'mode': 'no-cors',
                 'Content-Type': 'application/json',
                 'Access-Control-Allow-Headers': '*',
                 'Access-Control-Allow-Origin': '*',
             },
         )
 
-        response = await pyfetch(__CONFIG__['api_url'] + url, method=method, body=body, headers=headers, **opts)
+        response = await pyfetch(__config__['api_url'] + url, method=method, body=body, headers=headers, **opts)
 
         try:
             response.raise_for_status()
         except OSError as err:
             raise HTTPException(err) from err
 
         return (await response.json()) if method in ('GET', 'PUT', 'POST') else (await response.text())
@@ -53,15 +53,15 @@
             body = json.dumps(body, cls=UpgradedJSONEncoder)
 
         if headers is None:
             headers = {}
 
         # TODO: check opts argument compatibility
 
-        response = requests.request(method, __CONFIG__['api_url'] + url, data=body, headers=headers)
+        response = requests.request(method, __config__['api_url'] + url, data=body, headers=headers)
 
         if int(response.status_code) >= HTTPStatus.BAD_REQUEST:
             raise HTTPException(response.status_code)
 
         return response.json() if method in ('GET', 'PUT', 'POST') else response.text
```

### Comparing `beepy_web-0.9.7/beepy/utils/asyncio.py` & `beepy_web-0.9.8/beepy/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.7/beepy/utils/common.py` & `beepy_web-0.9.8/beepy/utils/common.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.7/beepy/utils/dev.py` & `beepy_web-0.9.8/beepy/utils/dev.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.7/beepy/utils/import_hooks.py` & `beepy_web-0.9.8/beepy/utils/import_hooks.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from importlib.abc import MetaPathFinder
 from importlib.util import spec_from_file_location
 from pathlib import Path
 
 from pyodide.ffi import JsException
 
 from beepy.utils.dev import _debugger
-from beepy.utils.internal import __CONFIG__, BEEPY_ROOT_PACKAGE
+from beepy.utils.internal import __config__, _beepy_root_package
 from beepy.utils.js_py import IN_BROWSER, js
 
-requirements = __CONFIG__['requirements']
-MODULES_NOT_EXISTING_ON_SERVER = [
-    BEEPY_ROOT_PACKAGE,
+requirements = __config__['requirements']
+_modules_not_existing_on_server = [
+    _beepy_root_package,
     *(requirements() if callable(requirements) else requirements),
     '_hashlib',  # TODO: FIX THIS...
     '_strptime',
     'unicodedata',
     'pprint',
     'numpy',
     'matplotlib',
@@ -49,26 +49,26 @@
 
 
 class ServerFinder(MetaPathFinder):
     def find_spec(self, fullname, path, target=None):  # noqa: ARG002 - override of MetaPathFinder
         if path and any(p.startswith('/lib') for p in path):
             return
 
-        if Path(f'/lib/python3.11/site-packages/{fullname}').exists() or fullname in MODULES_NOT_EXISTING_ON_SERVER:
+        if Path(f'/lib/python3.11/site-packages/{fullname}').exists() or fullname in _modules_not_existing_on_server:
             return
 
         current_path = js.beepy.files._lastLoadedFile
 
         try:
             js.beepy.loadModule(fullname)
         except JsException as err:
             js.beepy.files._lastLoadedFile = current_path
             _debugger(err)
-            MODULES_NOT_EXISTING_ON_SERVER.append(fullname)
+            _modules_not_existing_on_server.append(fullname)
             return
 
         return spec_from_file_location(fullname)
 
 
 if IN_BROWSER:
     sys.meta_path.insert(0, ServerFinder())
-    sys.path.append(BEEPY_ROOT_PACKAGE)
+    sys.path.append(_beepy_root_package)
```

### Comparing `beepy_web-0.9.7/beepy/utils/js.py` & `beepy_web-0.9.8/beepy/utils/js.py`

 * *Files 4% similar despite different names*

```diff
@@ -314,72 +314,72 @@
 #       .       #
 # . . . . . . . #
 #       .       #
 #       .       #
 #################
 
 
-EVENT_LISTENERS = {}
+_event_listeners = {}
 
 
 def add_event_listener(elt, event, listener):
     """Wrapper for JavaScript's addEventListener() which automatically manages the lifetime
     of a JsProxy corresponding to the listener param.
     """
     proxy = create_proxy(listener)
-    EVENT_LISTENERS[(elt.js_id, event, listener)] = proxy
+    _event_listeners[(elt.js_id, event, listener)] = proxy
     elt.addEventListener(event, proxy)
 
 
 def remove_event_listener(elt, event, listener):
     """Wrapper for JavaScript's removeEventListener() which automatically manages the lifetime
     of a JsProxy corresponding to the listener param.
     """
-    elt.removeEventListener(event, EVENT_LISTENERS.pop((elt.js_id, event, listener)))
+    elt.removeEventListener(event, _event_listeners.pop((elt.js_id, event, listener)))
 
 
-TIMEOUTS: dict[int, Callable] = {}
+_timeouts: dict[int, Callable] = {}
 
 
 def set_timeout(callback, timeout):
     """Wrapper for JavaScript's setTimeout() which automatically manages the lifetime
     of a JsProxy corresponding to the callback param.
     """
     id = -1
 
     def wrapper():
         callback()
-        TIMEOUTS.pop(id, None)
+        _timeouts.pop(id, None)
 
     callable = create_once_callable(wrapper)
     id = setTimeout(callable, timeout)
-    TIMEOUTS[id] = callable
+    _timeouts[id] = callable
     return id
 
 
 def clear_timeout(id):
     """Wrapper for JavaScript's clearTimeout() which automatically manages the lifetime
     of a JsProxy corresponding to the callback param.
     """
     clearTimeout(id)
-    TIMEOUTS.pop(id, None)
+    _timeouts.pop(id, None)
 
 
-INTERVAL_CALLBACKS: dict[int, Callable] = {}
+_interval_callbacks: dict[int, Callable] = {}
 
 
 def set_interval(callback, interval):
     """Wrapper for JavaScript's setInterval() which automatically manages the lifetime
     of a JsProxy corresponding to the callback param.
     """
     proxy = create_proxy(callback)
     id = setInterval(proxy, interval)
-    INTERVAL_CALLBACKS[id] = proxy
+    _interval_callbacks[id] = proxy
     return id
 
 
 def clear_interval(id):
     """Wrapper for JavaScript's clearInterval() which automatically manages the lifetime
     of a JsProxy corresponding to the callback param.
     """
     clearInterval(id)
-    INTERVAL_CALLBACKS.pop(id, None)
+    _interval_callbacks.pop(id, None)
```

### Comparing `beepy_web-0.9.7/beepy/utils/js_py.py` & `beepy_web-0.9.8/beepy/utils/js_py.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.7/scripts/publish.sh` & `beepy_web-0.9.8/scripts/publish.sh`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.7/web/package-lock.json` & `beepy_web-0.9.8/web/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.899982970027248%*

 * *Differences: {"'packages'": "{'': {'version': '0.9.8'}}", "'version'": "'0.9.8'"}*

```diff
@@ -12,15 +12,15 @@
                 "webpack": "^5.89.0",
                 "webpack-cli": "^5.1.4",
                 "webpack-dev-server": "^4.15.1",
                 "webpack-merge": "^5.10.0"
             },
             "license": "MIT",
             "name": "@kor0p/beepy",
-            "version": "0.9.7"
+            "version": "0.9.8"
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
-    "version": "0.9.7"
+    "version": "0.9.8"
 }
```

### Comparing `beepy_web-0.9.7/web/package.json` & `beepy_web-0.9.8/web/package.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.9.8'"}*

```diff
@@ -31,9 +31,9 @@
     "name": "@kor0p/beepy",
     "scripts": {
         "build": "webpack --config webpack.prod.js",
         "start": "webpack serve --config webpack.dev.js",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch"
     },
-    "version": "0.9.7"
+    "version": "0.9.8"
 }
```

### Comparing `beepy_web-0.9.7/web/webpack.prod.js` & `beepy_web-0.9.8/web/webpack.prod.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.7/web/src/beepy.js` & `beepy_web-0.9.8/web/src/beepy.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -21,23 +21,23 @@
 const _script = document.currentScript
 let localConfig = {}
 if (!!window.beepy) {
     localConfig = window.beepy
 }
 
 class BeePy {
-    __version__ = '0.9.7'
+    __version__ = '0.9.8'
 
     pyodideIndexURL = null
     globals = null
     dev_server = dev_server
     dev_path = ''
     python_api = python
 
-    static DEFAULT_CONFIG = {
+    static _default_config = {
         include: ['.env'],
         pyodideVersion: '0.25.1',
         requirements: [], // also could be function
     }
 
     // aliases for PythonAPI
     addElement = addHTMLElement
@@ -47,15 +47,15 @@
         if (!localConfig) {
             console.log(`
 No beepy config found! Default config will be used
 If you have config, you must define it before loading beepy script
             `)
         }
 
-        this.config = mergeDeep(BeePy.DEFAULT_CONFIG, localConfig.config || {})
+        this.config = mergeDeep(BeePy._default_config, localConfig.config || {})
         this._loadPyodideScript()
 
         const path = _script.src.substring(0, _script.src.indexOf('beepy.js') - 1).replace(/\/+$/, '')
         this.dev_path = path.split('/').slice(0, -2).join('/')
     }
 
     startLoading({
```

### Comparing `beepy_web-0.9.7/web/src/dev-server.js` & `beepy_web-0.9.8/web/src/dev-server.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.7/web/src/files.js` & `beepy_web-0.9.8/web/src/files.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.7/web/src/main.css` & `beepy_web-0.9.8/web/src/main.css`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.7/web/src/python.js` & `beepy_web-0.9.8/web/src/python.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.7/web/src/utils.js` & `beepy_web-0.9.8/web/src/utils.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -72,24 +72,24 @@
 }
 
 
 export function _lstrip(text) {
     return text.replace(/^\/+/, '')
 }
 
-export const _PY_TAG_ATTRIBUTE = '__PYTHON_TAG__'
+export const _py_tag_attribute = '__PYTHON_TAG__'
 
 function getPyTag(i) {
     /**
      * usage:
      * > py0
      * evaluates $0.__PYTHON_TAG__
      * available for py0-py9
      */
-    return () => window[`$${i}`][_PY_TAG_ATTRIBUTE]
+    return () => window[`$${i}`][_py_tag_attribute]
 }
 
 Object.defineProperties(
     window,
     Object.fromEntries(new Array(10).fill(null).map(
         (_, i) => [`py${i}`, {
             get: getPyTag(i)
```

### Comparing `beepy_web-0.9.7/.gitignore` & `beepy_web-0.9.8/.gitignore`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.7/LICENSE` & `beepy_web-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.7/README.md` & `beepy_web-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.7/pyproject.toml` & `beepy_web-0.9.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -112,10 +112,13 @@
 
 [tool.ruff.lint.pycodestyle]
 ignore-overlong-task-comments = true
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
+[tool.ruff.pylint]
+max-args = 7
+
 [tool.ruff.lint.mccabe]
 # Flag errors (`C901`) whenever the complexity level exceeds 11.
 max-complexity = 11
```

### Comparing `beepy_web-0.9.7/PKG-INFO` & `beepy_web-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beepy-web
-Version: 0.9.7
+Version: 0.9.8
 Summary: The modern frontend web framework for Python
 Project-URL: Homepage, https://beepy-web-ba63e5a12994.herokuapp.com/e/
 Project-URL: Repository, https://github.com/kor0p/BeePy
 Project-URL: Docs, https://bee-py.readthedocs.io/en/latest/
 Project-URL: Community, https://t.me/bee_py/
 Project-URL: Sandbox, https://kor0p.github.io/BeePy-examples/sandbox
 Project-URL: NPM, https://www.npmjs.com/package/@kor0p/beepy
```

