# Comparing `tmp/graphlit_client-1.0.20240420001.tar.gz` & `tmp/graphlit_client-1.0.20240420002.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphlit_client-1.0.20240420001.tar", last modified: Sat Apr 20 19:41:46 2024, max compression
+gzip compressed data, was "graphlit_client-1.0.20240420002.tar", last modified: Sat Apr 20 19:48:17 2024, max compression
```

## Comparing `graphlit_client-1.0.20240420001.tar` & `graphlit_client-1.0.20240420002.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 19:41:46.624794 graphlit_client-1.0.20240420001/
--rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-20 19:41:46.624794 graphlit_client-1.0.20240420001/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2321 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 19:41:46.604794 graphlit_client-1.0.20240420001/graphlit/
--rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1796 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit/graphlit.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 19:41:46.620794 graphlit_client-1.0.20240420001/graphlit_api/
--rw-r--r--   0 vsts      (1001) docker     (127)    58023 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/add_contents_to_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3472 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/async_base_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/base_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/clear_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41721 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/close_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      772 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7078 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3905 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/create_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/create_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/create_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/create_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/create_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/create_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      984 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_all_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_all_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_all_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_all_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_all_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/disable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/disable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/enable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/enable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16585 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/extract_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6950 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      677 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/ingest_encoded_file.py
--rw-r--r--   0 vsts      (1001) docker     (127)      606 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/ingest_text.py
--rw-r--r--   0 vsts      (1001) docker     (127)      598 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/ingest_uri.py
--rw-r--r--   0 vsts      (1001) docker     (127)    68146 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/input_types.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/is_content_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/is_feed_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/lookup_credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1568 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/lookup_usage.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39187 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/operations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1236 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/project.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3242 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/prompt_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2055 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/prompt_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)      796 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/publish_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/publish_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/query_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/query_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1112 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/query_content_facets.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7934 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/query_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4623 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/query_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7942 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/query_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4912 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/query_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8865 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/query_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/remove_contents_from_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4382 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/suggest_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/summarize_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/update_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/update_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      644 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/update_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/update_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/update_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/update_project.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/update_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/update_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1482 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/usage.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7663 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/workflow.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 19:41:46.624794 graphlit_client-1.0.20240420001/graphlit_client.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-20 19:41:46.000000 graphlit_client-1.0.20240420001/graphlit_client.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2799 2024-04-20 19:41:46.000000 graphlit_client-1.0.20240420001/graphlit_client.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-20 19:41:46.000000 graphlit_client-1.0.20240420001/graphlit_client.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-20 19:41:46.000000 graphlit_client-1.0.20240420001/graphlit_client.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-04-20 19:41:46.000000 graphlit_client-1.0.20240420001/graphlit_client.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      299 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-20 19:41:46.624794 graphlit_client-1.0.20240420001/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 19:48:17.755920 graphlit_client-1.0.20240420002/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-20 19:48:17.755920 graphlit_client-1.0.20240420002/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2321 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 19:48:17.743920 graphlit_client-1.0.20240420002/graphlit/
+-rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1796 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit/graphlit.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 19:48:17.755920 graphlit_client-1.0.20240420002/graphlit_api/
+-rw-r--r--   0 vsts      (1001) docker     (127)    58929 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/add_contents_to_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/async_base_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/base_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/clear_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    42057 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/close_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/create_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/create_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/create_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/create_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/create_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/create_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      984 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/delete_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/delete_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/delete_all_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/delete_all_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/delete_all_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/delete_all_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/delete_all_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/delete_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/delete_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/delete_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/delete_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/delete_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/delete_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/delete_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/delete_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/delete_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/delete_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/delete_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/disable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/disable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/enable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/enable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16585 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/extract_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3609 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/get_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/get_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7230 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/get_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4014 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/get_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7138 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/get_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1269 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/get_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4461 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/get_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7887 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/get_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      677 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/ingest_encoded_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      606 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/ingest_text.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      598 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/ingest_uri.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    68146 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/input_types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/is_content_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/is_feed_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/lookup_credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1568 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/lookup_usage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39275 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3242 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/prompt_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2055 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/prompt_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      796 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/publish_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/publish_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/query_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/query_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1112 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/query_content_facets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7934 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/query_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4623 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/query_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7942 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/query_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4912 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/query_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8865 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/query_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/remove_contents_from_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/suggest_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/summarize_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/update_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/update_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      644 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/update_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/update_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/update_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/update_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/update_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/update_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1482 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/graphlit_api/usage.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 19:48:17.755920 graphlit_client-1.0.20240420002/graphlit_client.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-20 19:48:17.000000 graphlit_client-1.0.20240420002/graphlit_client.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2831 2024-04-20 19:48:17.000000 graphlit_client-1.0.20240420002/graphlit_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-20 19:48:17.000000 graphlit_client-1.0.20240420002/graphlit_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-20 19:48:17.000000 graphlit_client-1.0.20240420002/graphlit_client.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-04-20 19:48:17.000000 graphlit_client-1.0.20240420002/graphlit_client.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      299 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-20 19:48:17.755920 graphlit_client-1.0.20240420002/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-04-20 19:48:02.000000 graphlit_client-1.0.20240420002/setup.py
```

### Comparing `graphlit_client-1.0.20240420001/LICENSE` & `graphlit_client-1.0.20240420002/LICENSE`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/PKG-INFO` & `graphlit_client-1.0.20240420002/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 1.0.20240420001
+Version: 1.0.20240420002
 Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
 Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `graphlit_client-1.0.20240420001/README.md` & `graphlit_client-1.0.20240420002/README.md`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit/graphlit.py` & `graphlit_client-1.0.20240420002/graphlit/graphlit.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/__init__.py` & `graphlit_client-1.0.20240420002/graphlit_api/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,88 +1,19 @@
 # Generated by ariadne-codegen
 
 from .add_contents_to_collections import (
     AddContentsToCollections,
     AddContentsToCollectionsAddContentsToCollections,
     AddContentsToCollectionsAddContentsToCollectionsContents,
 )
-from .alert import (
-    Alert,
-    AlertAlert,
-    AlertAlertFilter,
-    AlertAlertFilterCollections,
-    AlertAlertFilterContents,
-    AlertAlertFilterCreationDateRange,
-    AlertAlertFilterDateRange,
-    AlertAlertFilterFeeds,
-    AlertAlertFilterObservations,
-    AlertAlertFilterObservationsObservable,
-    AlertAlertFilterWorkflows,
-    AlertAlertIntegration,
-    AlertAlertIntegrationSlack,
-    AlertAlertOwner,
-    AlertAlertPublishing,
-    AlertAlertPublishingElevenLabs,
-    AlertAlertPublishSpecification,
-    AlertAlertSummarySpecification,
-)
 from .async_base_client import AsyncBaseClient
 from .base_model import BaseModel, Upload
 from .clear_conversation import ClearConversation, ClearConversationClearConversation
 from .client import Client
 from .close_conversation import CloseConversation, CloseConversationCloseConversation
-from .collection import (
-    Collection,
-    CollectionCollection,
-    CollectionCollectionContents,
-    CollectionCollectionOwner,
-)
-from .content import (
-    Content,
-    ContentContent,
-    ContentContentAudio,
-    ContentContentChildren,
-    ContentContentCollections,
-    ContentContentDocument,
-    ContentContentEmail,
-    ContentContentEmailBcc,
-    ContentContentEmailCc,
-    ContentContentEmailFrom,
-    ContentContentEmailTo,
-    ContentContentFeed,
-    ContentContentImage,
-    ContentContentIssue,
-    ContentContentLinks,
-    ContentContentObservations,
-    ContentContentObservationsObservable,
-    ContentContentObservationsOccurrences,
-    ContentContentObservationsOccurrencesBoundingBox,
-    ContentContentOwner,
-    ContentContentParent,
-    ContentContentVideo,
-    ContentContentWorkflow,
-)
-from .conversation import (
-    Conversation,
-    ConversationConversation,
-    ConversationConversationFilter,
-    ConversationConversationFilterCollections,
-    ConversationConversationFilterContents,
-    ConversationConversationFilterCreationDateRange,
-    ConversationConversationFilterDateRange,
-    ConversationConversationFilterFeeds,
-    ConversationConversationFilterObservations,
-    ConversationConversationFilterObservationsObservable,
-    ConversationConversationFilterWorkflows,
-    ConversationConversationMessages,
-    ConversationConversationMessagesCitations,
-    ConversationConversationMessagesCitationsContent,
-    ConversationConversationOwner,
-    ConversationConversationSpecification,
-)
 from .create_alert import CreateAlert, CreateAlertCreateAlert
 from .create_collection import CreateCollection, CreateCollectionCreateCollection
 from .create_conversation import (
     CreateConversation,
     CreateConversationCreateConversation,
 )
 from .create_feed import CreateFeed, CreateFeedCreateFeed
@@ -247,42 +178,164 @@
 )
 from .extract_contents import (
     ExtractContents,
     ExtractContentsExtractContents,
     ExtractContentsExtractContentsContent,
     ExtractContentsExtractContentsSpecification,
 )
-from .feed import (
-    Feed,
-    FeedFeed,
-    FeedFeedDiscord,
-    FeedFeedEmail,
-    FeedFeedEmailGoogle,
-    FeedFeedEmailMicrosoft,
-    FeedFeedIssue,
-    FeedFeedIssueGithub,
-    FeedFeedIssueJira,
-    FeedFeedIssueLinear,
-    FeedFeedNotion,
-    FeedFeedOwner,
-    FeedFeedReddit,
-    FeedFeedRss,
-    FeedFeedSchedulePolicy,
-    FeedFeedSite,
-    FeedFeedSiteAzureBlob,
-    FeedFeedSiteAzureFile,
-    FeedFeedSiteGoogle,
-    FeedFeedSiteGoogleDrive,
-    FeedFeedSiteOneDrive,
-    FeedFeedSiteS3,
-    FeedFeedSiteSharePoint,
-    FeedFeedSlack,
-    FeedFeedWeb,
-    FeedFeedWorkflow,
-    FeedFeedYoutube,
+from .get_alert import (
+    GetAlert,
+    GetAlertAlert,
+    GetAlertAlertFilter,
+    GetAlertAlertFilterCollections,
+    GetAlertAlertFilterContents,
+    GetAlertAlertFilterCreationDateRange,
+    GetAlertAlertFilterDateRange,
+    GetAlertAlertFilterFeeds,
+    GetAlertAlertFilterObservations,
+    GetAlertAlertFilterObservationsObservable,
+    GetAlertAlertFilterWorkflows,
+    GetAlertAlertIntegration,
+    GetAlertAlertIntegrationSlack,
+    GetAlertAlertOwner,
+    GetAlertAlertPublishing,
+    GetAlertAlertPublishingElevenLabs,
+    GetAlertAlertPublishSpecification,
+    GetAlertAlertSummarySpecification,
+)
+from .get_collection import (
+    GetCollection,
+    GetCollectionCollection,
+    GetCollectionCollectionContents,
+    GetCollectionCollectionOwner,
+)
+from .get_content import (
+    GetContent,
+    GetContentContent,
+    GetContentContentAudio,
+    GetContentContentChildren,
+    GetContentContentCollections,
+    GetContentContentDocument,
+    GetContentContentEmail,
+    GetContentContentEmailBcc,
+    GetContentContentEmailCc,
+    GetContentContentEmailFrom,
+    GetContentContentEmailTo,
+    GetContentContentFeed,
+    GetContentContentImage,
+    GetContentContentIssue,
+    GetContentContentLinks,
+    GetContentContentObservations,
+    GetContentContentObservationsObservable,
+    GetContentContentObservationsOccurrences,
+    GetContentContentObservationsOccurrencesBoundingBox,
+    GetContentContentOwner,
+    GetContentContentParent,
+    GetContentContentVideo,
+    GetContentContentWorkflow,
+)
+from .get_conversation import (
+    GetConversation,
+    GetConversationConversation,
+    GetConversationConversationFilter,
+    GetConversationConversationFilterCollections,
+    GetConversationConversationFilterContents,
+    GetConversationConversationFilterCreationDateRange,
+    GetConversationConversationFilterDateRange,
+    GetConversationConversationFilterFeeds,
+    GetConversationConversationFilterObservations,
+    GetConversationConversationFilterObservationsObservable,
+    GetConversationConversationFilterWorkflows,
+    GetConversationConversationMessages,
+    GetConversationConversationMessagesCitations,
+    GetConversationConversationMessagesCitationsContent,
+    GetConversationConversationOwner,
+    GetConversationConversationSpecification,
+)
+from .get_feed import (
+    GetFeed,
+    GetFeedFeed,
+    GetFeedFeedDiscord,
+    GetFeedFeedEmail,
+    GetFeedFeedEmailGoogle,
+    GetFeedFeedEmailMicrosoft,
+    GetFeedFeedIssue,
+    GetFeedFeedIssueGithub,
+    GetFeedFeedIssueJira,
+    GetFeedFeedIssueLinear,
+    GetFeedFeedNotion,
+    GetFeedFeedOwner,
+    GetFeedFeedReddit,
+    GetFeedFeedRss,
+    GetFeedFeedSchedulePolicy,
+    GetFeedFeedSite,
+    GetFeedFeedSiteAzureBlob,
+    GetFeedFeedSiteAzureFile,
+    GetFeedFeedSiteGoogle,
+    GetFeedFeedSiteGoogleDrive,
+    GetFeedFeedSiteOneDrive,
+    GetFeedFeedSiteS3,
+    GetFeedFeedSiteSharePoint,
+    GetFeedFeedSlack,
+    GetFeedFeedWeb,
+    GetFeedFeedWorkflow,
+    GetFeedFeedYoutube,
+)
+from .get_project import (
+    GetProject,
+    GetProjectProject,
+    GetProjectProjectQuota,
+    GetProjectProjectSpecification,
+    GetProjectProjectWorkflow,
+)
+from .get_specification import (
+    GetSpecification,
+    GetSpecificationSpecification,
+    GetSpecificationSpecificationAnthropic,
+    GetSpecificationSpecificationAzureOpenAi,
+    GetSpecificationSpecificationOpenAi,
+    GetSpecificationSpecificationOwner,
+    GetSpecificationSpecificationPromptStrategy,
+    GetSpecificationSpecificationReplicate,
+    GetSpecificationSpecificationRerankingStrategy,
+    GetSpecificationSpecificationRetrievalStrategy,
+    GetSpecificationSpecificationStrategy,
+    GetSpecificationSpecificationTools,
+)
+from .get_workflow import (
+    GetWorkflow,
+    GetWorkflowWorkflow,
+    GetWorkflowWorkflowActions,
+    GetWorkflowWorkflowActionsConnector,
+    GetWorkflowWorkflowActionsConnectorSlack,
+    GetWorkflowWorkflowEnrichment,
+    GetWorkflowWorkflowEnrichmentJobs,
+    GetWorkflowWorkflowEnrichmentJobsConnector,
+    GetWorkflowWorkflowEnrichmentLink,
+    GetWorkflowWorkflowExtraction,
+    GetWorkflowWorkflowExtractionJobs,
+    GetWorkflowWorkflowExtractionJobsConnector,
+    GetWorkflowWorkflowExtractionJobsConnectorAzureImage,
+    GetWorkflowWorkflowExtractionJobsConnectorAzureText,
+    GetWorkflowWorkflowExtractionJobsConnectorModelText,
+    GetWorkflowWorkflowExtractionJobsConnectorModelTextSpecification,
+    GetWorkflowWorkflowExtractionJobsConnectorOpenAiImage,
+    GetWorkflowWorkflowIngestion,
+    GetWorkflowWorkflowIngestionCollections,
+    GetWorkflowWorkflowIngestionIf,
+    GetWorkflowWorkflowOwner,
+    GetWorkflowWorkflowPreparation,
+    GetWorkflowWorkflowPreparationJobs,
+    GetWorkflowWorkflowPreparationJobsConnector,
+    GetWorkflowWorkflowPreparationJobsConnectorAzureDocument,
+    GetWorkflowWorkflowPreparationJobsConnectorDeepgram,
+    GetWorkflowWorkflowPreparationJobsConnectorDocument,
+    GetWorkflowWorkflowPreparationJobsConnectorEmail,
+    GetWorkflowWorkflowPreparationSummarizations,
+    GetWorkflowWorkflowPreparationSummarizationsSpecification,
 )
 from .ingest_encoded_file import IngestEncodedFile, IngestEncodedFileIngestEncodedFile
 from .ingest_text import IngestText, IngestTextIngestText
 from .ingest_uri import IngestUri, IngestUriIngestUri
 from .input_types import (
     AddressFilter,
     AddressInput,
@@ -468,20 +521,16 @@
 )
 from .is_content_done import IsContentDone, IsContentDoneIsContentDone
 from .is_feed_done import IsFeedDone, IsFeedDoneIsFeedDone
 from .lookup_credits import LookupCredits, LookupCreditsLookupCredits
 from .lookup_usage import LookupUsage, LookupUsageLookupUsage
 from .operations import (
     ADD_CONTENTS_TO_COLLECTIONS_GQL,
-    ALERT_GQL,
     CLEAR_CONVERSATION_GQL,
     CLOSE_CONVERSATION_GQL,
-    COLLECTION_GQL,
-    CONTENT_GQL,
-    CONVERSATION_GQL,
     CREATE_ALERT_GQL,
     CREATE_COLLECTION_GQL,
     CREATE_CONVERSATION_GQL,
     CREATE_FEED_GQL,
     CREATE_SPECIFICATION_GQL,
     CREATE_WORKFLOW_GQL,
     CREDITS_GQL,
@@ -504,56 +553,53 @@
     DELETE_WORKFLOW_GQL,
     DELETE_WORKFLOWS_GQL,
     DISABLE_ALERT_GQL,
     DISABLE_FEED_GQL,
     ENABLE_ALERT_GQL,
     ENABLE_FEED_GQL,
     EXTRACT_CONTENTS_GQL,
-    FEED_GQL,
+    GET_ALERT_GQL,
+    GET_COLLECTION_GQL,
+    GET_CONTENT_GQL,
+    GET_CONVERSATION_GQL,
+    GET_FEED_GQL,
+    GET_PROJECT_GQL,
+    GET_SPECIFICATION_GQL,
+    GET_WORKFLOW_GQL,
     INGEST_ENCODED_FILE_GQL,
     INGEST_TEXT_GQL,
     INGEST_URI_GQL,
     IS_CONTENT_DONE_GQL,
     IS_FEED_DONE_GQL,
     LOOKUP_CREDITS_GQL,
     LOOKUP_USAGE_GQL,
-    PROJECT_GQL,
     PROMPT_CONVERSATION_GQL,
     PROMPT_SPECIFICATIONS_GQL,
     PUBLISH_CONTENTS_GQL,
     PUBLISH_CONVERSATION_GQL,
     QUERY_ALERTS_GQL,
     QUERY_COLLECTIONS_GQL,
     QUERY_CONTENT_FACETS_GQL,
     QUERY_CONTENTS_GQL,
     QUERY_CONVERSATIONS_GQL,
     QUERY_FEEDS_GQL,
     QUERY_SPECIFICATIONS_GQL,
     QUERY_WORKFLOWS_GQL,
     REMOVE_CONTENTS_FROM_COLLECTION_GQL,
-    SPECIFICATION_GQL,
     SUGGEST_CONVERSATION_GQL,
     SUMMARIZE_CONTENTS_GQL,
     UPDATE_ALERT_GQL,
     UPDATE_COLLECTION_GQL,
     UPDATE_CONTENT_GQL,
     UPDATE_CONVERSATION_GQL,
     UPDATE_FEED_GQL,
     UPDATE_PROJECT_GQL,
     UPDATE_SPECIFICATION_GQL,
     UPDATE_WORKFLOW_GQL,
     USAGE_GQL,
-    WORKFLOW_GQL,
-)
-from .project import (
-    Project,
-    ProjectProject,
-    ProjectProjectQuota,
-    ProjectProjectSpecification,
-    ProjectProjectWorkflow,
 )
 from .prompt_conversation import (
     PromptConversation,
     PromptConversationPromptConversation,
     PromptConversationPromptConversationConversation,
     PromptConversationPromptConversationFacets,
     PromptConversationPromptConversationFacetsObservable,
@@ -735,28 +781,14 @@
     QueryWorkflowsWorkflowsResultsPreparationSummarizationsSpecification,
 )
 from .remove_contents_from_collection import (
     RemoveContentsFromCollection,
     RemoveContentsFromCollectionRemoveContentsFromCollection,
     RemoveContentsFromCollectionRemoveContentsFromCollectionContents,
 )
-from .specification import (
-    Specification,
-    SpecificationSpecification,
-    SpecificationSpecificationAnthropic,
-    SpecificationSpecificationAzureOpenAi,
-    SpecificationSpecificationOpenAi,
-    SpecificationSpecificationOwner,
-    SpecificationSpecificationPromptStrategy,
-    SpecificationSpecificationReplicate,
-    SpecificationSpecificationRerankingStrategy,
-    SpecificationSpecificationRetrievalStrategy,
-    SpecificationSpecificationStrategy,
-    SpecificationSpecificationTools,
-)
 from .suggest_conversation import (
     SuggestConversation,
     SuggestConversationSuggestConversation,
 )
 from .summarize_contents import (
     SummarizeContents,
     SummarizeContentsSummarizeContents,
@@ -805,73 +837,22 @@
     UpdateWorkflowUpdateWorkflowPreparationJobsConnectorDeepgram,
     UpdateWorkflowUpdateWorkflowPreparationJobsConnectorDocument,
     UpdateWorkflowUpdateWorkflowPreparationJobsConnectorEmail,
     UpdateWorkflowUpdateWorkflowPreparationSummarizations,
     UpdateWorkflowUpdateWorkflowPreparationSummarizationsSpecification,
 )
 from .usage import Usage, UsageUsage
-from .workflow import (
-    Workflow,
-    WorkflowWorkflow,
-    WorkflowWorkflowActions,
-    WorkflowWorkflowActionsConnector,
-    WorkflowWorkflowActionsConnectorSlack,
-    WorkflowWorkflowEnrichment,
-    WorkflowWorkflowEnrichmentJobs,
-    WorkflowWorkflowEnrichmentJobsConnector,
-    WorkflowWorkflowEnrichmentLink,
-    WorkflowWorkflowExtraction,
-    WorkflowWorkflowExtractionJobs,
-    WorkflowWorkflowExtractionJobsConnector,
-    WorkflowWorkflowExtractionJobsConnectorAzureImage,
-    WorkflowWorkflowExtractionJobsConnectorAzureText,
-    WorkflowWorkflowExtractionJobsConnectorModelText,
-    WorkflowWorkflowExtractionJobsConnectorModelTextSpecification,
-    WorkflowWorkflowExtractionJobsConnectorOpenAiImage,
-    WorkflowWorkflowIngestion,
-    WorkflowWorkflowIngestionCollections,
-    WorkflowWorkflowIngestionIf,
-    WorkflowWorkflowOwner,
-    WorkflowWorkflowPreparation,
-    WorkflowWorkflowPreparationJobs,
-    WorkflowWorkflowPreparationJobsConnector,
-    WorkflowWorkflowPreparationJobsConnectorAzureDocument,
-    WorkflowWorkflowPreparationJobsConnectorDeepgram,
-    WorkflowWorkflowPreparationJobsConnectorDocument,
-    WorkflowWorkflowPreparationJobsConnectorEmail,
-    WorkflowWorkflowPreparationSummarizations,
-    WorkflowWorkflowPreparationSummarizationsSpecification,
-)
 
 __all__ = [
     "ADD_CONTENTS_TO_COLLECTIONS_GQL",
-    "ALERT_GQL",
     "AddContentsToCollections",
     "AddContentsToCollectionsAddContentsToCollections",
     "AddContentsToCollectionsAddContentsToCollectionsContents",
     "AddressFilter",
     "AddressInput",
-    "Alert",
-    "AlertAlert",
-    "AlertAlertFilter",
-    "AlertAlertFilterCollections",
-    "AlertAlertFilterContents",
-    "AlertAlertFilterCreationDateRange",
-    "AlertAlertFilterDateRange",
-    "AlertAlertFilterFeeds",
-    "AlertAlertFilterObservations",
-    "AlertAlertFilterObservationsObservable",
-    "AlertAlertFilterWorkflows",
-    "AlertAlertIntegration",
-    "AlertAlertIntegrationSlack",
-    "AlertAlertOwner",
-    "AlertAlertPublishSpecification",
-    "AlertAlertPublishing",
-    "AlertAlertPublishingElevenLabs",
-    "AlertAlertSummarySpecification",
     "AlertFilter",
     "AlertInput",
     "AlertSchedulePolicyInput",
     "AlertTypes",
     "AlertUpdateInput",
     "AmazonFeedPropertiesInput",
     "AmazonFeedPropertiesUpdateInput",
@@ -894,17 +875,14 @@
     "AzureOpenAIModels",
     "AzureTextExtractionPropertiesInput",
     "BaseModel",
     "BillableMetrics",
     "BoundingBoxInput",
     "CLEAR_CONVERSATION_GQL",
     "CLOSE_CONVERSATION_GQL",
-    "COLLECTION_GQL",
-    "CONTENT_GQL",
-    "CONVERSATION_GQL",
     "CREATE_ALERT_GQL",
     "CREATE_COLLECTION_GQL",
     "CREATE_CONVERSATION_GQL",
     "CREATE_FEED_GQL",
     "CREATE_SPECIFICATION_GQL",
     "CREATE_WORKFLOW_GQL",
     "CREDITS_GQL",
@@ -914,72 +892,29 @@
     "CategoryInput",
     "CategoryUpdateInput",
     "ClearConversation",
     "ClearConversationClearConversation",
     "Client",
     "CloseConversation",
     "CloseConversationCloseConversation",
-    "Collection",
-    "CollectionCollection",
-    "CollectionCollectionContents",
-    "CollectionCollectionOwner",
     "CollectionFilter",
     "CollectionInput",
     "CollectionTypes",
     "CollectionUpdateInput",
-    "Content",
-    "ContentContent",
-    "ContentContentAudio",
-    "ContentContentChildren",
-    "ContentContentCollections",
-    "ContentContentDocument",
-    "ContentContentEmail",
-    "ContentContentEmailBcc",
-    "ContentContentEmailCc",
-    "ContentContentEmailFrom",
-    "ContentContentEmailTo",
-    "ContentContentFeed",
-    "ContentContentImage",
-    "ContentContentIssue",
-    "ContentContentLinks",
-    "ContentContentObservations",
-    "ContentContentObservationsObservable",
-    "ContentContentObservationsOccurrences",
-    "ContentContentObservationsOccurrencesBoundingBox",
-    "ContentContentOwner",
-    "ContentContentParent",
-    "ContentContentVideo",
-    "ContentContentWorkflow",
     "ContentCriteriaInput",
     "ContentFacetInput",
     "ContentFacetTypes",
     "ContentFilter",
     "ContentInput",
     "ContentPublishingConnectorInput",
     "ContentPublishingConnectorUpdateInput",
     "ContentPublishingFormats",
     "ContentPublishingServiceTypes",
     "ContentTypes",
     "ContentUpdateInput",
-    "Conversation",
-    "ConversationConversation",
-    "ConversationConversationFilter",
-    "ConversationConversationFilterCollections",
-    "ConversationConversationFilterContents",
-    "ConversationConversationFilterCreationDateRange",
-    "ConversationConversationFilterDateRange",
-    "ConversationConversationFilterFeeds",
-    "ConversationConversationFilterObservations",
-    "ConversationConversationFilterObservationsObservable",
-    "ConversationConversationFilterWorkflows",
-    "ConversationConversationMessages",
-    "ConversationConversationMessagesCitations",
-    "ConversationConversationMessagesCitationsContent",
-    "ConversationConversationOwner",
-    "ConversationConversationSpecification",
     "ConversationFilter",
     "ConversationInput",
     "ConversationRoleTypes",
     "ConversationSearchTypes",
     "ConversationStrategyInput",
     "ConversationStrategyTypes",
     "ConversationStrategyUpdateInput",
@@ -1125,54 +1060,169 @@
     "EventUpdateInput",
     "ExtractContents",
     "ExtractContentsExtractContents",
     "ExtractContentsExtractContentsContent",
     "ExtractContentsExtractContentsSpecification",
     "ExtractionWorkflowJobInput",
     "ExtractionWorkflowStageInput",
-    "FEED_GQL",
     "FacetValueTypes",
-    "Feed",
     "FeedConnectorTypes",
-    "FeedFeed",
-    "FeedFeedDiscord",
-    "FeedFeedEmail",
-    "FeedFeedEmailGoogle",
-    "FeedFeedEmailMicrosoft",
-    "FeedFeedIssue",
-    "FeedFeedIssueGithub",
-    "FeedFeedIssueJira",
-    "FeedFeedIssueLinear",
-    "FeedFeedNotion",
-    "FeedFeedOwner",
-    "FeedFeedReddit",
-    "FeedFeedRss",
-    "FeedFeedSchedulePolicy",
-    "FeedFeedSite",
-    "FeedFeedSiteAzureBlob",
-    "FeedFeedSiteAzureFile",
-    "FeedFeedSiteGoogle",
-    "FeedFeedSiteGoogleDrive",
-    "FeedFeedSiteOneDrive",
-    "FeedFeedSiteS3",
-    "FeedFeedSiteSharePoint",
-    "FeedFeedSlack",
-    "FeedFeedWeb",
-    "FeedFeedWorkflow",
-    "FeedFeedYoutube",
     "FeedFilter",
     "FeedInput",
     "FeedListingTypes",
     "FeedSchedulePolicyInput",
     "FeedServiceTypes",
     "FeedTypes",
     "FeedUpdateInput",
     "FilePreparationConnectorInput",
     "FilePreparationServiceTypes",
     "FileTypes",
+    "GET_ALERT_GQL",
+    "GET_COLLECTION_GQL",
+    "GET_CONTENT_GQL",
+    "GET_CONVERSATION_GQL",
+    "GET_FEED_GQL",
+    "GET_PROJECT_GQL",
+    "GET_SPECIFICATION_GQL",
+    "GET_WORKFLOW_GQL",
+    "GetAlert",
+    "GetAlertAlert",
+    "GetAlertAlertFilter",
+    "GetAlertAlertFilterCollections",
+    "GetAlertAlertFilterContents",
+    "GetAlertAlertFilterCreationDateRange",
+    "GetAlertAlertFilterDateRange",
+    "GetAlertAlertFilterFeeds",
+    "GetAlertAlertFilterObservations",
+    "GetAlertAlertFilterObservationsObservable",
+    "GetAlertAlertFilterWorkflows",
+    "GetAlertAlertIntegration",
+    "GetAlertAlertIntegrationSlack",
+    "GetAlertAlertOwner",
+    "GetAlertAlertPublishSpecification",
+    "GetAlertAlertPublishing",
+    "GetAlertAlertPublishingElevenLabs",
+    "GetAlertAlertSummarySpecification",
+    "GetCollection",
+    "GetCollectionCollection",
+    "GetCollectionCollectionContents",
+    "GetCollectionCollectionOwner",
+    "GetContent",
+    "GetContentContent",
+    "GetContentContentAudio",
+    "GetContentContentChildren",
+    "GetContentContentCollections",
+    "GetContentContentDocument",
+    "GetContentContentEmail",
+    "GetContentContentEmailBcc",
+    "GetContentContentEmailCc",
+    "GetContentContentEmailFrom",
+    "GetContentContentEmailTo",
+    "GetContentContentFeed",
+    "GetContentContentImage",
+    "GetContentContentIssue",
+    "GetContentContentLinks",
+    "GetContentContentObservations",
+    "GetContentContentObservationsObservable",
+    "GetContentContentObservationsOccurrences",
+    "GetContentContentObservationsOccurrencesBoundingBox",
+    "GetContentContentOwner",
+    "GetContentContentParent",
+    "GetContentContentVideo",
+    "GetContentContentWorkflow",
+    "GetConversation",
+    "GetConversationConversation",
+    "GetConversationConversationFilter",
+    "GetConversationConversationFilterCollections",
+    "GetConversationConversationFilterContents",
+    "GetConversationConversationFilterCreationDateRange",
+    "GetConversationConversationFilterDateRange",
+    "GetConversationConversationFilterFeeds",
+    "GetConversationConversationFilterObservations",
+    "GetConversationConversationFilterObservationsObservable",
+    "GetConversationConversationFilterWorkflows",
+    "GetConversationConversationMessages",
+    "GetConversationConversationMessagesCitations",
+    "GetConversationConversationMessagesCitationsContent",
+    "GetConversationConversationOwner",
+    "GetConversationConversationSpecification",
+    "GetFeed",
+    "GetFeedFeed",
+    "GetFeedFeedDiscord",
+    "GetFeedFeedEmail",
+    "GetFeedFeedEmailGoogle",
+    "GetFeedFeedEmailMicrosoft",
+    "GetFeedFeedIssue",
+    "GetFeedFeedIssueGithub",
+    "GetFeedFeedIssueJira",
+    "GetFeedFeedIssueLinear",
+    "GetFeedFeedNotion",
+    "GetFeedFeedOwner",
+    "GetFeedFeedReddit",
+    "GetFeedFeedRss",
+    "GetFeedFeedSchedulePolicy",
+    "GetFeedFeedSite",
+    "GetFeedFeedSiteAzureBlob",
+    "GetFeedFeedSiteAzureFile",
+    "GetFeedFeedSiteGoogle",
+    "GetFeedFeedSiteGoogleDrive",
+    "GetFeedFeedSiteOneDrive",
+    "GetFeedFeedSiteS3",
+    "GetFeedFeedSiteSharePoint",
+    "GetFeedFeedSlack",
+    "GetFeedFeedWeb",
+    "GetFeedFeedWorkflow",
+    "GetFeedFeedYoutube",
+    "GetProject",
+    "GetProjectProject",
+    "GetProjectProjectQuota",
+    "GetProjectProjectSpecification",
+    "GetProjectProjectWorkflow",
+    "GetSpecification",
+    "GetSpecificationSpecification",
+    "GetSpecificationSpecificationAnthropic",
+    "GetSpecificationSpecificationAzureOpenAi",
+    "GetSpecificationSpecificationOpenAi",
+    "GetSpecificationSpecificationOwner",
+    "GetSpecificationSpecificationPromptStrategy",
+    "GetSpecificationSpecificationReplicate",
+    "GetSpecificationSpecificationRerankingStrategy",
+    "GetSpecificationSpecificationRetrievalStrategy",
+    "GetSpecificationSpecificationStrategy",
+    "GetSpecificationSpecificationTools",
+    "GetWorkflow",
+    "GetWorkflowWorkflow",
+    "GetWorkflowWorkflowActions",
+    "GetWorkflowWorkflowActionsConnector",
+    "GetWorkflowWorkflowActionsConnectorSlack",
+    "GetWorkflowWorkflowEnrichment",
+    "GetWorkflowWorkflowEnrichmentJobs",
+    "GetWorkflowWorkflowEnrichmentJobsConnector",
+    "GetWorkflowWorkflowEnrichmentLink",
+    "GetWorkflowWorkflowExtraction",
+    "GetWorkflowWorkflowExtractionJobs",
+    "GetWorkflowWorkflowExtractionJobsConnector",
+    "GetWorkflowWorkflowExtractionJobsConnectorAzureImage",
+    "GetWorkflowWorkflowExtractionJobsConnectorAzureText",
+    "GetWorkflowWorkflowExtractionJobsConnectorModelText",
+    "GetWorkflowWorkflowExtractionJobsConnectorModelTextSpecification",
+    "GetWorkflowWorkflowExtractionJobsConnectorOpenAiImage",
+    "GetWorkflowWorkflowIngestion",
+    "GetWorkflowWorkflowIngestionCollections",
+    "GetWorkflowWorkflowIngestionIf",
+    "GetWorkflowWorkflowOwner",
+    "GetWorkflowWorkflowPreparation",
+    "GetWorkflowWorkflowPreparationJobs",
+    "GetWorkflowWorkflowPreparationJobsConnector",
+    "GetWorkflowWorkflowPreparationJobsConnectorAzureDocument",
+    "GetWorkflowWorkflowPreparationJobsConnectorDeepgram",
+    "GetWorkflowWorkflowPreparationJobsConnectorDocument",
+    "GetWorkflowWorkflowPreparationJobsConnectorEmail",
+    "GetWorkflowWorkflowPreparationSummarizations",
+    "GetWorkflowWorkflowPreparationSummarizationsSpecification",
     "GitHubIssuesFeedPropertiesInput",
     "GitHubIssuesFeedPropertiesUpdateInput",
     "GoogleDriveFeedPropertiesInput",
     "GoogleDriveFeedPropertiesUpdateInput",
     "GoogleEmailFeedPropertiesInput",
     "GoogleEmailFeedPropertiesUpdateInput",
     "GoogleFeedPropertiesInput",
@@ -1263,15 +1313,14 @@
     "OrderDirectionTypes",
     "OrganizationFacetInput",
     "OrganizationFacetTypes",
     "OrganizationFilter",
     "OrganizationInput",
     "OrganizationUpdateInput",
     "OrientationTypes",
-    "PROJECT_GQL",
     "PROMPT_CONVERSATION_GQL",
     "PROMPT_SPECIFICATIONS_GQL",
     "PUBLISH_CONTENTS_GQL",
     "PUBLISH_CONVERSATION_GQL",
     "PersonFacetInput",
     "PersonFacetTypes",
     "PersonFilter",
@@ -1288,21 +1337,16 @@
     "PreparationWorkflowJobInput",
     "PreparationWorkflowStageInput",
     "ProductFacetInput",
     "ProductFacetTypes",
     "ProductFilter",
     "ProductInput",
     "ProductUpdateInput",
-    "Project",
     "ProjectFilter",
     "ProjectInput",
-    "ProjectProject",
-    "ProjectProjectQuota",
-    "ProjectProjectSpecification",
-    "ProjectProjectWorkflow",
     "ProjectQuotaInput",
     "ProjectUpdateInput",
     "PromptConversation",
     "PromptConversationPromptConversation",
     "PromptConversationPromptConversationConversation",
     "PromptConversationPromptConversationFacets",
     "PromptConversationPromptConversationFacetsObservable",
@@ -1493,15 +1537,14 @@
     "RepoUpdateInput",
     "RerankingStrategyInput",
     "RerankingStrategyUpdateInput",
     "ResourceConnectorTypes",
     "RetrievalStrategyInput",
     "RetrievalStrategyTypes",
     "RetrievalStrategyUpdateInput",
-    "SPECIFICATION_GQL",
     "SUGGEST_CONVERSATION_GQL",
     "SUMMARIZE_CONTENTS_GQL",
     "SearchQueryTypes",
     "SearchTypes",
     "SharePointAuthenticationTypes",
     "SharePointFeedPropertiesInput",
     "SharePointFeedPropertiesUpdateInput",
@@ -1513,28 +1556,16 @@
     "SlackFeedPropertiesUpdateInput",
     "SlackIntegrationPropertiesInput",
     "SoftwareFacetInput",
     "SoftwareFacetTypes",
     "SoftwareFilter",
     "SoftwareInput",
     "SoftwareUpdateInput",
-    "Specification",
     "SpecificationFilter",
     "SpecificationInput",
-    "SpecificationSpecification",
-    "SpecificationSpecificationAnthropic",
-    "SpecificationSpecificationAzureOpenAi",
-    "SpecificationSpecificationOpenAi",
-    "SpecificationSpecificationOwner",
-    "SpecificationSpecificationPromptStrategy",
-    "SpecificationSpecificationReplicate",
-    "SpecificationSpecificationRerankingStrategy",
-    "SpecificationSpecificationRetrievalStrategy",
-    "SpecificationSpecificationStrategy",
-    "SpecificationSpecificationTools",
     "SpecificationTypes",
     "SpecificationUpdateInput",
     "SuggestConversation",
     "SuggestConversationSuggestConversation",
     "SummarizationStrategyInput",
     "SummarizationTypes",
     "SummarizeContents",
@@ -1600,48 +1631,17 @@
     "UpdateWorkflowUpdateWorkflowPreparationJobsConnectorDocument",
     "UpdateWorkflowUpdateWorkflowPreparationJobsConnectorEmail",
     "UpdateWorkflowUpdateWorkflowPreparationSummarizations",
     "UpdateWorkflowUpdateWorkflowPreparationSummarizationsSpecification",
     "Upload",
     "Usage",
     "UsageUsage",
-    "WORKFLOW_GQL",
     "WebFeedPropertiesInput",
     "WebFeedPropertiesUpdateInput",
-    "Workflow",
     "WorkflowActionInput",
     "WorkflowFilter",
     "WorkflowInput",
     "WorkflowUpdateInput",
-    "WorkflowWorkflow",
-    "WorkflowWorkflowActions",
-    "WorkflowWorkflowActionsConnector",
-    "WorkflowWorkflowActionsConnectorSlack",
-    "WorkflowWorkflowEnrichment",
-    "WorkflowWorkflowEnrichmentJobs",
-    "WorkflowWorkflowEnrichmentJobsConnector",
-    "WorkflowWorkflowEnrichmentLink",
-    "WorkflowWorkflowExtraction",
-    "WorkflowWorkflowExtractionJobs",
-    "WorkflowWorkflowExtractionJobsConnector",
-    "WorkflowWorkflowExtractionJobsConnectorAzureImage",
-    "WorkflowWorkflowExtractionJobsConnectorAzureText",
-    "WorkflowWorkflowExtractionJobsConnectorModelText",
-    "WorkflowWorkflowExtractionJobsConnectorModelTextSpecification",
-    "WorkflowWorkflowExtractionJobsConnectorOpenAiImage",
-    "WorkflowWorkflowIngestion",
-    "WorkflowWorkflowIngestionCollections",
-    "WorkflowWorkflowIngestionIf",
-    "WorkflowWorkflowOwner",
-    "WorkflowWorkflowPreparation",
-    "WorkflowWorkflowPreparationJobs",
-    "WorkflowWorkflowPreparationJobsConnector",
-    "WorkflowWorkflowPreparationJobsConnectorAzureDocument",
-    "WorkflowWorkflowPreparationJobsConnectorDeepgram",
-    "WorkflowWorkflowPreparationJobsConnectorDocument",
-    "WorkflowWorkflowPreparationJobsConnectorEmail",
-    "WorkflowWorkflowPreparationSummarizations",
-    "WorkflowWorkflowPreparationSummarizationsSpecification",
     "YouTubeFeedPropertiesInput",
     "YouTubeFeedPropertiesUpdateInput",
     "YouTubeTypes",
 ]
```

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/add_contents_to_collections.py` & `graphlit_client-1.0.20240420002/graphlit_api/add_contents_to_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/async_base_client.py` & `graphlit_client-1.0.20240420002/graphlit_api/async_base_client.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/base_model.py` & `graphlit_client-1.0.20240420002/graphlit_api/base_model.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/clear_conversation.py` & `graphlit_client-1.0.20240420002/graphlit_api/clear_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/client.py` & `graphlit_client-1.0.20240420002/graphlit_api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 # Generated by ariadne-codegen
 # Source: ./documents
 
 from typing import Any, Dict, List, Optional, Union
 
 from .add_contents_to_collections import AddContentsToCollections
