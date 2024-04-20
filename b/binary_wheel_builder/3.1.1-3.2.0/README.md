# Comparing `tmp/binary_wheel_builder-3.1.1.tar.gz` & `tmp/binary_wheel_builder-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binary_wheel_builder-3.1.1.tar", max compression
+gzip compressed data, was "binary_wheel_builder-3.2.0.tar", max compression
```

## Comparing `binary_wheel_builder-3.1.1.tar` & `binary_wheel_builder-3.2.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0     1069 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/LICENSE
--rw-r--r--   0        0        0    11735 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/README.md
--rw-r--r--   0        0        0      126 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/__init__.py
--rw-r--r--   0        0        0       90 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/__main__.py
--rw-r--r--   0        0        0      516 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/__init__.py
--rw-r--r--   0        0        0     4000 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/build.py
--rw-r--r--   0        0        0     4770 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/meta.py
--rw-r--r--   0        0        0      912 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/well_known_platforms.py
--rw-r--r--   0        0        0      316 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/wheel_sources/__init__.py
--rw-r--r--   0        0        0      420 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/wheel_sources/exceptions.py
--rw-r--r--   0        0        0     1571 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/wheel_sources/github.py
--rw-r--r--   0        0        0     1491 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/wheel_sources/github_test.py
--rw-r--r--   0        0        0     1172 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/wheel_sources/platform_based_file.py
--rw-r--r--   0        0        0      933 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/wheel_sources/platform_based_file_test.py
--rw-r--r--   0        0        0      465 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/wheel_sources/static.py
--rw-r--r--   0        0        0      211 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/cli/__init__.py
--rw-r--r--   0        0        0      534 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/cli/config_file.py
--rw-r--r--   0        0        0      951 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/cli/main.py
--rw-r--r--   0        0        0     4428 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/cli/yaml.py
--rw-r--r--   0        0        0     3982 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/cli/yaml_test.py
--rw-r--r--   0        0        0       90 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/wheel/__init__.py
--rw-r--r--   0        0        0      932 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/wheel/reproducible.py
--rw-r--r--   0        0        0      708 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/wheel/reproducible_test.py
--rw-r--r--   0        0        0     1015 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/wheel/util.py
--rw-r--r--   0        0        0      936 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/wheel/util_test.py
--rw-r--r--   0        0        0     4827 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/wrapper_templates.py
--rw-r--r--   0        0        0      199 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/wrapper_templates_test.py
--rw-r--r--   0        0        0     1511 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     4282 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/wheel.schema.json
--rw-r--r--   0        0        0    13078 1970-01-01 00:00:00.000000 binary_wheel_builder-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/LICENSE
+-rw-r--r--   0        0        0    11847 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/README.md
+-rw-r--r--   0        0        0      126 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/__init__.py
+-rw-r--r--   0        0        0       90 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/__main__.py
+-rw-r--r--   0        0        0      516 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/__init__.py
+-rw-r--r--   0        0        0     4000 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/build.py
+-rw-r--r--   0        0        0     4770 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/meta.py
+-rw-r--r--   0        0        0      912 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/well_known_platforms.py
+-rw-r--r--   0        0        0      316 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/__init__.py
+-rw-r--r--   0        0        0      420 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/exceptions.py
+-rw-r--r--   0        0        0     2311 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/github.py
+-rw-r--r--   0        0        0     1469 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/github_test.py
+-rw-r--r--   0        0        0     2450 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/gitlab_package_registry.py
+-rw-r--r--   0        0        0     1572 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/gitlab_package_registry_test.py
+-rw-r--r--   0        0        0     1389 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/platform_based_file.py
+-rw-r--r--   0        0        0      933 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/platform_based_file_test.py
+-rw-r--r--   0        0        0      465 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/static.py
+-rw-r--r--   0        0        0      211 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/cli/__init__.py
+-rw-r--r--   0        0        0      534 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/cli/config_file.py
+-rw-r--r--   0        0        0      951 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/cli/main.py
+-rw-r--r--   0        0        0     4428 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/cli/yaml.py
+-rw-r--r--   0        0        0     3982 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/cli/yaml_test.py
+-rw-r--r--   0        0        0       90 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/wheel/__init__.py
+-rw-r--r--   0        0        0      932 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/wheel/reproducible.py
+-rw-r--r--   0        0        0      708 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/wheel/reproducible_test.py
+-rw-r--r--   0        0        0     1015 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/wheel/util.py
+-rw-r--r--   0        0        0      936 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/wheel/util_test.py
+-rw-r--r--   0        0        0     4827 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/wrapper_templates.py
+-rw-r--r--   0        0        0      199 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/wrapper_templates_test.py
+-rw-r--r--   0        0        0     1511 2024-04-20 09:58:28.495794 binary_wheel_builder-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4282 2024-04-20 09:58:28.495794 binary_wheel_builder-3.2.0/wheel.schema.json
+-rw-r--r--   0        0        0    13190 1970-01-01 00:00:00.000000 binary_wheel_builder-3.2.0/PKG-INFO
```

### Comparing `binary_wheel_builder-3.1.1/LICENSE` & `binary_wheel_builder-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.1/README.md` & `binary_wheel_builder-3.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     Build deterministic python wheels to distribute CLI tools (third party or your own with python and make them easily usable using python code.
 </p>
 
 ## Features
 
 - deterministic wheel file output
 - Use with Python Code or as CLI
-- Prebuilt data sources for your binaries
+- [Prebuilt data sources](https://timo-reymann.github.io/python-binary-wheel-builder/binary_wheel_builder/api/wheel_sources/index.html) for your binaries
 - Ready to release and ship your binaries
 - Wrapper for cli calls inside Python
 - Exposes wheel as module entrypoint (`python -m your_cli`) and adds to path (`your-cli`)
 
 ## Requirements
 
 - Python 3.8+ for host running wheel build
```

### Comparing `binary_wheel_builder-3.1.1/binary_wheel_builder/api/__init__.py` & `binary_wheel_builder-3.2.0/binary_wheel_builder/api/__init__.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.1/binary_wheel_builder/api/build.py` & `binary_wheel_builder-3.2.0/binary_wheel_builder/api/build.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.1/binary_wheel_builder/api/meta.py` & `binary_wheel_builder-3.2.0/binary_wheel_builder/api/meta.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.1/binary_wheel_builder/api/well_known_platforms.py` & `binary_wheel_builder-3.2.0/binary_wheel_builder/api/well_known_platforms.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.1/binary_wheel_builder/api/wheel_sources/github_test.py` & `binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/github_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import urllib.request
 from unittest import mock
 from unittest.mock import patch, MagicMock
 from urllib.error import HTTPError
 
 import pytest
 
 from binary_wheel_builder.api import well_known_platforms
@@ -17,15 +16,15 @@
     ["v", 404],
     ["", 404]
 ])
 def test_github_release_binary_wheel_source(tag_prefix: str, status_code: int):
     request_fail = True if status_code < 200 or status_code > 300 else False
     with mock.patch("urllib.request.urlopen",
                     return_value=MagicMock(return_value=None),
-                    side_effect=HTTPError('http://example.com', 500, 'Internal Error', {},
+                    side_effect=HTTPError('http://example.com', status_code, 'status', {},
                                           None) if request_fail else None) as urlopen_mock:
         source = GithubReleaseBinarySource(
             "org/project",
             "0.0.1", {
                 well_known_platforms.LINUX_GENERIC_i386: "foo-bar"
             },
             "foo-bar",
```

### Comparing `binary_wheel_builder-3.1.1/binary_wheel_builder/api/wheel_sources/platform_based_file.py` & `binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/platform_based_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from pathlib import Path
 
-from binary_wheel_builder.api.meta import WheelSource, WheelPlatformIdentifier, WheelFileEntry
-from binary_wheel_builder.api.wheel_sources.exceptions import UnsupportedWheelPlatformException, SourceFileRequestFailed
+from binary_wheel_builder.api.meta import WheelFileEntry, WheelPlatformIdentifier, WheelSource
+from binary_wheel_builder.api.wheel_sources.exceptions import SourceFileRequestFailed, UnsupportedWheelPlatformException
 
 
 class PlatformBasedFileSource(WheelSource):
-    def __init__(self, executable_path : str, file_name_mapping: dict[WheelPlatformIdentifier, Path | str]):
+    def __init__(self, executable_path: str, file_name_mapping: dict[WheelPlatformIdentifier, Path | str]):
+        """
+
+        :param executable_path: Path to the executable that will be used in the generated wheel
+        :param file_name_mapping: Map wheel platform identifiers to the local binary file names.
+        """
         self.executable_path = executable_path
         self.file_name_mapping = file_name_mapping
 
     def generate_fileset(self, wheel_platform: WheelPlatformIdentifier) -> list[WheelFileEntry]:
         if wheel_platform not in self.file_name_mapping:
             raise UnsupportedWheelPlatformException(wheel_platform)
```

### Comparing `binary_wheel_builder-3.1.1/binary_wheel_builder/api/wheel_sources/platform_based_file_test.py` & `binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/platform_based_file_test.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.1/binary_wheel_builder/cli/config_file.py` & `binary_wheel_builder-3.2.0/binary_wheel_builder/cli/config_file.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.1/binary_wheel_builder/cli/main.py` & `binary_wheel_builder-3.2.0/binary_wheel_builder/cli/main.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.1/binary_wheel_builder/cli/yaml.py` & `binary_wheel_builder-3.2.0/binary_wheel_builder/cli/yaml.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.1/binary_wheel_builder/cli/yaml_test.py` & `binary_wheel_builder-3.2.0/binary_wheel_builder/cli/yaml_test.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.1/binary_wheel_builder/wheel/reproducible.py` & `binary_wheel_builder-3.2.0/binary_wheel_builder/wheel/reproducible.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.1/binary_wheel_builder/wheel/reproducible_test.py` & `binary_wheel_builder-3.2.0/binary_wheel_builder/wheel/reproducible_test.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.1/binary_wheel_builder/wheel/util.py` & `binary_wheel_builder-3.2.0/binary_wheel_builder/wheel/util.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.1/binary_wheel_builder/wheel/util_test.py` & `binary_wheel_builder-3.2.0/binary_wheel_builder/wheel/util_test.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.1/binary_wheel_builder/wrapper_templates.py` & `binary_wheel_builder-3.2.0/binary_wheel_builder/wrapper_templates.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.1/pyproject.toml` & `binary_wheel_builder-3.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "binary_wheel_builder"
-version = "3.1.1"
+version = "3.2.0"
 description = "Bundle CLI applications or other binary data as wheel to use them in code or as standalone binary"
 authors = ["Timo Reymann <mail@timo-reymann.de>"]
 readme = "README.md"
 packages = [
     { include = "binary_wheel_builder" }
 ]
 classifiers = [
```

### Comparing `binary_wheel_builder-3.1.1/wheel.schema.json` & `binary_wheel_builder-3.2.0/wheel.schema.json`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.1/PKG-INFO` & `binary_wheel_builder-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary_wheel_builder
-Version: 3.1.1
+Version: 3.2.0
 Summary: Bundle CLI applications or other binary data as wheel to use them in code or as standalone binary
 Home-page: https://github.com/timo-reymann/python-binary-wheel-builder
 Author: Timo Reymann
 Author-email: mail@timo-reymann.de
 Requires-Python: >3.8
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -46,15 +46,15 @@
     Build deterministic python wheels to distribute CLI tools (third party or your own with python and make them easily usable using python code.
 </p>
 
 ## Features
 
 - deterministic wheel file output
 - Use with Python Code or as CLI
-- Prebuilt data sources for your binaries
+- [Prebuilt data sources](https://timo-reymann.github.io/python-binary-wheel-builder/binary_wheel_builder/api/wheel_sources/index.html) for your binaries
 - Ready to release and ship your binaries
 - Wrapper for cli calls inside Python
 - Exposes wheel as module entrypoint (`python -m your_cli`) and adds to path (`your-cli`)
 
 ## Requirements
 
 - Python 3.8+ for host running wheel build
```

