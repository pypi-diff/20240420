# Comparing `tmp/mkdocs_ezglossary_plugin-1.6.0.tar.gz` & `tmp/mkdocs_ezglossary_plugin-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_ezglossary_plugin-1.6.0.tar", last modified: Fri Apr 19 13:38:18 2024, max compression
+gzip compressed data, was "mkdocs_ezglossary_plugin-1.6.1.tar", last modified: Sat Apr 20 07:37:23 2024, max compression
```

## Comparing `mkdocs_ezglossary_plugin-1.6.0.tar` & `mkdocs_ezglossary_plugin-1.6.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:18.375218 mkdocs_ezglossary_plugin-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 13:37:53.000000 mkdocs_ezglossary_plugin-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-19 13:38:18.375218 mkdocs_ezglossary_plugin-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-19 13:37:53.000000 mkdocs_ezglossary_plugin-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-19 13:37:53.000000 mkdocs_ezglossary_plugin-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-19 13:38:18.375218 mkdocs_ezglossary_plugin-1.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:18.371219 mkdocs_ezglossary_plugin-1.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:18.371219 mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:37:53.000000 mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-19 13:37:53.000000 mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin/glossary.py
--rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-04-19 13:37:53.000000 mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-19 13:37:53.000000 mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:18.375218 mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-19 13:37:53.000000 mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin/templates/definition.html
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-19 13:37:53.000000 mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin/templates/link.html
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-19 13:37:53.000000 mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin/templates/refs-list.html
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-19 13:37:53.000000 mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin/templates/refs-short.html
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-19 13:37:53.000000 mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-19 13:37:53.000000 mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin/templates/summary-table.html
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-19 13:37:53.000000 mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin/templates/summary.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:18.375218 mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-19 13:38:18.000000 mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-19 13:38:18.000000 mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:38:18.000000 mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-19 13:38:18.000000 mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 13:38:18.000000 mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 13:38:18.000000 mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:18.375218 mkdocs_ezglossary_plugin-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-19 13:37:53.000000 mkdocs_ezglossary_plugin-1.6.0/tests/test_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-19 13:37:53.000000 mkdocs_ezglossary_plugin-1.6.0/tests/test_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-19 13:37:53.000000 mkdocs_ezglossary_plugin-1.6.0/tests/test_page_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-19 13:37:53.000000 mkdocs_ezglossary_plugin-1.6.0/tests/test_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:37:23.754479 mkdocs_ezglossary_plugin-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-20 07:36:58.000000 mkdocs_ezglossary_plugin-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-20 07:37:23.754479 mkdocs_ezglossary_plugin-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-20 07:36:58.000000 mkdocs_ezglossary_plugin-1.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-20 07:36:58.000000 mkdocs_ezglossary_plugin-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-20 07:37:23.754479 mkdocs_ezglossary_plugin-1.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:37:23.750479 mkdocs_ezglossary_plugin-1.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:37:23.750479 mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 07:36:58.000000 mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-20 07:36:58.000000 mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin/glossary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-04-20 07:36:58.000000 mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-20 07:36:58.000000 mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:37:23.754479 mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-20 07:36:58.000000 mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin/templates/definition.html
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-20 07:36:58.000000 mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin/templates/link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-20 07:36:58.000000 mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin/templates/refs-list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-20 07:36:58.000000 mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin/templates/refs-short.html
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-20 07:36:58.000000 mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-20 07:36:58.000000 mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin/templates/summary-table.html
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-20 07:36:58.000000 mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin/templates/summary.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:37:23.754479 mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-20 07:37:23.000000 mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-20 07:37:23.000000 mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 07:37:23.000000 mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-20 07:37:23.000000 mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-20 07:37:23.000000 mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-20 07:37:23.000000 mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:37:23.754479 mkdocs_ezglossary_plugin-1.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-20 07:36:58.000000 mkdocs_ezglossary_plugin-1.6.1/tests/test_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-20 07:36:58.000000 mkdocs_ezglossary_plugin-1.6.1/tests/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-20 07:36:58.000000 mkdocs_ezglossary_plugin-1.6.1/tests/test_page_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-20 07:36:58.000000 mkdocs_ezglossary_plugin-1.6.1/tests/test_summary.py
```

### Comparing `mkdocs_ezglossary_plugin-1.6.0/LICENSE` & `mkdocs_ezglossary_plugin-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.0/PKG-INFO` & `mkdocs_ezglossary_plugin-1.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ezglossary-plugin
-Version: 1.6.0
+Version: 1.6.1
 Summary: manage multiple glossaries in mkdocs
 Project-URL: Homepage, https://github.com/realtimeprojects/mkdocs-ezglossary
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/mkdocs-ezglossary/issues
 Project-URL: Documentation, https://realtimeprojects.github.io/mkdocs-ezglossary
 Keywords: mkdocs,glossary,plugin,references,links
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mkdocs_ezglossary_plugin-1.6.0/README.md` & `mkdocs_ezglossary_plugin-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.0/setup.cfg` & `mkdocs_ezglossary_plugin-1.6.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mkdocs-ezglossary-plugin
-version = 1.6.0
+version = 1.6.1
 description = manage multiple glossaries in mkdocs
 keywords = mkdocs, glossary, plugin, references, links
 long_description = file: README.md
 long_description_content_type = text/markdown
 project_urls = 
 	Homepage = https://github.com/realtimeprojects/mkdocs-ezglossary
 	Bug Tracker = https://github.com/realtimeprojects/mkdocs-ezglossary/issues
