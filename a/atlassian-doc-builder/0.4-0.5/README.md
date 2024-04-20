# Comparing `tmp/atlassian-doc-builder-0.4.tar.gz` & `tmp/atlassian_doc_builder-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlassian-doc-builder-0.4.tar", last modified: Fri Feb 17 01:09:37 2023, max compression
+gzip compressed data, was "atlassian_doc_builder-0.5.tar", last modified: Sat Apr 20 09:48:40 2024, max compression
```

## Comparing `atlassian-doc-builder-0.4.tar` & `atlassian_doc_builder-0.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 01:09:37.130587 atlassian-doc-builder-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-17 01:09:21.000000 atlassian-doc-builder-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-02-17 01:09:37.130587 atlassian-doc-builder-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-02-17 01:09:21.000000 atlassian-doc-builder-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 01:09:37.126587 atlassian-doc-builder-0.4/atlassian_doc_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-02-17 01:09:21.000000 atlassian-doc-builder-0.4/atlassian_doc_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-02-17 01:09:21.000000 atlassian-doc-builder-0.4/atlassian_doc_builder/adf_content_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    11704 2023-02-17 01:09:21.000000 atlassian-doc-builder-0.4/atlassian_doc_builder/adf_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-02-17 01:09:21.000000 atlassian-doc-builder-0.4/atlassian_doc_builder/adf_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-02-17 01:09:21.000000 atlassian-doc-builder-0.4/atlassian_doc_builder/adf_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 01:09:37.126587 atlassian-doc-builder-0.4/atlassian_doc_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-02-17 01:09:37.000000 atlassian-doc-builder-0.4/atlassian_doc_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-02-17 01:09:37.000000 atlassian-doc-builder-0.4/atlassian_doc_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 01:09:37.000000 atlassian-doc-builder-0.4/atlassian_doc_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-17 01:09:37.000000 atlassian-doc-builder-0.4/atlassian_doc_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-17 01:09:37.000000 atlassian-doc-builder-0.4/atlassian_doc_builder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-02-17 01:09:21.000000 atlassian-doc-builder-0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 01:09:37.130587 atlassian-doc-builder-0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 01:09:37.130587 atlassian-doc-builder-0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-02-17 01:09:21.000000 atlassian-doc-builder-0.4/tests/test_adf_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-02-17 01:09:21.000000 atlassian-doc-builder-0.4/tests/test_content_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-02-17 01:09:21.000000 atlassian-doc-builder-0.4/tests/test_simple_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-02-17 01:09:21.000000 atlassian-doc-builder-0.4/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-02-17 01:09:21.000000 atlassian-doc-builder-0.4/tests/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:48:40.600785 atlassian_doc_builder-0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-20 09:48:35.000000 atlassian_doc_builder-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-20 09:48:40.600785 atlassian_doc_builder-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-20 09:48:35.000000 atlassian_doc_builder-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:48:40.596785 atlassian_doc_builder-0.5/atlassian_doc_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-20 09:48:35.000000 atlassian_doc_builder-0.5/atlassian_doc_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-20 09:48:35.000000 atlassian_doc_builder-0.5/atlassian_doc_builder/adf_content_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-20 09:48:35.000000 atlassian_doc_builder-0.5/atlassian_doc_builder/adf_marks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11752 2024-04-20 09:48:35.000000 atlassian_doc_builder-0.5/atlassian_doc_builder/adf_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-20 09:48:35.000000 atlassian_doc_builder-0.5/atlassian_doc_builder/adf_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-20 09:48:35.000000 atlassian_doc_builder-0.5/atlassian_doc_builder/adf_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:48:40.600785 atlassian_doc_builder-0.5/atlassian_doc_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-20 09:48:40.000000 atlassian_doc_builder-0.5/atlassian_doc_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-20 09:48:40.000000 atlassian_doc_builder-0.5/atlassian_doc_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 09:48:40.000000 atlassian_doc_builder-0.5/atlassian_doc_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 09:48:40.000000 atlassian_doc_builder-0.5/atlassian_doc_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 09:48:40.000000 atlassian_doc_builder-0.5/atlassian_doc_builder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-20 09:48:35.000000 atlassian_doc_builder-0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 09:48:40.600785 atlassian_doc_builder-0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:48:40.600785 atlassian_doc_builder-0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8097 2024-04-20 09:48:35.000000 atlassian_doc_builder-0.5/tests/test_adf_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-20 09:48:35.000000 atlassian_doc_builder-0.5/tests/test_content_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-20 09:48:35.000000 atlassian_doc_builder-0.5/tests/test_simple_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-20 09:48:35.000000 atlassian_doc_builder-0.5/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-20 09:48:35.000000 atlassian_doc_builder-0.5/tests/test_table.py
```

### Comparing `atlassian-doc-builder-0.4/LICENSE` & `atlassian_doc_builder-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `atlassian-doc-builder-0.4/PKG-INFO` & `atlassian_doc_builder-0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlassian-doc-builder
-Version: 0.4
+Version: 0.5
 Summary: Creating Atlassian Document in a programmatic way.
 Author-email: khwong-c <kin.hin.wong.c@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Kin Hin Wong
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,14 +29,15 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: jsonschema
 
 # Atlassian Document Builder
 
 Creating Atlassian Document in a programmatic way.
 
 ## Description
 
@@ -77,18 +78,22 @@
 
 ## Examples
 
 Please refer to [the "examples" directory](examples).
 
 ## Version History
 
+- 0.5
+  - Implement Task, Decision List and related item
+  - Implement Expand (Collapsible Section) and Placeholder
+  - Implement Date and a more marks for text decoration
 - 0.4
   - Implement Table Objects with creation routine
-  - Implement set of Block Nodes with children
-  - Index access to child nodes with `[]`. Multiple index supported. e.g. `doc[1,2,3]`
+  - Implement a set of Block Nodes with children
+  - Index access to child nodes with `[]`. Multiple indexes supported. e.g. `doc[1,2,3]`
 - 0.3
   - Support `ADFText`, `ADFLink` and a bunch of one line classes
   - ADFObject Class Factory for quick Class Development
 - 0.2
   - Add Test Suite
   - Improve ADFObject Implementations
 - 0.1
```

