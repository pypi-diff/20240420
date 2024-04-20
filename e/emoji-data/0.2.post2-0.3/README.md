# Comparing `tmp/emoji-data-0.2.post2.tar.gz` & `tmp/emoji_data-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emoji-data-0.2.post2.tar", last modified: Wed Mar 22 09:13:07 2023, max compression
+gzip compressed data, was "emoji_data-0.3.tar", last modified: Sat Apr 20 16:44:38 2024, max compression
```

## Comparing `emoji-data-0.2.post2.tar` & `emoji_data-0.3.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 09:13:07.563232 emoji-data-0.2.post2/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-22 09:12:56.000000 emoji-data-0.2.post2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-03-22 09:12:56.000000 emoji-data-0.2.post2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-03-22 09:12:56.000000 emoji-data-0.2.post2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-22 09:12:56.000000 emoji-data-0.2.post2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-03-22 09:13:07.563232 emoji-data-0.2.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-03-22 09:12:56.000000 emoji-data-0.2.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-03-22 09:12:56.000000 emoji-data-0.2.post2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 09:12:56.000000 emoji-data-0.2.post2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 09:13:07.563232 emoji-data-0.2.post2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 09:13:07.559232 emoji-data-0.2.post2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 09:13:07.559232 emoji-data-0.2.post2/src/emoji_data/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-22 09:12:56.000000 emoji-data-0.2.post2/src/emoji_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-03-22 09:12:56.000000 emoji-data-0.2.post2/src/emoji_data/character.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 09:13:07.563232 emoji-data-0.2.post2/src/emoji_data/data/
--rw-r--r--   0 runner    (1001) docker     (123)   111505 2023-03-22 09:12:56.000000 emoji-data-0.2.post2/src/emoji_data/data/emoji-data.txt
--rw-r--r--   0 runner    (1001) docker     (123)   191560 2023-03-22 09:12:56.000000 emoji-data-0.2.post2/src/emoji_data/data/emoji-sequences.txt
--rw-r--r--   0 runner    (1001) docker     (123)   593240 2023-03-22 09:12:56.000000 emoji-data-0.2.post2/src/emoji_data/data/emoji-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)    36542 2023-03-22 09:12:56.000000 emoji-data-0.2.post2/src/emoji_data/data/emoji-variation-sequences.txt
--rw-r--r--   0 runner    (1001) docker     (123)   231164 2023-03-22 09:12:56.000000 emoji-data-0.2.post2/src/emoji_data/data/emoji-zwj-sequences.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8953 2023-03-22 09:12:56.000000 emoji-data-0.2.post2/src/emoji_data/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-03-22 09:12:56.000000 emoji-data-0.2.post2/src/emoji_data/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-22 09:12:56.000000 emoji-data-0.2.post2/src/emoji_data/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-03-22 09:12:56.000000 emoji-data-0.2.post2/src/emoji_data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-22 09:13:07.000000 emoji-data-0.2.post2/src/emoji_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 09:13:07.559232 emoji-data-0.2.post2/src/emoji_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-03-22 09:13:07.000000 emoji-data-0.2.post2/src/emoji_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-22 09:13:07.000000 emoji-data-0.2.post2/src/emoji_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 09:13:07.000000 emoji-data-0.2.post2/src/emoji_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-22 09:13:07.000000 emoji-data-0.2.post2/src/emoji_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-22 09:13:07.000000 emoji-data-0.2.post2/src/emoji_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:44:38.438801 emoji_data-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-20 16:44:32.000000 emoji_data-0.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-20 16:44:32.000000 emoji_data-0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-20 16:44:32.000000 emoji_data-0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-20 16:44:32.000000 emoji_data-0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-20 16:44:38.438801 emoji_data-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-20 16:44:32.000000 emoji_data-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-20 16:44:32.000000 emoji_data-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-20 16:44:32.000000 emoji_data-0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 16:44:38.438801 emoji_data-0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:44:38.430801 emoji_data-0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:44:38.434801 emoji_data-0.3/src/emoji_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-20 16:44:38.000000 emoji_data-0.3/src/emoji_data/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/character.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:44:38.434801 emoji_data-0.3/src/emoji_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/data/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   111503 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/data/emoji-data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   191562 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/data/emoji-sequences.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   639404 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/data/emoji-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38358 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/data/emoji-variation-sequences.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   251595 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/data/emoji-zwj-sequences.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13192 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11302 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-20 16:44:32.000000 emoji_data-0.3/src/emoji_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:44:38.434801 emoji_data-0.3/src/emoji_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-20 16:44:38.000000 emoji_data-0.3/src/emoji_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-20 16:44:38.000000 emoji_data-0.3/src/emoji_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 16:44:38.000000 emoji_data-0.3/src/emoji_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-20 16:44:38.000000 emoji_data-0.3/src/emoji_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 16:44:38.000000 emoji_data-0.3/src/emoji_data.egg-info/top_level.txt
```

### Comparing `emoji-data-0.2.post2/CHANGELOG.md` & `emoji_data-0.3/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,23 @@
 # CHANGELOG
 
+## 0.3
+
+> 📅 **Date** 2024-4-21
+
+- 🌞 Highlights:
+  - Update to Emoji version 15.1
+- 🆕 New Features:
+  - #44: Add `py.typed` file, make the package PEP-561 friendly
+- Misc:
+  - Add lots of typeshed code
+  - Add pre-commit
+  - Update Sphinx-docs
+  - Other modifications
+
 ## 0.2
 
 - Update:
   - Emoji version 15.0
 
 - Changes:
   - New `pyproject.toml` setup
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `emoji-data-0.2.post2/LICENSE.txt` & `emoji_data-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `emoji-data-0.2.post2/src/emoji_data/character.py` & `emoji_data-0.3/src/emoji_data/character.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,113 +1,177 @@
+from __future__ import annotations
+
+import sys
 from enum import Enum
-from typing import Iterable, List, Tuple, Union
+from typing import Union
+
+if sys.version_info < (3, 11):  # pragma: no cover
+    from typing_extensions import Self
+else:  # pragma: no cover
+    from typing import Self
+
+if sys.version_info < (3, 9):  # pragma: no cover
+    from typing import Iterable, MutableSequence, Sequence, Tuple
+else:  # pragma: no cover
+    from collections.abc import Iterable, Sequence, MutableSequence
 
-from . import version
 from .types import BaseDictContainer
-from .utils import code_point_to_regex, read_data_file_iterable, resources_files
+from .utils import code_point_to_regex, data_file, read_data_file_iterable
 
-__all__ = ['EmojiCharProperty', 'EmojiCharacter', 'TEXT_PRESENTATION_SELECTOR', 'EMOJI_PRESENTATION_SELECTOR',
-           'EMOJI_KEYCAP', 'REGIONAL_INDICATORS', 'TAGS', 'ZWJ']
+__all__ = [
+    "EmojiCharProperty",
+    "EmojiCharacter",
+    "TEXT_PRESENTATION_SELECTOR",
+    "EMOJI_PRESENTATION_SELECTOR",
+    "EMOJI_KEYCAP",
+    "REGIONAL_INDICATORS",
+    "TAGS",
+    "ZWJ",
+]
 
 
 TEXT_PRESENTATION_SELECTOR = 0xFE0E
+"""The character U+FE0E VARIATION SELECTOR-15 (VS15), used to request a text presentation for an emoji character.
+(Also known as text variation selector in prior versions of this specification.)
+"""
+
 EMOJI_PRESENTATION_SELECTOR = 0xFE0F
+"""The character U+FE0F VARIATION SELECTOR-16 (VS16), used to request an emoji presentation for an emoji character.
+(Also known as emoji variation selector in prior versions of this specification.)
+"""
+
 EMOJI_KEYCAP = 0x20E3
+"""A sequence of the following form::
+
+    emoji_keycap_sequence := [0-9#*] \\x{FE0F 20E3}
+
+- These sequences are in the `emoji-sequences.txt` file listed under the type_field ``Emoji_Keycap_Sequence``
+"""
+
 ZWJ = 0x200D
+"""An emoji sequence with at least one joiner character.
+"""
+
 REGIONAL_INDICATORS = list(range(0x1F1E6, 0x1F1FF + 1))
+"""regional indicators"""
+
 TAGS = list(range(0xE0020, 0xE007F + 1))
+"""tags"""
 
 
 class EmojiCharProperty(Enum):
     """Emoji Character Properties
 
+    character properties are available for emoji characters.
+
     see: http://www.unicode.org/reports/tr51/#Emoji_Properties
     """
-    EMOJI = 'Emoji'
-    EPRES = 'Emoji_Presentation'
-    EMOD = 'Emoji_Modifier'
-    EBASE = 'Emoji_Modifier_Base'
-    ECOMP = 'Emoji_Component'
-    EXTPICT = 'Extended_Pictographic'
+
+    EMOJI = "Emoji"
+    """for characters that are emoji"""
+
+    EPRES = "Emoji_Presentation"
+    """ for characters that have emoji presentation by default"""
+
+    EMOD = "Emoji_Modifier"
+    """for characters that are emoji modifiers"""
+
+    EBASE = "Emoji_Modifier_Base"
+    """for characters that can serve as a base for emoji modifiers"""
+
+    ECOMP = "Emoji_Component"
+    """for characters used in emoji sequences that normally do not appear on emoji keyboards as separate choices, such as keycap base characters or Regional_Indicator characters.
+
+    All characters in emoji sequences are either Emoji or Emoji_Component.
+    Implementations must not, however, assume that all Emoji_Component characters are also Emoji.
+    There are some non-emoji characters that are used in various emoji sequences, such as tag characters and ZWJ.
+    """
+
+    EXTPICT = "Extended_Pictographic"
+    """for characters that are used to future-proof segmentation.
+
+    The Extended_Pictographic characters contain all the Emoji characters except for some Emoji_Component characters.
+    """
 
 
-class _MetaClass(BaseDictContainer):
+class MetaClass(BaseDictContainer):
     pass
 
 
-class EmojiCharacter(metaclass=_MetaClass):
-    """emoji character — A character that has the Emoji property. These characters are recommended for use as emoji.
+class EmojiCharacter(metaclass=MetaClass):
+    """emoji character — A character that has the Emoji property.
+
+    These characters are recommended for use as emoji.
 
     see: http://www.unicode.org/reports/tr51/#Emoji_Characters
     """
 
-    def __init__(self,
-                 code_point: int,
-                 properties: Union[Iterable[EmojiCharProperty], EmojiCharProperty, None] = None,
-                 comments: Union[Iterable[str], str, None] = None,
-                 ):
+    def __init__(
+        self,
+        code_point: int,
+        properties: Union[Iterable[EmojiCharProperty], EmojiCharProperty, None] = None,
+        comments: Union[Iterable[str], str, None] = None,
+    ):
         self._code_point = code_point
         self._string = chr(self._code_point)
         self._regex = code_point_to_regex(code_point)
         #
         if properties is None:
-            self._properties: List[EmojiCharProperty] = list()
+            self._properties: MutableSequence[EmojiCharProperty] = []
         elif isinstance(properties, EmojiCharProperty):
             self._properties = [properties]
         elif isinstance(properties, Iterable):
             self._properties = list(properties)
         else:
             raise TypeError(
-                f'Argument `properties` expects `EmojiCharProperty`, `Iterable[EmojiCharProperty]`, or `None`, but actual {type(properties)}'
+                f"Argument `properties` expects `EmojiCharProperty`, `Iterable[EmojiCharProperty]`, or `None`, but actual {type(properties)}"
             )
         #
         if comments is None:
-            self._comments: List[str] = list()
+            self._comments: MutableSequence[str] = []
         elif isinstance(comments, str):
             self._comments = [comments]
         elif isinstance(comments, Iterable):
             self._comments = [s for s in comments if isinstance(s, str)]
         else:
-            raise TypeError(
-                f'Argument `comments` expects `str`, `Iterable[str]`, or `None`, but actual {type(comments)}'
-            )
+            raise TypeError(f"Argument `comments` expects `str`, `Iterable[str]`, or `None`, but actual {type(comments)}")
 
     def __str__(self):
         return self._string
 
     def __repr__(self):
-        return '<{} hex={} char={!r}>'.format(
+        return "<{} code_point={} char={!r}>".format(
             type(self).__name__,
-            self.hex,
+            self.code_point_string,
             self.string,
         )
 
     _initialed = False
 
     @classmethod
     def initial(cls):
         """Initial the class
 
         Load Emoji Characters and it's properties from package data file into class internal dictionary
         """
         if cls._initialed:
             return
-        with resources_files(version.__package__).joinpath('data', 'emoji-data.txt').open(encoding='utf8') as fp:
+        with data_file("emoji-data.txt").open(encoding="utf8") as fp:
             for content, comment in read_data_file_iterable(fp):
-                cps, property_text = (part.strip() for part in content.split(';', 1))
-                cps_parts = cps.split('..', 1)
+                cps, property_text = (part.strip() for part in content.split(";", 1))
+                cps_parts = cps.split("..", 1)
                 property_ = EmojiCharProperty(property_text)
                 for cp in range(int(cps_parts[0], 16), 1 + int(cps_parts[-1], 16)):
                     try:
-                        inst = cls[cp]
+                        inst: Self = cls[cp]  # type:ignore[annotation-unchecked]
                     except KeyError:
                         cls[cp] = cls(cp, property_, comment)
                     else:
-                        inst.add_property(property_)
-                        inst.add_comment(comment)
+                        inst._add_property(property_)
+                        inst._add_comment(comment)
             for cp in TEXT_PRESENTATION_SELECTOR, EMOJI_PRESENTATION_SELECTOR, EMOJI_KEYCAP:
                 if cp not in cls:
                     cls[cp] = cls(cp)
         # OK!
         cls._initialed = True
 
     @classmethod
@@ -115,100 +179,105 @@
         if not cls._initialed:
             return
         keys = list(cls)
         for k in keys:
             del cls[k]
         cls._initialed = False
 
+    if sys.version_info < (3, 9):  # pragma: no cover
+
+        @classmethod
+        def items(cls) -> Iterable[Tuple[int, Self]]:
+            return ((k, cls[k]) for k in cls)
+
+    else:
+
+        @classmethod
+        def items(cls) -> Iterable[tuple[int, Self]]:
+            """Return an iterator of all code-point -> emoji-character pairs of the class"""
+            return ((k, cls[k]) for k in cls)
+
     @classmethod
-    def items(cls) -> Iterable[Tuple[int, 'EmojiCharacter']]:
-        """Return an iterator of all code-point -> emoji-character pairs of the class
-        """
-        return ((k, cls[k]) for k in cls)
+    def keys(cls) -> Iterable[int]:
+        """Return an iterator of each emoji-character's key code-point of the class"""
+        return (k for k in cls)
 
     @classmethod
-    def values(cls) -> Iterable['EmojiCharacter']:
-        """Return an iterator of all emoji-characters of the class
-        """
+    def values(cls) -> Iterable[Self]:
+        """Return an iterator of all emoji-characters of the class"""
         return (cls[k] for k in cls)
 
-    def add_property(self, val: EmojiCharProperty):
+    def _add_property(self, val: EmojiCharProperty):
         if val not in self._properties:
             self._properties.append(val)
 
-    def add_comment(self, val: str):
+    def _add_comment(self, val: str):
         if val not in self._properties:
             self._comments.append(val)
 
     @property
     def code_point(self) -> int:
-        """Unicode integer value of the Emoji
-
-        :type: int
-        """
+        """Unicode integer value of the emoji-characters"""
         return self._code_point
 
     @property
-    def properties(self) -> List[EmojiCharProperty]:
-        """Property description text of the Emoji
+    def code_point_string(self) -> str:
+        """Unicode style hex string of the emoji-characters's code-point
 
-        :type: List[EmojiCharProperty]
+        eg: ``25FB``
         """
-        return self._properties
+        return f"{self._code_point:04X}"
 
     @property
-    def comments(self) -> List[str]:
-        """Comments of the Emoji
+    def properties(self) -> Sequence[EmojiCharProperty]:
+        """Property description text of the emoji-characters"""
+        return self._properties
 
-        :type: List[str]
-        """
+    @property
+    def comments(self) -> Sequence[str]:
+        """Comments of the Emoji"""
         return self._comments
 
     @property
     def regex(self) -> str:
-        """Regular express for the Emoji
-
-        :type: str
-        """
+        """Regular express for the emoji-characters"""
         return self._regex
 
     @property
     def hex(self) -> str:
-        """Hex style text of the Emoji's Unicode
+        """Python style hex string of the emoji-characters's code-pint
 
-        :type: str
+        eg: ``0x25fb``
         """
         return hex(self._code_point)
 
     @property
     def string(self) -> str:
-        """Emoji character string
-
-        :type: str
-        """
+        """Emoji character string"""
         return self._string
 
     @classmethod
-    def from_string(cls, value: str) -> 'EmojiCharacter':
-        """Get an :class:`EmojiCharacter` instance by Emoji Unicode character
+    def from_character(cls, c: str) -> Self:
+        """Get :class:`EmojiCharacter` instance from a single Emoji Unicode character
+
+        .. note::
+            ``c`` should be a single unicode character.
 
-        :param str value: Emoji character
+        :param c: Emoji character
         :return: Instance returned from the class's internal dictionary
-        :rtype: EmojiCharacter
-        :raises KeyError: When character not found in the class' internal dictionary
+        :raise KeyError: When character not found in the class' internal dictionary
         """
-        return cls[ord(value)]
+        return cls[ord(c)]
 
     @classmethod
-    def from_hex(cls, value: Union[int, str]) -> 'EmojiCharacter':
+    def from_hex(cls, value: Union[int, str]) -> Self:
         """Get an :class:`EmojiCharacter` instance by Emoji Unicode integer value or it's hex string
 
-        :param Union[int, str] value: Emoji Unicode, either integer value or hex string
+        :param value: Emoji Unicode, either integer value or hex string
         :return: Instance returned from the class's internal dictionary