```

### Comparing `mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin/glossary.py` & `mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin/glossary.py`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin/plugin.py` & `mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,14 @@
                     if isinstance(term, dict):
                         for term, anchor in term.items():
                             _add2section(section, term, anchor)
         return content
 
     @event_priority(5000)
     def on_page_content(self, content, page, config, files):
-        log.warning(content)
         content = self._find_definitions(content, page)
         content = self._register_glossary_links(content, page)
         return content
 
     def on_post_page(self, output, page, config):
         _dir = os.path.dirname(page.url)
         levels = len(_dir.split("/"))
@@ -170,19 +169,17 @@
             term = term if term else "__None__"
             text = text if text else "__None__"
             log.warning(f"glossary: found {section}/{term}/{text}")
             _id = self._glossary.add(section, term, 'refs', page)
             return f"{self._uuid}:{section}:{term}:<{text}>:{_id}"
 
         def _replace(mo):
-            log.warning(mo.groups())
             return _add_link(mo.group(1), mo.group(2), mo.group(4))
 
         def _replace_default(mo):
-            log.warning(mo.groups())
             return _add_link(None, mo.group(1), mo.group(3))
 
         def _replace_href(mo):
             return _add_link(mo.group(2), mo.group(3), mo.group(4))
 
         regex = rf"<{_re.section}\:{_re.term}(\\?\|({_re.text}))?>"
         output = re.sub(regex, _replace, output)
```

### Comparing `mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin/template.py` & `mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin/template.py`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html` & `mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin/templates/summary-table.html` & `mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin/templates/summary-table.html`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin/templates/summary.html` & `mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin/templates/summary.html`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO` & `mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ezglossary-plugin
-Version: 1.6.0
+Version: 1.6.1
 Summary: manage multiple glossaries in mkdocs
 Project-URL: Homepage, https://github.com/realtimeprojects/mkdocs-ezglossary
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/mkdocs-ezglossary/issues
 Project-URL: Documentation, https://realtimeprojects.github.io/mkdocs-ezglossary
 Keywords: mkdocs,glossary,plugin,references,links
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mkdocs_ezglossary_plugin-1.6.0/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt` & `mkdocs_ezglossary_plugin-1.6.1/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs_ezglossary_plugin-1.6.0/tests/test_definitions.py` & `mkdocs_ezglossary_plugin-1.6.1/tests/test_definitions.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,70 +7,70 @@
 log = logging.getLogger(__name__)
 
 
 def test_default_config(simple, config):
     html = mock.render_single(simple, config)
     log.debug(html)
     dl = xpath.dl
-    dl = dl.has(xpath.dt.has(xpath.a(name="test_first_defs_0", text="first")))
+    dl = dl.has(xpath.dt.has(xpath.a(id="test_first_defs_0", text="first")))
     dl = dl.has(xpath.dd(text="first term"))
-    dl = dl.has(xpath.dt.has(xpath.a(name="test_second_defs_0", text="second")))
+    dl = dl.has(xpath.dt.has(xpath.a(id="test_second_defs_0", text="second")))
     dl = dl.has(xpath.dd(text="*second term"))
     assert len(html.xpath(str(dl)))
 
     dl = xpath.dl
-    dl = dl.has(xpath.dt.has(xpath.a(name="demo_first_defs_0", text="first")))
+    dl = dl.has(xpath.dt.has(xpath.a(id="demo_first_defs_0", text="first")))
     dl = dl.has(xpath.dd(text="demo 1"))
