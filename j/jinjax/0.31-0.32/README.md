# Comparing `tmp/jinjax-0.31.tar.gz` & `tmp/jinjax-0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinjax-0.31.tar", max compression
+gzip compressed data, was "jinjax-0.32.tar", max compression
```

## Comparing `jinjax-0.31.tar` & `jinjax-0.32.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      373 2024-02-25 00:03:38.985843 jinjax-0.31/README.md
--rw-r--r--   0        0        0     2687 2024-02-25 00:03:38.989843 jinjax-0.31/pyproject.toml
--rw-r--r--   0        0        0      189 2024-02-25 00:03:38.989843 jinjax-0.31/src/jinjax/__init__.py
--rw-r--r--   0        0        0    13193 2024-02-25 00:03:38.989843 jinjax-0.31/src/jinjax/catalog.py
--rw-r--r--   0        0        0     6124 2024-02-25 00:03:38.989843 jinjax-0.31/src/jinjax/component.py
--rw-r--r--   0        0        0      409 2024-02-25 00:03:38.989843 jinjax-0.31/src/jinjax/exceptions.py
--rw-r--r--   0        0        0     5248 2024-02-25 00:03:38.989843 jinjax-0.31/src/jinjax/html_attrs.py
--rw-r--r--   0        0        0     4599 2024-02-25 00:03:38.989843 jinjax-0.31/src/jinjax/jinjax.py
--rw-r--r--   0        0        0     1355 2024-02-25 00:03:38.989843 jinjax-0.31/src/jinjax/middleware.py
--rw-r--r--   0        0        0        0 2024-02-25 00:03:38.989843 jinjax-0.31/src/jinjax/py.typed
--rw-r--r--   0        0        0       54 2024-02-25 00:03:38.989843 jinjax-0.31/src/jinjax/utils.py
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 jinjax-0.31/PKG-INFO
+-rw-r--r--   0        0        0      497 2024-04-19 23:46:40.753900 jinjax-0.32/README.md
+-rw-r--r--   0        0        0     3833 2024-04-19 23:46:40.761900 jinjax-0.32/pyproject.toml
+-rw-r--r--   0        0        0      189 2024-04-19 23:46:40.761900 jinjax-0.32/src/jinjax/__init__.py
+-rw-r--r--   0        0        0    13704 2024-04-19 23:46:40.761900 jinjax-0.32/src/jinjax/catalog.py
+-rw-r--r--   0        0        0     6409 2024-04-19 23:46:40.761900 jinjax-0.32/src/jinjax/component.py
+-rw-r--r--   0        0        0      409 2024-04-19 23:46:40.761900 jinjax-0.32/src/jinjax/exceptions.py
+-rw-r--r--   0        0        0     5246 2024-04-19 23:46:40.761900 jinjax-0.32/src/jinjax/html_attrs.py
+-rw-r--r--   0        0        0     4594 2024-04-19 23:46:40.761900 jinjax-0.32/src/jinjax/jinjax.py
+-rw-r--r--   0        0        0     1298 2024-04-19 23:46:40.761900 jinjax-0.32/src/jinjax/middleware.py
+-rw-r--r--   0        0        0        0 2024-04-19 23:46:40.761900 jinjax-0.32/src/jinjax/py.typed
+-rw-r--r--   0        0        0       54 2024-04-19 23:46:40.761900 jinjax-0.32/src/jinjax/utils.py
+-rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 jinjax-0.32/PKG-INFO
```

### Comparing `jinjax-0.31/src/jinjax/catalog.py` & `jinjax-0.32/src/jinjax/catalog.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,21 @@
 from pathlib import Path
 
 import jinja2
 from markupsafe import Markup
 
 from .component import Component
 from .exceptions import ComponentNotFound, InvalidArgument
+from .html_attrs import HTMLAttrs
 from .jinjax import JinjaX
 from .middleware import ComponentsMiddleware
-from .html_attrs import HTMLAttrs
 from .utils import logger
 
 
-if t.TYPE_CHECKING:
-    TFileExt = tuple[str, ...] | str
-
+TFileExt = tuple[str, ...] | str
 
 DEFAULT_URL_ROOT = "/static/components/"
 ALLOWED_EXTENSIONS = (".css", ".js", ".mjs")
 DEFAULT_PREFIX = ""
 DEFAULT_EXTENSION = ".jinja"
 DELIMITER = "."
 SLASH = "/"
