# Comparing `tmp/opentelemetry_instrumentation_faststream-0.1.0.tar.gz` & `tmp/opentelemetry_instrumentation_faststream-0.1.1.tar.gz`

## Comparing `opentelemetry_instrumentation_faststream-0.1.0.tar` & `opentelemetry_instrumentation_faststream-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/src/opentelemetry/instrumentation/faststream/__about__.py
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/src/opentelemetry/instrumentation/faststream/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/src/opentelemetry/instrumentation/faststream/annotations.py
--rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/src/opentelemetry/instrumentation/faststream/middlewares.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/src/opentelemetry/instrumentation/faststream/package.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/src/opentelemetry/instrumentation/faststream/version.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/.gitignore
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/README.md
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.1/src/opentelemetry/instrumentation/faststream/__about__.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.1/src/opentelemetry/instrumentation/faststream/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.1/src/opentelemetry/instrumentation/faststream/annotations.py
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.1/src/opentelemetry/instrumentation/faststream/middlewares.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.1/src/opentelemetry/instrumentation/faststream/package.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.1/src/opentelemetry/instrumentation/faststream/version.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.1/README.md
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_faststream-0.1.1/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_faststream-0.1.0/src/opentelemetry/instrumentation/faststream/__init__.py` & `opentelemetry_instrumentation_faststream-0.1.1/src/opentelemetry/instrumentation/faststream/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_faststream-0.1.0/src/opentelemetry/instrumentation/faststream/middlewares.py` & `opentelemetry_instrumentation_faststream-0.1.1/src/opentelemetry/instrumentation/faststream/middlewares.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,16 +54,18 @@
         msg: StreamMessage[Any],
     ) -> Any:
         span_context = propagate.extract(msg.headers)
         attrs = self._attributes_from_message(msg)
         start = default_timer()
         active_requests_counter.add(1, attrs)
         try:
+            # TODO: Name should be the name of the handler function
+            # But it is not trivial as call_next is a wrapper/or partial function
             with tracer.start_as_current_span(
-                name=call_next.__self__._wrapped_call.__name__, context=span_context
+                name=call_next.__name__, context=span_context
             ) as current_span:
                 current_span.set_attributes(attrs)
                 faststream_context.set_local("span", current_span)
                 return await call_next(msg)
         finally:
             duration = max(round((default_timer() - start) * 1000), 0)
             duration_histogram.record(duration, attrs)
```

### Comparing `opentelemetry_instrumentation_faststream-0.1.0/.gitignore` & `opentelemetry_instrumentation_faststream-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_faststream-0.1.0/LICENSE.txt` & `opentelemetry_instrumentation_faststream-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_faststream-0.1.0/README.md` & `opentelemetry_instrumentation_faststream-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_faststream-0.1.0/pyproject.toml` & `opentelemetry_instrumentation_faststream-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_faststream-0.1.0/PKG-INFO` & `opentelemetry_instrumentation_faststream-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: opentelemetry-instrumentation-faststream
-Version: 0.1.0
+Version: 0.1.1
 Summary: FastStream instrumentation for OpenTelemetry
 Project-URL: Documentation, https://github.com/ashambalev/opentelemetry-instrumentation-faststream#readme
 Project-URL: Issues, https://github.com/ashambalev/opentelemetry-instrumentation-faststream/issues
 Project-URL: Source, https://github.com/ashambalev/opentelemetry-instrumentation-faststream
 Author-email: Artem Shambalev <a.shambalev@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

