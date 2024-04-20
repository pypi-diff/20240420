# Comparing `tmp/openapi_service_client-0.0.7.tar.gz` & `tmp/openapi_service_client-0.0.8.tar.gz`

## Comparing `openapi_service_client-0.0.7.tar` & `openapi_service_client-0.0.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/.github/workflows/pypi_release.yml
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/.github/workflows/tests.yml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/__init__.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/client.py
--rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/client_configuration.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/config/__init__.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/config/auth_strategy.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/config/configuration.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/http_client/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/http_client/client.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/providers/__init__.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/providers/anthropic.py
--rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/providers/cohere.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/providers/converter.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/providers/llm_provider.py
--rw-r--r--   0        0        0     7295 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/providers/openai.py
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/providers/payload_extractor.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/request_builder/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/request_builder/builder.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/spec/__init__.py
--rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/spec/open_api_spec.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/spec/operation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/__init__.py
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_client.py
--rw-r--r--   0        0        0     9768 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_client_auth.py
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_client_complex_request_body.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_client_complex_request_body_mixed.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_client_edge_cases.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_client_error_handling.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_client_live.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_client_live_anthropic.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_client_live_cohere.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_client_live_openai.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_cohere_conversion.py
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_openai_conversion.py
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/test_files/complex_types_openapi_service.json
--rw-r--r--   0        0        0    12430 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/test_files/github_compare.yml
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/test_files/openapi_edge_cases.yml
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/test_files/openapi_error_handling.yml
--rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/test_files/openapi_greeting_service.yml
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/test_files/openapi_order_service.json
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/test_files/openapi_order_service.yml
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/test_files/serper.yaml
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/LICENSE
--rw-r--r--   0        0        0     7829 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/README.md
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     8776 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/.github/workflows/pypi_release.yml
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/__init__.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/client.py
+-rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/client_configuration.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/config/__init__.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/config/auth_strategy.py
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/config/configuration.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/http_client/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/http_client/client.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/providers/__init__.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/providers/anthropic.py
+-rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/providers/cohere.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/providers/converter.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/providers/llm_provider.py
+-rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/providers/openai.py
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/providers/payload_extractor.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/request_builder/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/request_builder/builder.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/spec/__init__.py
+-rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/spec/open_api_spec.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/src/openapi_service_client/spec/operation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/__init__.py
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_client.py
+-rw-r--r--   0        0        0     9768 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_client_auth.py
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_client_complex_request_body.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_client_complex_request_body_mixed.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_client_edge_cases.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_client_error_handling.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_client_live.py
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_client_live_anthropic.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_client_live_cohere.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_client_live_openai.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_cohere_conversion.py
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/client/test_openai_conversion.py
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/test_files/complex_types_openapi_service.json
+-rw-r--r--   0        0        0    12430 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/test_files/github_compare.yml
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/test_files/openapi_edge_cases.yml
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/test_files/openapi_error_handling.yml
+-rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/test_files/openapi_greeting_service.yml
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/test_files/openapi_order_service.json
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/test_files/openapi_order_service.yml
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/tests/test_files/serper.yaml
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/LICENSE
+-rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/README.md
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     9423 2020-02-02 00:00:00.000000 openapi_service_client-0.0.8/PKG-INFO
```

### Comparing `openapi_service_client-0.0.7/.github/workflows/tests.yml` & `openapi_service_client-0.0.8/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/src/openapi_service_client/client.py` & `openapi_service_client-0.0.8/src/openapi_service_client/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict
+from typing import Any
 
 from openapi_service_client.client_configuration import ClientConfiguration
 from openapi_service_client.request_builder import RequestBuilder
 
 
 class OpenAPIServiceClient:
     def __init__(
@@ -10,15 +10,28 @@
         client_config: ClientConfiguration,
     ):
         self.openapi_spec = client_config.get_openapi_spec()
         self.http_client = client_config.get_http_client()
         self.request_builder = RequestBuilder(client_config)
         self.payload_extractor = client_config.get_payload_extractor()
 
