# Comparing `tmp/validate_pyproject_schema_store-2024.4.20.tar.gz` & `tmp/validate_pyproject_schema_store-2024.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Apr 20 05:10:51 2024, max compression
+gzip compressed data, last modified: Mon Apr  8 09:14:50 2024, max compression
```

## Comparing `validate_pyproject_schema_store-2024.4.20.tar` & `validate_pyproject_schema_store-2024.4.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     2272 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/.pre-commit-config.yaml
--rw-r--r--   0        0        0      305 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0     2412 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1007 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/.github/workflows/bump.yml
--rw-r--r--   0        0        0      843 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1193 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/.github/workflows/ci.yml
--rw-r--r--   0        0        0      188 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/py.typed
--rw-r--r--   0        0        0     1373 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/schema.py
--rw-r--r--   0        0        0     6871 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/black.schema.json
--rw-r--r--   0        0        0    20516 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json
--rw-r--r--   0        0        0    27093 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/hatch.schema.json
--rw-r--r--   0        0        0    44330 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/mypy.schema.json
--rw-r--r--   0        0        0    25354 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/pdm.schema.json
--rw-r--r--   0        0        0    20027 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/poetry.schema.json
--rw-r--r--   0        0        0    63177 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/pyright.schema.json
--rw-r--r--   0        0        0   127360 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/ruff.schema.json
--rw-r--r--   0        0        0    20535 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/scikit-build.schema.json
--rw-r--r--   0        0        0    13647 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/setuptools.schema.json
--rw-r--r--   0        0        0      643 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/tool.json
--rw-r--r--   0        0        0      890 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/tests/test_package.py
--rw-r--r--   0        0        0      425 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/tests/test_validate_pyproject.py
--rw-r--r--   0        0        0     2422 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/tools/sync.py
--rw-r--r--   0        0        0     2218 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/.gitignore
--rw-r--r--   0        0        0    11358 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/LICENSE
--rw-r--r--   0        0        0     2081 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/README.md
--rw-r--r--   0        0        0     5445 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/pyproject.toml
--rw-r--r--   0        0        0     4101 2024-04-20 05:10:51.000000 validate_pyproject_schema_store-2024.4.20/PKG-INFO
+-rw-r--r--   0        0        0     2272 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      305 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0     2412 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1007 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/.github/workflows/bump.yml
+-rw-r--r--   0        0        0      843 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1193 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      188 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/py.typed
+-rw-r--r--   0        0        0     1373 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/schema.py
+-rw-r--r--   0        0        0     6871 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/black.schema.json
+-rw-r--r--   0        0        0    20516 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json
+-rw-r--r--   0        0        0    27093 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/hatch.schema.json
+-rw-r--r--   0        0        0    44330 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/mypy.schema.json
+-rw-r--r--   0        0        0    25354 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/pdm.schema.json
+-rw-r--r--   0        0        0    20021 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/poetry.schema.json
+-rw-r--r--   0        0        0    63177 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/pyright.schema.json
+-rw-r--r--   0        0        0   125702 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/ruff.schema.json
+-rw-r--r--   0        0        0    18672 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/scikit-build.schema.json
+-rw-r--r--   0        0        0    13647 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/setuptools.schema.json
+-rw-r--r--   0        0        0      643 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/tool.json
+-rw-r--r--   0        0        0      890 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/tests/test_package.py
+-rw-r--r--   0        0        0      425 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/tests/test_validate_pyproject.py
+-rw-r--r--   0        0        0     2422 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/tools/sync.py
+-rw-r--r--   0        0        0     2218 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/.gitignore
+-rw-r--r--   0        0        0    11358 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/LICENSE
+-rw-r--r--   0        0        0     2081 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/README.md
+-rw-r--r--   0        0        0     5445 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/pyproject.toml
+-rw-r--r--   0        0        0     4100 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/PKG-INFO
```

### Comparing `validate_pyproject_schema_store-2024.4.20/.pre-commit-config.yaml` & `validate_pyproject_schema_store-2024.4.8/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   - repo: https://github.com/adamchainz/blacken-docs
     rev: "1.16.0"
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==24.*]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: "v4.6.0"
+    rev: "v4.5.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: debug-statements
@@ -30,15 +30,15 @@
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
         exclude: '^src/validate_pyproject_schema_store/resources/.*\.json'
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.3.7"
+    rev: "v0.3.5"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
       - id: ruff-format
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: "v1.9.0"
@@ -74,12 +74,12 @@
 
   - repo: https://github.com/abravalheri/validate-pyproject
     rev: v0.16
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.28.2
+    rev: 0.28.1
     hooks:
       - id: check-dependabot
       - id: check-github-workflows
       - id: check-readthedocs
```

### Comparing `validate_pyproject_schema_store-2024.4.20/.github/CONTRIBUTING.md` & `validate_pyproject_schema_store-2024.4.8/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.20/.github/matchers/pylint.json` & `validate_pyproject_schema_store-2024.4.8/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.20/.github/workflows/bump.yml` & `validate_pyproject_schema_store-2024.4.8/.github/workflows/bump.yml`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.20/.github/workflows/cd.yml` & `validate_pyproject_schema_store-2024.4.8/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.20/.github/workflows/ci.yml` & `validate_pyproject_schema_store-2024.4.8/.github/workflows/ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -48,8 +48,8 @@
 
       - name: Test package
         run: >-
           python -m pytest -ra --cov --cov-report=xml --cov-report=term
           --durations=20
 
       - name: Upload coverage report
-        uses: codecov/codecov-action@v4.3.0
+        uses: codecov/codecov-action@v4.2.0
```