-    dl = dl.has(xpath.dt.has(xpath.a(name="demo_second_defs_0", text="second")))
+    dl = dl.has(xpath.dt.has(xpath.a(id="demo_second_defs_0", text="second")))
     dl = dl.has(xpath.dd(text="demo 2"))
     assert len(html.xpath(str(dl)))
 
     dl = xpath.dl
     dl = dl.has(xpath.dd(text="*demo 2").has(xpath.a()))
     assert len(html.xpath(str(dl))) == 0
 
 
 def test_inline_refs(simple, config):
     config['inline_refs'] = "short"
     html = mock.render_single(simple, config)
 
     dl = xpath.dl
-    dl = dl.has(xpath.dt.has(xpath.a(name="test_first_defs_0", text="first")))
+    dl = dl.has(xpath.dt.has(xpath.a(id="test_first_defs_0", text="first")))
     dl = dl.has(xpath.dd(text="*first term").has(xpath.a()))
     assert len(html.xpath(str(dl))) == 0
 
     dl = xpath.dl()
-    dl = dl.has(xpath.dt.has(xpath.a(name="test_third_defs_0", text="third")))
+    dl = dl.has(xpath.dt.has(xpath.a(id="test_third_defs_0", text="third")))
     dl = dl.has(xpath.dd(text="*third term").has(xpath.a(title="Hello",
                                                          href="../simple.md#test_third_refs_0",
                                                          text="*[1]")))
     assert len(html.xpath(str(dl))) == 1
 
 
 def test_default_section(simple, config):
     config['use_default'] = True
     html = mock.render_single(simple, config)
     log.debug(html)
     dl = xpath.dl
-    dl = dl.has(xpath.dt.has(xpath.a(name="__default_defs_0", text="default")))
+    dl = dl.has(xpath.dt.has(xpath.a(id="__default_defs_0", text="default")))
     dl = dl.has(xpath.dd(text="default term"))
     assert len(html.xpath(str(dl)))
 
     dl = xpath.dl
-    dl = dl.has(xpath.dt.has(xpath.a(name="demo_first_defs_0", text="first")))
+    dl = dl.has(xpath.dt.has(xpath.a(id="demo_first_defs_0", text="first")))
     dl = dl.has(xpath.dd(text="demo 1"))
-    dl = dl.has(xpath.dt.has(xpath.a(name="demo_second_defs_0", text="second")))
+    dl = dl.has(xpath.dt.has(xpath.a(id="demo_second_defs_0", text="second")))
     dl = dl.has(xpath.dd(text="demo 2"))
     assert len(html.xpath(str(dl)))
 
     dl = xpath.dl
     dl = dl.has(xpath.dd(text="*demo 2").has(xpath.a()))
     assert len(html.xpath(str(dl))) == 0
 
 
 def test_formatted_dt(simple, config):
     html = mock.render_single(simple, config)
     log.debug(html)
     dl = xpath.dl
-    dl = dl.has(xpath.dt.bold.em.code.has(xpath.a(name="demo_formatted_defs_0", text="formatted")))
+    dl = dl.has(xpath.dt.bold.em.code.has(xpath.a(id="demo_formatted_defs_0", text="formatted")))
     dl = dl.has(xpath.dd(text="formatted dd"))
     assert len(html.xpath(str(dl)))
```

### Comparing `mkdocs_ezglossary_plugin-1.6.0/tests/test_link.py` & `mkdocs_ezglossary_plugin-1.6.1/tests/test_link.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,69 +5,69 @@
 
 log = logging.getLogger(__name__)
 
 
 def test_link_no_title(simple, config):
     html = mock.render_single(simple, config)
 
