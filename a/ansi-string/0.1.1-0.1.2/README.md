# Comparing `tmp/ansi-string-0.1.1.tar.gz` & `tmp/ansi-string-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansi-string-0.1.1.tar", last modified: Sat Apr 20 01:05:34 2024, max compression
+gzip compressed data, was "ansi-string-0.1.2.tar", last modified: Sat Apr 20 03:49:32 2024, max compression
```

## Comparing `ansi-string-0.1.1.tar` & `ansi-string-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:05:34.326753 ansi-string-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 01:05:23.000000 ansi-string-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-20 01:05:23.000000 ansi-string-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-20 01:05:34.326753 ansi-string-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-20 01:05:23.000000 ansi-string-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-20 01:05:23.000000 ansi-string-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-20 01:05:34.326753 ansi-string-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-20 01:05:23.000000 ansi-string-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:05:34.326753 ansi-string-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:05:34.326753 ansi-string-0.1.1/src/ansi_string/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-20 01:05:23.000000 ansi-string-0.1.1/src/ansi_string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52215 2024-04-20 01:05:23.000000 ansi-string-0.1.1/src/ansi_string/ansi_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:05:34.326753 ansi-string-0.1.1/src/ansi_string.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-20 01:05:34.000000 ansi-string-0.1.1/src/ansi_string.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-20 01:05:34.000000 ansi-string-0.1.1/src/ansi_string.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:05:34.000000 ansi-string-0.1.1/src/ansi_string.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 01:05:34.000000 ansi-string-0.1.1/src/ansi_string.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-20 01:05:34.000000 ansi-string-0.1.1/src/ansi_string.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:49:32.459931 ansi-string-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 03:49:22.000000 ansi-string-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-20 03:49:22.000000 ansi-string-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-20 03:49:32.459931 ansi-string-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-20 03:49:22.000000 ansi-string-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-20 03:49:22.000000 ansi-string-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-20 03:49:32.459931 ansi-string-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-20 03:49:22.000000 ansi-string-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:49:32.459931 ansi-string-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:49:32.459931 ansi-string-0.1.2/src/ansi_string/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-20 03:49:22.000000 ansi-string-0.1.2/src/ansi_string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55019 2024-04-20 03:49:22.000000 ansi-string-0.1.2/src/ansi_string/ansi_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:49:32.459931 ansi-string-0.1.2/src/ansi_string.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-20 03:49:32.000000 ansi-string-0.1.2/src/ansi_string.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-20 03:49:32.000000 ansi-string-0.1.2/src/ansi_string.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 03:49:32.000000 ansi-string-0.1.2/src/ansi_string.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 03:49:32.000000 ansi-string-0.1.2/src/ansi_string.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-20 03:49:32.000000 ansi-string-0.1.2/src/ansi_string.egg-info/top_level.txt
```

### Comparing `ansi-string-0.1.1/LICENSE` & `ansi-string-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansi-string-0.1.1/PKG-INFO` & `ansi-string-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansi-string
-Version: 0.1.1
+Version: 0.1.2
 Summary: ANSI String Formatter in Python for CLI Color and Style Formatting
 Home-page: https://github.com/Tails86/ansi-string
 Author: James Smith
 Author-email: jmsmith86@gmail.com
 Project-URL: Documentation, https://github.com/Tails86/ansi-string
 Project-URL: Bug Reports, https://github.com/Tails86/ansi-string/issues
 Project-URL: Source Code, https://github.com/Tails86/ansi-string