@@ -28,70 +26,71 @@
 PROP_CONTENT = "content"
 
 
 class Catalog:
     """
     Attributes:
 
-    - globals:
+        globals:
 
-    - filters:
+        filters:
 
-    - tests:
+        tests:
 
-    - extensions:
+        extensions:
 
-    - jinja_env:
+        jinja_env:
 
-    - root_url:
+        root_url:
 
-    - file_ext:
+        file_ext:
 
-    - fingerprint [False]:
-        If True, adds, insert a hash of the updated time to the URL of the
-        asset files (after the name of,but before the extension).
-        This strategy encourages long-term caching while ensuring that new copies
-        are only requested when the content changes, as any modification alter
-        the fingerprint and thus the filename.
+        fingerprint [False]:
+            If True, adds, insert a hash of the updated time to the URL of the
+            asset files (after the name of,but before the extension).
+            This strategy encourages long-term caching while ensuring that new copies
+            are only requested when the content changes, as any modification alter
+            the fingerprint and thus the filename.
 
-        *WARNING*: Only works if the server know how to filter the fingerprint
-        to get the real name of the file.
+            *WARNING*: Only works if the server know how to filter the fingerprint
+            to get the real name of the file.
 
     """
 
     __slots__ = (
         "prefixes",
         "root_url",
         "file_ext",
         "jinja_env",
         "fingerprint",
         "collected_css",
         "collected_js",
         "auto_reload",
+        "tmpl_globals",
         "use_cache",
         "_cache",
     )
 
     def __init__(
         self,
         *,
-        globals: "dict[str, t.Any] | None" = None,
-        filters: "dict[str, t.Any] | None" = None,
-        tests: "dict[str, t.Any] | None" = None,
-        extensions: "list | None" = None,
-        jinja_env: "jinja2.Environment | None" = None,
+        globals: dict[str, t.Any] | None = None,
+        filters: dict[str, t.Any] | None = None,
+        tests: dict[str, t.Any] | None = None,
+        extensions: list | None = None,
+        jinja_env: jinja2.Environment | None = None,
         root_url: str = DEFAULT_URL_ROOT,
-        file_ext: "TFileExt" = DEFAULT_EXTENSION,
+        file_ext: TFileExt = DEFAULT_EXTENSION,
         use_cache: bool = True,
         auto_reload: bool = True,
         fingerprint: bool = False,
     ) -> None:
-        self.prefixes: "dict[str, jinja2.FileSystemLoader]" = {}
-        self.collected_css: "list[str]" = []
-        self.collected_js: "list[str]" = []
+        self.prefixes: dict[str, jinja2.FileSystemLoader] = {}
+        self.collected_css: list[str] = []
+        self.collected_js: list[str] = []
         self.file_ext = file_ext
         self.use_cache = use_cache
         self.auto_reload = auto_reload
         self.fingerprint = fingerprint
 
         root_url = root_url.strip().rstrip(SLASH)
         self.root_url = f"{root_url}{SLASH}"
@@ -119,26 +118,27 @@
         env.globals.update(globals)
         env.filters.update(filters)
         env.tests.update(tests)
         env.extend(catalog=self)
 
         self.jinja_env = env
 
-        self._cache: "dict[str, dict]" = {}
+        self.tmpl_globals: t.MutableMapping[str, t.Any] | None = None
+        self._cache: dict[str, dict] = {}
 
     @property
-    def paths(self) -> "list[Path]":
+    def paths(self) -> list[Path]:
         _paths = []
         for loader in self.prefixes.values():
             _paths.extend(loader.searchpath)
         return _paths
 
     def add_folder(
         self,
-        root_path: "str | Path",
+        root_path: str | Path,
         *,
         prefix: str = DEFAULT_PREFIX,
     ) -> None:
         prefix = prefix.strip().strip(f"{DELIMITER}{SLASH}").replace(SLASH, DELIMITER)
 
         root_path = str(root_path)
         if prefix in self.prefixes:
