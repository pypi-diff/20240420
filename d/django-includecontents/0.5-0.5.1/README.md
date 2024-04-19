# Comparing `tmp/django_includecontents-0.5.tar.gz` & `tmp/django_includecontents-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_includecontents-0.5.tar", last modified: Fri Apr 19 04:40:01 2024, max compression
+gzip compressed data, was "django_includecontents-0.5.1.tar", last modified: Fri Apr 19 05:32:25 2024, max compression
```

## Comparing `django_includecontents-0.5.tar` & `django_includecontents-0.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     5293 2024-04-19 04:27:39.460145 django_includecontents-0.5/README.md
--rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-0.5/includecontents/__init__.py
--rw-r--r--   0        0        0     1000 2024-04-09 04:42:05.196722 django_includecontents-0.5/includecontents/backend.py
--rw-r--r--   0        0        0     4589 2024-04-18 05:37:15.283141 django_includecontents-0.5/includecontents/base.py
--rw-r--r--   0        0        0     1401 2024-04-09 04:42:05.196722 django_includecontents-0.5/includecontents/engine.py
--rw-r--r--   0        0        0     1663 2024-04-18 05:37:15.283141 django_includecontents-0.5/includecontents/loaders.py
--rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-0.5/includecontents/templatetags/__init__.py
--rw-r--r--   0        0        0    15216 2024-04-18 05:47:45.081186 django_includecontents-0.5/includecontents/templatetags/includecontents.py
--rw-r--r--   0        0        0     1218 2024-04-19 04:40:01.995012 django_includecontents-0.5/pyproject.toml
--rw-r--r--   0        0        0      144 2024-04-09 04:42:05.196722 django_includecontents-0.5/tests/settings.py
--rw-r--r--   0        0        0      168 2024-04-18 05:37:15.283141 django_includecontents-0.5/tests/templates/components/card.html
--rw-r--r--   0        0        0      160 2024-04-18 05:37:15.283141 django_includecontents-0.5/tests/templates/components/card_extend.html
--rw-r--r--   0        0        0       81 2024-04-09 04:52:09.297567 django_includecontents-0.5/tests/templates/multiline.html
--rw-r--r--   0        0        0      115 2024-04-09 21:50:46.125635 django_includecontents-0.5/tests/templates/test_component/attrs.html
--rw-r--r--   0        0        0      162 2024-04-18 05:37:15.283141 django_includecontents-0.5/tests/templates/test_component/extend_class.html
--rw-r--r--   0        0        0       73 2024-04-09 21:50:46.125635 django_includecontents-0.5/tests/templates/test_component/index.html
--rw-r--r--   0        0        0       34 2024-04-09 21:51:49.385743 django_includecontents-0.5/tests/templates/test_component/missing_attr.html
--rw-r--r--   0        0        0       24 2024-04-09 21:51:57.449090 django_includecontents-0.5/tests/templates/test_component/missing_closing_tag.html
--rw-r--r--   0        0        0      118 2024-04-09 21:50:46.115635 django_includecontents-0.5/tests/templates/test_tag/basic.html
--rw-r--r--   0        0        0       57 2024-04-09 04:52:09.297567 django_includecontents-0.5/tests/templates/test_tag/inner.html
--rw-r--r--   0        0        0      135 2024-04-09 21:50:46.115635 django_includecontents-0.5/tests/templates/test_tag/with_attr.html
--rw-r--r--   0        0        0     1478 2024-04-18 05:37:15.283141 django_includecontents-0.5/tests/test_component.py
--rw-r--r--   0        0        0      130 2024-04-09 04:52:09.297567 django_includecontents-0.5/tests/test_multiline.py
--rw-r--r--   0        0        0      454 2024-04-09 04:52:09.297567 django_includecontents-0.5/tests/test_tag.py
--rw-r--r--   0        0        0     6307 1970-01-01 00:00:00.000000 django_includecontents-0.5/PKG-INFO
+-rw-r--r--   0        0        0     5293 2024-04-19 04:27:39.460145 django_includecontents-0.5.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-0.5.1/includecontents/__init__.py
+-rw-r--r--   0        0        0     1000 2024-04-19 05:13:37.190112 django_includecontents-0.5.1/includecontents/backend.py
+-rw-r--r--   0        0        0     4596 2024-04-19 05:31:33.346108 django_includecontents-0.5.1/includecontents/base.py
+-rw-r--r--   0        0        0     1401 2024-04-09 04:42:05.196722 django_includecontents-0.5.1/includecontents/engine.py
+-rw-r--r--   0        0        0     1663 2024-04-18 05:37:15.283141 django_includecontents-0.5.1/includecontents/loaders.py
+-rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-0.5.1/includecontents/templatetags/__init__.py
+-rw-r--r--   0        0        0    15216 2024-04-18 05:47:45.081186 django_includecontents-0.5.1/includecontents/templatetags/includecontents.py
+-rw-r--r--   0        0        0     1220 2024-04-19 05:32:25.826233 django_includecontents-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      144 2024-04-19 05:31:17.752738 django_includecontents-0.5.1/tests/settings.py
+-rw-r--r--   0        0        0      168 2024-04-18 05:37:15.283141 django_includecontents-0.5.1/tests/templates/components/card.html
+-rw-r--r--   0        0        0      160 2024-04-18 05:37:15.283141 django_includecontents-0.5.1/tests/templates/components/card_extend.html
+-rw-r--r--   0        0        0       81 2024-04-09 04:52:09.297567 django_includecontents-0.5.1/tests/templates/multiline.html
+-rw-r--r--   0        0        0      115 2024-04-09 21:50:46.125635 django_includecontents-0.5.1/tests/templates/test_component/attrs.html
+-rw-r--r--   0        0        0      162 2024-04-18 05:37:15.283141 django_includecontents-0.5.1/tests/templates/test_component/extend_class.html
+-rw-r--r--   0        0        0       73 2024-04-09 21:50:46.125635 django_includecontents-0.5.1/tests/templates/test_component/index.html
+-rw-r--r--   0        0        0       34 2024-04-09 21:51:49.385743 django_includecontents-0.5.1/tests/templates/test_component/missing_attr.html
+-rw-r--r--   0        0        0       24 2024-04-09 21:51:57.449090 django_includecontents-0.5.1/tests/templates/test_component/missing_closing_tag.html
+-rw-r--r--   0        0        0      118 2024-04-09 21:50:46.115635 django_includecontents-0.5.1/tests/templates/test_tag/basic.html
+-rw-r--r--   0        0        0       57 2024-04-09 04:52:09.297567 django_includecontents-0.5.1/tests/templates/test_tag/inner.html
+-rw-r--r--   0        0        0      135 2024-04-09 21:50:46.115635 django_includecontents-0.5.1/tests/templates/test_tag/with_attr.html
+-rw-r--r--   0        0        0     1626 2024-04-19 05:30:37.315975 django_includecontents-0.5.1/tests/test_component.py
+-rw-r--r--   0        0        0      130 2024-04-09 04:52:09.297567 django_includecontents-0.5.1/tests/test_multiline.py
+-rw-r--r--   0        0        0      454 2024-04-09 04:52:09.297567 django_includecontents-0.5.1/tests/test_tag.py
+-rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 django_includecontents-0.5.1/PKG-INFO
```

### Comparing `django_includecontents-0.5/README.md` & `django_includecontents-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.5/includecontents/backend.py` & `django_includecontents-0.5.1/includecontents/backend.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.5/includecontents/base.py` & `django_includecontents-0.5.1/includecontents/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                 " ".join(content),
                 position,
                 lineno,
             )
         return super().create_token(token_string, position, lineno, in_tag)
 
 