@@ -30,8 +30,8 @@
 
 This is a work in progress.
 
 This code was originally written for [greplica](https://pypi.org/project/greplica/), but I felt it deserved its own, separate library.
 
 ## Examples:
 
-![Examples](https://raw.githubusercontent.com/Tails86/ansi-string/edfa8234f9b408c594c3659585c4e2c6de602cb8/docs/examples.jpg)
+![Examples](https://raw.githubusercontent.com/Tails86/ansi-string/d7d299bf8204ec205b9bee7ed76c25b39f23de5b/docs/examples.jpg)
```

### Comparing `ansi-string-0.1.1/setup.py` & `ansi-string-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `ansi-string-0.1.1/src/ansi_string/ansi_string.py` & `ansi-string-0.1.2/src/ansi_string/ansi_string.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import re
 import copy
 import math
 from enum import Enum, EnumMeta, auto as enum_auto
 import io
 from typing import Any, Union, List
 
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 PACKAGE_NAME = 'ansi-string'
 
 IS_WINDOWS = sys.platform.lower().startswith('win')
 
 if IS_WINDOWS:
     try:
         import ctypes
@@ -778,17 +778,17 @@
 
     Example 2:
     s = AnsiString('This string contains custom formatting', '38;2;175;95;95')
     print(s)
 
     Example 3:
     s = AnsiString('This string contains multiple color settings across different ranges')
-    s.apply_formatting(AnsiFormat.BOLD, 5, 6)
-    s.apply_formatting(AnsiFormat.BG_BLUE, 21, 8)
-    s.apply_formatting([AnsiFormat.FG_ORANGE, AnsiFormat.ITALIC], 21, 14)
+    s.apply_formatting(AnsiFormat.BOLD, 5, 11)
+    s.apply_formatting(AnsiFormat.BG_BLUE, 21, 29)
+    s.apply_formatting([AnsiFormat.FG_ORANGE, AnsiFormat.ITALIC], 21, 35)
     print(s)
 
     Example 4:
     s = AnsiString('This string will be formatted bold and red')
     print('{::01;31}'.format(s))
 
     Example 5:
@@ -822,24 +822,87 @@
             if not isinstance(setting_or_settings, list):
                 settings = [setting_or_settings]
             else:
                 settings = setting_or_settings
 
             for i, item in enumerate(settings):
                 if isinstance(item, str):
-                    # Use string verbatim
-                    pass
+                    settings[i] = __class__._scrub_ansi_format_string(item)
                 elif hasattr(item, 'value') and isinstance(item.value, str):
                     # Likely an enumeration - use the value
                     settings[i] = item.value
                 else:
                     raise TypeError('Unsupported type for setting_or_settings: {}'.format(type(setting_or_settings)))
 
             self._str = ';'.join(settings)
 
+        @staticmethod
+        def _parse_rgb_string(s:str):
+            component_dict = {
+                'ul_': ColorComponentType.UNDERLINE,
+                'bg_': ColorComponentType.BACKGROUND,
+                'fg_': ColorComponentType.FOREGROUND
+            }
+
+            # rgb(), fg_rgb(), bg_rgb(), or ul_rgb() with 3 distinct values as decimal or hex
+            match = re.search(r'^((?:fg_)?|(?:bg_)|(?:ul_))rgb\(\[?\s*(0x)?([0-9a-fA-F]+)\s*,\s*(0x)?([0-9a-fA-F]+)\s*,\s*(0x)?([0-9a-fA-F]+)\s*\]?\)$', s)
+            if match:
+                try:
+                    r = int(match.group(3), 16 if match.group(2) else 10)
+                    g = int(match.group(5), 16 if match.group(4) else 10)
+                    b = int(match.group(7), 16 if match.group(6) else 10)
+                except ValueError:
+                    raise ValueError('Invalid rgb value(s)')
+                return AnsiFormat.rgb(r, g, b, component_dict.get(match.group(1), ColorComponentType.FOREGROUND))
+
+            # rgb(), fg_rgb(), bg_rgb(), or ul_rgb() with 1 value as decimal or hex
+            match = re.search(r'^((?:fg_)?|(?:bg_)|(?:ul_))rgb\(\[?\s*(0x)?([0-9a-fA-F]+)\s*\]?\)$', s)
+            if match:
+                try:
+                    rgb = int(match.group(3), 16 if match.group(2) else 10)
+                except ValueError:
+                    raise ValueError('Invalid rgb value')
+                return AnsiFormat.rgb(rgb, component=component_dict.get(match.group(1), ColorComponentType.FOREGROUND))
+            return None
+
+        @staticmethod
+        def _scrub_ansi_format_string(ansi_format):
+            if ansi_format.startswith("["):
+                # Use the rest of the string as-is for settings
+                return ansi_format[1:]
+            else:
+                # The format string contains names within AnsiFormat or integers, separated by semicolon
+                formats = ansi_format.split(';')
+                format_settings_strs = []
+                for format in formats:
+                    ansi_fmt_enum = None
+                    try:
+                        ansi_fmt_enum = AnsiFormat[format.upper()]
+                    except KeyError:
+                        pass
+                    else:
+                        format_settings_strs.append(ansi_fmt_enum.value)
+
+                    if ansi_fmt_enum is None:
+                        rgb_format = __class__._parse_rgb_string(format)
+                        if not rgb_format:
+                            try:
+                                _ = int(format)
+                            except ValueError:
+                                raise ValueError(
+                                    'AnsiString.__format__ failed to parse format ({}); invalid name: {}'
+                                    .format(ansi_format, format)
+                                )
+                            else:
+                                # Value is an integer - use the format verbatim
+                                format_settings_strs.append(format)
+                        else:
+                            format_settings_strs.append(rgb_format)
+                return ';'.join(format_settings_strs)
+
         def __str__(self):
             return self._str
 
     def __init__(self, s:str='', setting_or_settings:Union[List[str], str, List[AnsiFormat], AnsiFormat]=None):
         self._s = s
         # Key is the string index to make a color change at
         # Each value element is a list of 2 lists
@@ -881,76 +944,63 @@
 
     def _insert_settings(self, idx:int, apply:bool, settings:Settings, topmost:bool=True):
         __class__._insert_settings_to_dict(self._color_settings, idx, apply, settings, topmost)
 
     def apply_formatting(
             self,
             setting_or_settings:Union[List[str], str, List[AnsiFormat], AnsiFormat],
-            start_idx_or_slice:Union[int, slice]=0,
-            length=None,
+            start:int=0,
+            end:Union[int,None]=None,
             topmost=True
     ):
         '''
         Sets the formatting for a given range of characters.
         Inputs: setting_or_settings - Can either be a single item or list of items;
                                       each item can either be a string or AnsiFormat type
-                start_idx_or_slice - If int, the string start index where setting(s) are to be applied
-                                     If slice, the slice specifying where to apply settings (length must not be set)
-                length - Number of characters to apply settings or None to apply until end of string
+                start - The string start index where setting(s) are to be applied
+                end - The string index where the setting(s) should be removed
                 topmost - When true, this setting is placed at the end of the set for the given
                         start_index meaning it is applied last; when false, setting is applied first
 
         Note: The desired effect may not be achieved if the same setting is applied over an
               overlapping range of characters.
         '''
-        if not setting_or_settings:
+        if not setting_or_settings or start >= len(self._s):
             # Ignore - nothing to apply
             return
 
-        settings = __class__.Settings(setting_or_settings)
-
-        if isinstance(start_idx_or_slice, slice):
-            if length is not None:
-                raise ValueError('length cannot be set when start_idx_or_slice is a slice')
-            elif start_idx_or_slice.step is not None and start_idx_or_slice.step != 1:
-                raise ValueError('Step other than 1 not supported')
-
-            if start_idx_or_slice.start is None:
-                start_idx = 0
-            else:
-                start_idx = start_idx_or_slice.start
-
-            if start_idx_or_slice.stop is not None:
-                length = start_idx_or_slice.stop - start_idx
+        if end is None:
+            length = None
         else:
-            start_idx = start_idx_or_slice
+            length = end - start
+            if length <= 0:
+                # Ignore - nothing to apply
+                return
 
-        if length is not None and length <= 0:
-            # Ignore - nothing to apply
-            return
+        settings = __class__.Settings(setting_or_settings)
 
         # Apply settings
-        self._insert_settings(start_idx, True, settings, topmost)
+        self._insert_settings(start, True, settings, topmost)
 
         if length is not None:
             # Remove settings
-            self._insert_settings(start_idx + length, False, settings, topmost)
+            self._insert_settings(start + length, False, settings, topmost)
 
     def apply_formatting_for_match(
             self,
             setting_or_settings:Union[List[str], str, List[AnsiFormat], AnsiFormat],
             match_object,
             group:int=0
     ):
         '''
         Apply formatting using a match object generated from re
         '''
         s = match_object.start(group)
         e = match_object.end(group)
-        self.apply_formatting(setting_or_settings, s, e - s)
+        self.apply_formatting(setting_or_settings, s, e)
 
     def clear_formatting(self):
         '''
         Clears all internal formatting.
         '''
         self._color_settings = {}
 
@@ -1035,43 +1085,14 @@
         Helper method so I can assign and check in the same "if" statement
         '''
         match = re.search(expr, string)
         if match:
             result.append(match)
         return match
 
-    @staticmethod
-    def _parse_rgb_string(s:str):
-        component_dict = {
-            'ul_': ColorComponentType.UNDERLINE,
-            'bg_': ColorComponentType.BACKGROUND,
-            'fg_': ColorComponentType.FOREGROUND
-        }
-
-        # rgb(), fg_rgb(), bg_rgb(), or ul_rgb() with 3 distinct values as decimal or hex
-        match = re.search(r'^((?:fg_)?|(?:bg_)|(?:ul_))rgb\(\s*(0x)?([0-9a-fA-F]+)\s*,\s*(0x)?([0-9a-fA-F]+)\s*,\s*(0x)?([0-9a-fA-F]+)\s*\)$', s)
-        if match:
-            try:
-                r = int(match.group(3), 16 if match.group(2) else 10)
-                g = int(match.group(5), 16 if match.group(4) else 10)
-                b = int(match.group(7), 16 if match.group(6) else 10)
-            except ValueError:
-                raise ValueError('Invalid rgb value(s)')
-            return AnsiFormat.rgb(r, g, b, component_dict.get(match.group(1), ColorComponentType.FOREGROUND))
-
-        # rgb(), fg_rgb(), bg_rgb(), or ul_rgb() with 1 value as decimal or hex
-        match = re.search(r'^((?:fg_)?|(?:bg_)|(?:ul_))rgb\(\s*(0x)?([0-9a-fA-F]+)\s*\)$', s)
-        if match:
-            try:
-                rgb = int(match.group(3), 16 if match.group(2) else 10)
-            except ValueError:
-                raise ValueError('Invalid rgb value')
-            return AnsiFormat.rgb(rgb, component=component_dict.get(match.group(1), ColorComponentType.FOREGROUND))
-        return None
-
     def __format__(self, __format_spec:str) -> str:
         '''
         Returns an ANSI format string with both internal and given formatting spec set.
         __format_spec: must be in the format "[string_format][:ansi_format]" where string_format is the standard
                        string format specifier and ansi_format contains 0 or more ansi directives separated by
                        semicolons (;)
                        ex: ">10:bold;fg_red" to make output right justify with width of 10, bold and red formatting
@@ -1138,47 +1159,15 @@
                 raise ValueError('Sign not allowed in string format specifier')
             elif __class__._re_search(r'^[<>\^]?[ ]?[0-9]*$', string_format, result):
                 raise ValueError('Space not allowed in string format specifier')
             else:
                 raise ValueError('Invalid format specifier')
 
         if ansi_format:
-            if ansi_format.startswith("["):
-                # Use the rest of the string as-is for settings
-                format_settings = __class__.Settings(ansi_format[1:])
-            else:
-                # The format string contains names within AnsiFormat or integers, separated by semicolon
-                formats = ansi_format.split(';')
-                format_settings_strs = []
-                for format in formats:
-                    ansi_fmt_enum = None
-                    try:
-                        ansi_fmt_enum = AnsiFormat[format.upper()]
-                    except KeyError:
-                        pass
-                    else:
-                        format_settings_strs.append(ansi_fmt_enum.value)
-
-                    if ansi_fmt_enum is None:
-                        rgb_format = __class__._parse_rgb_string(format)
-                        if not rgb_format:
-                            try:
-                                _ = int(format)
-                            except ValueError:
-                                raise ValueError(
-                                    'AnsiString.__format__ failed to parse format ({}); invalid name: {}'
-                                    .format(ansi_format, format)
-                                )
-                            else:
-                                # Value is an integer - use the format verbatim
-                                format_settings_strs.append(format)
-                        else:
-                            format_settings_strs.append(rgb_format)
-                format_settings = __class__.Settings(';'.join(format_settings_strs))
-
+            format_settings =  __class__.Settings(ansi_format)
             __class__._insert_settings_to_dict(settings_dict, 0, True, format_settings, True)
 
         clear_needed = False
         for idx, settings, current_settings in __class__.SettingsIterator(settings_dict):
             if idx >= len(normal_format_str):
                 # Invalid
                 break
@@ -1199,7 +1188,118 @@
         # Final catch up
         out_str += normal_format_str[last_idx:]
         if clear_needed:
             # Clear settings
             out_str += __class__.ANSI_ESCAPE_CLEAR
 
         return out_str
+
+    def capitalize(self):
+        cpy = copy.deepcopy(self)
+        cpy._s = cpy._s.capitalize()
+        return cpy
+
+    def casefold(self):
+        cpy = copy.deepcopy(self)
+        cpy._s = cpy._s.casefold()
+        return cpy
+
+    def center(self, width:int, fillchar:str=' '):
+        cpy = copy.deepcopy(self)
+        num = width - len(cpy._s)
+        if num > 0:
+            left_spaces = math.floor((num) / 2)
+            right_spaces = num - left_spaces
+            cpy._s = fillchar * left_spaces + cpy._s + fillchar * right_spaces
+            # Shift all indices except for the origin
+            __class__._shift_settings_idx(cpy._color_settings, left_spaces, True)
+        return cpy
+
+    def count(self, sub:str, start:int, end:int) -> int:
+        return self._s.count(sub, start, end)
+
+    def encode(self, encoding:str="utf-8", errors:str="strict") -> bytes:
+        return str(self).encode(encoding, errors)
+
+    def endswith(self, suffix:str, start:int=None, end:int=None) -> bool:
+        return self._s.endswith(suffix, start, end)
+
+    def expandtabs(self, tabsize:int=8):
+        cpy = copy.deepcopy(self)
+        cpy._s = cpy._s.expandtabs(tabsize)
+        return cpy
+
+    def find(self, sub:str, start:int=None, end:int=None) -> int:
+        return self._s.find(sub, start, end)
+
+    def index(self, sub:str, start:int=None, end:int=None) -> int:
+        return self._s.index(sub, start, end)
+
+    def isalnum(self) -> bool:
+        return self._s.isalnum()
+
+    def isalpha(self) -> bool:
+        return self._s.isalpha()
+
+    def isascii(self) -> bool:
+        return self._s.isascii()
+
+    def isdecimal(self) -> bool:
+        return self._s.isdecimal()
+
+    def isdigit(self) -> bool:
+        return self._s.isdigit()
+
+    def isidentifier(self) -> bool:
+        return self._s.isidentifier()
+
+    def islower(self) -> bool:
+        return self._s.islower()
+
+    def isnumeric(self) -> bool:
+        return self._s.isnumeric()
+
+    def isprintable(self) -> bool:
+        return self._s.isprintable()
+
+    def isspace(self) -> bool:
+        return self._s.isspace()
+
+    def istitle(self) -> bool:
+        return self._s.istitle()
+
+    def isupper(self) -> bool:
+        return self._s.isupper()
+
+    def __add__(self, value):
+        cpy = copy.deepcopy(self)
+        cpy += value
+        return cpy
+
+    def __iadd__(self, value):
+        if isinstance(value, str):
+            self._s += value
+        elif isinstance(value, AnsiString):
+            settings_cpy = copy.deepcopy(value._color_settings)
+            __class__._shift_settings_idx(settings_cpy, len(self._s), False)
+            self._s += value._s
+            for key, value in settings_cpy.values():
+                self._color_settings[key] = value
+        else:
+            raise ValueError(f'value is invalid type: {type(value)}')
+        return self
+
+    @staticmethod
+    def join(*args):
+        if not args:
+            return AnsiString()
+        args = list(args)
+        first_arg = args[0]
+        if isinstance(first_arg, str):
+            joint = AnsiString(first_arg)
+        elif isinstance(first_arg, AnsiString):
+            joint = copy.deepcopy(first_arg)
+        else:
+            raise ValueError(f'value is invalid type: {type(first_arg)}')
+        for arg in args[1:]:
+            joint += arg
+        return joint
```

### Comparing `ansi-string-0.1.1/src/ansi_string.egg-info/PKG-INFO` & `ansi-string-0.1.2/src/ansi_string.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansi-string
-Version: 0.1.1
+Version: 0.1.2
 Summary: ANSI String Formatter in Python for CLI Color and Style Formatting
 Home-page: https://github.com/Tails86/ansi-string
 Author: James Smith
 Author-email: jmsmith86@gmail.com
 Project-URL: Documentation, https://github.com/Tails86/ansi-string
 Project-URL: Bug Reports, https://github.com/Tails86/ansi-string/issues
 Project-URL: Source Code, https://github.com/Tails86/ansi-string
@@ -30,8 +30,8 @@
 
 This is a work in progress.
 
 This code was originally written for [greplica](https://pypi.org/project/greplica/), but I felt it deserved its own, separate library.
 
 ## Examples:
 
-![Examples](https://raw.githubusercontent.com/Tails86/ansi-string/edfa8234f9b408c594c3659585c4e2c6de602cb8/docs/examples.jpg)
+![Examples](https://raw.githubusercontent.com/Tails86/ansi-string/d7d299bf8204ec205b9bee7ed76c25b39f23de5b/docs/examples.jpg)
```