@@ -160,26 +160,27 @@
         for mprefix, path in module.components.items():
             self.add_folder(path, prefix=prefix or mprefix)
 
     def render(
         self,
         __name: str,
         *,
-        caller: "t.Callable | None" = None,
+        caller: t.Callable | None = None,
         **kw,
     ) -> str:
         self.collected_css = []
         self.collected_js = []
+        self.tmpl_globals = kw.pop("__globals", None)
         return self.irender(__name, caller=caller, **kw)
 
     def irender(
         self,
         __name: str,
         *,
-        caller: "t.Callable | None" = None,
+        caller: t.Callable | None = None,
         **kw,
     ) -> str:
         content = (kw.pop("__content", "") or "").strip()
         attrs = kw.pop("__attrs", None) or {}
         file_ext = kw.pop("__file_ext", "")
         source = kw.pop("__source", "")
 
@@ -191,20 +192,26 @@
             logger.debug("Rendering from source %s", __name)
             component = self._get_from_source(
                 name=name, url_prefix=url_prefix, source=source
             )
         elif self.use_cache:
             logger.debug("Rendering from cache or file %s", __name)
             component = self._get_from_cache(
-                prefix=prefix, name=name, url_prefix=url_prefix, file_ext=file_ext
+                prefix=prefix,
+                name=name,
+                url_prefix=url_prefix,
+                file_ext=file_ext,
             )
         else:
             logger.debug("Rendering from file %s", __name)
             component = self._get_from_file(
-                prefix=prefix, name=name, url_prefix=url_prefix, file_ext=file_ext
+                prefix=prefix,
+                name=name,
+                url_prefix=url_prefix,
+                file_ext=file_ext,
             )
 
         root_path = component.path.parent if component.path else None
 
         for url in component.css:
             if (
                 root_path
@@ -241,33 +248,31 @@
             ) from exc
 
         props[PROP_CONTENT] = content if content or not caller else caller().strip()
         return component.render(**props)
 
     def get_middleware(
         self,
-        application: "t.Callable",
-        allowed_ext: "t.Iterable[str] | None" = ALLOWED_EXTENSIONS,
+        application: t.Callable,
+        allowed_ext: t.Iterable[str] | None = ALLOWED_EXTENSIONS,
         **kwargs,
-    ) -> "ComponentsMiddleware":
+    ) -> ComponentsMiddleware:
         logger.debug("Creating middleware")
         middleware = ComponentsMiddleware(
-            application=application,
-            allowed_ext=tuple(allowed_ext or []),
-            **kwargs
+            application=application, allowed_ext=tuple(allowed_ext or []), **kwargs
         )
         for prefix, loader in self.prefixes.items():
             url_prefix = self._get_url_prefix(prefix)
             url = f"{self.root_url}{url_prefix}"
             for root in loader.searchpath[::-1]:
                 middleware.add_files(root, url)
 
         return middleware
 
-    def get_source(self, cname: str, file_ext: "TFileExt" = "") -> str:
+    def get_source(self, cname: str, file_ext: TFileExt = "") -> str:
         prefix, name = self._split_name(cname)
         path, _ = self._get_component_path(prefix, name, file_ext=file_ext)
         return path.read_text()
 
     def render_assets(self, fingerprint: bool = False) -> str:
         html_css = []
         for url in self.collected_css:
@@ -297,58 +302,84 @@
         ext = "".join(relpath.suffixes)
         stem = relpath.name.removesuffix(ext)
         parent = str(relpath.parent)
         parent = "" if parent == "." else f"{parent}/"
 
         return f"{parent}{stem}-{fingerprint}{ext}"
 
-    def _get_from_source(self, *, name: str, url_prefix: str, source: str) -> "Component":
-        tmpl = self.jinja_env.from_string(source)
-        component = Component(name=name, url_prefix=url_prefix, source=source, tmpl=tmpl)
+    def _get_from_source(
+        self,
+        *,
+        name: str,
+        url_prefix: str,
+        source: str,
+    ) -> Component:
+        tmpl = self.jinja_env.from_string(source, globals=self.tmpl_globals)
+        component = Component(
+            name=name, url_prefix=url_prefix, source=source, tmpl=tmpl
+        )
         return component
 
