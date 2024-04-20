# Comparing `tmp/mkdocs_section_index-0.3.8.tar.gz` & `tmp/mkdocs_section_index-0.3.9.tar.gz`

## Comparing `mkdocs_section_index-0.3.8.tar` & `mkdocs_section_index-0.3.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/mkdocs_section_index/__init__.py
--rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/mkdocs_section_index/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/mkdocs_section_index/py.typed
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/mkdocs_section_index/rewrites.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/tests/conftest.py
--rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/tests/test_integration.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/tests/test_plugin.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/tests/test_rewrites.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/tests/navs/basic.yml
--rw-r--r--   0        0        0     5970 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/tests/rewrites/material-nav-item-1.yml
--rw-r--r--   0        0        0     5434 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/tests/rewrites/material-nav-item-2.yml
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/tests/rewrites/material-nav-item-3.yml
--rw-r--r--   0        0        0     7385 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/tests/rewrites/material-nav-item-4.yml
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/tests/rewrites/material-tabs-item-1.yml
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/tests/rewrites/material-tabs-item-2.yml
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/tests/rewrites/mkdocs-sitemap-1.yml
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/tests/rewrites/readthedocs-base-1.yml
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/LICENSE.md
--rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/README.md
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/mkdocs_section_index/__init__.py
+-rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/mkdocs_section_index/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/mkdocs_section_index/py.typed
+-rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/mkdocs_section_index/rewrites.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/tests/conftest.py
+-rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/tests/test_integration.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/tests/test_plugin.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/tests/test_rewrites.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/tests/navs/basic.yml
+-rw-r--r--   0        0        0     5970 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/tests/rewrites/material-nav-item-1.yml
+-rw-r--r--   0        0        0     5434 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/tests/rewrites/material-nav-item-2.yml
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/tests/rewrites/material-nav-item-3.yml
+-rw-r--r--   0        0        0     7385 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/tests/rewrites/material-nav-item-4.yml
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/tests/rewrites/material-tabs-item-1.yml
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/tests/rewrites/material-tabs-item-2.yml
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/tests/rewrites/mkdocs-sitemap-1.yml
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/tests/rewrites/readthedocs-base-1.yml
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/LICENSE.md
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/README.md
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     7827 2020-02-02 00:00:00.000000 mkdocs_section_index-0.3.9/PKG-INFO
```

### Comparing `mkdocs_section_index-0.3.8/mkdocs_section_index/__init__.py` & `mkdocs_section_index-0.3.9/mkdocs_section_index/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 from mkdocs.structure.nav import Section
 from mkdocs.structure.pages import Page
 
-__version__ = "0.3.8"
+__version__ = "0.3.9"
 __all__ = ["SectionPage"]
 
 
 class SectionPage(Section, Page):  # type: ignore[misc]
     def __init__(self, title: str, file, config, children):
         Page.__init__(self, title=title, file=file, config=config)
         Section.__init__(self, title=title, children=children)
         self.is_section = self.is_page = True
 
-    active = Page.active  # type: ignore
+    active = Page.active  # type: ignore[assignment]
 
     def __repr__(self):
         result = Page.__repr__(self)
         if not result.startswith("Section"):
             result = "Section" + result
         return result
```

### Comparing `mkdocs_section_index-0.3.8/mkdocs_section_index/plugin.py` & `mkdocs_section_index-0.3.9/mkdocs_section_index/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_section_index-0.3.8/mkdocs_section_index/rewrites.py` & `mkdocs_section_index-0.3.9/mkdocs_section_index/rewrites.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,21 +58,21 @@
                 f"Failed to adapt the theme file '{filename}'. "
                 f"This is likely a bug in mkdocs-section-index, and things won't work as expected."
             )
         return src or old_src, filename, uptodate
 
 
 def _transform_mkdocs_sitemap_template(src: str) -> str | None:
-    if " in pages " not in src:
-        # The below only for versions <= 1.1.2.
-        return src.replace(
-            "{%- else %}",
-            "{%- endif %}{% if item.url %}",
-        )
-    return None
+    if " in pages " in src:
+        return None
+    # The below only for versions <= 1.1.2.
+    return src.replace(
+        "{%- else %}",
+        "{%- endif %}{% if item.url %}",
+    )
 
 
 def _transform_material_nav_item_template(src: str) -> str:
     if "navigation.indexes" in src:
         return src.replace(
             "{% set indexes = [] %}",
             "{% set indexes = [nav_item] if nav_item.url else [] %}",
@@ -116,15 +116,18 @@
         "(nav_item.url or (nav_item.children | first).url)",
     ).replace(
         "if (nav_item.children | first).children",
         "if (nav_item.children | first).children and not nav_item.url",
     )
 
 
