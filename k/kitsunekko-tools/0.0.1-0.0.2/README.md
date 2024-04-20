# Comparing `tmp/kitsunekko_tools-0.0.1.tar.gz` & `tmp/kitsunekko_tools-0.0.2.tar.gz`

## Comparing `kitsunekko_tools-0.0.1.tar` & `kitsunekko_tools-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.1/.github/ISSUE_TEMPLATE/issue.md
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.1/.github/workflows/black.yml
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.1/.github/workflows/ci-cd.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.1/kitsunekko_tools/__init__.py
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.1/kitsunekko_tools/__main__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.1/kitsunekko_tools/__version__.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.1/kitsunekko_tools/common.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.1/kitsunekko_tools/config.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.1/kitsunekko_tools/consts.py
--rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.1/kitsunekko_tools/download.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.1/kitsunekko_tools/ignore.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.1/kitsunekko_tools/mega_upload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.1/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.1/LICENSE
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.1/README.md
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    41485 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/.github/ISSUE_TEMPLATE/issue.md
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/.github/workflows/black.yml
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/.github/workflows/ci-cd.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/kitsunekko_tools/__init__.py
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/kitsunekko_tools/__main__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/kitsunekko_tools/__version__.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/kitsunekko_tools/common.py
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/kitsunekko_tools/config.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/kitsunekko_tools/consts.py
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/kitsunekko_tools/download.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/kitsunekko_tools/ignore.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/kitsunekko_tools/mega_upload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/README.md
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    41485 2020-02-02 00:00:00.000000 kitsunekko_tools-0.0.2/PKG-INFO
```

### Comparing `kitsunekko_tools-0.0.1/.github/ISSUE_TEMPLATE/config.yml` & `kitsunekko_tools-0.0.2/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-0.0.1/.github/workflows/ci-cd.yml` & `kitsunekko_tools-0.0.2/.github/workflows/ci-cd.yml`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-0.0.1/kitsunekko_tools/__main__.py` & `kitsunekko_tools-0.0.2/kitsunekko_tools/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,21 +59,27 @@
     """
     Manage the list of ignore patterns.
     """
 
     def __init__(self, ignore_list: IgnoreList):
         self._ignore_list = ignore_list
 
-    def show(self):
+    def locate(self) -> None:
+        """
+        Print path to the ignore file.
+        """
+        print(self._ignore_list.ignore_filepath)
+
+    def show(self) -> None:
         """
         Print the list of ignore rules as Unix shell-style wildcards.
         """
         print("\n".join(self._ignore_list.patterns()))
 
-    def add(self, pattern: str):
+    def add(self, pattern: str)-> None:
         """
         Add a new ignore rule.
         """
         if pattern:
             self._ignore_list.add(str(pattern))
             print(f"File written: {self._ignore_list.path()}")
         else:
```

### Comparing `kitsunekko_tools-0.0.1/kitsunekko_tools/config.py` & `kitsunekko_tools-0.0.2/kitsunekko_tools/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     def __post_init__(self):
         self.destination = pathlib.Path(self.destination)
 
     def as_toml_str(self) -> str:
         with io.StringIO() as si:
             for key, value in dataclasses.asdict(self).items():
                 match value:
-                    case str():
+                    case str() | pathlib.Path():
                         si.write(f'{key} = "{value}"\n')
                     case int():
                         si.write(f"{key} = {value}\n")
                     case dict():
                         si.write(f"[{key}]\n")
                         si.write("\n".join(f'{k} = "{v}"' for k, v in value.items()))
                     case _:
@@ -84,11 +84,10 @@
     file_path: pathlib.Path
 
 
 @functools.cache
 def get_config() -> ReadConfigResult:
     for config_file_path in config_locations():
         if os.path.isfile(config_file_path):
-            print(f"Reading config file: {config_file_path}", file=sys.stderr)
             with open(config_file_path, "rb") as f:
                 return ReadConfigResult(KitsuConfig(**tomllib.load(f)), config_file_path)
     raise ConfigFileNotFoundError()
```

### Comparing `kitsunekko_tools-0.0.1/kitsunekko_tools/download.py` & `kitsunekko_tools-0.0.2/kitsunekko_tools/download.py`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-0.0.1/kitsunekko_tools/ignore.py` & `kitsunekko_tools-0.0.2/kitsunekko_tools/ignore.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,19 +26,22 @@
         self._config = config or get_config().data
         self._ignore_filepath = pathlib.Path(self._config.destination) / IGNORE_FILENAME
         self._patterns = set()
         if not self._config.destination.is_dir():
             raise IgnoreListException(f"Destination directory does not exist: {self._config.destination}")
         try:
             with open(self._ignore_filepath, encoding="utf8") as f:
-                print(f"Reading ignore file: {self._ignore_filepath}", file=sys.stderr)
                 self._patterns.update(filter(bool, map(str.strip, f.read().splitlines())))
         except FileNotFoundError:
             pass
 
+    @property
+    def ignore_filepath(self) -> pathlib.Path:
+        return self._ignore_filepath
+
     def is_matching(self, file_path: str) -> bool:
         path_dest_stripped = os.path.relpath(file_path, self._config.destination)
         return any(fnmatch.fnmatch(path_dest_stripped, pattern) for pattern in self._patterns)
 
     def patterns(self) -> set[str]:
         """
         Return all known ignore patterns.
```

### Comparing `kitsunekko_tools-0.0.1/kitsunekko_tools/mega_upload.py` & `kitsunekko_tools-0.0.2/kitsunekko_tools/mega_upload.py`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-0.0.1/LICENSE` & `kitsunekko_tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-0.0.1/README.md` & `kitsunekko_tools-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-0.0.1/pyproject.toml` & `kitsunekko_tools-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-0.0.1/PKG-INFO` & `kitsunekko_tools-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kitsunekko-tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: A set of scripts for creating a local kitsunekko mirror.
 Author-email: Ren Tatsumoto <tatsu@autistici.org>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

