# Comparing `tmp/function2widgets-0.6.8.tar.gz` & `tmp/function2widgets-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function2widgets-0.6.8.tar", max compression
+gzip compressed data, was "function2widgets-0.6.9.tar", max compression
```

## Comparing `function2widgets-0.6.8.tar` & `function2widgets-0.6.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0        0 2024-02-26 14:06:46.014790 function2widgets-0.6.8/function2widgets/__init__.py
--rw-r--r--   0        0        0     2999 2024-04-06 12:13:58.866108 function2widgets-0.6.8/function2widgets/common.py
--rw-r--r--   0        0        0     3278 2024-03-31 08:24:42.424892 function2widgets-0.6.8/function2widgets/factory.py
--rw-r--r--   0        0        0     4810 2024-03-31 08:24:42.425891 function2widgets-0.6.8/function2widgets/info.py
--rw-r--r--   0        0        0        2 2024-03-31 08:24:42.425891 function2widgets-0.6.8/function2widgets/parser/__init__.py
--rw-r--r--   0        0        0     2751 2024-03-31 08:24:42.426892 function2widgets-0.6.8/function2widgets/parser/docstr_parser.py
--rw-r--r--   0        0        0     6537 2024-04-06 12:13:58.867110 function2widgets-0.6.8/function2widgets/parser/function_parser.py
--rw-r--r--   0        0        0     3068 2024-04-06 12:13:58.867110 function2widgets-0.6.8/function2widgets/parser/parameter_parser.py
--rw-r--r--   0        0        0     1670 2024-03-31 08:24:42.428417 function2widgets-0.6.8/function2widgets/parser/widgetconfigs_parser.py
--rw-r--r--   0        0        0     4498 2024-04-06 12:13:58.867110 function2widgets-0.6.8/function2widgets/widget.py
--rw-r--r--   0        0        0       27 2024-03-31 08:24:42.430443 function2widgets-0.6.8/function2widgets/widgets/__init__.py
--rw-r--r--   0        0        0     5853 2024-04-05 11:35:06.039590 function2widgets-0.6.8/function2widgets/widgets/_sourcecodeedit.py
--rw-r--r--   0        0        0     1930 2024-04-02 10:46:00.405726 function2widgets-0.6.8/function2widgets/widgets/allwidgets.py
--rw-r--r--   0        0        0     9123 2024-04-06 12:13:58.867110 function2widgets-0.6.8/function2widgets/widgets/base.py
--rw-r--r--   0        0        0      263 2024-03-31 08:24:42.433443 function2widgets-0.6.8/function2widgets/widgets/editor/__init__.py
--rw-r--r--   0        0        0     6067 2024-04-06 12:13:58.868617 function2widgets-0.6.8/function2widgets/widgets/editor/base.py
--rw-r--r--   0        0        0     2030 2024-04-06 12:13:58.868617 function2widgets-0.6.8/function2widgets/widgets/editor/codeeditor.py
--rw-r--r--   0        0        0     1170 2024-04-06 12:13:58.869627 function2widgets-0.6.8/function2widgets/widgets/editor/dicteditor.py
--rw-r--r--   0        0        0     4660 2024-04-06 12:13:58.869627 function2widgets-0.6.8/function2widgets/widgets/editor/jsoneditor.py
--rw-r--r--   0        0        0     1246 2024-04-06 12:13:58.869627 function2widgets-0.6.8/function2widgets/widgets/editor/listeditor.py
--rw-r--r--   0        0        0     1627 2024-04-06 12:13:58.870629 function2widgets-0.6.8/function2widgets/widgets/editor/tupleeditor.py
--rw-r--r--   0        0        0      153 2024-03-31 08:24:42.439428 function2widgets-0.6.8/function2widgets/widgets/lineedit/__init__.py
--rw-r--r--   0        0        0     2440 2024-04-06 12:13:58.870629 function2widgets-0.6.8/function2widgets/widgets/lineedit/floatedit.py
--rw-r--r--   0        0        0     2008 2024-04-06 12:13:58.870629 function2widgets-0.6.8/function2widgets/widgets/lineedit/intedit.py
--rw-r--r--   0        0        0     3137 2024-04-06 12:13:58.871627 function2widgets-0.6.8/function2widgets/widgets/lineedit/stredit.py
--rw-r--r--   0        0        0      150 2024-04-01 15:50:26.686578 function2widgets-0.6.8/function2widgets/widgets/misc/__init__.py
--rw-r--r--   0        0        0       22 2024-03-31 08:24:42.442430 function2widgets-0.6.8/function2widgets/widgets/misc/coloredit.py
--rw-r--r--   0        0        0     3528 2024-04-06 12:13:58.871627 function2widgets-0.6.8/function2widgets/widgets/misc/dateedit.py
--rw-r--r--   0        0        0     4076 2024-04-06 12:13:58.872627 function2widgets-0.6.8/function2widgets/widgets/misc/datetimeedit.py
--rw-r--r--   0        0        0     3409 2024-04-06 12:13:58.872627 function2widgets-0.6.8/function2widgets/widgets/misc/timeedit.py
--rw-r--r--   0        0        0      178 2024-03-31 08:24:42.444428 function2widgets-0.6.8/function2widgets/widgets/numberinput/__init__.py
--rw-r--r--   0        0        0     4699 2024-04-06 12:13:58.872627 function2widgets-0.6.8/function2widgets/widgets/numberinput/dial.py
--rw-r--r--   0        0        0     3132 2024-04-06 12:13:58.873629 function2widgets-0.6.8/function2widgets/widgets/numberinput/floatspin.py
--rw-r--r--   0        0        0     2794 2024-04-06 12:13:58.873629 function2widgets-0.6.8/function2widgets/widgets/numberinput/intspin.py
--rw-r--r--   0        0        0     5168 2024-04-06 12:13:58.873629 function2widgets-0.6.8/function2widgets/widgets/numberinput/slider.py
--rw-r--r--   0        0        0      321 2024-03-31 08:24:42.447443 function2widgets-0.6.8/function2widgets/widgets/pathedit/__init__.py
--rw-r--r--   0        0        0     6228 2024-04-06 12:13:58.874628 function2widgets-0.6.8/function2widgets/widgets/pathedit/base.py
--rw-r--r--   0        0        0      942 2024-04-06 12:13:58.874628 function2widgets-0.6.8/function2widgets/widgets/pathedit/dirpathedit.py
--rw-r--r--   0        0        0     1113 2024-04-06 12:13:58.875628 function2widgets-0.6.8/function2widgets/widgets/pathedit/filepathedit.py
--rw-r--r--   0        0        0      284 2024-03-31 08:24:42.450995 function2widgets-0.6.8/function2widgets/widgets/selectwidget/__init__.py
--rw-r--r--   0        0        0     1954 2024-04-06 12:13:58.875628 function2widgets-0.6.8/function2widgets/widgets/selectwidget/checkbox.py
--rw-r--r--   0        0        0     2829 2024-04-06 12:13:58.875628 function2widgets-0.6.8/function2widgets/widgets/selectwidget/checkbox_group.py
--rw-r--r--   0        0        0     2991 2024-04-06 12:13:58.876627 function2widgets-0.6.8/function2widgets/widgets/selectwidget/combobox.py
--rw-r--r--   0        0        0     2274 2024-04-06 12:13:58.876627 function2widgets-0.6.8/function2widgets/widgets/selectwidget/combobox_edit.py
--rw-r--r--   0        0        0     3575 2024-04-06 12:13:58.876627 function2widgets-0.6.8/function2widgets/widgets/selectwidget/radiobutton_group.py
--rw-r--r--   0        0        0      103 2024-03-31 08:24:42.454980 function2widgets-0.6.8/function2widgets/widgets/textedit/__init__.py
--rw-r--r--   0        0        0     1817 2024-04-06 12:13:58.877629 function2widgets-0.6.8/function2widgets/widgets/textedit/codeedit.py
--rw-r--r--   0        0        0     2362 2024-04-06 12:13:58.877629 function2widgets-0.6.8/function2widgets/widgets/textedit/plaintext.py
--rw-r--r--   0        0        0    35821 2024-03-07 14:10:28.559603 function2widgets-0.6.8/License
--rw-r--r--   0        0        0      714 2024-04-06 12:14:34.601098 function2widgets-0.6.8/pyproject.toml
--rw-r--r--   0        0        0      898 2024-03-31 08:24:42.401374 function2widgets-0.6.8/README.md
--rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 function2widgets-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-26 14:06:46.014790 function2widgets-0.6.9/function2widgets/__init__.py
+-rw-r--r--   0        0        0     2999 2024-04-06 12:13:58.866108 function2widgets-0.6.9/function2widgets/common.py
+-rw-r--r--   0        0        0     3278 2024-03-31 08:24:42.424892 function2widgets-0.6.9/function2widgets/factory.py
+-rw-r--r--   0        0        0     4810 2024-03-31 08:24:42.425891 function2widgets-0.6.9/function2widgets/info.py
+-rw-r--r--   0        0        0        2 2024-03-31 08:24:42.425891 function2widgets-0.6.9/function2widgets/parser/__init__.py
+-rw-r--r--   0        0        0     2751 2024-03-31 08:24:42.426892 function2widgets-0.6.9/function2widgets/parser/docstr_parser.py
+-rw-r--r--   0        0        0     6537 2024-04-06 12:13:58.867110 function2widgets-0.6.9/function2widgets/parser/function_parser.py
+-rw-r--r--   0        0        0     3068 2024-04-06 12:13:58.867110 function2widgets-0.6.9/function2widgets/parser/parameter_parser.py
+-rw-r--r--   0        0        0     1670 2024-03-31 08:24:42.428417 function2widgets-0.6.9/function2widgets/parser/widgetconfigs_parser.py
+-rw-r--r--   0        0        0     4498 2024-04-06 12:13:58.867110 function2widgets-0.6.9/function2widgets/widget.py
+-rw-r--r--   0        0        0       27 2024-03-31 08:24:42.430443 function2widgets-0.6.9/function2widgets/widgets/__init__.py
+-rw-r--r--   0        0        0     5853 2024-04-05 11:35:06.039590 function2widgets-0.6.9/function2widgets/widgets/_sourcecodeedit.py
+-rw-r--r--   0        0        0     1930 2024-04-02 10:46:00.405726 function2widgets-0.6.9/function2widgets/widgets/allwidgets.py
+-rw-r--r--   0        0        0     9036 2024-04-06 14:22:27.701529 function2widgets-0.6.9/function2widgets/widgets/base.py
+-rw-r--r--   0        0        0      263 2024-03-31 08:24:42.433443 function2widgets-0.6.9/function2widgets/widgets/editor/__init__.py
+-rw-r--r--   0        0        0     6067 2024-04-06 12:13:58.868617 function2widgets-0.6.9/function2widgets/widgets/editor/base.py
+-rw-r--r--   0        0        0     2030 2024-04-06 12:13:58.868617 function2widgets-0.6.9/function2widgets/widgets/editor/codeeditor.py
+-rw-r--r--   0        0        0     1170 2024-04-06 12:13:58.869627 function2widgets-0.6.9/function2widgets/widgets/editor/dicteditor.py
+-rw-r--r--   0        0        0     4660 2024-04-06 12:13:58.869627 function2widgets-0.6.9/function2widgets/widgets/editor/jsoneditor.py
+-rw-r--r--   0        0        0     1246 2024-04-06 12:13:58.869627 function2widgets-0.6.9/function2widgets/widgets/editor/listeditor.py
+-rw-r--r--   0        0        0     1627 2024-04-06 12:13:58.870629 function2widgets-0.6.9/function2widgets/widgets/editor/tupleeditor.py
+-rw-r--r--   0        0        0      153 2024-03-31 08:24:42.439428 function2widgets-0.6.9/function2widgets/widgets/lineedit/__init__.py
+-rw-r--r--   0        0        0     2440 2024-04-06 12:13:58.870629 function2widgets-0.6.9/function2widgets/widgets/lineedit/floatedit.py
+-rw-r--r--   0        0        0     2008 2024-04-06 12:13:58.870629 function2widgets-0.6.9/function2widgets/widgets/lineedit/intedit.py
+-rw-r--r--   0        0        0     3137 2024-04-06 12:13:58.871627 function2widgets-0.6.9/function2widgets/widgets/lineedit/stredit.py
+-rw-r--r--   0        0        0      150 2024-04-01 15:50:26.686578 function2widgets-0.6.9/function2widgets/widgets/misc/__init__.py
+-rw-r--r--   0        0        0       22 2024-03-31 08:24:42.442430 function2widgets-0.6.9/function2widgets/widgets/misc/coloredit.py
+-rw-r--r--   0        0        0     3528 2024-04-06 12:13:58.871627 function2widgets-0.6.9/function2widgets/widgets/misc/dateedit.py
+-rw-r--r--   0        0        0     4076 2024-04-06 12:13:58.872627 function2widgets-0.6.9/function2widgets/widgets/misc/datetimeedit.py
+-rw-r--r--   0        0        0     3409 2024-04-06 12:13:58.872627 function2widgets-0.6.9/function2widgets/widgets/misc/timeedit.py
+-rw-r--r--   0        0        0      178 2024-03-31 08:24:42.444428 function2widgets-0.6.9/function2widgets/widgets/numberinput/__init__.py
+-rw-r--r--   0        0        0     4699 2024-04-06 12:13:58.872627 function2widgets-0.6.9/function2widgets/widgets/numberinput/dial.py
+-rw-r--r--   0        0        0     3132 2024-04-06 12:13:58.873629 function2widgets-0.6.9/function2widgets/widgets/numberinput/floatspin.py
+-rw-r--r--   0        0        0     2794 2024-04-06 12:13:58.873629 function2widgets-0.6.9/function2widgets/widgets/numberinput/intspin.py
+-rw-r--r--   0        0        0     5168 2024-04-06 12:13:58.873629 function2widgets-0.6.9/function2widgets/widgets/numberinput/slider.py
+-rw-r--r--   0        0        0      321 2024-03-31 08:24:42.447443 function2widgets-0.6.9/function2widgets/widgets/pathedit/__init__.py
+-rw-r--r--   0        0        0     6228 2024-04-06 12:13:58.874628 function2widgets-0.6.9/function2widgets/widgets/pathedit/base.py
+-rw-r--r--   0        0        0      942 2024-04-06 12:13:58.874628 function2widgets-0.6.9/function2widgets/widgets/pathedit/dirpathedit.py
+-rw-r--r--   0        0        0     1113 2024-04-06 12:13:58.875628 function2widgets-0.6.9/function2widgets/widgets/pathedit/filepathedit.py
+-rw-r--r--   0        0        0      284 2024-03-31 08:24:42.450995 function2widgets-0.6.9/function2widgets/widgets/selectwidget/__init__.py
+-rw-r--r--   0        0        0     1954 2024-04-06 12:13:58.875628 function2widgets-0.6.9/function2widgets/widgets/selectwidget/checkbox.py
+-rw-r--r--   0        0        0     2829 2024-04-06 12:13:58.875628 function2widgets-0.6.9/function2widgets/widgets/selectwidget/checkbox_group.py
+-rw-r--r--   0        0        0     2991 2024-04-06 12:13:58.876627 function2widgets-0.6.9/function2widgets/widgets/selectwidget/combobox.py
+-rw-r--r--   0        0        0     2274 2024-04-06 12:13:58.876627 function2widgets-0.6.9/function2widgets/widgets/selectwidget/combobox_edit.py
+-rw-r--r--   0        0        0     3575 2024-04-06 12:13:58.876627 function2widgets-0.6.9/function2widgets/widgets/selectwidget/radiobutton_group.py
+-rw-r--r--   0        0        0      103 2024-03-31 08:24:42.454980 function2widgets-0.6.9/function2widgets/widgets/textedit/__init__.py
+-rw-r--r--   0        0        0     1817 2024-04-06 12:13:58.877629 function2widgets-0.6.9/function2widgets/widgets/textedit/codeedit.py
+-rw-r--r--   0        0        0     2362 2024-04-06 12:13:58.877629 function2widgets-0.6.9/function2widgets/widgets/textedit/plaintext.py
+-rw-r--r--   0        0        0    35821 2024-03-07 14:10:28.559603 function2widgets-0.6.9/License
+-rw-r--r--   0        0        0      714 2024-04-06 14:22:43.281463 function2widgets-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0      898 2024-03-31 08:24:42.401374 function2widgets-0.6.9/README.md
+-rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 function2widgets-0.6.9/PKG-INFO
```

### Comparing `function2widgets-0.6.8/function2widgets/common.py` & `function2widgets-0.6.9/function2widgets/common.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/factory.py` & `function2widgets-0.6.9/function2widgets/factory.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/info.py` & `function2widgets-0.6.9/function2widgets/info.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/parser/docstr_parser.py` & `function2widgets-0.6.9/function2widgets/parser/docstr_parser.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/parser/function_parser.py` & `function2widgets-0.6.9/function2widgets/parser/function_parser.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/parser/parameter_parser.py` & `function2widgets-0.6.9/function2widgets/parser/parameter_parser.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/parser/widgetconfigs_parser.py` & `function2widgets-0.6.9/function2widgets/parser/widgetconfigs_parser.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widget.py` & `function2widgets-0.6.9/function2widgets/widget.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/_sourcecodeedit.py` & `function2widgets-0.6.9/function2widgets/widgets/_sourcecodeedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/allwidgets.py` & `function2widgets-0.6.9/function2widgets/widgets/allwidgets.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/base.py` & `function2widgets-0.6.9/function2widgets/widgets/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,27 +198,23 @@
         self._label_widget.setObjectName(cls.OBJ_ID_LABEL_WIDGET)
         self._description_widget.setObjectName(cls.OBJ_ID_DESCRIPTION_WIDGET)
         self._center_widget.setObjectName(cls.OBJ_ID_CENTER_WIDGET)
         self._default_widget.setObjectName(cls.OBJ_ID_DEFAULT_VALUE_WIDGET)
 
         self._layout.setContentsMargins(0, 0, 0, 0)
 
