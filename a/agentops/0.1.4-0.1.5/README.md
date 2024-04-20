# Comparing `tmp/agentops-0.1.4.tar.gz` & `tmp/agentops-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentops-0.1.4.tar", last modified: Thu Apr 11 19:25:56 2024, max compression
+gzip compressed data, was "agentops-0.1.5.tar", last modified: Sat Apr 20 01:56:18 2024, max compression
```

## Comparing `agentops-0.1.4.tar` & `agentops-0.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:25:56.618158 agentops-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-11 19:25:52.000000 agentops-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-04-11 19:25:56.618158 agentops-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-04-11 19:25:52.000000 agentops-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:25:56.614158 agentops-0.1.4/agentops/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2879 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    12792 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/host_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22227 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/langchain_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12107 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/llm_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/meta_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-11 19:25:52.000000 agentops-0.1.4/agentops/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:25:56.618158 agentops-0.1.4/agentops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-04-11 19:25:56.000000 agentops-0.1.4/agentops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-11 19:25:56.000000 agentops-0.1.4/agentops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:25:56.000000 agentops-0.1.4/agentops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-11 19:25:56.000000 agentops-0.1.4/agentops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 19:25:56.000000 agentops-0.1.4/agentops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-11 19:25:52.000000 agentops-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:25:56.618158 agentops-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:25:56.618158 agentops-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-11 19:25:52.000000 agentops-0.1.4/tests/test_canary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-11 19:25:52.000000 agentops-0.1.4/tests/test_patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-11 19:25:52.000000 agentops-0.1.4/tests/test_record_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-11 19:25:52.000000 agentops-0.1.4/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-11 19:25:52.000000 agentops-0.1.4/tests/test_teardown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:56:18.529813 agentops-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 01:56:14.000000 agentops-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-04-20 01:56:18.529813 agentops-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-04-20 01:56:14.000000 agentops-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:56:18.525813 agentops-0.1.5/agentops/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3267 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13190 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/host_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21947 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/langchain_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11995 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/llm_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/meta_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-20 01:56:14.000000 agentops-0.1.5/agentops/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:56:18.529813 agentops-0.1.5/agentops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-04-20 01:56:18.000000 agentops-0.1.5/agentops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-20 01:56:18.000000 agentops-0.1.5/agentops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:56:18.000000 agentops-0.1.5/agentops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-20 01:56:18.000000 agentops-0.1.5/agentops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 01:56:18.000000 agentops-0.1.5/agentops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-20 01:56:14.000000 agentops-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 01:56:18.529813 agentops-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:56:18.529813 agentops-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-20 01:56:14.000000 agentops-0.1.5/tests/test_canary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-20 01:56:14.000000 agentops-0.1.5/tests/test_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-20 01:56:14.000000 agentops-0.1.5/tests/test_record_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-20 01:56:14.000000 agentops-0.1.5/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-20 01:56:14.000000 agentops-0.1.5/tests/test_teardown.py
```

### Comparing `agentops-0.1.4/LICENSE` & `agentops-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `agentops-0.1.4/PKG-INFO` & `agentops-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentops
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python SDK for developing AI agent evals and observability
 Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
 Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.4 Summary: Python SDK for
+Metadata-Version: 2.1 Name: agentops Version: 0.1.5 Summary: Python SDK for
 developing AI agent evals and observability Author-email: Alex Reibman
 gmail.com>, Shawn Qiu
 gmail.com>, Braelyn Boynton
 gmail.com>, Howard Gil
 gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
```

### Comparing `agentops-0.1.4/README.md` & `agentops-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `agentops-0.1.4/agentops/__init__.py` & `agentops-0.1.5/agentops/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 def init(api_key: Optional[str] = None,
          parent_key: Optional[str] = None,
          endpoint: Optional[str] = None,
          max_wait_time: Optional[int] = None,
          max_queue_size: Optional[int] = None,
          tags: Optional[List[str]] = None,
          override=True,