-        :rtype: EmojiCharacter
         :raises KeyError: When code not found in the class' internal dictionary
         """
         if isinstance(value, str):
             return cls[int(value, 16)]
         return cls[int(value)]
```

### Comparing `emoji-data-0.2.post2/src/emoji_data/data/emoji-data.txt` & `emoji_data-0.3/src/emoji_data/data/emoji-data.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # emoji-data.txt
-# Date: 2022-08-02, 00:26:10 GMT
-# © 2022 Unicode®, Inc.
+# Date: 2023-02-01, 02:22:54 GMT
+# © 2023 Unicode®, Inc.
 # Unicode and the Unicode Logo are registered trademarks of Unicode, Inc. in the U.S. and other countries.
 # For terms of use, see https://www.unicode.org/terms_of_use.html
 #
 # Emoji Data for UTS #51
-# Used with Emoji Version 15.0 and subsequent minor revisions (if any)
+# Used with Emoji Version 15.1 and subsequent minor revisions (if any)
 #
 # For documentation and usage, see https://www.unicode.org/reports/tr51
 #
-# Format: 
-# <codepoint(s)> ; <property> # <comments> 
+# Format:
+# <codepoint(s)> ; <property> # <comments>
 # Note: there is no guarantee as to the structure of whitespace or comments
 #
 # Characters and sequences are listed in code point order. Users should be shown a more natural order.
 # See the CLDR collation order for Emoji.
 
 
 # ================================================
```

### Comparing `emoji-data-0.2.post2/src/emoji_data/data/emoji-sequences.txt` & `emoji_data-0.3/src/emoji_data/data/emoji-sequences.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # emoji-sequences.txt
-# Date: 2022-08-15, 23:13:41 GMT
-# © 2022 Unicode®, Inc.
+# Date: 2023-06-05, 21:39:54 GMT
+# © 2023 Unicode®, Inc.
 # Unicode and the Unicode Logo are registered trademarks of Unicode, Inc. in the U.S. and other countries.
 # For terms of use, see https://www.unicode.org/terms_of_use.html
 #
 # Emoji Sequence Data for UTS #51
-# Version: 15.0
+# Version: 15.1
 #
 # For documentation and usage, see https://www.unicode.org/reports/tr51
 #
 # Format:
 #   code_point(s) ; type_field ; description # comments
 # Fields:
 #   code_point(s): one or more code points in hex format, separated by spaces
@@ -34,15 +34,14 @@
 # Characters and sequences are listed in code point order. Users should be shown a more natural order.
 # See the CLDR collation order for Emoji.
 
 # ================================================
 
 # Basic_Emoji
 
-
 231A..231B    ; Basic_Emoji                  ; watch..hourglass done                                          # E0.6   [2] (⌚..⌛)
 23E9..23EC    ; Basic_Emoji                  ; fast-forward button..fast down button                          # E0.6   [4] (⏩..⏬)
 23F0          ; Basic_Emoji                  ; alarm clock                                                    # E0.6   [1] (⏰)
 23F3          ; Basic_Emoji                  ; hourglass not done                                             # E0.6   [1] (⏳)
 25FD..25FE    ; Basic_Emoji                  ; white medium-small square..black medium-small square           # E0.6   [2] (◽..◾)
 2614..2615    ; Basic_Emoji                  ; umbrella with rain drops..hot beverage                         # E0.6   [2] (☔..☕)
 2648..2653    ; Basic_Emoji                  ; Aries..Pisces                                                  # E0.6  [12] (♈..♓)
@@ -530,15 +529,14 @@
 
 # Total elements: 1386
 
 # ================================================
 
 # Emoji_Keycap_Sequence
 
-
 0023 FE0F 20E3; Emoji_Keycap_Sequence        ; keycap: \x{23}                                                 # E0.6   [1] (#️⃣)
 002A FE0F 20E3; Emoji_Keycap_Sequence        ; keycap: *                                                      # E2.0   [1] (*️⃣)
 0030 FE0F 20E3; Emoji_Keycap_Sequence        ; keycap: 0                                                      # E0.6   [1] (0️⃣)
 0031 FE0F 20E3; Emoji_Keycap_Sequence        ; keycap: 1                                                      # E0.6   [1] (1️⃣)
 0032 FE0F 20E3; Emoji_Keycap_Sequence        ; keycap: 2                                                      # E0.6   [1] (2️⃣)
 0033 FE0F 20E3; Emoji_Keycap_Sequence        ; keycap: 3                                                      # E0.6   [1] (3️⃣)
 0034 FE0F 20E3; Emoji_Keycap_Sequence        ; keycap: 4                                                      # E0.6   [1] (4️⃣)
@@ -549,16 +547,15 @@
 0039 FE0F 20E3; Emoji_Keycap_Sequence        ; keycap: 9                                                      # E0.6   [1] (9️⃣)
 
 # Total elements: 12
 
 # ================================================
 
 # RGI_Emoji_Flag_Sequence: This list does not include deprecated or macroregion flags, except for UN and EU.
-# See Annex B of TR51 for more information.
-
+# See Annex B of UTS #51 for more information.
 
 1F1E6 1F1E8   ; RGI_Emoji_Flag_Sequence      ; flag: Ascension Island                                         # E2.0   [1] (🇦🇨)
 1F1E6 1F1E9   ; RGI_Emoji_Flag_Sequence      ; flag: Andorra                                                  # E2.0   [1] (🇦🇩)
 1F1E6 1F1EA   ; RGI_Emoji_Flag_Sequence      ; flag: United Arab Emirates                                     # E2.0   [1] (🇦🇪)
 1F1E6 1F1EB   ; RGI_Emoji_Flag_Sequence      ; flag: Afghanistan                                              # E2.0   [1] (🇦🇫)
 1F1E6 1F1EC   ; RGI_Emoji_Flag_Sequence      ; flag: Antigua & Barbuda                                        # E2.0   [1] (🇦🇬)
 1F1E6 1F1EE   ; RGI_Emoji_Flag_Sequence      ; flag: Anguilla                                                 # E2.0   [1] (🇦🇮)
@@ -783,15 +780,15 @@
 1F1F9 1F1ED   ; RGI_Emoji_Flag_Sequence      ; flag: Thailand                                                 # E2.0   [1] (🇹🇭)
 1F1F9 1F1EF   ; RGI_Emoji_Flag_Sequence      ; flag: Tajikistan                                               # E2.0   [1] (🇹🇯)
 1F1F9 1F1F0   ; RGI_Emoji_Flag_Sequence      ; flag: Tokelau                                                  # E2.0   [1] (🇹🇰)
 1F1F9 1F1F1   ; RGI_Emoji_Flag_Sequence      ; flag: Timor-Leste                                              # E2.0   [1] (🇹🇱)
 1F1F9 1F1F2   ; RGI_Emoji_Flag_Sequence      ; flag: Turkmenistan                                             # E2.0   [1] (🇹🇲)
 1F1F9 1F1F3   ; RGI_Emoji_Flag_Sequence      ; flag: Tunisia                                                  # E2.0   [1] (🇹🇳)
 1F1F9 1F1F4   ; RGI_Emoji_Flag_Sequence      ; flag: Tonga                                                    # E2.0   [1] (🇹🇴)
-1F1F9 1F1F7   ; RGI_Emoji_Flag_Sequence      ; flag: Turkey                                                   # E2.0   [1] (🇹🇷)
+1F1F9 1F1F7   ; RGI_Emoji_Flag_Sequence      ; flag: Türkiye                                                  # E2.0   [1] (🇹🇷)
 1F1F9 1F1F9   ; RGI_Emoji_Flag_Sequence      ; flag: Trinidad & Tobago                                        # E2.0   [1] (🇹🇹)
 1F1F9 1F1FB   ; RGI_Emoji_Flag_Sequence      ; flag: Tuvalu                                                   # E2.0   [1] (🇹🇻)
 1F1F9 1F1FC   ; RGI_Emoji_Flag_Sequence      ; flag: Taiwan                                                   # E2.0   [1] (🇹🇼)
 1F1F9 1F1FF   ; RGI_Emoji_Flag_Sequence      ; flag: Tanzania                                                 # E2.0   [1] (🇹🇿)
 1F1FA 1F1E6   ; RGI_Emoji_Flag_Sequence      ; flag: Ukraine                                                  # E2.0   [1] (🇺🇦)
 1F1FA 1F1EC   ; RGI_Emoji_Flag_Sequence      ; flag: Uganda                                                   # E2.0   [1] (🇺🇬)
 1F1FA 1F1F2   ; RGI_Emoji_Flag_Sequence      ; flag: U.S. Outlying Islands                                    # E2.0   [1] (🇺🇲)
@@ -815,28 +812,26 @@
 1F1FF 1F1F2   ; RGI_Emoji_Flag_Sequence      ; flag: Zambia                                                   # E2.0   [1] (🇿🇲)
 1F1FF 1F1FC   ; RGI_Emoji_Flag_Sequence      ; flag: Zimbabwe                                                 # E2.0   [1] (🇿🇼)
 
 # Total elements: 258
 
 # ================================================
 
-# RGI_Emoji_Tag_Sequence: See Annex C of TR51 for more information.
-
+# RGI_Emoji_Tag_Sequence: See Annex C of UTS #51 for more information.
 
 1F3F4 E0067 E0062 E0065 E006E E0067 E007F; RGI_Emoji_Tag_Sequence; flag: England                              # E5.0   [1] (🏴󠁧󠁢󠁥󠁮󠁧󠁿)
 1F3F4 E0067 E0062 E0073 E0063 E0074 E007F; RGI_Emoji_Tag_Sequence; flag: Scotland                             # E5.0   [1] (🏴󠁧󠁢󠁳󠁣󠁴󠁿)
 1F3F4 E0067 E0062 E0077 E006C E0073 E007F; RGI_Emoji_Tag_Sequence; flag: Wales                                # E5.0   [1] (🏴󠁧󠁢󠁷󠁬󠁳󠁿)
 
 # Total elements: 3
 
 # ================================================
 
 # RGI_Emoji_Modifier_Sequence
 
-
 261D 1F3FB    ; RGI_Emoji_Modifier_Sequence  ; index pointing up: light skin tone                             # E1.0   [1] (☝🏻)
 261D 1F3FC    ; RGI_Emoji_Modifier_Sequence  ; index pointing up: medium-light skin tone                      # E1.0   [1] (☝🏼)
 261D 1F3FD    ; RGI_Emoji_Modifier_Sequence  ; index pointing up: medium skin tone                            # E1.0   [1] (☝🏽)
 261D 1F3FE    ; RGI_Emoji_Modifier_Sequence  ; index pointing up: medium-dark skin tone                       # E1.0   [1] (☝🏾)
 261D 1F3FF    ; RGI_Emoji_Modifier_Sequence  ; index pointing up: dark skin tone                              # E1.0   [1] (☝🏿)
 26F9 1F3FB    ; RGI_Emoji_Modifier_Sequence  ; person bouncing ball: light skin tone                          # E2.0   [1] (⛹🏻)
 26F9 1F3FC    ; RGI_Emoji_Modifier_Sequence  ; person bouncing ball: medium-light skin tone                   # E2.0   [1] (⛹🏼)
```

### Comparing `emoji-data-0.2.post2/src/emoji_data/data/emoji-test.txt` & `emoji_data-0.3/src/emoji_data/data/emoji-test.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # emoji-test.txt
-# Date: 2022-08-12, 20:24:39 GMT
-# © 2022 Unicode®, Inc.
+# Date: 2023-06-05, 21:39:54 GMT
+# © 2023 Unicode®, Inc.
 # Unicode and the Unicode Logo are registered trademarks of Unicode, Inc. in the U.S. and other countries.
 # For terms of use, see https://www.unicode.org/terms_of_use.html
 #
 # Emoji Keyboard/Display Test Data for UTS #51
-# Version: 15.0
+# Version: 15.1
 #
 # For documentation and usage, see https://www.unicode.org/reports/tr51
 #
 # This file provides data for testing which emoji forms should be in keyboards and which should also be displayed/processed.
 # Format: code points; status # emoji name
 #     Code points — list of one or more hex code points, separated by spaces
 #     Status
@@ -19,15 +19,15 @@
 #                             excluding Emoji_Component
 #       minimally-qualified — a minimally-qualified emoji (see ED-18a in UTS #51)
 #       unqualified         — a unqualified emoji (See ED-19 in UTS #51)
 # Notes:
 #   • This includes the emoji components that need emoji presentation (skin tone and hair)
 #     when isolated, but omits the components that need not have an emoji
 #     presentation when isolated.
-#   • The RGI set is covered by the listed fully-qualified emoji. 
+#   • The RGI set is covered by the listed fully-qualified emoji.
 #   • The listed minimally-qualified and unqualified cover all cases where an
 #     element of the RGI set is missing one or more emoji presentation selectors.
 #   • The file is in CLDR order, not codepoint order. This is recommended (but not required!) for keyboard palettes.
 #   • The groups and subgroups are illustrative. See the Emoji Order chart for more information.
 
 
 # group: Smileys & Emotion
@@ -89,14 +89,18 @@
 1F60F                                                  ; fully-qualified     # 😏 E0.6 smirking face
 1F612                                                  ; fully-qualified     # 😒 E0.6 unamused face
 1F644                                                  ; fully-qualified     # 🙄 E1.0 face with rolling eyes
 1F62C                                                  ; fully-qualified     # 😬 E1.0 grimacing face
 1F62E 200D 1F4A8                                       ; fully-qualified     # 😮‍💨 E13.1 face exhaling
 1F925                                                  ; fully-qualified     # 🤥 E3.0 lying face
 1FAE8                                                  ; fully-qualified     # 🫨 E15.0 shaking face
+1F642 200D 2194 FE0F                                   ; fully-qualified     # 🙂‍↔️ E15.1 head shaking horizontally
+1F642 200D 2194                                        ; minimally-qualified # 🙂‍↔ E15.1 head shaking horizontally
+1F642 200D 2195 FE0F                                   ; fully-qualified     # 🙂‍↕️ E15.1 head shaking vertically
+1F642 200D 2195                                        ; minimally-qualified # 🙂‍↕ E15.1 head shaking vertically
 
 # subgroup: face-sleepy
 1F60C                                                  ; fully-qualified     # 😌 E0.6 relieved face
 1F614                                                  ; fully-qualified     # 😔 E0.6 pensive face
 1F62A                                                  ; fully-qualified     # 😪 E0.6 sleepy face
 1F924                                                  ; fully-qualified     # 🤤 E3.0 drooling face
 1F634                                                  ; fully-qualified     # 😴 E1.0 sleeping face
@@ -240,16 +244,16 @@
 1F5E8 FE0F                                             ; fully-qualified     # 🗨️ E2.0 left speech bubble
 1F5E8                                                  ; unqualified         # 🗨 E2.0 left speech bubble
 1F5EF FE0F                                             ; fully-qualified     # 🗯️ E0.7 right anger bubble
 1F5EF                                                  ; unqualified         # 🗯 E0.7 right anger bubble
 1F4AD                                                  ; fully-qualified     # 💭 E1.0 thought balloon
 1F4A4                                                  ; fully-qualified     # 💤 E0.6 ZZZ
 
-# Smileys & Emotion subtotal:		180
-# Smileys & Emotion subtotal:		180	w/o modifiers
+# Smileys & Emotion subtotal:		184
+# Smileys & Emotion subtotal:		184	w/o modifiers
 
 # group: People & Body
 
 # subgroup: hand-fingers-open
 1F44B                                                  ; fully-qualified     # 👋 E0.6 waving hand
 1F44B 1F3FB                                            ; fully-qualified     # 👋🏻 E1.0 waving hand: light skin tone
 1F44B 1F3FC                                            ; fully-qualified     # 👋🏼 E1.0 waving hand: medium-light skin tone
@@ -2061,14 +2065,74 @@
 1F6B6 1F3FC 200D 2640                                  ; minimally-qualified # 🚶🏼‍♀ E4.0 woman walking: medium-light skin tone
 1F6B6 1F3FD 200D 2640 FE0F                             ; fully-qualified     # 🚶🏽‍♀️ E4.0 woman walking: medium skin tone
 1F6B6 1F3FD 200D 2640                                  ; minimally-qualified # 🚶🏽‍♀ E4.0 woman walking: medium skin tone
 1F6B6 1F3FE 200D 2640 FE0F                             ; fully-qualified     # 🚶🏾‍♀️ E4.0 woman walking: medium-dark skin tone
 1F6B6 1F3FE 200D 2640                                  ; minimally-qualified # 🚶🏾‍♀ E4.0 woman walking: medium-dark skin tone
 1F6B6 1F3FF 200D 2640 FE0F                             ; fully-qualified     # 🚶🏿‍♀️ E4.0 woman walking: dark skin tone
 1F6B6 1F3FF 200D 2640                                  ; minimally-qualified # 🚶🏿‍♀ E4.0 woman walking: dark skin tone
+1F6B6 200D 27A1 FE0F                                   ; fully-qualified     # 🚶‍➡️ E15.1 person walking facing right
+1F6B6 200D 27A1                                        ; minimally-qualified # 🚶‍➡ E15.1 person walking facing right
+1F6B6 1F3FB 200D 27A1 FE0F                             ; fully-qualified     # 🚶🏻‍➡️ E15.1 person walking facing right: light skin tone
+1F6B6 1F3FB 200D 27A1                                  ; minimally-qualified # 🚶🏻‍➡ E15.1 person walking facing right: light skin tone
+1F6B6 1F3FC 200D 27A1 FE0F                             ; fully-qualified     # 🚶🏼‍➡️ E15.1 person walking facing right: medium-light skin tone
+1F6B6 1F3FC 200D 27A1                                  ; minimally-qualified # 🚶🏼‍➡ E15.1 person walking facing right: medium-light skin tone
+1F6B6 1F3FD 200D 27A1 FE0F                             ; fully-qualified     # 🚶🏽‍➡️ E15.1 person walking facing right: medium skin tone
+1F6B6 1F3FD 200D 27A1                                  ; minimally-qualified # 🚶🏽‍➡ E15.1 person walking facing right: medium skin tone
+1F6B6 1F3FE 200D 27A1 FE0F                             ; fully-qualified     # 🚶🏾‍➡️ E15.1 person walking facing right: medium-dark skin tone
+1F6B6 1F3FE 200D 27A1                                  ; minimally-qualified # 🚶🏾‍➡ E15.1 person walking facing right: medium-dark skin tone
+1F6B6 1F3FF 200D 27A1 FE0F                             ; fully-qualified     # 🚶🏿‍➡️ E15.1 person walking facing right: dark skin tone
+1F6B6 1F3FF 200D 27A1                                  ; minimally-qualified # 🚶🏿‍➡ E15.1 person walking facing right: dark skin tone
+1F6B6 200D 2640 FE0F 200D 27A1 FE0F                    ; fully-qualified     # 🚶‍♀️‍➡️ E15.1 woman walking facing right
+1F6B6 200D 2640 200D 27A1 FE0F                         ; minimally-qualified # 🚶‍♀‍➡️ E15.1 woman walking facing right
+1F6B6 200D 2640 FE0F 200D 27A1                         ; minimally-qualified # 🚶‍♀️‍➡ E15.1 woman walking facing right
+1F6B6 200D 2640 200D 27A1                              ; minimally-qualified # 🚶‍♀‍➡ E15.1 woman walking facing right
+1F6B6 1F3FB 200D 2640 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🚶🏻‍♀️‍➡️ E15.1 woman walking facing right: light skin tone
+1F6B6 1F3FB 200D 2640 200D 27A1 FE0F                   ; minimally-qualified # 🚶🏻‍♀‍➡️ E15.1 woman walking facing right: light skin tone
+1F6B6 1F3FB 200D 2640 FE0F 200D 27A1                   ; minimally-qualified # 🚶🏻‍♀️‍➡ E15.1 woman walking facing right: light skin tone
+1F6B6 1F3FB 200D 2640 200D 27A1                        ; minimally-qualified # 🚶🏻‍♀‍➡ E15.1 woman walking facing right: light skin tone
+1F6B6 1F3FC 200D 2640 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🚶🏼‍♀️‍➡️ E15.1 woman walking facing right: medium-light skin tone
+1F6B6 1F3FC 200D 2640 200D 27A1 FE0F                   ; minimally-qualified # 🚶🏼‍♀‍➡️ E15.1 woman walking facing right: medium-light skin tone
+1F6B6 1F3FC 200D 2640 FE0F 200D 27A1                   ; minimally-qualified # 🚶🏼‍♀️‍➡ E15.1 woman walking facing right: medium-light skin tone
+1F6B6 1F3FC 200D 2640 200D 27A1                        ; minimally-qualified # 🚶🏼‍♀‍➡ E15.1 woman walking facing right: medium-light skin tone
+1F6B6 1F3FD 200D 2640 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🚶🏽‍♀️‍➡️ E15.1 woman walking facing right: medium skin tone
+1F6B6 1F3FD 200D 2640 200D 27A1 FE0F                   ; minimally-qualified # 🚶🏽‍♀‍➡️ E15.1 woman walking facing right: medium skin tone
+1F6B6 1F3FD 200D 2640 FE0F 200D 27A1                   ; minimally-qualified # 🚶🏽‍♀️‍➡ E15.1 woman walking facing right: medium skin tone
+1F6B6 1F3FD 200D 2640 200D 27A1                        ; minimally-qualified # 🚶🏽‍♀‍➡ E15.1 woman walking facing right: medium skin tone
+1F6B6 1F3FE 200D 2640 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🚶🏾‍♀️‍➡️ E15.1 woman walking facing right: medium-dark skin tone
+1F6B6 1F3FE 200D 2640 200D 27A1 FE0F                   ; minimally-qualified # 🚶🏾‍♀‍➡️ E15.1 woman walking facing right: medium-dark skin tone
+1F6B6 1F3FE 200D 2640 FE0F 200D 27A1                   ; minimally-qualified # 🚶🏾‍♀️‍➡ E15.1 woman walking facing right: medium-dark skin tone
+1F6B6 1F3FE 200D 2640 200D 27A1                        ; minimally-qualified # 🚶🏾‍♀‍➡ E15.1 woman walking facing right: medium-dark skin tone
+1F6B6 1F3FF 200D 2640 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🚶🏿‍♀️‍➡️ E15.1 woman walking facing right: dark skin tone
+1F6B6 1F3FF 200D 2640 200D 27A1 FE0F                   ; minimally-qualified # 🚶🏿‍♀‍➡️ E15.1 woman walking facing right: dark skin tone
+1F6B6 1F3FF 200D 2640 FE0F 200D 27A1                   ; minimally-qualified # 🚶🏿‍♀️‍➡ E15.1 woman walking facing right: dark skin tone
+1F6B6 1F3FF 200D 2640 200D 27A1                        ; minimally-qualified # 🚶🏿‍♀‍➡ E15.1 woman walking facing right: dark skin tone
+1F6B6 200D 2642 FE0F 200D 27A1 FE0F                    ; fully-qualified     # 🚶‍♂️‍➡️ E15.1 man walking facing right
+1F6B6 200D 2642 200D 27A1 FE0F                         ; minimally-qualified # 🚶‍♂‍➡️ E15.1 man walking facing right
+1F6B6 200D 2642 FE0F 200D 27A1                         ; minimally-qualified # 🚶‍♂️‍➡ E15.1 man walking facing right
+1F6B6 200D 2642 200D 27A1                              ; minimally-qualified # 🚶‍♂‍➡ E15.1 man walking facing right
+1F6B6 1F3FB 200D 2642 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🚶🏻‍♂️‍➡️ E15.1 man walking facing right: light skin tone
+1F6B6 1F3FB 200D 2642 200D 27A1 FE0F                   ; minimally-qualified # 🚶🏻‍♂‍➡️ E15.1 man walking facing right: light skin tone
+1F6B6 1F3FB 200D 2642 FE0F 200D 27A1                   ; minimally-qualified # 🚶🏻‍♂️‍➡ E15.1 man walking facing right: light skin tone
+1F6B6 1F3FB 200D 2642 200D 27A1                        ; minimally-qualified # 🚶🏻‍♂‍➡ E15.1 man walking facing right: light skin tone
+1F6B6 1F3FC 200D 2642 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🚶🏼‍♂️‍➡️ E15.1 man walking facing right: medium-light skin tone
+1F6B6 1F3FC 200D 2642 200D 27A1 FE0F                   ; minimally-qualified # 🚶🏼‍♂‍➡️ E15.1 man walking facing right: medium-light skin tone
+1F6B6 1F3FC 200D 2642 FE0F 200D 27A1                   ; minimally-qualified # 🚶🏼‍♂️‍➡ E15.1 man walking facing right: medium-light skin tone
+1F6B6 1F3FC 200D 2642 200D 27A1                        ; minimally-qualified # 🚶🏼‍♂‍➡ E15.1 man walking facing right: medium-light skin tone
+1F6B6 1F3FD 200D 2642 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🚶🏽‍♂️‍➡️ E15.1 man walking facing right: medium skin tone
+1F6B6 1F3FD 200D 2642 200D 27A1 FE0F                   ; minimally-qualified # 🚶🏽‍♂‍➡️ E15.1 man walking facing right: medium skin tone
+1F6B6 1F3FD 200D 2642 FE0F 200D 27A1                   ; minimally-qualified # 🚶🏽‍♂️‍➡ E15.1 man walking facing right: medium skin tone
+1F6B6 1F3FD 200D 2642 200D 27A1                        ; minimally-qualified # 🚶🏽‍♂‍➡ E15.1 man walking facing right: medium skin tone
+1F6B6 1F3FE 200D 2642 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🚶🏾‍♂️‍➡️ E15.1 man walking facing right: medium-dark skin tone
+1F6B6 1F3FE 200D 2642 200D 27A1 FE0F                   ; minimally-qualified # 🚶🏾‍♂‍➡️ E15.1 man walking facing right: medium-dark skin tone
+1F6B6 1F3FE 200D 2642 FE0F 200D 27A1                   ; minimally-qualified # 🚶🏾‍♂️‍➡ E15.1 man walking facing right: medium-dark skin tone
+1F6B6 1F3FE 200D 2642 200D 27A1                        ; minimally-qualified # 🚶🏾‍♂‍➡ E15.1 man walking facing right: medium-dark skin tone
+1F6B6 1F3FF 200D 2642 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🚶🏿‍♂️‍➡️ E15.1 man walking facing right: dark skin tone
+1F6B6 1F3FF 200D 2642 200D 27A1 FE0F                   ; minimally-qualified # 🚶🏿‍♂‍➡️ E15.1 man walking facing right: dark skin tone
+1F6B6 1F3FF 200D 2642 FE0F 200D 27A1                   ; minimally-qualified # 🚶🏿‍♂️‍➡ E15.1 man walking facing right: dark skin tone
+1F6B6 1F3FF 200D 2642 200D 27A1                        ; minimally-qualified # 🚶🏿‍♂‍➡ E15.1 man walking facing right: dark skin tone
 1F9CD                                                  ; fully-qualified     # 🧍 E12.0 person standing
 1F9CD 1F3FB                                            ; fully-qualified     # 🧍🏻 E12.0 person standing: light skin tone
 1F9CD 1F3FC                                            ; fully-qualified     # 🧍🏼 E12.0 person standing: medium-light skin tone
 1F9CD 1F3FD                                            ; fully-qualified     # 🧍🏽 E12.0 person standing: medium skin tone
 1F9CD 1F3FE                                            ; fully-qualified     # 🧍🏾 E12.0 person standing: medium-dark skin tone
 1F9CD 1F3FF                                            ; fully-qualified     # 🧍🏿 E12.0 person standing: dark skin tone
 1F9CD 200D 2642 FE0F                                   ; fully-qualified     # 🧍‍♂️ E12.0 man standing
@@ -2121,68 +2185,236 @@
 1F9CE 1F3FC 200D 2640                                  ; minimally-qualified # 🧎🏼‍♀ E12.0 woman kneeling: medium-light skin tone
 1F9CE 1F3FD 200D 2640 FE0F                             ; fully-qualified     # 🧎🏽‍♀️ E12.0 woman kneeling: medium skin tone
 1F9CE 1F3FD 200D 2640                                  ; minimally-qualified # 🧎🏽‍♀ E12.0 woman kneeling: medium skin tone
 1F9CE 1F3FE 200D 2640 FE0F                             ; fully-qualified     # 🧎🏾‍♀️ E12.0 woman kneeling: medium-dark skin tone
 1F9CE 1F3FE 200D 2640                                  ; minimally-qualified # 🧎🏾‍♀ E12.0 woman kneeling: medium-dark skin tone
 1F9CE 1F3FF 200D 2640 FE0F                             ; fully-qualified     # 🧎🏿‍♀️ E12.0 woman kneeling: dark skin tone
 1F9CE 1F3FF 200D 2640                                  ; minimally-qualified # 🧎🏿‍♀ E12.0 woman kneeling: dark skin tone
+1F9CE 200D 27A1 FE0F                                   ; fully-qualified     # 🧎‍➡️ E15.1 person kneeling facing right
+1F9CE 200D 27A1                                        ; minimally-qualified # 🧎‍➡ E15.1 person kneeling facing right
+1F9CE 1F3FB 200D 27A1 FE0F                             ; fully-qualified     # 🧎🏻‍➡️ E15.1 person kneeling facing right: light skin tone
+1F9CE 1F3FB 200D 27A1                                  ; minimally-qualified # 🧎🏻‍➡ E15.1 person kneeling facing right: light skin tone
+1F9CE 1F3FC 200D 27A1 FE0F                             ; fully-qualified     # 🧎🏼‍➡️ E15.1 person kneeling facing right: medium-light skin tone
+1F9CE 1F3FC 200D 27A1                                  ; minimally-qualified # 🧎🏼‍➡ E15.1 person kneeling facing right: medium-light skin tone
+1F9CE 1F3FD 200D 27A1 FE0F                             ; fully-qualified     # 🧎🏽‍➡️ E15.1 person kneeling facing right: medium skin tone
+1F9CE 1F3FD 200D 27A1                                  ; minimally-qualified # 🧎🏽‍➡ E15.1 person kneeling facing right: medium skin tone
+1F9CE 1F3FE 200D 27A1 FE0F                             ; fully-qualified     # 🧎🏾‍➡️ E15.1 person kneeling facing right: medium-dark skin tone
+1F9CE 1F3FE 200D 27A1                                  ; minimally-qualified # 🧎🏾‍➡ E15.1 person kneeling facing right: medium-dark skin tone
+1F9CE 1F3FF 200D 27A1 FE0F                             ; fully-qualified     # 🧎🏿‍➡️ E15.1 person kneeling facing right: dark skin tone
+1F9CE 1F3FF 200D 27A1                                  ; minimally-qualified # 🧎🏿‍➡ E15.1 person kneeling facing right: dark skin tone
+1F9CE 200D 2640 FE0F 200D 27A1 FE0F                    ; fully-qualified     # 🧎‍♀️‍➡️ E15.1 woman kneeling facing right
+1F9CE 200D 2640 200D 27A1 FE0F                         ; minimally-qualified # 🧎‍♀‍➡️ E15.1 woman kneeling facing right
+1F9CE 200D 2640 FE0F 200D 27A1                         ; minimally-qualified # 🧎‍♀️‍➡ E15.1 woman kneeling facing right
+1F9CE 200D 2640 200D 27A1                              ; minimally-qualified # 🧎‍♀‍➡ E15.1 woman kneeling facing right
+1F9CE 1F3FB 200D 2640 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🧎🏻‍♀️‍➡️ E15.1 woman kneeling facing right: light skin tone
+1F9CE 1F3FB 200D 2640 200D 27A1 FE0F                   ; minimally-qualified # 🧎🏻‍♀‍➡️ E15.1 woman kneeling facing right: light skin tone
+1F9CE 1F3FB 200D 2640 FE0F 200D 27A1                   ; minimally-qualified # 🧎🏻‍♀️‍➡ E15.1 woman kneeling facing right: light skin tone
+1F9CE 1F3FB 200D 2640 200D 27A1                        ; minimally-qualified # 🧎🏻‍♀‍➡ E15.1 woman kneeling facing right: light skin tone
+1F9CE 1F3FC 200D 2640 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🧎🏼‍♀️‍➡️ E15.1 woman kneeling facing right: medium-light skin tone
+1F9CE 1F3FC 200D 2640 200D 27A1 FE0F                   ; minimally-qualified # 🧎🏼‍♀‍➡️ E15.1 woman kneeling facing right: medium-light skin tone
+1F9CE 1F3FC 200D 2640 FE0F 200D 27A1                   ; minimally-qualified # 🧎🏼‍♀️‍➡ E15.1 woman kneeling facing right: medium-light skin tone
+1F9CE 1F3FC 200D 2640 200D 27A1                        ; minimally-qualified # 🧎🏼‍♀‍➡ E15.1 woman kneeling facing right: medium-light skin tone
+1F9CE 1F3FD 200D 2640 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🧎🏽‍♀️‍➡️ E15.1 woman kneeling facing right: medium skin tone
+1F9CE 1F3FD 200D 2640 200D 27A1 FE0F                   ; minimally-qualified # 🧎🏽‍♀‍➡️ E15.1 woman kneeling facing right: medium skin tone
+1F9CE 1F3FD 200D 2640 FE0F 200D 27A1                   ; minimally-qualified # 🧎🏽‍♀️‍➡ E15.1 woman kneeling facing right: medium skin tone
+1F9CE 1F3FD 200D 2640 200D 27A1                        ; minimally-qualified # 🧎🏽‍♀‍➡ E15.1 woman kneeling facing right: medium skin tone
+1F9CE 1F3FE 200D 2640 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🧎🏾‍♀️‍➡️ E15.1 woman kneeling facing right: medium-dark skin tone
+1F9CE 1F3FE 200D 2640 200D 27A1 FE0F                   ; minimally-qualified # 🧎🏾‍♀‍➡️ E15.1 woman kneeling facing right: medium-dark skin tone
+1F9CE 1F3FE 200D 2640 FE0F 200D 27A1                   ; minimally-qualified # 🧎🏾‍♀️‍➡ E15.1 woman kneeling facing right: medium-dark skin tone
+1F9CE 1F3FE 200D 2640 200D 27A1                        ; minimally-qualified # 🧎🏾‍♀‍➡ E15.1 woman kneeling facing right: medium-dark skin tone
+1F9CE 1F3FF 200D 2640 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🧎🏿‍♀️‍➡️ E15.1 woman kneeling facing right: dark skin tone
+1F9CE 1F3FF 200D 2640 200D 27A1 FE0F                   ; minimally-qualified # 🧎🏿‍♀‍➡️ E15.1 woman kneeling facing right: dark skin tone
+1F9CE 1F3FF 200D 2640 FE0F 200D 27A1                   ; minimally-qualified # 🧎🏿‍♀️‍➡ E15.1 woman kneeling facing right: dark skin tone
+1F9CE 1F3FF 200D 2640 200D 27A1                        ; minimally-qualified # 🧎🏿‍♀‍➡ E15.1 woman kneeling facing right: dark skin tone
+1F9CE 200D 2642 FE0F 200D 27A1 FE0F                    ; fully-qualified     # 🧎‍♂️‍➡️ E15.1 man kneeling facing right
+1F9CE 200D 2642 200D 27A1 FE0F                         ; minimally-qualified # 🧎‍♂‍➡️ E15.1 man kneeling facing right
+1F9CE 200D 2642 FE0F 200D 27A1                         ; minimally-qualified # 🧎‍♂️‍➡ E15.1 man kneeling facing right
+1F9CE 200D 2642 200D 27A1                              ; minimally-qualified # 🧎‍♂‍➡ E15.1 man kneeling facing right
+1F9CE 1F3FB 200D 2642 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🧎🏻‍♂️‍➡️ E15.1 man kneeling facing right: light skin tone
+1F9CE 1F3FB 200D 2642 200D 27A1 FE0F                   ; minimally-qualified # 🧎🏻‍♂‍➡️ E15.1 man kneeling facing right: light skin tone
+1F9CE 1F3FB 200D 2642 FE0F 200D 27A1                   ; minimally-qualified # 🧎🏻‍♂️‍➡ E15.1 man kneeling facing right: light skin tone
+1F9CE 1F3FB 200D 2642 200D 27A1                        ; minimally-qualified # 🧎🏻‍♂‍➡ E15.1 man kneeling facing right: light skin tone
+1F9CE 1F3FC 200D 2642 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🧎🏼‍♂️‍➡️ E15.1 man kneeling facing right: medium-light skin tone
+1F9CE 1F3FC 200D 2642 200D 27A1 FE0F                   ; minimally-qualified # 🧎🏼‍♂‍➡️ E15.1 man kneeling facing right: medium-light skin tone
+1F9CE 1F3FC 200D 2642 FE0F 200D 27A1                   ; minimally-qualified # 🧎🏼‍♂️‍➡ E15.1 man kneeling facing right: medium-light skin tone
+1F9CE 1F3FC 200D 2642 200D 27A1                        ; minimally-qualified # 🧎🏼‍♂‍➡ E15.1 man kneeling facing right: medium-light skin tone
+1F9CE 1F3FD 200D 2642 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🧎🏽‍♂️‍➡️ E15.1 man kneeling facing right: medium skin tone
+1F9CE 1F3FD 200D 2642 200D 27A1 FE0F                   ; minimally-qualified # 🧎🏽‍♂‍➡️ E15.1 man kneeling facing right: medium skin tone
+1F9CE 1F3FD 200D 2642 FE0F 200D 27A1                   ; minimally-qualified # 🧎🏽‍♂️‍➡ E15.1 man kneeling facing right: medium skin tone
+1F9CE 1F3FD 200D 2642 200D 27A1                        ; minimally-qualified # 🧎🏽‍♂‍➡ E15.1 man kneeling facing right: medium skin tone
+1F9CE 1F3FE 200D 2642 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🧎🏾‍♂️‍➡️ E15.1 man kneeling facing right: medium-dark skin tone
+1F9CE 1F3FE 200D 2642 200D 27A1 FE0F                   ; minimally-qualified # 🧎🏾‍♂‍➡️ E15.1 man kneeling facing right: medium-dark skin tone
+1F9CE 1F3FE 200D 2642 FE0F 200D 27A1                   ; minimally-qualified # 🧎🏾‍♂️‍➡ E15.1 man kneeling facing right: medium-dark skin tone
+1F9CE 1F3FE 200D 2642 200D 27A1                        ; minimally-qualified # 🧎🏾‍♂‍➡ E15.1 man kneeling facing right: medium-dark skin tone
+1F9CE 1F3FF 200D 2642 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🧎🏿‍♂️‍➡️ E15.1 man kneeling facing right: dark skin tone
+1F9CE 1F3FF 200D 2642 200D 27A1 FE0F                   ; minimally-qualified # 🧎🏿‍♂‍➡️ E15.1 man kneeling facing right: dark skin tone
+1F9CE 1F3FF 200D 2642 FE0F 200D 27A1                   ; minimally-qualified # 🧎🏿‍♂️‍➡ E15.1 man kneeling facing right: dark skin tone
+1F9CE 1F3FF 200D 2642 200D 27A1                        ; minimally-qualified # 🧎🏿‍♂‍➡ E15.1 man kneeling facing right: dark skin tone
 1F9D1 200D 1F9AF                                       ; fully-qualified     # 🧑‍🦯 E12.1 person with white cane
 1F9D1 1F3FB 200D 1F9AF                                 ; fully-qualified     # 🧑🏻‍🦯 E12.1 person with white cane: light skin tone
 1F9D1 1F3FC 200D 1F9AF                                 ; fully-qualified     # 🧑🏼‍🦯 E12.1 person with white cane: medium-light skin tone
 1F9D1 1F3FD 200D 1F9AF                                 ; fully-qualified     # 🧑🏽‍🦯 E12.1 person with white cane: medium skin tone
 1F9D1 1F3FE 200D 1F9AF                                 ; fully-qualified     # 🧑🏾‍🦯 E12.1 person with white cane: medium-dark skin tone
 1F9D1 1F3FF 200D 1F9AF                                 ; fully-qualified     # 🧑🏿‍🦯 E12.1 person with white cane: dark skin tone
+1F9D1 200D 1F9AF 200D 27A1 FE0F                        ; fully-qualified     # 🧑‍🦯‍➡️ E15.1 person with white cane facing right
+1F9D1 200D 1F9AF 200D 27A1                             ; minimally-qualified # 🧑‍🦯‍➡ E15.1 person with white cane facing right
+1F9D1 1F3FB 200D 1F9AF 200D 27A1 FE0F                  ; fully-qualified     # 🧑🏻‍🦯‍➡️ E15.1 person with white cane facing right: light skin tone
+1F9D1 1F3FB 200D 1F9AF 200D 27A1                       ; minimally-qualified # 🧑🏻‍🦯‍➡ E15.1 person with white cane facing right: light skin tone
+1F9D1 1F3FC 200D 1F9AF 200D 27A1 FE0F                  ; fully-qualified     # 🧑🏼‍🦯‍➡️ E15.1 person with white cane facing right: medium-light skin tone
+1F9D1 1F3FC 200D 1F9AF 200D 27A1                       ; minimally-qualified # 🧑🏼‍🦯‍➡ E15.1 person with white cane facing right: medium-light skin tone
+1F9D1 1F3FD 200D 1F9AF 200D 27A1 FE0F                  ; fully-qualified     # 🧑🏽‍🦯‍➡️ E15.1 person with white cane facing right: medium skin tone
+1F9D1 1F3FD 200D 1F9AF 200D 27A1                       ; minimally-qualified # 🧑🏽‍🦯‍➡ E15.1 person with white cane facing right: medium skin tone
+1F9D1 1F3FE 200D 1F9AF 200D 27A1 FE0F                  ; fully-qualified     # 🧑🏾‍🦯‍➡️ E15.1 person with white cane facing right: medium-dark skin tone
+1F9D1 1F3FE 200D 1F9AF 200D 27A1                       ; minimally-qualified # 🧑🏾‍🦯‍➡ E15.1 person with white cane facing right: medium-dark skin tone
+1F9D1 1F3FF 200D 1F9AF 200D 27A1 FE0F                  ; fully-qualified     # 🧑🏿‍🦯‍➡️ E15.1 person with white cane facing right: dark skin tone
+1F9D1 1F3FF 200D 1F9AF 200D 27A1                       ; minimally-qualified # 🧑🏿‍🦯‍➡ E15.1 person with white cane facing right: dark skin tone
 1F468 200D 1F9AF                                       ; fully-qualified     # 👨‍🦯 E12.0 man with white cane
 1F468 1F3FB 200D 1F9AF                                 ; fully-qualified     # 👨🏻‍🦯 E12.0 man with white cane: light skin tone
 1F468 1F3FC 200D 1F9AF                                 ; fully-qualified     # 👨🏼‍🦯 E12.0 man with white cane: medium-light skin tone
 1F468 1F3FD 200D 1F9AF                                 ; fully-qualified     # 👨🏽‍🦯 E12.0 man with white cane: medium skin tone
 1F468 1F3FE 200D 1F9AF                                 ; fully-qualified     # 👨🏾‍🦯 E12.0 man with white cane: medium-dark skin tone
 1F468 1F3FF 200D 1F9AF                                 ; fully-qualified     # 👨🏿‍🦯 E12.0 man with white cane: dark skin tone
+1F468 200D 1F9AF 200D 27A1 FE0F                        ; fully-qualified     # 👨‍🦯‍➡️ E15.1 man with white cane facing right
+1F468 200D 1F9AF 200D 27A1                             ; minimally-qualified # 👨‍🦯‍➡ E15.1 man with white cane facing right
+1F468 1F3FB 200D 1F9AF 200D 27A1 FE0F                  ; fully-qualified     # 👨🏻‍🦯‍➡️ E15.1 man with white cane facing right: light skin tone
+1F468 1F3FB 200D 1F9AF 200D 27A1                       ; minimally-qualified # 👨🏻‍🦯‍➡ E15.1 man with white cane facing right: light skin tone
+1F468 1F3FC 200D 1F9AF 200D 27A1 FE0F                  ; fully-qualified     # 👨🏼‍🦯‍➡️ E15.1 man with white cane facing right: medium-light skin tone
+1F468 1F3FC 200D 1F9AF 200D 27A1                       ; minimally-qualified # 👨🏼‍🦯‍➡ E15.1 man with white cane facing right: medium-light skin tone
+1F468 1F3FD 200D 1F9AF 200D 27A1 FE0F                  ; fully-qualified     # 👨🏽‍🦯‍➡️ E15.1 man with white cane facing right: medium skin tone
+1F468 1F3FD 200D 1F9AF 200D 27A1                       ; minimally-qualified # 👨🏽‍🦯‍➡ E15.1 man with white cane facing right: medium skin tone
+1F468 1F3FE 200D 1F9AF 200D 27A1 FE0F                  ; fully-qualified     # 👨🏾‍🦯‍➡️ E15.1 man with white cane facing right: medium-dark skin tone
+1F468 1F3FE 200D 1F9AF 200D 27A1                       ; minimally-qualified # 👨🏾‍🦯‍➡ E15.1 man with white cane facing right: medium-dark skin tone
+1F468 1F3FF 200D 1F9AF 200D 27A1 FE0F                  ; fully-qualified     # 👨🏿‍🦯‍➡️ E15.1 man with white cane facing right: dark skin tone
+1F468 1F3FF 200D 1F9AF 200D 27A1                       ; minimally-qualified # 👨🏿‍🦯‍➡ E15.1 man with white cane facing right: dark skin tone
 1F469 200D 1F9AF                                       ; fully-qualified     # 👩‍🦯 E12.0 woman with white cane
 1F469 1F3FB 200D 1F9AF                                 ; fully-qualified     # 👩🏻‍🦯 E12.0 woman with white cane: light skin tone
 1F469 1F3FC 200D 1F9AF                                 ; fully-qualified     # 👩🏼‍🦯 E12.0 woman with white cane: medium-light skin tone
 1F469 1F3FD 200D 1F9AF                                 ; fully-qualified     # 👩🏽‍🦯 E12.0 woman with white cane: medium skin tone
 1F469 1F3FE 200D 1F9AF                                 ; fully-qualified     # 👩🏾‍🦯 E12.0 woman with white cane: medium-dark skin tone
 1F469 1F3FF 200D 1F9AF                                 ; fully-qualified     # 👩🏿‍🦯 E12.0 woman with white cane: dark skin tone
+1F469 200D 1F9AF 200D 27A1 FE0F                        ; fully-qualified     # 👩‍🦯‍➡️ E15.1 woman with white cane facing right
+1F469 200D 1F9AF 200D 27A1                             ; minimally-qualified # 👩‍🦯‍➡ E15.1 woman with white cane facing right
+1F469 1F3FB 200D 1F9AF 200D 27A1 FE0F                  ; fully-qualified     # 👩🏻‍🦯‍➡️ E15.1 woman with white cane facing right: light skin tone
+1F469 1F3FB 200D 1F9AF 200D 27A1                       ; minimally-qualified # 👩🏻‍🦯‍➡ E15.1 woman with white cane facing right: light skin tone
+1F469 1F3FC 200D 1F9AF 200D 27A1 FE0F                  ; fully-qualified     # 👩🏼‍🦯‍➡️ E15.1 woman with white cane facing right: medium-light skin tone
+1F469 1F3FC 200D 1F9AF 200D 27A1                       ; minimally-qualified # 👩🏼‍🦯‍➡ E15.1 woman with white cane facing right: medium-light skin tone
+1F469 1F3FD 200D 1F9AF 200D 27A1 FE0F                  ; fully-qualified     # 👩🏽‍🦯‍➡️ E15.1 woman with white cane facing right: medium skin tone
+1F469 1F3FD 200D 1F9AF 200D 27A1                       ; minimally-qualified # 👩🏽‍🦯‍➡ E15.1 woman with white cane facing right: medium skin tone
+1F469 1F3FE 200D 1F9AF 200D 27A1 FE0F                  ; fully-qualified     # 👩🏾‍🦯‍➡️ E15.1 woman with white cane facing right: medium-dark skin tone
+1F469 1F3FE 200D 1F9AF 200D 27A1                       ; minimally-qualified # 👩🏾‍🦯‍➡ E15.1 woman with white cane facing right: medium-dark skin tone
+1F469 1F3FF 200D 1F9AF 200D 27A1 FE0F                  ; fully-qualified     # 👩🏿‍🦯‍➡️ E15.1 woman with white cane facing right: dark skin tone
+1F469 1F3FF 200D 1F9AF 200D 27A1                       ; minimally-qualified # 👩🏿‍🦯‍➡ E15.1 woman with white cane facing right: dark skin tone
 1F9D1 200D 1F9BC                                       ; fully-qualified     # 🧑‍🦼 E12.1 person in motorized wheelchair
 1F9D1 1F3FB 200D 1F9BC                                 ; fully-qualified     # 🧑🏻‍🦼 E12.1 person in motorized wheelchair: light skin tone
 1F9D1 1F3FC 200D 1F9BC                                 ; fully-qualified     # 🧑🏼‍🦼 E12.1 person in motorized wheelchair: medium-light skin tone
 1F9D1 1F3FD 200D 1F9BC                                 ; fully-qualified     # 🧑🏽‍🦼 E12.1 person in motorized wheelchair: medium skin tone
 1F9D1 1F3FE 200D 1F9BC                                 ; fully-qualified     # 🧑🏾‍🦼 E12.1 person in motorized wheelchair: medium-dark skin tone
 1F9D1 1F3FF 200D 1F9BC                                 ; fully-qualified     # 🧑🏿‍🦼 E12.1 person in motorized wheelchair: dark skin tone
+1F9D1 200D 1F9BC 200D 27A1 FE0F                        ; fully-qualified     # 🧑‍🦼‍➡️ E15.1 person in motorized wheelchair facing right
+1F9D1 200D 1F9BC 200D 27A1                             ; minimally-qualified # 🧑‍🦼‍➡ E15.1 person in motorized wheelchair facing right
+1F9D1 1F3FB 200D 1F9BC 200D 27A1 FE0F                  ; fully-qualified     # 🧑🏻‍🦼‍➡️ E15.1 person in motorized wheelchair facing right: light skin tone
+1F9D1 1F3FB 200D 1F9BC 200D 27A1                       ; minimally-qualified # 🧑🏻‍🦼‍➡ E15.1 person in motorized wheelchair facing right: light skin tone
+1F9D1 1F3FC 200D 1F9BC 200D 27A1 FE0F                  ; fully-qualified     # 🧑🏼‍🦼‍➡️ E15.1 person in motorized wheelchair facing right: medium-light skin tone
+1F9D1 1F3FC 200D 1F9BC 200D 27A1                       ; minimally-qualified # 🧑🏼‍🦼‍➡ E15.1 person in motorized wheelchair facing right: medium-light skin tone
+1F9D1 1F3FD 200D 1F9BC 200D 27A1 FE0F                  ; fully-qualified     # 🧑🏽‍🦼‍➡️ E15.1 person in motorized wheelchair facing right: medium skin tone
+1F9D1 1F3FD 200D 1F9BC 200D 27A1                       ; minimally-qualified # 🧑🏽‍🦼‍➡ E15.1 person in motorized wheelchair facing right: medium skin tone
+1F9D1 1F3FE 200D 1F9BC 200D 27A1 FE0F                  ; fully-qualified     # 🧑🏾‍🦼‍➡️ E15.1 person in motorized wheelchair facing right: medium-dark skin tone
+1F9D1 1F3FE 200D 1F9BC 200D 27A1                       ; minimally-qualified # 🧑🏾‍🦼‍➡ E15.1 person in motorized wheelchair facing right: medium-dark skin tone
+1F9D1 1F3FF 200D 1F9BC 200D 27A1 FE0F                  ; fully-qualified     # 🧑🏿‍🦼‍➡️ E15.1 person in motorized wheelchair facing right: dark skin tone
+1F9D1 1F3FF 200D 1F9BC 200D 27A1                       ; minimally-qualified # 🧑🏿‍🦼‍➡ E15.1 person in motorized wheelchair facing right: dark skin tone
 1F468 200D 1F9BC                                       ; fully-qualified     # 👨‍🦼 E12.0 man in motorized wheelchair
 1F468 1F3FB 200D 1F9BC                                 ; fully-qualified     # 👨🏻‍🦼 E12.0 man in motorized wheelchair: light skin tone
 1F468 1F3FC 200D 1F9BC                                 ; fully-qualified     # 👨🏼‍🦼 E12.0 man in motorized wheelchair: medium-light skin tone
 1F468 1F3FD 200D 1F9BC                                 ; fully-qualified     # 👨🏽‍🦼 E12.0 man in motorized wheelchair: medium skin tone
 1F468 1F3FE 200D 1F9BC                                 ; fully-qualified     # 👨🏾‍🦼 E12.0 man in motorized wheelchair: medium-dark skin tone
 1F468 1F3FF 200D 1F9BC                                 ; fully-qualified     # 👨🏿‍🦼 E12.0 man in motorized wheelchair: dark skin tone
+1F468 200D 1F9BC 200D 27A1 FE0F                        ; fully-qualified     # 👨‍🦼‍➡️ E15.1 man in motorized wheelchair facing right
+1F468 200D 1F9BC 200D 27A1                             ; minimally-qualified # 👨‍🦼‍➡ E15.1 man in motorized wheelchair facing right
+1F468 1F3FB 200D 1F9BC 200D 27A1 FE0F                  ; fully-qualified     # 👨🏻‍🦼‍➡️ E15.1 man in motorized wheelchair facing right: light skin tone
+1F468 1F3FB 200D 1F9BC 200D 27A1                       ; minimally-qualified # 👨🏻‍🦼‍➡ E15.1 man in motorized wheelchair facing right: light skin tone
+1F468 1F3FC 200D 1F9BC 200D 27A1 FE0F                  ; fully-qualified     # 👨🏼‍🦼‍➡️ E15.1 man in motorized wheelchair facing right: medium-light skin tone
+1F468 1F3FC 200D 1F9BC 200D 27A1                       ; minimally-qualified # 👨🏼‍🦼‍➡ E15.1 man in motorized wheelchair facing right: medium-light skin tone
+1F468 1F3FD 200D 1F9BC 200D 27A1 FE0F                  ; fully-qualified     # 👨🏽‍🦼‍➡️ E15.1 man in motorized wheelchair facing right: medium skin tone
+1F468 1F3FD 200D 1F9BC 200D 27A1                       ; minimally-qualified # 👨🏽‍🦼‍➡ E15.1 man in motorized wheelchair facing right: medium skin tone
+1F468 1F3FE 200D 1F9BC 200D 27A1 FE0F                  ; fully-qualified     # 👨🏾‍🦼‍➡️ E15.1 man in motorized wheelchair facing right: medium-dark skin tone
+1F468 1F3FE 200D 1F9BC 200D 27A1                       ; minimally-qualified # 👨🏾‍🦼‍➡ E15.1 man in motorized wheelchair facing right: medium-dark skin tone
+1F468 1F3FF 200D 1F9BC 200D 27A1 FE0F                  ; fully-qualified     # 👨🏿‍🦼‍➡️ E15.1 man in motorized wheelchair facing right: dark skin tone
+1F468 1F3FF 200D 1F9BC 200D 27A1                       ; minimally-qualified # 👨🏿‍🦼‍➡ E15.1 man in motorized wheelchair facing right: dark skin tone
 1F469 200D 1F9BC                                       ; fully-qualified     # 👩‍🦼 E12.0 woman in motorized wheelchair
 1F469 1F3FB 200D 1F9BC                                 ; fully-qualified     # 👩🏻‍🦼 E12.0 woman in motorized wheelchair: light skin tone
 1F469 1F3FC 200D 1F9BC                                 ; fully-qualified     # 👩🏼‍🦼 E12.0 woman in motorized wheelchair: medium-light skin tone
 1F469 1F3FD 200D 1F9BC                                 ; fully-qualified     # 👩🏽‍🦼 E12.0 woman in motorized wheelchair: medium skin tone
 1F469 1F3FE 200D 1F9BC                                 ; fully-qualified     # 👩🏾‍🦼 E12.0 woman in motorized wheelchair: medium-dark skin tone
 1F469 1F3FF 200D 1F9BC                                 ; fully-qualified     # 👩🏿‍🦼 E12.0 woman in motorized wheelchair: dark skin tone
+1F469 200D 1F9BC 200D 27A1 FE0F                        ; fully-qualified     # 👩‍🦼‍➡️ E15.1 woman in motorized wheelchair facing right
+1F469 200D 1F9BC 200D 27A1                             ; minimally-qualified # 👩‍🦼‍➡ E15.1 woman in motorized wheelchair facing right
+1F469 1F3FB 200D 1F9BC 200D 27A1 FE0F                  ; fully-qualified     # 👩🏻‍🦼‍➡️ E15.1 woman in motorized wheelchair facing right: light skin tone
+1F469 1F3FB 200D 1F9BC 200D 27A1                       ; minimally-qualified # 👩🏻‍🦼‍➡ E15.1 woman in motorized wheelchair facing right: light skin tone
+1F469 1F3FC 200D 1F9BC 200D 27A1 FE0F                  ; fully-qualified     # 👩🏼‍🦼‍➡️ E15.1 woman in motorized wheelchair facing right: medium-light skin tone
+1F469 1F3FC 200D 1F9BC 200D 27A1                       ; minimally-qualified # 👩🏼‍🦼‍➡ E15.1 woman in motorized wheelchair facing right: medium-light skin tone
+1F469 1F3FD 200D 1F9BC 200D 27A1 FE0F                  ; fully-qualified     # 👩🏽‍🦼‍➡️ E15.1 woman in motorized wheelchair facing right: medium skin tone
+1F469 1F3FD 200D 1F9BC 200D 27A1                       ; minimally-qualified # 👩🏽‍🦼‍➡ E15.1 woman in motorized wheelchair facing right: medium skin tone
+1F469 1F3FE 200D 1F9BC 200D 27A1 FE0F                  ; fully-qualified     # 👩🏾‍🦼‍➡️ E15.1 woman in motorized wheelchair facing right: medium-dark skin tone
+1F469 1F3FE 200D 1F9BC 200D 27A1                       ; minimally-qualified # 👩🏾‍🦼‍➡ E15.1 woman in motorized wheelchair facing right: medium-dark skin tone
+1F469 1F3FF 200D 1F9BC 200D 27A1 FE0F                  ; fully-qualified     # 👩🏿‍🦼‍➡️ E15.1 woman in motorized wheelchair facing right: dark skin tone
+1F469 1F3FF 200D 1F9BC 200D 27A1                       ; minimally-qualified # 👩🏿‍🦼‍➡ E15.1 woman in motorized wheelchair facing right: dark skin tone
 1F9D1 200D 1F9BD                                       ; fully-qualified     # 🧑‍🦽 E12.1 person in manual wheelchair
 1F9D1 1F3FB 200D 1F9BD                                 ; fully-qualified     # 🧑🏻‍🦽 E12.1 person in manual wheelchair: light skin tone
 1F9D1 1F3FC 200D 1F9BD                                 ; fully-qualified     # 🧑🏼‍🦽 E12.1 person in manual wheelchair: medium-light skin tone
 1F9D1 1F3FD 200D 1F9BD                                 ; fully-qualified     # 🧑🏽‍🦽 E12.1 person in manual wheelchair: medium skin tone
 1F9D1 1F3FE 200D 1F9BD                                 ; fully-qualified     # 🧑🏾‍🦽 E12.1 person in manual wheelchair: medium-dark skin tone
 1F9D1 1F3FF 200D 1F9BD                                 ; fully-qualified     # 🧑🏿‍🦽 E12.1 person in manual wheelchair: dark skin tone
+1F9D1 200D 1F9BD 200D 27A1 FE0F                        ; fully-qualified     # 🧑‍🦽‍➡️ E15.1 person in manual wheelchair facing right
+1F9D1 200D 1F9BD 200D 27A1                             ; minimally-qualified # 🧑‍🦽‍➡ E15.1 person in manual wheelchair facing right
+1F9D1 1F3FB 200D 1F9BD 200D 27A1 FE0F                  ; fully-qualified     # 🧑🏻‍🦽‍➡️ E15.1 person in manual wheelchair facing right: light skin tone
+1F9D1 1F3FB 200D 1F9BD 200D 27A1                       ; minimally-qualified # 🧑🏻‍🦽‍➡ E15.1 person in manual wheelchair facing right: light skin tone
+1F9D1 1F3FC 200D 1F9BD 200D 27A1 FE0F                  ; fully-qualified     # 🧑🏼‍🦽‍➡️ E15.1 person in manual wheelchair facing right: medium-light skin tone
+1F9D1 1F3FC 200D 1F9BD 200D 27A1                       ; minimally-qualified # 🧑🏼‍🦽‍➡ E15.1 person in manual wheelchair facing right: medium-light skin tone
+1F9D1 1F3FD 200D 1F9BD 200D 27A1 FE0F                  ; fully-qualified     # 🧑🏽‍🦽‍➡️ E15.1 person in manual wheelchair facing right: medium skin tone
+1F9D1 1F3FD 200D 1F9BD 200D 27A1                       ; minimally-qualified # 🧑🏽‍🦽‍➡ E15.1 person in manual wheelchair facing right: medium skin tone
+1F9D1 1F3FE 200D 1F9BD 200D 27A1 FE0F                  ; fully-qualified     # 🧑🏾‍🦽‍➡️ E15.1 person in manual wheelchair facing right: medium-dark skin tone
+1F9D1 1F3FE 200D 1F9BD 200D 27A1                       ; minimally-qualified # 🧑🏾‍🦽‍➡ E15.1 person in manual wheelchair facing right: medium-dark skin tone
+1F9D1 1F3FF 200D 1F9BD 200D 27A1 FE0F                  ; fully-qualified     # 🧑🏿‍🦽‍➡️ E15.1 person in manual wheelchair facing right: dark skin tone
+1F9D1 1F3FF 200D 1F9BD 200D 27A1                       ; minimally-qualified # 🧑🏿‍🦽‍➡ E15.1 person in manual wheelchair facing right: dark skin tone
 1F468 200D 1F9BD                                       ; fully-qualified     # 👨‍🦽 E12.0 man in manual wheelchair
 1F468 1F3FB 200D 1F9BD                                 ; fully-qualified     # 👨🏻‍🦽 E12.0 man in manual wheelchair: light skin tone
 1F468 1F3FC 200D 1F9BD                                 ; fully-qualified     # 👨🏼‍🦽 E12.0 man in manual wheelchair: medium-light skin tone
 1F468 1F3FD 200D 1F9BD                                 ; fully-qualified     # 👨🏽‍🦽 E12.0 man in manual wheelchair: medium skin tone
 1F468 1F3FE 200D 1F9BD                                 ; fully-qualified     # 👨🏾‍🦽 E12.0 man in manual wheelchair: medium-dark skin tone
 1F468 1F3FF 200D 1F9BD                                 ; fully-qualified     # 👨🏿‍🦽 E12.0 man in manual wheelchair: dark skin tone
+1F468 200D 1F9BD 200D 27A1 FE0F                        ; fully-qualified     # 👨‍🦽‍➡️ E15.1 man in manual wheelchair facing right
+1F468 200D 1F9BD 200D 27A1                             ; minimally-qualified # 👨‍🦽‍➡ E15.1 man in manual wheelchair facing right
+1F468 1F3FB 200D 1F9BD 200D 27A1 FE0F                  ; fully-qualified     # 👨🏻‍🦽‍➡️ E15.1 man in manual wheelchair facing right: light skin tone
+1F468 1F3FB 200D 1F9BD 200D 27A1                       ; minimally-qualified # 👨🏻‍🦽‍➡ E15.1 man in manual wheelchair facing right: light skin tone
+1F468 1F3FC 200D 1F9BD 200D 27A1 FE0F                  ; fully-qualified     # 👨🏼‍🦽‍➡️ E15.1 man in manual wheelchair facing right: medium-light skin tone
+1F468 1F3FC 200D 1F9BD 200D 27A1                       ; minimally-qualified # 👨🏼‍🦽‍➡ E15.1 man in manual wheelchair facing right: medium-light skin tone
+1F468 1F3FD 200D 1F9BD 200D 27A1 FE0F                  ; fully-qualified     # 👨🏽‍🦽‍➡️ E15.1 man in manual wheelchair facing right: medium skin tone
+1F468 1F3FD 200D 1F9BD 200D 27A1                       ; minimally-qualified # 👨🏽‍🦽‍➡ E15.1 man in manual wheelchair facing right: medium skin tone
+1F468 1F3FE 200D 1F9BD 200D 27A1 FE0F                  ; fully-qualified     # 👨🏾‍🦽‍➡️ E15.1 man in manual wheelchair facing right: medium-dark skin tone
+1F468 1F3FE 200D 1F9BD 200D 27A1                       ; minimally-qualified # 👨🏾‍🦽‍➡ E15.1 man in manual wheelchair facing right: medium-dark skin tone
+1F468 1F3FF 200D 1F9BD 200D 27A1 FE0F                  ; fully-qualified     # 👨🏿‍🦽‍➡️ E15.1 man in manual wheelchair facing right: dark skin tone
+1F468 1F3FF 200D 1F9BD 200D 27A1                       ; minimally-qualified # 👨🏿‍🦽‍➡ E15.1 man in manual wheelchair facing right: dark skin tone
 1F469 200D 1F9BD                                       ; fully-qualified     # 👩‍🦽 E12.0 woman in manual wheelchair
 1F469 1F3FB 200D 1F9BD                                 ; fully-qualified     # 👩🏻‍🦽 E12.0 woman in manual wheelchair: light skin tone
 1F469 1F3FC 200D 1F9BD                                 ; fully-qualified     # 👩🏼‍🦽 E12.0 woman in manual wheelchair: medium-light skin tone
 1F469 1F3FD 200D 1F9BD                                 ; fully-qualified     # 👩🏽‍🦽 E12.0 woman in manual wheelchair: medium skin tone
 1F469 1F3FE 200D 1F9BD                                 ; fully-qualified     # 👩🏾‍🦽 E12.0 woman in manual wheelchair: medium-dark skin tone
 1F469 1F3FF 200D 1F9BD                                 ; fully-qualified     # 👩🏿‍🦽 E12.0 woman in manual wheelchair: dark skin tone
+1F469 200D 1F9BD 200D 27A1 FE0F                        ; fully-qualified     # 👩‍🦽‍➡️ E15.1 woman in manual wheelchair facing right
+1F469 200D 1F9BD 200D 27A1                             ; minimally-qualified # 👩‍🦽‍➡ E15.1 woman in manual wheelchair facing right
+1F469 1F3FB 200D 1F9BD 200D 27A1 FE0F                  ; fully-qualified     # 👩🏻‍🦽‍➡️ E15.1 woman in manual wheelchair facing right: light skin tone
+1F469 1F3FB 200D 1F9BD 200D 27A1                       ; minimally-qualified # 👩🏻‍🦽‍➡ E15.1 woman in manual wheelchair facing right: light skin tone
+1F469 1F3FC 200D 1F9BD 200D 27A1 FE0F                  ; fully-qualified     # 👩🏼‍🦽‍➡️ E15.1 woman in manual wheelchair facing right: medium-light skin tone
+1F469 1F3FC 200D 1F9BD 200D 27A1                       ; minimally-qualified # 👩🏼‍🦽‍➡ E15.1 woman in manual wheelchair facing right: medium-light skin tone
+1F469 1F3FD 200D 1F9BD 200D 27A1 FE0F                  ; fully-qualified     # 👩🏽‍🦽‍➡️ E15.1 woman in manual wheelchair facing right: medium skin tone
+1F469 1F3FD 200D 1F9BD 200D 27A1                       ; minimally-qualified # 👩🏽‍🦽‍➡ E15.1 woman in manual wheelchair facing right: medium skin tone
+1F469 1F3FE 200D 1F9BD 200D 27A1 FE0F                  ; fully-qualified     # 👩🏾‍🦽‍➡️ E15.1 woman in manual wheelchair facing right: medium-dark skin tone
+1F469 1F3FE 200D 1F9BD 200D 27A1                       ; minimally-qualified # 👩🏾‍🦽‍➡ E15.1 woman in manual wheelchair facing right: medium-dark skin tone
+1F469 1F3FF 200D 1F9BD 200D 27A1 FE0F                  ; fully-qualified     # 👩🏿‍🦽‍➡️ E15.1 woman in manual wheelchair facing right: dark skin tone
+1F469 1F3FF 200D 1F9BD 200D 27A1                       ; minimally-qualified # 👩🏿‍🦽‍➡ E15.1 woman in manual wheelchair facing right: dark skin tone
 1F3C3                                                  ; fully-qualified     # 🏃 E0.6 person running
 1F3C3 1F3FB                                            ; fully-qualified     # 🏃🏻 E1.0 person running: light skin tone
 1F3C3 1F3FC                                            ; fully-qualified     # 🏃🏼 E1.0 person running: medium-light skin tone
 1F3C3 1F3FD                                            ; fully-qualified     # 🏃🏽 E1.0 person running: medium skin tone
 1F3C3 1F3FE                                            ; fully-qualified     # 🏃🏾 E1.0 person running: medium-dark skin tone
 1F3C3 1F3FF                                            ; fully-qualified     # 🏃🏿 E1.0 person running: dark skin tone
 1F3C3 200D 2642 FE0F                                   ; fully-qualified     # 🏃‍♂️ E4.0 man running
@@ -2205,14 +2437,74 @@
 1F3C3 1F3FC 200D 2640                                  ; minimally-qualified # 🏃🏼‍♀ E4.0 woman running: medium-light skin tone
 1F3C3 1F3FD 200D 2640 FE0F                             ; fully-qualified     # 🏃🏽‍♀️ E4.0 woman running: medium skin tone
 1F3C3 1F3FD 200D 2640                                  ; minimally-qualified # 🏃🏽‍♀ E4.0 woman running: medium skin tone
 1F3C3 1F3FE 200D 2640 FE0F                             ; fully-qualified     # 🏃🏾‍♀️ E4.0 woman running: medium-dark skin tone
 1F3C3 1F3FE 200D 2640                                  ; minimally-qualified # 🏃🏾‍♀ E4.0 woman running: medium-dark skin tone
 1F3C3 1F3FF 200D 2640 FE0F                             ; fully-qualified     # 🏃🏿‍♀️ E4.0 woman running: dark skin tone
 1F3C3 1F3FF 200D 2640                                  ; minimally-qualified # 🏃🏿‍♀ E4.0 woman running: dark skin tone
+1F3C3 200D 27A1 FE0F                                   ; fully-qualified     # 🏃‍➡️ E15.1 person running facing right
+1F3C3 200D 27A1                                        ; minimally-qualified # 🏃‍➡ E15.1 person running facing right
+1F3C3 1F3FB 200D 27A1 FE0F                             ; fully-qualified     # 🏃🏻‍➡️ E15.1 person running facing right: light skin tone
+1F3C3 1F3FB 200D 27A1                                  ; minimally-qualified # 🏃🏻‍➡ E15.1 person running facing right: light skin tone
+1F3C3 1F3FC 200D 27A1 FE0F                             ; fully-qualified     # 🏃🏼‍➡️ E15.1 person running facing right: medium-light skin tone
+1F3C3 1F3FC 200D 27A1                                  ; minimally-qualified # 🏃🏼‍➡ E15.1 person running facing right: medium-light skin tone
+1F3C3 1F3FD 200D 27A1 FE0F                             ; fully-qualified     # 🏃🏽‍➡️ E15.1 person running facing right: medium skin tone
+1F3C3 1F3FD 200D 27A1                                  ; minimally-qualified # 🏃🏽‍➡ E15.1 person running facing right: medium skin tone
+1F3C3 1F3FE 200D 27A1 FE0F                             ; fully-qualified     # 🏃🏾‍➡️ E15.1 person running facing right: medium-dark skin tone
+1F3C3 1F3FE 200D 27A1                                  ; minimally-qualified # 🏃🏾‍➡ E15.1 person running facing right: medium-dark skin tone
+1F3C3 1F3FF 200D 27A1 FE0F                             ; fully-qualified     # 🏃🏿‍➡️ E15.1 person running facing right: dark skin tone
+1F3C3 1F3FF 200D 27A1                                  ; minimally-qualified # 🏃🏿‍➡ E15.1 person running facing right: dark skin tone
+1F3C3 200D 2640 FE0F 200D 27A1 FE0F                    ; fully-qualified     # 🏃‍♀️‍➡️ E15.1 woman running facing right
+1F3C3 200D 2640 200D 27A1 FE0F                         ; minimally-qualified # 🏃‍♀‍➡️ E15.1 woman running facing right
+1F3C3 200D 2640 FE0F 200D 27A1                         ; minimally-qualified # 🏃‍♀️‍➡ E15.1 woman running facing right
+1F3C3 200D 2640 200D 27A1                              ; minimally-qualified # 🏃‍♀‍➡ E15.1 woman running facing right
+1F3C3 1F3FB 200D 2640 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🏃🏻‍♀️‍➡️ E15.1 woman running facing right: light skin tone
+1F3C3 1F3FB 200D 2640 200D 27A1 FE0F                   ; minimally-qualified # 🏃🏻‍♀‍➡️ E15.1 woman running facing right: light skin tone
+1F3C3 1F3FB 200D 2640 FE0F 200D 27A1                   ; minimally-qualified # 🏃🏻‍♀️‍➡ E15.1 woman running facing right: light skin tone
+1F3C3 1F3FB 200D 2640 200D 27A1                        ; minimally-qualified # 🏃🏻‍♀‍➡ E15.1 woman running facing right: light skin tone
+1F3C3 1F3FC 200D 2640 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🏃🏼‍♀️‍➡️ E15.1 woman running facing right: medium-light skin tone
+1F3C3 1F3FC 200D 2640 200D 27A1 FE0F                   ; minimally-qualified # 🏃🏼‍♀‍➡️ E15.1 woman running facing right: medium-light skin tone
+1F3C3 1F3FC 200D 2640 FE0F 200D 27A1                   ; minimally-qualified # 🏃🏼‍♀️‍➡ E15.1 woman running facing right: medium-light skin tone
+1F3C3 1F3FC 200D 2640 200D 27A1                        ; minimally-qualified # 🏃🏼‍♀‍➡ E15.1 woman running facing right: medium-light skin tone
+1F3C3 1F3FD 200D 2640 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🏃🏽‍♀️‍➡️ E15.1 woman running facing right: medium skin tone
+1F3C3 1F3FD 200D 2640 200D 27A1 FE0F                   ; minimally-qualified # 🏃🏽‍♀‍➡️ E15.1 woman running facing right: medium skin tone
+1F3C3 1F3FD 200D 2640 FE0F 200D 27A1                   ; minimally-qualified # 🏃🏽‍♀️‍➡ E15.1 woman running facing right: medium skin tone
+1F3C3 1F3FD 200D 2640 200D 27A1                        ; minimally-qualified # 🏃🏽‍♀‍➡ E15.1 woman running facing right: medium skin tone
+1F3C3 1F3FE 200D 2640 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🏃🏾‍♀️‍➡️ E15.1 woman running facing right: medium-dark skin tone
+1F3C3 1F3FE 200D 2640 200D 27A1 FE0F                   ; minimally-qualified # 🏃🏾‍♀‍➡️ E15.1 woman running facing right: medium-dark skin tone
+1F3C3 1F3FE 200D 2640 FE0F 200D 27A1                   ; minimally-qualified # 🏃🏾‍♀️‍➡ E15.1 woman running facing right: medium-dark skin tone
+1F3C3 1F3FE 200D 2640 200D 27A1                        ; minimally-qualified # 🏃🏾‍♀‍➡ E15.1 woman running facing right: medium-dark skin tone
+1F3C3 1F3FF 200D 2640 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🏃🏿‍♀️‍➡️ E15.1 woman running facing right: dark skin tone
+1F3C3 1F3FF 200D 2640 200D 27A1 FE0F                   ; minimally-qualified # 🏃🏿‍♀‍➡️ E15.1 woman running facing right: dark skin tone
+1F3C3 1F3FF 200D 2640 FE0F 200D 27A1                   ; minimally-qualified # 🏃🏿‍♀️‍➡ E15.1 woman running facing right: dark skin tone
+1F3C3 1F3FF 200D 2640 200D 27A1                        ; minimally-qualified # 🏃🏿‍♀‍➡ E15.1 woman running facing right: dark skin tone
+1F3C3 200D 2642 FE0F 200D 27A1 FE0F                    ; fully-qualified     # 🏃‍♂️‍➡️ E15.1 man running facing right
+1F3C3 200D 2642 200D 27A1 FE0F                         ; minimally-qualified # 🏃‍♂‍➡️ E15.1 man running facing right
+1F3C3 200D 2642 FE0F 200D 27A1                         ; minimally-qualified # 🏃‍♂️‍➡ E15.1 man running facing right
+1F3C3 200D 2642 200D 27A1                              ; minimally-qualified # 🏃‍♂‍➡ E15.1 man running facing right
+1F3C3 1F3FB 200D 2642 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🏃🏻‍♂️‍➡️ E15.1 man running facing right: light skin tone
+1F3C3 1F3FB 200D 2642 200D 27A1 FE0F                   ; minimally-qualified # 🏃🏻‍♂‍➡️ E15.1 man running facing right: light skin tone
+1F3C3 1F3FB 200D 2642 FE0F 200D 27A1                   ; minimally-qualified # 🏃🏻‍♂️‍➡ E15.1 man running facing right: light skin tone
+1F3C3 1F3FB 200D 2642 200D 27A1                        ; minimally-qualified # 🏃🏻‍♂‍➡ E15.1 man running facing right: light skin tone
+1F3C3 1F3FC 200D 2642 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🏃🏼‍♂️‍➡️ E15.1 man running facing right: medium-light skin tone
+1F3C3 1F3FC 200D 2642 200D 27A1 FE0F                   ; minimally-qualified # 🏃🏼‍♂‍➡️ E15.1 man running facing right: medium-light skin tone
+1F3C3 1F3FC 200D 2642 FE0F 200D 27A1                   ; minimally-qualified # 🏃🏼‍♂️‍➡ E15.1 man running facing right: medium-light skin tone
+1F3C3 1F3FC 200D 2642 200D 27A1                        ; minimally-qualified # 🏃🏼‍♂‍➡ E15.1 man running facing right: medium-light skin tone
+1F3C3 1F3FD 200D 2642 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🏃🏽‍♂️‍➡️ E15.1 man running facing right: medium skin tone
+1F3C3 1F3FD 200D 2642 200D 27A1 FE0F                   ; minimally-qualified # 🏃🏽‍♂‍➡️ E15.1 man running facing right: medium skin tone
+1F3C3 1F3FD 200D 2642 FE0F 200D 27A1                   ; minimally-qualified # 🏃🏽‍♂️‍➡ E15.1 man running facing right: medium skin tone
+1F3C3 1F3FD 200D 2642 200D 27A1                        ; minimally-qualified # 🏃🏽‍♂‍➡ E15.1 man running facing right: medium skin tone
+1F3C3 1F3FE 200D 2642 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🏃🏾‍♂️‍➡️ E15.1 man running facing right: medium-dark skin tone
+1F3C3 1F3FE 200D 2642 200D 27A1 FE0F                   ; minimally-qualified # 🏃🏾‍♂‍➡️ E15.1 man running facing right: medium-dark skin tone
+1F3C3 1F3FE 200D 2642 FE0F 200D 27A1                   ; minimally-qualified # 🏃🏾‍♂️‍➡ E15.1 man running facing right: medium-dark skin tone
+1F3C3 1F3FE 200D 2642 200D 27A1                        ; minimally-qualified # 🏃🏾‍♂‍➡ E15.1 man running facing right: medium-dark skin tone
+1F3C3 1F3FF 200D 2642 FE0F 200D 27A1 FE0F              ; fully-qualified     # 🏃🏿‍♂️‍➡️ E15.1 man running facing right: dark skin tone
+1F3C3 1F3FF 200D 2642 200D 27A1 FE0F                   ; minimally-qualified # 🏃🏿‍♂‍➡️ E15.1 man running facing right: dark skin tone
+1F3C3 1F3FF 200D 2642 FE0F 200D 27A1                   ; minimally-qualified # 🏃🏿‍♂️‍➡ E15.1 man running facing right: dark skin tone
+1F3C3 1F3FF 200D 2642 200D 27A1                        ; minimally-qualified # 🏃🏿‍♂‍➡ E15.1 man running facing right: dark skin tone
 1F483                                                  ; fully-qualified     # 💃 E0.6 woman dancing
 1F483 1F3FB                                            ; fully-qualified     # 💃🏻 E1.0 woman dancing: light skin tone
 1F483 1F3FC                                            ; fully-qualified     # 💃🏼 E1.0 woman dancing: medium-light skin tone
 1F483 1F3FD                                            ; fully-qualified     # 💃🏽 E1.0 woman dancing: medium skin tone
 1F483 1F3FE                                            ; fully-qualified     # 💃🏾 E1.0 woman dancing: medium-dark skin tone
 1F483 1F3FF                                            ; fully-qualified     # 💃🏿 E1.0 woman dancing: dark skin tone
 1F57A                                                  ; fully-qualified     # 🕺 E3.0 man dancing
@@ -3240,15 +3532,14 @@
 1F469 1F3FF 200D 2764 200D 1F469 1F3FC                 ; minimally-qualified # 👩🏿‍❤‍👩🏼 E13.1 couple with heart: woman, woman, dark skin tone, medium-light skin tone
 1F469 1F3FF 200D 2764 FE0F 200D 1F469 1F3FD            ; fully-qualified     # 👩🏿‍❤️‍👩🏽 E13.1 couple with heart: woman, woman, dark skin tone, medium skin tone
 1F469 1F3FF 200D 2764 200D 1F469 1F3FD                 ; minimally-qualified # 👩🏿‍❤‍👩🏽 E13.1 couple with heart: woman, woman, dark skin tone, medium skin tone
 1F469 1F3FF 200D 2764 FE0F 200D 1F469 1F3FE            ; fully-qualified     # 👩🏿‍❤️‍👩🏾 E13.1 couple with heart: woman, woman, dark skin tone, medium-dark skin tone
 1F469 1F3FF 200D 2764 200D 1F469 1F3FE                 ; minimally-qualified # 👩🏿‍❤‍👩🏾 E13.1 couple with heart: woman, woman, dark skin tone, medium-dark skin tone
 1F469 1F3FF 200D 2764 FE0F 200D 1F469 1F3FF            ; fully-qualified     # 👩🏿‍❤️‍👩🏿 E13.1 couple with heart: woman, woman, dark skin tone
 1F469 1F3FF 200D 2764 200D 1F469 1F3FF                 ; minimally-qualified # 👩🏿‍❤‍👩🏿 E13.1 couple with heart: woman, woman, dark skin tone
-1F46A                                                  ; fully-qualified     # 👪 E0.6 family
 1F468 200D 1F469 200D 1F466                            ; fully-qualified     # 👨‍👩‍👦 E2.0 family: man, woman, boy
 1F468 200D 1F469 200D 1F467                            ; fully-qualified     # 👨‍👩‍👧 E2.0 family: man, woman, girl
 1F468 200D 1F469 200D 1F467 200D 1F466                 ; fully-qualified     # 👨‍👩‍👧‍👦 E2.0 family: man, woman, girl, boy
 1F468 200D 1F469 200D 1F466 200D 1F466                 ; fully-qualified     # 👨‍👩‍👦‍👦 E2.0 family: man, woman, boy, boy
 1F468 200D 1F469 200D 1F467 200D 1F467                 ; fully-qualified     # 👨‍👩‍👧‍👧 E2.0 family: man, woman, girl, girl
 1F468 200D 1F468 200D 1F466                            ; fully-qualified     # 👨‍👨‍👦 E2.0 family: man, man, boy
 1F468 200D 1F468 200D 1F467                            ; fully-qualified     # 👨‍👨‍👧 E2.0 family: man, man, girl
@@ -3273,18 +3564,23 @@
 
 # subgroup: person-symbol
 1F5E3 FE0F                                             ; fully-qualified     # 🗣️ E0.7 speaking head
 1F5E3                                                  ; unqualified         # 🗣 E0.7 speaking head
 1F464                                                  ; fully-qualified     # 👤 E0.6 bust in silhouette
 1F465                                                  ; fully-qualified     # 👥 E1.0 busts in silhouette
 1FAC2                                                  ; fully-qualified     # 🫂 E13.0 people hugging
+1F46A                                                  ; fully-qualified     # 👪 E0.6 family
+1F9D1 200D 1F9D1 200D 1F9D2                            ; fully-qualified     # 🧑‍🧑‍🧒 E15.1 family: adult, adult, child
+1F9D1 200D 1F9D1 200D 1F9D2 200D 1F9D2                 ; fully-qualified     # 🧑‍🧑‍🧒‍🧒 E15.1 family: adult, adult, child, child
+1F9D1 200D 1F9D2                                       ; fully-qualified     # 🧑‍🧒 E15.1 family: adult, child
+1F9D1 200D 1F9D2 200D 1F9D2                            ; fully-qualified     # 🧑‍🧒‍🧒 E15.1 family: adult, child, child
 1F463                                                  ; fully-qualified     # 👣 E0.6 footprints
 
-# People & Body subtotal:		2998
-# People & Body subtotal:		508	w/o modifiers
+# People & Body subtotal:		3290
+# People & Body subtotal:		560	w/o modifiers
 
 # group: Component
 
 # subgroup: skin-tone
 1F3FB                                                  ; component           # 🏻 E1.0 light skin tone
 1F3FC                                                  ; component           # 🏼 E1.0 medium-light skin tone
 1F3FD                                                  ; component           # 🏽 E1.0 medium skin tone
@@ -3391,14 +3687,15 @@
 1FAB6                                                  ; fully-qualified     # 🪶 E13.0 feather
 1F9A9                                                  ; fully-qualified     # 🦩 E12.0 flamingo
 1F99A                                                  ; fully-qualified     # 🦚 E11.0 peacock
 1F99C                                                  ; fully-qualified     # 🦜 E11.0 parrot
 1FABD                                                  ; fully-qualified     # 🪽 E15.0 wing
 1F426 200D 2B1B                                        ; fully-qualified     # 🐦‍⬛ E15.0 black bird
 1FABF                                                  ; fully-qualified     # 🪿 E15.0 goose
+1F426 200D 1F525                                       ; fully-qualified     # 🐦‍🔥 E15.1 phoenix
 
 # subgroup: animal-amphibian
 1F438                                                  ; fully-qualified     # 🐸 E0.6 frog
 
 # subgroup: animal-reptile
 1F40A                                                  ; fully-qualified     # 🐊 E1.0 crocodile
 1F422                                                  ; fully-qualified     # 🐢 E0.6 turtle
@@ -3473,25 +3770,26 @@
 1F341                                                  ; fully-qualified     # 🍁 E0.6 maple leaf
 1F342                                                  ; fully-qualified     # 🍂 E0.6 fallen leaf
 1F343                                                  ; fully-qualified     # 🍃 E0.6 leaf fluttering in wind
 1FAB9                                                  ; fully-qualified     # 🪹 E14.0 empty nest
 1FABA                                                  ; fully-qualified     # 🪺 E14.0 nest with eggs
 1F344                                                  ; fully-qualified     # 🍄 E0.6 mushroom
 
-# Animals & Nature subtotal:		159
-# Animals & Nature subtotal:		159	w/o modifiers
+# Animals & Nature subtotal:		160
+# Animals & Nature subtotal:		160	w/o modifiers
 
 # group: Food & Drink
 
 # subgroup: food-fruit
 1F347                                                  ; fully-qualified     # 🍇 E0.6 grapes
 1F348                                                  ; fully-qualified     # 🍈 E0.6 melon
 1F349                                                  ; fully-qualified     # 🍉 E0.6 watermelon
 1F34A                                                  ; fully-qualified     # 🍊 E0.6 tangerine
 1F34B                                                  ; fully-qualified     # 🍋 E1.0 lemon
+1F34B 200D 1F7E9                                       ; fully-qualified     # 🍋‍🟩 E15.1 lime
 1F34C                                                  ; fully-qualified     # 🍌 E0.6 banana
 1F34D                                                  ; fully-qualified     # 🍍 E0.6 pineapple
 1F96D                                                  ; fully-qualified     # 🥭 E11.0 mango
 1F34E                                                  ; fully-qualified     # 🍎 E0.6 red apple
 1F34F                                                  ; fully-qualified     # 🍏 E0.6 green apple
 1F350                                                  ; fully-qualified     # 🍐 E1.0 pear
 1F351                                                  ; fully-qualified     # 🍑 E0.6 peach
@@ -3518,14 +3816,15 @@
 1F9C4                                                  ; fully-qualified     # 🧄 E12.0 garlic
 1F9C5                                                  ; fully-qualified     # 🧅 E12.0 onion
 1F95C                                                  ; fully-qualified     # 🥜 E3.0 peanuts
 1FAD8                                                  ; fully-qualified     # 🫘 E14.0 beans
 1F330                                                  ; fully-qualified     # 🌰 E0.6 chestnut
 1FADA                                                  ; fully-qualified     # 🫚 E15.0 ginger root
 1FADB                                                  ; fully-qualified     # 🫛 E15.0 pea pod
+1F344 200D 1F7EB                                       ; fully-qualified     # 🍄‍🟫 E15.1 brown mushroom
 
 # subgroup: food-prepared
 1F35E                                                  ; fully-qualified     # 🍞 E0.6 bread
 1F950                                                  ; fully-qualified     # 🥐 E3.0 croissant
 1F956                                                  ; fully-qualified     # 🥖 E3.0 baguette bread
 1FAD3                                                  ; fully-qualified     # 🫓 E13.0 flatbread
 1F968                                                  ; fully-qualified     # 🥨 E5.0 pretzel
@@ -3629,16 +3928,16 @@
 1F37D                                                  ; unqualified         # 🍽 E0.7 fork and knife with plate
 1F374                                                  ; fully-qualified     # 🍴 E0.6 fork and knife
 1F944                                                  ; fully-qualified     # 🥄 E3.0 spoon
 1F52A                                                  ; fully-qualified     # 🔪 E0.6 kitchen knife
 1FAD9                                                  ; fully-qualified     # 🫙 E14.0 jar
 1F3FA                                                  ; fully-qualified     # 🏺 E1.0 amphora
 
-# Food & Drink subtotal:		135
-# Food & Drink subtotal:		135	w/o modifiers
+# Food & Drink subtotal:		137
+# Food & Drink subtotal:		137	w/o modifiers
 
 # group: Travel & Places
 
 # subgroup: place-map
 1F30D                                                  ; fully-qualified     # 🌍 E0.7 globe showing Europe-Africa
 1F30E                                                  ; fully-qualified     # 🌎 E0.7 globe showing Americas
 1F30F                                                  ; fully-qualified     # 🌏 E0.6 globe showing Asia-Australia
@@ -4317,14 +4616,16 @@
 2699                                                   ; unqualified         # ⚙ E1.0 gear
 1F5DC FE0F                                             ; fully-qualified     # 🗜️ E0.7 clamp
 1F5DC                                                  ; unqualified         # 🗜 E0.7 clamp
 2696 FE0F                                              ; fully-qualified     # ⚖️ E1.0 balance scale
 2696                                                   ; unqualified         # ⚖ E1.0 balance scale
 1F9AF                                                  ; fully-qualified     # 🦯 E12.0 white cane
 1F517                                                  ; fully-qualified     # 🔗 E0.6 link
+26D3 FE0F 200D 1F4A5                                   ; fully-qualified     # ⛓️‍💥 E15.1 broken chain
+26D3 200D 1F4A5                                        ; unqualified         # ⛓‍💥 E15.1 broken chain
 26D3 FE0F                                              ; fully-qualified     # ⛓️ E0.7 chains
 26D3                                                   ; unqualified         # ⛓ E0.7 chains
 1FA9D                                                  ; fully-qualified     # 🪝 E13.0 hook
 1F9F0                                                  ; fully-qualified     # 🧰 E11.0 toolbox
 1F9F2                                                  ; fully-qualified     # 🧲 E11.0 magnet
 1FA9C                                                  ; fully-qualified     # 🪜 E13.0 ladder
 
@@ -4385,16 +4686,16 @@
 26B1                                                   ; unqualified         # ⚱ E1.0 funeral urn
 1F9FF                                                  ; fully-qualified     # 🧿 E11.0 nazar amulet
 1FAAC                                                  ; fully-qualified     # 🪬 E14.0 hamsa
 1F5FF                                                  ; fully-qualified     # 🗿 E0.6 moai
 1FAA7                                                  ; fully-qualified     # 🪧 E13.0 placard
 1FAAA                                                  ; fully-qualified     # 🪪 E14.0 identification card
 
-# Objects subtotal:		310
-# Objects subtotal:		310	w/o modifiers
+# Objects subtotal:		312
+# Objects subtotal:		312	w/o modifiers
 
 # group: Symbols
 
 # subgroup: transport-sign
 1F3E7                                                  ; fully-qualified     # 🏧 E0.6 ATM sign
 1F6AE                                                  ; fully-qualified     # 🚮 E1.0 litter in bin sign
 1F6B0                                                  ; fully-qualified     # 🚰 E1.0 potable water
@@ -4975,15 +5276,15 @@
 1F1F9 1F1ED                                            ; fully-qualified     # 🇹🇭 E2.0 flag: Thailand
 1F1F9 1F1EF                                            ; fully-qualified     # 🇹🇯 E2.0 flag: Tajikistan
 1F1F9 1F1F0                                            ; fully-qualified     # 🇹🇰 E2.0 flag: Tokelau
 1F1F9 1F1F1                                            ; fully-qualified     # 🇹🇱 E2.0 flag: Timor-Leste
 1F1F9 1F1F2                                            ; fully-qualified     # 🇹🇲 E2.0 flag: Turkmenistan
 1F1F9 1F1F3                                            ; fully-qualified     # 🇹🇳 E2.0 flag: Tunisia
 1F1F9 1F1F4                                            ; fully-qualified     # 🇹🇴 E2.0 flag: Tonga
-1F1F9 1F1F7                                            ; fully-qualified     # 🇹🇷 E2.0 flag: Turkey
+1F1F9 1F1F7                                            ; fully-qualified     # 🇹🇷 E2.0 flag: Türkiye
 1F1F9 1F1F9                                            ; fully-qualified     # 🇹🇹 E2.0 flag: Trinidad & Tobago
 1F1F9 1F1FB                                            ; fully-qualified     # 🇹🇻 E2.0 flag: Tuvalu
 1F1F9 1F1FC                                            ; fully-qualified     # 🇹🇼 E2.0 flag: Taiwan
 1F1F9 1F1FF                                            ; fully-qualified     # 🇹🇿 E2.0 flag: Tanzania
 1F1FA 1F1E6                                            ; fully-qualified     # 🇺🇦 E2.0 flag: Ukraine
 1F1FA 1F1EC                                            ; fully-qualified     # 🇺🇬 E2.0 flag: Uganda
 1F1FA 1F1F2                                            ; fully-qualified     # 🇺🇲 E2.0 flag: U.S. Outlying Islands
@@ -5012,13 +5313,13 @@
 1F3F4 E0067 E0062 E0073 E0063 E0074 E007F              ; fully-qualified     # 🏴󠁧󠁢󠁳󠁣󠁴󠁿 E5.0 flag: Scotland
 1F3F4 E0067 E0062 E0077 E006C E0073 E007F              ; fully-qualified     # 🏴󠁧󠁢󠁷󠁬󠁳󠁿 E5.0 flag: Wales
 
 # Flags subtotal:		275
 # Flags subtotal:		275	w/o modifiers
 
 # Status Counts
-# fully-qualified : 3655
-# minimally-qualified : 827
-# unqualified : 242
+# fully-qualified : 3773
+# minimally-qualified : 1009
+# unqualified : 243
 # component : 9
 
 #EOF
```

### Comparing `emoji-data-0.2.post2/src/emoji_data/data/emoji-variation-sequences.txt` & `emoji_data-0.3/src/emoji_data/data/emoji-variation-sequences.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # emoji-variation-sequences.txt
-# Date: 2022-05-13, 21:54:24 GMT
-# © 2022 Unicode®, Inc.
+# Date: 2023-02-01, 02:22:54 GMT
+# © 2023 Unicode®, Inc.
 # Unicode and the Unicode Logo are registered trademarks of Unicode, Inc. in the U.S. and other countries.
 # For terms of use, see https://www.unicode.org/terms_of_use.html
 #
 # Emoji Variation Sequences for UTS #51
-# Used with Emoji Version 15.0 and subsequent minor revisions (if any)
+# Used with Emoji Version 15.1 and subsequent minor revisions (if any)
 #
 # For documentation and usage, see https://www.unicode.org/reports/tr51
 #
 0023 FE0E  ; text style;  # (1.1) NUMBER SIGN
 0023 FE0F  ; emoji style; # (1.1) NUMBER SIGN
 002A FE0E  ; text style;  # (1.1) ASTERISK
 002A FE0F  ; emoji style; # (1.1) ASTERISK
@@ -69,20 +69,26 @@
 2328 FE0F  ; emoji style; # (1.1) KEYBOARD
 23CF FE0E  ; text style;  # (4.0) EJECT SYMBOL
 23CF FE0F  ; emoji style; # (4.0) EJECT SYMBOL
 23E9 FE0E  ; text style;  # (6.0) BLACK RIGHT-POINTING DOUBLE TRIANGLE
 23E9 FE0F  ; emoji style; # (6.0) BLACK RIGHT-POINTING DOUBLE TRIANGLE
 23EA FE0E  ; text style;  # (6.0) BLACK LEFT-POINTING DOUBLE TRIANGLE
 23EA FE0F  ; emoji style; # (6.0) BLACK LEFT-POINTING DOUBLE TRIANGLE
+23EB FE0E  ; text style;  # (6.0) BLACK UP-POINTING DOUBLE TRIANGLE
+23EB FE0F  ; emoji style; # (6.0) BLACK UP-POINTING DOUBLE TRIANGLE
+23EC FE0E  ; text style;  # (6.0) BLACK DOWN-POINTING DOUBLE TRIANGLE
+23EC FE0F  ; emoji style; # (6.0) BLACK DOWN-POINTING DOUBLE TRIANGLE
 23ED FE0E  ; text style;  # (6.0) BLACK RIGHT-POINTING DOUBLE TRIANGLE WITH VERTICAL BAR
 23ED FE0F  ; emoji style; # (6.0) BLACK RIGHT-POINTING DOUBLE TRIANGLE WITH VERTICAL BAR
 23EE FE0E  ; text style;  # (6.0) BLACK LEFT-POINTING DOUBLE TRIANGLE WITH VERTICAL BAR
 23EE FE0F  ; emoji style; # (6.0) BLACK LEFT-POINTING DOUBLE TRIANGLE WITH VERTICAL BAR
 23EF FE0E  ; text style;  # (6.0) BLACK RIGHT-POINTING TRIANGLE WITH DOUBLE VERTICAL BAR
 23EF FE0F  ; emoji style; # (6.0) BLACK RIGHT-POINTING TRIANGLE WITH DOUBLE VERTICAL BAR
+23F0 FE0E  ; text style;  # (6.0) ALARM CLOCK
+23F0 FE0F  ; emoji style; # (6.0) ALARM CLOCK
 23F1 FE0E  ; text style;  # (6.0) STOPWATCH
 23F1 FE0F  ; emoji style; # (6.0) STOPWATCH
 23F2 FE0E  ; text style;  # (6.0) TIMER CLOCK
 23F2 FE0F  ; emoji style; # (6.0) TIMER CLOCK
 23F3 FE0E  ; text style;  # (6.0) HOURGLASS WITH FLOWING SAND
 23F3 FE0F  ; emoji style; # (6.0) HOURGLASS WITH FLOWING SAND
 23F8 FE0E  ; text style;  # (7.0) DOUBLE VERTICAL BAR
@@ -235,14 +241,16 @@
 26BE FE0F  ; emoji style; # (5.2) BASEBALL
 26C4 FE0E  ; text style;  # (5.2) SNOWMAN WITHOUT SNOW
 26C4 FE0F  ; emoji style; # (5.2) SNOWMAN WITHOUT SNOW
 26C5 FE0E  ; text style;  # (5.2) SUN BEHIND CLOUD
 26C5 FE0F  ; emoji style; # (5.2) SUN BEHIND CLOUD
 26C8 FE0E  ; text style;  # (5.2) THUNDER CLOUD AND RAIN
 26C8 FE0F  ; emoji style; # (5.2) THUNDER CLOUD AND RAIN
+26CE FE0E  ; text style;  # (6.0) OPHIUCHUS
+26CE FE0F  ; emoji style; # (6.0) OPHIUCHUS
 26CF FE0E  ; text style;  # (5.2) PICK
 26CF FE0F  ; emoji style; # (5.2) PICK
 26D1 FE0E  ; text style;  # (5.2) HELMET WITH WHITE CROSS
 26D1 FE0F  ; emoji style; # (5.2) HELMET WITH WHITE CROSS
 26D3 FE0E  ; text style;  # (5.2) CHAINS
 26D3 FE0F  ; emoji style; # (5.2) CHAINS
 26D4 FE0E  ; text style;  # (5.2) NO ENTRY
@@ -271,18 +279,24 @@
 26F9 FE0F  ; emoji style; # (5.2) PERSON WITH BALL
 26FA FE0E  ; text style;  # (5.2) TENT
 26FA FE0F  ; emoji style; # (5.2) TENT
 26FD FE0E  ; text style;  # (5.2) FUEL PUMP
 26FD FE0F  ; emoji style; # (5.2) FUEL PUMP
 2702 FE0E  ; text style;  # (1.1) BLACK SCISSORS
 2702 FE0F  ; emoji style; # (1.1) BLACK SCISSORS
+2705 FE0E  ; text style;  # (6.0) WHITE HEAVY CHECK MARK
+2705 FE0F  ; emoji style; # (6.0) WHITE HEAVY CHECK MARK
 2708 FE0E  ; text style;  # (1.1) AIRPLANE
 2708 FE0F  ; emoji style; # (1.1) AIRPLANE
 2709 FE0E  ; text style;  # (1.1) ENVELOPE
 2709 FE0F  ; emoji style; # (1.1) ENVELOPE
+270A FE0E  ; text style;  # (6.0) RAISED FIST
+270A FE0F  ; emoji style; # (6.0) RAISED FIST
+270B FE0E  ; text style;  # (6.0) RAISED HAND
+270B FE0F  ; emoji style; # (6.0) RAISED HAND
 270C FE0E  ; text style;  # (1.1) VICTORY HAND
 270C FE0F  ; emoji style; # (1.1) VICTORY HAND
 270D FE0E  ; text style;  # (1.1) WRITING HAND
 270D FE0F  ; emoji style; # (1.1) WRITING HAND
 270F FE0E  ; text style;  # (1.1) PENCIL
 270F FE0F  ; emoji style; # (1.1) PENCIL
 2712 FE0E  ; text style;  # (1.1) BLACK NIB
@@ -291,32 +305,52 @@
 2714 FE0F  ; emoji style; # (1.1) HEAVY CHECK MARK
 2716 FE0E  ; text style;  # (1.1) HEAVY MULTIPLICATION X
 2716 FE0F  ; emoji style; # (1.1) HEAVY MULTIPLICATION X
 271D FE0E  ; text style;  # (1.1) LATIN CROSS
 271D FE0F  ; emoji style; # (1.1) LATIN CROSS
 2721 FE0E  ; text style;  # (1.1) STAR OF DAVID
 2721 FE0F  ; emoji style; # (1.1) STAR OF DAVID
+2728 FE0E  ; text style;  # (6.0) SPARKLES
+2728 FE0F  ; emoji style; # (6.0) SPARKLES
 2733 FE0E  ; text style;  # (1.1) EIGHT SPOKED ASTERISK
 2733 FE0F  ; emoji style; # (1.1) EIGHT SPOKED ASTERISK
 2734 FE0E  ; text style;  # (1.1) EIGHT POINTED BLACK STAR
 2734 FE0F  ; emoji style; # (1.1) EIGHT POINTED BLACK STAR
 2744 FE0E  ; text style;  # (1.1) SNOWFLAKE
 2744 FE0F  ; emoji style; # (1.1) SNOWFLAKE
 2747 FE0E  ; text style;  # (1.1) SPARKLE
 2747 FE0F  ; emoji style; # (1.1) SPARKLE
+274C FE0E  ; text style;  # (6.0) CROSS MARK
+274C FE0F  ; emoji style; # (6.0) CROSS MARK
+274E FE0E  ; text style;  # (6.0) NEGATIVE SQUARED CROSS MARK
+274E FE0F  ; emoji style; # (6.0) NEGATIVE SQUARED CROSS MARK
 2753 FE0E  ; text style;  # (6.0) BLACK QUESTION MARK ORNAMENT
 2753 FE0F  ; emoji style; # (6.0) BLACK QUESTION MARK ORNAMENT
+2754 FE0E  ; text style;  # (6.0) WHITE QUESTION MARK ORNAMENT
+2754 FE0F  ; emoji style; # (6.0) WHITE QUESTION MARK ORNAMENT
+2755 FE0E  ; text style;  # (6.0) WHITE EXCLAMATION MARK ORNAMENT
+2755 FE0F  ; emoji style; # (6.0) WHITE EXCLAMATION MARK ORNAMENT
 2757 FE0E  ; text style;  # (5.2) HEAVY EXCLAMATION MARK SYMBOL
 2757 FE0F  ; emoji style; # (5.2) HEAVY EXCLAMATION MARK SYMBOL
 2763 FE0E  ; text style;  # (1.1) HEAVY HEART EXCLAMATION MARK ORNAMENT
 2763 FE0F  ; emoji style; # (1.1) HEAVY HEART EXCLAMATION MARK ORNAMENT
 2764 FE0E  ; text style;  # (1.1) HEAVY BLACK HEART
 2764 FE0F  ; emoji style; # (1.1) HEAVY BLACK HEART
+2795 FE0E  ; text style;  # (6.0) HEAVY PLUS SIGN
+2795 FE0F  ; emoji style; # (6.0) HEAVY PLUS SIGN
+2796 FE0E  ; text style;  # (6.0) HEAVY MINUS SIGN
+2796 FE0F  ; emoji style; # (6.0) HEAVY MINUS SIGN
+2797 FE0E  ; text style;  # (6.0) HEAVY DIVISION SIGN
+2797 FE0F  ; emoji style; # (6.0) HEAVY DIVISION SIGN
 27A1 FE0E  ; text style;  # (1.1) BLACK RIGHTWARDS ARROW
 27A1 FE0F  ; emoji style; # (1.1) BLACK RIGHTWARDS ARROW
+27B0 FE0E  ; text style;  # (6.0) CURLY LOOP
+27B0 FE0F  ; emoji style; # (6.0) CURLY LOOP
+27BF FE0E  ; text style;  # (6.0) DOUBLE CURLY LOOP
+27BF FE0F  ; emoji style; # (6.0) DOUBLE CURLY LOOP
 2934 FE0E  ; text style;  # (3.2) ARROW POINTING RIGHTWARDS THEN CURVING UPWARDS
 2934 FE0F  ; emoji style; # (3.2) ARROW POINTING RIGHTWARDS THEN CURVING UPWARDS
 2935 FE0E  ; text style;  # (3.2) ARROW POINTING RIGHTWARDS THEN CURVING DOWNWARDS
 2935 FE0F  ; emoji style; # (3.2) ARROW POINTING RIGHTWARDS THEN CURVING DOWNWARDS
 2B05 FE0E  ; text style;  # (4.0) LEFTWARDS BLACK ARROW
 2B05 FE0F  ; emoji style; # (4.0) LEFTWARDS BLACK ARROW
 2B06 FE0E  ; text style;  # (4.0) UPWARDS BLACK ARROW
@@ -714,10 +748,10 @@
 1F6E9 FE0E ; text style;  # (7.0) SMALL AIRPLANE
 1F6E9 FE0F ; emoji style; # (7.0) SMALL AIRPLANE
 1F6F0 FE0E ; text style;  # (7.0) SATELLITE
 1F6F0 FE0F ; emoji style; # (7.0) SATELLITE
 1F6F3 FE0E ; text style;  # (7.0) PASSENGER SHIP
 1F6F3 FE0F ; emoji style; # (7.0) PASSENGER SHIP
 
-#Total sequences: 354
+#Total sequences: 371
 
 #EOF
```

### Comparing `emoji-data-0.2.post2/src/emoji_data/data/emoji-zwj-sequences.txt` & `emoji_data-0.3/src/emoji_data/data/emoji-zwj-sequences.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # emoji-zwj-sequences.txt
-# Date: 2022-05-06, 16:14:52 GMT
-# © 2022 Unicode®, Inc.
+# Date: 2023-06-05, 20:04:50 GMT
+# © 2023 Unicode®, Inc.
 # Unicode and the Unicode Logo are registered trademarks of Unicode, Inc. in the U.S. and other countries.
 # For terms of use, see https://www.unicode.org/terms_of_use.html
 #
 # Emoji ZWJ Sequences for UTS #51
-# Version: 15.0
+# Version: 15.1
 #
 # For documentation and usage, see https://www.unicode.org/reports/tr51
 #
 # Format:
-#   code_point(s) ; type_field ; description # comments 
+#   code_point(s) ; type_field ; description # comments
 # Fields:
 #   code_point(s): one or more code points in hex format, separated by spaces
 #   type_field :RGI_Emoji_ZWJ_Sequence
 #     The type_field is a convenience for parsing the emoji sequence files, and is not intended to be maintained as a property.
 #   short name: CLDR short name of sequence; characters may be escaped with \x{hex}.
 #
 # For the purpose of regular expressions, the above type field defines the name of
@@ -265,79 +265,78 @@
 1F469 1F3FF 200D 1F91D 200D 1F468 1F3FD     ; RGI_Emoji_ZWJ_Sequence  ; woman and man holding hands: dark skin tone, medium skin tone  # E12.0  [1] (👩🏿‍🤝‍👨🏽)
 1F469 1F3FF 200D 1F91D 200D 1F468 1F3FE     ; RGI_Emoji_ZWJ_Sequence  ; woman and man holding hands: dark skin tone, medium-dark skin tone #E12.0[1] (👩🏿‍🤝‍👨🏾)
 1F469 1F3FF 200D 1F91D 200D 1F469 1F3FB     ; RGI_Emoji_ZWJ_Sequence  ; women holding hands: dark skin tone, light skin tone           # E12.0  [1] (👩🏿‍🤝‍👩🏻)
 1F469 1F3FF 200D 1F91D 200D 1F469 1F3FC     ; RGI_Emoji_ZWJ_Sequence  ; women holding hands: dark skin tone, medium-light skin tone    # E12.0  [1] (👩🏿‍🤝‍👩🏼)
 1F469 1F3FF 200D 1F91D 200D 1F469 1F3FD     ; RGI_Emoji_ZWJ_Sequence  ; women holding hands: dark skin tone, medium skin tone          # E12.0  [1] (👩🏿‍🤝‍👩🏽)
 1F469 1F3FF 200D 1F91D 200D 1F469 1F3FE     ; RGI_Emoji_ZWJ_Sequence  ; women holding hands: dark skin tone, medium-dark skin tone     # E12.0  [1] (👩🏿‍🤝‍👩🏾)
 1F9D1 200D 1F91D 200D 1F9D1                 ; RGI_Emoji_ZWJ_Sequence  ; people holding hands                                           # E12.0  [1] (🧑‍🤝‍🧑)
+1F9D1 200D 1F9D1 200D 1F9D2                 ; RGI_Emoji_ZWJ_Sequence  ; family: adult, adult, child                                    # E15.1  [1] (🧑‍🧑‍🧒)
+1F9D1 200D 1F9D1 200D 1F9D2 200D 1F9D2      ; RGI_Emoji_ZWJ_Sequence  ; family: adult, adult, child, child                             # E15.1  [1] (🧑‍🧑‍🧒‍🧒)
+1F9D1 200D 1F9D2                            ; RGI_Emoji_ZWJ_Sequence  ; family: adult, child                                           # E15.1  [1] (🧑‍🧒)
+1F9D1 200D 1F9D2 200D 1F9D2                 ; RGI_Emoji_ZWJ_Sequence  ; family: adult, child, child                                    # E15.1  [1] (🧑‍🧒‍🧒)
 1F9D1 1F3FB 200D 2764 FE0F 200D 1F48B 200D 1F9D1 1F3FC; RGI_Emoji_ZWJ_Sequence; kiss: person, person, light skin tone, medium-light skin tone #E13.1[1] (🧑🏻‍❤️‍💋‍🧑🏼)
 1F9D1 1F3FB 200D 2764 FE0F 200D 1F48B 200D 1F9D1 1F3FD; RGI_Emoji_ZWJ_Sequence; kiss: person, person, light skin tone, medium skin tone #E13.1  [1] (🧑🏻‍❤️‍💋‍🧑🏽)
 1F9D1 1F3FB 200D 2764 FE0F 200D 1F48B 200D 1F9D1 1F3FE; RGI_Emoji_ZWJ_Sequence; kiss: person, person, light skin tone, medium-dark skin tone #E13.1[1] (🧑🏻‍❤️‍💋‍🧑🏾)
 1F9D1 1F3FB 200D 2764 FE0F 200D 1F48B 200D 1F9D1 1F3FF; RGI_Emoji_ZWJ_Sequence; kiss: person, person, light skin tone, dark skin tone  # E13.1  [1] (🧑🏻‍❤️‍💋‍🧑🏿)
 1F9D1 1F3FB 200D 2764 FE0F 200D 1F9D1 1F3FC ; RGI_Emoji_ZWJ_Sequence  ; couple with heart: person, person, light skin tone, medium-light skin tone #E13.1[1] (🧑🏻‍❤️‍🧑🏼)
 1F9D1 1F3FB 200D 2764 FE0F 200D 1F9D1 1F3FD ; RGI_Emoji_ZWJ_Sequence  ; couple with heart: person, person, light skin tone, medium skin tone #E13.1[1] (🧑🏻‍❤️‍🧑🏽)
 1F9D1 1F3FB 200D 2764 FE0F 200D 1F9D1 1F3FE ; RGI_Emoji_ZWJ_Sequence  ; couple with heart: person, person, light skin tone, medium-dark skin tone #E13.1[1] (🧑🏻‍❤️‍🧑🏾)
 1F9D1 1F3FB 200D 2764 FE0F 200D 1F9D1 1F3FF ; RGI_Emoji_ZWJ_Sequence  ; couple with heart: person, person, light skin tone, dark skin tone #E13.1[1] (🧑🏻‍❤️‍🧑🏿)
-1F9D1 1F3FB 200D 1F384                      ; RGI_Emoji_ZWJ_Sequence  ; mx claus: light skin tone                                      # E13.0  [1] (🧑🏻‍🎄)
 1F9D1 1F3FB 200D 1F91D 200D 1F9D1 1F3FB     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: light skin tone                          # E12.0  [1] (🧑🏻‍🤝‍🧑🏻)
 1F9D1 1F3FB 200D 1F91D 200D 1F9D1 1F3FC     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: light skin tone, medium-light skin tone  # E12.1  [1] (🧑🏻‍🤝‍🧑🏼)
 1F9D1 1F3FB 200D 1F91D 200D 1F9D1 1F3FD     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: light skin tone, medium skin tone        # E12.1  [1] (🧑🏻‍🤝‍🧑🏽)
 1F9D1 1F3FB 200D 1F91D 200D 1F9D1 1F3FE     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: light skin tone, medium-dark skin tone   # E12.1  [1] (🧑🏻‍🤝‍🧑🏾)
 1F9D1 1F3FB 200D 1F91D 200D 1F9D1 1F3FF     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: light skin tone, dark skin tone          # E12.1  [1] (🧑🏻‍🤝‍🧑🏿)
 1F9D1 1F3FC 200D 2764 FE0F 200D 1F48B 200D 1F9D1 1F3FB; RGI_Emoji_ZWJ_Sequence; kiss: person, person, medium-light skin tone, light skin tone #E13.1[1] (🧑🏼‍❤️‍💋‍🧑🏻)
 1F9D1 1F3FC 200D 2764 FE0F 200D 1F48B 200D 1F9D1 1F3FD; RGI_Emoji_ZWJ_Sequence; kiss: person, person, medium-light skin tone, medium skin tone #E13.1[1] (🧑🏼‍❤️‍💋‍🧑🏽)
 1F9D1 1F3FC 200D 2764 FE0F 200D 1F48B 200D 1F9D1 1F3FE; RGI_Emoji_ZWJ_Sequence; kiss: person, person, medium-light skin tone, medium-dark skin tone #E13.1[1] (🧑🏼‍❤️‍💋‍🧑🏾)
 1F9D1 1F3FC 200D 2764 FE0F 200D 1F48B 200D 1F9D1 1F3FF; RGI_Emoji_ZWJ_Sequence; kiss: person, person, medium-light skin tone, dark skin tone #E13.1[1] (🧑🏼‍❤️‍💋‍🧑🏿)
 1F9D1 1F3FC 200D 2764 FE0F 200D 1F9D1 1F3FB ; RGI_Emoji_ZWJ_Sequence  ; couple with heart: person, person, medium-light skin tone, light skin tone #E13.1[1] (🧑🏼‍❤️‍🧑🏻)
 1F9D1 1F3FC 200D 2764 FE0F 200D 1F9D1 1F3FD ; RGI_Emoji_ZWJ_Sequence  ; couple with heart: person, person, medium-light skin tone, medium skin tone #E13.1[1] (🧑🏼‍❤️‍🧑🏽)
 1F9D1 1F3FC 200D 2764 FE0F 200D 1F9D1 1F3FE ; RGI_Emoji_ZWJ_Sequence  ; couple with heart: person, person, medium-light skin tone, medium-dark skin tone #E13.1[1] (🧑🏼‍❤️‍🧑🏾)
 1F9D1 1F3FC 200D 2764 FE0F 200D 1F9D1 1F3FF ; RGI_Emoji_ZWJ_Sequence  ; couple with heart: person, person, medium-light skin tone, dark skin tone #E13.1[1] (🧑🏼‍❤️‍🧑🏿)
-1F9D1 1F3FC 200D 1F384                      ; RGI_Emoji_ZWJ_Sequence  ; mx claus: medium-light skin tone                               # E13.0  [1] (🧑🏼‍🎄)
 1F9D1 1F3FC 200D 1F91D 200D 1F9D1 1F3FB     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: medium-light skin tone, light skin tone  # E12.0  [1] (🧑🏼‍🤝‍🧑🏻)
 1F9D1 1F3FC 200D 1F91D 200D 1F9D1 1F3FC     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: medium-light skin tone                   # E12.0  [1] (🧑🏼‍🤝‍🧑🏼)
 1F9D1 1F3FC 200D 1F91D 200D 1F9D1 1F3FD     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: medium-light skin tone, medium skin tone # E12.1  [1] (🧑🏼‍🤝‍🧑🏽)
 1F9D1 1F3FC 200D 1F91D 200D 1F9D1 1F3FE     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: medium-light skin tone, medium-dark skin tone #E12.1[1] (🧑🏼‍🤝‍🧑🏾)
 1F9D1 1F3FC 200D 1F91D 200D 1F9D1 1F3FF     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: medium-light skin tone, dark skin tone   # E12.1  [1] (🧑🏼‍🤝‍🧑🏿)
 1F9D1 1F3FD 200D 2764 FE0F 200D 1F48B 200D 1F9D1 1F3FB; RGI_Emoji_ZWJ_Sequence; kiss: person, person, medium skin tone, light skin tone #E13.1  [1] (🧑🏽‍❤️‍💋‍🧑🏻)
 1F9D1 1F3FD 200D 2764 FE0F 200D 1F48B 200D 1F9D1 1F3FC; RGI_Emoji_ZWJ_Sequence; kiss: person, person, medium skin tone, medium-light skin tone #E13.1[1] (🧑🏽‍❤️‍💋‍🧑🏼)
 1F9D1 1F3FD 200D 2764 FE0F 200D 1F48B 200D 1F9D1 1F3FE; RGI_Emoji_ZWJ_Sequence; kiss: person, person, medium skin tone, medium-dark skin tone #E13.1[1] (🧑🏽‍❤️‍💋‍🧑🏾)
 1F9D1 1F3FD 200D 2764 FE0F 200D 1F48B 200D 1F9D1 1F3FF; RGI_Emoji_ZWJ_Sequence; kiss: person, person, medium skin tone, dark skin tone # E13.1  [1] (🧑🏽‍❤️‍💋‍🧑🏿)
 1F9D1 1F3FD 200D 2764 FE0F 200D 1F9D1 1F3FB ; RGI_Emoji_ZWJ_Sequence  ; couple with heart: person, person, medium skin tone, light skin tone #E13.1[1] (🧑🏽‍❤️‍🧑🏻)
 1F9D1 1F3FD 200D 2764 FE0F 200D 1F9D1 1F3FC ; RGI_Emoji_ZWJ_Sequence  ; couple with heart: person, person, medium skin tone, medium-light skin tone #E13.1[1] (🧑🏽‍❤️‍🧑🏼)
 1F9D1 1F3FD 200D 2764 FE0F 200D 1F9D1 1F3FE ; RGI_Emoji_ZWJ_Sequence  ; couple with heart: person, person, medium skin tone, medium-dark skin tone #E13.1[1] (🧑🏽‍❤️‍🧑🏾)
 1F9D1 1F3FD 200D 2764 FE0F 200D 1F9D1 1F3FF ; RGI_Emoji_ZWJ_Sequence  ; couple with heart: person, person, medium skin tone, dark skin tone #E13.1[1] (🧑🏽‍❤️‍🧑🏿)
-1F9D1 1F3FD 200D 1F384                      ; RGI_Emoji_ZWJ_Sequence  ; mx claus: medium skin tone                                     # E13.0  [1] (🧑🏽‍🎄)
 1F9D1 1F3FD 200D 1F91D 200D 1F9D1 1F3FB     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: medium skin tone, light skin tone        # E12.0  [1] (🧑🏽‍🤝‍🧑🏻)
 1F9D1 1F3FD 200D 1F91D 200D 1F9D1 1F3FC     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: medium skin tone, medium-light skin tone # E12.0  [1] (🧑🏽‍🤝‍🧑🏼)
 1F9D1 1F3FD 200D 1F91D 200D 1F9D1 1F3FD     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: medium skin tone                         # E12.0  [1] (🧑🏽‍🤝‍🧑🏽)
 1F9D1 1F3FD 200D 1F91D 200D 1F9D1 1F3FE     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: medium skin tone, medium-dark skin tone  # E12.1  [1] (🧑🏽‍🤝‍🧑🏾)
 1F9D1 1F3FD 200D 1F91D 200D 1F9D1 1F3FF     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: medium skin tone, dark skin tone         # E12.1  [1] (🧑🏽‍🤝‍🧑🏿)
 1F9D1 1F3FE 200D 2764 FE0F 200D 1F48B 200D 1F9D1 1F3FB; RGI_Emoji_ZWJ_Sequence; kiss: person, person, medium-dark skin tone, light skin tone #E13.1[1] (🧑🏾‍❤️‍💋‍🧑🏻)
 1F9D1 1F3FE 200D 2764 FE0F 200D 1F48B 200D 1F9D1 1F3FC; RGI_Emoji_ZWJ_Sequence; kiss: person, person, medium-dark skin tone, medium-light skin tone #E13.1[1] (🧑🏾‍❤️‍💋‍🧑🏼)
 1F9D1 1F3FE 200D 2764 FE0F 200D 1F48B 200D 1F9D1 1F3FD; RGI_Emoji_ZWJ_Sequence; kiss: person, person, medium-dark skin tone, medium skin tone #E13.1[1] (🧑🏾‍❤️‍💋‍🧑🏽)
 1F9D1 1F3FE 200D 2764 FE0F 200D 1F48B 200D 1F9D1 1F3FF; RGI_Emoji_ZWJ_Sequence; kiss: person, person, medium-dark skin tone, dark skin tone #E13.1[1] (🧑🏾‍❤️‍💋‍🧑🏿)
 1F9D1 1F3FE 200D 2764 FE0F 200D 1F9D1 1F3FB ; RGI_Emoji_ZWJ_Sequence  ; couple with heart: person, person, medium-dark skin tone, light skin tone #E13.1[1] (🧑🏾‍❤️‍🧑🏻)
 1F9D1 1F3FE 200D 2764 FE0F 200D 1F9D1 1F3FC ; RGI_Emoji_ZWJ_Sequence  ; couple with heart: person, person, medium-dark skin tone, medium-light skin tone #E13.1[1] (🧑🏾‍❤️‍🧑🏼)
 1F9D1 1F3FE 200D 2764 FE0F 200D 1F9D1 1F3FD ; RGI_Emoji_ZWJ_Sequence  ; couple with heart: person, person, medium-dark skin tone, medium skin tone #E13.1[1] (🧑🏾‍❤️‍🧑🏽)
 1F9D1 1F3FE 200D 2764 FE0F 200D 1F9D1 1F3FF ; RGI_Emoji_ZWJ_Sequence  ; couple with heart: person, person, medium-dark skin tone, dark skin tone #E13.1[1] (🧑🏾‍❤️‍🧑🏿)
-1F9D1 1F3FE 200D 1F384                      ; RGI_Emoji_ZWJ_Sequence  ; mx claus: medium-dark skin tone                                # E13.0  [1] (🧑🏾‍🎄)
 1F9D1 1F3FE 200D 1F91D 200D 1F9D1 1F3FB     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: medium-dark skin tone, light skin tone   # E12.0  [1] (🧑🏾‍🤝‍🧑🏻)
 1F9D1 1F3FE 200D 1F91D 200D 1F9D1 1F3FC     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: medium-dark skin tone, medium-light skin tone #E12.0[1] (🧑🏾‍🤝‍🧑🏼)
 1F9D1 1F3FE 200D 1F91D 200D 1F9D1 1F3FD     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: medium-dark skin tone, medium skin tone  # E12.0  [1] (🧑🏾‍🤝‍🧑🏽)
 1F9D1 1F3FE 200D 1F91D 200D 1F9D1 1F3FE     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: medium-dark skin tone                    # E12.0  [1] (🧑🏾‍🤝‍🧑🏾)
 1F9D1 1F3FE 200D 1F91D 200D 1F9D1 1F3FF     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: medium-dark skin tone, dark skin tone    # E12.1  [1] (🧑🏾‍🤝‍🧑🏿)
 1F9D1 1F3FF 200D 2764 FE0F 200D 1F48B 200D 1F9D1 1F3FB; RGI_Emoji_ZWJ_Sequence; kiss: person, person, dark skin tone, light skin tone  # E13.1  [1] (🧑🏿‍❤️‍💋‍🧑🏻)
 1F9D1 1F3FF 200D 2764 FE0F 200D 1F48B 200D 1F9D1 1F3FC; RGI_Emoji_ZWJ_Sequence; kiss: person, person, dark skin tone, medium-light skin tone #E13.1[1] (🧑🏿‍❤️‍💋‍🧑🏼)
 1F9D1 1F3FF 200D 2764 FE0F 200D 1F48B 200D 1F9D1 1F3FD; RGI_Emoji_ZWJ_Sequence; kiss: person, person, dark skin tone, medium skin tone # E13.1  [1] (🧑🏿‍❤️‍💋‍🧑🏽)
 1F9D1 1F3FF 200D 2764 FE0F 200D 1F48B 200D 1F9D1 1F3FE; RGI_Emoji_ZWJ_Sequence; kiss: person, person, dark skin tone, medium-dark skin tone #E13.1[1] (🧑🏿‍❤️‍💋‍🧑🏾)
 1F9D1 1F3FF 200D 2764 FE0F 200D 1F9D1 1F3FB ; RGI_Emoji_ZWJ_Sequence  ; couple with heart: person, person, dark skin tone, light skin tone #E13.1[1] (🧑🏿‍❤️‍🧑🏻)
 1F9D1 1F3FF 200D 2764 FE0F 200D 1F9D1 1F3FC ; RGI_Emoji_ZWJ_Sequence  ; couple with heart: person, person, dark skin tone, medium-light skin tone #E13.1[1] (🧑🏿‍❤️‍🧑🏼)
 1F9D1 1F3FF 200D 2764 FE0F 200D 1F9D1 1F3FD ; RGI_Emoji_ZWJ_Sequence  ; couple with heart: person, person, dark skin tone, medium skin tone #E13.1[1] (🧑🏿‍❤️‍🧑🏽)
 1F9D1 1F3FF 200D 2764 FE0F 200D 1F9D1 1F3FE ; RGI_Emoji_ZWJ_Sequence  ; couple with heart: person, person, dark skin tone, medium-dark skin tone #E13.1[1] (🧑🏿‍❤️‍🧑🏾)
-1F9D1 1F3FF 200D 1F384                      ; RGI_Emoji_ZWJ_Sequence  ; mx claus: dark skin tone                                       # E13.0  [1] (🧑🏿‍🎄)
 1F9D1 1F3FF 200D 1F91D 200D 1F9D1 1F3FB     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: dark skin tone, light skin tone          # E12.0  [1] (🧑🏿‍🤝‍🧑🏻)
 1F9D1 1F3FF 200D 1F91D 200D 1F9D1 1F3FC     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: dark skin tone, medium-light skin tone   # E12.0  [1] (🧑🏿‍🤝‍🧑🏼)
 1F9D1 1F3FF 200D 1F91D 200D 1F9D1 1F3FD     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: dark skin tone, medium skin tone         # E12.0  [1] (🧑🏿‍🤝‍🧑🏽)
 1F9D1 1F3FF 200D 1F91D 200D 1F9D1 1F3FE     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: dark skin tone, medium-dark skin tone    # E12.0  [1] (🧑🏿‍🤝‍🧑🏾)
 1F9D1 1F3FF 200D 1F91D 200D 1F9D1 1F3FF     ; RGI_Emoji_ZWJ_Sequence  ; people holding hands: dark skin tone                           # E12.0  [1] (🧑🏿‍🤝‍🧑🏿)
 1FAF1 1F3FB 200D 1FAF2 1F3FC                ; RGI_Emoji_ZWJ_Sequence  ; handshake: light skin tone, medium-light skin tone             # E14.0  [1] (🫱🏻‍🫲🏼)
 1FAF1 1F3FB 200D 1FAF2 1F3FD                ; RGI_Emoji_ZWJ_Sequence  ; handshake: light skin tone, medium skin tone                   # E14.0  [1] (🫱🏻‍🫲🏽)
@@ -356,20 +355,26 @@
 1FAF1 1F3FE 200D 1FAF2 1F3FD                ; RGI_Emoji_ZWJ_Sequence  ; handshake: medium-dark skin tone, medium skin tone             # E14.0  [1] (🫱🏾‍🫲🏽)
 1FAF1 1F3FE 200D 1FAF2 1F3FF                ; RGI_Emoji_ZWJ_Sequence  ; handshake: medium-dark skin tone, dark skin tone               # E14.0  [1] (🫱🏾‍🫲🏿)
 1FAF1 1F3FF 200D 1FAF2 1F3FB                ; RGI_Emoji_ZWJ_Sequence  ; handshake: dark skin tone, light skin tone                     # E14.0  [1] (🫱🏿‍🫲🏻)
 1FAF1 1F3FF 200D 1FAF2 1F3FC                ; RGI_Emoji_ZWJ_Sequence  ; handshake: dark skin tone, medium-light skin tone              # E14.0  [1] (🫱🏿‍🫲🏼)
 1FAF1 1F3FF 200D 1FAF2 1F3FD                ; RGI_Emoji_ZWJ_Sequence  ; handshake: dark skin tone, medium skin tone                    # E14.0  [1] (🫱🏿‍🫲🏽)
 1FAF1 1F3FF 200D 1FAF2 1F3FE                ; RGI_Emoji_ZWJ_Sequence  ; handshake: dark skin tone, medium-dark skin tone               # E14.0  [1] (🫱🏿‍🫲🏾)
 
-# Total elements: 332
+# Total elements: 331
 
 # ================================================
 
 # RGI_Emoji_ZWJ_Sequence: Role
 
+1F3C3 200D 27A1 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; person running facing right                                    # E15.1  [1] (🏃‍➡️)
+1F3C3 1F3FB 200D 27A1 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; person running facing right: light skin tone                   # E15.1  [1] (🏃🏻‍➡️)
+1F3C3 1F3FC 200D 27A1 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; person running facing right: medium-light skin tone            # E15.1  [1] (🏃🏼‍➡️)
+1F3C3 1F3FD 200D 27A1 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; person running facing right: medium skin tone                  # E15.1  [1] (🏃🏽‍➡️)
+1F3C3 1F3FE 200D 27A1 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; person running facing right: medium-dark skin tone             # E15.1  [1] (🏃🏾‍➡️)
+1F3C3 1F3FF 200D 27A1 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; person running facing right: dark skin tone                    # E15.1  [1] (🏃🏿‍➡️)
 1F468 200D 2695 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; man health worker                                              # E4.0   [1] (👨‍⚕️)
 1F468 200D 2696 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; man judge                                                      # E4.0   [1] (👨‍⚖️)
 1F468 200D 2708 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; man pilot                                                      # E4.0   [1] (👨‍✈️)
 1F468 200D 1F33E                            ; RGI_Emoji_ZWJ_Sequence  ; man farmer                                                     # E4.0   [1] (👨‍🌾)
 1F468 200D 1F373                            ; RGI_Emoji_ZWJ_Sequence  ; man cook                                                       # E4.0   [1] (👨‍🍳)
 1F468 200D 1F37C                            ; RGI_Emoji_ZWJ_Sequence  ; man feeding baby                                               # E13.0  [1] (👨‍🍼)
 1F468 200D 1F393                            ; RGI_Emoji_ZWJ_Sequence  ; man student                                                    # E4.0   [1] (👨‍🎓)
@@ -380,16 +385,19 @@
 1F468 200D 1F4BB                            ; RGI_Emoji_ZWJ_Sequence  ; man technologist                                               # E4.0   [1] (👨‍💻)
 1F468 200D 1F4BC                            ; RGI_Emoji_ZWJ_Sequence  ; man office worker                                              # E4.0   [1] (👨‍💼)
 1F468 200D 1F527                            ; RGI_Emoji_ZWJ_Sequence  ; man mechanic                                                   # E4.0   [1] (👨‍🔧)
 1F468 200D 1F52C                            ; RGI_Emoji_ZWJ_Sequence  ; man scientist                                                  # E4.0   [1] (👨‍🔬)
 1F468 200D 1F680                            ; RGI_Emoji_ZWJ_Sequence  ; man astronaut                                                  # E4.0   [1] (👨‍🚀)
 1F468 200D 1F692                            ; RGI_Emoji_ZWJ_Sequence  ; man firefighter                                                # E4.0   [1] (👨‍🚒)
 1F468 200D 1F9AF                            ; RGI_Emoji_ZWJ_Sequence  ; man with white cane                                            # E12.0  [1] (👨‍🦯)
+1F468 200D 1F9AF 200D 27A1 FE0F             ; RGI_Emoji_ZWJ_Sequence  ; man with white cane facing right                               # E15.1  [1] (👨‍🦯‍➡️)
 1F468 200D 1F9BC                            ; RGI_Emoji_ZWJ_Sequence  ; man in motorized wheelchair                                    # E12.0  [1] (👨‍🦼)
+1F468 200D 1F9BC 200D 27A1 FE0F             ; RGI_Emoji_ZWJ_Sequence  ; man in motorized wheelchair facing right                       # E15.1  [1] (👨‍🦼‍➡️)
 1F468 200D 1F9BD                            ; RGI_Emoji_ZWJ_Sequence  ; man in manual wheelchair                                       # E12.0  [1] (👨‍🦽)
+1F468 200D 1F9BD 200D 27A1 FE0F             ; RGI_Emoji_ZWJ_Sequence  ; man in manual wheelchair facing right                          # E15.1  [1] (👨‍🦽‍➡️)
 1F468 1F3FB 200D 2695 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man health worker: light skin tone                             # E4.0   [1] (👨🏻‍⚕️)
 1F468 1F3FB 200D 2696 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man judge: light skin tone                                     # E4.0   [1] (👨🏻‍⚖️)
 1F468 1F3FB 200D 2708 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man pilot: light skin tone                                     # E4.0   [1] (👨🏻‍✈️)
 1F468 1F3FB 200D 1F33E                      ; RGI_Emoji_ZWJ_Sequence  ; man farmer: light skin tone                                    # E4.0   [1] (👨🏻‍🌾)
 1F468 1F3FB 200D 1F373                      ; RGI_Emoji_ZWJ_Sequence  ; man cook: light skin tone                                      # E4.0   [1] (👨🏻‍🍳)
 1F468 1F3FB 200D 1F37C                      ; RGI_Emoji_ZWJ_Sequence  ; man feeding baby: light skin tone                              # E13.0  [1] (👨🏻‍🍼)
 1F468 1F3FB 200D 1F393                      ; RGI_Emoji_ZWJ_Sequence  ; man student: light skin tone                                   # E4.0   [1] (👨🏻‍🎓)
@@ -400,16 +408,19 @@
 1F468 1F3FB 200D 1F4BB                      ; RGI_Emoji_ZWJ_Sequence  ; man technologist: light skin tone                              # E4.0   [1] (👨🏻‍💻)
 1F468 1F3FB 200D 1F4BC                      ; RGI_Emoji_ZWJ_Sequence  ; man office worker: light skin tone                             # E4.0   [1] (👨🏻‍💼)
 1F468 1F3FB 200D 1F527                      ; RGI_Emoji_ZWJ_Sequence  ; man mechanic: light skin tone                                  # E4.0   [1] (👨🏻‍🔧)
 1F468 1F3FB 200D 1F52C                      ; RGI_Emoji_ZWJ_Sequence  ; man scientist: light skin tone                                 # E4.0   [1] (👨🏻‍🔬)
 1F468 1F3FB 200D 1F680                      ; RGI_Emoji_ZWJ_Sequence  ; man astronaut: light skin tone                                 # E4.0   [1] (👨🏻‍🚀)
 1F468 1F3FB 200D 1F692                      ; RGI_Emoji_ZWJ_Sequence  ; man firefighter: light skin tone                               # E4.0   [1] (👨🏻‍🚒)
 1F468 1F3FB 200D 1F9AF                      ; RGI_Emoji_ZWJ_Sequence  ; man with white cane: light skin tone                           # E12.0  [1] (👨🏻‍🦯)
+1F468 1F3FB 200D 1F9AF 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; man with white cane facing right: light skin tone              # E15.1  [1] (👨🏻‍🦯‍➡️)
 1F468 1F3FB 200D 1F9BC                      ; RGI_Emoji_ZWJ_Sequence  ; man in motorized wheelchair: light skin tone                   # E12.0  [1] (👨🏻‍🦼)
+1F468 1F3FB 200D 1F9BC 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; man in motorized wheelchair facing right: light skin tone      # E15.1  [1] (👨🏻‍🦼‍➡️)
 1F468 1F3FB 200D 1F9BD                      ; RGI_Emoji_ZWJ_Sequence  ; man in manual wheelchair: light skin tone                      # E12.0  [1] (👨🏻‍🦽)
+1F468 1F3FB 200D 1F9BD 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; man in manual wheelchair facing right: light skin tone         # E15.1  [1] (👨🏻‍🦽‍➡️)
 1F468 1F3FC 200D 2695 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man health worker: medium-light skin tone                      # E4.0   [1] (👨🏼‍⚕️)
 1F468 1F3FC 200D 2696 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man judge: medium-light skin tone                              # E4.0   [1] (👨🏼‍⚖️)
 1F468 1F3FC 200D 2708 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man pilot: medium-light skin tone                              # E4.0   [1] (👨🏼‍✈️)
 1F468 1F3FC 200D 1F33E                      ; RGI_Emoji_ZWJ_Sequence  ; man farmer: medium-light skin tone                             # E4.0   [1] (👨🏼‍🌾)
 1F468 1F3FC 200D 1F373                      ; RGI_Emoji_ZWJ_Sequence  ; man cook: medium-light skin tone                               # E4.0   [1] (👨🏼‍🍳)
 1F468 1F3FC 200D 1F37C                      ; RGI_Emoji_ZWJ_Sequence  ; man feeding baby: medium-light skin tone                       # E13.0  [1] (👨🏼‍🍼)
 1F468 1F3FC 200D 1F393                      ; RGI_Emoji_ZWJ_Sequence  ; man student: medium-light skin tone                            # E4.0   [1] (👨🏼‍🎓)
@@ -420,16 +431,19 @@
 1F468 1F3FC 200D 1F4BB                      ; RGI_Emoji_ZWJ_Sequence  ; man technologist: medium-light skin tone                       # E4.0   [1] (👨🏼‍💻)
 1F468 1F3FC 200D 1F4BC                      ; RGI_Emoji_ZWJ_Sequence  ; man office worker: medium-light skin tone                      # E4.0   [1] (👨🏼‍💼)
 1F468 1F3FC 200D 1F527                      ; RGI_Emoji_ZWJ_Sequence  ; man mechanic: medium-light skin tone                           # E4.0   [1] (👨🏼‍🔧)
 1F468 1F3FC 200D 1F52C                      ; RGI_Emoji_ZWJ_Sequence  ; man scientist: medium-light skin tone                          # E4.0   [1] (👨🏼‍🔬)
 1F468 1F3FC 200D 1F680                      ; RGI_Emoji_ZWJ_Sequence  ; man astronaut: medium-light skin tone                          # E4.0   [1] (👨🏼‍🚀)
 1F468 1F3FC 200D 1F692                      ; RGI_Emoji_ZWJ_Sequence  ; man firefighter: medium-light skin tone                        # E4.0   [1] (👨🏼‍🚒)
 1F468 1F3FC 200D 1F9AF                      ; RGI_Emoji_ZWJ_Sequence  ; man with white cane: medium-light skin tone                    # E12.0  [1] (👨🏼‍🦯)
+1F468 1F3FC 200D 1F9AF 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; man with white cane facing right: medium-light skin tone       # E15.1  [1] (👨🏼‍🦯‍➡️)
 1F468 1F3FC 200D 1F9BC                      ; RGI_Emoji_ZWJ_Sequence  ; man in motorized wheelchair: medium-light skin tone            # E12.0  [1] (👨🏼‍🦼)
+1F468 1F3FC 200D 1F9BC 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; man in motorized wheelchair facing right: medium-light skin tone #E15.1 [1] (👨🏼‍🦼‍➡️)
 1F468 1F3FC 200D 1F9BD                      ; RGI_Emoji_ZWJ_Sequence  ; man in manual wheelchair: medium-light skin tone               # E12.0  [1] (👨🏼‍🦽)
+1F468 1F3FC 200D 1F9BD 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; man in manual wheelchair facing right: medium-light skin tone  # E15.1  [1] (👨🏼‍🦽‍➡️)
 1F468 1F3FD 200D 2695 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man health worker: medium skin tone                            # E4.0   [1] (👨🏽‍⚕️)
 1F468 1F3FD 200D 2696 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man judge: medium skin tone                                    # E4.0   [1] (👨🏽‍⚖️)
 1F468 1F3FD 200D 2708 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man pilot: medium skin tone                                    # E4.0   [1] (👨🏽‍✈️)
 1F468 1F3FD 200D 1F33E                      ; RGI_Emoji_ZWJ_Sequence  ; man farmer: medium skin tone                                   # E4.0   [1] (👨🏽‍🌾)
 1F468 1F3FD 200D 1F373                      ; RGI_Emoji_ZWJ_Sequence  ; man cook: medium skin tone                                     # E4.0   [1] (👨🏽‍🍳)
 1F468 1F3FD 200D 1F37C                      ; RGI_Emoji_ZWJ_Sequence  ; man feeding baby: medium skin tone                             # E13.0  [1] (👨🏽‍🍼)
 1F468 1F3FD 200D 1F393                      ; RGI_Emoji_ZWJ_Sequence  ; man student: medium skin tone                                  # E4.0   [1] (👨🏽‍🎓)
@@ -440,16 +454,19 @@
 1F468 1F3FD 200D 1F4BB                      ; RGI_Emoji_ZWJ_Sequence  ; man technologist: medium skin tone                             # E4.0   [1] (👨🏽‍💻)
 1F468 1F3FD 200D 1F4BC                      ; RGI_Emoji_ZWJ_Sequence  ; man office worker: medium skin tone                            # E4.0   [1] (👨🏽‍💼)
 1F468 1F3FD 200D 1F527                      ; RGI_Emoji_ZWJ_Sequence  ; man mechanic: medium skin tone                                 # E4.0   [1] (👨🏽‍🔧)
 1F468 1F3FD 200D 1F52C                      ; RGI_Emoji_ZWJ_Sequence  ; man scientist: medium skin tone                                # E4.0   [1] (👨🏽‍🔬)
 1F468 1F3FD 200D 1F680                      ; RGI_Emoji_ZWJ_Sequence  ; man astronaut: medium skin tone                                # E4.0   [1] (👨🏽‍🚀)
 1F468 1F3FD 200D 1F692                      ; RGI_Emoji_ZWJ_Sequence  ; man firefighter: medium skin tone                              # E4.0   [1] (👨🏽‍🚒)
 1F468 1F3FD 200D 1F9AF                      ; RGI_Emoji_ZWJ_Sequence  ; man with white cane: medium skin tone                          # E12.0  [1] (👨🏽‍🦯)
+1F468 1F3FD 200D 1F9AF 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; man with white cane facing right: medium skin tone             # E15.1  [1] (👨🏽‍🦯‍➡️)
 1F468 1F3FD 200D 1F9BC                      ; RGI_Emoji_ZWJ_Sequence  ; man in motorized wheelchair: medium skin tone                  # E12.0  [1] (👨🏽‍🦼)
+1F468 1F3FD 200D 1F9BC 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; man in motorized wheelchair facing right: medium skin tone     # E15.1  [1] (👨🏽‍🦼‍➡️)
 1F468 1F3FD 200D 1F9BD                      ; RGI_Emoji_ZWJ_Sequence  ; man in manual wheelchair: medium skin tone                     # E12.0  [1] (👨🏽‍🦽)
+1F468 1F3FD 200D 1F9BD 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; man in manual wheelchair facing right: medium skin tone        # E15.1  [1] (👨🏽‍🦽‍➡️)
 1F468 1F3FE 200D 2695 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man health worker: medium-dark skin tone                       # E4.0   [1] (👨🏾‍⚕️)
 1F468 1F3FE 200D 2696 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man judge: medium-dark skin tone                               # E4.0   [1] (👨🏾‍⚖️)
 1F468 1F3FE 200D 2708 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man pilot: medium-dark skin tone                               # E4.0   [1] (👨🏾‍✈️)
 1F468 1F3FE 200D 1F33E                      ; RGI_Emoji_ZWJ_Sequence  ; man farmer: medium-dark skin tone                              # E4.0   [1] (👨🏾‍🌾)
 1F468 1F3FE 200D 1F373                      ; RGI_Emoji_ZWJ_Sequence  ; man cook: medium-dark skin tone                                # E4.0   [1] (👨🏾‍🍳)
 1F468 1F3FE 200D 1F37C                      ; RGI_Emoji_ZWJ_Sequence  ; man feeding baby: medium-dark skin tone                        # E13.0  [1] (👨🏾‍🍼)
 1F468 1F3FE 200D 1F393                      ; RGI_Emoji_ZWJ_Sequence  ; man student: medium-dark skin tone                             # E4.0   [1] (👨🏾‍🎓)
@@ -460,16 +477,19 @@
 1F468 1F3FE 200D 1F4BB                      ; RGI_Emoji_ZWJ_Sequence  ; man technologist: medium-dark skin tone                        # E4.0   [1] (👨🏾‍💻)
 1F468 1F3FE 200D 1F4BC                      ; RGI_Emoji_ZWJ_Sequence  ; man office worker: medium-dark skin tone                       # E4.0   [1] (👨🏾‍💼)
 1F468 1F3FE 200D 1F527                      ; RGI_Emoji_ZWJ_Sequence  ; man mechanic: medium-dark skin tone                            # E4.0   [1] (👨🏾‍🔧)
 1F468 1F3FE 200D 1F52C                      ; RGI_Emoji_ZWJ_Sequence  ; man scientist: medium-dark skin tone                           # E4.0   [1] (👨🏾‍🔬)
 1F468 1F3FE 200D 1F680                      ; RGI_Emoji_ZWJ_Sequence  ; man astronaut: medium-dark skin tone                           # E4.0   [1] (👨🏾‍🚀)
 1F468 1F3FE 200D 1F692                      ; RGI_Emoji_ZWJ_Sequence  ; man firefighter: medium-dark skin tone                         # E4.0   [1] (👨🏾‍🚒)
 1F468 1F3FE 200D 1F9AF                      ; RGI_Emoji_ZWJ_Sequence  ; man with white cane: medium-dark skin tone                     # E12.0  [1] (👨🏾‍🦯)
+1F468 1F3FE 200D 1F9AF 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; man with white cane facing right: medium-dark skin tone        # E15.1  [1] (👨🏾‍🦯‍➡️)
 1F468 1F3FE 200D 1F9BC                      ; RGI_Emoji_ZWJ_Sequence  ; man in motorized wheelchair: medium-dark skin tone             # E12.0  [1] (👨🏾‍🦼)
+1F468 1F3FE 200D 1F9BC 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; man in motorized wheelchair facing right: medium-dark skin tone #E15.1  [1] (👨🏾‍🦼‍➡️)
 1F468 1F3FE 200D 1F9BD                      ; RGI_Emoji_ZWJ_Sequence  ; man in manual wheelchair: medium-dark skin tone                # E12.0  [1] (👨🏾‍🦽)
+1F468 1F3FE 200D 1F9BD 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; man in manual wheelchair facing right: medium-dark skin tone   # E15.1  [1] (👨🏾‍🦽‍➡️)
 1F468 1F3FF 200D 2695 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man health worker: dark skin tone                              # E4.0   [1] (👨🏿‍⚕️)
 1F468 1F3FF 200D 2696 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man judge: dark skin tone                                      # E4.0   [1] (👨🏿‍⚖️)
 1F468 1F3FF 200D 2708 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man pilot: dark skin tone                                      # E4.0   [1] (👨🏿‍✈️)
 1F468 1F3FF 200D 1F33E                      ; RGI_Emoji_ZWJ_Sequence  ; man farmer: dark skin tone                                     # E4.0   [1] (👨🏿‍🌾)
 1F468 1F3FF 200D 1F373                      ; RGI_Emoji_ZWJ_Sequence  ; man cook: dark skin tone                                       # E4.0   [1] (👨🏿‍🍳)
 1F468 1F3FF 200D 1F37C                      ; RGI_Emoji_ZWJ_Sequence  ; man feeding baby: dark skin tone                               # E13.0  [1] (👨🏿‍🍼)
 1F468 1F3FF 200D 1F393                      ; RGI_Emoji_ZWJ_Sequence  ; man student: dark skin tone                                    # E4.0   [1] (👨🏿‍🎓)
@@ -480,16 +500,19 @@
 1F468 1F3FF 200D 1F4BB                      ; RGI_Emoji_ZWJ_Sequence  ; man technologist: dark skin tone                               # E4.0   [1] (👨🏿‍💻)
 1F468 1F3FF 200D 1F4BC                      ; RGI_Emoji_ZWJ_Sequence  ; man office worker: dark skin tone                              # E4.0   [1] (👨🏿‍💼)
 1F468 1F3FF 200D 1F527                      ; RGI_Emoji_ZWJ_Sequence  ; man mechanic: dark skin tone                                   # E4.0   [1] (👨🏿‍🔧)
 1F468 1F3FF 200D 1F52C                      ; RGI_Emoji_ZWJ_Sequence  ; man scientist: dark skin tone                                  # E4.0   [1] (👨🏿‍🔬)
 1F468 1F3FF 200D 1F680                      ; RGI_Emoji_ZWJ_Sequence  ; man astronaut: dark skin tone                                  # E4.0   [1] (👨🏿‍🚀)
 1F468 1F3FF 200D 1F692                      ; RGI_Emoji_ZWJ_Sequence  ; man firefighter: dark skin tone                                # E4.0   [1] (👨🏿‍🚒)
 1F468 1F3FF 200D 1F9AF                      ; RGI_Emoji_ZWJ_Sequence  ; man with white cane: dark skin tone                            # E12.0  [1] (👨🏿‍🦯)
+1F468 1F3FF 200D 1F9AF 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; man with white cane facing right: dark skin tone               # E15.1  [1] (👨🏿‍🦯‍➡️)
 1F468 1F3FF 200D 1F9BC                      ; RGI_Emoji_ZWJ_Sequence  ; man in motorized wheelchair: dark skin tone                    # E12.0  [1] (👨🏿‍🦼)
+1F468 1F3FF 200D 1F9BC 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; man in motorized wheelchair facing right: dark skin tone       # E15.1  [1] (👨🏿‍🦼‍➡️)
 1F468 1F3FF 200D 1F9BD                      ; RGI_Emoji_ZWJ_Sequence  ; man in manual wheelchair: dark skin tone                       # E12.0  [1] (👨🏿‍🦽)
+1F468 1F3FF 200D 1F9BD 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; man in manual wheelchair facing right: dark skin tone          # E15.1  [1] (👨🏿‍🦽‍➡️)
 1F469 200D 2695 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; woman health worker                                            # E4.0   [1] (👩‍⚕️)
 1F469 200D 2696 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; woman judge                                                    # E4.0   [1] (👩‍⚖️)
 1F469 200D 2708 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; woman pilot                                                    # E4.0   [1] (👩‍✈️)
 1F469 200D 1F33E                            ; RGI_Emoji_ZWJ_Sequence  ; woman farmer                                                   # E4.0   [1] (👩‍🌾)
 1F469 200D 1F373                            ; RGI_Emoji_ZWJ_Sequence  ; woman cook                                                     # E4.0   [1] (👩‍🍳)
 1F469 200D 1F37C                            ; RGI_Emoji_ZWJ_Sequence  ; woman feeding baby                                             # E13.0  [1] (👩‍🍼)
 1F469 200D 1F393                            ; RGI_Emoji_ZWJ_Sequence  ; woman student                                                  # E4.0   [1] (👩‍🎓)
@@ -500,16 +523,19 @@
 1F469 200D 1F4BB                            ; RGI_Emoji_ZWJ_Sequence  ; woman technologist                                             # E4.0   [1] (👩‍💻)
 1F469 200D 1F4BC                            ; RGI_Emoji_ZWJ_Sequence  ; woman office worker                                            # E4.0   [1] (👩‍💼)
 1F469 200D 1F527                            ; RGI_Emoji_ZWJ_Sequence  ; woman mechanic                                                 # E4.0   [1] (👩‍🔧)
 1F469 200D 1F52C                            ; RGI_Emoji_ZWJ_Sequence  ; woman scientist                                                # E4.0   [1] (👩‍🔬)
 1F469 200D 1F680                            ; RGI_Emoji_ZWJ_Sequence  ; woman astronaut                                                # E4.0   [1] (👩‍🚀)
 1F469 200D 1F692                            ; RGI_Emoji_ZWJ_Sequence  ; woman firefighter                                              # E4.0   [1] (👩‍🚒)
 1F469 200D 1F9AF                            ; RGI_Emoji_ZWJ_Sequence  ; woman with white cane                                          # E12.0  [1] (👩‍🦯)
+1F469 200D 1F9AF 200D 27A1 FE0F             ; RGI_Emoji_ZWJ_Sequence  ; woman with white cane facing right                             # E15.1  [1] (👩‍🦯‍➡️)
 1F469 200D 1F9BC                            ; RGI_Emoji_ZWJ_Sequence  ; woman in motorized wheelchair                                  # E12.0  [1] (👩‍🦼)
+1F469 200D 1F9BC 200D 27A1 FE0F             ; RGI_Emoji_ZWJ_Sequence  ; woman in motorized wheelchair facing right                     # E15.1  [1] (👩‍🦼‍➡️)
 1F469 200D 1F9BD                            ; RGI_Emoji_ZWJ_Sequence  ; woman in manual wheelchair                                     # E12.0  [1] (👩‍🦽)
+1F469 200D 1F9BD 200D 27A1 FE0F             ; RGI_Emoji_ZWJ_Sequence  ; woman in manual wheelchair facing right                        # E15.1  [1] (👩‍🦽‍➡️)
 1F469 1F3FB 200D 2695 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman health worker: light skin tone                           # E4.0   [1] (👩🏻‍⚕️)
 1F469 1F3FB 200D 2696 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman judge: light skin tone                                   # E4.0   [1] (👩🏻‍⚖️)
 1F469 1F3FB 200D 2708 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman pilot: light skin tone                                   # E4.0   [1] (👩🏻‍✈️)
 1F469 1F3FB 200D 1F33E                      ; RGI_Emoji_ZWJ_Sequence  ; woman farmer: light skin tone                                  # E4.0   [1] (👩🏻‍🌾)
 1F469 1F3FB 200D 1F373                      ; RGI_Emoji_ZWJ_Sequence  ; woman cook: light skin tone                                    # E4.0   [1] (👩🏻‍🍳)
 1F469 1F3FB 200D 1F37C                      ; RGI_Emoji_ZWJ_Sequence  ; woman feeding baby: light skin tone                            # E13.0  [1] (👩🏻‍🍼)
 1F469 1F3FB 200D 1F393                      ; RGI_Emoji_ZWJ_Sequence  ; woman student: light skin tone                                 # E4.0   [1] (👩🏻‍🎓)
@@ -520,16 +546,19 @@
 1F469 1F3FB 200D 1F4BB                      ; RGI_Emoji_ZWJ_Sequence  ; woman technologist: light skin tone                            # E4.0   [1] (👩🏻‍💻)
 1F469 1F3FB 200D 1F4BC                      ; RGI_Emoji_ZWJ_Sequence  ; woman office worker: light skin tone                           # E4.0   [1] (👩🏻‍💼)
 1F469 1F3FB 200D 1F527                      ; RGI_Emoji_ZWJ_Sequence  ; woman mechanic: light skin tone                                # E4.0   [1] (👩🏻‍🔧)
 1F469 1F3FB 200D 1F52C                      ; RGI_Emoji_ZWJ_Sequence  ; woman scientist: light skin tone                               # E4.0   [1] (👩🏻‍🔬)
 1F469 1F3FB 200D 1F680                      ; RGI_Emoji_ZWJ_Sequence  ; woman astronaut: light skin tone                               # E4.0   [1] (👩🏻‍🚀)
 1F469 1F3FB 200D 1F692                      ; RGI_Emoji_ZWJ_Sequence  ; woman firefighter: light skin tone                             # E4.0   [1] (👩🏻‍🚒)
 1F469 1F3FB 200D 1F9AF                      ; RGI_Emoji_ZWJ_Sequence  ; woman with white cane: light skin tone                         # E12.0  [1] (👩🏻‍🦯)
+1F469 1F3FB 200D 1F9AF 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; woman with white cane facing right: light skin tone            # E15.1  [1] (👩🏻‍🦯‍➡️)
 1F469 1F3FB 200D 1F9BC                      ; RGI_Emoji_ZWJ_Sequence  ; woman in motorized wheelchair: light skin tone                 # E12.0  [1] (👩🏻‍🦼)
+1F469 1F3FB 200D 1F9BC 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; woman in motorized wheelchair facing right: light skin tone    # E15.1  [1] (👩🏻‍🦼‍➡️)
 1F469 1F3FB 200D 1F9BD                      ; RGI_Emoji_ZWJ_Sequence  ; woman in manual wheelchair: light skin tone                    # E12.0  [1] (👩🏻‍🦽)
+1F469 1F3FB 200D 1F9BD 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; woman in manual wheelchair facing right: light skin tone       # E15.1  [1] (👩🏻‍🦽‍➡️)
 1F469 1F3FC 200D 2695 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman health worker: medium-light skin tone                    # E4.0   [1] (👩🏼‍⚕️)
 1F469 1F3FC 200D 2696 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman judge: medium-light skin tone                            # E4.0   [1] (👩🏼‍⚖️)
 1F469 1F3FC 200D 2708 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman pilot: medium-light skin tone                            # E4.0   [1] (👩🏼‍✈️)
 1F469 1F3FC 200D 1F33E                      ; RGI_Emoji_ZWJ_Sequence  ; woman farmer: medium-light skin tone                           # E4.0   [1] (👩🏼‍🌾)
 1F469 1F3FC 200D 1F373                      ; RGI_Emoji_ZWJ_Sequence  ; woman cook: medium-light skin tone                             # E4.0   [1] (👩🏼‍🍳)
 1F469 1F3FC 200D 1F37C                      ; RGI_Emoji_ZWJ_Sequence  ; woman feeding baby: medium-light skin tone                     # E13.0  [1] (👩🏼‍🍼)
 1F469 1F3FC 200D 1F393                      ; RGI_Emoji_ZWJ_Sequence  ; woman student: medium-light skin tone                          # E4.0   [1] (👩🏼‍🎓)
@@ -540,16 +569,19 @@
 1F469 1F3FC 200D 1F4BB                      ; RGI_Emoji_ZWJ_Sequence  ; woman technologist: medium-light skin tone                     # E4.0   [1] (👩🏼‍💻)
 1F469 1F3FC 200D 1F4BC                      ; RGI_Emoji_ZWJ_Sequence  ; woman office worker: medium-light skin tone                    # E4.0   [1] (👩🏼‍💼)
 1F469 1F3FC 200D 1F527                      ; RGI_Emoji_ZWJ_Sequence  ; woman mechanic: medium-light skin tone                         # E4.0   [1] (👩🏼‍🔧)
 1F469 1F3FC 200D 1F52C                      ; RGI_Emoji_ZWJ_Sequence  ; woman scientist: medium-light skin tone                        # E4.0   [1] (👩🏼‍🔬)
 1F469 1F3FC 200D 1F680                      ; RGI_Emoji_ZWJ_Sequence  ; woman astronaut: medium-light skin tone                        # E4.0   [1] (👩🏼‍🚀)
 1F469 1F3FC 200D 1F692                      ; RGI_Emoji_ZWJ_Sequence  ; woman firefighter: medium-light skin tone                      # E4.0   [1] (👩🏼‍🚒)
 1F469 1F3FC 200D 1F9AF                      ; RGI_Emoji_ZWJ_Sequence  ; woman with white cane: medium-light skin tone                  # E12.0  [1] (👩🏼‍🦯)
+1F469 1F3FC 200D 1F9AF 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; woman with white cane facing right: medium-light skin tone     # E15.1  [1] (👩🏼‍🦯‍➡️)
 1F469 1F3FC 200D 1F9BC                      ; RGI_Emoji_ZWJ_Sequence  ; woman in motorized wheelchair: medium-light skin tone          # E12.0  [1] (👩🏼‍🦼)
+1F469 1F3FC 200D 1F9BC 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; woman in motorized wheelchair facing right: medium-light skin tone #E15.1[1] (👩🏼‍🦼‍➡️)
 1F469 1F3FC 200D 1F9BD                      ; RGI_Emoji_ZWJ_Sequence  ; woman in manual wheelchair: medium-light skin tone             # E12.0  [1] (👩🏼‍🦽)
+1F469 1F3FC 200D 1F9BD 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; woman in manual wheelchair facing right: medium-light skin tone #E15.1  [1] (👩🏼‍🦽‍➡️)
 1F469 1F3FD 200D 2695 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman health worker: medium skin tone                          # E4.0   [1] (👩🏽‍⚕️)
 1F469 1F3FD 200D 2696 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman judge: medium skin tone                                  # E4.0   [1] (👩🏽‍⚖️)
 1F469 1F3FD 200D 2708 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman pilot: medium skin tone                                  # E4.0   [1] (👩🏽‍✈️)
 1F469 1F3FD 200D 1F33E                      ; RGI_Emoji_ZWJ_Sequence  ; woman farmer: medium skin tone                                 # E4.0   [1] (👩🏽‍🌾)
 1F469 1F3FD 200D 1F373                      ; RGI_Emoji_ZWJ_Sequence  ; woman cook: medium skin tone                                   # E4.0   [1] (👩🏽‍🍳)
 1F469 1F3FD 200D 1F37C                      ; RGI_Emoji_ZWJ_Sequence  ; woman feeding baby: medium skin tone                           # E13.0  [1] (👩🏽‍🍼)
 1F469 1F3FD 200D 1F393                      ; RGI_Emoji_ZWJ_Sequence  ; woman student: medium skin tone                                # E4.0   [1] (👩🏽‍🎓)
@@ -560,16 +592,19 @@
 1F469 1F3FD 200D 1F4BB                      ; RGI_Emoji_ZWJ_Sequence  ; woman technologist: medium skin tone                           # E4.0   [1] (👩🏽‍💻)
 1F469 1F3FD 200D 1F4BC                      ; RGI_Emoji_ZWJ_Sequence  ; woman office worker: medium skin tone                          # E4.0   [1] (👩🏽‍💼)
 1F469 1F3FD 200D 1F527                      ; RGI_Emoji_ZWJ_Sequence  ; woman mechanic: medium skin tone                               # E4.0   [1] (👩🏽‍🔧)
 1F469 1F3FD 200D 1F52C                      ; RGI_Emoji_ZWJ_Sequence  ; woman scientist: medium skin tone                              # E4.0   [1] (👩🏽‍🔬)
 1F469 1F3FD 200D 1F680                      ; RGI_Emoji_ZWJ_Sequence  ; woman astronaut: medium skin tone                              # E4.0   [1] (👩🏽‍🚀)
 1F469 1F3FD 200D 1F692                      ; RGI_Emoji_ZWJ_Sequence  ; woman firefighter: medium skin tone                            # E4.0   [1] (👩🏽‍🚒)
 1F469 1F3FD 200D 1F9AF                      ; RGI_Emoji_ZWJ_Sequence  ; woman with white cane: medium skin tone                        # E12.0  [1] (👩🏽‍🦯)
+1F469 1F3FD 200D 1F9AF 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; woman with white cane facing right: medium skin tone           # E15.1  [1] (👩🏽‍🦯‍➡️)
 1F469 1F3FD 200D 1F9BC                      ; RGI_Emoji_ZWJ_Sequence  ; woman in motorized wheelchair: medium skin tone                # E12.0  [1] (👩🏽‍🦼)
+1F469 1F3FD 200D 1F9BC 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; woman in motorized wheelchair facing right: medium skin tone   # E15.1  [1] (👩🏽‍🦼‍➡️)
 1F469 1F3FD 200D 1F9BD                      ; RGI_Emoji_ZWJ_Sequence  ; woman in manual wheelchair: medium skin tone                   # E12.0  [1] (👩🏽‍🦽)
+1F469 1F3FD 200D 1F9BD 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; woman in manual wheelchair facing right: medium skin tone      # E15.1  [1] (👩🏽‍🦽‍➡️)
 1F469 1F3FE 200D 2695 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman health worker: medium-dark skin tone                     # E4.0   [1] (👩🏾‍⚕️)
 1F469 1F3FE 200D 2696 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman judge: medium-dark skin tone                             # E4.0   [1] (👩🏾‍⚖️)
 1F469 1F3FE 200D 2708 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman pilot: medium-dark skin tone                             # E4.0   [1] (👩🏾‍✈️)
 1F469 1F3FE 200D 1F33E                      ; RGI_Emoji_ZWJ_Sequence  ; woman farmer: medium-dark skin tone                            # E4.0   [1] (👩🏾‍🌾)
 1F469 1F3FE 200D 1F373                      ; RGI_Emoji_ZWJ_Sequence  ; woman cook: medium-dark skin tone                              # E4.0   [1] (👩🏾‍🍳)
 1F469 1F3FE 200D 1F37C                      ; RGI_Emoji_ZWJ_Sequence  ; woman feeding baby: medium-dark skin tone                      # E13.0  [1] (👩🏾‍🍼)
 1F469 1F3FE 200D 1F393                      ; RGI_Emoji_ZWJ_Sequence  ; woman student: medium-dark skin tone                           # E4.0   [1] (👩🏾‍🎓)
@@ -580,16 +615,19 @@
 1F469 1F3FE 200D 1F4BB                      ; RGI_Emoji_ZWJ_Sequence  ; woman technologist: medium-dark skin tone                      # E4.0   [1] (👩🏾‍💻)
 1F469 1F3FE 200D 1F4BC                      ; RGI_Emoji_ZWJ_Sequence  ; woman office worker: medium-dark skin tone                     # E4.0   [1] (👩🏾‍💼)
 1F469 1F3FE 200D 1F527                      ; RGI_Emoji_ZWJ_Sequence  ; woman mechanic: medium-dark skin tone                          # E4.0   [1] (👩🏾‍🔧)
 1F469 1F3FE 200D 1F52C                      ; RGI_Emoji_ZWJ_Sequence  ; woman scientist: medium-dark skin tone                         # E4.0   [1] (👩🏾‍🔬)
 1F469 1F3FE 200D 1F680                      ; RGI_Emoji_ZWJ_Sequence  ; woman astronaut: medium-dark skin tone                         # E4.0   [1] (👩🏾‍🚀)
 1F469 1F3FE 200D 1F692                      ; RGI_Emoji_ZWJ_Sequence  ; woman firefighter: medium-dark skin tone                       # E4.0   [1] (👩🏾‍🚒)
 1F469 1F3FE 200D 1F9AF                      ; RGI_Emoji_ZWJ_Sequence  ; woman with white cane: medium-dark skin tone                   # E12.0  [1] (👩🏾‍🦯)
+1F469 1F3FE 200D 1F9AF 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; woman with white cane facing right: medium-dark skin tone      # E15.1  [1] (👩🏾‍🦯‍➡️)
 1F469 1F3FE 200D 1F9BC                      ; RGI_Emoji_ZWJ_Sequence  ; woman in motorized wheelchair: medium-dark skin tone           # E12.0  [1] (👩🏾‍🦼)
+1F469 1F3FE 200D 1F9BC 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; woman in motorized wheelchair facing right: medium-dark skin tone #E15.1[1] (👩🏾‍🦼‍➡️)
 1F469 1F3FE 200D 1F9BD                      ; RGI_Emoji_ZWJ_Sequence  ; woman in manual wheelchair: medium-dark skin tone              # E12.0  [1] (👩🏾‍🦽)
+1F469 1F3FE 200D 1F9BD 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; woman in manual wheelchair facing right: medium-dark skin tone # E15.1  [1] (👩🏾‍🦽‍➡️)
 1F469 1F3FF 200D 2695 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman health worker: dark skin tone                            # E4.0   [1] (👩🏿‍⚕️)
 1F469 1F3FF 200D 2696 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman judge: dark skin tone                                    # E4.0   [1] (👩🏿‍⚖️)
 1F469 1F3FF 200D 2708 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman pilot: dark skin tone                                    # E4.0   [1] (👩🏿‍✈️)
 1F469 1F3FF 200D 1F33E                      ; RGI_Emoji_ZWJ_Sequence  ; woman farmer: dark skin tone                                   # E4.0   [1] (👩🏿‍🌾)
 1F469 1F3FF 200D 1F373                      ; RGI_Emoji_ZWJ_Sequence  ; woman cook: dark skin tone                                     # E4.0   [1] (👩🏿‍🍳)
 1F469 1F3FF 200D 1F37C                      ; RGI_Emoji_ZWJ_Sequence  ; woman feeding baby: dark skin tone                             # E13.0  [1] (👩🏿‍🍼)
 1F469 1F3FF 200D 1F393                      ; RGI_Emoji_ZWJ_Sequence  ; woman student: dark skin tone                                  # E4.0   [1] (👩🏿‍🎓)
@@ -600,138 +638,177 @@
 1F469 1F3FF 200D 1F4BB                      ; RGI_Emoji_ZWJ_Sequence  ; woman technologist: dark skin tone                             # E4.0   [1] (👩🏿‍💻)
 1F469 1F3FF 200D 1F4BC                      ; RGI_Emoji_ZWJ_Sequence  ; woman office worker: dark skin tone                            # E4.0   [1] (👩🏿‍💼)
 1F469 1F3FF 200D 1F527                      ; RGI_Emoji_ZWJ_Sequence  ; woman mechanic: dark skin tone                                 # E4.0   [1] (👩🏿‍🔧)
 1F469 1F3FF 200D 1F52C                      ; RGI_Emoji_ZWJ_Sequence  ; woman scientist: dark skin tone                                # E4.0   [1] (👩🏿‍🔬)
 1F469 1F3FF 200D 1F680                      ; RGI_Emoji_ZWJ_Sequence  ; woman astronaut: dark skin tone                                # E4.0   [1] (👩🏿‍🚀)
 1F469 1F3FF 200D 1F692                      ; RGI_Emoji_ZWJ_Sequence  ; woman firefighter: dark skin tone                              # E4.0   [1] (👩🏿‍🚒)
 1F469 1F3FF 200D 1F9AF                      ; RGI_Emoji_ZWJ_Sequence  ; woman with white cane: dark skin tone                          # E12.0  [1] (👩🏿‍🦯)
+1F469 1F3FF 200D 1F9AF 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; woman with white cane facing right: dark skin tone             # E15.1  [1] (👩🏿‍🦯‍➡️)
 1F469 1F3FF 200D 1F9BC                      ; RGI_Emoji_ZWJ_Sequence  ; woman in motorized wheelchair: dark skin tone                  # E12.0  [1] (👩🏿‍🦼)
+1F469 1F3FF 200D 1F9BC 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; woman in motorized wheelchair facing right: dark skin tone     # E15.1  [1] (👩🏿‍🦼‍➡️)
 1F469 1F3FF 200D 1F9BD                      ; RGI_Emoji_ZWJ_Sequence  ; woman in manual wheelchair: dark skin tone                     # E12.0  [1] (👩🏿‍🦽)
+1F469 1F3FF 200D 1F9BD 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; woman in manual wheelchair facing right: dark skin tone        # E15.1  [1] (👩🏿‍🦽‍➡️)
+1F6B6 200D 27A1 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; person walking facing right                                    # E15.1  [1] (🚶‍➡️)
+1F6B6 1F3FB 200D 27A1 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; person walking facing right: light skin tone                   # E15.1  [1] (🚶🏻‍➡️)
+1F6B6 1F3FC 200D 27A1 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; person walking facing right: medium-light skin tone            # E15.1  [1] (🚶🏼‍➡️)
+1F6B6 1F3FD 200D 27A1 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; person walking facing right: medium skin tone                  # E15.1  [1] (🚶🏽‍➡️)
+1F6B6 1F3FE 200D 27A1 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; person walking facing right: medium-dark skin tone             # E15.1  [1] (🚶🏾‍➡️)
+1F6B6 1F3FF 200D 27A1 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; person walking facing right: dark skin tone                    # E15.1  [1] (🚶🏿‍➡️)
+1F9CE 200D 27A1 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; person kneeling facing right                                   # E15.1  [1] (🧎‍➡️)
+1F9CE 1F3FB 200D 27A1 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; person kneeling facing right: light skin tone                  # E15.1  [1] (🧎🏻‍➡️)
+1F9CE 1F3FC 200D 27A1 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; person kneeling facing right: medium-light skin tone           # E15.1  [1] (🧎🏼‍➡️)
+1F9CE 1F3FD 200D 27A1 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; person kneeling facing right: medium skin tone                 # E15.1  [1] (🧎🏽‍➡️)
+1F9CE 1F3FE 200D 27A1 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; person kneeling facing right: medium-dark skin tone            # E15.1  [1] (🧎🏾‍➡️)
+1F9CE 1F3FF 200D 27A1 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; person kneeling facing right: dark skin tone                   # E15.1  [1] (🧎🏿‍➡️)
 1F9D1 200D 2695 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; health worker                                                  # E12.1  [1] (🧑‍⚕️)
 1F9D1 200D 2696 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; judge                                                          # E12.1  [1] (🧑‍⚖️)
 1F9D1 200D 2708 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; pilot                                                          # E12.1  [1] (🧑‍✈️)
 1F9D1 200D 1F33E                            ; RGI_Emoji_ZWJ_Sequence  ; farmer                                                         # E12.1  [1] (🧑‍🌾)
 1F9D1 200D 1F373                            ; RGI_Emoji_ZWJ_Sequence  ; cook                                                           # E12.1  [1] (🧑‍🍳)
 1F9D1 200D 1F37C                            ; RGI_Emoji_ZWJ_Sequence  ; person feeding baby                                            # E13.0  [1] (🧑‍🍼)
+1F9D1 200D 1F384                            ; RGI_Emoji_ZWJ_Sequence  ; mx claus                                                       # E13.0  [1] (🧑‍🎄)
 1F9D1 200D 1F393                            ; RGI_Emoji_ZWJ_Sequence  ; student                                                        # E12.1  [1] (🧑‍🎓)
 1F9D1 200D 1F3A4                            ; RGI_Emoji_ZWJ_Sequence  ; singer                                                         # E12.1  [1] (🧑‍🎤)
 1F9D1 200D 1F3A8                            ; RGI_Emoji_ZWJ_Sequence  ; artist                                                         # E12.1  [1] (🧑‍🎨)
 1F9D1 200D 1F3EB                            ; RGI_Emoji_ZWJ_Sequence  ; teacher                                                        # E12.1  [1] (🧑‍🏫)
 1F9D1 200D 1F3ED                            ; RGI_Emoji_ZWJ_Sequence  ; factory worker                                                 # E12.1  [1] (🧑‍🏭)
 1F9D1 200D 1F4BB                            ; RGI_Emoji_ZWJ_Sequence  ; technologist                                                   # E12.1  [1] (🧑‍💻)
 1F9D1 200D 1F4BC                            ; RGI_Emoji_ZWJ_Sequence  ; office worker                                                  # E12.1  [1] (🧑‍💼)
 1F9D1 200D 1F527                            ; RGI_Emoji_ZWJ_Sequence  ; mechanic                                                       # E12.1  [1] (🧑‍🔧)
 1F9D1 200D 1F52C                            ; RGI_Emoji_ZWJ_Sequence  ; scientist                                                      # E12.1  [1] (🧑‍🔬)
 1F9D1 200D 1F680                            ; RGI_Emoji_ZWJ_Sequence  ; astronaut                                                      # E12.1  [1] (🧑‍🚀)
 1F9D1 200D 1F692                            ; RGI_Emoji_ZWJ_Sequence  ; firefighter                                                    # E12.1  [1] (🧑‍🚒)
 1F9D1 200D 1F9AF                            ; RGI_Emoji_ZWJ_Sequence  ; person with white cane                                         # E12.1  [1] (🧑‍🦯)
+1F9D1 200D 1F9AF 200D 27A1 FE0F             ; RGI_Emoji_ZWJ_Sequence  ; person with white cane facing right                            # E15.1  [1] (🧑‍🦯‍➡️)
 1F9D1 200D 1F9BC                            ; RGI_Emoji_ZWJ_Sequence  ; person in motorized wheelchair                                 # E12.1  [1] (🧑‍🦼)
+1F9D1 200D 1F9BC 200D 27A1 FE0F             ; RGI_Emoji_ZWJ_Sequence  ; person in motorized wheelchair facing right                    # E15.1  [1] (🧑‍🦼‍➡️)
 1F9D1 200D 1F9BD                            ; RGI_Emoji_ZWJ_Sequence  ; person in manual wheelchair                                    # E12.1  [1] (🧑‍🦽)
+1F9D1 200D 1F9BD 200D 27A1 FE0F             ; RGI_Emoji_ZWJ_Sequence  ; person in manual wheelchair facing right                       # E15.1  [1] (🧑‍🦽‍➡️)
 1F9D1 1F3FB 200D 2695 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; health worker: light skin tone                                 # E12.1  [1] (🧑🏻‍⚕️)
 1F9D1 1F3FB 200D 2696 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; judge: light skin tone                                         # E12.1  [1] (🧑🏻‍⚖️)
 1F9D1 1F3FB 200D 2708 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; pilot: light skin tone                                         # E12.1  [1] (🧑🏻‍✈️)
 1F9D1 1F3FB 200D 1F33E                      ; RGI_Emoji_ZWJ_Sequence  ; farmer: light skin tone                                        # E12.1  [1] (🧑🏻‍🌾)
 1F9D1 1F3FB 200D 1F373                      ; RGI_Emoji_ZWJ_Sequence  ; cook: light skin tone                                          # E12.1  [1] (🧑🏻‍🍳)
 1F9D1 1F3FB 200D 1F37C                      ; RGI_Emoji_ZWJ_Sequence  ; person feeding baby: light skin tone                           # E13.0  [1] (🧑🏻‍🍼)
+1F9D1 1F3FB 200D 1F384                      ; RGI_Emoji_ZWJ_Sequence  ; mx claus: light skin tone                                      # E13.0  [1] (🧑🏻‍🎄)
 1F9D1 1F3FB 200D 1F393                      ; RGI_Emoji_ZWJ_Sequence  ; student: light skin tone                                       # E12.1  [1] (🧑🏻‍🎓)
 1F9D1 1F3FB 200D 1F3A4                      ; RGI_Emoji_ZWJ_Sequence  ; singer: light skin tone                                        # E12.1  [1] (🧑🏻‍🎤)
 1F9D1 1F3FB 200D 1F3A8                      ; RGI_Emoji_ZWJ_Sequence  ; artist: light skin tone                                        # E12.1  [1] (🧑🏻‍🎨)
 1F9D1 1F3FB 200D 1F3EB                      ; RGI_Emoji_ZWJ_Sequence  ; teacher: light skin tone                                       # E12.1  [1] (🧑🏻‍🏫)
 1F9D1 1F3FB 200D 1F3ED                      ; RGI_Emoji_ZWJ_Sequence  ; factory worker: light skin tone                                # E12.1  [1] (🧑🏻‍🏭)
 1F9D1 1F3FB 200D 1F4BB                      ; RGI_Emoji_ZWJ_Sequence  ; technologist: light skin tone                                  # E12.1  [1] (🧑🏻‍💻)
 1F9D1 1F3FB 200D 1F4BC                      ; RGI_Emoji_ZWJ_Sequence  ; office worker: light skin tone                                 # E12.1  [1] (🧑🏻‍💼)
 1F9D1 1F3FB 200D 1F527                      ; RGI_Emoji_ZWJ_Sequence  ; mechanic: light skin tone                                      # E12.1  [1] (🧑🏻‍🔧)
 1F9D1 1F3FB 200D 1F52C                      ; RGI_Emoji_ZWJ_Sequence  ; scientist: light skin tone                                     # E12.1  [1] (🧑🏻‍🔬)
 1F9D1 1F3FB 200D 1F680                      ; RGI_Emoji_ZWJ_Sequence  ; astronaut: light skin tone                                     # E12.1  [1] (🧑🏻‍🚀)
 1F9D1 1F3FB 200D 1F692                      ; RGI_Emoji_ZWJ_Sequence  ; firefighter: light skin tone                                   # E12.1  [1] (🧑🏻‍🚒)
 1F9D1 1F3FB 200D 1F9AF                      ; RGI_Emoji_ZWJ_Sequence  ; person with white cane: light skin tone                        # E12.1  [1] (🧑🏻‍🦯)
+1F9D1 1F3FB 200D 1F9AF 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; person with white cane facing right: light skin tone           # E15.1  [1] (🧑🏻‍🦯‍➡️)
 1F9D1 1F3FB 200D 1F9BC                      ; RGI_Emoji_ZWJ_Sequence  ; person in motorized wheelchair: light skin tone                # E12.1  [1] (🧑🏻‍🦼)
+1F9D1 1F3FB 200D 1F9BC 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; person in motorized wheelchair facing right: light skin tone   # E15.1  [1] (🧑🏻‍🦼‍➡️)
 1F9D1 1F3FB 200D 1F9BD                      ; RGI_Emoji_ZWJ_Sequence  ; person in manual wheelchair: light skin tone                   # E12.1  [1] (🧑🏻‍🦽)
+1F9D1 1F3FB 200D 1F9BD 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; person in manual wheelchair facing right: light skin tone      # E15.1  [1] (🧑🏻‍🦽‍➡️)
 1F9D1 1F3FC 200D 2695 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; health worker: medium-light skin tone                          # E12.1  [1] (🧑🏼‍⚕️)
 1F9D1 1F3FC 200D 2696 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; judge: medium-light skin tone                                  # E12.1  [1] (🧑🏼‍⚖️)
 1F9D1 1F3FC 200D 2708 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; pilot: medium-light skin tone                                  # E12.1  [1] (🧑🏼‍✈️)
 1F9D1 1F3FC 200D 1F33E                      ; RGI_Emoji_ZWJ_Sequence  ; farmer: medium-light skin tone                                 # E12.1  [1] (🧑🏼‍🌾)
 1F9D1 1F3FC 200D 1F373                      ; RGI_Emoji_ZWJ_Sequence  ; cook: medium-light skin tone                                   # E12.1  [1] (🧑🏼‍🍳)
 1F9D1 1F3FC 200D 1F37C                      ; RGI_Emoji_ZWJ_Sequence  ; person feeding baby: medium-light skin tone                    # E13.0  [1] (🧑🏼‍🍼)
+1F9D1 1F3FC 200D 1F384                      ; RGI_Emoji_ZWJ_Sequence  ; mx claus: medium-light skin tone                               # E13.0  [1] (🧑🏼‍🎄)
 1F9D1 1F3FC 200D 1F393                      ; RGI_Emoji_ZWJ_Sequence  ; student: medium-light skin tone                                # E12.1  [1] (🧑🏼‍🎓)
 1F9D1 1F3FC 200D 1F3A4                      ; RGI_Emoji_ZWJ_Sequence  ; singer: medium-light skin tone                                 # E12.1  [1] (🧑🏼‍🎤)
 1F9D1 1F3FC 200D 1F3A8                      ; RGI_Emoji_ZWJ_Sequence  ; artist: medium-light skin tone                                 # E12.1  [1] (🧑🏼‍🎨)
 1F9D1 1F3FC 200D 1F3EB                      ; RGI_Emoji_ZWJ_Sequence  ; teacher: medium-light skin tone                                # E12.1  [1] (🧑🏼‍🏫)
 1F9D1 1F3FC 200D 1F3ED                      ; RGI_Emoji_ZWJ_Sequence  ; factory worker: medium-light skin tone                         # E12.1  [1] (🧑🏼‍🏭)
 1F9D1 1F3FC 200D 1F4BB                      ; RGI_Emoji_ZWJ_Sequence  ; technologist: medium-light skin tone                           # E12.1  [1] (🧑🏼‍💻)
 1F9D1 1F3FC 200D 1F4BC                      ; RGI_Emoji_ZWJ_Sequence  ; office worker: medium-light skin tone                          # E12.1  [1] (🧑🏼‍💼)
 1F9D1 1F3FC 200D 1F527                      ; RGI_Emoji_ZWJ_Sequence  ; mechanic: medium-light skin tone                               # E12.1  [1] (🧑🏼‍🔧)
 1F9D1 1F3FC 200D 1F52C                      ; RGI_Emoji_ZWJ_Sequence  ; scientist: medium-light skin tone                              # E12.1  [1] (🧑🏼‍🔬)
 1F9D1 1F3FC 200D 1F680                      ; RGI_Emoji_ZWJ_Sequence  ; astronaut: medium-light skin tone                              # E12.1  [1] (🧑🏼‍🚀)
 1F9D1 1F3FC 200D 1F692                      ; RGI_Emoji_ZWJ_Sequence  ; firefighter: medium-light skin tone                            # E12.1  [1] (🧑🏼‍🚒)
 1F9D1 1F3FC 200D 1F9AF                      ; RGI_Emoji_ZWJ_Sequence  ; person with white cane: medium-light skin tone                 # E12.1  [1] (🧑🏼‍🦯)
+1F9D1 1F3FC 200D 1F9AF 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; person with white cane facing right: medium-light skin tone    # E15.1  [1] (🧑🏼‍🦯‍➡️)
 1F9D1 1F3FC 200D 1F9BC                      ; RGI_Emoji_ZWJ_Sequence  ; person in motorized wheelchair: medium-light skin tone         # E12.1  [1] (🧑🏼‍🦼)
+1F9D1 1F3FC 200D 1F9BC 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; person in motorized wheelchair facing right: medium-light skin tone #E15.1[1] (🧑🏼‍🦼‍➡️)
 1F9D1 1F3FC 200D 1F9BD                      ; RGI_Emoji_ZWJ_Sequence  ; person in manual wheelchair: medium-light skin tone            # E12.1  [1] (🧑🏼‍🦽)
+1F9D1 1F3FC 200D 1F9BD 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; person in manual wheelchair facing right: medium-light skin tone #E15.1 [1] (🧑🏼‍🦽‍➡️)
 1F9D1 1F3FD 200D 2695 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; health worker: medium skin tone                                # E12.1  [1] (🧑🏽‍⚕️)
 1F9D1 1F3FD 200D 2696 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; judge: medium skin tone                                        # E12.1  [1] (🧑🏽‍⚖️)
 1F9D1 1F3FD 200D 2708 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; pilot: medium skin tone                                        # E12.1  [1] (🧑🏽‍✈️)
 1F9D1 1F3FD 200D 1F33E                      ; RGI_Emoji_ZWJ_Sequence  ; farmer: medium skin tone                                       # E12.1  [1] (🧑🏽‍🌾)
 1F9D1 1F3FD 200D 1F373                      ; RGI_Emoji_ZWJ_Sequence  ; cook: medium skin tone                                         # E12.1  [1] (🧑🏽‍🍳)
 1F9D1 1F3FD 200D 1F37C                      ; RGI_Emoji_ZWJ_Sequence  ; person feeding baby: medium skin tone                          # E13.0  [1] (🧑🏽‍🍼)
+1F9D1 1F3FD 200D 1F384                      ; RGI_Emoji_ZWJ_Sequence  ; mx claus: medium skin tone                                     # E13.0  [1] (🧑🏽‍🎄)
 1F9D1 1F3FD 200D 1F393                      ; RGI_Emoji_ZWJ_Sequence  ; student: medium skin tone                                      # E12.1  [1] (🧑🏽‍🎓)
 1F9D1 1F3FD 200D 1F3A4                      ; RGI_Emoji_ZWJ_Sequence  ; singer: medium skin tone                                       # E12.1  [1] (🧑🏽‍🎤)
 1F9D1 1F3FD 200D 1F3A8                      ; RGI_Emoji_ZWJ_Sequence  ; artist: medium skin tone                                       # E12.1  [1] (🧑🏽‍🎨)
 1F9D1 1F3FD 200D 1F3EB                      ; RGI_Emoji_ZWJ_Sequence  ; teacher: medium skin tone                                      # E12.1  [1] (🧑🏽‍🏫)
 1F9D1 1F3FD 200D 1F3ED                      ; RGI_Emoji_ZWJ_Sequence  ; factory worker: medium skin tone                               # E12.1  [1] (🧑🏽‍🏭)
 1F9D1 1F3FD 200D 1F4BB                      ; RGI_Emoji_ZWJ_Sequence  ; technologist: medium skin tone                                 # E12.1  [1] (🧑🏽‍💻)
 1F9D1 1F3FD 200D 1F4BC                      ; RGI_Emoji_ZWJ_Sequence  ; office worker: medium skin tone                                # E12.1  [1] (🧑🏽‍💼)
 1F9D1 1F3FD 200D 1F527                      ; RGI_Emoji_ZWJ_Sequence  ; mechanic: medium skin tone                                     # E12.1  [1] (🧑🏽‍🔧)
 1F9D1 1F3FD 200D 1F52C                      ; RGI_Emoji_ZWJ_Sequence  ; scientist: medium skin tone                                    # E12.1  [1] (🧑🏽‍🔬)
 1F9D1 1F3FD 200D 1F680                      ; RGI_Emoji_ZWJ_Sequence  ; astronaut: medium skin tone                                    # E12.1  [1] (🧑🏽‍🚀)
 1F9D1 1F3FD 200D 1F692                      ; RGI_Emoji_ZWJ_Sequence  ; firefighter: medium skin tone                                  # E12.1  [1] (🧑🏽‍🚒)
 1F9D1 1F3FD 200D 1F9AF                      ; RGI_Emoji_ZWJ_Sequence  ; person with white cane: medium skin tone                       # E12.1  [1] (🧑🏽‍🦯)
+1F9D1 1F3FD 200D 1F9AF 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; person with white cane facing right: medium skin tone          # E15.1  [1] (🧑🏽‍🦯‍➡️)
 1F9D1 1F3FD 200D 1F9BC                      ; RGI_Emoji_ZWJ_Sequence  ; person in motorized wheelchair: medium skin tone               # E12.1  [1] (🧑🏽‍🦼)
+1F9D1 1F3FD 200D 1F9BC 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; person in motorized wheelchair facing right: medium skin tone  # E15.1  [1] (🧑🏽‍🦼‍➡️)
 1F9D1 1F3FD 200D 1F9BD                      ; RGI_Emoji_ZWJ_Sequence  ; person in manual wheelchair: medium skin tone                  # E12.1  [1] (🧑🏽‍🦽)
+1F9D1 1F3FD 200D 1F9BD 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; person in manual wheelchair facing right: medium skin tone     # E15.1  [1] (🧑🏽‍🦽‍➡️)
 1F9D1 1F3FE 200D 2695 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; health worker: medium-dark skin tone                           # E12.1  [1] (🧑🏾‍⚕️)
 1F9D1 1F3FE 200D 2696 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; judge: medium-dark skin tone                                   # E12.1  [1] (🧑🏾‍⚖️)
 1F9D1 1F3FE 200D 2708 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; pilot: medium-dark skin tone                                   # E12.1  [1] (🧑🏾‍✈️)
 1F9D1 1F3FE 200D 1F33E                      ; RGI_Emoji_ZWJ_Sequence  ; farmer: medium-dark skin tone                                  # E12.1  [1] (🧑🏾‍🌾)
 1F9D1 1F3FE 200D 1F373                      ; RGI_Emoji_ZWJ_Sequence  ; cook: medium-dark skin tone                                    # E12.1  [1] (🧑🏾‍🍳)
 1F9D1 1F3FE 200D 1F37C                      ; RGI_Emoji_ZWJ_Sequence  ; person feeding baby: medium-dark skin tone                     # E13.0  [1] (🧑🏾‍🍼)
+1F9D1 1F3FE 200D 1F384                      ; RGI_Emoji_ZWJ_Sequence  ; mx claus: medium-dark skin tone                                # E13.0  [1] (🧑🏾‍🎄)
 1F9D1 1F3FE 200D 1F393                      ; RGI_Emoji_ZWJ_Sequence  ; student: medium-dark skin tone                                 # E12.1  [1] (🧑🏾‍🎓)
 1F9D1 1F3FE 200D 1F3A4                      ; RGI_Emoji_ZWJ_Sequence  ; singer: medium-dark skin tone                                  # E12.1  [1] (🧑🏾‍🎤)
 1F9D1 1F3FE 200D 1F3A8                      ; RGI_Emoji_ZWJ_Sequence  ; artist: medium-dark skin tone                                  # E12.1  [1] (🧑🏾‍🎨)
 1F9D1 1F3FE 200D 1F3EB                      ; RGI_Emoji_ZWJ_Sequence  ; teacher: medium-dark skin tone                                 # E12.1  [1] (🧑🏾‍🏫)
 1F9D1 1F3FE 200D 1F3ED                      ; RGI_Emoji_ZWJ_Sequence  ; factory worker: medium-dark skin tone                          # E12.1  [1] (🧑🏾‍🏭)
 1F9D1 1F3FE 200D 1F4BB                      ; RGI_Emoji_ZWJ_Sequence  ; technologist: medium-dark skin tone                            # E12.1  [1] (🧑🏾‍💻)
 1F9D1 1F3FE 200D 1F4BC                      ; RGI_Emoji_ZWJ_Sequence  ; office worker: medium-dark skin tone                           # E12.1  [1] (🧑🏾‍💼)
 1F9D1 1F3FE 200D 1F527                      ; RGI_Emoji_ZWJ_Sequence  ; mechanic: medium-dark skin tone                                # E12.1  [1] (🧑🏾‍🔧)
 1F9D1 1F3FE 200D 1F52C                      ; RGI_Emoji_ZWJ_Sequence  ; scientist: medium-dark skin tone                               # E12.1  [1] (🧑🏾‍🔬)
 1F9D1 1F3FE 200D 1F680                      ; RGI_Emoji_ZWJ_Sequence  ; astronaut: medium-dark skin tone                               # E12.1  [1] (🧑🏾‍🚀)
 1F9D1 1F3FE 200D 1F692                      ; RGI_Emoji_ZWJ_Sequence  ; firefighter: medium-dark skin tone                             # E12.1  [1] (🧑🏾‍🚒)
 1F9D1 1F3FE 200D 1F9AF                      ; RGI_Emoji_ZWJ_Sequence  ; person with white cane: medium-dark skin tone                  # E12.1  [1] (🧑🏾‍🦯)
+1F9D1 1F3FE 200D 1F9AF 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; person with white cane facing right: medium-dark skin tone     # E15.1  [1] (🧑🏾‍🦯‍➡️)
 1F9D1 1F3FE 200D 1F9BC                      ; RGI_Emoji_ZWJ_Sequence  ; person in motorized wheelchair: medium-dark skin tone          # E12.1  [1] (🧑🏾‍🦼)
+1F9D1 1F3FE 200D 1F9BC 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; person in motorized wheelchair facing right: medium-dark skin tone #E15.1[1] (🧑🏾‍🦼‍➡️)
 1F9D1 1F3FE 200D 1F9BD                      ; RGI_Emoji_ZWJ_Sequence  ; person in manual wheelchair: medium-dark skin tone             # E12.1  [1] (🧑🏾‍🦽)
+1F9D1 1F3FE 200D 1F9BD 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; person in manual wheelchair facing right: medium-dark skin tone #E15.1  [1] (🧑🏾‍🦽‍➡️)
 1F9D1 1F3FF 200D 2695 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; health worker: dark skin tone                                  # E12.1  [1] (🧑🏿‍⚕️)
 1F9D1 1F3FF 200D 2696 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; judge: dark skin tone                                          # E12.1  [1] (🧑🏿‍⚖️)
 1F9D1 1F3FF 200D 2708 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; pilot: dark skin tone                                          # E12.1  [1] (🧑🏿‍✈️)
 1F9D1 1F3FF 200D 1F33E                      ; RGI_Emoji_ZWJ_Sequence  ; farmer: dark skin tone                                         # E12.1  [1] (🧑🏿‍🌾)
 1F9D1 1F3FF 200D 1F373                      ; RGI_Emoji_ZWJ_Sequence  ; cook: dark skin tone                                           # E12.1  [1] (🧑🏿‍🍳)
 1F9D1 1F3FF 200D 1F37C                      ; RGI_Emoji_ZWJ_Sequence  ; person feeding baby: dark skin tone                            # E13.0  [1] (🧑🏿‍🍼)
+1F9D1 1F3FF 200D 1F384                      ; RGI_Emoji_ZWJ_Sequence  ; mx claus: dark skin tone                                       # E13.0  [1] (🧑🏿‍🎄)
 1F9D1 1F3FF 200D 1F393                      ; RGI_Emoji_ZWJ_Sequence  ; student: dark skin tone                                        # E12.1  [1] (🧑🏿‍🎓)
 1F9D1 1F3FF 200D 1F3A4                      ; RGI_Emoji_ZWJ_Sequence  ; singer: dark skin tone                                         # E12.1  [1] (🧑🏿‍🎤)
 1F9D1 1F3FF 200D 1F3A8                      ; RGI_Emoji_ZWJ_Sequence  ; artist: dark skin tone                                         # E12.1  [1] (🧑🏿‍🎨)
 1F9D1 1F3FF 200D 1F3EB                      ; RGI_Emoji_ZWJ_Sequence  ; teacher: dark skin tone                                        # E12.1  [1] (🧑🏿‍🏫)
 1F9D1 1F3FF 200D 1F3ED                      ; RGI_Emoji_ZWJ_Sequence  ; factory worker: dark skin tone                                 # E12.1  [1] (🧑🏿‍🏭)
 1F9D1 1F3FF 200D 1F4BB                      ; RGI_Emoji_ZWJ_Sequence  ; technologist: dark skin tone                                   # E12.1  [1] (🧑🏿‍💻)
 1F9D1 1F3FF 200D 1F4BC                      ; RGI_Emoji_ZWJ_Sequence  ; office worker: dark skin tone                                  # E12.1  [1] (🧑🏿‍💼)
 1F9D1 1F3FF 200D 1F527                      ; RGI_Emoji_ZWJ_Sequence  ; mechanic: dark skin tone                                       # E12.1  [1] (🧑🏿‍🔧)
 1F9D1 1F3FF 200D 1F52C                      ; RGI_Emoji_ZWJ_Sequence  ; scientist: dark skin tone                                      # E12.1  [1] (🧑🏿‍🔬)
 1F9D1 1F3FF 200D 1F680                      ; RGI_Emoji_ZWJ_Sequence  ; astronaut: dark skin tone                                      # E12.1  [1] (🧑🏿‍🚀)
 1F9D1 1F3FF 200D 1F692                      ; RGI_Emoji_ZWJ_Sequence  ; firefighter: dark skin tone                                    # E12.1  [1] (🧑🏿‍🚒)
 1F9D1 1F3FF 200D 1F9AF                      ; RGI_Emoji_ZWJ_Sequence  ; person with white cane: dark skin tone                         # E12.1  [1] (🧑🏿‍🦯)
+1F9D1 1F3FF 200D 1F9AF 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; person with white cane facing right: dark skin tone            # E15.1  [1] (🧑🏿‍🦯‍➡️)
 1F9D1 1F3FF 200D 1F9BC                      ; RGI_Emoji_ZWJ_Sequence  ; person in motorized wheelchair: dark skin tone                 # E12.1  [1] (🧑🏿‍🦼)
+1F9D1 1F3FF 200D 1F9BC 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; person in motorized wheelchair facing right: dark skin tone    # E15.1  [1] (🧑🏿‍🦼‍➡️)
 1F9D1 1F3FF 200D 1F9BD                      ; RGI_Emoji_ZWJ_Sequence  ; person in manual wheelchair: dark skin tone                    # E12.1  [1] (🧑🏿‍🦽)
+1F9D1 1F3FF 200D 1F9BD 200D 27A1 FE0F       ; RGI_Emoji_ZWJ_Sequence  ; person in manual wheelchair facing right: dark skin tone       # E15.1  [1] (🧑🏿‍🦽‍➡️)
 
-# Total elements: 360
+# Total elements: 438
 
 # ================================================
 
 # RGI_Emoji_ZWJ_Sequence: Gendered
 
 26F9 1F3FB 200D 2640 FE0F                   ; RGI_Emoji_ZWJ_Sequence  ; woman bouncing ball: light skin tone                           # E4.0   [1] (⛹🏻‍♀️)
 26F9 1F3FB 200D 2642 FE0F                   ; RGI_Emoji_ZWJ_Sequence  ; man bouncing ball: light skin tone                             # E4.0   [1] (⛹🏻‍♂️)
@@ -742,25 +819,37 @@
 26F9 1F3FE 200D 2640 FE0F                   ; RGI_Emoji_ZWJ_Sequence  ; woman bouncing ball: medium-dark skin tone                     # E4.0   [1] (⛹🏾‍♀️)
 26F9 1F3FE 200D 2642 FE0F                   ; RGI_Emoji_ZWJ_Sequence  ; man bouncing ball: medium-dark skin tone                       # E4.0   [1] (⛹🏾‍♂️)
 26F9 1F3FF 200D 2640 FE0F                   ; RGI_Emoji_ZWJ_Sequence  ; woman bouncing ball: dark skin tone                            # E4.0   [1] (⛹🏿‍♀️)
 26F9 1F3FF 200D 2642 FE0F                   ; RGI_Emoji_ZWJ_Sequence  ; man bouncing ball: dark skin tone                              # E4.0   [1] (⛹🏿‍♂️)
 26F9 FE0F 200D 2640 FE0F                    ; RGI_Emoji_ZWJ_Sequence  ; woman bouncing ball                                            # E4.0   [1] (⛹️‍♀️)
 26F9 FE0F 200D 2642 FE0F                    ; RGI_Emoji_ZWJ_Sequence  ; man bouncing ball                                              # E4.0   [1] (⛹️‍♂️)
 1F3C3 200D 2640 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; woman running                                                  # E4.0   [1] (🏃‍♀️)
+1F3C3 200D 2640 FE0F 200D 27A1 FE0F         ; RGI_Emoji_ZWJ_Sequence  ; woman running facing right                                     # E15.1  [1] (🏃‍♀️‍➡️)
 1F3C3 200D 2642 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; man running                                                    # E4.0   [1] (🏃‍♂️)
+1F3C3 200D 2642 FE0F 200D 27A1 FE0F         ; RGI_Emoji_ZWJ_Sequence  ; man running facing right                                       # E15.1  [1] (🏃‍♂️‍➡️)
 1F3C3 1F3FB 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman running: light skin tone                                 # E4.0   [1] (🏃🏻‍♀️)
+1F3C3 1F3FB 200D 2640 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; woman running facing right: light skin tone                    # E15.1  [1] (🏃🏻‍♀️‍➡️)
 1F3C3 1F3FB 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man running: light skin tone                                   # E4.0   [1] (🏃🏻‍♂️)
+1F3C3 1F3FB 200D 2642 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; man running facing right: light skin tone                      # E15.1  [1] (🏃🏻‍♂️‍➡️)
 1F3C3 1F3FC 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman running: medium-light skin tone                          # E4.0   [1] (🏃🏼‍♀️)
+1F3C3 1F3FC 200D 2640 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; woman running facing right: medium-light skin tone             # E15.1  [1] (🏃🏼‍♀️‍➡️)
 1F3C3 1F3FC 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man running: medium-light skin tone                            # E4.0   [1] (🏃🏼‍♂️)
+1F3C3 1F3FC 200D 2642 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; man running facing right: medium-light skin tone               # E15.1  [1] (🏃🏼‍♂️‍➡️)
 1F3C3 1F3FD 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman running: medium skin tone                                # E4.0   [1] (🏃🏽‍♀️)
+1F3C3 1F3FD 200D 2640 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; woman running facing right: medium skin tone                   # E15.1  [1] (🏃🏽‍♀️‍➡️)
 1F3C3 1F3FD 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man running: medium skin tone                                  # E4.0   [1] (🏃🏽‍♂️)
+1F3C3 1F3FD 200D 2642 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; man running facing right: medium skin tone                     # E15.1  [1] (🏃🏽‍♂️‍➡️)
 1F3C3 1F3FE 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman running: medium-dark skin tone                           # E4.0   [1] (🏃🏾‍♀️)
+1F3C3 1F3FE 200D 2640 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; woman running facing right: medium-dark skin tone              # E15.1  [1] (🏃🏾‍♀️‍➡️)
 1F3C3 1F3FE 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man running: medium-dark skin tone                             # E4.0   [1] (🏃🏾‍♂️)
+1F3C3 1F3FE 200D 2642 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; man running facing right: medium-dark skin tone                # E15.1  [1] (🏃🏾‍♂️‍➡️)
 1F3C3 1F3FF 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman running: dark skin tone                                  # E4.0   [1] (🏃🏿‍♀️)
+1F3C3 1F3FF 200D 2640 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; woman running facing right: dark skin tone                     # E15.1  [1] (🏃🏿‍♀️‍➡️)
 1F3C3 1F3FF 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man running: dark skin tone                                    # E4.0   [1] (🏃🏿‍♂️)
+1F3C3 1F3FF 200D 2642 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; man running facing right: dark skin tone                       # E15.1  [1] (🏃🏿‍♂️‍➡️)
 1F3C4 200D 2640 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; woman surfing                                                  # E4.0   [1] (🏄‍♀️)
 1F3C4 200D 2642 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; man surfing                                                    # E4.0   [1] (🏄‍♂️)
 1F3C4 1F3FB 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman surfing: light skin tone                                 # E4.0   [1] (🏄🏻‍♀️)
 1F3C4 1F3FB 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man surfing: light skin tone                                   # E4.0   [1] (🏄🏻‍♂️)
 1F3C4 1F3FC 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman surfing: medium-light skin tone                          # E4.0   [1] (🏄🏼‍♀️)
 1F3C4 1F3FC 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man surfing: medium-light skin tone                            # E4.0   [1] (🏄🏼‍♂️)
 1F3C4 1F3FD 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman surfing: medium skin tone                                # E4.0   [1] (🏄🏽‍♀️)
@@ -1032,25 +1121,37 @@
 1F6B5 1F3FD 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman mountain biking: medium skin tone                        # E4.0   [1] (🚵🏽‍♀️)
 1F6B5 1F3FD 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man mountain biking: medium skin tone                          # E4.0   [1] (🚵🏽‍♂️)
 1F6B5 1F3FE 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman mountain biking: medium-dark skin tone                   # E4.0   [1] (🚵🏾‍♀️)
 1F6B5 1F3FE 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man mountain biking: medium-dark skin tone                     # E4.0   [1] (🚵🏾‍♂️)
 1F6B5 1F3FF 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman mountain biking: dark skin tone                          # E4.0   [1] (🚵🏿‍♀️)
 1F6B5 1F3FF 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man mountain biking: dark skin tone                            # E4.0   [1] (🚵🏿‍♂️)
 1F6B6 200D 2640 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; woman walking                                                  # E4.0   [1] (🚶‍♀️)
+1F6B6 200D 2640 FE0F 200D 27A1 FE0F         ; RGI_Emoji_ZWJ_Sequence  ; woman walking facing right                                     # E15.1  [1] (🚶‍♀️‍➡️)
 1F6B6 200D 2642 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; man walking                                                    # E4.0   [1] (🚶‍♂️)
+1F6B6 200D 2642 FE0F 200D 27A1 FE0F         ; RGI_Emoji_ZWJ_Sequence  ; man walking facing right                                       # E15.1  [1] (🚶‍♂️‍➡️)
 1F6B6 1F3FB 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman walking: light skin tone                                 # E4.0   [1] (🚶🏻‍♀️)
+1F6B6 1F3FB 200D 2640 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; woman walking facing right: light skin tone                    # E15.1  [1] (🚶🏻‍♀️‍➡️)
 1F6B6 1F3FB 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man walking: light skin tone                                   # E4.0   [1] (🚶🏻‍♂️)
+1F6B6 1F3FB 200D 2642 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; man walking facing right: light skin tone                      # E15.1  [1] (🚶🏻‍♂️‍➡️)
 1F6B6 1F3FC 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman walking: medium-light skin tone                          # E4.0   [1] (🚶🏼‍♀️)
+1F6B6 1F3FC 200D 2640 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; woman walking facing right: medium-light skin tone             # E15.1  [1] (🚶🏼‍♀️‍➡️)
 1F6B6 1F3FC 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man walking: medium-light skin tone                            # E4.0   [1] (🚶🏼‍♂️)
+1F6B6 1F3FC 200D 2642 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; man walking facing right: medium-light skin tone               # E15.1  [1] (🚶🏼‍♂️‍➡️)
 1F6B6 1F3FD 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman walking: medium skin tone                                # E4.0   [1] (🚶🏽‍♀️)
+1F6B6 1F3FD 200D 2640 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; woman walking facing right: medium skin tone                   # E15.1  [1] (🚶🏽‍♀️‍➡️)
 1F6B6 1F3FD 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man walking: medium skin tone                                  # E4.0   [1] (🚶🏽‍♂️)
+1F6B6 1F3FD 200D 2642 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; man walking facing right: medium skin tone                     # E15.1  [1] (🚶🏽‍♂️‍➡️)
 1F6B6 1F3FE 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman walking: medium-dark skin tone                           # E4.0   [1] (🚶🏾‍♀️)
+1F6B6 1F3FE 200D 2640 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; woman walking facing right: medium-dark skin tone              # E15.1  [1] (🚶🏾‍♀️‍➡️)
 1F6B6 1F3FE 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man walking: medium-dark skin tone                             # E4.0   [1] (🚶🏾‍♂️)
+1F6B6 1F3FE 200D 2642 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; man walking facing right: medium-dark skin tone                # E15.1  [1] (🚶🏾‍♂️‍➡️)
 1F6B6 1F3FF 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman walking: dark skin tone                                  # E4.0   [1] (🚶🏿‍♀️)
+1F6B6 1F3FF 200D 2640 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; woman walking facing right: dark skin tone                     # E15.1  [1] (🚶🏿‍♀️‍➡️)
 1F6B6 1F3FF 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man walking: dark skin tone                                    # E4.0   [1] (🚶🏿‍♂️)
+1F6B6 1F3FF 200D 2642 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; man walking facing right: dark skin tone                       # E15.1  [1] (🚶🏿‍♂️‍➡️)
 1F926 200D 2640 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; woman facepalming                                              # E4.0   [1] (🤦‍♀️)
 1F926 200D 2642 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; man facepalming                                                # E4.0   [1] (🤦‍♂️)
 1F926 1F3FB 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman facepalming: light skin tone                             # E4.0   [1] (🤦🏻‍♀️)
 1F926 1F3FB 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man facepalming: light skin tone                               # E4.0   [1] (🤦🏻‍♂️)
 1F926 1F3FC 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman facepalming: medium-light skin tone                      # E4.0   [1] (🤦🏼‍♀️)
 1F926 1F3FC 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man facepalming: medium-light skin tone                        # E4.0   [1] (🤦🏼‍♂️)
 1F926 1F3FD 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman facepalming: medium skin tone                            # E4.0   [1] (🤦🏽‍♀️)
@@ -1166,25 +1267,37 @@
 1F9CD 1F3FD 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman standing: medium skin tone                               # E12.0  [1] (🧍🏽‍♀️)
 1F9CD 1F3FD 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man standing: medium skin tone                                 # E12.0  [1] (🧍🏽‍♂️)
 1F9CD 1F3FE 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman standing: medium-dark skin tone                          # E12.0  [1] (🧍🏾‍♀️)
 1F9CD 1F3FE 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man standing: medium-dark skin tone                            # E12.0  [1] (🧍🏾‍♂️)
 1F9CD 1F3FF 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman standing: dark skin tone                                 # E12.0  [1] (🧍🏿‍♀️)
 1F9CD 1F3FF 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man standing: dark skin tone                                   # E12.0  [1] (🧍🏿‍♂️)
 1F9CE 200D 2640 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; woman kneeling                                                 # E12.0  [1] (🧎‍♀️)
+1F9CE 200D 2640 FE0F 200D 27A1 FE0F         ; RGI_Emoji_ZWJ_Sequence  ; woman kneeling facing right                                    # E15.1  [1] (🧎‍♀️‍➡️)
 1F9CE 200D 2642 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; man kneeling                                                   # E12.0  [1] (🧎‍♂️)
+1F9CE 200D 2642 FE0F 200D 27A1 FE0F         ; RGI_Emoji_ZWJ_Sequence  ; man kneeling facing right                                      # E15.1  [1] (🧎‍♂️‍➡️)
 1F9CE 1F3FB 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman kneeling: light skin tone                                # E12.0  [1] (🧎🏻‍♀️)
+1F9CE 1F3FB 200D 2640 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; woman kneeling facing right: light skin tone                   # E15.1  [1] (🧎🏻‍♀️‍➡️)
 1F9CE 1F3FB 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man kneeling: light skin tone                                  # E12.0  [1] (🧎🏻‍♂️)
+1F9CE 1F3FB 200D 2642 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; man kneeling facing right: light skin tone                     # E15.1  [1] (🧎🏻‍♂️‍➡️)
 1F9CE 1F3FC 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman kneeling: medium-light skin tone                         # E12.0  [1] (🧎🏼‍♀️)
+1F9CE 1F3FC 200D 2640 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; woman kneeling facing right: medium-light skin tone            # E15.1  [1] (🧎🏼‍♀️‍➡️)
 1F9CE 1F3FC 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man kneeling: medium-light skin tone                           # E12.0  [1] (🧎🏼‍♂️)
+1F9CE 1F3FC 200D 2642 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; man kneeling facing right: medium-light skin tone              # E15.1  [1] (🧎🏼‍♂️‍➡️)
 1F9CE 1F3FD 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman kneeling: medium skin tone                               # E12.0  [1] (🧎🏽‍♀️)
+1F9CE 1F3FD 200D 2640 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; woman kneeling facing right: medium skin tone                  # E15.1  [1] (🧎🏽‍♀️‍➡️)
 1F9CE 1F3FD 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man kneeling: medium skin tone                                 # E12.0  [1] (🧎🏽‍♂️)
+1F9CE 1F3FD 200D 2642 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; man kneeling facing right: medium skin tone                    # E15.1  [1] (🧎🏽‍♂️‍➡️)
 1F9CE 1F3FE 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman kneeling: medium-dark skin tone                          # E12.0  [1] (🧎🏾‍♀️)
+1F9CE 1F3FE 200D 2640 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; woman kneeling facing right: medium-dark skin tone             # E15.1  [1] (🧎🏾‍♀️‍➡️)
 1F9CE 1F3FE 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man kneeling: medium-dark skin tone                            # E12.0  [1] (🧎🏾‍♂️)
+1F9CE 1F3FE 200D 2642 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; man kneeling facing right: medium-dark skin tone               # E15.1  [1] (🧎🏾‍♂️‍➡️)
 1F9CE 1F3FF 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman kneeling: dark skin tone                                 # E12.0  [1] (🧎🏿‍♀️)
+1F9CE 1F3FF 200D 2640 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; woman kneeling facing right: dark skin tone                    # E15.1  [1] (🧎🏿‍♀️‍➡️)
 1F9CE 1F3FF 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man kneeling: dark skin tone                                   # E12.0  [1] (🧎🏿‍♂️)
+1F9CE 1F3FF 200D 2642 FE0F 200D 27A1 FE0F   ; RGI_Emoji_ZWJ_Sequence  ; man kneeling facing right: dark skin tone                      # E15.1  [1] (🧎🏿‍♂️‍➡️)
 1F9CF 200D 2640 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; deaf woman                                                     # E12.0  [1] (🧏‍♀️)
 1F9CF 200D 2642 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; deaf man                                                       # E12.0  [1] (🧏‍♂️)
 1F9CF 1F3FB 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; deaf woman: light skin tone                                    # E12.0  [1] (🧏🏻‍♀️)
 1F9CF 1F3FB 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; deaf man: light skin tone                                      # E12.0  [1] (🧏🏻‍♂️)
 1F9CF 1F3FC 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; deaf woman: medium-light skin tone                             # E12.0  [1] (🧏🏼‍♀️)
 1F9CF 1F3FC 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; deaf man: medium-light skin tone                               # E12.0  [1] (🧏🏼‍♂️)
 1F9CF 1F3FD 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; deaf woman: medium skin tone                                   # E12.0  [1] (🧏🏽‍♀️)
@@ -1302,15 +1415,15 @@
 1F9DD 1F3FF 200D 2640 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; woman elf: dark skin tone                                      # E5.0   [1] (🧝🏿‍♀️)
 1F9DD 1F3FF 200D 2642 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; man elf: dark skin tone                                        # E5.0   [1] (🧝🏿‍♂️)
 1F9DE 200D 2640 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; woman genie                                                    # E5.0   [1] (🧞‍♀️)
 1F9DE 200D 2642 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; man genie                                                      # E5.0   [1] (🧞‍♂️)
 1F9DF 200D 2640 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; woman zombie                                                   # E5.0   [1] (🧟‍♀️)
 1F9DF 200D 2642 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; man zombie                                                     # E5.0   [1] (🧟‍♂️)
 
-# Total elements: 572
+# Total elements: 608
 
 # ================================================
 
 # RGI_Emoji_ZWJ_Sequence: Hair
 
 1F468 200D 1F9B0                            ; RGI_Emoji_ZWJ_Sequence  ; man: red hair                                                  # E11.0  [1] (👨‍🦰)
 1F468 200D 1F9B1                            ; RGI_Emoji_ZWJ_Sequence  ; man: curly hair                                                # E11.0  [1] (👨‍🦱)
@@ -1387,25 +1500,30 @@
 
 # Total elements: 72
 
 # ================================================
 
 # RGI_Emoji_ZWJ_Sequence: Other
 
+26D3 FE0F 200D 1F4A5                        ; RGI_Emoji_ZWJ_Sequence  ; broken chain                                                   # E15.1  [1] (⛓️‍💥)
 2764 FE0F 200D 1F525                        ; RGI_Emoji_ZWJ_Sequence  ; heart on fire                                                  # E13.1  [1] (❤️‍🔥)
 2764 FE0F 200D 1FA79                        ; RGI_Emoji_ZWJ_Sequence  ; mending heart                                                  # E13.1  [1] (❤️‍🩹)
+1F344 200D 1F7EB                            ; RGI_Emoji_ZWJ_Sequence  ; brown mushroom                                                 # E15.1  [1] (🍄‍🟫)
+1F34B 200D 1F7E9                            ; RGI_Emoji_ZWJ_Sequence  ; lime                                                           # E15.1  [1] (🍋‍🟩)
 1F3F3 FE0F 200D 26A7 FE0F                   ; RGI_Emoji_ZWJ_Sequence  ; transgender flag                                               # E13.0  [1] (🏳️‍⚧️)
 1F3F3 FE0F 200D 1F308                       ; RGI_Emoji_ZWJ_Sequence  ; rainbow flag                                                   # E4.0   [1] (🏳️‍🌈)
 1F3F4 200D 2620 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; pirate flag                                                    # E11.0  [1] (🏴‍☠️)
 1F408 200D 2B1B                             ; RGI_Emoji_ZWJ_Sequence  ; black cat                                                      # E13.0  [1] (🐈‍⬛)
 1F415 200D 1F9BA                            ; RGI_Emoji_ZWJ_Sequence  ; service dog                                                    # E12.0  [1] (🐕‍🦺)
 1F426 200D 2B1B                             ; RGI_Emoji_ZWJ_Sequence  ; black bird                                                     # E15.0  [1] (🐦‍⬛)
+1F426 200D 1F525                            ; RGI_Emoji_ZWJ_Sequence  ; phoenix                                                        # E15.1  [1] (🐦‍🔥)
 1F43B 200D 2744 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; polar bear                                                     # E13.0  [1] (🐻‍❄️)
 1F441 FE0F 200D 1F5E8 FE0F                  ; RGI_Emoji_ZWJ_Sequence  ; eye in speech bubble                                           # E2.0   [1] (👁️‍🗨️)
 1F62E 200D 1F4A8                            ; RGI_Emoji_ZWJ_Sequence  ; face exhaling                                                  # E13.1  [1] (😮‍💨)
 1F635 200D 1F4AB                            ; RGI_Emoji_ZWJ_Sequence  ; face with spiral eyes                                          # E13.1  [1] (😵‍💫)
 1F636 200D 1F32B FE0F                       ; RGI_Emoji_ZWJ_Sequence  ; face in clouds                                                 # E13.1  [1] (😶‍🌫️)
-1F9D1 200D 1F384                            ; RGI_Emoji_ZWJ_Sequence  ; mx claus                                                       # E13.0  [1] (🧑‍🎄)
+1F642 200D 2194 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; head shaking horizontally                                      # E15.1  [1] (🙂‍↔️)
+1F642 200D 2195 FE0F                        ; RGI_Emoji_ZWJ_Sequence  ; head shaking vertically                                        # E15.1  [1] (🙂‍↕️)
 
-# Total elements: 14
+# Total elements: 19
 
 #EOF
```

### Comparing `emoji-data-0.2.post2/src/emoji_data/sequence.py` & `emoji_data-0.3/src/emoji_data/sequence.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,300 +1,331 @@
+from __future__ import annotations
+
 import re
-from typing import Iterable, List, Tuple, Union
+import sys
+from typing import Pattern, Union
+
+if sys.version_info < (3, 11):  # pragma: no cover
+    from typing_extensions import Self
+else:  # pragma: no cover
+    from typing import Self
+
+if sys.version_info < (3, 9):  # pragma: no cover
+    from typing import Iterable, Sequence, Tuple, Generator
+else:  # pragma: no cover
+    from collections.abc import Iterable, Sequence, Generator
 
-from . import version
 from .character import EmojiCharacter
 from .types import BaseDictContainer
-from .utils import read_data_file_iterable, resources_files
-
-__all__ = ['EmojiSequence']
+from .utils import data_file, read_data_file_iterable
 
+__all__ = ["EmojiSequence"]
 
-DATA_FILES = {
-    'zwj-sequences': 'emoji-zwj-sequences.txt',
-    'sequences': 'emoji-sequences.txt',
-    'variation-sequences': 'emoji-variation-sequences.txt',
-    'test': 'emoji-test.txt',
-}
+# http://www.unicode.org/reports/tr51/#Data_Files_Table
+# keep the order!
+DATA_FILES = [
+    "emoji-variation-sequences.txt",
+    "emoji-zwj-sequences.txt",
+    "emoji-sequences.txt",
+]
 
 
-class _MetaClass(BaseDictContainer):
+class MetaClass(BaseDictContainer):
     pass
 
 
-class EmojiSequence(metaclass=_MetaClass):
+class EmojiSequence(metaclass=MetaClass):
     """Emoji and Text Presentation Sequences used to represent emoji
 
