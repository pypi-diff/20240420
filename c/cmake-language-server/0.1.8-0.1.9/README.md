# Comparing `tmp/cmake_language_server-0.1.8.tar.gz` & `tmp/cmake_language_server-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmake_language_server-0.1.8.tar", last modified: Tue Oct 17 14:00:48 2023, max compression
+gzip compressed data, was "cmake_language_server-0.1.9.tar", last modified: Mon Jan  1 03:40:01 2024, max compression
```

## Comparing `cmake_language_server-0.1.8.tar` & `cmake_language_server-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1062 2023-10-17 14:00:32.920831 cmake_language_server-0.1.8/LICENSE
--rw-r--r--   0        0        0     2359 2023-10-17 14:00:32.920831 cmake_language_server-0.1.8/README.md
--rw-r--r--   0        0        0       60 2023-10-17 14:00:32.920831 cmake_language_server-0.1.8/cmake_language_server/__init__.py
--rw-r--r--   0        0        0    11760 2023-10-17 14:00:32.920831 cmake_language_server-0.1.8/cmake_language_server/api.py
--rw-r--r--   0        0        0     9028 2023-10-17 14:00:32.920831 cmake_language_server-0.1.8/cmake_language_server/server.py
--rw-r--r--   0        0        0       22 2023-10-17 14:00:48.524893 cmake_language_server-0.1.8/cmake_language_server/version.py
--rw-r--r--   0        0        0     1563 2023-10-17 14:00:48.524893 cmake_language_server-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-17 14:00:32.920831 cmake_language_server-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0     1733 2023-10-17 14:00:32.920831 cmake_language_server-0.1.8/tests/conftest.py
--rw-r--r--   0        0        0      129 2023-10-17 14:00:32.920831 cmake_language_server-0.1.8/tests/data/cmake/CMakeLists.txt
--rw-r--r--   0        0        0        0 2023-10-17 14:00:32.920831 cmake_language_server-0.1.8/tests/data/cmake/lib.cpp
--rw-r--r--   0        0        0       47 2023-10-17 14:00:32.920831 cmake_language_server-0.1.8/tests/data/cmake/main.cpp
--rw-r--r--   0        0        0     3566 2023-10-17 14:00:32.920831 cmake_language_server-0.1.8/tests/test_api.py
--rw-r--r--   0        0        0     5012 2023-10-17 14:00:32.920831 cmake_language_server-0.1.8/tests/test_server.py
--rw-r--r--   0        0        0     3017 1970-01-01 00:00:00.000000 cmake_language_server-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-01-01 03:39:50.260384 cmake_language_server-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2359 2024-01-01 03:39:50.260384 cmake_language_server-0.1.9/README.md
+-rw-r--r--   0        0        0       60 2024-01-01 03:39:50.260384 cmake_language_server-0.1.9/cmake_language_server/__init__.py
+-rw-r--r--   0        0        0    11760 2024-01-01 03:39:50.260384 cmake_language_server-0.1.9/cmake_language_server/api.py
+-rw-r--r--   0        0        0     9607 2024-01-01 03:39:50.260384 cmake_language_server-0.1.9/cmake_language_server/server.py
+-rw-r--r--   0        0        0       22 2024-01-01 03:40:01.860449 cmake_language_server-0.1.9/cmake_language_server/version.py
+-rw-r--r--   0        0        0     1563 2024-01-01 03:40:01.860449 cmake_language_server-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-01 03:39:50.264384 cmake_language_server-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0     1733 2024-01-01 03:39:50.264384 cmake_language_server-0.1.9/tests/conftest.py
+-rw-r--r--   0        0        0      129 2024-01-01 03:39:50.264384 cmake_language_server-0.1.9/tests/data/cmake/CMakeLists.txt
+-rw-r--r--   0        0        0        0 2024-01-01 03:39:50.264384 cmake_language_server-0.1.9/tests/data/cmake/lib.cpp
+-rw-r--r--   0        0        0       47 2024-01-01 03:39:50.264384 cmake_language_server-0.1.9/tests/data/cmake/main.cpp
+-rw-r--r--   0        0        0     3566 2024-01-01 03:39:50.264384 cmake_language_server-0.1.9/tests/test_api.py
+-rw-r--r--   0        0        0     5047 2024-01-01 03:39:50.264384 cmake_language_server-0.1.9/tests/test_server.py
+-rw-r--r--   0        0        0     3017 1970-01-01 00:00:00.000000 cmake_language_server-0.1.9/PKG-INFO
```

### Comparing `cmake_language_server-0.1.8/LICENSE` & `cmake_language_server-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cmake_language_server-0.1.8/README.md` & `cmake_language_server-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cmake_language_server-0.1.8/cmake_language_server/api.py` & `cmake_language_server-0.1.9/cmake_language_server/api.py`

 * *Files identical despite different names*

### Comparing `cmake_language_server-0.1.8/cmake_language_server/server.py` & `cmake_language_server-0.1.9/cmake_language_server/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -88,27 +88,27 @@
 
             if trigger is None:
                 commands = self._api.search_command(token)
                 items.extend(
                     CompletionItem(
                         label=x,
                         kind=CompletionItemKind.Function,
-                        documentation=self._api.get_command_doc(x),
+                        documentation=self._get_command_doc(x),
                         insert_text=x,
                     )
                     for x in commands
                 )
 
             if trigger is None or trigger == "{":
                 variables = self._api.search_variable(token)
                 items.extend(
                     CompletionItem(
                         label=x,
                         kind=CompletionItemKind.Variable,
-                        documentation=self._api.get_variable_doc(x),
+                        documentation=self._get_variable_doc(x),
                         insert_text=x,
                     )
                     for x in variables
                 )
 
             if trigger is None:
                 targets = self._api.search_target(token)
