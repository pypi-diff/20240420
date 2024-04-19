# Comparing `tmp/athena_intelligence-0.1.44.tar.gz` & `tmp/athena_intelligence-0.1.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athena_intelligence-0.1.44.tar", max compression
+gzip compressed data, was "athena_intelligence-0.1.45.tar", max compression
```

## Comparing `athena_intelligence-0.1.44.tar` & `athena_intelligence-0.1.45.tar`

### file list

```diff
@@ -1,61 +1,59 @@
--rw-r--r--   0        0        0     4235 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/README.md
--rw-r--r--   0        0        0      435 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/pyproject.toml
--rw-r--r--   0        0        0     1489 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/__init__.py
--rw-r--r--   0        0        0     5416 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/base_client.py
--rw-r--r--   0        0        0      159 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/chain/__init__.py
--rw-r--r--   0        0        0     8333 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/chain/client.py
--rw-r--r--   0        0        0      187 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/chain/types/__init__.py
--rw-r--r--   0        0        0     2203 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/chain/types/structured_parse_in_parsing_model.py
--rw-r--r--   0        0        0     3576 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/client.py
--rw-r--r--   0        0        0      790 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/core/api_error.py
--rw-r--r--   0        0        0     1198 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/core/file.py
--rw-r--r--   0        0        0     4882 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/core/request_options.py
--rw-r--r--   0        0        0       65 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/dataset/__init__.py
--rw-r--r--   0        0        0     6087 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/dataset/client.py
--rw-r--r--   0        0        0      165 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/environment.py
--rw-r--r--   0        0        0      170 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/message/__init__.py
--rw-r--r--   0        0        0    12185 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/message/client.py
--rw-r--r--   0        0        0     3998 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/polling_message_client.py
--rw-r--r--   0        0        0        0 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/py.typed
--rw-r--r--   0        0        0       65 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/query/__init__.py
--rw-r--r--   0        0        0     6243 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/query/client.py
--rw-r--r--   0        0        0       65 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/report/__init__.py
--rw-r--r--   0        0        0     6528 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/report/client.py
--rw-r--r--   0        0        0       65 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/search/__init__.py
--rw-r--r--   0        0        0     7515 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/search/client.py
--rw-r--r--   0        0        0       65 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/snippet/__init__.py
--rw-r--r--   0        0        0     6087 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/snippet/client.py
--rw-r--r--   0        0        0       65 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/tools/__init__.py
--rw-r--r--   0        0        0    19643 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/tools/client.py
--rw-r--r--   0        0        0     1607 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/types/__init__.py
--rw-r--r--   0        0        0     1014 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/types/dataset.py
--rw-r--r--   0        0        0     1081 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/types/document.py
--rw-r--r--   0        0        0      895 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/types/excecute_tool_first_workflow_out.py
--rw-r--r--   0        0        0     1021 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py
--rw-r--r--   0        0        0     1128 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/types/firecrawl_scrape_url_metadata.py
--rw-r--r--   0        0        0      989 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/types/get_datasets_response.py
--rw-r--r--   0        0        0      989 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/types/get_snippets_response.py
--rw-r--r--   0        0        0      973 2024-04-18 17:52:21.270816 athena_intelligence-0.1.44/src/athena/types/http_validation_error.py
--rw-r--r--   0        0        0      939 2024-04-18 17:52:21.274816 athena_intelligence-0.1.44/src/athena/types/langchain_documents_request_out.py
--rw-r--r--   0        0        0      865 2024-04-18 17:52:21.274816 athena_intelligence-0.1.44/src/athena/types/message_out.py
--rw-r--r--   0        0        0     1051 2024-04-18 17:52:21.274816 athena_intelligence-0.1.44/src/athena/types/message_out_dto.py
--rw-r--r--   0        0        0     2767 2024-04-18 17:52:21.274816 athena_intelligence-0.1.44/src/athena/types/model.py
--rw-r--r--   0        0        0      946 2024-04-18 17:52:21.274816 athena_intelligence-0.1.44/src/athena/types/report.py
--rw-r--r--   0        0        0     1126 2024-04-18 17:52:21.274816 athena_intelligence-0.1.44/src/athena/types/snippet.py
--rw-r--r--   0        0        0      900 2024-04-18 17:52:21.274816 athena_intelligence-0.1.44/src/athena/types/sql_results.py
--rw-r--r--   0        0        0      672 2024-04-18 17:52:21.274816 athena_intelligence-0.1.44/src/athena/types/status_enum.py
--rw-r--r--   0        0        0      905 2024-04-18 17:52:21.274816 athena_intelligence-0.1.44/src/athena/types/structured_parse_result.py
--rw-r--r--   0        0        0     1829 2024-04-18 17:52:21.274816 athena_intelligence-0.1.44/src/athena/types/tool_models.py
--rw-r--r--   0        0        0     1422 2024-04-18 17:52:21.274816 athena_intelligence-0.1.44/src/athena/types/tools.py
--rw-r--r--   0        0        0      893 2024-04-18 17:52:21.274816 athena_intelligence-0.1.44/src/athena/types/url_result.py
--rw-r--r--   0        0        0      992 2024-04-18 17:52:21.274816 athena_intelligence-0.1.44/src/athena/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-18 17:52:21.274816 athena_intelligence-0.1.44/src/athena/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.44/PKG-INFO
+-rw-r--r--   0        0        0     4235 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/README.md
+-rw-r--r--   0        0        0      435 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/pyproject.toml
+-rw-r--r--   0        0        0     1389 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/__init__.py
+-rw-r--r--   0        0        0     5416 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/base_client.py
+-rw-r--r--   0        0        0      159 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/chain/__init__.py
+-rw-r--r--   0        0        0     8333 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/chain/client.py
+-rw-r--r--   0        0        0      187 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/chain/types/__init__.py
+-rw-r--r--   0        0        0     2203 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/chain/types/structured_parse_in_parsing_model.py
+-rw-r--r--   0        0        0     3576 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/client.py
+-rw-r--r--   0        0        0      790 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/core/api_error.py
+-rw-r--r--   0        0        0     1198 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/core/file.py
+-rw-r--r--   0        0        0     4882 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/core/http_client.py
+-rw-r--r--   0        0        0     3799 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/core/request_options.py
+-rw-r--r--   0        0        0       65 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/dataset/__init__.py
+-rw-r--r--   0        0        0     6087 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/dataset/client.py
+-rw-r--r--   0        0        0      165 2024-04-19 22:38:25.247562 athena_intelligence-0.1.45/src/athena/environment.py
+-rw-r--r--   0        0        0      170 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/message/__init__.py
+-rw-r--r--   0        0        0    12185 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/message/client.py
+-rw-r--r--   0        0        0     3998 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/polling_message_client.py
+-rw-r--r--   0        0        0        0 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/py.typed
+-rw-r--r--   0        0        0       65 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/query/__init__.py
+-rw-r--r--   0        0        0     6243 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/query/client.py
+-rw-r--r--   0        0        0       65 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/report/__init__.py
+-rw-r--r--   0        0        0     6528 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/report/client.py
+-rw-r--r--   0        0        0       65 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/search/__init__.py
+-rw-r--r--   0        0        0     7515 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/search/client.py
+-rw-r--r--   0        0        0       65 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/snippet/__init__.py
+-rw-r--r--   0        0        0     6087 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/snippet/client.py
+-rw-r--r--   0        0        0       65 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/tools/__init__.py
+-rw-r--r--   0        0        0    13328 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/tools/client.py
+-rw-r--r--   0        0        0     1450 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/__init__.py
+-rw-r--r--   0        0        0     1014 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/dataset.py
+-rw-r--r--   0        0        0      895 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/excecute_tool_first_workflow_out.py
+-rw-r--r--   0        0        0     1021 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py
+-rw-r--r--   0        0        0     1128 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/firecrawl_scrape_url_metadata.py
+-rw-r--r--   0        0        0      989 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/get_datasets_response.py
+-rw-r--r--   0        0        0      989 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/get_snippets_response.py
+-rw-r--r--   0        0        0      973 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/http_validation_error.py
+-rw-r--r--   0        0        0      865 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/message_out.py
+-rw-r--r--   0        0        0     1051 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/message_out_dto.py
+-rw-r--r--   0        0        0     3180 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/model.py
+-rw-r--r--   0        0        0      946 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/report.py
+-rw-r--r--   0        0        0     1126 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/snippet.py
+-rw-r--r--   0        0        0      900 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/sql_results.py
+-rw-r--r--   0        0        0      672 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/status_enum.py
+-rw-r--r--   0        0        0      905 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/structured_parse_result.py
+-rw-r--r--   0        0        0     1829 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/tool_models.py
+-rw-r--r--   0        0        0     1422 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/tools.py
+-rw-r--r--   0        0        0      893 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/url_result.py
+-rw-r--r--   0        0        0      992 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-19 22:38:25.251562 athena_intelligence-0.1.45/src/athena/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.45/PKG-INFO
```

### Comparing `athena_intelligence-0.1.44/README.md` & `athena_intelligence-0.1.45/README.md`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/__init__.py` & `athena_intelligence-0.1.45/src/athena/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
     Dataset,
-    Document,
     ExcecuteToolFirstWorkflowOut,
     FirecrawlScrapeUrlDataReponseDto,
     FirecrawlScrapeUrlMetadata,
     GetDatasetsResponse,
     GetSnippetsResponse,
     HttpValidationError,
-    LangchainDocumentsRequestOut,
     MessageOut,
     MessageOutDto,
     Model,
     Report,
     Snippet,
     SqlResults,
     StatusEnum,
@@ -28,22 +26,20 @@
 from . import chain, dataset, message, query, report, search, snippet, tools
 from .chain import StructuredParseInParsingModel
 from .environment import AthenaEnvironment
 
 __all__ = [
     "AthenaEnvironment",
     "Dataset",
-    "Document",
     "ExcecuteToolFirstWorkflowOut",
     "FirecrawlScrapeUrlDataReponseDto",
     "FirecrawlScrapeUrlMetadata",
     "GetDatasetsResponse",
     "GetSnippetsResponse",
     "HttpValidationError",
-    "LangchainDocumentsRequestOut",
     "MessageOut",
     "MessageOutDto",
     "Model",
     "Report",
     "Snippet",
     "SqlResults",
     "StatusEnum",
```