-    see: http://www.unicode.org/reports/tr51/#Emoji_Variation_Sequences
+    see: http://www.unicode.org/reports/tr51/#Emoji_Sequences
     """
 
-    def __init__(self,
-                 code_points: Union[Iterable[int], int],
-                 status: str = '',
-                 type_field: str = '',
-                 description: str = '',
-                 comment: str = ''):
+    def __init__(
+        self,
+        code_points: Union[Iterable[int], int],
+        type_field: str = "",
+        description: str = "",
+        comment: str = "",
+    ):
         if isinstance(code_points, Iterable):
             self._code_points = list(code_points)
         else:
             self._code_points = [code_points]
-        self._status = status.strip()
-        self._string = ''.join(chr(n) for n in self._code_points)
+        self._string = "".join(chr(n) for n in self._code_points)
         self._characters = [EmojiCharacter.from_hex(n) for n in self._code_points]
         self._type_field = type_field.strip()
         self._comment = comment.strip()
         self._description = description
         # regex
-        self._regex = r''
+        self._regex = r""
         if not self._regex:
-            self._regex = ''.join(m.regex for m in self._characters)
-        self._regex_compiled = re.compile(self._regex)
+            self._regex = "".join(m.regex for m in self._characters)
+        self._regex_pat = re.compile(self._regex)
 
     def __len__(self):
         return len(self._code_points)
 
     def __str__(self):
         return self._string
 
     def __repr__(self):
-        return '<{} code_points={!r} status={!r}, string={!r}, description={!r}>'.format(
+        return "<{} code_points={!r} string={!r}, description={!r}>".format(
             type(self).__name__,
-            ' '.join('{:04X}'.format(n) for n in self._code_points),
-            self._status,
-            self._string,
-            self._description
+            self.code_points_string,
+            self.string,
+            self.description,
         )
 
     _initialed = False
 
-    pattern = re.compile(r'')
-    """Compiled regular express pattern object for all-together Emoji sequences.
+    pattern: Pattern
+    """Compiled regular expression pattern object for all-together Emoji sequences.
     """
 
     @classmethod
     def initial(cls):
         """Initial the class
 
         Load Emoji Sequences from package data file into class internal dictionary
         """
         if cls._initialed:
             return
         EmojiCharacter.initial()