-from .alert import Alert
 from .async_base_client import AsyncBaseClient
 from .base_model import UNSET, UnsetType
 from .clear_conversation import ClearConversation
 from .close_conversation import CloseConversation
-from .collection import Collection
-from .content import Content
-from .conversation import Conversation
 from .create_alert import CreateAlert
 from .create_collection import CreateCollection
 from .create_conversation import CreateConversation
 from .create_feed import CreateFeed
 from .create_specification import CreateSpecification
 from .create_workflow import CreateWorkflow
 from .credits import Credits
@@ -39,15 +35,22 @@
 from .delete_workflows import DeleteWorkflows
 from .disable_alert import DisableAlert
 from .disable_feed import DisableFeed
 from .enable_alert import EnableAlert
 from .enable_feed import EnableFeed
 from .enums import TextTypes
 from .extract_contents import ExtractContents
-from .feed import Feed
+from .get_alert import GetAlert
+from .get_collection import GetCollection
+from .get_content import GetContent
+from .get_conversation import GetConversation
+from .get_feed import GetFeed
+from .get_project import GetProject
+from .get_specification import GetSpecification
+from .get_workflow import GetWorkflow
 from .ingest_encoded_file import IngestEncodedFile
 from .ingest_text import IngestText
 from .ingest_uri import IngestUri
 from .input_types import (
     AlertFilter,
     AlertInput,
     AlertUpdateInput,
@@ -76,20 +79,16 @@
 )
 from .is_content_done import IsContentDone
 from .is_feed_done import IsFeedDone
 from .lookup_credits import LookupCredits
 from .lookup_usage import LookupUsage
 from .operations import (
     ADD_CONTENTS_TO_COLLECTIONS_GQL,
-    ALERT_GQL,
     CLEAR_CONVERSATION_GQL,
     CLOSE_CONVERSATION_GQL,
-    COLLECTION_GQL,
-    CONTENT_GQL,
-    CONVERSATION_GQL,
     CREATE_ALERT_GQL,
     CREATE_COLLECTION_GQL,
     CREATE_CONVERSATION_GQL,
     CREATE_FEED_GQL,
     CREATE_SPECIFICATION_GQL,
     CREATE_WORKFLOW_GQL,
     CREDITS_GQL,
@@ -112,77 +111,78 @@
     DELETE_WORKFLOW_GQL,
     DELETE_WORKFLOWS_GQL,
     DISABLE_ALERT_GQL,
     DISABLE_FEED_GQL,
     ENABLE_ALERT_GQL,
     ENABLE_FEED_GQL,
     EXTRACT_CONTENTS_GQL,
-    FEED_GQL,
+    GET_ALERT_GQL,
+    GET_COLLECTION_GQL,
+    GET_CONTENT_GQL,
+    GET_CONVERSATION_GQL,
+    GET_FEED_GQL,
+    GET_PROJECT_GQL,
+    GET_SPECIFICATION_GQL,
+    GET_WORKFLOW_GQL,
     INGEST_ENCODED_FILE_GQL,
     INGEST_TEXT_GQL,
     INGEST_URI_GQL,
     IS_CONTENT_DONE_GQL,
     IS_FEED_DONE_GQL,
     LOOKUP_CREDITS_GQL,
     LOOKUP_USAGE_GQL,
-    PROJECT_GQL,
     PROMPT_CONVERSATION_GQL,
     PROMPT_SPECIFICATIONS_GQL,
     PUBLISH_CONTENTS_GQL,
     PUBLISH_CONVERSATION_GQL,
     QUERY_ALERTS_GQL,
     QUERY_COLLECTIONS_GQL,
     QUERY_CONTENT_FACETS_GQL,
     QUERY_CONTENTS_GQL,
     QUERY_CONVERSATIONS_GQL,
     QUERY_FEEDS_GQL,
     QUERY_SPECIFICATIONS_GQL,
     QUERY_WORKFLOWS_GQL,
     REMOVE_CONTENTS_FROM_COLLECTION_GQL,
-    SPECIFICATION_GQL,
     SUGGEST_CONVERSATION_GQL,
     SUMMARIZE_CONTENTS_GQL,
     UPDATE_ALERT_GQL,
     UPDATE_COLLECTION_GQL,
     UPDATE_CONTENT_GQL,
     UPDATE_CONVERSATION_GQL,
     UPDATE_FEED_GQL,
     UPDATE_PROJECT_GQL,
     UPDATE_SPECIFICATION_GQL,
     UPDATE_WORKFLOW_GQL,
     USAGE_GQL,
-    WORKFLOW_GQL,
 )
