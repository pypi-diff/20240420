# Comparing `tmp/stac_model-0.1.1a3.tar.gz` & `tmp/stac_model-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_model-0.1.1a3.tar", max compression
+gzip compressed data, was "stac_model-0.1.2.tar", max compression
```

## Comparing `stac_model-0.1.1a3.tar` & `stac_model-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-12-04 20:59:28.570283 stac_model-0.1.1a3/LICENSE
--rw-r--r--   0        0        0    30641 2024-02-23 22:19:38.925658 stac_model-0.1.1a3/README.md
--rw-r--r--   0        0        0     4826 2024-02-26 04:07:40.569243 stac_model-0.1.1a3/pyproject.toml
--rw-r--r--   0        0        0      241 2024-01-11 02:41:03.834963 stac_model-0.1.1a3/stac_model/__init__.py
--rw-r--r--   0        0        0     1287 2024-02-26 03:07:07.944590 stac_model-0.1.1a3/stac_model/__main__.py
--rw-r--r--   0        0        0     3598 2024-02-26 03:57:47.433252 stac_model-0.1.1a3/stac_model/examples.py
--rw-r--r--   0        0        0     1493 2024-02-26 03:56:20.153587 stac_model-0.1.1a3/stac_model/input.py
--rw-r--r--   0        0        0     1184 2024-02-23 19:13:39.976809 stac_model-0.1.1a3/stac_model/output.py
--rw-r--r--   0        0        0     1646 2024-02-23 19:30:48.582625 stac_model-0.1.1a3/stac_model/paths.py
--rw-r--r--   0        0        0     1596 2024-02-26 03:57:47.433252 stac_model-0.1.1a3/stac_model/runtime.py
--rw-r--r--   0        0        0     1154 2024-02-26 03:48:52.947466 stac_model-0.1.1a3/stac_model/schema.py
--rw-r--r--   0        0        0    32277 1970-01-01 00:00:00.000000 stac_model-0.1.1a3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-19 16:28:59.671806 stac_model-0.1.2/LICENSE
+-rw-r--r--   0        0        0    55385 2024-04-19 16:28:59.671806 stac_model-0.1.2/README.md
+-rw-r--r--   0        0        0     5300 2024-04-19 17:04:43.667216 stac_model-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      265 2024-04-19 16:28:59.671806 stac_model-0.1.2/stac_model/__init__.py
+-rw-r--r--   0        0        0     1215 2024-04-19 16:28:59.671806 stac_model-0.1.2/stac_model/__main__.py
+-rw-r--r--   0        0        0     3035 2024-04-19 16:28:59.671806 stac_model-0.1.2/stac_model/base.py
+-rw-r--r--   0        0        0     7036 2024-04-19 16:28:59.671806 stac_model-0.1.2/stac_model/examples.py
+-rw-r--r--   0        0        0     2026 2024-04-19 16:28:59.671806 stac_model-0.1.2/stac_model/input.py
+-rw-r--r--   0        0        0     3007 2024-04-19 16:28:59.671806 stac_model-0.1.2/stac_model/output.py
+-rw-r--r--   0        0        0     1476 2024-04-19 16:28:59.671806 stac_model-0.1.2/stac_model/runtime.py
+-rw-r--r--   0        0        0     9406 2024-04-19 16:28:59.671806 stac_model-0.1.2/stac_model/schema.py
+-rw-r--r--   0        0        0    57086 1970-01-01 00:00:00.000000 stac_model-0.1.2/PKG-INFO
```

### Comparing `stac_model-0.1.1a3/LICENSE` & `stac_model-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stac_model-0.1.1a3/pyproject.toml` & `stac_model-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "stac-model"
-version = "0.1.1.alpha3"
+version = "0.1.2"
 description = "A PydanticV2 validation and serialization libary for the STAC ML Model Extension"
 readme = "README.md"
 authors = ["Ryan Avery <ryan@wherobots.com>"]
 license = "Apache Software License 2.0"
 repository = "https://github.com/rbavery/stac-model"
 homepage = "https://github.com/rbavery/stac-model"
 packages = [
@@ -51,33 +51,32 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 typer = {extras = ["all"], version = "^0.9.0"}
 rich = "^13.7.0"
-pydantic = "^2.6.2" # bug in post 2.3 https://github.com/pydantic/pydantic/issues/7720
-pydantic-core = "^2.16.3"
-numpy = "^1.26.2"
-# fastapi="^0.108.0"
-
+pydantic = "^2.6.3" # bug in post 2.3 https://github.com/pydantic/pydantic/issues/7720
+pydantic-core = "^2"
+pystac = "^1.9.0"
+shapely = "^2"
+jsonschema = "^4.21.1"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.0.0"
 mypy-extensions = "^0.4.3"
 pre-commit = "^2.21.0"
 bandit = "^1.7.5"
 safety = "^2.3.4"
-
+pystac = "^1.10.0"  # custom validator required (https://github.com/stac-utils/pystac/pull/1320)
 
 pydocstyle = {extras = ["toml"], version = "^6.2.0"}
 pydoclint = "^0.3.0"
 
 pytest = "^7.2.1"
-pytest-html = "^3.2.0"
 pytest-cov = "^4.1.0"
 pytest-mock = "^3.10.0"
 pytest-timeout = "^2.2.0"
 pytest-benchmark = "^4.0.0"
 pytest-sugar = "^0.9.7"
 pytest-click = "^1.1.0"
 pytest-pikachu = "^1.0.0"
@@ -92,16 +91,20 @@
     ".tox",
     ".venv",
     "_build",
     "buck-out",
     "build",
     "dist",
     "env",
-    "venv"
+    "venv",
+    "node_modules",
 ]