-        for data_name, data_file in DATA_FILES.items():
-            with resources_files(version.__package__).joinpath('data', data_file).open(encoding='utf8') as fp:
+
+        def _decode_code_points(_cps, **_kwargs):
+            try:
+                _cp_head, _cp_tail = _cps.split("..", 1)  # begin..end form
+            except ValueError:
+                _arr_cp = [int(x, 16) for x in _cps.split()]
+                _seq = cls(_arr_cp, **_kwargs)
+                cls[_seq.string] = _seq
+            else:
+                # begin..end form: A range of single char emoji-seq
+                for _cp in range(int(_cp_head, 16), 1 + int(_cp_tail, 16)):
+                    _seq = cls(_cp, **_kwargs)
+                    cls[_seq.string] = _seq
+
+        for fname in DATA_FILES:
+            with data_file(fname).open(encoding="utf8") as fp:
                 for content, comment in read_data_file_iterable(fp):
-                    if data_name == 'test':
-                        cps, status = (part.strip() for part in content.split(';', 1))
-                        code_points = [int(cp, 16) for cp in cps.split()]
-                        inst = cls(code_points, status=status, comment=comment)
-                        s = inst.string
-                        try:
-                            existed_inst = cls[s]
-                        except KeyError:
-                            cls[s] = inst
-                        else:
-                            existed_inst.status = status
+                    if fname in ("emoji-sequences.txt", "emoji-zwj-sequences.txt"):
+                        cps, type_field, description = (part.strip() for part in content.split(";", 2))
+                        _decode_code_points(cps, type_field=type_field, description=description, comment=comment)
+                    elif fname == "emoji-variation-sequences.txt":
+                        cps, description = (part.strip() for part in content.split(";", 1))
+                        _decode_code_points(cps, description=description, comment=comment)
                     else:
-                        cps, type_field, description = (part.strip() for part in content.split(';', 2))
-                        # codes ...
-                        try:
-                            cp_head, cp_tail = cps.split('..', 1)  # begin..end form
-                        except ValueError:
-                            code_points = [int(cp, 16) for cp in cps.split()]
-                            inst = cls(code_points, type_field, '', description, comment)
-                            text = inst.string
-                            if text not in cls:
-                                cls[text] = inst
-                        else:
-                            # A range of single char emoji-seq
-                            for cp in range(int(cp_head, 16), 1 + int(cp_tail, 16)):
-                                inst = cls(cp, type_field, '', description, comment)
-                                if inst.string not in cls:
-                                    cls[inst.string] = inst
+                        raise RuntimeError(f"Invalid data file name {fname}")
         # build regex
-        ordered_list = sorted((m for m in cls.values()), key=lambda x: len(x.code_points), reverse=True)
-        exp = r'|'.join(m.regex for m in ordered_list)
-        cls.pattern = re.compile(exp)
+        cls.pattern = re.compile(
+            r"|".join(m.regex for m in sorted((m for m in cls.values()), key=lambda x: len(x.code_points), reverse=True))
+        )
         # initialed OK
         cls._initialed = True
 
     @classmethod
     def release(cls):
         if not cls._initialed:
             return
         keys = list(cls)
         for k in keys:
             del cls[k]
         cls._initialed = False
 
