# Comparing `tmp/reprompt-0.0.7.5.tar.gz` & `tmp/reprompt-0.0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprompt-0.0.7.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "reprompt-0.0.7.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `reprompt-0.0.7.5.tar` & `reprompt-0.0.7.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      334 2024-04-18 23:41:16.576013 reprompt-0.0.7.5/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1157 2024-04-18 23:41:16.576013 reprompt-0.0.7.5/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      417 2024-04-18 23:41:16.576013 reprompt-0.0.7.5/.github/dependabot.yml
--rw-r--r--   0        0        0      418 2024-04-18 23:41:16.576013 reprompt-0.0.7.5/.github/template-sync.yml
--rw-r--r--   0        0        0      472 2024-04-18 23:41:16.576013 reprompt-0.0.7.5/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-04-18 23:41:16.576013 reprompt-0.0.7.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      368 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/.gitignore
--rw-r--r--   0        0        0     1540 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/.pypirc
--rw-r--r--   0        0        0      459 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/.vscode/launch.json
--rw-r--r--   0        0        0      817 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/.vscode/settings.json
--rw-r--r--   0        0        0     1127 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/LICENSE
--rw-r--r--   0        0        0     7737 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/README.md
--rw-r--r--   0        0        0      634 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/Makefile
--rw-r--r--   0        0        0     2321 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/conf.py
--rw-r--r--   0        0        0      360 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/developer.md
--rw-r--r--   0        0        0      468 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/index.rst
--rw-r--r--   0        0        0      800 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/make.bat
--rw-r--r--   0        0        0       51 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/pyproject.md
--rw-r--r--   0        0        0      425 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      415 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/python_package.rst
--rw-r--r--   0        0        0       42 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/docs/workflows.md
--rw-r--r--   0        0        0     6649 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/pyproject.toml
--rw-r--r--   0        0        0     1241 2024-04-18 23:41:29.063994 reprompt-0.0.7.5/src/reprompt/__init__.py
--rw-r--r--   0        0        0      859 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/src/reprompt/background_task_manager.py
--rw-r--r--   0        0        0      167 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/src/reprompt/config.py
--rw-r--r--   0        0        0     3371 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/src/reprompt/tracing.py
--rw-r--r--   0        0        0      989 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/tests/conftest.py
--rw-r--r--   0        0        0      511 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/tests/openai_example_script.py
--rw-r--r--   0        0        0      283 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/tests/test_init.py
--rw-r--r--   0        0        0     1673 2024-04-18 23:41:16.580013 reprompt-0.0.7.5/tests/test_openai_tracing.py
--rw-r--r--   0        0        0     9640 1970-01-01 00:00:00.000000 reprompt-0.0.7.5/PKG-INFO
+-rw-r--r--   0        0        0      334 2024-04-04 23:08:33.473524 reprompt-0.0.7.6/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1157 2024-04-04 23:08:33.473643 reprompt-0.0.7.6/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      417 2024-04-04 23:08:33.473790 reprompt-0.0.7.6/.github/dependabot.yml
+-rw-r--r--   0        0        0      418 2024-04-04 23:08:33.473883 reprompt-0.0.7.6/.github/template-sync.yml
+-rw-r--r--   0        0        0      472 2024-04-07 21:52:20.071061 reprompt-0.0.7.6/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-07 21:52:20.071267 reprompt-0.0.7.6/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-19 03:54:13.429435 reprompt-0.0.7.6/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      368 2024-04-04 23:08:33.474380 reprompt-0.0.7.6/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2024-04-19 03:54:13.429968 reprompt-0.0.7.6/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2024-04-04 23:08:33.474551 reprompt-0.0.7.6/.gitignore
+-rw-r--r--   0        0        0     1540 2024-04-04 23:08:33.474640 reprompt-0.0.7.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-04 23:08:33.474722 reprompt-0.0.7.6/.pypirc
+-rw-r--r--   0        0        0      459 2024-04-04 23:08:33.474853 reprompt-0.0.7.6/.vscode/launch.json
+-rw-r--r--   0        0        0      817 2024-04-04 23:08:33.474937 reprompt-0.0.7.6/.vscode/settings.json
+-rw-r--r--   0        0        0     1127 2024-04-07 21:52:20.071438 reprompt-0.0.7.6/LICENSE
+-rw-r--r--   0        0        0     7737 2024-04-19 03:54:13.430955 reprompt-0.0.7.6/README.md
+-rw-r--r--   0        0        0      634 2024-04-04 23:08:33.475348 reprompt-0.0.7.6/docs/Makefile
+-rw-r--r--   0        0        0     2321 2024-04-04 23:08:33.475439 reprompt-0.0.7.6/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-04-04 23:08:33.475525 reprompt-0.0.7.6/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-04-04 23:08:33.475604 reprompt-0.0.7.6/docs/developer.md
+-rw-r--r--   0        0        0      468 2024-04-04 23:08:33.475685 reprompt-0.0.7.6/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-04-04 23:08:33.475772 reprompt-0.0.7.6/docs/make.bat
+-rw-r--r--   0        0        0       51 2024-04-04 23:08:33.475852 reprompt-0.0.7.6/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-04-04 23:08:33.475929 reprompt-0.0.7.6/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-04-04 23:08:33.476081 reprompt-0.0.7.6/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-04-04 23:08:33.476163 reprompt-0.0.7.6/docs/pyproject.md
+-rw-r--r--   0        0        0      425 2024-04-04 23:08:33.476254 reprompt-0.0.7.6/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      415 2024-04-04 23:08:33.476339 reprompt-0.0.7.6/docs/python_package.rst
+-rw-r--r--   0        0        0       42 2024-04-04 23:08:33.476409 reprompt-0.0.7.6/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-04-04 23:08:33.476479 reprompt-0.0.7.6/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-04-04 23:08:33.476563 reprompt-0.0.7.6/docs/workflows.md
+-rw-r--r--   0        0        0     6649 2024-04-19 03:54:13.431657 reprompt-0.0.7.6/pyproject.toml
+-rw-r--r--   0        0        0     1241 2024-04-19 05:11:51.041646 reprompt-0.0.7.6/src/reprompt/__init__.py
+-rw-r--r--   0        0        0      859 2024-04-07 23:40:24.407699 reprompt-0.0.7.6/src/reprompt/background_task_manager.py
+-rw-r--r--   0        0        0      167 2024-04-19 03:54:13.432588 reprompt-0.0.7.6/src/reprompt/config.py
+-rw-r--r--   0        0        0     3581 2024-04-19 04:59:40.091869 reprompt-0.0.7.6/src/reprompt/tracing.py
+-rw-r--r--   0        0        0      989 2024-04-04 23:08:33.477233 reprompt-0.0.7.6/tests/conftest.py
+-rw-r--r--   0        0        0      511 2024-04-07 21:52:20.073113 reprompt-0.0.7.6/tests/openai_example_script.py
+-rw-r--r--   0        0        0      283 2024-04-07 21:52:20.073222 reprompt-0.0.7.6/tests/test_init.py
+-rw-r--r--   0        0        0     1673 2024-04-07 21:52:20.073331 reprompt-0.0.7.6/tests/test_openai_tracing.py
+-rw-r--r--   0        0        0     9640 1970-01-01 00:00:00.000000 reprompt-0.0.7.6/PKG-INFO
```

### Comparing `reprompt-0.0.7.5/.devcontainer/devcontainer.json` & `reprompt-0.0.7.6/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.5/.github/workflows/schedule-update-actions.yml` & `reprompt-0.0.7.6/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.5/.gitignore` & `reprompt-0.0.7.6/.gitignore`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.5/.pre-commit-config.yaml` & `reprompt-0.0.7.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.5/.vscode/settings.json` & `reprompt-0.0.7.6/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.5/LICENSE` & `reprompt-0.0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.5/README.md` & `reprompt-0.0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.5/docs/Makefile` & `reprompt-0.0.7.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.5/docs/conf.py` & `reprompt-0.0.7.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.5/docs/make.bat` & `reprompt-0.0.7.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.5/docs/pylint.md` & `reprompt-0.0.7.6/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.5/pyproject.toml` & `reprompt-0.0.7.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.5/src/reprompt/__init__.py` & `reprompt-0.0.7.6/src/reprompt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from . import config
 from .tracing import FunctionTrace, get_edits, write_traces
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 # IMPORTANT: setting version for Reprompt package
-__version__ = "0.0.7.5"
+__version__ = "0.0.7.6"
 # IMPORTANT: All the functions we want to expose publicly from the reprompt module
 __all__ = ["init", "FunctionTrace", "write_traces", "get_edits"]
 
 
 def init(api_base_url: str = None, api_key: str = None, debug: bool = False):
     if debug:
         logger.setLevel(logging.DEBUG)
```