### Comparing `atlassian-doc-builder-0.4/README.md` & `atlassian_doc_builder-0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -41,18 +41,22 @@
 
 ## Examples
 
 Please refer to [the "examples" directory](examples).
 
 ## Version History
 
+- 0.5
+  - Implement Task, Decision List and related item
+  - Implement Expand (Collapsible Section) and Placeholder
+  - Implement Date and a more marks for text decoration
 - 0.4
   - Implement Table Objects with creation routine
-  - Implement set of Block Nodes with children
-  - Index access to child nodes with `[]`. Multiple index supported. e.g. `doc[1,2,3]`
+  - Implement a set of Block Nodes with children
+  - Index access to child nodes with `[]`. Multiple indexes supported. e.g. `doc[1,2,3]`
 - 0.3
   - Support `ADFText`, `ADFLink` and a bunch of one line classes
   - ADFObject Class Factory for quick Class Development
 - 0.2
   - Add Test Suite
   - Improve ADFObject Implementations
 - 0.1
```

### Comparing `atlassian-doc-builder-0.4/atlassian_doc_builder/__init__.py` & `atlassian_doc_builder-0.5/atlassian_doc_builder/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 from .adf_object import ADFObject
 from .adf_object import adf_mark_list, adf_node_list
 from .adf_object import load_adf
 
-from .adf_simple import ADFStrong, ADFEm, ADFStrike, ADFCode, ADFUnderline, ADFHardBreak, ADFRule
-from .adf_simple import ADFText, ADFLink
+from .adf_simple import ADFHardBreak, ADFRule
+from .adf_simple import ADFText, ADFDate, ADFPlaceholder
+from .adf_simple import ADFStatus
 
 from .adf_content_node import ADFParagraph, ADFBlockquote, ADFBulletList, ADFOrderList, ADFListItem