-    def _get_from_cache(self, *, prefix: str, name: str, url_prefix: str, file_ext: str) -> "Component":
+    def _get_from_cache(
+        self,
+        *,
+        prefix: str,
+        name: str,
+        url_prefix: str,
+        file_ext: str,
+    ) -> Component:
         key = f"{prefix}.{name}.{file_ext}"
         cache = self._from_cache(key)
         if cache:
-            component = Component.from_cache(cache, auto_reload=self.auto_reload)
+            component = Component.from_cache(
+                cache, auto_reload=self.auto_reload, globals=self.tmpl_globals
+            )
             if component:
                 return component
 
         logger.debug("Loading %s", key)
         component = self._get_from_file(
             prefix=prefix,
             name=name,
             url_prefix=url_prefix,
             file_ext=file_ext,
         )
         self._to_cache(key, component)
         return component
 
-    def _from_cache(self, key: str) -> "dict[str, t.Any]":
+    def _from_cache(self, key: str) -> dict[str, t.Any]:
         if key not in self._cache:
             return {}
         cache = self._cache[key]
         logger.debug("Loading from cache %s", key)
         return cache
 
     def _to_cache(self, key: str, component: Component) -> None:
         self._cache[key] = component.serialize()
 
-    def _get_from_file(self, *, prefix: str, name: str, url_prefix: str, file_ext: str) -> "Component":
+    def _get_from_file(
+        self,
+        *,
+        prefix: str,
+        name: str,
+        url_prefix: str,
+        file_ext: str,
+    ) -> Component:
         path, tmpl_name = self._get_component_path(prefix, name, file_ext=file_ext)
         component = Component(
             name=name,
             url_prefix=url_prefix,
             path=path,
         )
-        component.tmpl = self.jinja_env.get_template(tmpl_name)
+        component.tmpl = self.jinja_env.get_template(
+            tmpl_name, globals=self.tmpl_globals
+        )
         return component
 
-    def _split_name(self, cname: str) -> "tuple[str, str]":
+    def _split_name(self, cname: str) -> tuple[str, str]:
         cname = cname.strip().strip(DELIMITER)
         if DELIMITER not in cname:
             return DEFAULT_PREFIX, cname
         for prefix in self.prefixes.keys():
             _prefix = f"{prefix}{DELIMITER}"
             if cname.startswith(_prefix):
                 return prefix, cname.removeprefix(_prefix)