+respect-gitignore = true
+line-length = 120
+show-fixes = true
 
 [tool.ruff.lint]
 select = [
     # pycodestyle
     "E",
     # Pyflakes
     "F",
@@ -152,52 +155,43 @@
 init_typed = true
 warn_required_dynamic_aliases = true
 
 [tool.pydocstyle]
 # https://github.com/PyCQA/pydocstyle
 # http://www.pydocstyle.org/en/stable/usage.html#available-options
 convention = "google"
-
+match_dir = "^(stac_model|tests)"
+# ignore missing documentation, just validate provided ones
+add_ignore = "D100,D101,D102,D103,D104,D105,D107,D200,D202,D204,D212,D401"
 
 [tool.pydoclint]
 # https://github.com/jsh9/pydoclint
 # https://jsh9.github.io/pydoclint/how_to_config.html
 style = "google"
-exclude = '''
-/(
-  \.git
-  | \.hg
-  | \.mypy_cache
-  | \.tox
-  | \.venv
-  | __pycache__
-  | _build
-  | buck-out
-  | build
-  | dist
-  | env
-  | venv
-)/
-'''
-
+exclude = '\.git|\.hg|\.mypy_cache|\.tox|.?v?env|__pycache__|_build|buck-out|dist|node_modules'
+# don't require type hints, since we have them in the signature instead (don't duplicate)
+arg-type-hints-in-docstring = false
+arg-type-hints-in-signature = true
+check-return-types = false
 
 [tool.pytest.ini_options]
 # https://github.com/pytest-dev/pytest
 # https://docs.pytest.org/en/6.2.x/customize.html#pyproject-toml
 # Directories that are not visited by pytest collector:
 norecursedirs =[
   "hooks",
   "*.egg",
   ".eggs",
   "dist",
   "build",
   "docs",
   ".tox",
   ".git",
-  "__pycache__"
+  "__pycache__",
+  "node_modules",
 ]
 doctest_optionflags = ["NUMBER", "NORMALIZE_WHITESPACE", "IGNORE_EXCEPTION_DETAIL"]
 timeout = 1000
 
 # Extra options:
 addopts = [
   "--strict-markers",
```