-from .adf_content_node import ADFHeading, ADFCodeBlock, ADFPanel
+from .adf_content_node import ADFHeading, ADFCodeBlock, ADFPanel, ADFExpand, ADFTaskList, ADFTaskItem
+from .adf_content_node import ADFDecisionList, ADFDecisionItem
 from .adf_content_node import ADFDoc
 
 from .adf_table import ADFTable, ADFTableRow, ADFTableCell, ADFTableHeader
 
-__all__ = [ADFObject, ADFDoc]
-__all__ += [adf_node_list, adf_mark_list]
-__all__ += [load_adf]
-__all__ += [ADFStrong, ADFEm, ADFStrike, ADFCode, ADFUnderline, ADFHardBreak, ADFRule]
-__all__ += [ADFText, ADFLink]
-__all__ += [ADFParagraph, ADFBlockquote, ADFBulletList, ADFOrderList, ADFListItem]
-__all__ += [ADFHeading, ADFCodeBlock, ADFPanel]
-__all__ += [ADFTable, ADFTableRow, ADFTableCell, ADFTableHeader]
+from .adf_marks import ADFStrong, ADFEm, ADFStrike, ADFCode, ADFUnderline
+from .adf_marks import ADFLink, ADFBreakout
 
 if __name__ == '__main__':
     pass
```

### Comparing `atlassian-doc-builder-0.4/atlassian_doc_builder/adf_content_node.py` & `atlassian_doc_builder-0.5/atlassian_doc_builder/adf_simple.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,96 +1,90 @@
-from copy import deepcopy
-from .adf_object import adf_schema, ADFObject
+from datetime import datetime
 
-import jsonschema
+from .adf_object import ADFObject
 