### Comparing `validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/schema.py` & `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/schema.py`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/black.schema.json` & `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/black.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json` & `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/hatch.schema.json` & `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/hatch.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/mypy.schema.json` & `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/mypy.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/pdm.schema.json` & `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/pdm.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/poetry.schema.json` & `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/poetry.schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999999749599359%*

 * *Differences: {"'definitions'": "{'poetry-git-dependency': {'properties': {'git': {'anyOf': {1: {'pattern': "*

 * *                  "'^([A-Za-z0-9\\\\-]+@|https://|http://)[A-Za-z][A-Za-z0-9+.-]*(:|/)[A-Za-z0-9\\\\-]+/[A-Za-z0-9\\\\-_]+\\\\.git$'}}}}}}"}*

```diff
@@ -189,15 +189,15 @@
                 },
                 "git": {
                     "anyOf": [
                         {
                             "format": "uri"
                         },
                         {
-                            "pattern": "^([A-Za-z0-9\\-]+@|https://|http://)[A-Za-z][A-Za-z0-9+.-]*(:|/)[A-Za-z0-9\\-\\.]+/[A-Za-z0-9\\-_\\.]+\\.git$"
+                            "pattern": "^([A-Za-z0-9\\-]+@|https://|http://)[A-Za-z][A-Za-z0-9+.-]*(:|/)[A-Za-z0-9\\-]+/[A-Za-z0-9\\-_]+\\.git$"
                         }
                     ],
                     "description": "The url of the git repository.",
                     "type": "string"
                 },
                 "markers": {
                     "description": "The PEP 508 compliant environment markers for which the dependency should be installed.",
```

### Comparing `validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/pyright.schema.json` & `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/pyright.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/ruff.schema.json` & `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/ruff.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996361735727161%*

 * *Differences: {"'definitions'": "{'Flake8CopyrightOptions': {'properties': {'author': {'type': {insert: [(1, "*

 * *                  "'string')], delete: [0]}}, 'notice-rgx': {'description': 'The regular "*

 * *                  'expression used to match the copyright notice, compiled with the '*

 * *                  '[`regex`](https://docs.rs/regex/latest/regex/) crate. Defaults to '*

 * *                  '`(?i)Copyright\\\\s+((?:\\\\(C\\\\)|©)\\\\s+)?\\\\d{4}((-|,\\\\s)\\\\d{4})*`, '*

 * *                  'which matches the following: - `C […]*

```diff
@@ -151,30 +151,14 @@
                         "array",
                         "null"
                     ]
                 }
             },
             "type": "object"
         },
-        "Flake8BooleanTrapOptions": {
-            "additionalProperties": false,
-            "properties": {
-                "extend-allowed-calls": {
-                    "description": "Additional callable functions with which to allow boolean traps.\n\nExpects to receive a list of fully-qualified names (e.g., `pydantic.Field`, rather than `Field`).",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": [
-                        "array",
-                        "null"
-                    ]
-                }
-            },
-            "type": "object"
-        },
         "Flake8BugbearOptions": {
             "additionalProperties": false,
             "properties": {
                 "extend-immutable-calls": {
                     "description": "Additional callable functions to consider \"immutable\" when evaluating, e.g., the `function-call-in-default-argument` rule (`B008`) or `function-call-in-dataclass-defaults` rule (`RUF009`).\n\nExpects to receive a list of fully-qualified names (e.g., `fastapi.Query`, rather than `Query`).",
                     "items": {
                         "type": "string"
@@ -218,44 +202,44 @@
         },
         "Flake8CopyrightOptions": {
             "additionalProperties": false,
             "properties": {
                 "author": {
                     "description": "Author to enforce within the copyright notice. If provided, the author must be present immediately following the copyright notice.",
                     "type": [
-                        "string",
-                        "null"
+                        "null",
+                        "string"
                     ]
                 },
                 "min-file-size": {
                     "description": "A minimum file size (in bytes) required for a copyright notice to be enforced. By default, all files are validated.",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "notice-rgx": {
-                    "description": "The regular expression used to match the copyright notice, compiled with the [`regex`](https://docs.rs/regex/latest/regex/) crate. Defaults to `(?i)Copyright\\s+((?:\\(C\\)|\u00a9)\\s+)?\\d{4}((-|,\\s)\\d{4})*`, which matches the following:\n\n- `Copyright 2023` - `Copyright (C) 2023` - `Copyright 2021-2023` - `Copyright (C) 2021-2023` - `Copyright (C) 2021, 2023`",
+                    "description": "The regular expression used to match the copyright notice, compiled with the [`regex`](https://docs.rs/regex/latest/regex/) crate. Defaults to `(?i)Copyright\\s+((?:\\(C\\)|\u00a9)\\s+)?\\d{4}((-|,\\s)\\d{4})*`, which matches the following: - `Copyright 2023` - `Copyright (C) 2023` - `Copyright 2021-2023` - `Copyright (C) 2021-2023` - `Copyright (C) 2021, 2023`",
                     "type": [
-                        "string",
-                        "null"
+                        "null",
+                        "string"
                     ]
                 }
             },
             "type": "object"
         },
         "Flake8ErrMsgOptions": {
             "additionalProperties": false,
             "properties": {
                 "max-string-length": {
                     "description": "Maximum string length for string literals in exception messages.",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 }
             },
             "type": "object"
@@ -302,28 +286,28 @@
         "Flake8ImportConventionsOptions": {
             "additionalProperties": false,
             "properties": {
                 "aliases": {
                     "additionalProperties": {
                         "type": "string"
                     },
-                    "description": "The conventional aliases for imports. These aliases can be extended by the `extend-aliases` option.",
+                    "description": "The conventional aliases for imports. These aliases can be extended by the `extend_aliases` option.",
                     "type": [
-                        "object",
-                        "null"
+                        "null",
+                        "object"
                     ]
                 },
                 "banned-aliases": {
                     "additionalProperties": {
                         "$ref": "#/definitions/BannedAliases"
                     },
                     "description": "A mapping from module to its banned import aliases.",
                     "type": [
-                        "object",
-                        "null"
+                        "null",
+                        "object"
                     ]
                 },
                 "banned-from": {
                     "description": "A list of modules that should not be imported from using the `from ... import ...` syntax.\n\nFor example, given `banned-from = [\"pandas\"]`, `from pandas import DataFrame` would be disallowed, while `import pandas` would be allowed.",
                     "items": {
                         "type": "string"
                     },
@@ -335,16 +319,16 @@
                 },
                 "extend-aliases": {
                     "additionalProperties": {
                         "type": "string"
                     },
                     "description": "A mapping from module to conventional import alias. These aliases will be added to the `aliases` mapping.",
                     "type": [
-                        "object",
-                        "null"
+                        "null",
+                        "object"
                     ]
                 }
             },
             "type": "object"
         },
         "Flake8PytestStyleOptions": {
             "additionalProperties": false,
@@ -507,16 +491,16 @@
                 },
                 "banned-api": {
                     "additionalProperties": {
                         "$ref": "#/definitions/ApiBan"
                     },
                     "description": "Specific modules or module members that may not be imported or accessed. Note that this rule is only meant to flag accidental uses, and can be circumvented via `eval` or `importlib`.",
                     "type": [
-                        "object",
-                        "null"
+                        "null",
+                        "object"
                     ]
                 },
                 "banned-module-level-imports": {
                     "description": "List of specific modules that may not be imported at module level, and should instead be imported lazily (e.g., within a function definition, or an `if TYPE_CHECKING:` block, or some other nested context).",
                     "items": {
                         "type": "string"
                     },
@@ -657,15 +641,15 @@
                         {
                             "$ref": "#/definitions/QuoteStyle"
                         },
                         {
                             "type": "null"
                         }
                     ],