-    def invoke(self, function_payload: Dict[str, Any]) -> Any:
+    def invoke(self, function_payload: Any) -> Any:
+        """
+        Invokes a function specified in the function payload.
+
+        Function payload is traversed to extract the function name and arguments, construct a request based on an
+        OpenAPI specification, and send the request using a configured HTTP client.
+
+        Function payload can be a dictionary, dataclass, or pydantic v1 and v2 model.
+
+        :param function_payload: The function payload containing the details of the function to be invoked.
+        :returns: The response from the service after invoking the function.
+        :raises OpenAPIClientError: If the function invocation payload cannot be extracted from the function payload.
+        :raises HttpClientError: If an error occurs while sending the request and receiving the response.
+        """
         fn_invocation_payload = self.payload_extractor.extract_function_invocation(function_payload)
         if not fn_invocation_payload:
             raise OpenAPIClientError(
                 f"Failed to extract function invocation payload from {function_payload} using "
                 f"{self.payload_extractor.__class__.__name__}. Ensure the payload format matches the expected "
                 "structure for the designated LLM extractor."
             )
```

### Comparing `openapi_service_client-0.0.7/src/openapi_service_client/client_configuration.py` & `openapi_service_client-0.0.8/src/openapi_service_client/client_configuration.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/src/openapi_service_client/config/configuration.py` & `openapi_service_client-0.0.8/src/openapi_service_client/config/configuration.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/src/openapi_service_client/http_client/client.py` & `openapi_service_client-0.0.8/src/openapi_service_client/http_client/client.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/src/openapi_service_client/providers/__init__.py` & `openapi_service_client-0.0.8/src/openapi_service_client/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/src/openapi_service_client/providers/anthropic.py` & `openapi_service_client-0.0.8/src/openapi_service_client/providers/anthropic.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/src/openapi_service_client/providers/cohere.py` & `openapi_service_client-0.0.8/src/openapi_service_client/providers/cohere.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/src/openapi_service_client/providers/openai.py` & `openapi_service_client-0.0.8/src/openapi_service_client/providers/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 MIN_REQUIRED_OPENAPI_SPEC_VERSION = 3
 
 logger = logging.getLogger(__name__)
 
 
 class OpenAIPayloadExtractor(FunctionPayloadExtractor):