-    dl = xpath.body.p.a(name="test_third_refs_0",
+    dl = xpath.body.p.a(id="test_third_refs_0",
                         title="",
                         href="../simple.md#test_third_defs_0",
                         text="third")
     assert len(html.xpath(str(dl))) == 1
 
 
 def test_link_short_title(simple, config):
     config['tooltip'] = "short"
     html = mock.render_single(simple, config)
     log.debug(html)
 
-    dl = xpath.body.p.a(name="test_third_refs_0",
+    dl = xpath.body.p.a(id="test_third_refs_0",
                         title="third term",
                         href="../simple.md#test_third_defs_0",
                         text="third")
     assert len(html.xpath(str(dl))) == 1
 
 
 def test_link_full_title(simple, config):
     config['tooltip'] = "full"
     html = mock.render_single(simple, config)
     log.debug(html)
 
     dl = xpath.body.p.a(_class="mkdocs-ezglossary-link",
-                        name="test_third_refs_0",
+                        id="test_third_refs_0",
                         title="*detailed description of third term",
                         href="../simple.md#test_third_defs_0",
                         text="third")
     assert len(html.xpath(str(dl))) == 1
 
 
 def test_link_replace_html(simple, config):
     config['tooltip'] = "full"
     html = mock.render_single(simple, config)
     log.debug(html)
 
-    dl = xpath.body.p.a(name="test_second_refs_0",
+    dl = xpath.body.p.a(id="test_second_refs_0",
                         title="*this text is formatted",
                         href="../simple.md#test_second_defs_0",
                         text="mysecond")
     assert len(html.xpath(str(dl))) == 1
 
 
 def test_link_second_ref(simple, summary, config):
     config['tooltip'] = "full"
     summary = mock.render([simple, summary], config)['summary.md']
     log.debug(summary)
 
-    dl = xpath.body.p.a(name="test_third_refs_1",
+    dl = xpath.body.p.a(id="test_third_refs_1",
                         title="*third term",
                         href="../simple.md#test_third_defs_0",
                         text="third")
     assert len(summary.xpath(str(dl))) == 1
-    dl = xpath.body.p.a(name="test_third_refs_2",
+    dl = xpath.body.p.a(id="test_third_refs_2",
                         title="*third term",
                         href="../simple.md#test_third_defs_0",
                         text="mythird")
     assert len(summary.xpath(str(dl))) == 1
 
 
 def test_link_default_ref_dis(simple, summary, config):
@@ -75,15 +75,15 @@
         ignored when the configuration `use_default` is set
         to `False`.
     """
     summary = mock.render([simple, summary], config)['summary.md']
     log.debug(summary)
 
     dl = xpath.body.p.a(_class="mkdocs-ezglossary-link",
-                        name="__default_refs_0",
+                        id="__default_refs_0",
                         title="",
                         href="../simple.md#__default_defs_0",
                         text="default")
     assert len(summary.xpath(str(dl))) == 0
 
 
 def test_link_default_ref_enabled(simple, summary, config):
@@ -92,27 +92,27 @@
         to `True`.
     """
     config['use_default'] = True
     summary = mock.render([simple, summary], config)['summary.md']
     log.debug(summary)
 
     dl = xpath.body.p.a(_class="mkdocs-ezglossary-link",
-                        name="__default_refs_0",
+                        id="__default_refs_0",
                         title="",
                         href="../simple.md#__default_defs_0",
                         text="default")
     assert len(summary.xpath(str(dl))) == 1
     dl = xpath.body.p.a(_class="mkdocs-ezglossary-link",
-                        name="__default2_refs_0",
+                        id="__default2_refs_0",
                         title="",
                         href="../simple.md#__default2_defs_0",
                         text="mydef2")
     assert len(summary.xpath(str(dl))) == 1
     dl = xpath.body.p.a(_class="mkdocs-ezglossary-link",
-                        name="__default3_refs_0",
+                        id="__default3_refs_0",
                         title="",
                         href="../simple.md#__default3_defs_0",
                         text="mydef3")
     assert len(summary.xpath(str(dl))) == 1
 
 
 def test_markdown_links_disabled(simple, summary, config):
@@ -129,17 +129,17 @@
 def test_markdown_links_enabled(simple, summary, config):
     """ Ensure markdown links are resolved when `markdown_links` is set to true.
     """
     config['markdown_links'] = True
     summary = mock.render([simple, summary], config)['summary.md']
     log.debug(summary)
 
-    dl = xpath.body.p.a(name="test_third_refs_1",
+    dl = xpath.body.p.a(id="test_third_refs_1",
                         title="",
                         href="../simple.md#test_third_defs_0",
                         text="third")
     assert len(summary.xpath(str(dl))) == 1
-    dl = xpath.body.p.a(name="test_third_refs_2",
+    dl = xpath.body.p.a(id="test_third_refs_2",
                         title="",
                         href="../simple.md#test_third_defs_0",
                         text="mythird")
     assert len(summary.xpath(str(dl))) == 1
```

### Comparing `mkdocs_ezglossary_plugin-1.6.0/tests/test_page_ref.py` & `mkdocs_ezglossary_plugin-1.6.1/tests/test_page_ref.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,12 +127,12 @@
     assert len(pages['commands.md'].xpath(str(dl))) == 1
 
 
 def test_page_ref_link(config):
     pages = mock.render([mycommand, commands], config)
 
     dl = xp.body.p.a(_class="mkdocs-ezglossary-link",
-                     name="cmd_help2_refs_0",
+                     id="cmd_help2_refs_0",
                      title="page subtitle",
                      href="../mycommand.md#",
                      text="help2")
     assert len(pages['commands.md'].xpath(str(dl))) == 1
```

### Comparing `mkdocs_ezglossary_plugin-1.6.0/tests/test_summary.py` & `mkdocs_ezglossary_plugin-1.6.1/tests/test_summary.py`

 * *Files identical despite different names*