-         auto_start_session=True):
+         auto_start_session=True,
+         inherited_session_id: Optional[str] = None
+         ):
     """
         Initializes the AgentOps singleton pattern.
 
         Args:
 
             api_key (str, optional): API Key for AgentOps services. If none is provided, key will
                 be read from the AGENTOPS_API_KEY environment variable.
@@ -32,35 +34,40 @@
             max_wait_time (int, optional): The maximum time to wait in milliseconds before flushing the queue.
                 Defaults to 30,000 (30 seconds)
             max_queue_size (int, optional): The maximum size of the event queue. Defaults to 100.
             tags (List[str], optional): Tags for the sessions that can be used for grouping or
                 sorting later (e.g. ["GPT-4"]).
             override (bool): Whether to override and LLM calls to emit as events.
             auto_start_session (bool): Whether to start a session automatically when the client is created.
+            inherited_session_id (optional, str): Init Agentops with an existing Session
         Attributes:
         """
 
-    Client(api_key=api_key,
-           parent_key=parent_key,
-           endpoint=endpoint,
-           max_wait_time=max_wait_time,
-           max_queue_size=max_queue_size,
-           tags=tags,
-           override=override,
-           auto_start_session=auto_start_session)
+    c = Client(api_key=api_key,
+               parent_key=parent_key,
+               endpoint=endpoint,
+               max_wait_time=max_wait_time,
+               max_queue_size=max_queue_size,
+               tags=tags,
+               override=override,
+               auto_start_session=auto_start_session,
+               inherited_session_id=inherited_session_id
+               )
+
+    return inherited_session_id or c.current_session_id
 
 
 def end_session(end_state: str,
                 end_state_reason: Optional[str] = None,
                 video: Optional[str] = None):
     Client().end_session(end_state, end_state_reason, video)
 
 
-def start_session(tags: Optional[List[str]] = None, config: Optional[Configuration] = None):
-    Client().start_session(tags, config)
+def start_session(tags: Optional[List[str]] = None, config: Optional[Configuration] = None, inherited_session_id: Optional[str] = None):
+    return Client().start_session(tags, config, inherited_session_id)
 
 
 def record(event: Event | ErrorEvent):
     Client().record(event)
 
 
 def add_tags(tags: List[str]):
```

### Comparing `agentops-0.1.4/agentops/agent.py` & `agentops-0.1.5/agentops/agent.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.4/agentops/client.py` & `agentops-0.1.5/agentops/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from typing import Optional, List
 import traceback
 import logging
 import inspect
 import atexit
 import signal
 import sys
+import threading
 
 from .meta_client import MetaClient
 from .config import Configuration, ConfigurationError
 from .llm_tracker import LlmTracker
 
 
 @singleton
@@ -41,28 +42,30 @@
         max_wait_time (int, optional): The maximum time to wait in milliseconds before flushing the queue. 
             Defaults to 30,000 (30 seconds)
         max_queue_size (int, optional): The maximum size of the event queue. Defaults to 100.
         tags (List[str], optional): Tags for the sessions that can be used for grouping or 
             sorting later (e.g. ["GPT-4"]).
         override (bool): Whether to override and LLM calls to emit as events.
         auto_start_session (bool): Whether to start a session automatically when the client is created.