-    def extract_function_invocation(self, payload: Dict[str, Any]) -> Dict[str, Any]:
+    def extract_function_invocation(self, payload: Any) -> Dict[str, Any]:
         fields_and_values = self.search(payload)
         if fields_and_values:
             args = fields_and_values.get("arguments")
             if not isinstance(args, (str, dict)):
                 raise ValueError(f"Invalid arguments type {type(args)} for OpenAI function call, expected str or dict")
             return {
                 "name": fields_and_values.get("name"),
```

### Comparing `openapi_service_client-0.0.7/src/openapi_service_client/providers/payload_extractor.py` & `openapi_service_client-0.0.8/src/openapi_service_client/providers/payload_extractor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import dataclasses
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List
 
 
 class FunctionPayloadExtractor(ABC):
 
     @abstractmethod
-    def extract_function_invocation(self, payload: Dict[str, Any]) -> Dict[str, Any]:
+    def extract_function_invocation(self, payload: Any) -> Dict[str, Any]:
         """
         Extracts the function name and arguments from the LLM generated function call payload.
 
         Regardless of the LLM provider the return value should be a dictionary containing the function name
         and arguments under the keys "name" and "arguments" respectively. If payload is not found, an empty
         dictionary should be returned.
 
@@ -24,37 +25,52 @@
     def required_fields(self) -> List[str]:
         """
         Returns a list of required fields that must be present in the function call payload.
         :returns: A list of required fields to find in the function call payload.
         """
         pass
 
-    def search(self, payload: Dict[str, Any]) -> Dict[str, Any]:
+    def search(self, payload: Any) -> Dict[str, Any]:
+        if self.is_pydantic(payload):
+            payload = payload.dict()
+
+        elif dataclasses.is_dataclass(payload):
+            payload = dataclasses.asdict(payload)
+
         if isinstance(payload, dict):
             if all(field in payload for field in self.required_fields()):
                 return payload
             for _, value in payload.items():
-                if isinstance(value, dict):
+                if isinstance(value, (dict, list)):
                     result = self.search(value)
                     if result:
                         return result
+                elif self.is_pydantic(value):
+                    result = self.search(value.dict())
+                    if result:
+                        return result
 
         elif isinstance(payload, list):
             for item in payload:
                 result = self.search(item)
                 if result:
                     return result
+
         return {}
 
+    def is_pydantic(self, payload: Any) -> bool:
+        # pydantic v1 and v2 models have a dict method that can be used to convert the model to a dictionary
+        return hasattr(payload, "dict") and callable(payload.dict)
+
 
 class GenericPayloadExtractor(FunctionPayloadExtractor):
     def __init__(self, arguments_field_name: str):
         self.arguments_field_name = arguments_field_name
 
-    def extract_function_invocation(self, payload: Dict[str, Any]) -> Dict[str, Any]:
+    def extract_function_invocation(self, payload: Any) -> Dict[str, Any]:
         fields_and_values = self.search(payload)
         if fields_and_values:
             arguments = fields_and_values.get(self.arguments_field_name)
             if not isinstance(arguments, dict):
                 raise ValueError(
                     f"Invalid {self.arguments_field_name} type {type(arguments)} for function call, expected dict"
                 )
```

### Comparing `openapi_service_client-0.0.7/src/openapi_service_client/request_builder/builder.py` & `openapi_service_client-0.0.8/src/openapi_service_client/request_builder/builder.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/src/openapi_service_client/spec/open_api_spec.py` & `openapi_service_client-0.0.8/src/openapi_service_client/spec/open_api_spec.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/src/openapi_service_client/spec/operation.py` & `openapi_service_client-0.0.8/src/openapi_service_client/spec/operation.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/tests/conftest.py` & `openapi_service_client-0.0.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/tests/client/test_client.py` & `openapi_service_client-0.0.8/tests/client/test_client.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/tests/client/test_client_auth.py` & `openapi_service_client-0.0.8/tests/client/test_client_auth.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/tests/client/test_client_complex_request_body.py` & `openapi_service_client-0.0.8/tests/client/test_client_complex_request_body.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/tests/client/test_client_complex_request_body_mixed.py` & `openapi_service_client-0.0.8/tests/client/test_client_complex_request_body_mixed.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/tests/client/test_client_edge_cases.py` & `openapi_service_client-0.0.8/tests/client/test_client_edge_cases.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/tests/client/test_client_error_handling.py` & `openapi_service_client-0.0.8/tests/client/test_client_error_handling.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/tests/client/test_client_live.py` & `openapi_service_client-0.0.8/tests/client/test_client_live.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/tests/client/test_client_live_anthropic.py` & `openapi_service_client-0.0.8/tests/client/test_client_live_anthropic.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/tests/client/test_client_live_cohere.py` & `openapi_service_client-0.0.8/tests/client/test_client_live_cohere.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/tests/client/test_client_live_openai.py` & `openapi_service_client-0.0.8/tests/client/test_client_live_openai.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/tests/client/test_cohere_conversion.py` & `openapi_service_client-0.0.8/tests/client/test_cohere_conversion.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/tests/client/test_openai_conversion.py` & `openapi_service_client-0.0.8/tests/client/test_openai_conversion.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/tests/test_files/complex_types_openapi_service.json` & `openapi_service_client-0.0.8/tests/test_files/complex_types_openapi_service.json`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/tests/test_files/github_compare.yml` & `openapi_service_client-0.0.8/tests/test_files/github_compare.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/tests/test_files/openapi_error_handling.yml` & `openapi_service_client-0.0.8/tests/test_files/openapi_error_handling.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/tests/test_files/openapi_greeting_service.yml` & `openapi_service_client-0.0.8/tests/test_files/openapi_greeting_service.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/tests/test_files/openapi_order_service.json` & `openapi_service_client-0.0.8/tests/test_files/openapi_order_service.json`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/tests/test_files/openapi_order_service.yml` & `openapi_service_client-0.0.8/tests/test_files/openapi_order_service.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/tests/test_files/serper.yaml` & `openapi_service_client-0.0.8/tests/test_files/serper.yaml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/.gitignore` & `openapi_service_client-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/LICENSE` & `openapi_service_client-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/README.md` & `openapi_service_client-0.0.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openapi-service-client.svg)](https://pypi.org/project/openapi-service-client)
 
 
 OpenAPI Service Client is a Python library that enables effortless integration between Large Language Models (LLMs) and services defined by OpenAPI specifications. It provides a simple and intuitive way to invoke REST services using the function-calling JSON format, making it easy to integrate with LLM-generated function calls.
 
 ## Motivation
 
-The OpenAPI Service Client library aims to simplify the process of invoking OpenAPI-defined services using function calling payloads from various LLM providers. By abstracting away the complexities of making HTTP requests, handling authentication, preparing invocation payloads and processing responses, it allows users to easily invoke underlying services with LLM generated function calls.
+The OpenAPI Service Client library aims to simplify the process of invoking OpenAPI-defined services using function-calling payloads from various LLM providers. By abstracting away the complexities of making HTTP requests, handling authentication, preparing invocation payloads, and processing responses, it allows users to easily invoke underlying services with LLM-generated function calls.
 
-The library supports multiple LLM providers, including OpenAI, Anthropic, and Cohere, streamlining the process of integrating LLMs with OpenAPI services. It also provides a flexible and extensible architecture that allows users to add support for additional LLM providers and function-calling formats.
+The library supports multiple LLM providers, including OpenAI, Anthropic, and Cohere. Each LLM provider uses a unique function-calling schema definition format; OpenAPI Service Client abstracts these differences, enabling a uniform approach to service invocation. Additionally, the library provides a flexible and extensible architecture that allows users to add support for additional LLM providers and function-calling formats.
 
 ## Features
 
 - Easy integration with LLM-generated function calls
 - Support for various LLM providers, including OpenAI, Anthropic, and Cohere
 - Automatic handling of REST invocations based on OpenAPI specifications
 - Support for various authentication strategies, including API key, HTTP authentication, and OAuth2
@@ -43,34 +43,38 @@
 
 ```python
 import os
 from openai import OpenAI
 from openapi_service_client.client import OpenAPIServiceClient
 from openapi_service_client.client_configuration import ClientConfigurationBuilder
 
+# Configure the API client
 builder = ClientConfigurationBuilder()
 config = (
     builder.with_openapi_spec("https://bit.ly/serper_dev_spec_yaml")
     .with_credentials(os.getenv("SERPERDEV_API_KEY"))
     .build()
 )
 
+# Initialize the OpenAPIServiceClient with configuration
+serper_api = OpenAPIServiceClient(config)
+
+# Setup the OpenAI API client and send the chat message
 client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))
 tool_choice = config.get_tools_definitions()
 response = client.chat.completions.create(
     model="gpt-3.5-turbo",
     messages=[{"role": "user", "content": "Do a google search: Who was Nikola Tesla?"}],
     tools=[{"type": "function", "function": tool_choice[0]}],
     tool_choice={"type": "function", "function": {"name": tool_choice[0]["name"]}},
 )
 
-tool_payloads = response.choices[0].message.tool_calls
-serper_api = OpenAPIServiceClient(config)
-response = serper_api.invoke(tool_payloads[0].to_dict())
-print(response)
+# Extract the function-calling payload from response and invoke the service
+service_response = serper_api.invoke(response)
+print(service_response)
 ```
 
 ### Anthropic Example
 
 To run the Anthropic Claude Opus example below, you need:
 
 1) Install anthropic package (`pip install anthropic`)
@@ -81,37 +85,40 @@
 ```python
 import os
 import anthropic
 from openapi_service_client.client import OpenAPIServiceClient
 from openapi_service_client.client_configuration import ClientConfigurationBuilder
 from openapi_service_client.providers import AnthropicLLMProvider
 
-
+# Configure the API client
 builder = ClientConfigurationBuilder()
 config = (
     builder.with_openapi_spec("https://bit.ly/serper_dev_spec_yaml")
     .with_credentials(os.getenv("SERPERDEV_API_KEY"))
     .with_provider(AnthropicLLMProvider())
     .build()
 )
 
+# Initialize the OpenAPIServiceClient with configuration
+serper_api = OpenAPIServiceClient(config)
+
+# Setup the Anthropic API client and send the chat message
 client = anthropic.Anthropic(api_key=os.getenv("ANTHROPIC_API_KEY"))
-tool_choice = config.get_tools_definitions()
 
+# Create a message request using the Anthropic API client
 response = client.beta.tools.messages.create(
     model="claude-3-opus-20240229",
     max_tokens=1024,
-    tools=[tool_choice[0]],
+    tools=config.get_tools_definitions(),
     messages=[{"role": "user", "content": "Do a google search: Who was Nikola Tesla?"}],
 )
 
-tool_payload = response.content[1].to_dict()
-serper_api = OpenAPIServiceClient(config)
-response = serper_api.invoke(tool_payload)
-print(response)
+# Extract the function-calling payload from the response and invoke the service
+service_response = serper_api.invoke(response)
+print(service_response)
 ```
 ### Cohere Example
 
 To run the Cohere Command-R example below, you need:
 
 1) Install cohere package (`pip install cohere`)
 2) Cohere API key. You can obtain Cohere API key by signing up for an account on the Cohere platform. See https://cohere.ai/ for more details.
@@ -121,36 +128,40 @@
 ```python
 import os
 import cohere
 from openapi_service_client.client import OpenAPIServiceClient
 from openapi_service_client.client_configuration import ClientConfigurationBuilder
 from openapi_service_client.providers import CohereLLMProvider
 
+# Configure the API client
 builder = ClientConfigurationBuilder()
 config = (
     builder.with_openapi_spec("https://bit.ly/serper_dev_spec_yaml")
     .with_credentials(os.getenv("SERPERDEV_API_KEY"))
     .with_provider(CohereLLMProvider())
     .build()
 )
 
+# Initialize the OpenAPIServiceClient with configuration
+serper_api = OpenAPIServiceClient(config)
+
+# Setup the Cohere client 
 client = cohere.Client(api_key=os.getenv("COHERE_API_KEY"))
-tool_choices = config.get_tools_definitions()
 
+# And send the chat message
 response = client.chat(
     model="command-r",
     preamble="A preamble aka system prompt goes here.",
-    tools=tool_choices,
+    tools=config.get_tools_definitions(),
     message="Do a google search: Who was Nikola Tesla?",
 )
 
-tool_payload = response.tool_calls[0].dict()
-serper_api = OpenAPIServiceClient(config)
-response = serper_api.invoke(tool_payload)
-print(response)
+# Extract the function-calling payload and invoke the service
+service_response = serper_api.invoke(response)
+print(service_response)
 ```
 
 ## How It Works
 `OpenAPIServiceClient` simplifies the process of invoking REST services defined by OpenAPI specifications. It takes care of the complexities involved in making HTTP requests, handling authentication, and processing responses.
 
 When you provide an OpenAPI specification file to the client, it parses the specification and sets up the necessary request payloads and configurations to interact with the API based on the provided specification. You can then invoke specific operations using the OpenAI function-calling JSON format, which specifies the operation name and its arguments.
```

### Comparing `openapi_service_client-0.0.7/pyproject.toml` & `openapi_service_client-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.7/PKG-INFO` & `openapi_service_client-0.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openapi-service-client
-Version: 0.0.7
+Version: 0.0.8
 Summary: A client library for invoking APIs based on provided OpenAPI specifications
 Project-URL: Documentation, https://github.com/vblagoje/openapi-service-client/blob/main/README.md
 Project-URL: Issues, https://github.com/vblagoje/openapi-service-client/issues
 Project-URL: Source, https://github.com/vblagoje/openapi-service-client
 Author-email: Vladimir Blagojevic <dovlex@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -25,17 +25,17 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openapi-service-client.svg)](https://pypi.org/project/openapi-service-client)
 
 
 OpenAPI Service Client is a Python library that enables effortless integration between Large Language Models (LLMs) and services defined by OpenAPI specifications. It provides a simple and intuitive way to invoke REST services using the function-calling JSON format, making it easy to integrate with LLM-generated function calls.
 
 ## Motivation
 
-The OpenAPI Service Client library aims to simplify the process of invoking OpenAPI-defined services using function calling payloads from various LLM providers. By abstracting away the complexities of making HTTP requests, handling authentication, preparing invocation payloads and processing responses, it allows users to easily invoke underlying services with LLM generated function calls.
+The OpenAPI Service Client library aims to simplify the process of invoking OpenAPI-defined services using function-calling payloads from various LLM providers. By abstracting away the complexities of making HTTP requests, handling authentication, preparing invocation payloads, and processing responses, it allows users to easily invoke underlying services with LLM-generated function calls.
 
-The library supports multiple LLM providers, including OpenAI, Anthropic, and Cohere, streamlining the process of integrating LLMs with OpenAPI services. It also provides a flexible and extensible architecture that allows users to add support for additional LLM providers and function-calling formats.
+The library supports multiple LLM providers, including OpenAI, Anthropic, and Cohere. Each LLM provider uses a unique function-calling schema definition format; OpenAPI Service Client abstracts these differences, enabling a uniform approach to service invocation. Additionally, the library provides a flexible and extensible architecture that allows users to add support for additional LLM providers and function-calling formats.
 
 ## Features
 
 - Easy integration with LLM-generated function calls
 - Support for various LLM providers, including OpenAI, Anthropic, and Cohere
 - Automatic handling of REST invocations based on OpenAPI specifications
 - Support for various authentication strategies, including API key, HTTP authentication, and OAuth2
@@ -65,34 +65,38 @@
 
 ```python
 import os
 from openai import OpenAI
 from openapi_service_client.client import OpenAPIServiceClient
 from openapi_service_client.client_configuration import ClientConfigurationBuilder
 
+# Configure the API client
 builder = ClientConfigurationBuilder()
 config = (
     builder.with_openapi_spec("https://bit.ly/serper_dev_spec_yaml")
     .with_credentials(os.getenv("SERPERDEV_API_KEY"))
     .build()
 )
 
+# Initialize the OpenAPIServiceClient with configuration
+serper_api = OpenAPIServiceClient(config)
+
+# Setup the OpenAI API client and send the chat message
 client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))
 tool_choice = config.get_tools_definitions()
 response = client.chat.completions.create(
     model="gpt-3.5-turbo",
     messages=[{"role": "user", "content": "Do a google search: Who was Nikola Tesla?"}],
     tools=[{"type": "function", "function": tool_choice[0]}],
     tool_choice={"type": "function", "function": {"name": tool_choice[0]["name"]}},
 )
 
-tool_payloads = response.choices[0].message.tool_calls
-serper_api = OpenAPIServiceClient(config)
-response = serper_api.invoke(tool_payloads[0].to_dict())
-print(response)
+# Extract the function-calling payload from response and invoke the service
+service_response = serper_api.invoke(response)
+print(service_response)
 ```
 
 ### Anthropic Example
 
 To run the Anthropic Claude Opus example below, you need:
 
 1) Install anthropic package (`pip install anthropic`)
@@ -103,37 +107,40 @@
 ```python
 import os
 import anthropic
 from openapi_service_client.client import OpenAPIServiceClient
 from openapi_service_client.client_configuration import ClientConfigurationBuilder
 from openapi_service_client.providers import AnthropicLLMProvider
 
-
+# Configure the API client
 builder = ClientConfigurationBuilder()
 config = (
     builder.with_openapi_spec("https://bit.ly/serper_dev_spec_yaml")
     .with_credentials(os.getenv("SERPERDEV_API_KEY"))
     .with_provider(AnthropicLLMProvider())
     .build()
 )
 
+# Initialize the OpenAPIServiceClient with configuration
+serper_api = OpenAPIServiceClient(config)
+
+# Setup the Anthropic API client and send the chat message
 client = anthropic.Anthropic(api_key=os.getenv("ANTHROPIC_API_KEY"))
-tool_choice = config.get_tools_definitions()
 
+# Create a message request using the Anthropic API client
 response = client.beta.tools.messages.create(
     model="claude-3-opus-20240229",
     max_tokens=1024,
-    tools=[tool_choice[0]],
+    tools=config.get_tools_definitions(),
     messages=[{"role": "user", "content": "Do a google search: Who was Nikola Tesla?"}],
 )
 
-tool_payload = response.content[1].to_dict()
-serper_api = OpenAPIServiceClient(config)
-response = serper_api.invoke(tool_payload)
-print(response)
+# Extract the function-calling payload from the response and invoke the service
+service_response = serper_api.invoke(response)
+print(service_response)
 ```
 ### Cohere Example
 
 To run the Cohere Command-R example below, you need:
 
 1) Install cohere package (`pip install cohere`)
 2) Cohere API key. You can obtain Cohere API key by signing up for an account on the Cohere platform. See https://cohere.ai/ for more details.
@@ -143,36 +150,40 @@
 ```python
 import os
 import cohere
 from openapi_service_client.client import OpenAPIServiceClient
 from openapi_service_client.client_configuration import ClientConfigurationBuilder
 from openapi_service_client.providers import CohereLLMProvider
 
+# Configure the API client
 builder = ClientConfigurationBuilder()
 config = (
     builder.with_openapi_spec("https://bit.ly/serper_dev_spec_yaml")
     .with_credentials(os.getenv("SERPERDEV_API_KEY"))
     .with_provider(CohereLLMProvider())
     .build()
 )
 
+# Initialize the OpenAPIServiceClient with configuration
+serper_api = OpenAPIServiceClient(config)
+
+# Setup the Cohere client 
 client = cohere.Client(api_key=os.getenv("COHERE_API_KEY"))
-tool_choices = config.get_tools_definitions()
 
+# And send the chat message
 response = client.chat(
     model="command-r",
     preamble="A preamble aka system prompt goes here.",
-    tools=tool_choices,
+    tools=config.get_tools_definitions(),
     message="Do a google search: Who was Nikola Tesla?",
 )
 
-tool_payload = response.tool_calls[0].dict()
-serper_api = OpenAPIServiceClient(config)
-response = serper_api.invoke(tool_payload)
-print(response)
+# Extract the function-calling payload and invoke the service
+service_response = serper_api.invoke(response)
+print(service_response)
 ```
 
 ## How It Works
 `OpenAPIServiceClient` simplifies the process of invoking REST services defined by OpenAPI specifications. It takes care of the complexities involved in making HTTP requests, handling authentication, and processing responses.
 
 When you provide an OpenAPI specification file to the client, it parses the specification and sets up the necessary request payloads and configurations to interact with the API based on the provided specification. You can then invoke specific operations using the OpenAI function-calling JSON format, which specifies the operation name and its arguments.
```

