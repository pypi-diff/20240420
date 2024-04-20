# Comparing `tmp/taskiq-0.9.2.tar.gz` & `tmp/taskiq-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq-0.9.2.tar", max compression
+gzip compressed data, was "taskiq-0.9.3.tar", max compression
```

## Comparing `taskiq-0.9.2.tar` & `taskiq-0.9.3.tar`

### file list

```diff
@@ -1,67 +1,71 @@
--rw-r--r--   0        0        0     1075 2023-10-01 19:02:41.957400 taskiq-0.9.2/LICENSE
--rw-r--r--   0        0        0     1875 2023-10-01 19:02:41.957400 taskiq-0.9.2/README.md
--rw-r--r--   0        0        0     5147 2023-10-01 19:02:41.961400 taskiq-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     2022 2023-10-01 19:02:41.961400 taskiq-0.9.2/taskiq/__init__.py
--rw-r--r--   0        0        0     2147 2023-10-01 19:02:41.961400 taskiq-0.9.2/taskiq/__main__.py
--rw-r--r--   0        0        0      194 2023-10-01 19:02:41.961400 taskiq-0.9.2/taskiq/abc/__init__.py
--rw-r--r--   0        0        0    15673 2023-10-01 19:02:41.961400 taskiq-0.9.2/taskiq/abc/broker.py
--rw-r--r--   0        0        0      342 2023-10-01 19:02:41.961400 taskiq-0.9.2/taskiq/abc/cmd.py
--rw-r--r--   0        0        0      629 2023-10-01 19:02:41.961400 taskiq-0.9.2/taskiq/abc/formatter.py
--rw-r--r--   0        0        0     3562 2023-10-01 19:02:41.961400 taskiq-0.9.2/taskiq/abc/middleware.py
--rw-r--r--   0        0        0     1376 2023-10-01 19:02:41.961400 taskiq-0.9.2/taskiq/abc/result_backend.py
--rw-r--r--   0        0        0     1623 2023-10-01 19:02:41.961400 taskiq-0.9.2/taskiq/abc/schedule_source.py
--rw-r--r--   0        0        0      496 2023-10-01 19:02:41.961400 taskiq-0.9.2/taskiq/acks.py
--rw-r--r--   0        0        0      311 2023-10-01 19:02:41.961400 taskiq-0.9.2/taskiq/api/__init__.py
--rw-r--r--   0        0        0     2953 2023-10-01 19:02:41.961400 taskiq-0.9.2/taskiq/api/receiver.py
--rw-r--r--   0        0        0      652 2023-10-01 19:02:41.961400 taskiq-0.9.2/taskiq/api/scheduler.py
--rw-r--r--   0        0        0       34 2023-10-01 19:02:41.961400 taskiq-0.9.2/taskiq/brokers/__init__.py
--rw-r--r--   0        0        0     4955 2023-10-01 19:02:41.961400 taskiq-0.9.2/taskiq/brokers/inmemory_broker.py
--rw-r--r--   0        0        0     2421 2023-10-01 19:02:41.961400 taskiq-0.9.2/taskiq/brokers/shared_broker.py
--rw-r--r--   0        0        0     2767 2023-10-01 19:02:41.961400 taskiq-0.9.2/taskiq/brokers/zmq_broker.py
--rw-r--r--   0        0        0       31 2023-10-01 19:02:41.961400 taskiq-0.9.2/taskiq/cli/__init__.py
--rw-r--r--   0        0        0      181 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/cli/common_args.py
--rw-r--r--   0        0        0       37 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/cli/scheduler/__init__.py
--rw-r--r--   0        0        0     2346 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/cli/scheduler/args.py
--rw-r--r--   0        0        0      651 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/cli/scheduler/cmd.py
--rw-r--r--   0        0        0     6511 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/cli/scheduler/run.py
--rw-r--r--   0        0        0     2545 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/cli/utils.py
--rw-r--r--   0        0        0     1517 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/cli/watcher.py
--rw-r--r--   0        0        0       43 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/cli/worker/__init__.py
--rw-r--r--   0        0        0     6012 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/cli/worker/args.py
--rw-r--r--   0        0        0      685 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/cli/worker/cmd.py
--rw-r--r--   0        0        0     1742 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/cli/worker/log_collector.py
--rw-r--r--   0        0        0     9081 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/cli/worker/process_manager.py
--rw-r--r--   0        0        0     6477 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/cli/worker/run.py
--rw-r--r--   0        0        0     1567 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/compat.py
--rw-r--r--   0        0        0     1247 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/context.py
--rw-r--r--   0        0        0     2914 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/decor.py
--rw-r--r--   0        0        0      511 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/events.py
--rw-r--r--   0        0        0     1010 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/exceptions.py
--rw-r--r--   0        0        0       25 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/formatters/__init__.py
--rw-r--r--   0        0        0      928 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/formatters/json_formatter.py
--rw-r--r--   0        0        0     1833 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/funcs.py
--rw-r--r--   0        0        0     5497 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/kicker.py
--rw-r--r--   0        0        0      507 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/message.py
--rw-r--r--   0        0        0       26 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/middlewares/__init__.py
--rw-r--r--   0        0        0     4161 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/middlewares/prometheus_middleware.py
--rw-r--r--   0        0        0     2438 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/middlewares/retry_middleware.py
--rw-r--r--   0        0        0        0 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/py.typed
--rw-r--r--   0        0        0      107 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/receiver/__init__.py
--rw-r--r--   0        0        0     2778 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/receiver/params_parser.py
--rw-r--r--   0        0        0    13942 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/receiver/receiver.py
--rw-r--r--   0        0        0      237 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/result/__init__.py
--rw-r--r--   0        0        0     2054 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/result/v1.py
--rw-r--r--   0        0        0     1893 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/result/v2.py
--rw-r--r--   0        0        0       35 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/result_backends/__init__.py
--rw-r--r--   0        0        0     1268 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/result_backends/dummy.py
--rw-r--r--   0        0        0      146 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/schedule_sources/__init__.py
--rw-r--r--   0        0        0     2619 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/schedule_sources/label_based.py
--rw-r--r--   0        0        0      264 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/scheduler/__init__.py
--rw-r--r--   0        0        0     1056 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/scheduler/merge_functions.py
--rw-r--r--   0        0        0     2615 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/scheduler/scheduler.py
--rw-r--r--   0        0        0    11515 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/serialization.py
--rw-r--r--   0        0        0     1149 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/state.py
--rw-r--r--   0        0        0     4135 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/task.py
--rw-r--r--   0        0        0      884 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/utils.py
--rw-r--r--   0        0        0      106 2023-10-01 19:02:41.965400 taskiq-0.9.2/taskiq/warnings.py
--rw-r--r--   0        0        0     3654 1970-01-01 00:00:00.000000 taskiq-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-10-11 08:33:21.141755 taskiq-0.9.3/LICENSE
+-rw-r--r--   0        0        0     4348 2023-10-11 08:33:21.141755 taskiq-0.9.3/README.md
+-rw-r--r--   0        0        0     5174 2023-10-11 08:33:21.149756 taskiq-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2022 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/__init__.py
+-rw-r--r--   0        0        0     2147 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/__main__.py
+-rw-r--r--   0        0        0      194 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/abc/__init__.py
+-rw-r--r--   0        0        0    16175 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/abc/broker.py
+-rw-r--r--   0        0        0      342 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/abc/cmd.py
+-rw-r--r--   0        0        0      629 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/abc/formatter.py
+-rw-r--r--   0        0        0     3562 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/abc/middleware.py
+-rw-r--r--   0        0        0     1376 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/abc/result_backend.py
+-rw-r--r--   0        0        0     1623 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/abc/schedule_source.py
+-rw-r--r--   0        0        0      565 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/abc/serializer.py
+-rw-r--r--   0        0        0      496 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/acks.py
+-rw-r--r--   0        0        0      311 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/api/__init__.py
+-rw-r--r--   0        0        0     2953 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/api/receiver.py
+-rw-r--r--   0        0        0      652 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/api/scheduler.py
+-rw-r--r--   0        0        0       34 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/brokers/__init__.py
+-rw-r--r--   0        0        0     4955 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/brokers/inmemory_broker.py
+-rw-r--r--   0        0        0     2421 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/brokers/shared_broker.py
+-rw-r--r--   0        0        0     2767 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/brokers/zmq_broker.py
+-rw-r--r--   0        0        0       31 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/cli/__init__.py
+-rw-r--r--   0        0        0      181 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/cli/common_args.py
+-rw-r--r--   0        0        0       37 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/cli/scheduler/__init__.py
+-rw-r--r--   0        0        0     2346 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/cli/scheduler/args.py
+-rw-r--r--   0        0        0      651 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/cli/scheduler/cmd.py
+-rw-r--r--   0        0        0     6511 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/cli/scheduler/run.py
+-rw-r--r--   0        0        0     2545 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/cli/utils.py
+-rw-r--r--   0        0        0     1517 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/cli/watcher.py
+-rw-r--r--   0        0        0       43 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/cli/worker/__init__.py
+-rw-r--r--   0        0        0     6012 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/cli/worker/args.py
+-rw-r--r--   0        0        0      685 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/cli/worker/cmd.py
+-rw-r--r--   0        0        0     1742 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/cli/worker/log_collector.py
+-rw-r--r--   0        0        0     9081 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/cli/worker/process_manager.py
+-rw-r--r--   0        0        0     6477 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/cli/worker/run.py
+-rw-r--r--   0        0        0     2060 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/compat.py
+-rw-r--r--   0        0        0     1247 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/context.py
+-rw-r--r--   0        0        0     2914 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/decor.py
+-rw-r--r--   0        0        0      511 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/events.py
+-rw-r--r--   0        0        0     1010 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/exceptions.py
+-rw-r--r--   0        0        0       25 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/formatters/__init__.py
+-rw-r--r--   0        0        0      925 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/formatters/json_formatter.py
+-rw-r--r--   0        0        0     1144 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/formatters/proxy_formatter.py
+-rw-r--r--   0        0        0     1833 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/funcs.py
+-rw-r--r--   0        0        0     5497 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/kicker.py
+-rw-r--r--   0        0        0      507 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/message.py
+-rw-r--r--   0        0        0       26 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/middlewares/__init__.py
+-rw-r--r--   0        0        0     4161 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/middlewares/prometheus_middleware.py
+-rw-r--r--   0        0        0     2438 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/middlewares/retry_middleware.py
+-rw-r--r--   0        0        0        0 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/py.typed
+-rw-r--r--   0        0        0      107 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/receiver/__init__.py
+-rw-r--r--   0        0        0     2778 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/receiver/params_parser.py
+-rw-r--r--   0        0        0    13942 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/receiver/receiver.py
+-rw-r--r--   0        0        0      237 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/result/__init__.py
+-rw-r--r--   0        0        0     2054 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/result/v1.py
+-rw-r--r--   0        0        0     1893 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/result/v2.py
+-rw-r--r--   0        0        0       35 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/result_backends/__init__.py
+-rw-r--r--   0        0        0     1268 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/result_backends/dummy.py
+-rw-r--r--   0        0        0      146 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/schedule_sources/__init__.py
+-rw-r--r--   0        0        0     2619 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/schedule_sources/label_based.py
+-rw-r--r--   0        0        0      264 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/scheduler/__init__.py
+-rw-r--r--   0        0        0     1056 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/scheduler/merge_functions.py
+-rw-r--r--   0        0        0     2615 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/scheduler/scheduler.py
+-rw-r--r--   0        0        0    11515 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/serialization.py
+-rw-r--r--   0        0        0       26 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/serializers/__init__.py
+-rw-r--r--   0        0        0      658 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/serializers/json_serializer.py
+-rw-r--r--   0        0        0     1149 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/state.py
+-rw-r--r--   0        0        0     4135 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/task.py
+-rw-r--r--   0        0        0      884 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/utils.py
+-rw-r--r--   0        0        0      106 2023-10-11 08:33:21.149756 taskiq-0.9.3/taskiq/warnings.py
+-rw-r--r--   0        0        0     6127 1970-01-01 00:00:00.000000 taskiq-0.9.3/PKG-INFO
```

### Comparing `taskiq-0.9.2/LICENSE` & `taskiq-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/pyproject.toml` & `taskiq-0.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq"
-version = "0.9.2"
+version = "0.9.3"
 description = "Distributed task queue with full async support"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 maintainers = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 repository = "https://github.com/taskiq-python/taskiq"
 homepage = "https://taskiq-python.github.io/"
 documentation = "https://taskiq-python.github.io/"