-
-class ADFContentObject(ADFObject):
-    def __getitem__(self, idx):
-        if type(idx) is int:
-            return self.local_info['content'][idx]
-        levels, cur_obj = list(idx), self.local_info['content']
-        while levels:
-            cur_idx = levels.pop(0)
-            cur_obj = cur_obj[cur_idx]
-            if not levels:
-                return cur_obj
-            cur_obj = cur_obj.local_info['content']
-
-    def __len__(self):
-        return len(self.local_info['content'])
-
-    def __iter__(self):
-        return self.local_info['content'].__iter__()
-
-
-ADFParagraph, ADFBlockquote, ADFBulletList, ADFOrderList, ADFListItem = tuple(
-    ADFContentObject.node_class_factory(node_type)
-    for node_type in (
-        'paragraph', 'blockquote',
-        'bulletList', 'orderedList', 'listItem',
-    )
+# Node Type with no inputs
+ADFHardBreak, ADFRule = tuple(
+    ADFObject.node_class_factory(node_type)
+    for node_type in ('hardBreak', 'rule',)
 )
 
 
-class ADFDoc(ADFContentObject.node_class_factory('doc')):
-    def __init__(self, chain_mode=True, **kwargs):
-        super(ADFDoc, self).__init__(chain_mode=chain_mode, **kwargs)
-        self.local_info['version'] = 1
-
-    def validate(self):
-        """
-        Validate the output object with the ADF Schema. Raise Exception when validation fails.
-        :return: Rendered result
-        """
-        render_result = self.render()
-        jsonschema.validate(render_result, adf_schema())
-        return render_result
-
-
-class ADFHeading(ADFContentObject.node_class_factory('heading')):
-    def __init__(self, level=None, chain_mode=True, **kwargs):
-        new_attrs = {'level': level} \
-            if level is not None else deepcopy(kwargs.get('attrs', {}))
+class ADFText(ADFObject.node_class_factory('text')):
+    def __init__(self, text=None, chain_mode=True, **kwargs):
+        if not text and 'text' not in kwargs:
+            raise ValueError('Text cannot be empty.')
+        super(ADFText, self).__init__(text=text, chain_mode=chain_mode, **kwargs)
+
+    @property
+    def text(self):
+        return self.local_info['text']
+
+    @text.setter
+    def text(self, value):
+        self.assign_info('text', value)
+
+
+class ADFDate(ADFObject.node_class_factory('date')):
+    def __init__(self, timestamp=None, chain_mode=True, **kwargs):
         new_kwargs = {k: v for k, v in kwargs.items() if k != 'attrs'}
-        super(ADFHeading, self).__init__(chain_mode=chain_mode, attrs=new_attrs, **new_kwargs)
+        super(ADFDate, self).__init__(chain_mode=chain_mode, **new_kwargs)
+        self.timestamp = int(timestamp) if timestamp is not None else \
+            int(kwargs.get('attrs', {}).get('timestamp', (datetime.now().timestamp())))
 
     @property
-    def level(self):
-        return self.local_info['attrs']['level']
+    def timestamp(self):
+        return int(self.local_info['attrs'].get('timestamp')) // 1000
 
-    @level.setter
-    def level(self, value):
-        self.local_info['attrs']['level'] = value
+    @timestamp.setter
+    def timestamp(self, value):
+        if isinstance(value, str):
+            if len(value) != 13:  # len(1676596381123), Looks like in ms format
+                value = f"{value}000"[:13]  # Multiply by 1000 to turn this in ms.
+        else:
+            value = int(value)
+            if value <= 9999999999:  # Looks like in sec format, which have 10 digits or less
+                value *= 1000
+            value = str(value)
+        self.assign_info('attrs', timestamp=value)
 
 
-class ADFCodeBlock(ADFContentObject.node_class_factory('codeBlock')):
-    def __init__(self, language=None, chain_mode=True, **kwargs):
-        new_attrs = {'language': language} \
-            if language is not None else deepcopy(kwargs.get('attrs', {}))
+class ADFPlaceholder(ADFObject.node_class_factory('placeholder')):
+    def __init__(self, text=None, chain_mode=True, **kwargs):
         new_kwargs = {k: v for k, v in kwargs.items() if k != 'attrs'}
-        super(ADFCodeBlock, self).__init__(chain_mode=chain_mode, attrs=new_attrs, **new_kwargs)
+        super(ADFPlaceholder, self).__init__(chain_mode=chain_mode, **new_kwargs)
+        self.text = text if text is not None else \
+            kwargs.get('attrs', {}).get('text', '')
 
     @property
-    def language(self):
-        return self.local_info['attrs']['language']
+    def text(self):
+        return self.local_info['attrs'].get('text')
 
-    @language.setter
-    def language(self, value):
-        self.local_info['attrs']['language'] = value
+    @text.setter
+    def text(self, value):
+        self.assign_info('attrs', text=value)
 
 
-class ADFPanel(ADFContentObject.node_class_factory('panel')):
-    def __init__(self, panel_type=None, chain_mode=True, **kwargs):
-        new_attrs = {'panelType': panel_type} \
-            if panel_type is not None else deepcopy(kwargs.get('attrs', {}))
+class ADFStatus(ADFObject.node_class_factory('status')):
+    def __init__(self, text=None, color=None, chain_mode=True, **kwargs):
         new_kwargs = {k: v for k, v in kwargs.items() if k != 'attrs'}
-        super(ADFPanel, self).__init__(chain_mode=chain_mode, attrs=new_attrs, **new_kwargs)
+        super(ADFPlaceholder, self).__init__(chain_mode=chain_mode, **new_kwargs)
+        self.text = text if text is not None else \
+            kwargs.get('attrs', {}).get('text', '')
+        self.color = color if color is not None else \
+            kwargs.get('attrs', {}).get('color', 'neutral')
 
     @property
-    def panel_type(self):
-        return self.local_info['attrs']['panelType']
+    def text(self):
+        return self.local_info['attrs'].get('text')
 
-    @panel_type.setter
-    def panel_type(self, value):
-        self.local_info['attrs']['panelType'] = value
+    @text.setter
+    def text(self, value):
+        self.assign_info('attrs', text=value)
+
+    @property
+    def color(self):
+        return self.local_info['attrs'].get('color')
 
+    @color.setter
+    def color(self, value):
+        self.assign_info('attrs', color=value)
```

### Comparing `atlassian-doc-builder-0.4/atlassian_doc_builder/adf_object.py` & `atlassian_doc_builder-0.5/atlassian_doc_builder/adf_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,23 +32,23 @@
     }
 
 
 @cache
 def adf_mark_list():
     return _decode_schema_with_filter(
         adf_schema(),
-        lambda key, value: 'mark' in key[-4:]
+        lambda key, value: 'mark' in key[-4:] and value.get('type') == 'object'
     )
 
 
 @cache
 def adf_node_list():
     return _decode_schema_with_filter(
         adf_schema(),
-        lambda key, value: 'node' in key[-4:] and 'type' in value
+        lambda key, value: 'node' in key[-4:] and value.get('type') == 'object'
     )
 
 
 class ADFObject(object):
     PATTERN_EXP, PATTERN_VAR = re.compile(r'\{[^}]+\}'), re.compile('[0-9a-zA-Z_]+')
     node_class_registry, node_class_attr_name = {}, '__adf_type__'
