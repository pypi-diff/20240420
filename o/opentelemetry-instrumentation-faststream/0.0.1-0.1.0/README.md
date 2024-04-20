# Comparing `tmp/opentelemetry_instrumentation_faststream-0.0.1.tar.gz` & `tmp/opentelemetry_instrumentation_faststream-0.1.0.tar.gz`

## Comparing `opentelemetry_instrumentation_faststream-0.0.1.tar` & `opentelemetry_instrumentation_faststream-0.1.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.0.1/src/opentelemetry/instrumentation/faststream/__about__.py
--rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.0.1/src/opentelemetry/instrumentation/faststream/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.0.1/src/opentelemetry/instrumentation/faststream/annotations.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.0.1/src/opentelemetry/instrumentation/faststream/package.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.0.1/src/opentelemetry/instrumentation/faststream/version.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.0.1/.gitignore
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.0.1/README.md
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/src/opentelemetry/instrumentation/faststream/__about__.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/src/opentelemetry/instrumentation/faststream/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/src/opentelemetry/instrumentation/faststream/annotations.py
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/src/opentelemetry/instrumentation/faststream/middlewares.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/src/opentelemetry/instrumentation/faststream/package.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/src/opentelemetry/instrumentation/faststream/version.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/README.md
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_faststream-0.0.1/.gitignore` & `opentelemetry_instrumentation_faststream-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_faststream-0.0.1/LICENSE.txt` & `opentelemetry_instrumentation_faststream-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_faststream-0.0.1/pyproject.toml` & `opentelemetry_instrumentation_faststream-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -23,19 +23,24 @@
   "opentelemetry-api ~= 1.5",
   "opentelemetry-instrumentation ~= 0.44b0",
   "wrapt >= 1.0.0, < 2.0.0",
 ]
 
 
 [project.optional-dependencies]
-instruments = ["faststream[redis] >= 0.4.4, < 0.5.0"]
+instruments = ["faststream[redis] >= 0.5.2, < 0.6.0"]
 quality = ["mypy~=1.8.0", "pre-commit~=3.6.0", "ruff~=0.3.0"]
 tests = [
-  "opentelemetry-instrumentation-faststream[instruments]",
-  "opentelemetry-test-utils ~= 0.44b0",
+  "opentelemetry-test-utils ~= 0.45b0",
+  "pytest-asyncio==0.23.6",
+  "aiokafka",
+  "nats-py",
+  "aio_pika",
+  "redis",
+  "faststream[redis,rabbit,nats,kafka] >= 0.5.2, < 0.6.0",
   "wrapt >= 1.0.0, < 2.0.0",
   "pytest~=8.0.0",
   "pytest-cov~=4.1",
 ]
 
 
 [project.urls]
@@ -45,15 +50,15 @@
 
 
 [tool.hatch.version]
 path = "src/opentelemetry/instrumentation/faststream/__about__.py"
 
 
 [tool.hatch.envs.quality]
-features = ["quality"]
+features = ["quality", "tests"]
 
 [tool.hatch.envs.quality.scripts]
 check = ["ruff check src tests --fix"]
 format = ["ruff format src tests", "check"]
 typecheck = ["mypy src --install-types --non-interactive"]
 
 [tool.mypy]
@@ -92,25 +97,18 @@
 
 [tool.hatch.envs.tests.scripts]
 run = "pytest --cov=REPLACE_PACKAGE_NAME --cov-report=term-missing tests/ --durations 0 -s {args:tests}"
 
 [[tool.hatch.envs.tests.matrix]]
 python = ["311", "312"]
 
-[tool.hatch.envs.docs]
-features = ["docs"]
-
-[tool.hatch.envs.docs.scripts]
-build = ["mkdocs build"]
-serve = ["mkdocs serve"]
-
 [tool.hatch.build.targets.sdist]
 exclude = [
   "/.github",
   "/.vscode",
   "/.pre-commit-config.yaml",
   "/.gitignore",
   "/tests",
 ]
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/opentelemetry"]
+packages = ["src/opentelemetry"]
```