### Comparing `reprompt-0.0.7.5/src/reprompt/background_task_manager.py` & `reprompt-0.0.7.6/src/reprompt/background_task_manager.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.5/src/reprompt/tracing.py` & `reprompt-0.0.7.6/src/reprompt/tracing.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,44 +9,56 @@
 
 from . import config
 from .background_task_manager import BackgroundTaskManager
 
 logger = logging.getLogger(__name__)
 
 
-async def write_traces_task(traces):
-    timestamp = datetime.now().isoformat()
-    data = {"traces": [{"function_calls": traces, "timestamp": timestamp}]}
+# Core business logic for uploading traces
+async def upload_traces(data):
     if config.api_key is None:
         print("API key is required to upload traces")
         return
     try:
         async with aiohttp.ClientSession() as session:
-            logger.debug(f"Uploading traces asynchronously")
+            logger.debug("Uploading traces asynchronously")
             async with session.post(
                 f"{config.api_base_url}/api/tracer/upload_batch",
                 json=data,
                 headers={"Content-Type": "application/json", "apiKey": config.api_key},
             ) as response:
                 if response.status != 200:
                     logger.error(f"Failed to upload batch: {response.status}")
                 else:
                     logger.debug("Batch uploaded successfully")
     except aiohttp.ClientError:
         logger.error("Cannot connect to reprompt to upload traces")
 
 