-                    "description": "Configures the preferred quote character for strings. The recommended options are\n\n* `double` (default): Use double quotes `\"` * `single`: Use single quotes `'`\n\nIn compliance with [PEP 8](https://peps.python.org/pep-0008/) and [PEP 257](https://peps.python.org/pep-0257/), Ruff prefers double quotes for triple quoted strings and docstrings even when using `quote-style = \"single\"`.\n\nRuff deviates from using the configured quotes if doing so prevents the need for escaping quote characters inside the string:\n\n```python a = \"a string without any quotes\" b = \"It's monday morning\" ```\n\nRuff will change the quotes of the string assigned to `a` to single quotes when using `quote-style = \"single\"`. However, ruff uses double quotes for he string assigned to `b` because using single quotes would require escaping the `'`, which leads to the less readable code: `'It\\'s monday morning'`.\n\nIn addition, Ruff supports the quote style `preserve` for projects that already use a mixture of single and double quotes and can't migrate to the `double` or `single` style. The quote style `preserve` leaves the quotes of all strings unchanged."
+                    "description": "Configures the preferred quote character for strings. The recommended options are * `double` (default): Use double quotes `\"` * `single`: Use single quotes `'`\n\nIn compliance with [PEP 8](https://peps.python.org/pep-0008/) and [PEP 257](https://peps.python.org/pep-0257/), Ruff prefers double quotes for triple quoted strings and docstrings even when using `quote-style = \"single\"`.\n\nRuff deviates from using the configured quotes if doing so prevents the need for escaping quote characters inside the string:\n\n```python a = \"a string without any quotes\" b = \"It's monday morning\" ```\n\nRuff will change the quotes of the string assigned to `a` to single quotes when using `quote-style = \"single\"`. However, ruff uses double quotes for he string assigned to `b` because using single quotes would require escaping the `'`, which leads to the less readable code: `'It\\'s monday morning'`.\n\nIn addition, Ruff supports the quote style `preserve` for projects that already use a mixture of single and double quotes and can't migrate to the `double` or `single` style. The quote style `preserve` leaves the quotes of all strings unchanged."
                 },
                 "skip-magic-trailing-comma": {
                     "description": "Ruff uses existing trailing commas as an indication that short lines should be left separate. If this option is set to `true`, the magic trailing comma is ignored.\n\nFor example, Ruff leaves the arguments separate even though collapsing the arguments to a single line doesn't exceed the line length if `skip-magic-trailing-comma = false`:\n\n```python # The arguments remain on separate lines because of the trailing comma after `b` def test( a, b, ): pass ```\n\nSetting `skip-magic-trailing-comma = true` changes the formatting to:\n\n```python # The arguments remain on separate lines because of the trailing comma after `b` def test(a, b): pass ```",
                     "type": [
                         "boolean",
                         "null"
                     ]
@@ -681,19 +665,19 @@
                 {
                     "type": "string"
                 }
             ]
         },
         "ImportType": {
             "enum": [
+                "first-party",
                 "future",
+                "local-folder",
                 "standard-library",
-                "third-party",
-                "first-party",
-                "local-folder"
+                "third-party"
             ],
             "type": "string"
         },
         "IndentStyle": {
             "oneOf": [
                 {
                     "description": "Use tabs to indent code.",
@@ -710,15 +694,15 @@
                     "type": "string"
                 }
             ]
         },
         "IndentWidth": {
             "description": "The size of a tab.",
             "format": "uint8",
-            "minimum": 1.0,
+            "minimum": 1,
             "type": "integer"
         },
         "IsortOptions": {
             "additionalProperties": false,
             "properties": {
                 "case-sensitive": {
                     "description": "Sort imports taking into account case sensitivity.",
@@ -881,15 +865,15 @@
                         "integer",
                         "null"
                     ]
                 },
                 "lines-between-types": {
                     "description": "The number of lines to place between \"direct\" and `import from` imports.\n\nWhen using the formatter, only the values `0` and `1` are compatible because it preserves up to one empty line after imports in nested blocks.",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "no-lines-before": {
                     "description": "A list of sections that should _not_ be delineated from the previous section via empty lines.",
@@ -951,16 +935,16 @@
                         "items": {
                             "type": "string"
                         },
                         "type": "array"
                     },
                     "description": "A list of mappings from section names to modules. By default custom sections are output last, but this can be overridden with `section-order`.",
                     "type": [
-                        "object",
-                        "null"
+                        "null",
+                        "object"
                     ]
                 },
                 "single-line-exclusions": {
                     "description": "One or more modules to exclude from the single line rule.",
                     "items": {
                         "type": "string"
                     },
@@ -1020,22 +1004,22 @@
                     "type": "string"
                 }
             ]
         },
         "LineLength": {
             "description": "The length of a line of text that is considered too long.\n\nThe allowed range of values is 1..=320",
             "format": "uint16",
-            "maximum": 320.0,
-            "minimum": 1.0,
+            "maximum": 320,
+            "minimum": 1,
             "type": "integer"
         },
         "LineWidth": {
             "description": "The maximum visual width to which the formatter should try to limit a line.",
             "format": "uint16",
-            "minimum": 1.0,
+            "minimum": 1,
             "type": "integer"
         },
         "LintOptions": {
             "additionalProperties": false,
             "description": "Configures how ruff checks your code.\n\nOptions specified in the `lint` section take precedence over the deprecated top-level settings.",
             "properties": {
                 "allowed-confusables": {
@@ -1049,16 +1033,16 @@
                         "array",
                         "null"
                     ]
                 },
                 "dummy-variable-rgx": {
                     "description": "A regular expression used to identify \"dummy\" variables, or those which should be ignored when enforcing (e.g.) unused-variable rules. The default expression matches `_`, `__`, and `_var`, but not `_var_`.",
                     "type": [
-                        "string",
-                        "null"
+                        "null",
+                        "string"
                     ]
                 },
                 "exclude": {
                     "description": "A list of file patterns to exclude from linting in addition to the files excluded globally (see [`exclude`](#exclude), and [`extend-exclude`](#extend-exclude)).\n\nExclusions are based on globs, and can be either:\n\n- Single-path patterns, like `.mypy_cache` (to exclude any directory named `.mypy_cache` in the tree), `foo.py` (to exclude any file named `foo.py`), or `foo_*.py` (to exclude any file matching `foo_*.py` ). - Relative patterns, like `directory/foo.py` (to exclude that specific file) or `directory/*.py` (to exclude any Python files in `directory`). Note that these paths are relative to the project root (e.g., the directory containing your `pyproject.toml`).\n\nFor more information on the glob syntax, refer to the [`globset` documentation](https://docs.rs/globset/latest/globset/#syntax).",
                     "items": {
                         "type": "string"
                     },
@@ -1100,16 +1084,16 @@
                         "items": {
                             "$ref": "#/definitions/RuleSelector"
                         },
                         "type": "array"
                     },
                     "description": "A list of mappings from file pattern to rule codes or prefixes to exclude, in addition to any rules excluded by `per-file-ignores`.",
                     "type": [
-                        "object",
-                        "null"
+                        "null",
+                        "object"
                     ]
                 },
                 "extend-safe-fixes": {
                     "description": "A list of rule codes or prefixes for which unsafe fixes should be considered safe.",
                     "items": {
                         "$ref": "#/definitions/RuleSelector"
                     },
@@ -1187,25 +1171,14 @@
                         },
                         {
                             "type": "null"
                         }
                     ],
                     "description": "Options for the `flake8-bandit` plugin."
                 },
