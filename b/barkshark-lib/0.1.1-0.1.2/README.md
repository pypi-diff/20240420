# Comparing `tmp/barkshark_lib-0.1.1.tar.gz` & `tmp/barkshark_lib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barkshark_lib-0.1.1.tar", last modified: Fri Apr 19 13:51:44 2024, max compression
+gzip compressed data, was "barkshark_lib-0.1.2.tar", last modified: Sat Apr 20 15:05:24 2024, max compression
```

## Comparing `barkshark_lib-0.1.1.tar` & `barkshark_lib-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-19 13:51:44.107366 barkshark_lib-0.1.1/
--rw-r--r--   0 zoey      (1000) zoey      (1000)    24909 2023-10-06 18:44:07.000000 barkshark_lib-0.1.1/LICENSE.md
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1498 2024-04-19 13:51:44.107366 barkshark_lib-0.1.1/PKG-INFO
--rw-r--r--   0 zoey      (1000) zoey      (1000)       85 2024-04-19 02:44:00.000000 barkshark_lib-0.1.1/README.md
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-19 13:51:44.107366 barkshark_lib-0.1.1/barkshark_lib.egg-info/
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1498 2024-04-19 13:51:44.000000 barkshark_lib-0.1.1/barkshark_lib.egg-info/PKG-INFO
--rw-r--r--   0 zoey      (1000) zoey      (1000)      372 2024-04-19 13:51:44.000000 barkshark_lib-0.1.1/barkshark_lib.egg-info/SOURCES.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)        1 2024-04-19 13:51:44.000000 barkshark_lib-0.1.1/barkshark_lib.egg-info/dependency_links.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)      157 2024-04-19 13:51:44.000000 barkshark_lib-0.1.1/barkshark_lib.egg-info/requires.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)        5 2024-04-19 13:51:44.000000 barkshark_lib-0.1.1/barkshark_lib.egg-info/top_level.txt
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-19 13:51:44.107366 barkshark_lib-0.1.1/blib/
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1079 2024-04-19 13:47:24.000000 barkshark_lib-0.1.1/blib/__init__.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     4255 2024-04-19 01:58:34.000000 barkshark_lib-0.1.1/blib/application.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     5944 2024-04-19 13:20:08.000000 barkshark_lib-0.1.1/blib/enums.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     9416 2024-04-19 13:08:39.000000 barkshark_lib-0.1.1/blib/errors.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)    21594 2024-04-19 13:44:32.000000 barkshark_lib-0.1.1/blib/misc.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     4230 2024-04-19 13:08:48.000000 barkshark_lib-0.1.1/blib/objects.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     5632 2024-04-19 02:05:31.000000 barkshark_lib-0.1.1/blib/path.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)    11737 2024-04-19 02:38:22.000000 barkshark_lib-0.1.1/blib/router.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     3369 2024-04-19 02:02:39.000000 barkshark_lib-0.1.1/blib/transport.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     7564 2024-04-19 02:07:08.000000 barkshark_lib-0.1.1/blib/url.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1912 2024-04-19 03:24:57.000000 barkshark_lib-0.1.1/pyproject.toml
--rw-r--r--   0 zoey      (1000) zoey      (1000)       38 2024-04-19 13:51:44.107366 barkshark_lib-0.1.1/setup.cfg
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-20 15:05:24.282629 barkshark_lib-0.1.2/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    24909 2023-10-06 18:44:07.000000 barkshark_lib-0.1.2/LICENSE.md
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1498 2024-04-20 15:05:24.282629 barkshark_lib-0.1.2/PKG-INFO
+-rw-r--r--   0 zoey      (1000) zoey      (1000)       85 2024-04-19 02:44:00.000000 barkshark_lib-0.1.2/README.md
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-20 15:05:24.282629 barkshark_lib-0.1.2/barkshark_lib.egg-info/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1498 2024-04-20 15:05:24.000000 barkshark_lib-0.1.2/barkshark_lib.egg-info/PKG-INFO
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      405 2024-04-20 15:05:24.000000 barkshark_lib-0.1.2/barkshark_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        1 2024-04-20 15:05:24.000000 barkshark_lib-0.1.2/barkshark_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      157 2024-04-20 15:05:24.000000 barkshark_lib-0.1.2/barkshark_lib.egg-info/requires.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        5 2024-04-20 15:05:24.000000 barkshark_lib-0.1.2/barkshark_lib.egg-info/top_level.txt
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-20 15:05:24.282629 barkshark_lib-0.1.2/blib/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1193 2024-04-20 14:52:49.000000 barkshark_lib-0.1.2/blib/__init__.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     4255 2024-04-19 01:58:34.000000 barkshark_lib-0.1.2/blib/application.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     5992 2024-04-20 14:35:11.000000 barkshark_lib-0.1.2/blib/enums.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     9511 2024-04-20 12:54:19.000000 barkshark_lib-0.1.2/blib/errors.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     5149 2024-04-20 14:55:36.000000 barkshark_lib-0.1.2/blib/icon_theme.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    22554 2024-04-19 19:35:29.000000 barkshark_lib-0.1.2/blib/misc.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     4230 2024-04-19 13:08:48.000000 barkshark_lib-0.1.2/blib/objects.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     6700 2024-04-20 13:01:47.000000 barkshark_lib-0.1.2/blib/path.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        0 2024-04-19 15:02:18.000000 barkshark_lib-0.1.2/blib/py.typed
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    11737 2024-04-19 02:38:22.000000 barkshark_lib-0.1.2/blib/router.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     3369 2024-04-19 02:02:39.000000 barkshark_lib-0.1.2/blib/transport.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     7564 2024-04-19 02:07:08.000000 barkshark_lib-0.1.2/blib/url.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1912 2024-04-19 03:24:57.000000 barkshark_lib-0.1.2/pyproject.toml
+-rw-r--r--   0 zoey      (1000) zoey      (1000)       38 2024-04-20 15:05:24.282629 barkshark_lib-0.1.2/setup.cfg
```

### Comparing `barkshark_lib-0.1.1/LICENSE.md` & `barkshark_lib-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `barkshark_lib-0.1.1/PKG-INFO` & `barkshark_lib-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barkshark-lib
-Version: 0.1.1
+Version: 0.1.2
 Summary: Collection of classes and functions used in most Barkshark projects
 Author-email: Zoey Mae <admin@barkshark.xyz>
 License: CNPL 7+
 Project-URL: Bug Tracker, https://git.barkshark.xyz/barkshark/blib/issues
 Project-URL: Documentation, https://docs.barkshark.xyz/blib
 Project-URL: Source Code, https://git.barkshark.xyz/barkshark/blib
 Keywords: python
```