-from .project import Project
 from .prompt_conversation import PromptConversation
 from .prompt_specifications import PromptSpecifications
 from .publish_contents import PublishContents
 from .publish_conversation import PublishConversation
 from .query_alerts import QueryAlerts
 from .query_collections import QueryCollections
 from .query_content_facets import QueryContentFacets
 from .query_contents import QueryContents
 from .query_conversations import QueryConversations
 from .query_feeds import QueryFeeds
 from .query_specifications import QuerySpecifications
 from .query_workflows import QueryWorkflows
 from .remove_contents_from_collection import RemoveContentsFromCollection
-from .specification import Specification
 from .suggest_conversation import SuggestConversation
 from .summarize_contents import SummarizeContents
 from .update_alert import UpdateAlert
 from .update_collection import UpdateCollection
 from .update_content import UpdateContent
 from .update_conversation import UpdateConversation
 from .update_feed import UpdateFeed
 from .update_project import UpdateProject
 from .update_specification import UpdateSpecification
 from .update_workflow import UpdateWorkflow
 from .usage import Usage
-from .workflow import Workflow
 
 
 def gql(q: str) -> str:
     return q
 
 
 class Client(AsyncBaseClient):
@@ -253,21 +253,24 @@
             operation_name="EnableAlert",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return EnableAlert.model_validate(data)
 
