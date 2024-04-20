# Comparing `tmp/django_includecontents-0.5.1.tar.gz` & `tmp/django_includecontents-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_includecontents-0.5.1.tar", last modified: Fri Apr 19 05:32:25 2024, max compression
+gzip compressed data, was "django_includecontents-0.6.tar", last modified: Fri Apr 19 22:07:11 2024, max compression
```

## Comparing `django_includecontents-0.5.1.tar` & `django_includecontents-0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     5293 2024-04-19 04:27:39.460145 django_includecontents-0.5.1/README.md
--rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-0.5.1/includecontents/__init__.py
--rw-r--r--   0        0        0     1000 2024-04-19 05:13:37.190112 django_includecontents-0.5.1/includecontents/backend.py
--rw-r--r--   0        0        0     4596 2024-04-19 05:31:33.346108 django_includecontents-0.5.1/includecontents/base.py
--rw-r--r--   0        0        0     1401 2024-04-09 04:42:05.196722 django_includecontents-0.5.1/includecontents/engine.py
--rw-r--r--   0        0        0     1663 2024-04-18 05:37:15.283141 django_includecontents-0.5.1/includecontents/loaders.py
--rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-0.5.1/includecontents/templatetags/__init__.py
--rw-r--r--   0        0        0    15216 2024-04-18 05:47:45.081186 django_includecontents-0.5.1/includecontents/templatetags/includecontents.py
--rw-r--r--   0        0        0     1220 2024-04-19 05:32:25.826233 django_includecontents-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      144 2024-04-19 05:31:17.752738 django_includecontents-0.5.1/tests/settings.py
--rw-r--r--   0        0        0      168 2024-04-18 05:37:15.283141 django_includecontents-0.5.1/tests/templates/components/card.html
--rw-r--r--   0        0        0      160 2024-04-18 05:37:15.283141 django_includecontents-0.5.1/tests/templates/components/card_extend.html
--rw-r--r--   0        0        0       81 2024-04-09 04:52:09.297567 django_includecontents-0.5.1/tests/templates/multiline.html
--rw-r--r--   0        0        0      115 2024-04-09 21:50:46.125635 django_includecontents-0.5.1/tests/templates/test_component/attrs.html
--rw-r--r--   0        0        0      162 2024-04-18 05:37:15.283141 django_includecontents-0.5.1/tests/templates/test_component/extend_class.html
--rw-r--r--   0        0        0       73 2024-04-09 21:50:46.125635 django_includecontents-0.5.1/tests/templates/test_component/index.html
--rw-r--r--   0        0        0       34 2024-04-09 21:51:49.385743 django_includecontents-0.5.1/tests/templates/test_component/missing_attr.html
--rw-r--r--   0        0        0       24 2024-04-09 21:51:57.449090 django_includecontents-0.5.1/tests/templates/test_component/missing_closing_tag.html
--rw-r--r--   0        0        0      118 2024-04-09 21:50:46.115635 django_includecontents-0.5.1/tests/templates/test_tag/basic.html
--rw-r--r--   0        0        0       57 2024-04-09 04:52:09.297567 django_includecontents-0.5.1/tests/templates/test_tag/inner.html
--rw-r--r--   0        0        0      135 2024-04-09 21:50:46.115635 django_includecontents-0.5.1/tests/templates/test_tag/with_attr.html
--rw-r--r--   0        0        0     1626 2024-04-19 05:30:37.315975 django_includecontents-0.5.1/tests/test_component.py
--rw-r--r--   0        0        0      130 2024-04-09 04:52:09.297567 django_includecontents-0.5.1/tests/test_multiline.py
--rw-r--r--   0        0        0      454 2024-04-09 04:52:09.297567 django_includecontents-0.5.1/tests/test_tag.py
--rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 django_includecontents-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     5368 2024-04-19 13:06:52.939340 django_includecontents-0.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-13 05:42:59.457047 django_includecontents-0.6/includecontents/__init__.py
+-rw-r--r--   0        0        0     1000 2024-04-13 05:42:59.457047 django_includecontents-0.6/includecontents/backend.py
+-rw-r--r--   0        0        0     4596 2024-04-19 10:22:53.849115 django_includecontents-0.6/includecontents/base.py
+-rw-r--r--   0        0        0     1401 2024-04-13 05:42:59.457047 django_includecontents-0.6/includecontents/engine.py
+-rw-r--r--   0        0        0     1663 2024-04-19 10:22:53.849115 django_includecontents-0.6/includecontents/loaders.py
+-rw-r--r--   0        0        0        0 2024-04-13 05:42:59.457047 django_includecontents-0.6/includecontents/templatetags/__init__.py
+-rw-r--r--   0        0        0    15521 2024-04-19 12:55:11.624488 django_includecontents-0.6/includecontents/templatetags/includecontents.py
+-rw-r--r--   0        0        0     1218 2024-04-19 22:07:11.750242 django_includecontents-0.6/pyproject.toml
+-rw-r--r--   0        0        0      144 2024-04-13 05:42:59.457047 django_includecontents-0.6/tests/settings.py
+-rw-r--r--   0        0        0      168 2024-04-19 10:22:53.849115 django_includecontents-0.6/tests/templates/components/card.html
+-rw-r--r--   0        0        0      163 2024-04-19 12:22:24.408372 django_includecontents-0.6/tests/templates/components/card_extend.html
+-rw-r--r--   0        0        0       81 2024-04-13 05:42:59.457047 django_includecontents-0.6/tests/templates/multiline.html
+-rw-r--r--   0        0        0      115 2024-04-13 05:42:59.457047 django_includecontents-0.6/tests/templates/test_component/attrs.html
+-rw-r--r--   0        0        0      162 2024-04-19 10:22:53.849115 django_includecontents-0.6/tests/templates/test_component/extend_class.html
+-rw-r--r--   0        0        0       73 2024-04-13 05:42:59.457047 django_includecontents-0.6/tests/templates/test_component/index.html
+-rw-r--r--   0        0        0       34 2024-04-13 05:42:59.457047 django_includecontents-0.6/tests/templates/test_component/missing_attr.html
+-rw-r--r--   0        0        0       24 2024-04-13 05:42:59.457047 django_includecontents-0.6/tests/templates/test_component/missing_closing_tag.html
+-rw-r--r--   0        0        0      118 2024-04-13 05:42:59.457047 django_includecontents-0.6/tests/templates/test_tag/basic.html
+-rw-r--r--   0        0        0       54 2024-04-19 13:05:19.856298 django_includecontents-0.6/tests/templates/test_tag/inner.html
+-rw-r--r--   0        0        0      135 2024-04-13 05:42:59.457047 django_includecontents-0.6/tests/templates/test_tag/with_attr.html
+-rw-r--r--   0        0        0     1626 2024-04-19 10:22:53.849115 django_includecontents-0.6/tests/test_component.py
+-rw-r--r--   0        0        0      130 2024-04-13 05:42:59.457047 django_includecontents-0.6/tests/test_multiline.py
+-rw-r--r--   0        0        0      454 2024-04-13 05:42:59.457047 django_includecontents-0.6/tests/test_tag.py
+-rw-r--r--   0        0        0     6382 1970-01-01 00:00:00.000000 django_includecontents-0.6/PKG-INFO
```

### Comparing `django_includecontents-0.5.1/README.md` & `django_includecontents-0.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -183,32 +183,32 @@
   {% if label %}{{ '<label>'|safe }}{% endif %}
   {{ label }}
   <input {% attrs.input type="text" value=value %}>
   {% if label %}{{ '</label>'|safe }}{% endif %}
 </div>
 ```
 
-#### Conditional classes
+#### Extended / conditional classes
 
-You can also provide conditional classes for the `class` attribute using the following format:
+Prepend your class list with `"& "` to have it extended rather than replaced:
+
+```jinja
+{% attrs class="lg" %}        {# sets default class attribute to "lg" but can be overridden #}
+{% attrs class="& lg p-3" %}  {# always add 'lg p-3' classes #}
+```
+
+You can provide conditional classes for the `class` attribute using the svelte class directive format:
 
 ```jinja
 {# props large=False #}
 
-{% attrs class="lg" %}     {# sets class attribute to "lg" but can be overridden #}
-{% attrs class:lg %}       {# always adds 'lg' class #}
 {% attrs class:lg=large %} {# adds 'lg' class if large prop is truthy #}
+{% attrs class:lg %}       {# always adds 'lg' class #}
 ```
 
-You can use this same conditional format on the template tag / component itself too:
+You can use this same conditional format on the component attributes directly:
 
 ```html
 <include:card title="Hello" class:lg={is_large}>
   <p>World</p>
 </include:card>
 ```
-
-```jinja
-{% includecontents "hello.html" class:lg=is_large %}
-  <p>World</p>
-{% endincludecontents %}
-```
```

### Comparing `django_includecontents-0.5.1/includecontents/backend.py` & `django_includecontents-0.6/includecontents/backend.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.5.1/includecontents/base.py` & `django_includecontents-0.6/includecontents/base.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.5.1/includecontents/engine.py` & `django_includecontents-0.6/includecontents/engine.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.5.1/includecontents/loaders.py` & `django_includecontents-0.6/includecontents/loaders.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.5.1/includecontents/templatetags/includecontents.py` & `django_includecontents-0.6/includecontents/templatetags/includecontents.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         for i, bit in enumerate(bits[3:], start=3):
             if "=" not in bit:
                 bits[i] = f"{bit}=True"
         # Split out nested attributes (those with a dot in the name).
         new_bits = []
         nested_attrs = {}
         for bit in bits:
-            if match := re.match(r"(^\w+\.[-\w:]+)(?:=(.+))?", bit):
+            if match := re.match(r"(^\w+[.:][-.\w:]+)(?:=(.+))?", bit):
                 attr, value = match.groups()
                 nested_attrs[attr] = parser.compile_filter(value or "True")
             else:
                 new_bits.append(bit)
         bits = new_bits
         token.contents = " ".join(bits)
     else:
@@ -291,15 +291,15 @@
 NO_VALUE = object()
 
 
 class Attrs(MutableMapping):
     def __init__(self):
         self._attrs: dict[str, Any] = {}
         self._nested_attrs: dict[str, Attrs] = {}
-        self._extended: dict[str, list[str]] = {}
+        self._extended: dict[str, dict[str, bool]] = {}
 
     def __getattr__(self, key):
         return self._nested_attrs[key]
 
     def __getitem__(self, key):
         return self._attrs[key]
 
@@ -307,21 +307,21 @@
         if "." in key:
             nested_key, key = key.split(".", 1)
             nested_attrs = self._nested_attrs.setdefault(nested_key, Attrs())
             nested_attrs[key] = value
             return
         if ":" in key:
             key, extend = key.split(":", 1)
-            extended = self._extended.setdefault(key, [])
-            if value:
-                if extend not in extended:
-                    extended.append(extend)
-            else:
-                if extend in extended:
-                    extended.remove(extend)
+            extended = self._extended.setdefault(key, {})
+            extended[extend] = value
+            return
+        if key == "class" and value.startswith("& "):
+            extended = self._extended.setdefault(key, {})
+            for bit in value[2:].split(" "):
+                extended[bit] = True
             return
         self._attrs[key] = value
 
     def __delitem__(self, key):
         del self._attrs[key]
 
     def __iter__(self):
@@ -336,33 +336,39 @@
                 (f'{key}="{escape(value)}"' if value is not True else key)
                 for key, value in self.all_attrs()
                 if value is not None
             )
         )
 
     def all_attrs(self):
+        extended = {}
+        for key, parts in self._extended.items():
+            parts = [key for key, value in parts.items() if value]
+            if parts:
+                extended[key] = parts
         for key, value in self._attrs.items():
-            if key in self._extended:
+            if key in extended:
                 if value is True or not value:
                     value_parts = []
                 else:
                     value_parts = str(value).split(" ")
-                for part in self._extended[key]:
+                for part in extended[key]:
                     if part not in value_parts:
                         value_parts.append(part)
                 value = " ".join(value_parts)
             yield key, value or None
-        for key, parts in self._extended.items():
+        for key, parts in extended.items():
             if key not in self._attrs:
                 yield key, " ".join(parts) or None
 
     def update(self, attrs):
         super().update(attrs)
         if isinstance(attrs, Attrs):
-            self._extended.update(attrs._extended)
+            for key, extended in attrs._extended.items():
+                self._extended.setdefault(key, {}).update(extended)
             for key, nested_attrs in attrs._nested_attrs.items():
                 self._nested_attrs.setdefault(key, Attrs()).update(nested_attrs)
 
 
 @register.tag
 def attrs(parser: Parser, token):
     """
```

### Comparing `django_includecontents-0.5.1/pyproject.toml` & `django_includecontents-0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-includecontents"
-version = "0.5.1"
+version = "0.6"
 description = "Django includecontents component-like tag"
 authors = [
     { name = "Chris Beaven", email = "smileychris@gmail.com" },
 ]
 dependencies = [
     "django",
 ]
```

### Comparing `django_includecontents-0.5.1/tests/test_component.py` & `django_includecontents-0.6/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.5.1/PKG-INFO` & `django_includecontents-0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-includecontents
-Version: 0.5.1
+Version: 0.6
 Summary: Django includecontents component-like tag
 Author-Email: Chris Beaven <smileychris@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -209,32 +209,32 @@
   {% if label %}{{ '<label>'|safe }}{% endif %}
   {{ label }}
   <input {% attrs.input type="text" value=value %}>
   {% if label %}{{ '</label>'|safe }}{% endif %}
 </div>
 ```
 
-#### Conditional classes
+#### Extended / conditional classes
 
-You can also provide conditional classes for the `class` attribute using the following format:
+Prepend your class list with `"& "` to have it extended rather than replaced:
+
+```jinja
+{% attrs class="lg" %}        {# sets default class attribute to "lg" but can be overridden #}
+{% attrs class="& lg p-3" %}  {# always add 'lg p-3' classes #}
+```
+
+You can provide conditional classes for the `class` attribute using the svelte class directive format:
 
 ```jinja
 {# props large=False #}
 
-{% attrs class="lg" %}     {# sets class attribute to "lg" but can be overridden #}
-{% attrs class:lg %}       {# always adds 'lg' class #}
 {% attrs class:lg=large %} {# adds 'lg' class if large prop is truthy #}
+{% attrs class:lg %}       {# always adds 'lg' class #}
 ```
 
-You can use this same conditional format on the template tag / component itself too:
+You can use this same conditional format on the component attributes directly:
 
 ```html
 <include:card title="Hello" class:lg={is_large}>
   <p>World</p>
 </include:card>
 ```
-
-```jinja
-{% includecontents "hello.html" class:lg=is_large %}
-  <p>World</p>
-{% endincludecontents %}
-```
```