+    if sys.version_info < (3, 9):
+
+        @classmethod
+        def items(cls) -> Iterable[Tuple[str, Self]]:
+            return ((k, cls[k]) for k in cls)
+
+    else:
+
+        @classmethod
+        def items(cls) -> Iterable[tuple[str, Self]]:
+            """Return an iterator of all string -> emoji-sequence pairs of the class"""
+            return ((k, cls[k]) for k in cls)
+
     @classmethod
-    def items(cls) -> Iterable[Tuple[str, 'EmojiSequence']]:
-        """Return an iterator of all string -> emoji-sequence pairs of the class
-        """
-        return ((k, cls[k]) for k in cls)
+    def keys(cls) -> Iterable[str]:
+        """Return an iterator of each emoji-sequence's key string of the class"""
+        return (k for k in cls)
 
     @classmethod
-    def values(cls) -> Iterable['EmojiSequence']:
-        """Return an iterator of all emoji-sequences of the class
-        """
+    def values(cls) -> Iterable[Self]:
+        """Return an iterator of all emoji-sequences of the class"""
         return (cls[k] for k in cls)
 
     @classmethod
-    def from_text(cls, value: str) -> 'EmojiSequence':
-        """Get an :class:`EmojiSequence` instance by text
+    def from_string(cls, s: str) -> Self:
+        """Get an :class:`EmojiSequence` instance from string
 
