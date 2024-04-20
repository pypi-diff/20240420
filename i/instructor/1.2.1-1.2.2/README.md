# Comparing `tmp/instructor-1.2.1.tar.gz` & `tmp/instructor-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructor-1.2.1.tar", max compression
+gzip compressed data, was "instructor-1.2.2.tar", max compression
```

## Comparing `instructor-1.2.1.tar` & `instructor-1.2.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1066 2024-04-18 00:19:56.934164 instructor-1.2.1/LICENSE
--rw-r--r--   0        0        0     9715 2024-04-18 00:19:56.934164 instructor-1.2.1/README.md
--rw-r--r--   0        0        0     1312 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/_types/__init__.py
--rw-r--r--   0        0        0      654 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/_types/_alias.py
--rw-r--r--   0        0        0        0 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/cli/__init__.py
--rw-r--r--   0        0        0      807 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/cli/cli.py
--rw-r--r--   0        0        0     3792 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/cli/files.py
--rw-r--r--   0        0        0     5348 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/cli/hub.py
--rw-r--r--   0        0        0     8255 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/cli/jobs.py
--rw-r--r--   0        0        0     6494 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/cli/usage.py
--rw-r--r--   0        0        0     9662 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/client.py
--rw-r--r--   0        0        0     2445 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/client_anthropic.py
--rw-r--r--   0        0        0     2340 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/client_cohere.py
--rw-r--r--   0        0        0     1371 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/client_groq.py
--rw-r--r--   0        0        0     8968 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/distil.py
--rw-r--r--   0        0        0      424 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/dsl/__init__.py
--rw-r--r--   0        0        0     2985 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/dsl/citation.py
--rw-r--r--   0        0        0     7929 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/dsl/iterable.py
--rw-r--r--   0        0        0     2165 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/dsl/maybe.py
--rw-r--r--   0        0        0     2580 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/dsl/parallel.py
--rw-r--r--   0        0        0    11052 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/dsl/partial.py
--rw-r--r--   0        0        0     1733 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/dsl/simple_type.py
--rw-r--r--   0        0        0     4381 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/dsl/validators.py
--rw-r--r--   0        0        0      346 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/exceptions.py
--rw-r--r--   0        0        0     7878 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/function_calls.py
--rw-r--r--   0        0        0      852 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/mode.py
--rw-r--r--   0        0        0     4845 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/patch.py
--rw-r--r--   0        0        0    13509 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/process_response.py
--rw-r--r--   0        0        0        1 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/py.typed
--rw-r--r--   0        0        0     7595 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/retry.py
--rw-r--r--   0        0        0     4767 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/utils.py
--rw-r--r--   0        0        0     2252 2024-04-18 00:19:57.002164 instructor-1.2.1/pyproject.toml
--rw-r--r--   0        0        0    11542 1970-01-01 00:00:00.000000 instructor-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-20 01:01:31.282748 instructor-1.2.2/LICENSE
+-rw-r--r--   0        0        0     9715 2024-04-20 01:01:31.282748 instructor-1.2.2/README.md
+-rw-r--r--   0        0        0     1445 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/_types/__init__.py
+-rw-r--r--   0        0        0      654 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/_types/_alias.py
+-rw-r--r--   0        0        0        0 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/cli/__init__.py
+-rw-r--r--   0        0        0      807 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/cli/cli.py
+-rw-r--r--   0        0        0     3792 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/cli/files.py
+-rw-r--r--   0        0        0     5348 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/cli/hub.py
+-rw-r--r--   0        0        0     8255 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/cli/jobs.py
+-rw-r--r--   0        0        0     6476 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/cli/usage.py
+-rw-r--r--   0        0        0     9666 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/client.py
+-rw-r--r--   0        0        0     2453 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/client_anthropic.py
+-rw-r--r--   0        0        0     2348 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/client_cohere.py
+-rw-r--r--   0        0        0     1379 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/client_groq.py
+-rw-r--r--   0        0        0     1709 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/client_mistral.py
+-rw-r--r--   0        0        0     8968 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/distil.py
+-rw-r--r--   0        0        0      424 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/dsl/__init__.py
+-rw-r--r--   0        0        0     2985 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/dsl/citation.py
+-rw-r--r--   0        0        0     7929 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/dsl/iterable.py
+-rw-r--r--   0        0        0     2165 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/dsl/maybe.py
+-rw-r--r--   0        0        0     2580 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/dsl/parallel.py
+-rw-r--r--   0        0        0    11052 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/dsl/partial.py
+-rw-r--r--   0        0        0     1733 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/dsl/simple_type.py
+-rw-r--r--   0        0        0     4381 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/dsl/validators.py
+-rw-r--r--   0        0        0      346 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/exceptions.py
+-rw-r--r--   0        0        0     7878 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/function_calls.py
+-rw-r--r--   0        0        0      852 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/mode.py
+-rw-r--r--   0        0        0     4877 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/patch.py
+-rw-r--r--   0        0        0    13509 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/process_response.py
+-rw-r--r--   0        0        0        1 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/py.typed
+-rw-r--r--   0        0        0     8898 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/retry.py
+-rw-r--r--   0        0        0     4860 2024-04-20 01:01:31.350749 instructor-1.2.2/instructor/utils.py
+-rw-r--r--   0        0        0     2364 2024-04-20 01:01:31.350749 instructor-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0    11657 1970-01-01 00:00:00.000000 instructor-1.2.2/PKG-INFO
```

### Comparing `instructor-1.2.1/LICENSE` & `instructor-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `instructor-1.2.1/README.md` & `instructor-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `instructor-1.2.1/instructor/__init__.py` & `instructor-1.2.2/instructor/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,11 +53,16 @@
     __all__ += ["from_anthropic"]
 
 if importlib.util.find_spec("groq") is not None:
     from .client_groq import from_groq
 
     __all__ += ["from_groq"]
 