@@ -57,14 +57,15 @@
 pytest-xdist = { version = "^2.5.0", extras = ["psutil"] }
 types-mock = "^4.0.15"
 tox = "^4.6.4"
 freezegun = "^1.2.2"
 pytest-mock = "^3.11.1"
 tzlocal = "^5.0.1"
 types-tzlocal = "^5.0.1.1"
+types-pytz = "^2023.3.1.1"
 
 [tool.poetry.extras]
 zmq = ["pyzmq"]
 uv = ["uvloop"]
 metrics = ["prometheus_client"]
 reload = ["watchdog", "gitignore-parser"]
```

### Comparing `taskiq-0.9.2/taskiq/__init__.py` & `taskiq-0.9.3/taskiq/__init__.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/__main__.py` & `taskiq-0.9.3/taskiq/__main__.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/abc/broker.py` & `taskiq-0.9.3/taskiq/abc/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,22 @@
     overload,
 )
 from uuid import uuid4
 
 from typing_extensions import ParamSpec, Self, TypeAlias
 
 from taskiq.abc.middleware import TaskiqMiddleware
+from taskiq.abc.serializer import TaskiqSerializer
 from taskiq.acks import AckableMessage
 from taskiq.decor import AsyncTaskiqDecoratedTask
 from taskiq.events import TaskiqEvents