@@ -359,16 +390,16 @@
             prefix.strip().strip(f"{DELIMITER}{SLASH}").replace(DELIMITER, SLASH)
         )
         if url_prefix:
             url_prefix = f"{url_prefix}{SLASH}"
         return url_prefix
 
     def _get_component_path(
-        self, prefix: str, name: str, file_ext: "TFileExt" = ""
-    ) -> "tuple[Path, str]":
+        self, prefix: str, name: str, file_ext: TFileExt = ""
+    ) -> tuple[Path, str]:
         name = name.replace(DELIMITER, SLASH)
         root_paths = self.prefixes[prefix].searchpath
         name_dot = f"{name}."
         file_ext = file_ext or self.file_ext
 
         for root_path in root_paths:
             for curr_folder, _, files in os.walk(
@@ -387,15 +418,15 @@
                         return Path(curr_folder) / filename, filepath
 
         raise ComponentNotFound(
             f"Unable to find a file named {name}{file_ext} "
             f"or one following the pattern {name_dot}*{file_ext}"
         )
 
-    def _render_attrs(self, attrs: "dict") -> "Markup":
+    def _render_attrs(self, attrs: dict[str, t.Any]) -> Markup:
         html_attrs = []
         for name, value in attrs.items():
             if value != "":
                 html_attrs.append(f"{name}={value}")
             else:
                 html_attrs.append(name)
         return Markup(" ".join(html_attrs))
```

### Comparing `jinjax-0.31/src/jinjax/component.py` & `jinjax-0.32/src/jinjax/component.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import ast
 import re
 import typing as t
 from keyword import iskeyword
-from markupsafe import Markup
 from pathlib import Path
 
+from jinja2 import Template
+from markupsafe import Markup
+
 from .exceptions import InvalidArgument, MissingRequiredArgument
 
+
 if t.TYPE_CHECKING:
-    from jinja2 import Template
+    from typing_extensions import Self
 
 
 RX_PROPS_START = re.compile(r"{#-?\s*def\s+")
 RX_CSS_START = re.compile(r"{#-?\s*css\s+")
 RX_JS_START = re.compile(r"{#-?\s*js\s+")
 RX_META_END = re.compile(r"\s*-?#}")
 RX_COMMA = re.compile(r"\s*,\s*")
@@ -33,15 +36,15 @@
     code = compile(input_string, "<string>", "eval")
     for name in code.co_names:
         if name not in ALLOWED_NAMES_IN_EXPRESSION_VALUES:
             raise InvalidArgument(f"Use of {name} not allowed")
     try:
         return eval(code, {"__builtins__": {}}, ALLOWED_NAMES_IN_EXPRESSION_VALUES)
     except NameError as err:
-        raise InvalidArgument(err)
+        raise InvalidArgument(err) from err
 
 
 def is_valid_variable_name(name):
     return name.isidentifier() and not iskeyword(name)
 
 
 class Component:
@@ -60,36 +63,41 @@
     def __init__(
         self,
         *,
         name: str,
         url_prefix: str = "",
         source: str = "",
         mtime: float = 0,
-        tmpl: "Template | None" = None,
-        path: "Path | None" = None,
+        tmpl: Template | None = None,
+        path: Path | None = None,
     ) -> None:
         self.name = name
         self.url_prefix = url_prefix
-        self.required: "list[str]" = []
-        self.optional: "dict[str, t.Any]" = {}
-        self.css: "list[str]" = []
-        self.js: "list[str]" = []
+        self.required: list[str] = []
+        self.optional: dict[str, t.Any] = {}
+        self.css: list[str] = []
+        self.js: list[str] = []
 
         if path is not None:
             source = source or path.read_text()
             mtime = mtime or path.stat().st_mtime
         if source:
             self.load_metadata(source)
 
         self.path = path
         self.mtime = mtime
         self.tmpl = tmpl
 
     @classmethod
-    def from_cache(cls, cache: "dict[str, t.Any]", auto_reload: bool = True) -> "Component | None":
+    def from_cache(
+        cls,
+        cache: dict[str, t.Any],
+        auto_reload: bool = True,
+        globals: t.MutableMapping[str, t.Any] | None = None,
+    ) -> "Self | None":
         path = cache["path"]
         mtime = cache["mtime"]
 
         if auto_reload:
             if not path.is_file() or path.stat().st_mtime != mtime:
                 return None
 
@@ -97,17 +105,22 @@
         self.required = cache["required"]
         self.optional = cache["optional"]
         self.css = cache["css"]
         self.js = cache["js"]
         self.path = path
         self.mtime = cache["mtime"]
         self.tmpl = cache["tmpl"]
+
+        if globals:
+            # updating the template globals, does not affect the environment globals
+            self.tmpl.globals.update(globals)
+
         return self
 
-    def serialize(self) -> "dict[str, t.Any]":
+    def serialize(self) -> dict[str, t.Any]:
         return {
             "name": self.name,
             "required": self.required,
             "optional": self.optional,
             "css": self.css,
             "js": self.js,
             "path": self.path,
@@ -148,49 +161,50 @@
         if not start:
             return ""
         end = RX_META_END.search(source, pos=start.end())
         if not end:
             raise InvalidArgument(self.name)
         return source[start.end() : end.start()].strip()
 
-    def parse_args_expr(self, expr: str) -> "tuple[list[str], dict[str, t.Any]]":
+    def parse_args_expr(self, expr: str) -> tuple[list[str], dict[str, t.Any]]:
         expr = expr.strip(" *,/")
         required = []
         optional = {}
 
         try:
             p = ast.parse(f"def component(*, {expr}): pass")
         except SyntaxError as err:
-            raise InvalidArgument(err)
+            raise InvalidArgument(err) from err
+
         args = p.body[0].args  # type: ignore
         arg_names = [arg.arg for arg in args.kwonlyargs]
-        for name, value in zip(arg_names, args.kw_defaults):
+        for name, value in zip(arg_names, args.kw_defaults, strict=True):
             if value is None:
                 required.append(name)
                 continue
             expr = ast.unparse(value)
             optional[name] = eval_expression(expr)
 
         return required, optional
 
-    def parse_files_expr(self, expr: str) -> "list[str]":
+    def parse_files_expr(self, expr: str) -> list[str]:
         files = []
         for url in RX_COMMA.split(expr):
             url = url.strip("\"'").rstrip("/")
             if not url:
                 continue
             if url.startswith(("/", "http://", "https://")):
                 files.append(url)
             else:
                 files.append(f"{self.url_prefix}{url}")
         return files
 
     def filter_args(
-        self, kw: "dict[str, t.Any]"
-    ) -> "tuple[dict[str, t.Any], dict[str, t.Any]]":
+        self, kw: dict[str, t.Any]
+    ) -> tuple[dict[str, t.Any], dict[str, t.Any]]:
         props = {}
 
         for key in self.required:
             if key not in kw:
                 raise MissingRequiredArgument(self.name, key)
             props[key] = kw.pop(key)
```

### Comparing `jinjax-0.31/src/jinjax/html_attrs.py` & `jinjax-0.32/src/jinjax/html_attrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 CLASS_KEY = "class"
 CLASS_ALT_KEY = "classes"
 CLASS_KEYS = (CLASS_KEY, CLASS_ALT_KEY)
 
 
-def split(ssl: str) -> "list[str]":
+def split(ssl: str) -> list[str]:
     return re.split(r"\s+", ssl.strip())
 
 
 def quote(text: str) -> str:
     if '"' in text:
         if "'" in text:
             text = text.replace('"', "&quot;")
@@ -30,22 +30,22 @@
 
     __slots__ = ("_seq",)
 
     def __init__(self, seq):
         self._seq = seq
 
     @cached_property
-    def data(self):
+    def data(self):  # type: ignore
         return str(self._seq)
 
 
 class HTMLAttrs:
     def __init__(self, attrs) -> None:
-        attributes: "dict[str, str|LazyString]" = {}
-        properties: "set[str]" = set()
+        attributes: dict[str, str|LazyString] = {}
+        properties: set[str] = set()
 
         class_names = split(" ".join([
             attrs.pop(CLASS_KEY, ""),
             attrs.get(CLASS_ALT_KEY, ""),
         ]))
         self.__classes = {name for name in class_names if name}
 
@@ -57,25 +57,25 @@
                 attributes[name] = LazyString(value)
 
         self.__attributes = attributes
         self.__properties = properties
 
     @property
     def classes(self) -> str:
-        return " ".join(sorted(list(self.__classes)))
+        return " ".join(sorted((self.__classes)))
 
     @property
     def as_dict(self) -> dict[str, Any]:
         attributes = self.__attributes.copy()
         classes = self.classes
         if classes:
             attributes[CLASS_KEY] = classes
 
         out: dict[str, Any] = dict(sorted(attributes.items()))
-        for name in sorted(list(self.__properties)):
+        for name in sorted((self.__properties)):
             out[name] = True
         return out
 
     def __getitem__(self, name: str) -> Any:
         return self.get(name)
 
     def __delitem__(self, name: str) -> None:
@@ -166,15 +166,15 @@
         attributes = self.__attributes.copy()
 
         classes = self.classes
         if classes:
             attributes[CLASS_KEY] = classes
 
         attributes = dict(sorted(attributes.items()))
-        properties = sorted(list(self.__properties))
+        properties = sorted((self.__properties))
 
         html_attrs = [
             f"{name}={quote(str(value))}"
             for name, value in attributes.items()
         ]
         html_attrs.extend(properties)
```

### Comparing `jinjax-0.31/src/jinjax/jinjax.py` & `jinjax-0.32/src/jinjax/jinjax.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import typing as t
 from uuid import uuid4
 
-from jinja2.ext import Extension
 from jinja2.exceptions import TemplateSyntaxError
+from jinja2.ext import Extension
 
 from .utils import logger
 
 
 RENDER_CMD = "catalog.irender"
 BLOCK_CALL = '{% call [CMD]("[TAG]"[ATTRS]) -%}[CONTENT]{%- endcall %}'
 BLOCK_CALL = BLOCK_CALL.replace("[CMD]", RENDER_CMD)
@@ -84,15 +84,14 @@
 
     def _process_tag(self, source: str, match: re.Match) -> str:
         start, end = match.span(0)
         tag = match.group("tag")
         attrs = (match.group("attrs") or "").strip()
         inline = match.group(0).endswith("/>")
         logger.debug(f"{tag} {attrs} {'inline' if not inline else ''}")
-
         if inline:
             content = ""
         else:
             end_tag = f"</{tag}>"
             index = source.find(end_tag, end, None)
             if index == -1:
                 raise TemplateSyntaxError(
@@ -122,19 +121,19 @@
     ) -> str:
         logger.debug(f"{tag} {attrs_list} {'inline' if not content else ''}")
         attrs = []
         for name, value in attrs_list:
             name = name.strip().replace("-", "_")
             value = value.strip()
             if not value:
-                attrs.append(f"\"{name}\"=True")
+                attrs.append(f'"{name}"=True')
             else:
                 if value.startswith(ATTR_START) and value.endswith(ATTR_END):
                     value = value[1:-1].strip()
-                attrs.append(f"\"{name}\"={value}")
+                attrs.append(f'"{name}"={value}')
 
         str_attrs = "**{" + ", ".join([a.replace("=", ":", 1) for a in attrs]) + "}"
         if str_attrs:
             str_attrs = f", {str_attrs}"
 
         if not content:
             call = INLINE_CALL.replace("[TAG]", tag).replace("[ATTRS]", str_attrs)
```

### Comparing `jinjax-0.31/src/jinjax/middleware.py` & `jinjax-0.32/src/jinjax/middleware.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import re
 import typing as t
 from pathlib import Path
 
-from whitenoise import WhiteNoise  # type: ignore
-
-if t.TYPE_CHECKING:
-    from whitenoise.responders import Redirect, StaticFile  # type: ignore
+from whitenoise import WhiteNoise
+from whitenoise.responders import Redirect, StaticFile
 
 
 RX_FINGERPRINT = re.compile("(.*)-([abcdef0-9]{64})")
 
 
 class ComponentsMiddleware(WhiteNoise):
     """WSGI middleware for serving components assets"""
     allowed_ext: tuple[str, ...]
 
     def __init__(self, **kwargs) -> None:
-        self.allowed_ext = kwargs.pop("allowed_ext", tuple())
+        self.allowed_ext = kwargs.pop("allowed_ext", ())
         super().__init__(**kwargs)
 
-    def find_file(self, url: str) -> "StaticFile|Redirect|None":
+    def find_file(self, url: str) -> StaticFile|Redirect|None:
 
         if self.allowed_ext and not url.endswith(self.allowed_ext):
             return None
 
         # Ignore the fingerprint in the filename
         # since is only for managing the cache in the client
         relpath = Path(url)
@@ -32,10 +30,10 @@
         fingerprinted = RX_FINGERPRINT.match(stem)
         if fingerprinted:
             stem = fingerprinted.group(1)
             relpath = relpath.with_name(f"{stem}{ext}")
 
         return super().find_file(str(relpath))
 
-    def add_file_to_dictionary(self, url: str, path: str, stat_cache: t.Any) -> None:
+    def add_file_to_dictionary(self, url: str, path: str, stat_cache: t.Any = None) -> None:
         if not self.allowed_ext or url.endswith(self.allowed_ext):
             super().add_file_to_dictionary(url, path, stat_cache)
```

### Comparing `jinjax-0.31/PKG-INFO` & `jinjax-0.32/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjax
-Version: 0.31
+Version: 0.32
 Summary: Replace your HTML templates with Python server-Side components
 Home-page: https://jinjax.scaletti.dev/
 License: MIT
 Author: Juan-Pablo Scaletti
 Author-email: juanpablo@jpscaletti.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -38,7 +38,14 @@
 From chaos to clarity: The power of components in your server-side-rendered Python web app.
 
 **Documentation:** https://jinjax.scaletti.dev/
 
 Write server-side components as single Jinja template files.
 Use them as HTML tags without doing any importing.
 
+
+## Roadmap
+
+- Slots
+- Autoloading assets (optional?) (`Card.jinja` autoloads `Card.css` and/or `Card.js` if exists)
+- ...
+
```