-                "flake8-boolean-trap": {
-                    "anyOf": [
-                        {
-                            "$ref": "#/definitions/Flake8BooleanTrapOptions"
-                        },
-                        {
-                            "type": "null"
-                        }
-                    ],
-                    "description": "Options for the `flake8-boolean-trap` plugin."
-                },
                 "flake8-bugbear": {
                     "anyOf": [
                         {
                             "$ref": "#/definitions/Flake8BugbearOptions"
                         },
                         {
                             "type": "null"
@@ -1419,18 +1392,18 @@
                 "per-file-ignores": {
                     "additionalProperties": {
                         "items": {
                             "$ref": "#/definitions/RuleSelector"
                         },
                         "type": "array"
                     },
-                    "description": "A list of mappings from file pattern to rule codes or prefixes to exclude, when considering any matching files. An initial '!' negates the file pattern.",
+                    "description": "A list of mappings from file pattern to rule codes or prefixes to exclude, when considering any matching files.",
                     "type": [
-                        "object",
-                        "null"
+                        "null",
+                        "object"
                     ]
                 },
                 "preview": {
                     "description": "Whether to enable preview mode. When preview mode is enabled, Ruff will use unstable rules and fixes.",
                     "type": [
                         "boolean",
                         "null"
@@ -1536,42 +1509,42 @@
         },
         "McCabeOptions": {
             "additionalProperties": false,
             "properties": {
                 "max-complexity": {
                     "description": "The maximum McCabe complexity to allow before triggering `C901` errors.",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 }
             },
             "type": "object"
         },
         "ParametrizeNameType": {
             "enum": [
                 "csv",
-                "tuple",
-                "list"
+                "list",
+                "tuple"
             ],
             "type": "string"
         },
         "ParametrizeValuesRowType": {
             "enum": [
-                "tuple",
-                "list"
+                "list",
+                "tuple"
             ],
             "type": "string"
         },
         "ParametrizeValuesType": {
             "enum": [
-                "tuple",
-                "list"
+                "list",
+                "tuple"
             ],
             "type": "string"
         },
         "Pep8NamingOptions": {
             "additionalProperties": false,
             "properties": {
                 "classmethod-decorators": {
@@ -1741,103 +1714,103 @@
                         "array",
                         "null"
                     ]
                 },
                 "max-args": {
                     "description": "Maximum number of arguments allowed for a function or method definition (see: `PLR0913`).",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-bool-expr": {
                     "description": "Maximum number of Boolean expressions allowed within a single `if` statement (see: `PLR0916`).",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-branches": {
                     "description": "Maximum number of branches allowed for a function or method body (see: `PLR0912`).",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-locals": {
                     "description": "Maximum number of local variables allowed for a function or method body (see: `PLR0914`).",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-nested-blocks": {
                     "description": "Maximum number of nested blocks allowed within a function or method body (see: `PLR1702`).",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-positional-args": {
                     "description": "Maximum number of positional arguments allowed for a function or method definition (see: `PLR0917`).\n\nIf not specified, defaults to the value of `max-args`.",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-public-methods": {
                     "description": "Maximum number of public methods allowed for a class (see: `PLR0904`).",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-returns": {
                     "description": "Maximum number of return statements allowed for a function or method body (see `PLR0911`)",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-statements": {
                     "description": "Maximum number of statements allowed for a function or method body (see: `PLR0915`).",
                     "format": "uint",
-                    "minimum": 0.0,
+                    "minimum": 0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 }
             },
             "type": "object"
         },
         "PythonVersion": {
             "enum": [
-                "py37",
-                "py38",
-                "py39",
                 "py310",
                 "py311",
-                "py312"
+                "py312",
+                "py37",
+                "py38",
+                "py39"
             ],
             "type": "string"
         },
         "Quote": {
             "oneOf": [
                 {
                     "description": "Use double quotes.",
@@ -1853,17 +1826,17 @@
                     ],
                     "type": "string"
                 }
             ]
         },
         "QuoteStyle": {
             "enum": [
-                "single",
                 "double",
-                "preserve"
+                "preserve",
+                "single"
             ],
             "type": "string"
         },
         "RelativeImportsOrder": {
             "oneOf": [
                 {
                     "description": "Place \"closer\" imports (fewer `.` characters, most local) before \"further\" imports (more `.` characters, least local).",
@@ -1971,15 +1944,14 @@
                 "B033",
                 "B034",
                 "B035",
                 "B9",
                 "B90",
                 "B904",
                 "B905",
-                "B909",
                 "BLE",
                 "BLE0",
                 "BLE00",
                 "BLE001",
                 "C",
                 "C4",
                 "C40",
@@ -2286,39 +2258,33 @@
                 "FLY0",
                 "FLY00",
                 "FLY002",
                 "FURB",
                 "FURB1",
                 "FURB10",
                 "FURB101",
-                "FURB103",
                 "FURB105",
                 "FURB11",
-                "FURB110",
                 "FURB113",
                 "FURB118",
                 "FURB12",
                 "FURB129",
                 "FURB13",
                 "FURB131",
                 "FURB132",
                 "FURB136",
                 "FURB14",
                 "FURB140",
-                "FURB142",
                 "FURB145",
                 "FURB148",
                 "FURB15",
                 "FURB152",
-                "FURB157",
                 "FURB16",
                 "FURB161",
                 "FURB163",
-                "FURB164",
-                "FURB166",
                 "FURB167",
                 "FURB168",
                 "FURB169",
                 "FURB17",
                 "FURB171",
                 "FURB177",
                 "FURB18",
@@ -2511,18 +2477,16 @@
                 "PLE023",
                 "PLE0237",
                 "PLE024",
                 "PLE0241",
                 "PLE03",
                 "PLE030",
                 "PLE0302",
-                "PLE0303",
                 "PLE0304",
                 "PLE0307",
-                "PLE0308",
                 "PLE06",
                 "PLE060",
                 "PLE0604",
                 "PLE0605",
                 "PLE064",
                 "PLE0643",
                 "PLE07",
@@ -2561,18 +2525,14 @@
                 "PLE2502",
                 "PLE251",
                 "PLE2510",
                 "PLE2512",
                 "PLE2513",
                 "PLE2514",
                 "PLE2515",
-                "PLE4",
-                "PLE47",
-                "PLE470",
-                "PLE4703",
                 "PLR",
                 "PLR0",
                 "PLR01",
                 "PLR012",
                 "PLR0124",
                 "PLR013",
                 "PLR0133",
@@ -2603,67 +2563,59 @@
                 "PLR1704",
                 "PLR171",
                 "PLR1711",
                 "PLR1714",
                 "PLR172",
                 "PLR1722",
                 "PLR173",
-                "PLR1730",
                 "PLR1733",
                 "PLR1736",
                 "PLR2",
                 "PLR20",
                 "PLR200",
                 "PLR2004",
                 "PLR204",
                 "PLR2044",
                 "PLR5",
                 "PLR55",
                 "PLR550",
                 "PLR5501",
                 "PLR6",
-                "PLR61",
-                "PLR610",
-                "PLR6104",
                 "PLR62",
                 "PLR620",
                 "PLR6201",
                 "PLR63",
                 "PLR630",
                 "PLR6301",
                 "PLW",
                 "PLW0",
                 "PLW01",
                 "PLW010",
                 "PLW0108",
+                "PLW011",
+                "PLW0117",
                 "PLW012",
                 "PLW0120",
                 "PLW0127",
                 "PLW0128",
                 "PLW0129",
                 "PLW013",
                 "PLW0131",
                 "PLW0133",
-                "PLW017",
-                "PLW0177",
                 "PLW02",
-                "PLW021",
-                "PLW0211",
                 "PLW024",
                 "PLW0245",
                 "PLW04",
                 "PLW040",
                 "PLW0406",
                 "PLW06",
                 "PLW060",
                 "PLW0602",
                 "PLW0603",
                 "PLW0604",
-                "PLW064",
-                "PLW0642",
                 "PLW07",
                 "PLW071",
                 "PLW0711",
                 "PLW1",
                 "PLW15",
                 "PLW150",
                 "PLW1501",
@@ -2865,15 +2817,14 @@
                 "RUF022",
                 "RUF023",
                 "RUF024",
                 "RUF025",
                 "RUF026",
                 "RUF027",
                 "RUF028",
-                "RUF029",
                 "RUF1",
                 "RUF10",
                 "RUF100",
                 "RUF2",
                 "RUF20",
                 "RUF200",
                 "S",
@@ -3123,15 +3074,14 @@
                 "UP036",
                 "UP037",
                 "UP038",
                 "UP039",
                 "UP04",
                 "UP040",
                 "UP041",
-                "UP042",
                 "W",
                 "W1",
                 "W19",
                 "W191",
                 "W2",
                 "W29",
                 "W291",
@@ -3164,26 +3114,26 @@
                 "YTT302",
                 "YTT303"
             ],
             "type": "string"
         },
         "SerializationFormat": {
             "enum": [
-                "text",
+                "azure",
                 "concise",
                 "full",
+                "github",
+                "gitlab",
+                "grouped",
                 "json",
                 "json-lines",
                 "junit",
-                "grouped",
-                "github",
-                "gitlab",
                 "pylint",
-                "azure",
-                "sarif"
+                "sarif",
+                "text"
             ],
             "type": "string"
         },
         "Strictness": {
             "oneOf": [
                 {
                     "description": "Ban imports that extend into the parent module or beyond.",
@@ -3225,24 +3175,24 @@
                 "array",
                 "null"
             ]
         },
         "cache-dir": {
             "description": "A path to the cache directory.\n\nBy default, Ruff stores cache results in a `.ruff_cache` directory in the current project root.\n\nHowever, Ruff will also respect the `RUFF_CACHE_DIR` environment variable, which takes precedence over that default.\n\nThis setting will override even the `RUFF_CACHE_DIR` environment variable, if set.",
             "type": [
-                "string",
-                "null"
+                "null",
+                "string"
             ]
         },
         "dummy-variable-rgx": {
             "deprecated": true,
             "description": "A regular expression used to identify \"dummy\" variables, or those which should be ignored when enforcing (e.g.) unused-variable rules. The default expression matches `_`, `__`, and `_var`, but not `_var_`.",
             "type": [
-                "string",
-                "null"
+                "null",
+                "string"
             ]
         },
         "exclude": {
             "description": "A list of file patterns to exclude from formatting and linting.\n\nExclusions are based on globs, and can be either:\n\n- Single-path patterns, like `.mypy_cache` (to exclude any directory named `.mypy_cache` in the tree), `foo.py` (to exclude any file named `foo.py`), or `foo_*.py` (to exclude any file matching `foo_*.py` ). - Relative patterns, like `directory/foo.py` (to exclude that specific file) or `directory/*.py` (to exclude any Python files in `directory`). Note that these paths are relative to the project root (e.g., the directory containing your `pyproject.toml`).\n\nFor more information on the glob syntax, refer to the [`globset` documentation](https://docs.rs/globset/latest/globset/#syntax).\n\nNote that you'll typically want to use [`extend-exclude`](#extend-exclude) to modify the excluded paths.",
             "items": {
                 "type": "string"
             },
@@ -3258,16 +3208,16 @@
                 "boolean",
                 "null"
             ]
         },
         "extend": {
             "description": "A path to a local `pyproject.toml` file to merge into this configuration. User home directory and environment variables will be expanded.\n\nTo resolve the current `pyproject.toml` file, Ruff will first resolve this base configuration file, then merge in any properties defined in the current configuration file.",
             "type": [
-                "string",
-                "null"
+                "null",
+                "string"
             ]
         },
         "extend-exclude": {
             "description": "A list of file patterns to omit from formatting and linting, in addition to those specified by `exclude`.\n\nExclusions are based on globs, and can be either:\n\n- Single-path patterns, like `.mypy_cache` (to exclude any directory named `.mypy_cache` in the tree), `foo.py` (to exclude any file named `foo.py`), or `foo_*.py` (to exclude any file matching `foo_*.py` ). - Relative patterns, like `directory/foo.py` (to exclude that specific file) or `directory/*.py` (to exclude any Python files in `directory`). Note that these paths are relative to the project root (e.g., the directory containing your `pyproject.toml`).\n\nFor more information on the glob syntax, refer to the [`globset` documentation](https://docs.rs/globset/latest/globset/#syntax).",
             "items": {
                 "type": "string"
             },
@@ -3314,16 +3264,16 @@
                     "$ref": "#/definitions/RuleSelector"
                 },
                 "type": "array"
             },
             "deprecated": true,
             "description": "A list of mappings from file pattern to rule codes or prefixes to exclude, in addition to any rules excluded by `per-file-ignores`.",
             "type": [
-                "object",
-                "null"
+                "null",
+                "object"
             ]
         },
         "extend-safe-fixes": {
             "deprecated": true,
             "description": "A list of rule codes or prefixes for which unsafe fixes should be considered safe.",
             "items": {
                 "$ref": "#/definitions/RuleSelector"
@@ -3422,26 +3372,14 @@
                 {
                     "type": "null"
                 }
             ],
             "deprecated": true,
             "description": "Options for the `flake8-bandit` plugin."
         },
-        "flake8-boolean-trap": {
-            "anyOf": [
-                {
-                    "$ref": "#/definitions/Flake8BooleanTrapOptions"
-                },
-                {
-                    "type": "null"
-                }
-            ],
-            "deprecated": true,
-            "description": "Options for the `flake8-boolean-trap` plugin."
-        },
         "flake8-bugbear": {
             "anyOf": [
                 {
                     "$ref": "#/definitions/Flake8BugbearOptions"
                 },
                 {
                     "type": "null"
@@ -3717,15 +3655,15 @@
                     "type": "null"
                 }
             ],
             "deprecated": true,
             "description": "Options for the `mccabe` plugin."
         },
         "namespace-packages": {
-            "description": "Mark the specified directories as namespace packages. For the purpose of module resolution, Ruff will treat those directories and all their subdirectories as if they contained an `__init__.py` file.",
+            "description": "Mark the specified directories as namespace packages. For the purpose of module resolution, Ruff will treat those directories as if they contained an `__init__.py` file.",
             "items": {
                 "type": "string"
             },
             "type": [
                 "array",
                 "null"
             ]
@@ -3757,18 +3695,18 @@
             "additionalProperties": {
                 "items": {
                     "$ref": "#/definitions/RuleSelector"
                 },
                 "type": "array"
             },
             "deprecated": true,
-            "description": "A list of mappings from file pattern to rule codes or prefixes to exclude, when considering any matching files. An initial '!' negates the file pattern.",
+            "description": "A list of mappings from file pattern to rule codes or prefixes to exclude, when considering any matching files.",
             "type": [
-                "object",
-                "null"
+                "null",
+                "object"
             ]
         },
         "preview": {
             "description": "Whether to enable preview mode. When preview mode is enabled, Ruff will use unstable rules, fixes, and formatting.",
             "type": [
                 "boolean",
                 "null"
```

### Comparing `validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/scikit-build.schema.json` & `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/scikit-build.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761732987948265%*

 * *Differences: {"'$defs'": "{delete: ['inherit']}",*

 * * "'properties'": "{'ninja': {'properties': {'make-fallback': {'description': 'If CMake is not "*

 * *                 'present on the system or is older required, it will be downloaded via PyPI if '*

 * *                 "possible. An empty string will disable this check.'}}}, 'wheel': {'properties': "*

 * *                 "{'exclude': {'description': 'A set of patterns to exclude from the wheel. This "*

 * *                 'is additive to the SDist exclude patterns. This applies to the s […]*

```diff
@@ -49,22 +49,14 @@
                 "state": {
                     "description": "The state of the build, one of `sdist`, `wheel`, `editable`, `metadata_wheel`, and `metadata_editable`. Takes a regex.",
                     "type": "string"
                 }
             },
             "type": "object"
         },
-        "inherit": {
-            "default": "none",
-            "enum": [
-                "none",
-                "append",
-                "prepend"
-            ]
-        },
         "metadata": {
             "properties": {
                 "provider": {
                     "type": "string"
                 },
                 "provider-path": {
                     "type": "string"
@@ -368,15 +360,15 @@
             "type": "string"
         },
         "ninja": {
             "additionalProperties": false,
             "properties": {
                 "make-fallback": {
                     "default": true,
-                    "description": "If Ninja is not present on the system or is older than required, it will be downloaded via PyPI if this is false.",
+                    "description": "If CMake is not present on the system or is older required, it will be downloaded via PyPI if possible. An empty string will disable this check.",
                     "type": "boolean"
                 },
                 "minimum-version": {
                     "deprecated": true,
                     "description": "DEPRECATED in 0.8; use version instead.",
                     "type": "string"
                 },
@@ -427,71 +419,14 @@
                                 "required": [
                                     "any"
                                 ],
                                 "type": "object"
                             }
                         ]
                     },
-                    "inherit": {
-                        "additionalProperties": false,
-                        "properties": {
-                            "cmake": {
-                                "additionalProperties": false,
-                                "properties": {
-                                    "args": {
-                                        "$ref": "#/$defs/inherit"
-                                    },
-                                    "define": {
-                                        "$ref": "#/$defs/inherit"
-                                    },
-                                    "targets": {
-                                        "$ref": "#/$defs/inherit"
-                                    }
-                                },
-                                "type": "object"
-                            },
-                            "install": {
-                                "additionalProperties": false,
-                                "properties": {
-                                    "components": {
-                                        "$ref": "#/$defs/inherit"
-                                    }
-                                },
-                                "type": "object"
-                            },
-                            "sdist": {
-                                "additionalProperties": false,
-                                "properties": {
-                                    "exclude": {
-                                        "$ref": "#/$defs/inherit"
-                                    },
-                                    "include": {
-                                        "$ref": "#/$defs/inherit"
-                                    }
-                                },
-                                "type": "object"
-                            },
-                            "wheel": {
-                                "additionalProperties": false,
-                                "properties": {
-                                    "exclude": {
-                                        "$ref": "#/$defs/inherit"
-                                    },
-                                    "license-files": {
-                                        "$ref": "#/$defs/inherit"
-                                    },
-                                    "packages": {
-                                        "$ref": "#/$defs/inherit"
-                                    }
-                                },
-                                "type": "object"
-                            }
-                        },
-                        "type": "object"
-                    },
                     "install": {
                         "$ref": "#/properties/install"
                     },
                     "logging": {
                         "$ref": "#/properties/logging"
                     },
                     "metadata": {
@@ -565,15 +500,15 @@
                 },
                 "cmake": {
                     "default": true,
                     "description": "If set to True (the default), CMake will be run before building the wheel.",
                     "type": "boolean"
                 },
                 "exclude": {
-                    "description": "A set of patterns to exclude from the wheel. This is additive to the SDist exclude patterns. This applies to the final paths in the wheel, and can exclude files from CMake output as well.  Editable installs may not respect this exclusion.",
+                    "description": "A set of patterns to exclude from the wheel. This is additive to the SDist exclude patterns. This applies to the source files, not the final paths. Editable installs may not respect this exclusion.",
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
                 "expand-macos-universal-tags": {
                     "default": false,
```

### Comparing `validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/setuptools.schema.json` & `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/setuptools.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.20/src/validate_pyproject_schema_store/resources/tool.json` & `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/tool.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.20/tests/test_package.py` & `validate_pyproject_schema_store-2024.4.8/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.20/tools/sync.py` & `validate_pyproject_schema_store-2024.4.8/tools/sync.py`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.20/.gitignore` & `validate_pyproject_schema_store-2024.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.20/LICENSE` & `validate_pyproject_schema_store-2024.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.20/README.md` & `validate_pyproject_schema_store-2024.4.8/README.md`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.20/pyproject.toml` & `validate_pyproject_schema_store-2024.4.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "validate-pyproject-schema-store"
-version = "2024.04.20"
+version = "2024.04.08"
 authors = [
   { name = "Henry Schreiner", email = "henryfs@princeton.edu" },
 ]
 description = "A plugin set for validate-pyproject and schema-store."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `validate_pyproject_schema_store-2024.4.20/PKG-INFO` & `validate_pyproject_schema_store-2024.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: validate-pyproject-schema-store
-Version: 2024.4.20
+Version: 2024.4.8
 Summary: A plugin set for validate-pyproject and schema-store.
 Project-URL: Homepage, https://github.com/henryiii/validate-pyproject-schema-store
 Project-URL: Bug Tracker, https://github.com/henryiii/validate-pyproject-schema-store/issues
 Project-URL: Discussions, https://github.com/henryiii/validate-pyproject-schema-store/discussions
 Project-URL: Changelog, https://github.com/henryiii/validate-pyproject-schema-store/releases
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License-File: LICENSE
```