-        :param str value: Emoji string
+        :param s: Emoji string
         :return: Instance from internal dictionary
-        :rtype: EmojiSequence
-        :raises RuntimeError: When non-emoji character in text
-        :raises KeyError: When passed-in value not found in internal dictionary
+        :raise KeyError: When passed-in ``s`` not found in internal dictionary
         """
-        value = value.strip()
-        if not all(ord(s) in EmojiCharacter for s in value):
-            raise RuntimeError('Not all characters in the text is Emoji character.')
-        try:
-            return cls[value]
-        except KeyError:
-            code_points_text = ' '.join('{:04X}'.format(ord(c)) for c in value)
-            raise KeyError('[{}]({!r})'.format(code_points_text, value))
+        return cls[s]
 
     @classmethod
-    def from_emoji_character(cls, value: Union[EmojiCharacter, Iterable[EmojiCharacter]]) -> 'EmojiSequence':
-        """Get an :class:`EmojiSequence` instance by :class:`EmojiCharacter` object or list
+    def from_characters(cls, value: Union[EmojiCharacter, Iterable[EmojiCharacter]]) -> Self:
+        """Get an :class:`EmojiSequence` instance from :class:`EmojiCharacter` object or list
 
         :param value: Single or iterable object of :class:`EmojiCharacter`, composing the sequence
         :return: Instance from internal dictionary
-        :rtype: EmojiSequence
-        :raises KeyError: When passed-in value not found in internal dictionary
+        :raise KeyError: When passed-in value not found in internal dictionary
+        :raise TypeError: When passed-in value is not :class:`.EmojiCharacter` object or list
         """
         if isinstance(value, EmojiCharacter):
             s = value.string
         elif isinstance(value, Iterable):