@@ -125,26 +125,26 @@
                     func = func.lower()
                     if func == "include":
                         modules = self._api.search_module(token, False)
                         items.extend(
                             CompletionItem(
                                 label=x,
                                 kind=CompletionItemKind.Module,
-                                documentation=self._api.get_module_doc(x, False),
+                                documentation=self._get_module_doc(x, False),
                                 insert_text=x,
                             )
                             for x in modules
                         )
                     elif func == "find_package":
                         modules = self._api.search_module(token, True)
                         items.extend(
                             CompletionItem(
                                 label=x,
                                 kind=CompletionItemKind.Module,
-                                documentation=self._api.get_module_doc(x, True),
+                                documentation=self._get_module_doc(x, True),
                                 insert_text=x,
                             )
                             for x in modules
                         )
 
             return CompletionList(is_incomplete=False, items=items)
 
@@ -171,35 +171,29 @@
                         ),
                         new_text=formatted,
                     )
                 ]
 
         @self.feature(TEXT_DOCUMENT_HOVER)
         def hover(params: TextDocumentPositionParams) -> Optional[Hover]:
-            assert self._api is not None
-            api = self._api
-
             word = self._cursor_word(params.text_document.uri, params.position, True)
             if not word:
                 return None
 
-            candidates: List[Callable[[str], Optional[str]]] = [
-                lambda x: api.get_command_doc(x.lower()),
-                lambda x: api.get_variable_doc(x),
-                lambda x: api.get_module_doc(x, False),
-                lambda x: api.get_module_doc(x, True),
+            candidates: List[Callable[[str], Optional[MarkupContent]]] = [
+                lambda x: self._get_command_doc(x.lower()),
+                lambda x: self._get_variable_doc(x),
+                lambda x: self._get_module_doc(x, False),
+                lambda x: self._get_module_doc(x, True),
             ]
             for c in candidates:
                 doc = c(word[0])
                 if doc is None:
                     continue
-                return Hover(
-                    contents=MarkupContent(kind=MarkupKind.Markdown, value=doc),
-                    range=word[1],
-                )
+                return Hover(contents=doc, range=word[1])
             return None
 
         @self.thread()
         @self.feature(
             TEXT_DOCUMENT_DID_SAVE,
             SaveOptions(include_text=False),
         )
@@ -237,14 +231,29 @@
                         start=Position(line=position.line, character=m.start()),
                         end=Position(line=position.line, character=end),
                     ),
                 )
                 return word
         return None
 