+        inherited_session_id (optional, str): Init Agentops with an existing Session
     Attributes:
         _session (Session, optional): A Session is a grouping of events (e.g. a run of your agent).
         _worker (Worker, optional): A Worker manages the event queue and sends session updates to the AgentOps api server
     """
 
     def __init__(self,
                  api_key: Optional[str] = None,
                  parent_key: Optional[str] = None,
                  endpoint: Optional[str] = None,
                  max_wait_time: Optional[int] = None,
                  max_queue_size: Optional[int] = None,
                  tags: Optional[List[str]] = None,
                  override=True,
-                 auto_start_session=True
+                 auto_start_session=True,
+                 inherited_session_id: Optional[str] = None
                  ):
 
         self._session = None
         self._worker = None
         self._tags = tags
 
         try:
@@ -73,15 +76,15 @@
                                         max_queue_size=max_queue_size)
         except ConfigurationError:
             return
 
         self._handle_unclean_exits()
 
         if auto_start_session:
-            self.start_session(tags, self.config)
+            self.start_session(tags, self.config, inherited_session_id)
 
         if override:
             if 'openai' in sys.modules:
                 self.llm_tracker = LlmTracker(self)
                 self.llm_tracker.override_api('openai')
 
     def add_tags(self, tags: List[str]):
@@ -143,16 +146,15 @@
             event.end_timestamp = get_ISO_time()
             # TODO: If func excepts this will never get called
             # the dev loses all the useful stuff in ActionEvent they would need for debugging
             # we should either record earlier or have Error post the supplied event to supabase
             self.record(event)
 
         except Exception as e:
-            # TODO: add the stack trace
-            self.record(ErrorEvent(trigger_event=event, details={f"{type(e).__name__}": str(e)}))
+            self.record(ErrorEvent(trigger_event=event, exception=e))
 
             # Re-raise the exception
             raise
 
         return returns
 
     async def _record_event_async(self, func, event_name, *args, **kwargs):
@@ -183,47 +185,49 @@
             event.end_timestamp = get_ISO_time()
             # TODO: If func excepts this will never get called
             # the dev loses all the useful stuff in ActionEvent they would need for debugging
             # we should either record earlier or have Error post the supplied event to supabase
             self.record(event)
 
         except Exception as e:
-            # TODO: add the stack trace
-            self.record(ErrorEvent(trigger_event=event, details={f"{type(e).__name__}": str(e)}))
+            self.record(ErrorEvent(trigger_event=event, exception=e))
 
             # Re-raise the exception
             raise
 
         return returns
 
-    def start_session(self, tags: Optional[List[str]] = None, config: Optional[Configuration] = None):
+    def start_session(self, tags: Optional[List[str]] = None, config: Optional[Configuration] = None, inherited_session_id: Optional[str] = None):
         """
         Start a new session for recording events.
 
         Args:
             tags (List[str], optional): Tags that can be used for grouping or sorting later.
                 e.g. ["test_run"].
             config: (Configuration, optional): Client configuration object
+            inherited_session_id (optional, str): assign session id to match existing Session
         """
         if self._session is not None:
             return logging.warning("🖇 AgentOps: Cannot start session - session already started")
 
         if not config and not self.config:
             return logging.warning("🖇 AgentOps: Cannot start session - missing configuration")
 
-        self._session = Session(uuid4(), tags or self._tags, host_env=get_host_env())
+        self._session = Session(inherited_session_id or uuid4(), tags or self._tags, host_env=get_host_env())
         self._worker = Worker(config or self.config)
         start_session_result = self._worker.start_session(self._session)
         if not start_session_result:
             self._session = None
             return logging.warning("🖇 AgentOps: Cannot start session")
 
         logging.info('View info on this session at https://app.agentops.ai/drilldown?session_id={}'
                      .format(self._session.session_id))
 
+        return self._session.session_id
+
     def end_session(self,
                     end_state: str,
                     end_state_reason: Optional[str] = None,
                     video: Optional[str] = None):
         """
         End the current session with the AgentOps service.
 
@@ -289,23 +293,25 @@
 
             self.end_session(end_state='Fail',
                              end_state_reason=f"{str(exc_value)}: {formatted_traceback}")
 
             # Then call the default excepthook to exit the program
             sys.__excepthook__(exc_type, exc_value, exc_traceback)
 
-        atexit.register(lambda: cleanup(end_state="Indeterminate",
-                        end_state_reason="Process exited without calling end_session()"))
-        signal.signal(signal.SIGINT, signal_handler)
-        signal.signal(signal.SIGTERM, signal_handler)
-        sys.excepthook = handle_exception
+        # if main thread
+        if isinstance(threading.current_thread(), threading._MainThread):
+            atexit.register(lambda: cleanup(end_state="Indeterminate",
+                            end_state_reason="Process exited without calling end_session()"))
+            signal.signal(signal.SIGINT, signal_handler)
+            signal.signal(signal.SIGTERM, signal_handler)
+            sys.excepthook = handle_exception
 
     @property
     def current_session_id(self):
-        return self._session.session_id
+        return self._session.session_id if self._session else None
 
     @property
     def api_key(self):
         return self.config.api_key
 
     def set_parent_key(self, parent_key):
         if self._worker:
```

### Comparing `agentops-0.1.4/agentops/config.py` & `agentops-0.1.5/agentops/config.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.4/agentops/decorators.py` & `agentops-0.1.5/agentops/decorators.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.4/agentops/enums.py` & `agentops-0.1.5/agentops/enums.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.4/agentops/event.py` & `agentops-0.1.5/agentops/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
 AgentOps events.
 
 Data Class:
     Event: Represents discrete events to be recorded.
 """
 
-from dataclasses import dataclass, field
+from dataclasses import asdict, dataclass, field
 from typing import List, Optional
 from .helpers import get_ISO_time, check_call_stack_for_agent_id
 from .enums import EventType, Models
 from uuid import UUID, uuid4
+import traceback
 
 
 @dataclass
 class Event:
 
     """
     Abstract base class for events that will be recorded. Should not be instantiated directly.