### Comparing `barkshark_lib-0.1.1/barkshark_lib.egg-info/PKG-INFO` & `barkshark_lib-0.1.2/barkshark_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barkshark-lib
-Version: 0.1.1
+Version: 0.1.2
 Summary: Collection of classes and functions used in most Barkshark projects
 Author-email: Zoey Mae <admin@barkshark.xyz>
 License: CNPL 7+
 Project-URL: Bug Tracker, https://git.barkshark.xyz/barkshark/blib/issues
 Project-URL: Documentation, https://docs.barkshark.xyz/blib
 Project-URL: Source Code, https://git.barkshark.xyz/barkshark/blib
 Keywords: python
```

### Comparing `barkshark_lib-0.1.1/blib/__init__.py` & `barkshark_lib-0.1.2/blib/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __software__ = "Barkshark Lib"
 "Name of the library"
 
-__version_info__ = (0, 1, 1)
+__version_info__ = (0, 1, 2)
 "Version of the library"
 
 __version__ = ".".join(str(v) for v in __version_info__)
 "Version of the library in string form"
 
 
 from .application import Application
@@ -33,22 +33,31 @@
 
 # todo: convert these errors to use the new Error class
 from .errors import (
 	HttpError
 
 )
 
+from .icon_theme import (
+	FileIconTheme,
+	Icon,
+	IconTheme,
+	IconThemes,
+	MemoryIconTheme
+)
+
 from .misc import (
 	catch_errors,
 	convert_to_boolean,
 	convert_to_bytes,
 	convert_to_string,
 	deprecated,
 	get_object_name,
 	get_object_properties,
+	get_resource_path,
 	get_top_domain,
 	http_request,
 	is_loop_running,
 	random_str,
 	time_function,
 	time_function_pprint,
 	DictProperty,
```

### Comparing `barkshark_lib-0.1.1/blib/application.py` & `barkshark_lib-0.1.2/blib/application.py`

 * *Files identical despite different names*

### Comparing `barkshark_lib-0.1.1/blib/enums.py` & `barkshark_lib-0.1.2/blib/enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -231,15 +231,16 @@
 	PreconditionFailed = 412
 	RequestEntityTooLarge = 413
 	RequestUriTooLong = 414
 	UnsupportedMediaType = 415
 	RequestRangeNotSatisfiable = 416
 	ExpectationFailed = 417
 	IAmATeapot = 418
-	TooHighToHandleYourShit = 420
+	EnhanceYourCalm = 420
+	TooHighToHandleYourShit = 420 # this will get removed in the future
 	MisdirectedRequest = 421
 	UnprocessableEntity = 422
 	Locked = 423
 	FailedDependency = 424
 	TooEarly = 425
 	UpgradeRequired = 426
 	PreconditionRequired = 428
@@ -259,16 +260,16 @@
 	NotExtended = 510
 	NetworkAuthenticationRequired = 511
 
 
 	@property
 	def reason(self) -> str:
 		"The text associated with the code"
-		data = HTTP_REASON_REGEX.findall(self.name)
-		return ' '.join(data)
+
+		return " ".join(HTTP_REASON_REGEX.findall(self.name))
 
 
 class ProtocolPort(IntEnum):
 	"Protocol names and their associated default port"
 
 	FILE = 0
 	FTP = 21
```

### Comparing `barkshark_lib-0.1.1/blib/errors.py` & `barkshark_lib-0.1.2/blib/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,55 +124,51 @@
 		"Name of the error group"
 		return self.__class__.__name__
 
 
 class FileError(Error, metaclass = ErrorMeta):
 	"Raised on errors involving files"
 
-	NotFound = 0
+	NotFound: ErrorCode = 0 # type: ignore[assignment]
 	"Raised when a file or directory could not be found"
 
-	Found = 1
+	Found: ErrorCode = 1 # type: ignore[assignment]
 	"Raised when a file or directory exists when it should not"
 
-	IsDirectory = 2
+	IsDirectory: ErrorCode = 2 # type: ignore[assignment]
 	"Raised when the path is a directory when it should not be"
 
-	IsFile = 3
+	IsFile: ErrorCode = 3 # type: ignore[assignment]
 	"Raised when the path is a file when it should not be"
 
 
 class HttpError(Exception):
 	"Error raised from a client or server response"
 
-	status: HttpStatus
-	"Status code and reason"
-
-	message: str
-	"Message body of the error"
-
-	headers: dict[str, str]
-	"Headers associated with the error"
-
 
 	def __init__(self,
 				status: HttpStatus | int,
 				message: str | None = None,
 				headers: dict[str, str] | None = None) -> None:
 		"""
 			Create a new http error
 
 			:param status: Status code of the error
 			:param message: Body of the error
 			:param headers: Headers of the error
 		"""
 
 		self.status = HttpStatus.parse(status)
+		"Status code and reason"
+
 		self.message = message or self.status.reason
+		"Message body of the error"
+
 		self.headers = headers or {}
+		"Headers associated with the error"
 
 
 	def __str__(self) -> str:
 		return f"HTTP Error {self.status}: {self.message}"
 
 
 	def __repr__(self) -> str:
```

### Comparing `barkshark_lib-0.1.1/blib/misc.py` & `barkshark_lib-0.1.2/blib/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,34 @@
 from typing import Any, Generic, TypeVar
 from urllib.request import Request, urlopen
 
 from . import __version__
 from .enums import FileSizeUnit, HttpMethod
 
 try:
+	from importlib.resources import files as pkgfiles
+
+except ImportError:
+	# this is a mess and I'm now debating my decision to never have outside dependencies
+	# outside of docs and dev stuff
+	import inspect
+	from importlib import import_module
+	from importlib.resources.abc import Traversable
+	from types import ModuleType
+
+	def pkgfiles(anchor: str | ModuleType | None = None) -> Traversable:
+		if anchor is None:
+			raise ValueError("A module or name must be specified")
+
+		if isinstance(anchor, str):
+			anchor = import_module(anchor)
+
+		return Path(inspect.getfile(anchor)).parent
+
+try:
 	from typing import Self
 
 except ImportError:
 	from typing_extensions import Self
 
 
 DictValueType = TypeVar("DictValueType")
@@ -197,14 +217,26 @@
 
 		if callable(value := getattr(obj, key)):
 			continue
 
 		yield key, value
 
 
+def get_resource_path(module: str, path: str | None = None) -> Path:
+	"""
+		Get a path to a module resource
+
+		:param module: Name of the module to get the resource from
+		:param path: Path of the resource starting from the path of the module
+	"""
+
+	new_path = Path(str(pkgfiles(module)))
+	return new_path.joinpath(path.lstrip("/")) if path is not None else new_path
+
+
 def get_top_domain(domain: str) -> str:
 	'''
 		Get the main domain from a string. The top-level domain list is cached as
 		``~/.cache/public_suffix_list.txt`` for 7 days
 
 		:param str domain: The domain to extract the top-level domain from
 		:raises ValueError: When the top domain cannot be found
```

### Comparing `barkshark_lib-0.1.1/blib/objects.py` & `barkshark_lib-0.1.2/blib/objects.py`

 * *Files identical despite different names*

### Comparing `barkshark_lib-0.1.1/blib/path.py` & `barkshark_lib-0.1.2/blib/path.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from __future__ import annotations
 
 import os
 import shutil
 import sys
 
+from collections.abc import Iterator, Sequence
+from glob import iglob
+
 from .enums import FileType, XdgDir
+from .errors import FileError
 from .misc import FileSize
 
 try:
 	from typing import Self
 
 except ImportError:
 	from typing_extensions import Self
@@ -65,14 +69,19 @@
 
 	@property
 	def parent(self) -> Self:
 		"Remove the last path segment"
 		return self.__class__(os.path.dirname(self))
 
 
+	@property
+	def stem(self) -> str:
+		return self.name.rstrip(self.ext).rstrip(".")
+
+
 	def join(self, *parts: str, normalize: bool = False) -> Self: # type: ignore[override]
 		"""
 			Append a path segment
 
 			:param parts: Path segments to append
 			:param normalize: Normalize the path before returning it
 		"""
@@ -204,14 +213,44 @@
 
 		if self.islink:
 			types.append(FileType.LINK)
 
 		return tuple(types)
 
 
+	def glob(self,
+			pattern: str = "**",
+			recursive: bool = False,
+			hidden: bool = False,
+			ext: Sequence[str] | None = None) -> Iterator[File]:
+		"""
+			Iterate through a directory with paths matching a specific pattern
+
+			.. note:: See :class:`glob.iglob` for pattern usage
+
+			:param pattern: Filename pattern to match
+			:param recursive: Whether or not to search through sub-directories
+			:param hidden: List hidden files
+			:param ext: Include only the specified extensions in the result if set
+			:raises FileError: If the path is not a directory or does not exist
+		"""
+
+		if self.isfile:
+			raise FileError.IsFile(self)
+
+		if not self.exists:
+			raise FileError.NotFound(self)
+
+		for path in iglob(pattern, root_dir = self, recursive = recursive, include_hidden = hidden):
+			filepath = self.join(path)
+
+			if ext is None or filepath.ext in ext:
+				yield filepath
+
+
 	def mkdir(self, mode: int = 0o755) -> None:
 		"""
 			Create a directory and all parent directories
 
 			.. note:: ``mode`` will eventually use a ``UnixPerm`` object. Use an octal
 				(ex: ``0o755``) for now
```

### Comparing `barkshark_lib-0.1.1/blib/router.py` & `barkshark_lib-0.1.2/blib/router.py`

 * *Files identical despite different names*

### Comparing `barkshark_lib-0.1.1/blib/transport.py` & `barkshark_lib-0.1.2/blib/transport.py`

 * *Files identical despite different names*

### Comparing `barkshark_lib-0.1.1/blib/url.py` & `barkshark_lib-0.1.2/blib/url.py`

 * *Files identical despite different names*

### Comparing `barkshark_lib-0.1.1/pyproject.toml` & `barkshark_lib-0.1.2/pyproject.toml`

 * *Files identical despite different names*