-    async def get_alert(self, id: str, **kwargs: Any) -> Alert:
+    async def get_alert(self, id: str, **kwargs: Any) -> GetAlert:
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
-            query=ALERT_GQL, operation_name="Alert", variables=variables, **kwargs
+            query=GET_ALERT_GQL,
+            operation_name="GetAlert",
+            variables=variables,
+            **kwargs
         )
         data = self.get_data(response)
-        return Alert.model_validate(data)
+        return GetAlert.model_validate(data)
 
     async def query_alerts(
         self, filter: Union[Optional[AlertFilter], UnsetType] = UNSET, **kwargs: Any
     ) -> QueryAlerts:
         variables: Dict[str, object] = {"filter": filter}
         response = await self.execute(
             query=QUERY_ALERTS_GQL,
@@ -341,24 +344,24 @@
             operation_name="DeleteCollections",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteCollections.model_validate(data)
 
-    async def get_collection(self, id: str, **kwargs: Any) -> Collection:
+    async def get_collection(self, id: str, **kwargs: Any) -> GetCollection:
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
-            query=COLLECTION_GQL,
-            operation_name="Collection",
+            query=GET_COLLECTION_GQL,
+            operation_name="GetCollection",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
-        return Collection.model_validate(data)
+        return GetCollection.model_validate(data)
 
     async def query_collections(
         self,
         filter: Union[Optional[CollectionFilter], UnsetType] = UNSET,
         **kwargs: Any
     ) -> QueryCollections:
         variables: Dict[str, object] = {"filter": filter}
@@ -452,21 +455,24 @@
             operation_name="ExtractContents",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return ExtractContents.model_validate(data)
 
-    async def get_content(self, id: str, **kwargs: Any) -> Content:
+    async def get_content(self, id: str, **kwargs: Any) -> GetContent:
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
-            query=CONTENT_GQL, operation_name="Content", variables=variables, **kwargs
+            query=GET_CONTENT_GQL,
+            operation_name="GetContent",
+            variables=variables,
+            **kwargs
         )
         data = self.get_data(response)