@@ -111,29 +112,34 @@
 @dataclass
 class ErrorEvent():
 
     """
     For recording any errors e.g. ones related to agent execution
 
     trigger_event(Event, optional): The event object that triggered the error if applicable.
+    exception(BaseException, optional): The thrown exception. We will automatically parse the error_type and details from this.
     error_type(str, optional): The type of error e.g. "ValueError".
     code(str, optional): A code that can be used to identify the error e.g. 501.
     details(str, optional): Detailed information about the error.
     logs(str, optional): For detailed information/logging related to the error.
     timestamp(str): A timestamp indicating when the error occurred. Defaults to the time when this ErrorEvent was instantiated.
 
     """
 
-    trigger_event: Optional[Event] = None  # TODO: remove from serialization?
+    trigger_event: Optional[Event] = None
+    exception: Optional[BaseException] = None
     error_type: Optional[str] = None
     code: Optional[str] = None
     details: Optional[str] = None
-    logs: Optional[str] = None
+    logs: Optional[str] = field(default_factory=traceback.format_exc)
     timestamp: str = field(default_factory=get_ISO_time)
 
     def __post_init__(self):
         self.event_type = EventType.ERROR.value
         if self.trigger_event:
             self.trigger_event_id = self.trigger_event.id
             self.trigger_event_type = self.trigger_event.event_type
-            # TODO: remove trigger_event from serialization
-            # e.g. field(repr=False, compare=False, hash=False, metadata={'serialize': False})
+            self.trigger_event = None  # removes trigger_event from serialization
+        if self.exception:
+            self.error_type = self.error_type or type(self.exception).__name__
+            self.details = self.details or str(self.exception)
+            self.exception = None  # removes exception from serialization
```

### Comparing `agentops-0.1.4/agentops/helpers.py` & `agentops-0.1.5/agentops/helpers.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.4/agentops/host_env.py` & `agentops-0.1.5/agentops/host_env.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.4/agentops/http_client.py` & `agentops-0.1.5/agentops/http_client.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.4/agentops/langchain_callback_handler.py` & `agentops-0.1.5/agentops/langchain_callback_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             run_id: UUID,
             parent_run_id: Optional[UUID] = None,
             **kwargs: Any,
     ) -> Any:
         llm_event: LLMEvent = self.events.llm[str(run_id)]
         self.ao_client.record(llm_event)
 