-class DebugLexer(django.template.base.DebugLexer):
+class DebugLexer(django.template.base.DebugLexer, Lexer):
     def _tag_re_split_positions(self):
         last = 0
         for match in tag_re.finditer(self.template_string):
             start, end = match.span()
             yield last, start
             yield start, end
             last = end
```

### Comparing `django_includecontents-0.5/includecontents/engine.py` & `django_includecontents-0.5.1/includecontents/engine.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.5/includecontents/loaders.py` & `django_includecontents-0.5.1/includecontents/loaders.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.5/includecontents/templatetags/includecontents.py` & `django_includecontents-0.5.1/includecontents/templatetags/includecontents.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.5/pyproject.toml` & `django_includecontents-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-includecontents"
-version = "0.5"
+version = "0.5.1"
 description = "Django includecontents component-like tag"
 authors = [
     { name = "Chris Beaven", email = "smileychris@gmail.com" },
 ]
 dependencies = [
     "django",
 ]
```

### Comparing `django_includecontents-0.5/tests/test_component.py` & `django_includecontents-0.5.1/tests/test_component.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import re
 
 import pytest
 from django.template import TemplateSyntaxError
 from django.template.loader import render_to_string
+from django.test import override_settings
 
 
 def test_basic():
     assert render_to_string("test_component/index.html") == (
         """<main>
   <section class="card">
   <h3 >hello</h3>
   <div>some content</div>
 </section>
 </main>
 """
     )
 
 
+@override_settings(DEBUG=True)
+def test_debug_mode():
+    render_to_string("test_component/index.html")
+
+
 def test_attrs():
     assert render_to_string("test_component/attrs.html") == (
         """<main>
   <section class="mycard" id="topcard">
   <h3 class="large">hello</h3>
   <div>
     some content
```

### Comparing `django_includecontents-0.5/PKG-INFO` & `django_includecontents-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-includecontents
-Version: 0.5
+Version: 0.5.1
 Summary: Django includecontents component-like tag
 Author-Email: Chris Beaven <smileychris@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