-        return Content.model_validate(data)
+        return GetContent.model_validate(data)
 
     async def ingest_encoded_file(
         self,
         name: str,
         data: str,
         mime_type: str,
         id: Union[Optional[str], UnsetType] = UNSET,
@@ -730,24 +736,24 @@
             operation_name="DeleteConversations",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteConversations.model_validate(data)
 
-    async def get_conversation(self, id: str, **kwargs: Any) -> Conversation:
+    async def get_conversation(self, id: str, **kwargs: Any) -> GetConversation:
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
-            query=CONVERSATION_GQL,
-            operation_name="Conversation",
+            query=GET_CONVERSATION_GQL,
+            operation_name="GetConversation",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
-        return Conversation.model_validate(data)
+        return GetConversation.model_validate(data)
 
     async def prompt_conversation(
         self,
         prompt: str,
         id: Union[Optional[str], UnsetType] = UNSET,
         correlation_id: Union[Optional[str], UnsetType] = UNSET,
         **kwargs: Any
@@ -907,21 +913,21 @@
             operation_name="EnableFeed",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return EnableFeed.model_validate(data)
 
-    async def get_feed(self, id: str, **kwargs: Any) -> Feed:
+    async def get_feed(self, id: str, **kwargs: Any) -> GetFeed:
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
-            query=FEED_GQL, operation_name="Feed", variables=variables, **kwargs
+            query=GET_FEED_GQL, operation_name="GetFeed", variables=variables, **kwargs
         )
         data = self.get_data(response)
-        return Feed.model_validate(data)
+        return GetFeed.model_validate(data)
 
     async def is_feed_done(self, id: str, **kwargs: Any) -> IsFeedDone:
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
             query=IS_FEED_DONE_GQL,
             operation_name="IsFeedDone",
             variables=variables,
@@ -958,14 +964,25 @@
         variables: Dict[str, object] = {"startDate": start_date, "duration": duration}
         response = await self.execute(
             query=CREDITS_GQL, operation_name="Credits", variables=variables, **kwargs
         )
         data = self.get_data(response)
         return Credits.model_validate(data)
 
+    async def get_project(self, **kwargs: Any) -> GetProject:
+        variables: Dict[str, object] = {}
+        response = await self.execute(
+            query=GET_PROJECT_GQL,
+            operation_name="GetProject",
+            variables=variables,
+            **kwargs
+        )
+        data = self.get_data(response)
+        return GetProject.model_validate(data)
+
     async def lookup_credits(self, correlation_id: str, **kwargs: Any) -> LookupCredits:
         variables: Dict[str, object] = {"correlationId": correlation_id}
         response = await self.execute(
             query=LOOKUP_CREDITS_GQL,
             operation_name="LookupCredits",
             variables=variables,
             **kwargs
@@ -980,22 +997,14 @@
             operation_name="LookupUsage",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return LookupUsage.model_validate(data)
 
-    async def get_project(self, **kwargs: Any) -> Project:
-        variables: Dict[str, object] = {}
-        response = await self.execute(
-            query=PROJECT_GQL, operation_name="Project", variables=variables, **kwargs
-        )
-        data = self.get_data(response)
-        return Project.model_validate(data)
-
     async def update_project(
         self, project: ProjectUpdateInput, **kwargs: Any
     ) -> UpdateProject:
         variables: Dict[str, object] = {"project": project}
         response = await self.execute(
             query=UPDATE_PROJECT_GQL,
             operation_name="UpdateProject",
@@ -1033,24 +1042,24 @@
             operation_name="DeleteSpecification",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteSpecification.model_validate(data)
 
-    async def get_specification(self, id: str, **kwargs: Any) -> Specification:
+    async def get_specification(self, id: str, **kwargs: Any) -> GetSpecification:
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
-            query=SPECIFICATION_GQL,
-            operation_name="Specification",
+            query=GET_SPECIFICATION_GQL,
+            operation_name="GetSpecification",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
-        return Specification.model_validate(data)
+        return GetSpecification.model_validate(data)
 
     async def prompt_specifications(
         self, prompt: str, ids: List[str], **kwargs: Any
     ) -> PromptSpecifications:
         variables: Dict[str, object] = {"prompt": prompt, "ids": ids}
         response = await self.execute(
             query=PROMPT_SPECIFICATIONS_GQL,
@@ -1131,21 +1140,24 @@
             operation_name="DeleteWorkflows",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteWorkflows.model_validate(data)
 
-    async def get_workflow(self, id: str, **kwargs: Any) -> Workflow:
+    async def get_workflow(self, id: str, **kwargs: Any) -> GetWorkflow:
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
-            query=WORKFLOW_GQL, operation_name="Workflow", variables=variables, **kwargs
+            query=GET_WORKFLOW_GQL,
+            operation_name="GetWorkflow",
+            variables=variables,
+            **kwargs
         )
         data = self.get_data(response)
-        return Workflow.model_validate(data)
+        return GetWorkflow.model_validate(data)
 
     async def query_workflows(
         self, filter: Union[Optional[WorkflowFilter], UnsetType] = UNSET, **kwargs: Any
     ) -> QueryWorkflows:
         variables: Dict[str, object] = {"filter": filter}
         response = await self.execute(
             query=QUERY_WORKFLOWS_GQL,
```

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/close_conversation.py` & `graphlit_client-1.0.20240420002/graphlit_api/close_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/collection.py` & `graphlit_client-1.0.20240420002/graphlit_api/create_collection.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,25 @@
 # Generated by ariadne-codegen
 # Source: ./documents
 
-from typing import Any, List, Optional
+from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import CollectionTypes, EntityState
 
 
-class Collection(BaseModel):
-    collection: Optional["CollectionCollection"]
+class CreateCollection(BaseModel):
+    create_collection: Optional["CreateCollectionCreateCollection"] = Field(
+        alias="createCollection"
+    )
 
 
-class CollectionCollection(BaseModel):
+class CreateCollectionCreateCollection(BaseModel):
     id: str
     name: str
-    creation_date: Any = Field(alias="creationDate")
-    owner: "CollectionCollectionOwner"
     state: EntityState
     type: Optional[CollectionTypes]
-    contents: Optional[List[Optional["CollectionCollectionContents"]]]
 
 
-class CollectionCollectionOwner(BaseModel):
-    id: str
-
-
-class CollectionCollectionContents(BaseModel):
-    id: str
-    name: str
-
-
-Collection.model_rebuild()
-CollectionCollection.model_rebuild()
+CreateCollection.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/content.py` & `graphlit_client-1.0.20240420002/graphlit_api/get_content.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     MailPriority,
     MailSensitivity,
     ObservableTypes,
     OccurrenceTypes,
 )
 
 
-class Content(BaseModel):
-    content: Optional["ContentContent"]
+class GetContent(BaseModel):
+    content: Optional["GetContentContent"]
 
 
-class ContentContent(BaseModel):
+class GetContentContent(BaseModel):
     id: str
     name: str
     creation_date: Any = Field(alias="creationDate")
-    owner: "ContentContentOwner"
+    owner: "GetContentContentOwner"
     state: EntityState
     original_date: Optional[Any] = Field(alias="originalDate")
     finished_date: Optional[Any] = Field(alias="finishedDate")
     workflow_duration: Optional[Any] = Field(alias="workflowDuration")
     uri: Optional[Any]
     type: Optional[ContentTypes]
     file_type: Optional[FileTypes] = Field(alias="fileType")
@@ -39,45 +39,45 @@
     file_name: Optional[str] = Field(alias="fileName")
     file_size: Optional[Any] = Field(alias="fileSize")
     master_uri: Optional[Any] = Field(alias="masterUri")
     image_uri: Optional[Any] = Field(alias="imageUri")
     text_uri: Optional[Any] = Field(alias="textUri")
     audio_uri: Optional[Any] = Field(alias="audioUri")
     transcript_uri: Optional[Any] = Field(alias="transcriptUri")
-    video: Optional["ContentContentVideo"]
-    audio: Optional["ContentContentAudio"]
-    image: Optional["ContentContentImage"]
-    document: Optional["ContentContentDocument"]
-    email: Optional["ContentContentEmail"]
-    issue: Optional["ContentContentIssue"]
-    observations: Optional[List[Optional["ContentContentObservations"]]]
-    parent: Optional["ContentContentParent"]
-    children: Optional[List[Optional["ContentContentChildren"]]]
-    collections: Optional[List[Optional["ContentContentCollections"]]]
-    feed: Optional["ContentContentFeed"]
-    workflow: Optional["ContentContentWorkflow"]
+    video: Optional["GetContentContentVideo"]
+    audio: Optional["GetContentContentAudio"]
+    image: Optional["GetContentContentImage"]
+    document: Optional["GetContentContentDocument"]
+    email: Optional["GetContentContentEmail"]
+    issue: Optional["GetContentContentIssue"]
+    observations: Optional[List[Optional["GetContentContentObservations"]]]
+    parent: Optional["GetContentContentParent"]
+    children: Optional[List[Optional["GetContentContentChildren"]]]
+    collections: Optional[List[Optional["GetContentContentCollections"]]]
+    feed: Optional["GetContentContentFeed"]
+    workflow: Optional["GetContentContentWorkflow"]
     markdown: Optional[str]
-    links: Optional[List["ContentContentLinks"]]
+    links: Optional[List["GetContentContentLinks"]]
     error: Optional[str]
 
 
-class ContentContentOwner(BaseModel):
+class GetContentContentOwner(BaseModel):
     id: str
 
 
-class ContentContentVideo(BaseModel):
+class GetContentContentVideo(BaseModel):
     width: Optional[int]
     height: Optional[int]
     duration: Optional[str]
     software: Optional[str]
     make: Optional[str]
     model: Optional[str]
 
 
-class ContentContentAudio(BaseModel):
+class GetContentContentAudio(BaseModel):
     keywords: Optional[List[Optional[str]]]
     author: Optional[str]
     series: Optional[str]
     episode: Optional[str]
     episode_type: Optional[str] = Field(alias="episodeType")
     season: Optional[str]
     publisher: Optional[str]
@@ -88,25 +88,25 @@
     bitrate: Optional[int]
     channels: Optional[int]
     sample_rate: Optional[int] = Field(alias="sampleRate")
     bits_per_sample: Optional[int] = Field(alias="bitsPerSample")
     duration: Optional[str]
 
 
-class ContentContentImage(BaseModel):
+class GetContentContentImage(BaseModel):
     width: Optional[int]
     height: Optional[int]
     description: Optional[str]
     software: Optional[str]
     identifier: Optional[str]
     make: Optional[str]
     model: Optional[str]
 
 
-class ContentContentDocument(BaseModel):
+class GetContentContentDocument(BaseModel):
     title: Optional[str]
     subject: Optional[str]
     author: Optional[str]
     software: Optional[str]
     publisher: Optional[str]
     description: Optional[str]
     summary: Optional[str]
@@ -118,118 +118,118 @@
     line_count: Optional[int] = Field(alias="lineCount")
     paragraph_count: Optional[int] = Field(alias="paragraphCount")
     character_count: Optional[int] = Field(alias="characterCount")
     is_encrypted: Optional[bool] = Field(alias="isEncrypted")
     has_digital_signature: Optional[bool] = Field(alias="hasDigitalSignature")
 
 
-class ContentContentEmail(BaseModel):
+class GetContentContentEmail(BaseModel):
     subject: Optional[str]
     identifier: Optional[str]
     sensitivity: Optional[MailSensitivity]
     priority: Optional[MailPriority]
     importance: Optional[MailImportance]
     labels: Optional[List[Optional[str]]]
-    from_: Optional[List[Optional["ContentContentEmailFrom"]]] = Field(alias="from")
-    to: Optional[List[Optional["ContentContentEmailTo"]]]
-    cc: Optional[List[Optional["ContentContentEmailCc"]]]
-    bcc: Optional[List[Optional["ContentContentEmailBcc"]]]
+    from_: Optional[List[Optional["GetContentContentEmailFrom"]]] = Field(alias="from")
+    to: Optional[List[Optional["GetContentContentEmailTo"]]]
+    cc: Optional[List[Optional["GetContentContentEmailCc"]]]
+    bcc: Optional[List[Optional["GetContentContentEmailBcc"]]]
 
 
-class ContentContentEmailFrom(BaseModel):
+class GetContentContentEmailFrom(BaseModel):
     name: Optional[str]
     family_name: Optional[str] = Field(alias="familyName")
     given_name: Optional[str] = Field(alias="givenName")
     email: Optional[str]
 
 
-class ContentContentEmailTo(BaseModel):
+class GetContentContentEmailTo(BaseModel):
     name: Optional[str]
     family_name: Optional[str] = Field(alias="familyName")
     given_name: Optional[str] = Field(alias="givenName")
     email: Optional[str]
 
 
-class ContentContentEmailCc(BaseModel):
+class GetContentContentEmailCc(BaseModel):
     name: Optional[str]
     family_name: Optional[str] = Field(alias="familyName")
     given_name: Optional[str] = Field(alias="givenName")
     email: Optional[str]
 
 
-class ContentContentEmailBcc(BaseModel):
+class GetContentContentEmailBcc(BaseModel):
     name: Optional[str]
     family_name: Optional[str] = Field(alias="familyName")
     given_name: Optional[str] = Field(alias="givenName")
     email: Optional[str]
 
 
-class ContentContentIssue(BaseModel):
+class GetContentContentIssue(BaseModel):
     title: Optional[str]
     project: Optional[str]
     team: Optional[str]
     status: Optional[str]
     priority: Optional[str]
     type: Optional[str]
     identifier: Optional[str]
     labels: Optional[List[Optional[str]]]
 
 
-class ContentContentObservations(BaseModel):
+class GetContentContentObservations(BaseModel):
     type: ObservableTypes
-    observable: "ContentContentObservationsObservable"
-    occurrences: Optional[List[Optional["ContentContentObservationsOccurrences"]]]
+    observable: "GetContentContentObservationsObservable"
+    occurrences: Optional[List[Optional["GetContentContentObservationsOccurrences"]]]
 
 
-class ContentContentObservationsObservable(BaseModel):
+class GetContentContentObservationsObservable(BaseModel):
     id: str
     name: Optional[str]
 
 
-class ContentContentObservationsOccurrences(BaseModel):
+class GetContentContentObservationsOccurrences(BaseModel):
     type: Optional[OccurrenceTypes]
     confidence: Optional[float]
-    bounding_box: Optional["ContentContentObservationsOccurrencesBoundingBox"] = Field(
-        alias="boundingBox"
+    bounding_box: Optional["GetContentContentObservationsOccurrencesBoundingBox"] = (
+        Field(alias="boundingBox")
     )
     page_index: Optional[int] = Field(alias="pageIndex")
     start_time: Optional[Any] = Field(alias="startTime")
     end_time: Optional[Any] = Field(alias="endTime")
 
 
-class ContentContentObservationsOccurrencesBoundingBox(BaseModel):
+class GetContentContentObservationsOccurrencesBoundingBox(BaseModel):
     left: Optional[float]
     top: Optional[float]
     width: Optional[float]
     height: Optional[float]
 
 
-class ContentContentParent(BaseModel):
+class GetContentContentParent(BaseModel):
     id: str
 
 
-class ContentContentChildren(BaseModel):
+class GetContentContentChildren(BaseModel):
     id: str
 
 
-class ContentContentCollections(BaseModel):
+class GetContentContentCollections(BaseModel):
     id: str
 
 
-class ContentContentFeed(BaseModel):
+class GetContentContentFeed(BaseModel):
     id: str
 
 
-class ContentContentWorkflow(BaseModel):
+class GetContentContentWorkflow(BaseModel):
     id: str
 
 
-class ContentContentLinks(BaseModel):
+class GetContentContentLinks(BaseModel):
     uri: Optional[Any]
     link_type: Optional[LinkTypes] = Field(alias="linkType")
 
 
-Content.model_rebuild()
-ContentContent.model_rebuild()
-ContentContentEmail.model_rebuild()
-ContentContentObservations.model_rebuild()
-ContentContentObservationsOccurrences.model_rebuild()
+GetContent.model_rebuild()
+GetContentContent.model_rebuild()
+GetContentContentEmail.model_rebuild()
+GetContentContentObservations.model_rebuild()
+GetContentContentObservationsOccurrences.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/conversation.py` & `graphlit_client-1.0.20240420002/graphlit_api/get_conversation.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,118 +13,118 @@
     EntityState,
     FileTypes,
     ModelServiceTypes,
     ObservableTypes,
 )
 
 
-class Conversation(BaseModel):
-    conversation: Optional["ConversationConversation"]
+class GetConversation(BaseModel):
+    conversation: Optional["GetConversationConversation"]
 
 
-class ConversationConversation(BaseModel):
+class GetConversationConversation(BaseModel):
     id: str
     name: str
     creation_date: Any = Field(alias="creationDate")
-    owner: "ConversationConversationOwner"
+    owner: "GetConversationConversationOwner"
     state: EntityState
     correlation_id: Optional[str] = Field(alias="correlationId")
     type: Optional[ConversationTypes]
-    messages: Optional[List[Optional["ConversationConversationMessages"]]]
-    specification: Optional["ConversationConversationSpecification"]
-    filter: Optional["ConversationConversationFilter"]
+    messages: Optional[List[Optional["GetConversationConversationMessages"]]]
+    specification: Optional["GetConversationConversationSpecification"]
+    filter: Optional["GetConversationConversationFilter"]
 
 
-class ConversationConversationOwner(BaseModel):
+class GetConversationConversationOwner(BaseModel):
     id: str
 
 
-class ConversationConversationMessages(BaseModel):
+class GetConversationConversationMessages(BaseModel):
     role: ConversationRoleTypes
     author: Optional[str]
     message: str
-    citations: Optional[List[Optional["ConversationConversationMessagesCitations"]]]
+    citations: Optional[List[Optional["GetConversationConversationMessagesCitations"]]]
     tokens: int
     throughput: Optional[float]
     completion_time: Optional[Any] = Field(alias="completionTime")
     timestamp: Any
     model_service: Optional[ModelServiceTypes] = Field(alias="modelService")
     model: Optional[str]
 
 
-class ConversationConversationMessagesCitations(BaseModel):
-    content: Optional["ConversationConversationMessagesCitationsContent"]
+class GetConversationConversationMessagesCitations(BaseModel):
+    content: Optional["GetConversationConversationMessagesCitationsContent"]
     index: Optional[int]
     text: Optional[str]
     start_time: Optional[Any] = Field(alias="startTime")
     end_time: Optional[Any] = Field(alias="endTime")
     page_number: Optional[int] = Field(alias="pageNumber")
     frame_number: Optional[int] = Field(alias="frameNumber")
 
 
-class ConversationConversationMessagesCitationsContent(BaseModel):
+class GetConversationConversationMessagesCitationsContent(BaseModel):
     id: str
 
 
-class ConversationConversationSpecification(BaseModel):
+class GetConversationConversationSpecification(BaseModel):
     id: str
     name: str
 
 
-class ConversationConversationFilter(BaseModel):
-    date_range: Optional["ConversationConversationFilterDateRange"] = Field(
+class GetConversationConversationFilter(BaseModel):
+    date_range: Optional["GetConversationConversationFilterDateRange"] = Field(
         alias="dateRange"
     )
-    creation_date_range: Optional["ConversationConversationFilterCreationDateRange"] = (
-        Field(alias="creationDateRange")
-    )
+    creation_date_range: Optional[
+        "GetConversationConversationFilterCreationDateRange"
+    ] = Field(alias="creationDateRange")
     types: Optional[List[ContentTypes]]
     file_types: Optional[List[Optional[FileTypes]]] = Field(alias="fileTypes")
-    contents: Optional[List["ConversationConversationFilterContents"]]
-    feeds: Optional[List["ConversationConversationFilterFeeds"]]
-    workflows: Optional[List["ConversationConversationFilterWorkflows"]]
-    collections: Optional[List["ConversationConversationFilterCollections"]]
-    observations: Optional[List["ConversationConversationFilterObservations"]]
+    contents: Optional[List["GetConversationConversationFilterContents"]]
+    feeds: Optional[List["GetConversationConversationFilterFeeds"]]
+    workflows: Optional[List["GetConversationConversationFilterWorkflows"]]
+    collections: Optional[List["GetConversationConversationFilterCollections"]]
+    observations: Optional[List["GetConversationConversationFilterObservations"]]
 
 
-class ConversationConversationFilterDateRange(BaseModel):
+class GetConversationConversationFilterDateRange(BaseModel):
     from_: Optional[Any] = Field(alias="from")
     to: Optional[Any]
 
 
-class ConversationConversationFilterCreationDateRange(BaseModel):
+class GetConversationConversationFilterCreationDateRange(BaseModel):
     from_: Optional[Any] = Field(alias="from")
     to: Optional[Any]
 
 
-class ConversationConversationFilterContents(BaseModel):
+class GetConversationConversationFilterContents(BaseModel):
     id: str
 
 
-class ConversationConversationFilterFeeds(BaseModel):
+class GetConversationConversationFilterFeeds(BaseModel):
     id: str
 
 
-class ConversationConversationFilterWorkflows(BaseModel):
+class GetConversationConversationFilterWorkflows(BaseModel):
     id: str
 
 
-class ConversationConversationFilterCollections(BaseModel):
+class GetConversationConversationFilterCollections(BaseModel):
     id: str
 
 
-class ConversationConversationFilterObservations(BaseModel):
+class GetConversationConversationFilterObservations(BaseModel):
     type: ObservableTypes
-    observable: "ConversationConversationFilterObservationsObservable"
+    observable: "GetConversationConversationFilterObservationsObservable"
     states: Optional[List[Optional[EntityState]]]
 
 
-class ConversationConversationFilterObservationsObservable(BaseModel):
+class GetConversationConversationFilterObservationsObservable(BaseModel):
     id: str
 
 
-Conversation.model_rebuild()
-ConversationConversation.model_rebuild()
-ConversationConversationMessages.model_rebuild()
-ConversationConversationMessagesCitations.model_rebuild()
-ConversationConversationFilter.model_rebuild()
-ConversationConversationFilterObservations.model_rebuild()
+GetConversation.model_rebuild()
+GetConversationConversation.model_rebuild()
+GetConversationConversationMessages.model_rebuild()
+GetConversationConversationMessagesCitations.model_rebuild()
+GetConversationConversationFilter.model_rebuild()
+GetConversationConversationFilterObservations.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/create_collection.py` & `graphlit_client-1.0.20240420002/graphlit_api/update_collection.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import CollectionTypes, EntityState
 
 
-class CreateCollection(BaseModel):
-    create_collection: Optional["CreateCollectionCreateCollection"] = Field(
-        alias="createCollection"
+class UpdateCollection(BaseModel):
+    update_collection: Optional["UpdateCollectionUpdateCollection"] = Field(
+        alias="updateCollection"
     )
 
 
-class CreateCollectionCreateCollection(BaseModel):
+class UpdateCollectionUpdateCollection(BaseModel):
     id: str
     name: str
     state: EntityState
     type: Optional[CollectionTypes]
 
 
-CreateCollection.model_rebuild()
+UpdateCollection.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/create_conversation.py` & `graphlit_client-1.0.20240420002/graphlit_api/create_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/create_specification.py` & `graphlit_client-1.0.20240420002/graphlit_api/create_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/create_workflow.py` & `graphlit_client-1.0.20240420002/graphlit_api/create_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/credits.py` & `graphlit_client-1.0.20240420002/graphlit_api/credits.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/delete_all_conversations.py` & `graphlit_client-1.0.20240420002/graphlit_api/delete_all_conversations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/enums.py` & `graphlit_client-1.0.20240420002/graphlit_api/enums.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/exceptions.py` & `graphlit_client-1.0.20240420002/graphlit_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/extract_contents.py` & `graphlit_client-1.0.20240420002/graphlit_api/extract_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/feed.py` & `graphlit_client-1.0.20240420002/graphlit_api/get_feed.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,213 +16,215 @@
     SharePointAuthenticationTypes,
     SiteTypes,
     TimedPolicyRecurrenceTypes,
     YouTubeTypes,
 )
 
 
-class Feed(BaseModel):
-    feed: Optional["FeedFeed"]
+class GetFeed(BaseModel):
+    feed: Optional["GetFeedFeed"]
 
 
-class FeedFeed(BaseModel):
+class GetFeedFeed(BaseModel):
     id: str
     name: str
     creation_date: Any = Field(alias="creationDate")
-    owner: "FeedFeedOwner"
+    owner: "GetFeedFeedOwner"
     state: EntityState
     correlation_id: Optional[str] = Field(alias="correlationId")
     type: FeedTypes
-    site: Optional["FeedFeedSite"]
-    email: Optional["FeedFeedEmail"]
-    issue: Optional["FeedFeedIssue"]
-    rss: Optional["FeedFeedRss"]
-    web: Optional["FeedFeedWeb"]
-    reddit: Optional["FeedFeedReddit"]
-    notion: Optional["FeedFeedNotion"]
-    youtube: Optional["FeedFeedYoutube"]
-    slack: Optional["FeedFeedSlack"]
-    discord: Optional["FeedFeedDiscord"]
+    site: Optional["GetFeedFeedSite"]
+    email: Optional["GetFeedFeedEmail"]
+    issue: Optional["GetFeedFeedIssue"]
+    rss: Optional["GetFeedFeedRss"]
+    web: Optional["GetFeedFeedWeb"]
+    reddit: Optional["GetFeedFeedReddit"]
+    notion: Optional["GetFeedFeedNotion"]
+    youtube: Optional["GetFeedFeedYoutube"]
+    slack: Optional["GetFeedFeedSlack"]
+    discord: Optional["GetFeedFeedDiscord"]
     error: Optional[str]
     last_post_date: Optional[Any] = Field(alias="lastPostDate")
     last_read_date: Optional[Any] = Field(alias="lastReadDate")
     read_count: Optional[int] = Field(alias="readCount")
-    workflow: Optional["FeedFeedWorkflow"]
-    schedule_policy: Optional["FeedFeedSchedulePolicy"] = Field(alias="schedulePolicy")
+    workflow: Optional["GetFeedFeedWorkflow"]
+    schedule_policy: Optional["GetFeedFeedSchedulePolicy"] = Field(
+        alias="schedulePolicy"
+    )
 
 
-class FeedFeedOwner(BaseModel):
+class GetFeedFeedOwner(BaseModel):
     id: str
 
 
-class FeedFeedSite(BaseModel):
+class GetFeedFeedSite(BaseModel):
     site_type: SiteTypes = Field(alias="siteType")
     type: FeedServiceTypes
     is_recursive: Optional[bool] = Field(alias="isRecursive")
-    s_3: Optional["FeedFeedSiteS3"] = Field(alias="s3")
-    azure_blob: Optional["FeedFeedSiteAzureBlob"] = Field(alias="azureBlob")
-    azure_file: Optional["FeedFeedSiteAzureFile"] = Field(alias="azureFile")
-    google: Optional["FeedFeedSiteGoogle"]
-    share_point: Optional["FeedFeedSiteSharePoint"] = Field(alias="sharePoint")
-    one_drive: Optional["FeedFeedSiteOneDrive"] = Field(alias="oneDrive")
-    google_drive: Optional["FeedFeedSiteGoogleDrive"] = Field(alias="googleDrive")
+    s_3: Optional["GetFeedFeedSiteS3"] = Field(alias="s3")
+    azure_blob: Optional["GetFeedFeedSiteAzureBlob"] = Field(alias="azureBlob")
+    azure_file: Optional["GetFeedFeedSiteAzureFile"] = Field(alias="azureFile")
+    google: Optional["GetFeedFeedSiteGoogle"]
+    share_point: Optional["GetFeedFeedSiteSharePoint"] = Field(alias="sharePoint")
+    one_drive: Optional["GetFeedFeedSiteOneDrive"] = Field(alias="oneDrive")
+    google_drive: Optional["GetFeedFeedSiteGoogleDrive"] = Field(alias="googleDrive")
 
 
-class FeedFeedSiteS3(BaseModel):
+class GetFeedFeedSiteS3(BaseModel):
     access_key: Optional[str] = Field(alias="accessKey")
     secret_access_key: Optional[str] = Field(alias="secretAccessKey")
     bucket_name: Optional[str] = Field(alias="bucketName")
     prefix: Optional[str]
     region: Optional[str]
 
 
-class FeedFeedSiteAzureBlob(BaseModel):
+class GetFeedFeedSiteAzureBlob(BaseModel):
     storage_access_key: Optional[str] = Field(alias="storageAccessKey")
     account_name: Optional[str] = Field(alias="accountName")
     container_name: Optional[str] = Field(alias="containerName")
     prefix: Optional[str]
 
 
-class FeedFeedSiteAzureFile(BaseModel):
+class GetFeedFeedSiteAzureFile(BaseModel):
     storage_access_key: Optional[str] = Field(alias="storageAccessKey")
     account_name: Optional[str] = Field(alias="accountName")
     share_name: Optional[str] = Field(alias="shareName")
     prefix: Optional[str]
 
 
-class FeedFeedSiteGoogle(BaseModel):
+class GetFeedFeedSiteGoogle(BaseModel):
     credentials: Optional[str]
     container_name: Optional[str] = Field(alias="containerName")
     prefix: Optional[str]
 
 
-class FeedFeedSiteSharePoint(BaseModel):
+class GetFeedFeedSiteSharePoint(BaseModel):
     authentication_type: Optional[SharePointAuthenticationTypes] = Field(
         alias="authenticationType"
     )
     account_name: Optional[str] = Field(alias="accountName")
     library_id: Optional[str] = Field(alias="libraryId")
     tenant_id: Optional[str] = Field(alias="tenantId")
     refresh_token: Optional[str] = Field(alias="refreshToken")
 
 
-class FeedFeedSiteOneDrive(BaseModel):
+class GetFeedFeedSiteOneDrive(BaseModel):
     folder_id: Optional[str] = Field(alias="folderId")
     refresh_token: str = Field(alias="refreshToken")
 
 
-class FeedFeedSiteGoogleDrive(BaseModel):
+class GetFeedFeedSiteGoogleDrive(BaseModel):
     folder_id: Optional[str] = Field(alias="folderId")
     refresh_token: str = Field(alias="refreshToken")
 
 
-class FeedFeedEmail(BaseModel):
+class GetFeedFeedEmail(BaseModel):
     type: FeedServiceTypes
     include_attachments: Optional[bool] = Field(alias="includeAttachments")
-    google: Optional["FeedFeedEmailGoogle"]
-    microsoft: Optional["FeedFeedEmailMicrosoft"]
+    google: Optional["GetFeedFeedEmailGoogle"]
+    microsoft: Optional["GetFeedFeedEmailMicrosoft"]
 
 
-class FeedFeedEmailGoogle(BaseModel):
+class GetFeedFeedEmailGoogle(BaseModel):
     type: Optional[EmailListingTypes]
     refresh_token: Optional[str] = Field(alias="refreshToken")
 
 
-class FeedFeedEmailMicrosoft(BaseModel):
+class GetFeedFeedEmailMicrosoft(BaseModel):
     type: Optional[EmailListingTypes]
     tenant_id: Optional[str] = Field(alias="tenantId")
     refresh_token: Optional[str] = Field(alias="refreshToken")
 
 
-class FeedFeedIssue(BaseModel):
+class GetFeedFeedIssue(BaseModel):
     type: FeedServiceTypes
     include_attachments: Optional[bool] = Field(alias="includeAttachments")
-    jira: Optional["FeedFeedIssueJira"]
-    linear: Optional["FeedFeedIssueLinear"]
-    github: Optional["FeedFeedIssueGithub"]
+    jira: Optional["GetFeedFeedIssueJira"]
+    linear: Optional["GetFeedFeedIssueLinear"]
+    github: Optional["GetFeedFeedIssueGithub"]
 
 
-class FeedFeedIssueJira(BaseModel):
+class GetFeedFeedIssueJira(BaseModel):
     uri: Any
     project: str
     email: str
     token: str
 
 
-class FeedFeedIssueLinear(BaseModel):
+class GetFeedFeedIssueLinear(BaseModel):
     key: str
     project: str
 
 
-class FeedFeedIssueGithub(BaseModel):
+class GetFeedFeedIssueGithub(BaseModel):
     uri: Optional[Any]
     repository_owner: str = Field(alias="repositoryOwner")
     repository_name: str = Field(alias="repositoryName")
     refresh_token: Optional[str] = Field(alias="refreshToken")
     personal_access_token: Optional[str] = Field(alias="personalAccessToken")
 
 
-class FeedFeedRss(BaseModel):
+class GetFeedFeedRss(BaseModel):
     read_limit: Optional[int] = Field(alias="readLimit")
     uri: Any
 
 
-class FeedFeedWeb(BaseModel):
+class GetFeedFeedWeb(BaseModel):
     read_limit: Optional[int] = Field(alias="readLimit")
     uri: Any
     include_files: Optional[bool] = Field(alias="includeFiles")
 
 
-class FeedFeedReddit(BaseModel):
+class GetFeedFeedReddit(BaseModel):
     read_limit: Optional[int] = Field(alias="readLimit")
     subreddit_name: str = Field(alias="subredditName")
 
 
-class FeedFeedNotion(BaseModel):
+class GetFeedFeedNotion(BaseModel):
     read_limit: Optional[int] = Field(alias="readLimit")
     token: str
     identifiers: List[str]
     type: NotionTypes
 
 
-class FeedFeedYoutube(BaseModel):
+class GetFeedFeedYoutube(BaseModel):
     read_limit: Optional[int] = Field(alias="readLimit")
     type: YouTubeTypes
     video_name: Optional[str] = Field(alias="videoName")
     video_identifiers: Optional[List[str]] = Field(alias="videoIdentifiers")
     channel_identifier: Optional[str] = Field(alias="channelIdentifier")
     playlist_identifier: Optional[str] = Field(alias="playlistIdentifier")
 
 
-class FeedFeedSlack(BaseModel):
+class GetFeedFeedSlack(BaseModel):
     read_limit: Optional[int] = Field(alias="readLimit")
     type: Optional[FeedListingTypes]
     token: str
     channel: str
     include_attachments: Optional[bool] = Field(alias="includeAttachments")
 
 
-class FeedFeedDiscord(BaseModel):
+class GetFeedFeedDiscord(BaseModel):
     read_limit: Optional[int] = Field(alias="readLimit")
     type: Optional[FeedListingTypes]
     token: str
     channel: str
     include_attachments: Optional[bool] = Field(alias="includeAttachments")
 
 
-class FeedFeedWorkflow(BaseModel):
+class GetFeedFeedWorkflow(BaseModel):
     id: str
     name: str
 
 
-class FeedFeedSchedulePolicy(BaseModel):
+class GetFeedFeedSchedulePolicy(BaseModel):
     recurrence_type: Optional[TimedPolicyRecurrenceTypes] = Field(
         alias="recurrenceType"
     )
     repeat_interval: Optional[Any] = Field(alias="repeatInterval")
 
 
-Feed.model_rebuild()
-FeedFeed.model_rebuild()
-FeedFeedSite.model_rebuild()
-FeedFeedEmail.model_rebuild()
-FeedFeedIssue.model_rebuild()
+GetFeed.model_rebuild()
+GetFeedFeed.model_rebuild()
+GetFeedFeedSite.model_rebuild()
+GetFeedFeedEmail.model_rebuild()
+GetFeedFeedIssue.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/ingest_encoded_file.py` & `graphlit_client-1.0.20240420002/graphlit_api/ingest_encoded_file.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/ingest_text.py` & `graphlit_client-1.0.20240420002/graphlit_api/ingest_text.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/ingest_uri.py` & `graphlit_client-1.0.20240420002/graphlit_api/ingest_uri.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/input_types.py` & `graphlit_client-1.0.20240420002/graphlit_api/input_types.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/lookup_credits.py` & `graphlit_client-1.0.20240420002/graphlit_api/lookup_credits.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/lookup_usage.py` & `graphlit_client-1.0.20240420002/graphlit_api/lookup_usage.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/operations.py` & `graphlit_client-1.0.20240420002/graphlit_api/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 # Generated by ariadne-codegen
 # Source: ./documents
 
 __all__ = [
     "ADD_CONTENTS_TO_COLLECTIONS_GQL",
-    "ALERT_GQL",
     "CLEAR_CONVERSATION_GQL",
     "CLOSE_CONVERSATION_GQL",
-    "COLLECTION_GQL",
-    "CONTENT_GQL",
-    "CONVERSATION_GQL",
     "CREATE_ALERT_GQL",
     "CREATE_COLLECTION_GQL",
     "CREATE_CONVERSATION_GQL",
     "CREATE_FEED_GQL",
     "CREATE_SPECIFICATION_GQL",
     "CREATE_WORKFLOW_GQL",
     "CREDITS_GQL",
@@ -35,49 +31,53 @@
     "DELETE_WORKFLOWS_GQL",
     "DELETE_WORKFLOW_GQL",
     "DISABLE_ALERT_GQL",
     "DISABLE_FEED_GQL",
     "ENABLE_ALERT_GQL",
     "ENABLE_FEED_GQL",
     "EXTRACT_CONTENTS_GQL",
-    "FEED_GQL",
+    "GET_ALERT_GQL",
+    "GET_COLLECTION_GQL",
+    "GET_CONTENT_GQL",
+    "GET_CONVERSATION_GQL",
+    "GET_FEED_GQL",
+    "GET_PROJECT_GQL",
+    "GET_SPECIFICATION_GQL",
+    "GET_WORKFLOW_GQL",
     "INGEST_ENCODED_FILE_GQL",
     "INGEST_TEXT_GQL",
     "INGEST_URI_GQL",
     "IS_CONTENT_DONE_GQL",
     "IS_FEED_DONE_GQL",
     "LOOKUP_CREDITS_GQL",
     "LOOKUP_USAGE_GQL",
-    "PROJECT_GQL",
     "PROMPT_CONVERSATION_GQL",
     "PROMPT_SPECIFICATIONS_GQL",
     "PUBLISH_CONTENTS_GQL",
     "PUBLISH_CONVERSATION_GQL",
     "QUERY_ALERTS_GQL",
     "QUERY_COLLECTIONS_GQL",
     "QUERY_CONTENTS_GQL",
     "QUERY_CONTENT_FACETS_GQL",
     "QUERY_CONVERSATIONS_GQL",
     "QUERY_FEEDS_GQL",
     "QUERY_SPECIFICATIONS_GQL",
     "QUERY_WORKFLOWS_GQL",
     "REMOVE_CONTENTS_FROM_COLLECTION_GQL",
-    "SPECIFICATION_GQL",
     "SUGGEST_CONVERSATION_GQL",
     "SUMMARIZE_CONTENTS_GQL",
     "UPDATE_ALERT_GQL",
     "UPDATE_COLLECTION_GQL",
     "UPDATE_CONTENT_GQL",
     "UPDATE_CONVERSATION_GQL",
     "UPDATE_FEED_GQL",
     "UPDATE_PROJECT_GQL",
     "UPDATE_SPECIFICATION_GQL",
     "UPDATE_WORKFLOW_GQL",
     "USAGE_GQL",
-    "WORKFLOW_GQL",
 ]
 
 CREATE_ALERT_GQL = """
 mutation CreateAlert($alert: AlertInput!, $correlationId: String) {
   createAlert(alert: $alert, correlationId: $correlationId) {
     id
     name
@@ -128,16 +128,16 @@
   enableAlert(id: $id) {
     id
     state
   }
 }
 """
 
-ALERT_GQL = """
-query Alert($id: ID!) {
+GET_ALERT_GQL = """
+query GetAlert($id: ID!) {
   alert(id: $id) {
     id
     name
     creationDate
     owner {
       id
     }
@@ -327,16 +327,16 @@
   deleteCollections(ids: $ids) {
     id
     state
   }
 }
 """
 
-COLLECTION_GQL = """
-query Collection($id: ID!) {
+GET_COLLECTION_GQL = """
+query GetCollection($id: ID!) {
   collection(id: $id) {
     id
     name
     creationDate
     owner {
       id
     }
@@ -443,16 +443,16 @@
     endTime
     pageNumber
     error
   }
 }
 """
 
-CONTENT_GQL = """
-query Content($id: ID!) {
+GET_CONTENT_GQL = """
+query GetContent($id: ID!) {
   content(id: $id) {
     id
     name
     creationDate
     owner {
       id
     }
@@ -993,16 +993,16 @@
   deleteConversations(ids: $ids) {
     id
     state
   }
 }
 """
 
-CONVERSATION_GQL = """
-query Conversation($id: ID!) {
+GET_CONVERSATION_GQL = """
+query GetConversation($id: ID!) {
   conversation(id: $id) {
     id
     name
     creationDate
     owner {
       id
     }
@@ -1292,16 +1292,16 @@
   enableFeed(id: $id) {
     id
     state
   }
 }
 """
 
-FEED_GQL = """
-query Feed($id: ID!) {
+GET_FEED_GQL = """
+query GetFeed($id: ID!) {
   feed(id: $id) {
     id
     name
     creationDate
     owner {
       id
     }
@@ -1625,14 +1625,45 @@
     publishingRatio
     searchRatio
     conversationRatio
   }
 }
 """
 
+GET_PROJECT_GQL = """
+query GetProject {
+  project {
+    id
+    name
+    creationDate
+    modifiedDate
+    state
+    environmentType
+    platform
+    region
+    workflow {
+      id
+      name
+    }
+    specification {
+      id
+      name
+    }
+    quota {
+      storage
+      contents
+      feeds
+      posts
+      conversations
+    }
+    callbackUri
+  }
+}
+"""
+
 LOOKUP_CREDITS_GQL = """
 query LookupCredits($correlationId: String!) {
   lookupCredits(correlationId: $correlationId) {
     correlationId
     ownerId
     credits
     storageRatio
@@ -1677,45 +1708,14 @@
     request
     variables
     response
   }
 }
 """
 
-PROJECT_GQL = """
-query Project {
-  project {
-    id
-    name
-    creationDate
-    modifiedDate
-    state
-    environmentType
-    platform
-    region
-    workflow {
-      id
-      name
-    }
-    specification {
-      id
-      name
-    }
-    quota {
-      storage
-      contents
-      feeds
-      posts
-      conversations
-    }
-    callbackUri
-  }
-}
-"""
-
 UPDATE_PROJECT_GQL = """
 mutation UpdateProject($project: ProjectUpdateInput!) {
   updateProject(project: $project) {
     id
     name
   }
 }
@@ -1772,16 +1772,16 @@
   deleteSpecification(id: $id) {
     id
     state
   }
 }
 """
 
-SPECIFICATION_GQL = """
-query Specification($id: ID!) {
+GET_SPECIFICATION_GQL = """
+query GetSpecification($id: ID!) {
   specification(id: $id) {
     id
     name
     creationDate
     owner {
       id
     }
@@ -2110,16 +2110,16 @@
   deleteWorkflows(ids: $ids) {
     id
     state
   }
 }
 """
 
-WORKFLOW_GQL = """
-query Workflow($id: ID!) {
+GET_WORKFLOW_GQL = """
+query GetWorkflow($id: ID!) {
   workflow(id: $id) {
     id
     name
     creationDate
     owner {
       id
     }
```

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/project.py` & `graphlit_client-1.0.20240420002/graphlit_api/get_project.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,46 +5,46 @@
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import EntityState, EnvironmentTypes, ResourceConnectorTypes
 
 
-class Project(BaseModel):
-    project: Optional["ProjectProject"]
+class GetProject(BaseModel):
+    project: Optional["GetProjectProject"]
 
 
-class ProjectProject(BaseModel):
+class GetProjectProject(BaseModel):
     id: str
     name: str
     creation_date: Any = Field(alias="creationDate")
     modified_date: Optional[Any] = Field(alias="modifiedDate")
     state: EntityState
     environment_type: Optional[EnvironmentTypes] = Field(alias="environmentType")
     platform: Optional[ResourceConnectorTypes]
     region: Optional[str]
-    workflow: Optional["ProjectProjectWorkflow"]
-    specification: Optional["ProjectProjectSpecification"]
-    quota: Optional["ProjectProjectQuota"]
+    workflow: Optional["GetProjectProjectWorkflow"]
+    specification: Optional["GetProjectProjectSpecification"]
+    quota: Optional["GetProjectProjectQuota"]
     callback_uri: Optional[Any] = Field(alias="callbackUri")
 
 
-class ProjectProjectWorkflow(BaseModel):
+class GetProjectProjectWorkflow(BaseModel):
     id: str
     name: str
 
 
-class ProjectProjectSpecification(BaseModel):
+class GetProjectProjectSpecification(BaseModel):
     id: str
     name: str
 
 
-class ProjectProjectQuota(BaseModel):
+class GetProjectProjectQuota(BaseModel):
     storage: Optional[int]
     contents: Optional[int]
     feeds: Optional[int]
     posts: Optional[int]
     conversations: Optional[int]
 
 
-Project.model_rebuild()
-ProjectProject.model_rebuild()
+GetProject.model_rebuild()
+GetProjectProject.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/prompt_conversation.py` & `graphlit_client-1.0.20240420002/graphlit_api/prompt_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/prompt_specifications.py` & `graphlit_client-1.0.20240420002/graphlit_api/prompt_specifications.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/publish_contents.py` & `graphlit_client-1.0.20240420002/graphlit_api/publish_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/publish_conversation.py` & `graphlit_client-1.0.20240420002/graphlit_api/publish_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/query_alerts.py` & `graphlit_client-1.0.20240420002/graphlit_api/query_alerts.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/query_collections.py` & `graphlit_client-1.0.20240420002/graphlit_api/query_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/query_content_facets.py` & `graphlit_client-1.0.20240420002/graphlit_api/query_content_facets.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/query_contents.py` & `graphlit_client-1.0.20240420002/graphlit_api/query_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/query_conversations.py` & `graphlit_client-1.0.20240420002/graphlit_api/query_conversations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/query_feeds.py` & `graphlit_client-1.0.20240420002/graphlit_api/query_feeds.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/query_specifications.py` & `graphlit_client-1.0.20240420002/graphlit_api/query_specifications.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/query_workflows.py` & `graphlit_client-1.0.20240420002/graphlit_api/query_workflows.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/remove_contents_from_collection.py` & `graphlit_client-1.0.20240420002/graphlit_api/remove_contents_from_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/specification.py` & `graphlit_client-1.0.20240420002/graphlit_api/get_specification.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,116 +16,116 @@
     PromptStrategyTypes,
     ReplicateModels,
     RetrievalStrategyTypes,
     SpecificationTypes,
 )
 
 
-class Specification(BaseModel):
-    specification: Optional["SpecificationSpecification"]
+class GetSpecification(BaseModel):
+    specification: Optional["GetSpecificationSpecification"]
 
 
-class SpecificationSpecification(BaseModel):
+class GetSpecificationSpecification(BaseModel):
     id: str
     name: str
     creation_date: Any = Field(alias="creationDate")
-    owner: "SpecificationSpecificationOwner"
+    owner: "GetSpecificationSpecificationOwner"
     state: EntityState
     type: Optional[SpecificationTypes]
     service_type: Optional[ModelServiceTypes] = Field(alias="serviceType")
     system_prompt: Optional[str] = Field(alias="systemPrompt")
     custom_guidance: Optional[str] = Field(alias="customGuidance")
-    strategy: Optional["SpecificationSpecificationStrategy"]
-    prompt_strategy: Optional["SpecificationSpecificationPromptStrategy"] = Field(
+    strategy: Optional["GetSpecificationSpecificationStrategy"]
+    prompt_strategy: Optional["GetSpecificationSpecificationPromptStrategy"] = Field(
         alias="promptStrategy"
     )
-    retrieval_strategy: Optional["SpecificationSpecificationRetrievalStrategy"] = Field(
-        alias="retrievalStrategy"
+    retrieval_strategy: Optional["GetSpecificationSpecificationRetrievalStrategy"] = (
+        Field(alias="retrievalStrategy")
     )
-    reranking_strategy: Optional["SpecificationSpecificationRerankingStrategy"] = Field(
-        alias="rerankingStrategy"
+    reranking_strategy: Optional["GetSpecificationSpecificationRerankingStrategy"] = (
+        Field(alias="rerankingStrategy")
     )
-    open_ai: Optional["SpecificationSpecificationOpenAi"] = Field(alias="openAI")
-    azure_open_ai: Optional["SpecificationSpecificationAzureOpenAi"] = Field(
+    open_ai: Optional["GetSpecificationSpecificationOpenAi"] = Field(alias="openAI")
+    azure_open_ai: Optional["GetSpecificationSpecificationAzureOpenAi"] = Field(
         alias="azureOpenAI"
     )
-    anthropic: Optional["SpecificationSpecificationAnthropic"]
-    replicate: Optional["SpecificationSpecificationReplicate"]
-    tools: Optional[List["SpecificationSpecificationTools"]]
+    anthropic: Optional["GetSpecificationSpecificationAnthropic"]
+    replicate: Optional["GetSpecificationSpecificationReplicate"]
+    tools: Optional[List["GetSpecificationSpecificationTools"]]
 
 
-class SpecificationSpecificationOwner(BaseModel):
+class GetSpecificationSpecificationOwner(BaseModel):
     id: str
 
 
-class SpecificationSpecificationStrategy(BaseModel):
+class GetSpecificationSpecificationStrategy(BaseModel):
     type: Optional[ConversationStrategyTypes]
     message_limit: Optional[int] = Field(alias="messageLimit")
     embed_citations: Optional[bool] = Field(alias="embedCitations")
     enable_facets: Optional[bool] = Field(alias="enableFacets")
     messages_weight: Optional[float] = Field(alias="messagesWeight")
     contents_weight: Optional[float] = Field(alias="contentsWeight")
 
 
-class SpecificationSpecificationPromptStrategy(BaseModel):
+class GetSpecificationSpecificationPromptStrategy(BaseModel):
     type: PromptStrategyTypes
 
 
-class SpecificationSpecificationRetrievalStrategy(BaseModel):
+class GetSpecificationSpecificationRetrievalStrategy(BaseModel):
     type: RetrievalStrategyTypes
     content_limit: Optional[int] = Field(alias="contentLimit")
 
 
-class SpecificationSpecificationRerankingStrategy(BaseModel):
+class GetSpecificationSpecificationRerankingStrategy(BaseModel):
     service_type: ModelServiceTypes = Field(alias="serviceType")
 
 
-class SpecificationSpecificationOpenAi(BaseModel):
+class GetSpecificationSpecificationOpenAi(BaseModel):
     token_limit: Optional[int] = Field(alias="tokenLimit")
     completion_token_limit: Optional[int] = Field(alias="completionTokenLimit")
     model: OpenAIModels
     key: Optional[str]
     model_name: Optional[str] = Field(alias="modelName")
     temperature: Optional[float]
     probability: Optional[float]
 
 
-class SpecificationSpecificationAzureOpenAi(BaseModel):
+class GetSpecificationSpecificationAzureOpenAi(BaseModel):
     token_limit: Optional[int] = Field(alias="tokenLimit")
     completion_token_limit: Optional[int] = Field(alias="completionTokenLimit")
     model: AzureOpenAIModels
     key: Optional[str]
     endpoint: Optional[Any]
     deployment_name: Optional[str] = Field(alias="deploymentName")
     temperature: Optional[float]
     probability: Optional[float]
 
 
-class SpecificationSpecificationAnthropic(BaseModel):
+class GetSpecificationSpecificationAnthropic(BaseModel):
     token_limit: Optional[int] = Field(alias="tokenLimit")
     completion_token_limit: Optional[int] = Field(alias="completionTokenLimit")
     model: AnthropicModels
     key: Optional[str]
     model_name: Optional[str] = Field(alias="modelName")
     temperature: Optional[float]
     probability: Optional[float]
 
 
-class SpecificationSpecificationReplicate(BaseModel):
+class GetSpecificationSpecificationReplicate(BaseModel):
     token_limit: Optional[int] = Field(alias="tokenLimit")
     completion_token_limit: Optional[int] = Field(alias="completionTokenLimit")
     model: ReplicateModels
     key: Optional[str]
     model_name: Optional[str] = Field(alias="modelName")
     temperature: Optional[float]
     probability: Optional[float]
 
 
-class SpecificationSpecificationTools(BaseModel):
+class GetSpecificationSpecificationTools(BaseModel):
     name: str
     description: Optional[str]
     schema_: str = Field(alias="schema")
     uri: Optional[Any]
 
 
-Specification.model_rebuild()
-SpecificationSpecification.model_rebuild()
+GetSpecification.model_rebuild()
+GetSpecificationSpecification.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/summarize_contents.py` & `graphlit_client-1.0.20240420002/graphlit_api/summarize_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/update_collection.py` & `graphlit_client-1.0.20240420002/graphlit_api/update_conversation.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 # Source: ./documents
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
-from .enums import CollectionTypes, EntityState
+from .enums import ConversationTypes, EntityState
 
 
-class UpdateCollection(BaseModel):
-    update_collection: Optional["UpdateCollectionUpdateCollection"] = Field(
-        alias="updateCollection"
+class UpdateConversation(BaseModel):
+    update_conversation: Optional["UpdateConversationUpdateConversation"] = Field(
+        alias="updateConversation"
     )
 
 
-class UpdateCollectionUpdateCollection(BaseModel):
+class UpdateConversationUpdateConversation(BaseModel):
     id: str
     name: str
     state: EntityState
-    type: Optional[CollectionTypes]
+    type: Optional[ConversationTypes]
 
 
-UpdateCollection.model_rebuild()
+UpdateConversation.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/update_content.py` & `graphlit_client-1.0.20240420002/graphlit_api/update_content.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/update_specification.py` & `graphlit_client-1.0.20240420002/graphlit_api/update_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/update_workflow.py` & `graphlit_client-1.0.20240420002/graphlit_api/update_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/usage.py` & `graphlit_client-1.0.20240420002/graphlit_api/usage.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420001/graphlit_api/workflow.py` & `graphlit_client-1.0.20240420002/graphlit_api/get_workflow.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,204 +19,204 @@
     LinkTypes,
     ObservableTypes,
     OpenAIVisionDetailLevels,
     SummarizationTypes,
 )
 
 
-class Workflow(BaseModel):
-    workflow: Optional["WorkflowWorkflow"]
+class GetWorkflow(BaseModel):
+    workflow: Optional["GetWorkflowWorkflow"]
 
 
-class WorkflowWorkflow(BaseModel):
+class GetWorkflowWorkflow(BaseModel):
     id: str
     name: str
     creation_date: Any = Field(alias="creationDate")
-    owner: "WorkflowWorkflowOwner"
+    owner: "GetWorkflowWorkflowOwner"
     state: EntityState
-    ingestion: Optional["WorkflowWorkflowIngestion"]
-    preparation: Optional["WorkflowWorkflowPreparation"]
-    extraction: Optional["WorkflowWorkflowExtraction"]
-    enrichment: Optional["WorkflowWorkflowEnrichment"]
-    actions: Optional[List[Optional["WorkflowWorkflowActions"]]]
+    ingestion: Optional["GetWorkflowWorkflowIngestion"]
+    preparation: Optional["GetWorkflowWorkflowPreparation"]
+    extraction: Optional["GetWorkflowWorkflowExtraction"]
+    enrichment: Optional["GetWorkflowWorkflowEnrichment"]
+    actions: Optional[List[Optional["GetWorkflowWorkflowActions"]]]
 
 
-class WorkflowWorkflowOwner(BaseModel):
+class GetWorkflowWorkflowOwner(BaseModel):
     id: str
 
 
-class WorkflowWorkflowIngestion(BaseModel):
-    if_: Optional["WorkflowWorkflowIngestionIf"] = Field(alias="if")
-    collections: Optional[List[Optional["WorkflowWorkflowIngestionCollections"]]]
+class GetWorkflowWorkflowIngestion(BaseModel):
+    if_: Optional["GetWorkflowWorkflowIngestionIf"] = Field(alias="if")
+    collections: Optional[List[Optional["GetWorkflowWorkflowIngestionCollections"]]]
 
 
-class WorkflowWorkflowIngestionIf(BaseModel):
+class GetWorkflowWorkflowIngestionIf(BaseModel):
     types: Optional[List[Optional[ContentTypes]]]
     file_types: Optional[List[Optional[FileTypes]]] = Field(alias="fileTypes")
 
 
-class WorkflowWorkflowIngestionCollections(BaseModel):
+class GetWorkflowWorkflowIngestionCollections(BaseModel):
     id: str
 
 
-class WorkflowWorkflowPreparation(BaseModel):
+class GetWorkflowWorkflowPreparation(BaseModel):
     disable_smart_capture: Optional[bool] = Field(alias="disableSmartCapture")
     summarizations: Optional[
-        List[Optional["WorkflowWorkflowPreparationSummarizations"]]
+        List[Optional["GetWorkflowWorkflowPreparationSummarizations"]]
     ]
-    jobs: Optional[List[Optional["WorkflowWorkflowPreparationJobs"]]]
+    jobs: Optional[List[Optional["GetWorkflowWorkflowPreparationJobs"]]]
 
 
-class WorkflowWorkflowPreparationSummarizations(BaseModel):
+class GetWorkflowWorkflowPreparationSummarizations(BaseModel):
     type: SummarizationTypes
-    specification: Optional["WorkflowWorkflowPreparationSummarizationsSpecification"]
+    specification: Optional["GetWorkflowWorkflowPreparationSummarizationsSpecification"]
     tokens: Optional[int]
     items: Optional[int]
 
 
-class WorkflowWorkflowPreparationSummarizationsSpecification(BaseModel):
+class GetWorkflowWorkflowPreparationSummarizationsSpecification(BaseModel):
     id: str
 
 
-class WorkflowWorkflowPreparationJobs(BaseModel):
-    connector: Optional["WorkflowWorkflowPreparationJobsConnector"]
+class GetWorkflowWorkflowPreparationJobs(BaseModel):
+    connector: Optional["GetWorkflowWorkflowPreparationJobsConnector"]
 
 
-class WorkflowWorkflowPreparationJobsConnector(BaseModel):
+class GetWorkflowWorkflowPreparationJobsConnector(BaseModel):
     type: FilePreparationServiceTypes
     file_types: Optional[List[FileTypes]] = Field(alias="fileTypes")
     azure_document: Optional[
-        "WorkflowWorkflowPreparationJobsConnectorAzureDocument"
+        "GetWorkflowWorkflowPreparationJobsConnectorAzureDocument"
     ] = Field(alias="azureDocument")
-    deepgram: Optional["WorkflowWorkflowPreparationJobsConnectorDeepgram"]
-    document: Optional["WorkflowWorkflowPreparationJobsConnectorDocument"]
-    email: Optional["WorkflowWorkflowPreparationJobsConnectorEmail"]
+    deepgram: Optional["GetWorkflowWorkflowPreparationJobsConnectorDeepgram"]
+    document: Optional["GetWorkflowWorkflowPreparationJobsConnectorDocument"]
+    email: Optional["GetWorkflowWorkflowPreparationJobsConnectorEmail"]
 
 
-class WorkflowWorkflowPreparationJobsConnectorAzureDocument(BaseModel):
+class GetWorkflowWorkflowPreparationJobsConnectorAzureDocument(BaseModel):
     model: Optional[AzureDocumentIntelligenceModels]
 
 
-class WorkflowWorkflowPreparationJobsConnectorDeepgram(BaseModel):
+class GetWorkflowWorkflowPreparationJobsConnectorDeepgram(BaseModel):
     model: Optional[DeepgramModels]
     key: Optional[str]
     enable_redaction: Optional[bool] = Field(alias="enableRedaction")
     enable_speaker_diarization: Optional[bool] = Field(alias="enableSpeakerDiarization")
 
 
-class WorkflowWorkflowPreparationJobsConnectorDocument(BaseModel):
+class GetWorkflowWorkflowPreparationJobsConnectorDocument(BaseModel):
     include_images: Optional[bool] = Field(alias="includeImages")
 
 
-class WorkflowWorkflowPreparationJobsConnectorEmail(BaseModel):
+class GetWorkflowWorkflowPreparationJobsConnectorEmail(BaseModel):
     include_attachments: Optional[bool] = Field(alias="includeAttachments")
 
 
-class WorkflowWorkflowExtraction(BaseModel):
-    jobs: Optional[List[Optional["WorkflowWorkflowExtractionJobs"]]]
+class GetWorkflowWorkflowExtraction(BaseModel):
+    jobs: Optional[List[Optional["GetWorkflowWorkflowExtractionJobs"]]]
 
 
-class WorkflowWorkflowExtractionJobs(BaseModel):
-    connector: Optional["WorkflowWorkflowExtractionJobsConnector"]
+class GetWorkflowWorkflowExtractionJobs(BaseModel):
+    connector: Optional["GetWorkflowWorkflowExtractionJobsConnector"]
 
 
-class WorkflowWorkflowExtractionJobsConnector(BaseModel):
+class GetWorkflowWorkflowExtractionJobsConnector(BaseModel):
     type: EntityExtractionServiceTypes
     content_types: Optional[List[ContentTypes]] = Field(alias="contentTypes")
     file_types: Optional[List[FileTypes]] = Field(alias="fileTypes")
     extracted_types: Optional[List[ObservableTypes]] = Field(alias="extractedTypes")
-    azure_text: Optional["WorkflowWorkflowExtractionJobsConnectorAzureText"] = Field(
+    azure_text: Optional["GetWorkflowWorkflowExtractionJobsConnectorAzureText"] = Field(
         alias="azureText"
     )
-    azure_image: Optional["WorkflowWorkflowExtractionJobsConnectorAzureImage"] = Field(
-        alias="azureImage"
+    azure_image: Optional["GetWorkflowWorkflowExtractionJobsConnectorAzureImage"] = (
+        Field(alias="azureImage")
     )
-    open_ai_image: Optional["WorkflowWorkflowExtractionJobsConnectorOpenAiImage"] = (
+    open_ai_image: Optional["GetWorkflowWorkflowExtractionJobsConnectorOpenAiImage"] = (
         Field(alias="openAIImage")
     )
-    model_text: Optional["WorkflowWorkflowExtractionJobsConnectorModelText"] = Field(
+    model_text: Optional["GetWorkflowWorkflowExtractionJobsConnectorModelText"] = Field(
         alias="modelText"
     )
 
 
-class WorkflowWorkflowExtractionJobsConnectorAzureText(BaseModel):
+class GetWorkflowWorkflowExtractionJobsConnectorAzureText(BaseModel):
     confidence_threshold: Optional[float] = Field(alias="confidenceThreshold")
     enable_pii: Optional[bool] = Field(alias="enablePII")
 
 
-class WorkflowWorkflowExtractionJobsConnectorAzureImage(BaseModel):
+class GetWorkflowWorkflowExtractionJobsConnectorAzureImage(BaseModel):
     confidence_threshold: Optional[float] = Field(alias="confidenceThreshold")
 
 
-class WorkflowWorkflowExtractionJobsConnectorOpenAiImage(BaseModel):
+class GetWorkflowWorkflowExtractionJobsConnectorOpenAiImage(BaseModel):
     confidence_threshold: Optional[float] = Field(alias="confidenceThreshold")
     detail_level: Optional[OpenAIVisionDetailLevels] = Field(alias="detailLevel")
 
 
-class WorkflowWorkflowExtractionJobsConnectorModelText(BaseModel):
+class GetWorkflowWorkflowExtractionJobsConnectorModelText(BaseModel):
     specification: Optional[
-        "WorkflowWorkflowExtractionJobsConnectorModelTextSpecification"
+        "GetWorkflowWorkflowExtractionJobsConnectorModelTextSpecification"
     ]
 
 
-class WorkflowWorkflowExtractionJobsConnectorModelTextSpecification(BaseModel):
+class GetWorkflowWorkflowExtractionJobsConnectorModelTextSpecification(BaseModel):
     id: str
 
 
-class WorkflowWorkflowEnrichment(BaseModel):
-    link: Optional["WorkflowWorkflowEnrichmentLink"]
-    jobs: Optional[List[Optional["WorkflowWorkflowEnrichmentJobs"]]]
+class GetWorkflowWorkflowEnrichment(BaseModel):
+    link: Optional["GetWorkflowWorkflowEnrichmentLink"]
+    jobs: Optional[List[Optional["GetWorkflowWorkflowEnrichmentJobs"]]]
 
 
-class WorkflowWorkflowEnrichmentLink(BaseModel):
+class GetWorkflowWorkflowEnrichmentLink(BaseModel):
     enable_crawling: Optional[bool] = Field(alias="enableCrawling")
     allowed_domains: Optional[List[str]] = Field(alias="allowedDomains")
     excluded_domains: Optional[List[str]] = Field(alias="excludedDomains")
     allowed_links: Optional[List[LinkTypes]] = Field(alias="allowedLinks")
     excluded_links: Optional[List[LinkTypes]] = Field(alias="excludedLinks")
     allowed_files: Optional[List[FileTypes]] = Field(alias="allowedFiles")
     excluded_files: Optional[List[FileTypes]] = Field(alias="excludedFiles")
     allow_content_domain: Optional[bool] = Field(alias="allowContentDomain")
     maximum_links: Optional[int] = Field(alias="maximumLinks")
 
 
-class WorkflowWorkflowEnrichmentJobs(BaseModel):
-    connector: Optional["WorkflowWorkflowEnrichmentJobsConnector"]
+class GetWorkflowWorkflowEnrichmentJobs(BaseModel):
+    connector: Optional["GetWorkflowWorkflowEnrichmentJobsConnector"]
 
 
-class WorkflowWorkflowEnrichmentJobsConnector(BaseModel):
+class GetWorkflowWorkflowEnrichmentJobsConnector(BaseModel):
     type: Optional[EntityEnrichmentServiceTypes]
     enriched_types: Optional[List[Optional[ObservableTypes]]] = Field(
         alias="enrichedTypes"
     )
 
 
-class WorkflowWorkflowActions(BaseModel):
-    connector: Optional["WorkflowWorkflowActionsConnector"]
+class GetWorkflowWorkflowActions(BaseModel):
+    connector: Optional["GetWorkflowWorkflowActionsConnector"]
 
 
-class WorkflowWorkflowActionsConnector(BaseModel):
+class GetWorkflowWorkflowActionsConnector(BaseModel):
     type: IntegrationServiceTypes
     uri: Optional[str]
-    slack: Optional["WorkflowWorkflowActionsConnectorSlack"]
+    slack: Optional["GetWorkflowWorkflowActionsConnectorSlack"]
 
 
-class WorkflowWorkflowActionsConnectorSlack(BaseModel):
+class GetWorkflowWorkflowActionsConnectorSlack(BaseModel):
     token: str
     channel: str
 
 
-Workflow.model_rebuild()
-WorkflowWorkflow.model_rebuild()
-WorkflowWorkflowIngestion.model_rebuild()
-WorkflowWorkflowPreparation.model_rebuild()
-WorkflowWorkflowPreparationSummarizations.model_rebuild()
-WorkflowWorkflowPreparationJobs.model_rebuild()
-WorkflowWorkflowPreparationJobsConnector.model_rebuild()
-WorkflowWorkflowExtraction.model_rebuild()
-WorkflowWorkflowExtractionJobs.model_rebuild()
-WorkflowWorkflowExtractionJobsConnector.model_rebuild()
-WorkflowWorkflowExtractionJobsConnectorModelText.model_rebuild()
-WorkflowWorkflowEnrichment.model_rebuild()
-WorkflowWorkflowEnrichmentJobs.model_rebuild()
-WorkflowWorkflowActions.model_rebuild()
-WorkflowWorkflowActionsConnector.model_rebuild()
+GetWorkflow.model_rebuild()
+GetWorkflowWorkflow.model_rebuild()
+GetWorkflowWorkflowIngestion.model_rebuild()
+GetWorkflowWorkflowPreparation.model_rebuild()
+GetWorkflowWorkflowPreparationSummarizations.model_rebuild()
+GetWorkflowWorkflowPreparationJobs.model_rebuild()
+GetWorkflowWorkflowPreparationJobsConnector.model_rebuild()
+GetWorkflowWorkflowExtraction.model_rebuild()
+GetWorkflowWorkflowExtractionJobs.model_rebuild()
+GetWorkflowWorkflowExtractionJobsConnector.model_rebuild()
+GetWorkflowWorkflowExtractionJobsConnectorModelText.model_rebuild()
+GetWorkflowWorkflowEnrichment.model_rebuild()
+GetWorkflowWorkflowEnrichmentJobs.model_rebuild()
+GetWorkflowWorkflowActions.model_rebuild()
+GetWorkflowWorkflowActionsConnector.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240420001/graphlit_client.egg-info/PKG-INFO` & `graphlit_client-1.0.20240420002/graphlit_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 1.0.20240420001
+Version: 1.0.20240420002
 Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
 Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `graphlit_client-1.0.20240420001/graphlit_client.egg-info/SOURCES.txt` & `graphlit_client-1.0.20240420002/graphlit_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,19 @@
 README.md
 pyproject.toml
 setup.py
 graphlit/__init__.py
 graphlit/graphlit.py
 graphlit_api/__init__.py
 graphlit_api/add_contents_to_collections.py
-graphlit_api/alert.py
 graphlit_api/async_base_client.py
 graphlit_api/base_model.py
 graphlit_api/clear_conversation.py
 graphlit_api/client.py
 graphlit_api/close_conversation.py
-graphlit_api/collection.py
-graphlit_api/content.py
-graphlit_api/conversation.py
 graphlit_api/create_alert.py
 graphlit_api/create_collection.py
 graphlit_api/create_conversation.py
 graphlit_api/create_feed.py
 graphlit_api/create_specification.py
 graphlit_api/create_workflow.py
 graphlit_api/credits.py
@@ -43,49 +39,53 @@
 graphlit_api/disable_alert.py
 graphlit_api/disable_feed.py
 graphlit_api/enable_alert.py
 graphlit_api/enable_feed.py
 graphlit_api/enums.py
 graphlit_api/exceptions.py
 graphlit_api/extract_contents.py
-graphlit_api/feed.py
+graphlit_api/get_alert.py
+graphlit_api/get_collection.py
+graphlit_api/get_content.py
+graphlit_api/get_conversation.py
+graphlit_api/get_feed.py
+graphlit_api/get_project.py
+graphlit_api/get_specification.py
+graphlit_api/get_workflow.py
 graphlit_api/ingest_encoded_file.py
 graphlit_api/ingest_text.py
 graphlit_api/ingest_uri.py
 graphlit_api/input_types.py
 graphlit_api/is_content_done.py
 graphlit_api/is_feed_done.py
 graphlit_api/lookup_credits.py
 graphlit_api/lookup_usage.py
 graphlit_api/operations.py
-graphlit_api/project.py
 graphlit_api/prompt_conversation.py
 graphlit_api/prompt_specifications.py
 graphlit_api/publish_contents.py
 graphlit_api/publish_conversation.py
 graphlit_api/query_alerts.py
 graphlit_api/query_collections.py
 graphlit_api/query_content_facets.py
 graphlit_api/query_contents.py
 graphlit_api/query_conversations.py
 graphlit_api/query_feeds.py
 graphlit_api/query_specifications.py
 graphlit_api/query_workflows.py
 graphlit_api/remove_contents_from_collection.py
-graphlit_api/specification.py
 graphlit_api/suggest_conversation.py
 graphlit_api/summarize_contents.py
 graphlit_api/update_alert.py
 graphlit_api/update_collection.py
 graphlit_api/update_content.py
 graphlit_api/update_conversation.py
 graphlit_api/update_feed.py
 graphlit_api/update_project.py
 graphlit_api/update_specification.py
 graphlit_api/update_workflow.py
 graphlit_api/usage.py
-graphlit_api/workflow.py
 graphlit_client.egg-info/PKG-INFO
 graphlit_client.egg-info/SOURCES.txt
 graphlit_client.egg-info/dependency_links.txt
 graphlit_client.egg-info/requires.txt
 graphlit_client.egg-info/top_level.txt
```

### Comparing `graphlit_client-1.0.20240420001/setup.py` & `graphlit_client-1.0.20240420002/setup.py`

 * *Files identical despite different names*