-        error_event = ErrorEvent(trigger_event=llm_event, details=str(error), timestamp=get_ISO_time())
+        error_event = ErrorEvent(trigger_event=llm_event, exception=error)
         self.ao_client.record(error_event)
 
     @debug_print_function_params
     def on_llm_end(
         self,
         response: LLMResult,
         *,
@@ -102,16 +102,15 @@
             llm_event.completion = response.generations[0][0].message.content  # TODO
             llm_event.prompt_tokens = response.llm_output['token_usage']['prompt_tokens']
             llm_event.completion_tokens = response.llm_output['token_usage']['completion_tokens']
         self.ao_client.record(llm_event)
 
         if len(response.generations) == 0:
             # TODO: more descriptive error
-            error_event = ErrorEvent(trigger_event=self.events.llm[str(run_id)],
-                                     details="on_llm_end: No generations", timestamp=get_ISO_time())
+            error_event = ErrorEvent(trigger_event=self.events.llm[str(run_id)], error_type="NoGenerations", details="on_llm_end: No generations")
             self.ao_client.record(error_event)
 
     @debug_print_function_params
     def on_chain_start(
         self,
         serialized: Dict[str, Any],
         inputs: Dict[str, Any],
@@ -152,15 +151,15 @@
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
         **kwargs: Any,
     ) -> Any:
         action_event: ActionEvent = self.events.chain[str(run_id)]
         self.ao_client.record(action_event)
 
-        error_event = ErrorEvent(trigger_event=action_event, details=str(error), timestamp=get_ISO_time())
+        error_event = ErrorEvent(trigger_event=action_event, exception=error)
         self.ao_client.record(error_event)
 
     @debug_print_function_params
     def on_tool_start(
         self,
         serialized: Dict[str, Any],
         input_str: str,
@@ -195,30 +194,30 @@
         tool_event.end_timestamp = get_ISO_time()
         tool_event.returns = output
         self.ao_client.record(tool_event)
 
         # Tools are capable of failing `on_tool_end` quietly.
         # This is a workaround to make sure we can log it as an error.
         if kwargs.get('name') == '_Exception':
-            error_event = ErrorEvent(trigger_event=tool_event, details=output, timestamp=get_ISO_time())
+            error_event = ErrorEvent(trigger_event=tool_event, error_type="LangchainToolException", details=output)
             self.ao_client.record(error_event)
 
     @debug_print_function_params
     def on_tool_error(
             self,
             error: BaseException,
             *,
             run_id: UUID,
             parent_run_id: Optional[UUID] = None,
             **kwargs: Any,
     ) -> Any:
         tool_event: ToolEvent = self.events.tool[str(run_id)]
         self.ao_client.record(tool_event)
 
-        error_event = ErrorEvent(trigger_event=tool_event, details=str(error), timestamp=get_ISO_time())
+        error_event = ErrorEvent(trigger_event=tool_event, exception=error)
         self.ao_client.record(error_event)
 
     @debug_print_function_params
     def on_retriever_start(
             self,
             serialized: Dict[str, Any],
             query: str,
@@ -261,15 +260,15 @@
             parent_run_id: Optional[UUID] = None,
             tags: Optional[List[str]] = None,
             **kwargs: Any,
     ) -> None:
         action_event: ActionEvent = self.events.retriever[str(run_id)]
         self.ao_client.record(action_event)
 
-        error_event = ErrorEvent(trigger_event=action_event, details=str(error), timestamp=get_ISO_time())
+        error_event = ErrorEvent(trigger_event=action_event, exception=error)
         self.ao_client.record(error_event)
 
     @debug_print_function_params
     def on_agent_action(
         self,
         action: AgentAction,
         *,
@@ -401,15 +400,15 @@
             run_id: UUID,
             parent_run_id: Optional[UUID] = None,
             **kwargs: Any,
     ) -> Any:
         llm_event: LLMEvent = self.events.llm[str(run_id)]
         self.ao_client.record(llm_event)
 
-        error_event = ErrorEvent(trigger_event=llm_event, details=str(error), timestamp=get_ISO_time())
+        error_event = ErrorEvent(trigger_event=llm_event, exception=error)
         self.ao_client.record(error_event)
 
     @debug_print_function_params
     async def on_llm_end(
         self,
         response: LLMResult,
         *,
@@ -427,16 +426,15 @@
             llm_event.completion = response.generations[0][0].message.content  # TODO
             llm_event.prompt_tokens = response.llm_output['token_usage']['prompt_tokens']
             llm_event.completion_tokens = response.llm_output['token_usage']['completion_tokens']
         self.ao_client.record(llm_event)
 
         if len(response.generations) == 0:
             # TODO: more descriptive error
-            error_event = ErrorEvent(trigger_event=self.events.llm[str(run_id)],
-                                     details="on_llm_end: No generations", timestamp=get_ISO_time())
+            error_event = ErrorEvent(trigger_event=self.events.llm[str(run_id)], error_type="NoGenerations", details="on_llm_end: No generations")
             self.ao_client.record(error_event)
 
     @debug_print_function_params
     async def on_chain_start(
         self,
         serialized: Dict[str, Any],
         inputs: Dict[str, Any],
@@ -477,15 +475,15 @@
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
         **kwargs: Any,
     ) -> Any:
         action_event: ActionEvent = self.events.chain[str(run_id)]
         self.ao_client.record(action_event)
 
-        error_event = ErrorEvent(trigger_event=action_event, details=str(error), timestamp=get_ISO_time())
+        error_event = ErrorEvent(trigger_event=action_event, exception=error)
         self.ao_client.record(error_event)
 
     @debug_print_function_params
     async def on_tool_start(
         self,
         serialized: Dict[str, Any],
         input_str: str,
@@ -520,30 +518,30 @@
         tool_event.end_timestamp = get_ISO_time()
         tool_event.returns = output
         self.ao_client.record(tool_event)
 
         # Tools are capable of failing `on_tool_end` quietly.
         # This is a workaround to make sure we can log it as an error.
         if kwargs.get('name') == '_Exception':
-            error_event = ErrorEvent(trigger_event=tool_event, details=output, timestamp=get_ISO_time())
+            error_event = ErrorEvent(trigger_event=tool_event, error_type="LangchainToolException", details=output)
             self.ao_client.record(error_event)
 
     @debug_print_function_params
     async def on_tool_error(
             self,
             error: BaseException,
             *,
             run_id: UUID,
             parent_run_id: Optional[UUID] = None,
             **kwargs: Any,
     ) -> Any:
         tool_event: ToolEvent = self.events.tool[str(run_id)]
         self.ao_client.record(tool_event)
 
-        error_event = ErrorEvent(trigger_event=tool_event, details=str(error), timestamp=get_ISO_time())
+        error_event = ErrorEvent(trigger_event=tool_event, exception=error)
         self.ao_client.record(error_event)
 
     @debug_print_function_params
     async def on_retriever_start(
             self,
             serialized: Dict[str, Any],
             query: str,
@@ -586,15 +584,15 @@
             parent_run_id: Optional[UUID] = None,
             tags: Optional[List[str]] = None,
             **kwargs: Any,
     ) -> None:
         action_event: ActionEvent = self.events.retriever[str(run_id)]
         self.ao_client.record(action_event)
 
-        error_event = ErrorEvent(trigger_event=action_event, details=str(error), timestamp=get_ISO_time())
+        error_event = ErrorEvent(trigger_event=action_event, exception=error)
         self.ao_client.record(error_event)
 
     @debug_print_function_params
     async def on_agent_action(
         self,
         action: AgentAction,
         *,
```

### Comparing `agentops-0.1.4/agentops/llm_tracker.py` & `agentops-0.1.5/agentops/llm_tracker.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                     self.llm_event.completion = {"role": "assistant", "content": self.completion}
                     self.llm_event.returns = {"finish_reason": finish_reason, "content": self.completion}
                     self.llm_event.model = model
                     self.llm_event.end_timestamp = get_ISO_time()
 
                     self.client.record(self.llm_event)
             except Exception as e:
-                self.client.record(ErrorEvent(trigger_event=self.llm_event, details={f"{type(e).__name__}": str(e)}))
+                self.client.record(ErrorEvent(trigger_event=self.llm_event, exception=e))
                 # TODO: This error is specific to only one path of failure. Should be more generic or have different logging for different paths
                 logging.warning(
                     f"🖇 AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
 
         # if the response is a generator, decorate the generator
         if inspect.isasyncgen(response):
             async def async_generator():
@@ -93,15 +93,15 @@
             self.llm_event.completion_tokens = response['usage']['completion_tokens']
             self.llm_event.returns = {"content": response['choices'][0]['message']['content']}
             self.llm_event.model = response["model"]
             self.llm_event.end_timestamp = get_ISO_time()
 
             self.client.record(self.llm_event)
         except Exception as e:
-            self.client.record(ErrorEvent(trigger_event=self.llm_event, details={f"{type(e).__name__}": str(e)}))
+            self.client.record(ErrorEvent(trigger_event=self.llm_event, exception=e))
             # TODO: This error is specific to only one path of failure. Should be more generic or have different logging for different paths
             logging.warning(
                 f"🖇 AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
 
         return response
 
     def _handle_response_v1_openai(self, response, kwargs, init_timestamp):
@@ -139,15 +139,15 @@
                     self.llm_event.returns = {"finish_reason": finish_reason, "content": self.completion,
                                               "function_call": function_call, "tool_calls": tool_calls, "role": role}
                     self.llm_event.model = model
                     self.llm_event.end_timestamp = get_ISO_time()
 
                     self.client.record(self.llm_event)
             except Exception as e:
-                self.client.record(ErrorEvent(trigger_event=self.llm_event, details={f"{type(e).__name__}": str(e)}))
+                self.client.record(ErrorEvent(trigger_event=self.llm_event, exception=e))
                 # TODO: This error is specific to only one path of failure. Should be more generic or have different logging for different paths
                 logging.warning(
                     f"🖇 AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
 
         # if the response is a generator, decorate the generator
         if isinstance(response, Stream):
             def generator():
@@ -184,15 +184,15 @@
             self.llm_event.completion = response.choices[0].message.model_dump()
             self.llm_event.completion_tokens = response.usage.completion_tokens
             self.llm_event.returns = response.model_dump()
             self.llm_event.model = response.model
 
             self.client.record(self.llm_event)
         except Exception as e:
-            self.client.record(ErrorEvent(trigger_event=self.llm_event, details={f"{type(e).__name__}": str(e)}))
+            self.client.record(ErrorEvent(trigger_event=self.llm_event, exception=e))
             # TODO: This error is specific to only one path of failure. Should be more generic or have different logging for different paths
             logging.warning(
                 f"🖇 AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
 
         return response
 
     def override_openai_v1_completion(self):
```

### Comparing `agentops-0.1.4/agentops/meta_client.py` & `agentops-0.1.5/agentops/meta_client.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.4/agentops/session.py` & `agentops-0.1.5/agentops/session.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.4/agentops/worker.py` & `agentops-0.1.5/agentops/worker.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.4/agentops.egg-info/PKG-INFO` & `agentops-0.1.5/agentops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentops
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python SDK for developing AI agent evals and observability
 Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
 Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.4 Summary: Python SDK for
+Metadata-Version: 2.1 Name: agentops Version: 0.1.5 Summary: Python SDK for
 developing AI agent evals and observability Author-email: Alex Reibman
 gmail.com>, Shawn Qiu
 gmail.com>, Braelyn Boynton
 gmail.com>, Howard Gil
 gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
```

### Comparing `agentops-0.1.4/agentops.egg-info/SOURCES.txt` & `agentops-0.1.5/agentops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agentops-0.1.4/pyproject.toml` & `agentops-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "agentops"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Alex Reibman", email="areibman@gmail.com" },
   { name="Shawn Qiu", email="siyangqiu@gmail.com" },
   { name="Braelyn Boynton", email="bboynton97@gmail.com" },
   { name="Howard Gil", email="howardbgil@gmail.com" }
 ]
 description = "Python SDK for developing AI agent evals and observability"
```

### Comparing `agentops-0.1.4/tests/test_canary.py` & `agentops-0.1.5/tests/test_canary.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.4/tests/test_patcher.py` & `agentops-0.1.5/tests/test_patcher.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.4/tests/test_record_function.py` & `agentops-0.1.5/tests/test_record_function.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.4/tests/test_session.py` & `agentops-0.1.5/tests/test_session.py`

 * *Files 24% similar despite different names*

```diff
@@ -65,13 +65,36 @@
         assert request_json['events'][0]['event_type'] == self.event_type
 
         # Act
         end_state = 'Success'
         agentops.end_session(end_state)
         time.sleep(0.15)
 
-        # Assert 3 requets, 1 for session init, 1 for event, 1 for end session
+        # Assert 3 requests, 1 for session init, 1 for event, 1 for end session
         assert len(mock_req.request_history) == 3
         assert mock_req.last_request.headers['X-Agentops-Auth'] == self.api_key
         request_json = mock_req.last_request.json()
         assert request_json['session']['end_state'] == end_state
-        assert request_json['session']['tags'] == tags
+        assert request_json['session']['tags'] == tags
+
+    def test_inherit_session_id(self, mock_req):
+        # Arrange
+        inherited_id = '4f72e834-ff26-4802-ba2d-62e7613446f1'
+        agentops.start_session(tags=['test'], config=self.config, inherited_session_id=inherited_id)
+
+        # Act
+        agentops.record(ActionEvent(self.event_type))
+        agentops.record(ActionEvent(self.event_type))
+        time.sleep(0.15)
+
+        # event session_id correct
+        request_json = mock_req.last_request.json()
+        assert request_json['session_id'] == inherited_id
+
+        # Act
+        end_state = 'Success'
+        agentops.end_session(end_state)
+        time.sleep(0.15)
+
+        # Assert session ended with correct id
+        request_json = mock_req.last_request.json()
+        assert request_json['session']['session_id'] == inherited_id
```

### Comparing `agentops-0.1.4/tests/test_teardown.py` & `agentops-0.1.5/tests/test_teardown.py`

 * *Files identical despite different names*