-def write_traces(traces):
-    loop = asyncio.get_event_loop()
-    if loop.is_running():
-        loop.create_task(write_traces_task([trace.get_trace_info() for trace in traces]))
+# Asynchronous wrapper
+async def write_traces_async(traces):
+    timestamp = datetime.now().isoformat()
+    data = {"traces": [{"function_calls": traces, "timestamp": timestamp}]}
+    await upload_traces(data)
+
+
+# Synchronous wrapper
+async def write_traces_sync(traces):
+    timestamp = datetime.now().isoformat()
+    data = {"traces": [{"function_calls": traces, "timestamp": timestamp}]}
+    await upload_traces(data)
+
+
+# Unified interface to call either sync or async based on need
+async def write_traces(traces, async_mode=False):
+    traces = [trace.get_trace_info() for trace in traces]
+    if async_mode:
+        asyncio.create_task(write_traces_async(traces))
     else:
-        # Handling the case where loop is not running is tricky
-        # It's usually not recommended to try to start the loop yourself in a library function
-        print("Event loop is not running. Can't schedule write_traces_task.")
+        await write_traces_sync(traces)
 
 
 class FunctionTrace:
     def __init__(self, func_name, func_inputs):
         logger.debug(f"Creating trace for function {func_name}")
         self.func_name = func_name
         self.start_time = datetime.now()
```

### Comparing `reprompt-0.0.7.5/tests/conftest.py` & `reprompt-0.0.7.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.5/tests/test_openai_tracing.py` & `reprompt-0.0.7.6/tests/test_openai_tracing.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.7.5/PKG-INFO` & `reprompt-0.0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprompt
-Version: 0.0.7.5
+Version: 0.0.7.6
 Summary: Reprompt
 Author-email: Lukas Martinelli <me@lukasmartinelli.ch>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
```