-from taskiq.formatters.json_formatter import JSONFormatter
+from taskiq.formatters.proxy_formatter import ProxyFormatter
 from taskiq.message import BrokerMessage
 from taskiq.result_backends.dummy import DummyResultBackend
+from taskiq.serializers.json_serializer import JSONSerializer
 from taskiq.state import TaskiqState
 from taskiq.utils import maybe_awaitable, remove_suffix
 from taskiq.warnings import TaskiqDeprecationWarning
 
 if TYPE_CHECKING:  # pragma: no cover
     from taskiq.abc.formatter import TaskiqFormatter
     from taskiq.abc.result_backend import AsyncResultBackend
@@ -93,15 +95,16 @@
                 "Please use `with_id_generator` instead.",
                 TaskiqDeprecationWarning,
                 stacklevel=2,
             )
         self.middlewares: "List[TaskiqMiddleware]" = []
         self.result_backend = result_backend
         self.decorator_class = AsyncTaskiqDecoratedTask
-        self.formatter: "TaskiqFormatter" = JSONFormatter()
+        self.serializer: TaskiqSerializer = JSONSerializer()
+        self.formatter: "TaskiqFormatter" = ProxyFormatter(self)
         self.id_generator = task_id_generator
         self.local_task_registry: Dict[str, AsyncTaskiqDecoratedTask[Any, Any]] = {}
         # Every event has a list of handlers.
         # Every handler is a function which takes state as a first argument.
         # And handler can be either sync or async.
         self.event_handlers: DefaultDict[
             TaskiqEvents,
@@ -475,14 +478,27 @@
         :param event: event to handle.
         :param handlers: event handlers.
         :return: self
         """
         self.event_handlers[event].extend(handlers)
         return self
 
+    def with_serializer(
+        self,
+        serializer: TaskiqSerializer,
+    ) -> "Self":  # pragma: no cover
+        """
+        Set a new serializer and return an updated broker.
+
+        :param serializer: new serializer.
+        :return: self
+        """
+        self.serializer = serializer
+        return self
+
     def _register_task(
         self,
         task_name: str,
         task: AsyncTaskiqDecoratedTask[Any, Any],
     ) -> None:
         """
         Mehtod is used to register tasks.
```

### Comparing `taskiq-0.9.2/taskiq/abc/formatter.py` & `taskiq-0.9.3/taskiq/abc/formatter.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/abc/middleware.py` & `taskiq-0.9.3/taskiq/abc/middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/abc/result_backend.py` & `taskiq-0.9.3/taskiq/abc/result_backend.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/abc/schedule_source.py` & `taskiq-0.9.3/taskiq/abc/schedule_source.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/api/receiver.py` & `taskiq-0.9.3/taskiq/api/receiver.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/api/scheduler.py` & `taskiq-0.9.3/taskiq/api/scheduler.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/brokers/inmemory_broker.py` & `taskiq-0.9.3/taskiq/brokers/inmemory_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/brokers/shared_broker.py` & `taskiq-0.9.3/taskiq/brokers/shared_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/brokers/zmq_broker.py` & `taskiq-0.9.3/taskiq/brokers/zmq_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/cli/scheduler/args.py` & `taskiq-0.9.3/taskiq/cli/scheduler/args.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/cli/scheduler/cmd.py` & `taskiq-0.9.3/taskiq/cli/scheduler/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/cli/scheduler/run.py` & `taskiq-0.9.3/taskiq/cli/scheduler/run.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/cli/utils.py` & `taskiq-0.9.3/taskiq/cli/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/cli/watcher.py` & `taskiq-0.9.3/taskiq/cli/watcher.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/cli/worker/args.py` & `taskiq-0.9.3/taskiq/cli/worker/args.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/cli/worker/cmd.py` & `taskiq-0.9.3/taskiq/cli/worker/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/cli/worker/log_collector.py` & `taskiq-0.9.3/taskiq/cli/worker/log_collector.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/cli/worker/process_manager.py` & `taskiq-0.9.3/taskiq/cli/worker/process_manager.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/cli/worker/run.py` & `taskiq-0.9.3/taskiq/cli/worker/run.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/context.py` & `taskiq-0.9.3/taskiq/context.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/decor.py` & `taskiq-0.9.3/taskiq/decor.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/exceptions.py` & `taskiq-0.9.3/taskiq/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/formatters/json_formatter.py` & `taskiq-0.9.3/taskiq/formatters/json_formatter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from taskiq.abc.formatter import TaskiqFormatter
 from taskiq.compat import model_dump_json, model_validate_json
 from taskiq.message import BrokerMessage, TaskiqMessage
 
 
 class JSONFormatter(TaskiqFormatter):
-    """Default taskiq formatter."""
+    """JSON taskiq formatter."""
 
     def dumps(self, message: TaskiqMessage) -> BrokerMessage:
         """
         Dumps taskiq message to some broker message format.
 
         :param message: message to send.
         :return: Dumped message.
```

### Comparing `taskiq-0.9.2/taskiq/funcs.py` & `taskiq-0.9.3/taskiq/funcs.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/kicker.py` & `taskiq-0.9.3/taskiq/kicker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/middlewares/prometheus_middleware.py` & `taskiq-0.9.3/taskiq/middlewares/prometheus_middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/middlewares/retry_middleware.py` & `taskiq-0.9.3/taskiq/middlewares/retry_middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/receiver/params_parser.py` & `taskiq-0.9.3/taskiq/receiver/params_parser.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/receiver/receiver.py` & `taskiq-0.9.3/taskiq/receiver/receiver.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/result/v1.py` & `taskiq-0.9.3/taskiq/result/v1.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/result/v2.py` & `taskiq-0.9.3/taskiq/result/v2.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/result_backends/dummy.py` & `taskiq-0.9.3/taskiq/result_backends/dummy.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/schedule_sources/label_based.py` & `taskiq-0.9.3/taskiq/schedule_sources/label_based.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/scheduler/merge_functions.py` & `taskiq-0.9.3/taskiq/scheduler/merge_functions.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/scheduler/scheduler.py` & `taskiq-0.9.3/taskiq/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/serialization.py` & `taskiq-0.9.3/taskiq/serialization.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/state.py` & `taskiq-0.9.3/taskiq/state.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/task.py` & `taskiq-0.9.3/taskiq/task.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.9.2/taskiq/utils.py` & `taskiq-0.9.3/taskiq/utils.py`

 * *Files identical despite different names*