+if importlib.util.find_spec("mistralai") is not None:
+    from .client_mistral import from_mistral
+
+    __all__ += ["from_mistral"]
+
 if importlib.util.find_spec("cohere") is not None:
     from .client_cohere import from_cohere
 
     __all__ += ["from_cohere"]
```

### Comparing `instructor-1.2.1/instructor/_types/_alias.py` & `instructor-1.2.2/instructor/_types/_alias.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.1/instructor/cli/cli.py` & `instructor-1.2.2/instructor/cli/cli.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.1/instructor/cli/files.py` & `instructor-1.2.2/instructor/cli/files.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.1/instructor/cli/hub.py` & `instructor-1.2.2/instructor/cli/hub.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.1/instructor/cli/jobs.py` & `instructor-1.2.2/instructor/cli/jobs.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.1/instructor/cli/usage.py` & `instructor-1.2.2/instructor/cli/usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,19 +110,19 @@
     prompt_cost = cost["prompt"] * n_context_tokens
     completion_cost = cost["completion"] * n_generated_tokens
     return prompt_cost + completion_cost
 
 
 def group_and_sum_by_date_and_snapshot(usage_data: List[Dict[str, Any]]) -> Table:
     """Group and sum the usage data by date and snapshot, including costs."""
-    summary: DefaultDict[str, DefaultDict[str, Dict[str, Union[int, float]]]] = (
-        defaultdict(
-            lambda: defaultdict(
-                lambda: {"total_requests": 0, "total_tokens": 0, "total_cost": 0.0}
-            )
+    summary: DefaultDict[
+        str, DefaultDict[str, Dict[str, Union[int, float]]]
+    ] = defaultdict(
+        lambda: defaultdict(
+            lambda: {"total_requests": 0, "total_tokens": 0, "total_cost": 0.0}
         )
     )
 
     for usage in usage_data:
         snapshot_id = usage["snapshot_id"]
         date = datetime.fromtimestamp(usage["aggregation_timestamp"]).strftime(
             "%Y-%m-%d"
```

### Comparing `instructor-1.2.1/instructor/client.py` & `instructor-1.2.2/instructor/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,16 @@
 
 
 @overload
 def from_litellm(
     completion: Callable,
     mode: instructor.Mode = instructor.Mode.TOOLS,
     **kwargs,
-) -> Instructor: ...
+) -> Instructor:
+    ...
 
 
 @overload
 def from_litellm(
     completion: Awaitable,
     mode: instructor.Mode = instructor.Mode.TOOLS,
     **kwargs,
```

### Comparing `instructor-1.2.1/instructor/client_anthropic.py` & `instructor-1.2.2/instructor/client_anthropic.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 @overload
 def from_anthropic(
     client: anthropic.Anthropic
     | anthropic.AnthropicBedrock
     | anthropic.AnthropicVertex,
     mode: instructor.Mode = instructor.Mode.ANTHROPIC_JSON,
     **kwargs,
-) -> instructor.Instructor: ...
+) -> instructor.Instructor:
+    ...
 
 
 @overload
 def from_anthropic(
     client: anthropic.AsyncAnthropic
     | anthropic.AsyncAnthropicBedrock
     | anthropic.AsyncAnthropicVertex,
     mode: instructor.Mode = instructor.Mode.ANTHROPIC_JSON,
     **kwargs,
-) -> instructor.Instructor: ...
+) -> instructor.Instructor:
+    ...
 
 
 def from_anthropic(
     client: (
         anthropic.Anthropic
         | anthropic.AsyncAnthropic
         | anthropic.AnthropicBedrock
```

### Comparing `instructor-1.2.1/instructor/client_cohere.py` & `instructor-1.2.2/instructor/client_cohere.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,23 +19,25 @@
 
 
 @overload
 def from_cohere(
     client: cohere.Client,
     mode: instructor.Mode = instructor.Mode.COHERE_TOOLS,
     **kwargs,
-) -> instructor.Instructor: ...
+) -> instructor.Instructor:
+    ...
 
 
 @overload
 def from_cohere(
     client: cohere.AsyncClient,
     mode: instructor.Mode = instructor.Mode.COHERE_TOOLS,
     **kwargs,
-) -> instructor.AsyncInstructor: ...
+) -> instructor.AsyncInstructor:
+    ...
 
 
 def from_cohere(
     client: cohere.Client | cohere.AsyncClient,
     mode: instructor.Mode = instructor.Mode.COHERE_TOOLS,
     **kwargs,
 ):
```

### Comparing `instructor-1.2.1/instructor/client_groq.py` & `instructor-1.2.2/instructor/client_groq.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 
 
 @overload
 def from_groq(
     client: groq.Groq,
     mode: instructor.Mode = instructor.Mode.TOOLS,
     **kwargs,
-) -> instructor.Instructor: ...
+) -> instructor.Instructor:
+    ...
 
 
 @overload
 def from_groq(
     client: groq.AsyncGroq,
     mode: instructor.Mode = instructor.Mode.TOOLS,
     **kwargs,
-) -> instructor.Instructor: ...
+) -> instructor.Instructor:
+    ...
 
 
 def from_groq(
     client: groq.Groq | groq.AsyncGroq,
     mode: instructor.Mode = instructor.Mode.TOOLS,
     **kwargs,
 ) -> instructor.Instructor:
```

### Comparing `instructor-1.2.1/instructor/distil.py` & `instructor-1.2.2/instructor/distil.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.1/instructor/dsl/citation.py` & `instructor-1.2.2/instructor/dsl/citation.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.1/instructor/dsl/iterable.py` & `instructor-1.2.2/instructor/dsl/iterable.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.1/instructor/dsl/maybe.py` & `instructor-1.2.2/instructor/dsl/maybe.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.1/instructor/dsl/parallel.py` & `instructor-1.2.2/instructor/dsl/parallel.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.1/instructor/dsl/partial.py` & `instructor-1.2.2/instructor/dsl/partial.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.1/instructor/dsl/simple_type.py` & `instructor-1.2.2/instructor/dsl/simple_type.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.1/instructor/dsl/validators.py` & `instructor-1.2.2/instructor/dsl/validators.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.1/instructor/function_calls.py` & `instructor-1.2.2/instructor/function_calls.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.1/instructor/mode.py` & `instructor-1.2.2/instructor/mode.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.1/instructor/patch.py` & `instructor-1.2.2/instructor/patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,54 +32,60 @@
     def __call__(
         self,
         response_model: Type[T_Model] = None,
         validation_context: dict = None,
         max_retries: int = 1,
         *args: T_ParamSpec.args,
         **kwargs: T_ParamSpec.kwargs,
-    ) -> T_Model: ...
+    ) -> T_Model:
+        ...
 
 
 class AsyncInstructorChatCompletionCreate(Protocol):
     async def __call__(
         self,
         response_model: Type[T_Model] = None,
         validation_context: dict = None,
         max_retries: int = 1,
         *args: T_ParamSpec.args,
         **kwargs: T_ParamSpec.kwargs,
-    ) -> T_Model: ...
+    ) -> T_Model:
+        ...
 
 
 @overload
 def patch(
     client: OpenAI,
     mode: Mode = Mode.TOOLS,
-) -> OpenAI: ...
+) -> OpenAI:
+    ...
 
 
 @overload
 def patch(
     client: AsyncOpenAI,
     mode: Mode = Mode.TOOLS,
-) -> AsyncOpenAI: ...
+) -> AsyncOpenAI:
+    ...
 
 
 @overload
 def patch(
     create: Callable[T_ParamSpec, T_Retval],
     mode: Mode = Mode.TOOLS,
-) -> InstructorChatCompletionCreate: ...
+) -> InstructorChatCompletionCreate:
+    ...
 
 
 @overload
 def patch(
     create: Awaitable[T_Retval],
     mode: Mode = Mode.TOOLS,
-) -> InstructorChatCompletionCreate: ...
+) -> InstructorChatCompletionCreate:
+    ...
 
 
 def patch(
     client: Union[OpenAI, AsyncOpenAI] = None,
     create: Callable[T_ParamSpec, T_Retval] = None,
     mode: Mode = Mode.TOOLS,
 ) -> Union[OpenAI, AsyncOpenAI]:
```

### Comparing `instructor-1.2.1/instructor/process_response.py` & `instructor-1.2.2/instructor/process_response.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.1/instructor/retry.py` & `instructor-1.2.2/instructor/retry.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,14 +26,31 @@
 
 T_Model = TypeVar("T_Model", bound=BaseModel)
 T_Retval = TypeVar("T_Retval")
 T_ParamSpec = ParamSpec("T_ParamSpec")
 T = TypeVar("T")
 
 
+class InstructorRetryException(Exception):
+    def __init__(
+        self,
+        *args,
+        last_completion,
+        messages: list,
+        n_attempts: int,
+        total_usage,
+        **kwargs,
+    ):
+        self.last_completion = last_completion
+        self.messages = messages
+        self.n_attempts = n_attempts
+        self.total_usage = total_usage
+        super().__init__(*args, **kwargs)
+
+
 def reask_messages(response: ChatCompletion, mode: Mode, exception: Exception):
     if mode == Mode.ANTHROPIC_TOOLS:
         # The original response
         assistant_content = []
         tool_use_id = None
         for content in response.content:
             assistant_content.append(content.model_dump())
@@ -140,32 +157,42 @@
                 except (ValidationError, JSONDecodeError) as e:
                     logger.debug(f"Error response: {response}")
                     kwargs["messages"].extend(reask_messages(response, mode, e))
                     if mode in {Mode.ANTHROPIC_TOOLS, Mode.ANTHROPIC_JSON}:
                         kwargs["messages"] = merge_consecutive_messages(
                             kwargs["messages"]
                         )
-                    raise e
+                    raise InstructorRetryException(
+                        e,
+                        last_completion=response,
+                        n_attempts=attempt.retry_state.attempt_number,
+                        messages=kwargs["messages"],
+                        total_usage=total_usage,
+                    ) from e
     except RetryError as e:
-        logger.exception(f"Failed after retries: {e.last_attempt.exception}")
-        raise e.last_attempt.exception from e
+        raise InstructorRetryException(
+            e,
+            last_completion=response,
+            n_attempts=attempt.retry_state.attempt_number,
+            messages=kwargs["messages"],
+            total_usage=total_usage,
+        ) from e
 
 
 async def retry_async(
     func: Callable[T_ParamSpec, T_Retval],
     response_model: Type[T],
     validation_context,
     args,
     kwargs,
     max_retries: int | AsyncRetrying = 1,
     strict: Optional[bool] = None,
     mode: Mode = Mode.TOOLS,
 ) -> T:
     total_usage = CompletionUsage(completion_tokens=0, prompt_tokens=0, total_tokens=0)
-
     # If max_retries is int, then create a AsyncRetrying object
     if isinstance(max_retries, int):
         logger.debug(f"max_retries: {max_retries}")
         max_retries = AsyncRetrying(
             stop=stop_after_attempt(max_retries),
             reraise=True,
         )
@@ -193,11 +220,23 @@
                 except (ValidationError, JSONDecodeError) as e:
                     logger.debug(f"Error response: {response}", e)
                     kwargs["messages"].extend(reask_messages(response, mode, e))
                     if mode in {Mode.ANTHROPIC_TOOLS, Mode.ANTHROPIC_JSON}:
                         kwargs["messages"] = merge_consecutive_messages(
                             kwargs["messages"]
                         )
-                    raise e
+                    raise InstructorRetryException(
+                        e,
+                        last_completion=response,
+                        n_attempts=e.attempt_number,
+                        messages=kwargs["messages"],
+                        total_usage=total_usage,
+                    ) from e
     except RetryError as e:
         logger.exception(f"Failed after retries: {e.last_attempt.exception}")
-        raise e.last_attempt.exception from e
+        raise InstructorRetryException(
+            e,
+            last_completion=response,
+            n_attempts=e.attempt_number,
+            messages=kwargs["messages"],
+            total_usage=total_usage,
+        ) from e
```

### Comparing `instructor-1.2.1/instructor/utils.py` & `instructor-1.2.2/instructor/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 class Provider(Enum):
     OPENAI = "openai"
     ANTHROPIC = "anthropic"
     ANYSCALE = "anyscale"
     TOGETHER = "together"
     GROQ = "groq"