+    def _get_command_doc(self, command: str) -> Optional[MarkupContent]:
+        assert self._api is not None
+        docs = self._api.get_command_doc(command)
+        return None if docs is None else MarkupContent(MarkupKind.Markdown, docs)
+
+    def _get_variable_doc(self, variable: str) -> Optional[MarkupContent]:
+        assert self._api is not None
+        docs = self._api.get_variable_doc(variable)
+        return None if docs is None else MarkupContent(MarkupKind.Markdown, docs)
+
+    def _get_module_doc(self, module: str, package: bool) -> Optional[MarkupContent]:
+        assert self._api is not None
+        docs = self._api.get_module_doc(module, package)
+        return None if docs is None else MarkupContent(MarkupKind.Markdown, docs)
+
 
 def main() -> None:
     from argparse import ArgumentParser
 
     from . import __version__
 
     parser = ArgumentParser(description="CMake Language Server")
```

### Comparing `cmake_language_server-0.1.8/pyproject.toml` & `cmake_language_server-0.1.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 description = "CMake LSP Implementation"
 authors = [
     { name = "Regen" },
 ]
 dependencies = [
     "pygls>=1.1.1",
 ]
-requires-python = ">=3.7.9,<3.12"
+requires-python = ">=3.8.0,<3.13"
 readme = "README.md"
 keywords = [
     "cmake",
     "completion",
     "vim",
     "lsp",
 ]
@@ -21,15 +21,15 @@
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development",
     "Topic :: Text Editors :: Integrated Development Environments (IDE)",
     "Topic :: Utilities",
 ]
-version = "0.1.8"
+version = "0.1.9"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 repository = "https://github.com/regen100/cmake-language-server"
```

### Comparing `cmake_language_server-0.1.8/tests/conftest.py` & `cmake_language_server-0.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cmake_language_server-0.1.8/tests/test_api.py` & `cmake_language_server-0.1.9/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `cmake_language_server-0.1.8/tests/test_server.py` & `cmake_language_server-0.1.9/tests/test_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     CompletionParams,
     CompletionTriggerKind,
     DidOpenTextDocumentParams,
     DocumentFormattingParams,
     FormattingOptions,
     HoverParams,
     InitializeParams,
+    MarkupContent,
     Position,
     TextDocumentIdentifier,
     TextDocumentItem,
 )
 from pygls.server import LanguageServer
 
 from cmake_language_server.server import CMakeLanguageServer
@@ -101,16 +102,16 @@
     context: Optional[CompletionContext],
     client_server: Tuple[LanguageServer, CMakeLanguageServer],
     datadir: Path,
 ) -> None:
     response = _test_completion(client_server, datadir, "projec", context)
     item = next(filter(lambda x: x.label == "project", response.items), None)
     assert item is not None
-    assert isinstance(item.documentation, str)
-    assert "<PROJECT-NAME>" in item.documentation
+    assert isinstance(item.documentation, MarkupContent)
+    assert "<PROJECT-NAME>" in item.documentation.value
 
 
 @pytest.mark.parametrize(
     "text, item",
     [("find_package(", "Boost"), ("include(", "GoogleTest"), ("${", "PROJECT_VERSION")],
 )
 def test_completions_triggercharacter(
```

### Comparing `cmake_language_server-0.1.8/PKG-INFO` & `cmake_language_server-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cmake-language-server
-Version: 0.1.8
+Version: 0.1.9
 Summary: CMake LSP Implementation
 Keywords: cmake completion vim lsp
 Author: Regen
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Topic :: Text Editors :: Integrated Development Environments (IDE)
 Classifier: Topic :: Utilities
 Project-URL: Repository, https://github.com/regen100/cmake-language-server
-Requires-Python: <3.12,>=3.7.9
+Requires-Python: <3.13,>=3.8.0
 Requires-Dist: pygls>=1.1.1
 Description-Content-Type: text/markdown
 
 # cmake-language-server
 [![PyPI](https://img.shields.io/pypi/v/cmake-language-server)](https://pypi.org/project/cmake-language-server)
 [![AUR version](https://img.shields.io/aur/version/cmake-language-server)](https://aur.archlinux.org/packages/cmake-language-server/)
 [![GitHub Actions (Tests)](https://github.com/regen100/cmake-language-server/workflows/Tests/badge.svg)](https://github.com/regen100/cmake-language-server/actions)
```