-        description_pos = (
-            self._args.description_position or self.DEFAULT_DESCRIPTION_POS
-        )
-
         self._layout.addWidget(self._label_widget)
 
-        if description_pos == POS_TOP:
+        if self._args.description_position == POS_TOP:
             self._layout.addWidget(self._description_widget)
 
         self._layout.addWidget(self._center_widget)
         self._layout.addWidget(self._default_widget)
 
-        if description_pos != POS_TOP:
+        if self._args.description_position != POS_TOP:
             self._layout.addWidget(self._description_widget)
 
         if self._args.separate_line:
             line = self._create_separate_line()
             self._layout.addWidget(line)
         # spacer = QSpacerItem(
         #     0, 0, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding
```

### Comparing `function2widgets-0.6.8/function2widgets/widgets/editor/base.py` & `function2widgets-0.6.9/function2widgets/widgets/editor/base.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/editor/codeeditor.py` & `function2widgets-0.6.9/function2widgets/widgets/editor/codeeditor.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/editor/dicteditor.py` & `function2widgets-0.6.9/function2widgets/widgets/editor/dicteditor.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/editor/jsoneditor.py` & `function2widgets-0.6.9/function2widgets/widgets/editor/jsoneditor.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/editor/listeditor.py` & `function2widgets-0.6.9/function2widgets/widgets/editor/listeditor.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/editor/tupleeditor.py` & `function2widgets-0.6.9/function2widgets/widgets/editor/tupleeditor.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/lineedit/floatedit.py` & `function2widgets-0.6.9/function2widgets/widgets/lineedit/floatedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/lineedit/intedit.py` & `function2widgets-0.6.9/function2widgets/widgets/lineedit/intedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/lineedit/stredit.py` & `function2widgets-0.6.9/function2widgets/widgets/lineedit/stredit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/misc/dateedit.py` & `function2widgets-0.6.9/function2widgets/widgets/misc/dateedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/misc/datetimeedit.py` & `function2widgets-0.6.9/function2widgets/widgets/misc/datetimeedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/misc/timeedit.py` & `function2widgets-0.6.9/function2widgets/widgets/misc/timeedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/numberinput/dial.py` & `function2widgets-0.6.9/function2widgets/widgets/numberinput/dial.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/numberinput/floatspin.py` & `function2widgets-0.6.9/function2widgets/widgets/numberinput/floatspin.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/numberinput/intspin.py` & `function2widgets-0.6.9/function2widgets/widgets/numberinput/intspin.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/numberinput/slider.py` & `function2widgets-0.6.9/function2widgets/widgets/numberinput/slider.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/pathedit/base.py` & `function2widgets-0.6.9/function2widgets/widgets/pathedit/base.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/pathedit/dirpathedit.py` & `function2widgets-0.6.9/function2widgets/widgets/pathedit/dirpathedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/pathedit/filepathedit.py` & `function2widgets-0.6.9/function2widgets/widgets/pathedit/filepathedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/selectwidget/checkbox.py` & `function2widgets-0.6.9/function2widgets/widgets/selectwidget/checkbox.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/selectwidget/checkbox_group.py` & `function2widgets-0.6.9/function2widgets/widgets/selectwidget/checkbox_group.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/selectwidget/combobox.py` & `function2widgets-0.6.9/function2widgets/widgets/selectwidget/combobox.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/selectwidget/combobox_edit.py` & `function2widgets-0.6.9/function2widgets/widgets/selectwidget/combobox_edit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/selectwidget/radiobutton_group.py` & `function2widgets-0.6.9/function2widgets/widgets/selectwidget/radiobutton_group.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/textedit/codeedit.py` & `function2widgets-0.6.9/function2widgets/widgets/textedit/codeedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/function2widgets/widgets/textedit/plaintext.py` & `function2widgets-0.6.9/function2widgets/widgets/textedit/plaintext.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/License` & `function2widgets-0.6.9/License`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/pyproject.toml` & `function2widgets-0.6.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "function2widgets"
-version = "0.6.8"
+version = "0.6.9"
 description = ""
 authors = ["zimolab <zimolab@aliyun.com>"]
 readme = "README.md"
 license = "GPL-3.0"
 packages = [
     {include="function2widgets"}
 ]
```

### Comparing `function2widgets-0.6.8/README.md` & `function2widgets-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.8/PKG-INFO` & `function2widgets-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function2widgets
-Version: 0.6.8
+Version: 0.6.9
 Summary: 
 Home-page: https://github.com/zimolab/function2widgets
 License: GPL-3.0
 Author: zimolab
 Author-email: zimolab@aliyun.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