-            s = ''.join(m.string for m in value)
+            s = "".join(m.string for m in value)
         else:
-            raise TypeError('Argument `value` must be one of `EmojiCharacter` or `Iterable[EmojiCharacter]`')
-        return cls.from_text(s)
+            raise TypeError("Argument `value` must be one of `EmojiCharacter` or `Iterable[EmojiCharacter]`")
+        return cls.from_string(s)
 
     @classmethod
-    def from_hex(cls, value: Union[str, int, Iterable[str], Iterable[int]]) -> 'EmojiSequence':
+    def from_hex(cls, value: Union[str, int, Iterable[str], Iterable[int]]) -> Self:
         """Get an :class:`EmojiSequence` instance by unicode code point(s)
 
         :type value: Union[str, int, Iterable[str], Iterable[int]]
         :param value: A single or sequence of HEX string/code.
 
             - it could be:
 
-              - one or more code points in hex format string, separated by spaces
-              - one code point integer
-              - An iterable object whose members are code point in hex format string
-              - An iterable object whose members are code point integer
+              - one or more code-point(s) in HEX format string, separated by spaces
+              - a single code-point integer
+              - An iterable object whose members are code-point string in HEX format
+              - An iterable object whose members are code-point integer
 
         :return: Instance returned from the class's internal dictionary
-        :rtype: EmojiSequence
 
-        :raises KeyError: When passed-in value not found in the class' internal dictionary
+        :raise KeyError: When passed-in value not found in the class' internal dictionary
         """
         if isinstance(value, str):
-            cps_array = value.split()
+            cps_array = value.split()  # type: ignore[assignment]
         elif isinstance(value, int):
-            cps_array = (value,)
-        elif isinstance(value, Iterable):
-            cps_array = value
+            cps_array = (value,)  # type: ignore[assignment]
+        elif isinstance(value, Iterable) and not isinstance(value, str) and all(isinstance(m, (str, int)) for m in value):
+            cps_array = value  # type: ignore[assignment]
         else:
             raise TypeError(
-                'The `args` should be one of `str`, `int`, or a sequence of that'
+                f"Argument `value` expects to be one of `str`, `bytes`, `int`, or a sequence of that, but actual is {type(value)}"
             )
-        return cls.from_emoji_character(EmojiCharacter.from_hex(cp) for cp in cps_array)
+        return cls.from_characters(EmojiCharacter.from_hex(cp) for cp in cps_array)
 
     @property
     def type_field(self) -> str:
         """A convenience for parsing the emoji sequence files, and is not intended to be maintained as a property.
 
-        one of the following:
+        may be one of:
 
         - `"Basic_Emoji"`
         - `"Emoji_Keycap_Sequence"`
         - `"Emoji_Flag_Sequence"`
         - `"Emoji_Tag_Sequence"`
         - `"Emoji_Modifier_Sequence"`
-
-        :type: str
+        - `"RGI_Emoji_ZWJ_Sequence"`
         """
         return self._type_field
 
     @property
     def description(self) -> str:
         return self._description
 
     @property
     def comment(self) -> str:
         return self._comment
 
     @property
-    def status(self) -> str:
-        return self._status
-
-    @status.setter
-    def status(self, value: str):
-        self._status = value
+    def characters(self) -> Sequence[EmojiCharacter]:
+        """Emoji character objects list which makes up the Emoji Sequence"""
+        return self._characters
 
     @property
-    def characters(self) -> List[EmojiCharacter]:
-        """Emoji character objects list which makes up the Emoji Sequence
+    def hex(self) -> str:
+        """Python style hex string of each emoji-characters's code-point, separated by spaces
 
-        :type: List[EmojiCharacter]
+        eg: ``0xa9 0xfe0f``
         """
-        return self._characters
+        return " ".join(c.hex for c in self.characters)
 
     @property
     def string(self) -> str:
-        """string of the Emoji Sequence
-
-        :type: str
-        """
+        """string of the Emoji Sequence"""
         return self._string
 
     @property
     def regex(self) -> str:
-        """Regular express of the Emoji Sequence
-
-        :type: str
-        """
+        """Regular expression string of the Emoji Sequence"""
         return self._regex
 
     @property
-    def regex_compiled(self):
-        """Compiled regular express pattern of the Emoji Sequence
-        """
-        return self._regex_compiled
+    def regex_pattern(self):
+        """Compiled regular expression pattern of the Emoji Sequence"""
+        return self._regex_pat
 
     @property
-    def code_points(self) -> List[int]:
-        """List of unicode integer value of the characters who make up Emoji Sequence
-
-        :type: List[int]
-        """
+    def code_points(self) -> Sequence[int]:
+        """List of unicode integer value of the characters who make up Emoji Sequence"""
         return self._code_points
 
-    @classmethod
-    def find(cls, s: str) -> List[Tuple['EmojiSequence', int, int]]:
-        """Finds out all emoji sequences in a string, and return them in a list
+    @property
+    def code_points_string(self) -> str:
+        """Unicode style hex string of each emoji-characters's code-point, separated by spaces
+
+        eg: ``00A9 FE0F``
         """
-        return list(cls.iter_find(s))
+        return " ".join(c.code_point_string for c in self.characters)
 
-    @classmethod
-    def iter_find(cls, s: str) -> Iterable[Tuple['EmojiSequence', int, int]]:
-        """Return an iterator which yields all emoji sequences in a string, without actually storing them all simultaneously.
+    if sys.version_info < (3, 9):
 
-        Item of the iterator is a 3-member tuple:
+        @classmethod
+        def find_all(cls, s: str) -> Sequence[Tuple[Self, int, int]]:
+            return list(cls.find(s))
 
-        #. ``0``: The found :class:`.EmojiSequence` object
-        #. ``1``: Begin position of the emoji sequence string
-        #. ``2``: End position of the emoji sequence string
-        """
-        m = cls.pattern.search(s)
-        while m:
-            yield cls.from_text(m.group()), m.start(), m.end()
-            m = cls.pattern.search(s, m.end())
+    else:
+
+        @classmethod
+        def find_all(cls, s: str) -> Sequence[tuple[Self, int, int]]:
+            """Find out all emoji sequences in a string, and return them in a list
+
+            Item of the returned list is as same as that in the iterator of :meth:`find`
+
+            The function equals::
+
+                list(EmojiSequence.find(s))
+
+            or ::
+
+                [x for x in EmojiSequence.find(s)]
+            """
+            return list(cls.find(s))
+
+    if sys.version_info < (3, 9):
+
+        @classmethod
+        def find(cls, s: str) -> Generator[Tuple[Self, int, int], None, None]:
+            m = cls.pattern.search(s)
+            while m:
+                yield cls.from_string(m.group()), m.start(), m.end()
+                m = cls.pattern.search(s, m.end())
+
+    else:
+
+        @classmethod
+        def find(cls, s: str) -> Generator[tuple[Self, int, int], None, None]:
+            """Return an iterator which yields all emoji sequences in a string, without actually storing them all simultaneously.
+
+            :param s: The string to find emoji sequences in it
+
+            :return: Item of the iterator is a 3-member tuple:
+
+                0. The found :class:`.EmojiSequence` object
+                1. Begin position of the emoji sequence in the string
+                2. End position of the emoji sequence in the string
+            """
+            m = cls.pattern.search(s)
+            while m:
+                yield cls.from_string(m.group()), m.start(), m.end()
+                m = cls.pattern.search(s, m.end())
 
 
 EmojiSequence.initial()
```

### Comparing `emoji-data-0.2.post2/src/emoji_data/utils.py` & `emoji_data-0.3/src/emoji_data/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,57 @@
-from typing import Iterable, TextIO, Tuple, Union
+from __future__ import annotations
 
-try:
-    from importlib.resources import files  # type: ignore
-except ImportError:
-    from importlib_resources import files  # type: ignore
+import sys
+from typing import Union, TextIO
 
+if sys.version_info < (3, 9):  # pragma: no cover
+    from typing import Generator, Iterable, Tuple
+    from importlib_resources import files
+else:  # pragma: no cover
+    from collections.abc import Generator, Iterable
+    from importlib.resources import files
 
-__all__ = ['code_points_to_string', 'code_point_to_regex', 'resources_files']
 
-resources_files = files
+__all__ = ["code_points_to_string", "code_point_to_regex", "data_file", "read_data_file_iterable"]
 
 
-def read_data_file_iterable(handle: TextIO) -> Iterable[Tuple[str, str]]:
+def data_file(file):
+    return files(__package__).joinpath("data").joinpath(file)
+
+
+def _read_data_file_iterable(handle: TextIO):
     for line in handle:
         line = line.strip()
         if not line:
             continue
-        if line[0] in '#;':
+        if line[0] in "#;":
             continue
-        parts = [s.strip() for s in line.split('#', 1)]
+        parts = [s.strip() for s in line.split("#", 1)]
         content = parts[0]
         try:
             comment = parts[1]
         except IndexError:
-            comment = ''
+            comment = ""
         yield content, comment
 
 
+if sys.version_info < (3, 9):
+
+    def read_data_file_iterable(handle) -> Generator[Tuple[str, str], None, None]:
+        yield from _read_data_file_iterable(handle)
+
+else:
+
+    def read_data_file_iterable(handle) -> Generator[tuple[str, str], None, None]:
+        yield from _read_data_file_iterable(handle)
+
+
 def code_points_to_string(code_points: Union[int, str, Iterable[int], Iterable[str]]) -> str:
     if isinstance(code_points, str):
-        return ''.join(chr(int(s, 16)) for s in code_points.split())
+        return "".join(chr(int(s, 16)) for s in code_points.split())
     if isinstance(code_points, Iterable):
-        return ''.join(chr(int(n, 16)) if isinstance(n, str) else chr(n) for n in code_points)
+        return "".join(chr(int(n, 16)) if isinstance(n, str) else chr(n) for n in code_points)
     return chr(code_points)
 
 
 def code_point_to_regex(code_point: int) -> str:
-    if code_point > 0xffff:
-        return r'\U{:08X}'.format(code_point)
-    return r'\u{:04X}'.format(code_point)
+    return rf"\U{code_point:08X}" if code_point > 0xFFFF else rf"\u{code_point:04X}"
```

### Comparing `emoji-data-0.2.post2/src/emoji_data.egg-info/SOURCES.txt` & `emoji_data-0.3/src/emoji_data.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 AUTHORS.md
 CHANGELOG.md
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
+src/emoji_data/.gitignore
 src/emoji_data/__init__.py
+src/emoji_data/_version.py
 src/emoji_data/character.py
 src/emoji_data/definitions.py
+src/emoji_data/py.typed
 src/emoji_data/sequence.py
 src/emoji_data/types.py
 src/emoji_data/utils.py
-src/emoji_data/version.py
 src/emoji_data.egg-info/PKG-INFO
 src/emoji_data.egg-info/SOURCES.txt
 src/emoji_data.egg-info/dependency_links.txt
 src/emoji_data.egg-info/requires.txt
 src/emoji_data.egg-info/top_level.txt
+src/emoji_data/data/README.txt
 src/emoji_data/data/emoji-data.txt
 src/emoji_data/data/emoji-sequences.txt
 src/emoji_data/data/emoji-test.txt
 src/emoji_data/data/emoji-variation-sequences.txt
 src/emoji_data/data/emoji-zwj-sequences.txt
```