-def _transform_readthedocs_base_template(src: str) -> str:
+def _transform_readthedocs_base_template(src: str) -> str | None:
+    if " if nav_item.is_page " in src:
+        return None
+    # The below only for versions < 1.6:
     repl = """\
         {% if nav_item.url %}
             <ul><li{% if nav_item == page %} class="current"{% endif %}>
                 <a href="{{ nav_item.url|url }}" style="padding: 0; font-size: inherit; line-height: inherit">
         {% endif %}
                 [...]
         {% if nav_item.url %}
```

### Comparing `mkdocs_section_index-0.3.8/tests/conftest.py` & `mkdocs_section_index-0.3.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mkdocs_section_index-0.3.8/tests/test_integration.py` & `mkdocs_section_index-0.3.9/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `mkdocs_section_index-0.3.8/tests/test_plugin.py` & `mkdocs_section_index-0.3.9/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_section_index-0.3.8/tests/test_rewrites.py` & `mkdocs_section_index-0.3.9/tests/test_rewrites.py`

 * *Files identical despite different names*

### Comparing `mkdocs_section_index-0.3.8/tests/navs/basic.yml` & `mkdocs_section_index-0.3.9/tests/navs/basic.yml`

 * *Files identical despite different names*

### Comparing `mkdocs_section_index-0.3.8/tests/rewrites/material-nav-item-1.yml` & `mkdocs_section_index-0.3.9/tests/rewrites/material-nav-item-1.yml`

 * *Files identical despite different names*

### Comparing `mkdocs_section_index-0.3.8/tests/rewrites/material-nav-item-2.yml` & `mkdocs_section_index-0.3.9/tests/rewrites/material-nav-item-2.yml`

 * *Files identical despite different names*

### Comparing `mkdocs_section_index-0.3.8/tests/rewrites/material-nav-item-3.yml` & `mkdocs_section_index-0.3.9/tests/rewrites/material-nav-item-3.yml`

 * *Files identical despite different names*

### Comparing `mkdocs_section_index-0.3.8/tests/rewrites/material-nav-item-4.yml` & `mkdocs_section_index-0.3.9/tests/rewrites/material-nav-item-4.yml`

 * *Files identical despite different names*

### Comparing `mkdocs_section_index-0.3.8/tests/rewrites/material-tabs-item-1.yml` & `mkdocs_section_index-0.3.9/tests/rewrites/material-tabs-item-1.yml`

 * *Files identical despite different names*

### Comparing `mkdocs_section_index-0.3.8/tests/rewrites/material-tabs-item-2.yml` & `mkdocs_section_index-0.3.9/tests/rewrites/material-tabs-item-2.yml`

 * *Files identical despite different names*

### Comparing `mkdocs_section_index-0.3.8/tests/rewrites/mkdocs-sitemap-1.yml` & `mkdocs_section_index-0.3.9/tests/rewrites/mkdocs-sitemap-1.yml`

 * *Files identical despite different names*

### Comparing `mkdocs_section_index-0.3.8/tests/rewrites/readthedocs-base-1.yml` & `mkdocs_section_index-0.3.9/tests/rewrites/readthedocs-base-1.yml`

 * *Files identical despite different names*

### Comparing `mkdocs_section_index-0.3.8/LICENSE.md` & `mkdocs_section_index-0.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs_section_index-0.3.8/README.md` & `mkdocs_section_index-0.3.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # mkdocs-section-index
 
 **[Plugin][] for [MkDocs][] to allow clickable sections that lead to an index page**
 
 [![PyPI](https://img.shields.io/pypi/v/mkdocs-section-index)](https://pypi.org/project/mkdocs-section-index/)
-[![GitHub](https://img.shields.io/github/license/oprypin/mkdocs-section-index)](https://github.com/oprypin/mkdocs-section-index/blob/master/LICENSE.md)
+[![License](https://img.shields.io/github/license/oprypin/mkdocs-section-index)](https://github.com/oprypin/mkdocs-section-index/blob/master/LICENSE.md)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/oprypin/mkdocs-section-index/ci.yml.svg)](https://github.com/oprypin/mkdocs-section-index/actions?query=event%3Apush+branch%3Amaster)
 
 ```shell
 pip install mkdocs-section-index
 ```
 
 [mkdocs]: https://www.mkdocs.org/
```

### Comparing `mkdocs_section_index-0.3.8/PKG-INFO` & `mkdocs_section_index-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mkdocs-section-index
-Version: 0.3.8
+Version: 0.3.9
 Summary: MkDocs plugin to allow clickable sections that lead to an index page
 Project-URL: Documentation, https://oprypin.github.io/mkdocs-section-index/
 Project-URL: Source, https://github.com/oprypin/mkdocs-section-index
 Project-URL: Issues, https://github.com/oprypin/mkdocs-section-index/issues
 Project-URL: History, https://github.com/oprypin/mkdocs-section-index/releases
 Author-email: Oleh Prypin <oleh@pryp.in>
 License-Expression: MIT
@@ -13,33 +13,33 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: mkdocs>=1.2
 Description-Content-Type: text/markdown
 
 # mkdocs-section-index
 
 **[Plugin][] for [MkDocs][] to allow clickable sections that lead to an index page**
 
 [![PyPI](https://img.shields.io/pypi/v/mkdocs-section-index)](https://pypi.org/project/mkdocs-section-index/)
-[![GitHub](https://img.shields.io/github/license/oprypin/mkdocs-section-index)](https://github.com/oprypin/mkdocs-section-index/blob/master/LICENSE.md)
+[![License](https://img.shields.io/github/license/oprypin/mkdocs-section-index)](https://github.com/oprypin/mkdocs-section-index/blob/master/LICENSE.md)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/oprypin/mkdocs-section-index/ci.yml.svg)](https://github.com/oprypin/mkdocs-section-index/actions?query=event%3Apush+branch%3Amaster)
 
 ```shell
 pip install mkdocs-section-index
 ```
 
 [mkdocs]: https://www.mkdocs.org/
```