+    MISTRAL = "mistral"
     COHERE = "cohere"
     UNKNOWN = "unknown"
 
 
 def get_provider(base_url: str) -> Provider:
     if "anyscale" in str(base_url):
         return Provider.ANYSCALE
@@ -34,14 +35,16 @@
         return Provider.TOGETHER
     elif "anthropic" in str(base_url):
         return Provider.ANTHROPIC
     elif "groq" in str(base_url):
         return Provider.GROQ
     elif "openai" in str(base_url):
         return Provider.OPENAI
+    elif "mistral" in str(base_url):
+        return Provider.MISTRAL
     elif "cohere" in str(base_url):
         return Provider.COHERE
     return Provider.UNKNOWN
 
 
 def extract_json_from_codeblock(content: str) -> str:
     first_paren = content.find("{")
```

### Comparing `instructor-1.2.1/pyproject.toml` & `instructor-1.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "instructor"
-version = "1.2.1"
+version = "1.2.2"
 description = "structured outputs for llm"
 authors = ["Jason Liu <jason@jxnl.co>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "instructor"}]
 repository = "https://github.com/jxnl/instructor"
 
@@ -27,20 +27,22 @@
 tabulate = { version = "^0.9.0", optional = true }
 pydantic_extra_types = { version = "^2.6.0", optional = true }
 litellm = { version = "^1.0.0", optional = true }
 anthropic = { version = "^0.23.1", optional = true }
 xmltodict = { version = "^0.13.0", optional = true }
 groq = { version = "^0.4.2", optional = true }
 cohere = { version = "^5.1.8", optional = true }
+mistralai = { version = "^0.1.8", optional = true }
 
 [tool.poetry.extras]
 anthropic = ["anthropic", "xmltodict"]
 groq = ["groq"]
 cohere = ["cohere"]
-test-docs = ["fastapi", "redis", "diskcache", "pandas", "tabulate", "pydantic_extra_types", "litellm", "anthropic", "groq", "cohere"]
+test-docs = ["fastapi", "redis", "diskcache", "pandas", "tabulate", "pydantic_extra_types", "litellm", "anthropic", "groq", "cohere", "mistralai"]
+mistralai = ["mistralai"]
 
 [tool.poetry.scripts]
 instructor = "instructor.cli.cli:app"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-asyncio = "^0.21.1"
@@ -70,11 +72,12 @@
 pydantic_extra_types = "^2.6.0"
 litellm = "^1.0.0"
 anthropic = "^0.23.1"
 xmltodict = "^0.13.0"
 groq = "^0.4.2"
 phonenumbers = "^8.13.33"
 cohere = "^5.1.8"
+mistralai = "^0.1.8"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `instructor-1.2.1/PKG-INFO` & `instructor-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructor
-Version: 1.2.1
+Version: 1.2.2
 Summary: structured outputs for llm
 Home-page: https://github.com/jxnl/instructor
 License: MIT
 Author: Jason Liu
 Author-email: jason@jxnl.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,23 +12,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: anthropic
 Provides-Extra: cohere
 Provides-Extra: groq
+Provides-Extra: mistralai
 Provides-Extra: test-docs
 Requires-Dist: aiohttp (>=3.9.1,<4.0.0)
 Requires-Dist: anthropic (>=0.23.1,<0.24.0) ; extra == "anthropic" or extra == "test-docs"
 Requires-Dist: cohere (>=5.1.8,<6.0.0) ; extra == "cohere" or extra == "test-docs"
 Requires-Dist: diskcache (>=5.6.3,<6.0.0) ; extra == "test-docs"
 Requires-Dist: docstring-parser (>=0.16,<0.17)
 Requires-Dist: fastapi (>=0.109.2,<0.110.0) ; extra == "test-docs"
 Requires-Dist: groq (>=0.4.2,<0.5.0) ; extra == "groq" or extra == "test-docs"
 Requires-Dist: litellm (>=1.0.0,<2.0.0) ; extra == "test-docs"
+Requires-Dist: mistralai (>=0.1.8,<0.2.0) ; extra == "test-docs" or extra == "mistralai"
 Requires-Dist: openai (>=1.1.0,<2.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0) ; extra == "test-docs"
 Requires-Dist: pydantic (==2.7.0)
 Requires-Dist: pydantic-core (>=2.18.0,<3.0.0)
 Requires-Dist: pydantic_extra_types (>=2.6.0,<3.0.0) ; extra == "test-docs"
 Requires-Dist: redis (>=5.0.1,<6.0.0) ; extra == "test-docs"
 Requires-Dist: rich (>=13.7.0,<14.0.0)
```