### Comparing `athena_intelligence-0.1.44/src/athena/base_client.py` & `athena_intelligence-0.1.45/src/athena/base_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/chain/client.py` & `athena_intelligence-0.1.45/src/athena/chain/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/chain/types/structured_parse_in_parsing_model.py` & `athena_intelligence-0.1.45/src/athena/chain/types/structured_parse_in_parsing_model.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/client.py` & `athena_intelligence-0.1.45/src/athena/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/core/__init__.py` & `athena_intelligence-0.1.45/src/athena/core/__init__.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/core/client_wrapper.py` & `athena_intelligence-0.1.45/src/athena/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.api_key = api_key
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "athena-intelligence",
-            "X-Fern-SDK-Version": "0.1.44",
+            "X-Fern-SDK-Version": "0.1.45",
         }
         headers["X-API-KEY"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `athena_intelligence-0.1.44/src/athena/core/datetime_utils.py` & `athena_intelligence-0.1.45/src/athena/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/core/file.py` & `athena_intelligence-0.1.45/src/athena/core/file.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/core/http_client.py` & `athena_intelligence-0.1.45/src/athena/core/http_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/core/jsonable_encoder.py` & `athena_intelligence-0.1.45/src/athena/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/core/request_options.py` & `athena_intelligence-0.1.45/src/athena/core/request_options.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/dataset/client.py` & `athena_intelligence-0.1.45/src/athena/dataset/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/message/client.py` & `athena_intelligence-0.1.45/src/athena/message/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/polling_message_client.py` & `athena_intelligence-0.1.45/src/athena/polling_message_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/query/client.py` & `athena_intelligence-0.1.45/src/athena/query/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/report/client.py` & `athena_intelligence-0.1.45/src/athena/report/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/search/client.py` & `athena_intelligence-0.1.45/src/athena/search/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/snippet/client.py` & `athena_intelligence-0.1.45/src/athena/snippet/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/tools/client.py` & `athena_intelligence-0.1.45/src/athena/tools/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.excecute_tool_first_workflow_out import ExcecuteToolFirstWorkflowOut
 from ..types.firecrawl_scrape_url_data_reponse_dto import FirecrawlScrapeUrlDataReponseDto
 from ..types.http_validation_error import HttpValidationError
-from ..types.langchain_documents_request_out import LangchainDocumentsRequestOut
 from ..types.tool_models import ToolModels
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
@@ -88,84 +87,14 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def langchain_documents(
-        self,
-        *,
-        document_id: str,
-        pagination_limit: typing.Optional[int] = OMIT,
-        pagination_offset: typing.Optional[int] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> LangchainDocumentsRequestOut:
-        """
-        Parameters:
-            - document_id: str.
-
-            - pagination_limit: typing.Optional[int].
-
-            - pagination_offset: typing.Optional[int].
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from athena.client import Athena
-
-        client = Athena(
-            api_key="YOUR_API_KEY",
-        )
-        client.tools.langchain_documents(
-            document_id="doc_9249292-d118-42d3-95b4-00eccfe0754f",
-            pagination_limit=250,
-            pagination_offset=0,
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {"document_id": document_id}
-        if pagination_limit is not OMIT:
-            _request["pagination_limit"] = pagination_limit
-        if pagination_offset is not OMIT:
-            _request["pagination_offset"] = pagination_offset
-        _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/tools/file/langchain-documents"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(LangchainDocumentsRequestOut, _response.json())  # type: ignore
-        if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
     def tool_first_workflow(
         self,
         *,
         model: typing.Optional[ToolModels] = OMIT,
         tool_name: str,
         content: str,
         tool_kwargs: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
@@ -300,84 +229,14 @@
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def langchain_documents(
-        self,
-        *,
-        document_id: str,
-        pagination_limit: typing.Optional[int] = OMIT,
-        pagination_offset: typing.Optional[int] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> LangchainDocumentsRequestOut:
-        """
-        Parameters:
-            - document_id: str.
-
-            - pagination_limit: typing.Optional[int].
-
-            - pagination_offset: typing.Optional[int].
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from athena.client import AsyncAthena
-
-        client = AsyncAthena(
-            api_key="YOUR_API_KEY",
-        )
-        await client.tools.langchain_documents(
-            document_id="doc_9249292-d118-42d3-95b4-00eccfe0754f",
-            pagination_limit=250,
-            pagination_offset=0,
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {"document_id": document_id}
-        if pagination_limit is not OMIT:
-            _request["pagination_limit"] = pagination_limit
-        if pagination_offset is not OMIT:
-            _request["pagination_offset"] = pagination_offset
-        _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/tools/file/langchain-documents"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(LangchainDocumentsRequestOut, _response.json())  # type: ignore
-        if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def tool_first_workflow(
         self,
         *,
         model: typing.Optional[ToolModels] = OMIT,
         tool_name: str,
         content: str,
```

### Comparing `athena_intelligence-0.1.44/src/athena/types/__init__.py` & `athena_intelligence-0.1.45/src/athena/types/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .dataset import Dataset
-from .document import Document
 from .excecute_tool_first_workflow_out import ExcecuteToolFirstWorkflowOut
 from .firecrawl_scrape_url_data_reponse_dto import FirecrawlScrapeUrlDataReponseDto
 from .firecrawl_scrape_url_metadata import FirecrawlScrapeUrlMetadata
 from .get_datasets_response import GetDatasetsResponse
 from .get_snippets_response import GetSnippetsResponse
 from .http_validation_error import HttpValidationError
-from .langchain_documents_request_out import LangchainDocumentsRequestOut
 from .message_out import MessageOut
 from .message_out_dto import MessageOutDto
 from .model import Model
 from .report import Report
 from .snippet import Snippet
 from .sql_results import SqlResults
 from .status_enum import StatusEnum
@@ -21,22 +19,20 @@
 from .tools import Tools
 from .url_result import UrlResult
 from .validation_error import ValidationError
 from .validation_error_loc_item import ValidationErrorLocItem
 
 __all__ = [
     "Dataset",
-    "Document",
     "ExcecuteToolFirstWorkflowOut",
     "FirecrawlScrapeUrlDataReponseDto",
     "FirecrawlScrapeUrlMetadata",
     "GetDatasetsResponse",
     "GetSnippetsResponse",
     "HttpValidationError",
-    "LangchainDocumentsRequestOut",
     "MessageOut",
     "MessageOutDto",
     "Model",
     "Report",
     "Snippet",
     "SqlResults",
     "StatusEnum",
```

### Comparing `athena_intelligence-0.1.44/src/athena/types/dataset.py` & `athena_intelligence-0.1.45/src/athena/types/dataset.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/types/document.py` & `athena_intelligence-0.1.45/src/athena/types/structured_parse_result.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,22 +7,16 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class Document(pydantic.BaseModel):
-    """
-    Class for storing a piece of text and associated metadata.
-    """
-
-    page_content: str
-    metadata: typing.Optional[typing.Dict[str, typing.Any]] = None
-    type: typing.Optional[typing.Literal["Document"]] = None
+class StructuredParseResult(pydantic.BaseModel):
+    result: typing.Dict[str, typing.Any]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `athena_intelligence-0.1.44/src/athena/types/excecute_tool_first_workflow_out.py` & `athena_intelligence-0.1.45/src/athena/types/excecute_tool_first_workflow_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py` & `athena_intelligence-0.1.45/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/types/firecrawl_scrape_url_metadata.py` & `athena_intelligence-0.1.45/src/athena/types/firecrawl_scrape_url_metadata.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/types/get_datasets_response.py` & `athena_intelligence-0.1.45/src/athena/types/get_datasets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/types/get_snippets_response.py` & `athena_intelligence-0.1.45/src/athena/types/get_snippets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/types/http_validation_error.py` & `athena_intelligence-0.1.45/src/athena/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/types/langchain_documents_request_out.py` & `athena_intelligence-0.1.45/src/athena/types/url_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .document import Document
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class LangchainDocumentsRequestOut(pydantic.BaseModel):
-    documents: typing.List[Document]
+class UrlResult(pydantic.BaseModel):
+    result: typing.Dict[str, typing.Any]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `athena_intelligence-0.1.44/src/athena/types/message_out.py` & `athena_intelligence-0.1.45/src/athena/types/message_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/types/message_out_dto.py` & `athena_intelligence-0.1.45/src/athena/types/message_out_dto.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/types/model.py` & `athena_intelligence-0.1.45/src/athena/types/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     GPT_4_TURBO = "gpt-4-turbo"
     GPT_4_TURBO_PREVIEW = "gpt-4-turbo-preview"
     GPT_4 = "gpt-4"
     MIXTRAL_SMALL_8_X_7_B_0211 = "mixtral-small-8x7b-0211"
     MISTRAL_LARGE_0224 = "mistral-large-0224"
     MIXTRAL_8_X_22_B_INSTRUCT = "mixtral-8x22b-instruct"
     LLAMA_V_270_B_CHAT = "llama-v2-70b-chat"
+    LLAMA_V_370_B_INSTRUCT = "llama-v3-70b-instruct"
+    LLAMA_V_38_B_INSTRUCT = "llama-v3-8b-instruct"
     CLAUDE_3_OPUS_20240229 = "claude-3-opus-20240229"
     CLAUDE_3_SONNET_20240229 = "claude-3-sonnet-20240229"
     CLAUDE_3_HAIKU_20240307 = "claude-3-haiku-20240307"
     GOOGLE_GEMINI_10_PRO_LATEST = "google-gemini-1.0-pro-latest"
     DATABRICKS_DBRX = "databricks-dbrx"
 
     def visit(
@@ -31,14 +33,16 @@
         gpt_4_turbo: typing.Callable[[], T_Result],
         gpt_4_turbo_preview: typing.Callable[[], T_Result],
         gpt_4: typing.Callable[[], T_Result],
         mixtral_small_8_x_7_b_0211: typing.Callable[[], T_Result],
         mistral_large_0224: typing.Callable[[], T_Result],
         mixtral_8_x_22_b_instruct: typing.Callable[[], T_Result],
         llama_v_270_b_chat: typing.Callable[[], T_Result],
+        llama_v_370_b_instruct: typing.Callable[[], T_Result],
+        llama_v_38_b_instruct: typing.Callable[[], T_Result],
         claude_3_opus_20240229: typing.Callable[[], T_Result],
         claude_3_sonnet_20240229: typing.Callable[[], T_Result],
         claude_3_haiku_20240307: typing.Callable[[], T_Result],
         google_gemini_10_pro_latest: typing.Callable[[], T_Result],
         databricks_dbrx: typing.Callable[[], T_Result],
     ) -> T_Result:
         if self is Model.GPT_35_TURBO:
@@ -53,14 +57,18 @@
             return mixtral_small_8_x_7_b_0211()
         if self is Model.MISTRAL_LARGE_0224:
             return mistral_large_0224()
         if self is Model.MIXTRAL_8_X_22_B_INSTRUCT:
             return mixtral_8_x_22_b_instruct()
         if self is Model.LLAMA_V_270_B_CHAT:
             return llama_v_270_b_chat()
+        if self is Model.LLAMA_V_370_B_INSTRUCT:
+            return llama_v_370_b_instruct()
+        if self is Model.LLAMA_V_38_B_INSTRUCT:
+            return llama_v_38_b_instruct()
         if self is Model.CLAUDE_3_OPUS_20240229:
             return claude_3_opus_20240229()
         if self is Model.CLAUDE_3_SONNET_20240229:
             return claude_3_sonnet_20240229()
         if self is Model.CLAUDE_3_HAIKU_20240307:
             return claude_3_haiku_20240307()
         if self is Model.GOOGLE_GEMINI_10_PRO_LATEST:
```

### Comparing `athena_intelligence-0.1.44/src/athena/types/report.py` & `athena_intelligence-0.1.45/src/athena/types/report.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/types/snippet.py` & `athena_intelligence-0.1.45/src/athena/types/snippet.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/types/sql_results.py` & `athena_intelligence-0.1.45/src/athena/types/sql_results.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/types/status_enum.py` & `athena_intelligence-0.1.45/src/athena/types/status_enum.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/types/structured_parse_result.py` & `athena_intelligence-0.1.45/src/athena/types/validation_error.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .validation_error_loc_item import ValidationErrorLocItem
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class StructuredParseResult(pydantic.BaseModel):
-    result: typing.Dict[str, typing.Any]
+class ValidationError(pydantic.BaseModel):
+    loc: typing.List[ValidationErrorLocItem]
+    msg: str
+    type: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `athena_intelligence-0.1.44/src/athena/types/tool_models.py` & `athena_intelligence-0.1.45/src/athena/types/tool_models.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/src/athena/types/tools.py` & `athena_intelligence-0.1.45/src/athena/types/tools.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.44/PKG-INFO` & `athena_intelligence-0.1.45/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athena-intelligence
-Version: 0.1.44
+Version: 0.1.45
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