```

### Comparing `atlassian-doc-builder-0.4/atlassian_doc_builder/adf_table.py` & `atlassian_doc_builder-0.5/atlassian_doc_builder/adf_table.py`

 * *Files identical despite different names*

### Comparing `atlassian-doc-builder-0.4/atlassian_doc_builder.egg-info/PKG-INFO` & `atlassian_doc_builder-0.5/atlassian_doc_builder.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlassian-doc-builder
-Version: 0.4
+Version: 0.5
 Summary: Creating Atlassian Document in a programmatic way.
 Author-email: khwong-c <kin.hin.wong.c@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Kin Hin Wong
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,14 +29,15 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: jsonschema
 
 # Atlassian Document Builder
 
 Creating Atlassian Document in a programmatic way.
 
 ## Description
 
@@ -77,18 +78,22 @@
 
 ## Examples
 
 Please refer to [the "examples" directory](examples).
 
 ## Version History
 
+- 0.5
+  - Implement Task, Decision List and related item
+  - Implement Expand (Collapsible Section) and Placeholder
+  - Implement Date and a more marks for text decoration
 - 0.4
   - Implement Table Objects with creation routine
-  - Implement set of Block Nodes with children
-  - Index access to child nodes with `[]`. Multiple index supported. e.g. `doc[1,2,3]`
+  - Implement a set of Block Nodes with children
+  - Index access to child nodes with `[]`. Multiple indexes supported. e.g. `doc[1,2,3]`
 - 0.3
   - Support `ADFText`, `ADFLink` and a bunch of one line classes
   - ADFObject Class Factory for quick Class Development
 - 0.2
   - Add Test Suite
   - Improve ADFObject Implementations
 - 0.1
```

### Comparing `atlassian-doc-builder-0.4/atlassian_doc_builder.egg-info/SOURCES.txt` & `atlassian_doc_builder-0.5/atlassian_doc_builder.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 atlassian_doc_builder/__init__.py
 atlassian_doc_builder/adf_content_node.py
+atlassian_doc_builder/adf_marks.py
 atlassian_doc_builder/adf_object.py
 atlassian_doc_builder/adf_simple.py
 atlassian_doc_builder/adf_table.py
 atlassian_doc_builder.egg-info/PKG-INFO
 atlassian_doc_builder.egg-info/SOURCES.txt
 atlassian_doc_builder.egg-info/dependency_links.txt
 atlassian_doc_builder.egg-info/requires.txt
```

### Comparing `atlassian-doc-builder-0.4/pyproject.toml` & `atlassian_doc_builder-0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "atlassian-doc-builder"
-version = "0.4"
+version = "0.5"
 description = "Creating Atlassian Document in a programmatic way."
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [{ name = "khwong-c", email = "kin.hin.wong.c@gmail.com" }]
 license = { file = "LICENSE" }
 
 classifiers = [
```

### Comparing `atlassian-doc-builder-0.4/tests/test_adf_object.py` & `atlassian_doc_builder-0.5/tests/test_adf_object.py`

 * *Files identical despite different names*

### Comparing `atlassian-doc-builder-0.4/tests/test_smoke.py` & `atlassian_doc_builder-0.5/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `atlassian-doc-builder-0.4/tests/test_table.py` & `atlassian_doc_builder-0.5/tests/test_table.py`

 * *Files identical despite different names*

