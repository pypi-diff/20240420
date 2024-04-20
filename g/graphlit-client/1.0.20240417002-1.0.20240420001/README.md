# Comparing `tmp/graphlit_client-1.0.20240417002.tar.gz` & `tmp/graphlit_client-1.0.20240420001.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphlit_client-1.0.20240417002.tar", last modified: Thu Apr 18 01:47:12 2024, max compression
+gzip compressed data, was "graphlit_client-1.0.20240420001.tar", last modified: Sat Apr 20 19:41:46 2024, max compression
```

## Comparing `graphlit_client-1.0.20240417002.tar` & `graphlit_client-1.0.20240420001.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 01:47:12.872147 graphlit_client-1.0.20240417002/
--rw-r--r--   0 vsts      (1001) docker     (127)     1074 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-18 01:47:12.872147 graphlit_client-1.0.20240417002/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2253 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 01:47:12.856147 graphlit_client-1.0.20240417002/graphlit/
--rw-r--r--   0 vsts      (1001) docker     (127)       31 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1757 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit/graphlit.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 01:47:12.864147 graphlit_client-1.0.20240417002/graphlit_api/
--rw-r--r--   0 vsts      (1001) docker     (127)    58887 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/add_contents_to_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/async_base_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/base_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/clear_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41993 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/close_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/create_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/create_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/create_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/create_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/create_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/create_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      984 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/delete_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/delete_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/delete_all_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/delete_all_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/delete_all_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/delete_all_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/delete_all_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/delete_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/delete_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/delete_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/delete_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/delete_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/delete_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/delete_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/delete_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/delete_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/delete_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/delete_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/disable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/disable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/enable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/enable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16585 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/extract_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3609 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/get_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/get_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7230 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/get_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4014 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/get_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7138 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/get_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4451 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/get_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7887 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/get_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      677 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/ingest_encoded_file.py
--rw-r--r--   0 vsts      (1001) docker     (127)      606 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/ingest_text.py
--rw-r--r--   0 vsts      (1001) docker     (127)      598 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/ingest_uri.py
--rw-r--r--   0 vsts      (1001) docker     (127)    67968 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/input_types.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/is_content_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/is_feed_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/lookup_credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1568 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/lookup_usage.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39264 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/operations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1236 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/project.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3242 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/prompt_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2055 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/prompt_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)      796 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/publish_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/publish_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/query_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/query_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1112 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/query_content_facets.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7934 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/query_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4623 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/query_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7942 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/query_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4902 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/query_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8865 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/query_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/remove_contents_from_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/suggest_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/summarize_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/update_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/update_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      644 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/update_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/update_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/update_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/update_project.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/update_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/update_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1482 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/graphlit_api/usage.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 01:47:12.872147 graphlit_client-1.0.20240417002/graphlit_client.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-18 01:47:12.000000 graphlit_client-1.0.20240417002/graphlit_client.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2827 2024-04-18 01:47:12.000000 graphlit_client-1.0.20240417002/graphlit_client.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-18 01:47:12.000000 graphlit_client-1.0.20240417002/graphlit_client.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-18 01:47:12.000000 graphlit_client-1.0.20240417002/graphlit_client.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-04-18 01:47:12.000000 graphlit_client-1.0.20240417002/graphlit_client.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      292 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-18 01:47:12.872147 graphlit_client-1.0.20240417002/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      739 2024-04-18 01:47:01.000000 graphlit_client-1.0.20240417002/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 19:41:46.624794 graphlit_client-1.0.20240420001/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-20 19:41:46.624794 graphlit_client-1.0.20240420001/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2321 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 19:41:46.604794 graphlit_client-1.0.20240420001/graphlit/
+-rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1796 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit/graphlit.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 19:41:46.620794 graphlit_client-1.0.20240420001/graphlit_api/
+-rw-r--r--   0 vsts      (1001) docker     (127)    58023 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/add_contents_to_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3472 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/async_base_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/base_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/clear_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41721 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/close_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      772 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7078 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3905 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/create_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/create_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/create_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/create_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/create_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/create_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      984 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_all_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_all_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_all_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_all_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_all_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/delete_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/disable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/disable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/enable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/enable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16585 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/extract_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6950 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      677 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/ingest_encoded_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      606 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/ingest_text.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      598 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/ingest_uri.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    68146 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/input_types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/is_content_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/is_feed_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/lookup_credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1568 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/lookup_usage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39187 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1236 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3242 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/prompt_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2055 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/prompt_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      796 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/publish_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/publish_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/query_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/query_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1112 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/query_content_facets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7934 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/query_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4623 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/query_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7942 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/query_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4912 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/query_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8865 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/query_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/remove_contents_from_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4382 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/suggest_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/summarize_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/update_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/update_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      644 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/update_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/update_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/update_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/update_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/update_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/update_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1482 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/usage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7663 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/graphlit_api/workflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 19:41:46.624794 graphlit_client-1.0.20240420001/graphlit_client.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-20 19:41:46.000000 graphlit_client-1.0.20240420001/graphlit_client.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2799 2024-04-20 19:41:46.000000 graphlit_client-1.0.20240420001/graphlit_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-20 19:41:46.000000 graphlit_client-1.0.20240420001/graphlit_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-20 19:41:46.000000 graphlit_client-1.0.20240420001/graphlit_client.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-04-20 19:41:46.000000 graphlit_client-1.0.20240420001/graphlit_client.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      299 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-20 19:41:46.624794 graphlit_client-1.0.20240420001/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-04-20 19:41:32.000000 graphlit_client-1.0.20240420001/setup.py
```

### Comparing `graphlit_client-1.0.20240417002/LICENSE` & `graphlit_client-1.0.20240420001/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Unstruk Data Inc.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Unstruk Data Inc.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `graphlit_client-1.0.20240417002/PKG-INFO` & `graphlit_client-1.0.20240420001/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 1.0.20240417002
+Version: 1.0.20240420001
 Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
 Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `graphlit_client-1.0.20240417002/README.md` & `graphlit_client-1.0.20240420001/graphlit_client.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: graphlit-client
+Version: 1.0.20240420001
+Summary: Graphlit API Python Client
+Home-page: https://github.com/graphlit/graphlit-client-python
+Author: Unstruk Data Inc.
+Author-email: questions@graphlit.com
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: httpx
+Requires-Dist: pydantic<3.0.0,>=2.0.0
+Requires-Dist: PyJWT
+Requires-Dist: websockets
+
 # Python Client for Graphlit Platform
 
 ## Overview
 
 The Graphlit Client for Python enables easy interaction with the Graphlit API, allowing developers to execute queries and mutations against the Graphlit service. This document outlines the setup process and provides a basic example of using the client.
 
 ## Prerequisites
```

### Comparing `graphlit_client-1.0.20240417002/graphlit/graphlit.py` & `graphlit_client-1.0.20240420001/graphlit/graphlit.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-import os
-import jwt
-import datetime
-import httpx
-from graphlit_api.client import Client
-
-class Graphlit:
-    def __init__(self, organization_id=None, environment_id=None, jwt_secret=None, owner_id=None, api_uri=None):
-        self.organization_id = organization_id if organization_id is not None else os.getenv("GRAPHLIT_ORGANIZATION_ID")
-        self.environment_id = environment_id if environment_id is not None else os.getenv("GRAPHLIT_ENVIRONMENT_ID")
-        self.owner_id = owner_id if owner_id is not None else os.getenv("GRAPHLIT_OWNER_ID")
-        self.secret_key = jwt_secret if jwt_secret is not None else os.getenv("GRAPHLIT_JWT_SECRET")
-
-        self.api_uri = api_uri if api_uri is not None else "https://data-scus.graphlit.io/api/v1/graphql/"
-
-        # Specify the expiration (one hour from now in UTC)
-        expiration = datetime.datetime.now(datetime.timezone.utc) + datetime.timedelta(hours=1)
-
-        # Define the payload
-        payload = {
-            "https://graphlit.io/jwt/claims": {
-                "x-graphlit-organization-id": self.organization_id,
-                "x-graphlit-environment-id": self.environment_id,
-                "x-graphlit-role": "Owner",
-            },
-            "exp": expiration,
-            "iss": "graphlit",
-            "aud": "https://portal.graphlit.io",
-        }
-
-        if self.owner_id is not None:
-            payload["https://graphlit.io/jwt/claims"]["x-graphlit-owner-id"] = self.owner_id
-
-        # Sign the JWT
-        self.token = jwt.encode(payload, self.secret_key, algorithm="HS256")
-
-        headers = {"Authorization": f"Bearer {self.token}"}
-
-        self.client = Client(url=self.api_uri, headers=headers)
+import os
+import jwt
+import datetime
+import httpx
+from graphlit_api.client import Client
+
+class Graphlit:
+    def __init__(self, organization_id=None, environment_id=None, jwt_secret=None, owner_id=None, api_uri=None):
+        self.organization_id = organization_id if organization_id is not None else os.getenv("GRAPHLIT_ORGANIZATION_ID")
+        self.environment_id = environment_id if environment_id is not None else os.getenv("GRAPHLIT_ENVIRONMENT_ID")
+        self.owner_id = owner_id if owner_id is not None else os.getenv("GRAPHLIT_OWNER_ID")
+        self.secret_key = jwt_secret if jwt_secret is not None else os.getenv("GRAPHLIT_JWT_SECRET")
+
+        self.api_uri = api_uri if api_uri is not None else "https://data-scus.graphlit.io/api/v1/graphql/"
+
+        # Specify the expiration (one hour from now in UTC)
+        expiration = datetime.datetime.now(datetime.timezone.utc) + datetime.timedelta(hours=1)
+
+        # Define the payload
+        payload = {
+            "https://graphlit.io/jwt/claims": {
+                "x-graphlit-organization-id": self.organization_id,
+                "x-graphlit-environment-id": self.environment_id,
+                "x-graphlit-role": "Owner",
+            },
+            "exp": expiration,
+            "iss": "graphlit",
+            "aud": "https://portal.graphlit.io",
+        }
+
+        if self.owner_id is not None:
+            payload["https://graphlit.io/jwt/claims"]["x-graphlit-owner-id"] = self.owner_id
+
+        # Sign the JWT
+        self.token = jwt.encode(payload, self.secret_key, algorithm="HS256")
+
+        headers = {"Authorization": f"Bearer {self.token}"}
+
+        self.client = Client(url=self.api_uri, headers=headers)
         self.client.http_client.timeout = httpx.Timeout(timeout=600.0)
```

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/__init__.py` & `graphlit_client-1.0.20240420001/graphlit_api/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,88 @@
 # Generated by ariadne-codegen
 
 from .add_contents_to_collections import (
     AddContentsToCollections,
     AddContentsToCollectionsAddContentsToCollections,
     AddContentsToCollectionsAddContentsToCollectionsContents,
 )
+from .alert import (
+    Alert,
+    AlertAlert,
+    AlertAlertFilter,
+    AlertAlertFilterCollections,
+    AlertAlertFilterContents,
+    AlertAlertFilterCreationDateRange,
+    AlertAlertFilterDateRange,
+    AlertAlertFilterFeeds,
+    AlertAlertFilterObservations,
+    AlertAlertFilterObservationsObservable,
+    AlertAlertFilterWorkflows,
+    AlertAlertIntegration,
+    AlertAlertIntegrationSlack,
+    AlertAlertOwner,
+    AlertAlertPublishing,
+    AlertAlertPublishingElevenLabs,
+    AlertAlertPublishSpecification,
+    AlertAlertSummarySpecification,
+)
 from .async_base_client import AsyncBaseClient
 from .base_model import BaseModel, Upload
 from .clear_conversation import ClearConversation, ClearConversationClearConversation
 from .client import Client
 from .close_conversation import CloseConversation, CloseConversationCloseConversation
+from .collection import (
+    Collection,
+    CollectionCollection,
+    CollectionCollectionContents,
+    CollectionCollectionOwner,
+)
+from .content import (
+    Content,
+    ContentContent,
+    ContentContentAudio,
+    ContentContentChildren,
+    ContentContentCollections,
+    ContentContentDocument,
+    ContentContentEmail,
+    ContentContentEmailBcc,
+    ContentContentEmailCc,
+    ContentContentEmailFrom,
+    ContentContentEmailTo,
+    ContentContentFeed,
+    ContentContentImage,
+    ContentContentIssue,
+    ContentContentLinks,
+    ContentContentObservations,
+    ContentContentObservationsObservable,
+    ContentContentObservationsOccurrences,
+    ContentContentObservationsOccurrencesBoundingBox,
+    ContentContentOwner,
+    ContentContentParent,
+    ContentContentVideo,
+    ContentContentWorkflow,
+)
+from .conversation import (
+    Conversation,
+    ConversationConversation,
+    ConversationConversationFilter,
+    ConversationConversationFilterCollections,
+    ConversationConversationFilterContents,
+    ConversationConversationFilterCreationDateRange,
+    ConversationConversationFilterDateRange,
+    ConversationConversationFilterFeeds,
+    ConversationConversationFilterObservations,
+    ConversationConversationFilterObservationsObservable,
+    ConversationConversationFilterWorkflows,
+    ConversationConversationMessages,
+    ConversationConversationMessagesCitations,
+    ConversationConversationMessagesCitationsContent,
+    ConversationConversationOwner,
+    ConversationConversationSpecification,
+)
 from .create_alert import CreateAlert, CreateAlertCreateAlert
 from .create_collection import CreateCollection, CreateCollectionCreateCollection
 from .create_conversation import (
     CreateConversation,
     CreateConversationCreateConversation,
 )
 from .create_feed import CreateFeed, CreateFeedCreateFeed
@@ -178,157 +247,42 @@
 )
 from .extract_contents import (
     ExtractContents,
     ExtractContentsExtractContents,
     ExtractContentsExtractContentsContent,
     ExtractContentsExtractContentsSpecification,
 )
-from .get_alert import (
-    GetAlert,
-    GetAlertAlert,
-    GetAlertAlertFilter,
-    GetAlertAlertFilterCollections,
-    GetAlertAlertFilterContents,
-    GetAlertAlertFilterCreationDateRange,
-    GetAlertAlertFilterDateRange,
-    GetAlertAlertFilterFeeds,
-    GetAlertAlertFilterObservations,
-    GetAlertAlertFilterObservationsObservable,
-    GetAlertAlertFilterWorkflows,
-    GetAlertAlertIntegration,
-    GetAlertAlertIntegrationSlack,
-    GetAlertAlertOwner,
-    GetAlertAlertPublishing,
-    GetAlertAlertPublishingElevenLabs,
-    GetAlertAlertPublishSpecification,
-    GetAlertAlertSummarySpecification,
-)
-from .get_collection import (
-    GetCollection,
-    GetCollectionCollection,
-    GetCollectionCollectionContents,
-    GetCollectionCollectionOwner,
-)
-from .get_content import (
-    GetContent,
-    GetContentContent,
-    GetContentContentAudio,
-    GetContentContentChildren,
-    GetContentContentCollections,
-    GetContentContentDocument,
-    GetContentContentEmail,
-    GetContentContentEmailBcc,
-    GetContentContentEmailCc,
-    GetContentContentEmailFrom,
-    GetContentContentEmailTo,
-    GetContentContentFeed,
-    GetContentContentImage,
-    GetContentContentIssue,
-    GetContentContentLinks,
-    GetContentContentObservations,
-    GetContentContentObservationsObservable,
-    GetContentContentObservationsOccurrences,
-    GetContentContentObservationsOccurrencesBoundingBox,
-    GetContentContentOwner,
-    GetContentContentParent,
-    GetContentContentVideo,
-    GetContentContentWorkflow,
-)
-from .get_conversation import (
-    GetConversation,
-    GetConversationConversation,
-    GetConversationConversationFilter,
-    GetConversationConversationFilterCollections,
-    GetConversationConversationFilterContents,
-    GetConversationConversationFilterCreationDateRange,
-    GetConversationConversationFilterDateRange,
-    GetConversationConversationFilterFeeds,
-    GetConversationConversationFilterObservations,
-    GetConversationConversationFilterObservationsObservable,
-    GetConversationConversationFilterWorkflows,
-    GetConversationConversationMessages,
-    GetConversationConversationMessagesCitations,
-    GetConversationConversationMessagesCitationsContent,
-    GetConversationConversationOwner,
-    GetConversationConversationSpecification,
-)
-from .get_feed import (
-    GetFeed,
-    GetFeedFeed,
-    GetFeedFeedDiscord,
-    GetFeedFeedEmail,
-    GetFeedFeedEmailGoogle,
-    GetFeedFeedEmailMicrosoft,
-    GetFeedFeedIssue,
-    GetFeedFeedIssueGithub,
-    GetFeedFeedIssueJira,
-    GetFeedFeedIssueLinear,
-    GetFeedFeedNotion,
-    GetFeedFeedOwner,
-    GetFeedFeedReddit,
-    GetFeedFeedRss,
-    GetFeedFeedSchedulePolicy,
-    GetFeedFeedSite,
-    GetFeedFeedSiteAzureBlob,
-    GetFeedFeedSiteAzureFile,
-    GetFeedFeedSiteGoogle,
-    GetFeedFeedSiteGoogleDrive,
-    GetFeedFeedSiteOneDrive,
-    GetFeedFeedSiteS3,
-    GetFeedFeedSiteSharePoint,
-    GetFeedFeedSlack,
-    GetFeedFeedWeb,
-    GetFeedFeedWorkflow,
-    GetFeedFeedYoutube,
-)
-from .get_specification import (
-    GetSpecification,
-    GetSpecificationSpecification,
-    GetSpecificationSpecificationAnthropic,
-    GetSpecificationSpecificationAzureOpenAi,
-    GetSpecificationSpecificationOpenAi,
-    GetSpecificationSpecificationOwner,
-    GetSpecificationSpecificationPromptStrategy,
-    GetSpecificationSpecificationReplicate,
-    GetSpecificationSpecificationRerankingStrategy,
-    GetSpecificationSpecificationRetrievalStrategy,
-    GetSpecificationSpecificationStrategy,
-    GetSpecificationSpecificationTools,
-)
-from .get_workflow import (
-    GetWorkflow,
-    GetWorkflowWorkflow,
-    GetWorkflowWorkflowActions,
-    GetWorkflowWorkflowActionsConnector,
-    GetWorkflowWorkflowActionsConnectorSlack,
-    GetWorkflowWorkflowEnrichment,
-    GetWorkflowWorkflowEnrichmentJobs,
-    GetWorkflowWorkflowEnrichmentJobsConnector,
-    GetWorkflowWorkflowEnrichmentLink,
-    GetWorkflowWorkflowExtraction,
-    GetWorkflowWorkflowExtractionJobs,
-    GetWorkflowWorkflowExtractionJobsConnector,
-    GetWorkflowWorkflowExtractionJobsConnectorAzureImage,
-    GetWorkflowWorkflowExtractionJobsConnectorAzureText,
-    GetWorkflowWorkflowExtractionJobsConnectorModelText,
-    GetWorkflowWorkflowExtractionJobsConnectorModelTextSpecification,
-    GetWorkflowWorkflowExtractionJobsConnectorOpenAiImage,
-    GetWorkflowWorkflowIngestion,
-    GetWorkflowWorkflowIngestionCollections,
-    GetWorkflowWorkflowIngestionIf,
-    GetWorkflowWorkflowOwner,
-    GetWorkflowWorkflowPreparation,
-    GetWorkflowWorkflowPreparationJobs,
-    GetWorkflowWorkflowPreparationJobsConnector,
-    GetWorkflowWorkflowPreparationJobsConnectorAzureDocument,
-    GetWorkflowWorkflowPreparationJobsConnectorDeepgram,
-    GetWorkflowWorkflowPreparationJobsConnectorDocument,
-    GetWorkflowWorkflowPreparationJobsConnectorEmail,
-    GetWorkflowWorkflowPreparationSummarizations,
-    GetWorkflowWorkflowPreparationSummarizationsSpecification,
+from .feed import (
+    Feed,
+    FeedFeed,
+    FeedFeedDiscord,
+    FeedFeedEmail,
+    FeedFeedEmailGoogle,
+    FeedFeedEmailMicrosoft,
+    FeedFeedIssue,
+    FeedFeedIssueGithub,
+    FeedFeedIssueJira,
+    FeedFeedIssueLinear,
+    FeedFeedNotion,
+    FeedFeedOwner,
+    FeedFeedReddit,
+    FeedFeedRss,
+    FeedFeedSchedulePolicy,
+    FeedFeedSite,
+    FeedFeedSiteAzureBlob,
+    FeedFeedSiteAzureFile,
+    FeedFeedSiteGoogle,
+    FeedFeedSiteGoogleDrive,
+    FeedFeedSiteOneDrive,
+    FeedFeedSiteS3,
+    FeedFeedSiteSharePoint,
+    FeedFeedSlack,
+    FeedFeedWeb,
+    FeedFeedWorkflow,
+    FeedFeedYoutube,
 )
 from .ingest_encoded_file import IngestEncodedFile, IngestEncodedFileIngestEncodedFile
 from .ingest_text import IngestText, IngestTextIngestText
 from .ingest_uri import IngestUri, IngestUriIngestUri
 from .input_types import (
     AddressFilter,
     AddressInput,
@@ -514,16 +468,20 @@
 )
 from .is_content_done import IsContentDone, IsContentDoneIsContentDone
 from .is_feed_done import IsFeedDone, IsFeedDoneIsFeedDone
 from .lookup_credits import LookupCredits, LookupCreditsLookupCredits
 from .lookup_usage import LookupUsage, LookupUsageLookupUsage
 from .operations import (
     ADD_CONTENTS_TO_COLLECTIONS_GQL,
+    ALERT_GQL,
     CLEAR_CONVERSATION_GQL,
     CLOSE_CONVERSATION_GQL,
+    COLLECTION_GQL,
+    CONTENT_GQL,
+    CONVERSATION_GQL,
     CREATE_ALERT_GQL,
     CREATE_COLLECTION_GQL,
     CREATE_CONVERSATION_GQL,
     CREATE_FEED_GQL,
     CREATE_SPECIFICATION_GQL,
     CREATE_WORKFLOW_GQL,
     CREDITS_GQL,
@@ -546,21 +504,15 @@
     DELETE_WORKFLOW_GQL,
     DELETE_WORKFLOWS_GQL,
     DISABLE_ALERT_GQL,
     DISABLE_FEED_GQL,
     ENABLE_ALERT_GQL,
     ENABLE_FEED_GQL,
     EXTRACT_CONTENTS_GQL,
-    GET_ALERT_GQL,
-    GET_COLLECTION_GQL,
-    GET_CONTENT_GQL,
-    GET_CONVERSATION_GQL,
-    GET_FEED_GQL,
-    GET_SPECIFICATION_GQL,
-    GET_WORKFLOW_GQL,
+    FEED_GQL,
     INGEST_ENCODED_FILE_GQL,
     INGEST_TEXT_GQL,
     INGEST_URI_GQL,
     IS_CONTENT_DONE_GQL,
     IS_FEED_DONE_GQL,
     LOOKUP_CREDITS_GQL,
     LOOKUP_USAGE_GQL,
@@ -574,25 +526,27 @@
     QUERY_CONTENT_FACETS_GQL,
     QUERY_CONTENTS_GQL,
     QUERY_CONVERSATIONS_GQL,
     QUERY_FEEDS_GQL,
     QUERY_SPECIFICATIONS_GQL,
     QUERY_WORKFLOWS_GQL,
     REMOVE_CONTENTS_FROM_COLLECTION_GQL,
+    SPECIFICATION_GQL,
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
+    WORKFLOW_GQL,
 )
 from .project import (
     Project,
     ProjectProject,
     ProjectProjectQuota,
     ProjectProjectSpecification,
     ProjectProjectWorkflow,
@@ -781,14 +735,28 @@
     QueryWorkflowsWorkflowsResultsPreparationSummarizationsSpecification,
 )
 from .remove_contents_from_collection import (
     RemoveContentsFromCollection,
     RemoveContentsFromCollectionRemoveContentsFromCollection,
     RemoveContentsFromCollectionRemoveContentsFromCollectionContents,
 )
+from .specification import (
+    Specification,
+    SpecificationSpecification,
+    SpecificationSpecificationAnthropic,
+    SpecificationSpecificationAzureOpenAi,
+    SpecificationSpecificationOpenAi,
+    SpecificationSpecificationOwner,
+    SpecificationSpecificationPromptStrategy,
+    SpecificationSpecificationReplicate,
+    SpecificationSpecificationRerankingStrategy,
+    SpecificationSpecificationRetrievalStrategy,
+    SpecificationSpecificationStrategy,
+    SpecificationSpecificationTools,
+)
 from .suggest_conversation import (
     SuggestConversation,
     SuggestConversationSuggestConversation,
 )
 from .summarize_contents import (
     SummarizeContents,
     SummarizeContentsSummarizeContents,
@@ -837,22 +805,73 @@
     UpdateWorkflowUpdateWorkflowPreparationJobsConnectorDeepgram,
     UpdateWorkflowUpdateWorkflowPreparationJobsConnectorDocument,
     UpdateWorkflowUpdateWorkflowPreparationJobsConnectorEmail,
     UpdateWorkflowUpdateWorkflowPreparationSummarizations,
     UpdateWorkflowUpdateWorkflowPreparationSummarizationsSpecification,
 )
 from .usage import Usage, UsageUsage
+from .workflow import (
+    Workflow,
+    WorkflowWorkflow,
+    WorkflowWorkflowActions,
+    WorkflowWorkflowActionsConnector,
+    WorkflowWorkflowActionsConnectorSlack,
+    WorkflowWorkflowEnrichment,
+    WorkflowWorkflowEnrichmentJobs,
+    WorkflowWorkflowEnrichmentJobsConnector,
+    WorkflowWorkflowEnrichmentLink,
+    WorkflowWorkflowExtraction,
+    WorkflowWorkflowExtractionJobs,
+    WorkflowWorkflowExtractionJobsConnector,
+    WorkflowWorkflowExtractionJobsConnectorAzureImage,
+    WorkflowWorkflowExtractionJobsConnectorAzureText,
+    WorkflowWorkflowExtractionJobsConnectorModelText,
+    WorkflowWorkflowExtractionJobsConnectorModelTextSpecification,
+    WorkflowWorkflowExtractionJobsConnectorOpenAiImage,
+    WorkflowWorkflowIngestion,
+    WorkflowWorkflowIngestionCollections,
+    WorkflowWorkflowIngestionIf,
+    WorkflowWorkflowOwner,
+    WorkflowWorkflowPreparation,
+    WorkflowWorkflowPreparationJobs,
+    WorkflowWorkflowPreparationJobsConnector,
+    WorkflowWorkflowPreparationJobsConnectorAzureDocument,
+    WorkflowWorkflowPreparationJobsConnectorDeepgram,
+    WorkflowWorkflowPreparationJobsConnectorDocument,
+    WorkflowWorkflowPreparationJobsConnectorEmail,
+    WorkflowWorkflowPreparationSummarizations,
+    WorkflowWorkflowPreparationSummarizationsSpecification,
+)
 
 __all__ = [
     "ADD_CONTENTS_TO_COLLECTIONS_GQL",
+    "ALERT_GQL",
     "AddContentsToCollections",
     "AddContentsToCollectionsAddContentsToCollections",
     "AddContentsToCollectionsAddContentsToCollectionsContents",
     "AddressFilter",
     "AddressInput",
+    "Alert",
+    "AlertAlert",
+    "AlertAlertFilter",
+    "AlertAlertFilterCollections",
+    "AlertAlertFilterContents",
+    "AlertAlertFilterCreationDateRange",
+    "AlertAlertFilterDateRange",
+    "AlertAlertFilterFeeds",
+    "AlertAlertFilterObservations",
+    "AlertAlertFilterObservationsObservable",
+    "AlertAlertFilterWorkflows",
+    "AlertAlertIntegration",
+    "AlertAlertIntegrationSlack",
+    "AlertAlertOwner",
+    "AlertAlertPublishSpecification",
+    "AlertAlertPublishing",
+    "AlertAlertPublishingElevenLabs",
+    "AlertAlertSummarySpecification",
     "AlertFilter",
     "AlertInput",
     "AlertSchedulePolicyInput",
     "AlertTypes",
     "AlertUpdateInput",
     "AmazonFeedPropertiesInput",
     "AmazonFeedPropertiesUpdateInput",
@@ -875,14 +894,17 @@
     "AzureOpenAIModels",
     "AzureTextExtractionPropertiesInput",
     "BaseModel",
     "BillableMetrics",
     "BoundingBoxInput",
     "CLEAR_CONVERSATION_GQL",
     "CLOSE_CONVERSATION_GQL",
+    "COLLECTION_GQL",
+    "CONTENT_GQL",
+    "CONVERSATION_GQL",
     "CREATE_ALERT_GQL",
     "CREATE_COLLECTION_GQL",
     "CREATE_CONVERSATION_GQL",
     "CREATE_FEED_GQL",
     "CREATE_SPECIFICATION_GQL",
     "CREATE_WORKFLOW_GQL",
     "CREDITS_GQL",
@@ -892,29 +914,72 @@
     "CategoryInput",
     "CategoryUpdateInput",
     "ClearConversation",
     "ClearConversationClearConversation",
     "Client",
     "CloseConversation",
     "CloseConversationCloseConversation",
+    "Collection",
+    "CollectionCollection",
+    "CollectionCollectionContents",
+    "CollectionCollectionOwner",
     "CollectionFilter",
     "CollectionInput",
     "CollectionTypes",
     "CollectionUpdateInput",
+    "Content",
+    "ContentContent",
+    "ContentContentAudio",
+    "ContentContentChildren",
+    "ContentContentCollections",
+    "ContentContentDocument",
+    "ContentContentEmail",
+    "ContentContentEmailBcc",
+    "ContentContentEmailCc",
+    "ContentContentEmailFrom",
+    "ContentContentEmailTo",
+    "ContentContentFeed",
+    "ContentContentImage",
+    "ContentContentIssue",
+    "ContentContentLinks",
+    "ContentContentObservations",
+    "ContentContentObservationsObservable",
+    "ContentContentObservationsOccurrences",
+    "ContentContentObservationsOccurrencesBoundingBox",
+    "ContentContentOwner",
+    "ContentContentParent",
+    "ContentContentVideo",
+    "ContentContentWorkflow",
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
+    "Conversation",
+    "ConversationConversation",
+    "ConversationConversationFilter",
+    "ConversationConversationFilterCollections",
+    "ConversationConversationFilterContents",
+    "ConversationConversationFilterCreationDateRange",
+    "ConversationConversationFilterDateRange",
+    "ConversationConversationFilterFeeds",
+    "ConversationConversationFilterObservations",
+    "ConversationConversationFilterObservationsObservable",
+    "ConversationConversationFilterWorkflows",
+    "ConversationConversationMessages",
+    "ConversationConversationMessagesCitations",
+    "ConversationConversationMessagesCitationsContent",
+    "ConversationConversationOwner",
+    "ConversationConversationSpecification",
     "ConversationFilter",
     "ConversationInput",
     "ConversationRoleTypes",
     "ConversationSearchTypes",
     "ConversationStrategyInput",
     "ConversationStrategyTypes",
     "ConversationStrategyUpdateInput",
@@ -1060,163 +1125,54 @@
     "EventUpdateInput",
     "ExtractContents",
     "ExtractContentsExtractContents",
     "ExtractContentsExtractContentsContent",
     "ExtractContentsExtractContentsSpecification",
     "ExtractionWorkflowJobInput",
     "ExtractionWorkflowStageInput",
+    "FEED_GQL",
     "FacetValueTypes",
+    "Feed",
     "FeedConnectorTypes",
+    "FeedFeed",
+    "FeedFeedDiscord",
+    "FeedFeedEmail",
+    "FeedFeedEmailGoogle",
+    "FeedFeedEmailMicrosoft",
+    "FeedFeedIssue",
+    "FeedFeedIssueGithub",
+    "FeedFeedIssueJira",
+    "FeedFeedIssueLinear",
+    "FeedFeedNotion",
+    "FeedFeedOwner",
+    "FeedFeedReddit",
+    "FeedFeedRss",
+    "FeedFeedSchedulePolicy",
+    "FeedFeedSite",
+    "FeedFeedSiteAzureBlob",
+    "FeedFeedSiteAzureFile",
+    "FeedFeedSiteGoogle",
+    "FeedFeedSiteGoogleDrive",
+    "FeedFeedSiteOneDrive",
+    "FeedFeedSiteS3",
+    "FeedFeedSiteSharePoint",
+    "FeedFeedSlack",
+    "FeedFeedWeb",
+    "FeedFeedWorkflow",
+    "FeedFeedYoutube",
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
-    "GET_ALERT_GQL",
-    "GET_COLLECTION_GQL",
-    "GET_CONTENT_GQL",
-    "GET_CONVERSATION_GQL",
-    "GET_FEED_GQL",
-    "GET_SPECIFICATION_GQL",
-    "GET_WORKFLOW_GQL",
-    "GetAlert",
-    "GetAlertAlert",
-    "GetAlertAlertFilter",
-    "GetAlertAlertFilterCollections",
-    "GetAlertAlertFilterContents",
-    "GetAlertAlertFilterCreationDateRange",
-    "GetAlertAlertFilterDateRange",
-    "GetAlertAlertFilterFeeds",
-    "GetAlertAlertFilterObservations",
-    "GetAlertAlertFilterObservationsObservable",
-    "GetAlertAlertFilterWorkflows",
-    "GetAlertAlertIntegration",
-    "GetAlertAlertIntegrationSlack",
-    "GetAlertAlertOwner",
-    "GetAlertAlertPublishSpecification",
-    "GetAlertAlertPublishing",
-    "GetAlertAlertPublishingElevenLabs",
-    "GetAlertAlertSummarySpecification",
-    "GetCollection",
-    "GetCollectionCollection",
-    "GetCollectionCollectionContents",
-    "GetCollectionCollectionOwner",
-    "GetContent",
-    "GetContentContent",
-    "GetContentContentAudio",
-    "GetContentContentChildren",
-    "GetContentContentCollections",
-    "GetContentContentDocument",
-    "GetContentContentEmail",
-    "GetContentContentEmailBcc",
-    "GetContentContentEmailCc",
-    "GetContentContentEmailFrom",
-    "GetContentContentEmailTo",
-    "GetContentContentFeed",
-    "GetContentContentImage",
-    "GetContentContentIssue",
-    "GetContentContentLinks",
-    "GetContentContentObservations",
-    "GetContentContentObservationsObservable",
-    "GetContentContentObservationsOccurrences",
-    "GetContentContentObservationsOccurrencesBoundingBox",
-    "GetContentContentOwner",
-    "GetContentContentParent",
-    "GetContentContentVideo",
-    "GetContentContentWorkflow",
-    "GetConversation",
-    "GetConversationConversation",
-    "GetConversationConversationFilter",
-    "GetConversationConversationFilterCollections",
-    "GetConversationConversationFilterContents",
-    "GetConversationConversationFilterCreationDateRange",
-    "GetConversationConversationFilterDateRange",
-    "GetConversationConversationFilterFeeds",
-    "GetConversationConversationFilterObservations",
-    "GetConversationConversationFilterObservationsObservable",
-    "GetConversationConversationFilterWorkflows",
-    "GetConversationConversationMessages",
-    "GetConversationConversationMessagesCitations",
-    "GetConversationConversationMessagesCitationsContent",
-    "GetConversationConversationOwner",
-    "GetConversationConversationSpecification",
-    "GetFeed",
-    "GetFeedFeed",
-    "GetFeedFeedDiscord",
-    "GetFeedFeedEmail",
-    "GetFeedFeedEmailGoogle",
-    "GetFeedFeedEmailMicrosoft",
-    "GetFeedFeedIssue",
-    "GetFeedFeedIssueGithub",
-    "GetFeedFeedIssueJira",
-    "GetFeedFeedIssueLinear",
-    "GetFeedFeedNotion",
-    "GetFeedFeedOwner",
-    "GetFeedFeedReddit",
-    "GetFeedFeedRss",
-    "GetFeedFeedSchedulePolicy",
-    "GetFeedFeedSite",
-    "GetFeedFeedSiteAzureBlob",
-    "GetFeedFeedSiteAzureFile",
-    "GetFeedFeedSiteGoogle",
-    "GetFeedFeedSiteGoogleDrive",
-    "GetFeedFeedSiteOneDrive",
-    "GetFeedFeedSiteS3",
-    "GetFeedFeedSiteSharePoint",
-    "GetFeedFeedSlack",
-    "GetFeedFeedWeb",
-    "GetFeedFeedWorkflow",
-    "GetFeedFeedYoutube",
-    "GetSpecification",
-    "GetSpecificationSpecification",
-    "GetSpecificationSpecificationAnthropic",
-    "GetSpecificationSpecificationAzureOpenAi",
-    "GetSpecificationSpecificationOpenAi",
-    "GetSpecificationSpecificationOwner",
-    "GetSpecificationSpecificationPromptStrategy",
-    "GetSpecificationSpecificationReplicate",
-    "GetSpecificationSpecificationRerankingStrategy",
-    "GetSpecificationSpecificationRetrievalStrategy",
-    "GetSpecificationSpecificationStrategy",
-    "GetSpecificationSpecificationTools",
-    "GetWorkflow",
-    "GetWorkflowWorkflow",
-    "GetWorkflowWorkflowActions",
-    "GetWorkflowWorkflowActionsConnector",
-    "GetWorkflowWorkflowActionsConnectorSlack",
-    "GetWorkflowWorkflowEnrichment",
-    "GetWorkflowWorkflowEnrichmentJobs",
-    "GetWorkflowWorkflowEnrichmentJobsConnector",
-    "GetWorkflowWorkflowEnrichmentLink",
-    "GetWorkflowWorkflowExtraction",
-    "GetWorkflowWorkflowExtractionJobs",
-    "GetWorkflowWorkflowExtractionJobsConnector",
-    "GetWorkflowWorkflowExtractionJobsConnectorAzureImage",
-    "GetWorkflowWorkflowExtractionJobsConnectorAzureText",
-    "GetWorkflowWorkflowExtractionJobsConnectorModelText",
-    "GetWorkflowWorkflowExtractionJobsConnectorModelTextSpecification",
-    "GetWorkflowWorkflowExtractionJobsConnectorOpenAiImage",
-    "GetWorkflowWorkflowIngestion",
-    "GetWorkflowWorkflowIngestionCollections",
-    "GetWorkflowWorkflowIngestionIf",
-    "GetWorkflowWorkflowOwner",
-    "GetWorkflowWorkflowPreparation",
-    "GetWorkflowWorkflowPreparationJobs",
-    "GetWorkflowWorkflowPreparationJobsConnector",
-    "GetWorkflowWorkflowPreparationJobsConnectorAzureDocument",
-    "GetWorkflowWorkflowPreparationJobsConnectorDeepgram",
-    "GetWorkflowWorkflowPreparationJobsConnectorDocument",
-    "GetWorkflowWorkflowPreparationJobsConnectorEmail",
-    "GetWorkflowWorkflowPreparationSummarizations",
-    "GetWorkflowWorkflowPreparationSummarizationsSpecification",
     "GitHubIssuesFeedPropertiesInput",
     "GitHubIssuesFeedPropertiesUpdateInput",
     "GoogleDriveFeedPropertiesInput",
     "GoogleDriveFeedPropertiesUpdateInput",
     "GoogleEmailFeedPropertiesInput",
     "GoogleEmailFeedPropertiesUpdateInput",
     "GoogleFeedPropertiesInput",
@@ -1537,14 +1493,15 @@
     "RepoUpdateInput",
     "RerankingStrategyInput",
     "RerankingStrategyUpdateInput",
     "ResourceConnectorTypes",
     "RetrievalStrategyInput",
     "RetrievalStrategyTypes",
     "RetrievalStrategyUpdateInput",
+    "SPECIFICATION_GQL",
     "SUGGEST_CONVERSATION_GQL",
     "SUMMARIZE_CONTENTS_GQL",
     "SearchQueryTypes",
     "SearchTypes",
     "SharePointAuthenticationTypes",
     "SharePointFeedPropertiesInput",
     "SharePointFeedPropertiesUpdateInput",
@@ -1556,16 +1513,28 @@
     "SlackFeedPropertiesUpdateInput",
     "SlackIntegrationPropertiesInput",
     "SoftwareFacetInput",
     "SoftwareFacetTypes",
     "SoftwareFilter",
     "SoftwareInput",
     "SoftwareUpdateInput",
+    "Specification",
     "SpecificationFilter",
     "SpecificationInput",
+    "SpecificationSpecification",
+    "SpecificationSpecificationAnthropic",
+    "SpecificationSpecificationAzureOpenAi",
+    "SpecificationSpecificationOpenAi",
+    "SpecificationSpecificationOwner",
+    "SpecificationSpecificationPromptStrategy",
+    "SpecificationSpecificationReplicate",
+    "SpecificationSpecificationRerankingStrategy",
+    "SpecificationSpecificationRetrievalStrategy",
+    "SpecificationSpecificationStrategy",
+    "SpecificationSpecificationTools",
     "SpecificationTypes",
     "SpecificationUpdateInput",
     "SuggestConversation",
     "SuggestConversationSuggestConversation",
     "SummarizationStrategyInput",
     "SummarizationTypes",
     "SummarizeContents",
@@ -1631,17 +1600,48 @@
     "UpdateWorkflowUpdateWorkflowPreparationJobsConnectorDocument",
     "UpdateWorkflowUpdateWorkflowPreparationJobsConnectorEmail",
     "UpdateWorkflowUpdateWorkflowPreparationSummarizations",
     "UpdateWorkflowUpdateWorkflowPreparationSummarizationsSpecification",
     "Upload",
     "Usage",
     "UsageUsage",
+    "WORKFLOW_GQL",
     "WebFeedPropertiesInput",
     "WebFeedPropertiesUpdateInput",
+    "Workflow",
     "WorkflowActionInput",
     "WorkflowFilter",
     "WorkflowInput",
     "WorkflowUpdateInput",
+    "WorkflowWorkflow",
+    "WorkflowWorkflowActions",
+    "WorkflowWorkflowActionsConnector",
+    "WorkflowWorkflowActionsConnectorSlack",
+    "WorkflowWorkflowEnrichment",
+    "WorkflowWorkflowEnrichmentJobs",
+    "WorkflowWorkflowEnrichmentJobsConnector",
+    "WorkflowWorkflowEnrichmentLink",
+    "WorkflowWorkflowExtraction",
+    "WorkflowWorkflowExtractionJobs",
+    "WorkflowWorkflowExtractionJobsConnector",
+    "WorkflowWorkflowExtractionJobsConnectorAzureImage",
+    "WorkflowWorkflowExtractionJobsConnectorAzureText",
+    "WorkflowWorkflowExtractionJobsConnectorModelText",
+    "WorkflowWorkflowExtractionJobsConnectorModelTextSpecification",
+    "WorkflowWorkflowExtractionJobsConnectorOpenAiImage",
+    "WorkflowWorkflowIngestion",
+    "WorkflowWorkflowIngestionCollections",
+    "WorkflowWorkflowIngestionIf",
+    "WorkflowWorkflowOwner",
+    "WorkflowWorkflowPreparation",
+    "WorkflowWorkflowPreparationJobs",
+    "WorkflowWorkflowPreparationJobsConnector",
+    "WorkflowWorkflowPreparationJobsConnectorAzureDocument",
+    "WorkflowWorkflowPreparationJobsConnectorDeepgram",
+    "WorkflowWorkflowPreparationJobsConnectorDocument",
+    "WorkflowWorkflowPreparationJobsConnectorEmail",
+    "WorkflowWorkflowPreparationSummarizations",
+    "WorkflowWorkflowPreparationSummarizationsSpecification",
     "YouTubeFeedPropertiesInput",
     "YouTubeFeedPropertiesUpdateInput",
     "YouTubeTypes",
 ]
```

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/add_contents_to_collections.py` & `graphlit_client-1.0.20240420001/graphlit_api/add_contents_to_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/async_base_client.py` & `graphlit_client-1.0.20240420001/graphlit_api/async_base_client.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/base_model.py` & `graphlit_client-1.0.20240420001/graphlit_api/base_model.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/clear_conversation.py` & `graphlit_client-1.0.20240420001/graphlit_api/clear_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/client.py` & `graphlit_client-1.0.20240420001/graphlit_api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # Generated by ariadne-codegen
 # Source: ./documents
 
 from typing import Any, Dict, List, Optional, Union
 
 from .add_contents_to_collections import AddContentsToCollections
+from .alert import Alert
 from .async_base_client import AsyncBaseClient
 from .base_model import UNSET, UnsetType
 from .clear_conversation import ClearConversation
 from .close_conversation import CloseConversation
+from .collection import Collection
+from .content import Content
+from .conversation import Conversation
 from .create_alert import CreateAlert
 from .create_collection import CreateCollection
 from .create_conversation import CreateConversation
 from .create_feed import CreateFeed
 from .create_specification import CreateSpecification
 from .create_workflow import CreateWorkflow
 from .credits import Credits
@@ -35,21 +39,15 @@
 from .delete_workflows import DeleteWorkflows
 from .disable_alert import DisableAlert
 from .disable_feed import DisableFeed
 from .enable_alert import EnableAlert
 from .enable_feed import EnableFeed
 from .enums import TextTypes
 from .extract_contents import ExtractContents
-from .get_alert import GetAlert
-from .get_collection import GetCollection
-from .get_content import GetContent
-from .get_conversation import GetConversation
-from .get_feed import GetFeed
-from .get_specification import GetSpecification
-from .get_workflow import GetWorkflow
+from .feed import Feed
 from .ingest_encoded_file import IngestEncodedFile
 from .ingest_text import IngestText
 from .ingest_uri import IngestUri
 from .input_types import (
     AlertFilter,
     AlertInput,
     AlertUpdateInput,
@@ -78,16 +76,20 @@
 )
 from .is_content_done import IsContentDone
 from .is_feed_done import IsFeedDone
 from .lookup_credits import LookupCredits
 from .lookup_usage import LookupUsage
 from .operations import (
     ADD_CONTENTS_TO_COLLECTIONS_GQL,
+    ALERT_GQL,
     CLEAR_CONVERSATION_GQL,
     CLOSE_CONVERSATION_GQL,
+    COLLECTION_GQL,
+    CONTENT_GQL,
+    CONVERSATION_GQL,
     CREATE_ALERT_GQL,
     CREATE_COLLECTION_GQL,
     CREATE_CONVERSATION_GQL,
     CREATE_FEED_GQL,
     CREATE_SPECIFICATION_GQL,
     CREATE_WORKFLOW_GQL,
     CREDITS_GQL,
@@ -110,21 +112,15 @@
     DELETE_WORKFLOW_GQL,
     DELETE_WORKFLOWS_GQL,
     DISABLE_ALERT_GQL,
     DISABLE_FEED_GQL,
     ENABLE_ALERT_GQL,
     ENABLE_FEED_GQL,
     EXTRACT_CONTENTS_GQL,
-    GET_ALERT_GQL,
-    GET_COLLECTION_GQL,
-    GET_CONTENT_GQL,
-    GET_CONVERSATION_GQL,
-    GET_FEED_GQL,
-    GET_SPECIFICATION_GQL,
-    GET_WORKFLOW_GQL,
+    FEED_GQL,
     INGEST_ENCODED_FILE_GQL,
     INGEST_TEXT_GQL,
     INGEST_URI_GQL,
     IS_CONTENT_DONE_GQL,
     IS_FEED_DONE_GQL,
     LOOKUP_CREDITS_GQL,
     LOOKUP_USAGE_GQL,
@@ -138,25 +134,27 @@
     QUERY_CONTENT_FACETS_GQL,
     QUERY_CONTENTS_GQL,
     QUERY_CONVERSATIONS_GQL,
     QUERY_FEEDS_GQL,
     QUERY_SPECIFICATIONS_GQL,
     QUERY_WORKFLOWS_GQL,
     REMOVE_CONTENTS_FROM_COLLECTION_GQL,
+    SPECIFICATION_GQL,
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
+    WORKFLOW_GQL,
 )
 from .project import Project
 from .prompt_conversation import PromptConversation
 from .prompt_specifications import PromptSpecifications
 from .publish_contents import PublishContents
 from .publish_conversation import PublishConversation
 from .query_alerts import QueryAlerts
@@ -164,25 +162,27 @@
 from .query_content_facets import QueryContentFacets
 from .query_contents import QueryContents
 from .query_conversations import QueryConversations
 from .query_feeds import QueryFeeds
 from .query_specifications import QuerySpecifications
 from .query_workflows import QueryWorkflows
 from .remove_contents_from_collection import RemoveContentsFromCollection
+from .specification import Specification
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
+from .workflow import Workflow
 
 
 def gql(q: str) -> str:
     return q
 
 
 class Client(AsyncBaseClient):
@@ -253,24 +253,21 @@
             operation_name="EnableAlert",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return EnableAlert.model_validate(data)
 
-    async def get_alert(self, id: str, **kwargs: Any) -> GetAlert:
+    async def get_alert(self, id: str, **kwargs: Any) -> Alert:
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
-            query=GET_ALERT_GQL,
-            operation_name="GetAlert",
-            variables=variables,
-            **kwargs
+            query=ALERT_GQL, operation_name="Alert", variables=variables, **kwargs
         )
         data = self.get_data(response)
-        return GetAlert.model_validate(data)
+        return Alert.model_validate(data)
 
     async def query_alerts(
         self, filter: Union[Optional[AlertFilter], UnsetType] = UNSET, **kwargs: Any
     ) -> QueryAlerts:
         variables: Dict[str, object] = {"filter": filter}
         response = await self.execute(
             query=QUERY_ALERTS_GQL,
@@ -344,24 +341,24 @@
             operation_name="DeleteCollections",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteCollections.model_validate(data)
 
-    async def get_collection(self, id: str, **kwargs: Any) -> GetCollection:
+    async def get_collection(self, id: str, **kwargs: Any) -> Collection:
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
-            query=GET_COLLECTION_GQL,
-            operation_name="GetCollection",
+            query=COLLECTION_GQL,
+            operation_name="Collection",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
-        return GetCollection.model_validate(data)
+        return Collection.model_validate(data)
 
     async def query_collections(
         self,
         filter: Union[Optional[CollectionFilter], UnsetType] = UNSET,
         **kwargs: Any
     ) -> QueryCollections:
         variables: Dict[str, object] = {"filter": filter}
@@ -455,24 +452,21 @@
             operation_name="ExtractContents",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return ExtractContents.model_validate(data)
 
-    async def get_content(self, id: str, **kwargs: Any) -> GetContent:
+    async def get_content(self, id: str, **kwargs: Any) -> Content:
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
-            query=GET_CONTENT_GQL,
-            operation_name="GetContent",
-            variables=variables,
-            **kwargs
+            query=CONTENT_GQL, operation_name="Content", variables=variables, **kwargs
         )
         data = self.get_data(response)
-        return GetContent.model_validate(data)
+        return Content.model_validate(data)
 
     async def ingest_encoded_file(
         self,
         name: str,
         data: str,
         mime_type: str,
         id: Union[Optional[str], UnsetType] = UNSET,
@@ -736,24 +730,24 @@
             operation_name="DeleteConversations",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteConversations.model_validate(data)
 
-    async def get_conversation(self, id: str, **kwargs: Any) -> GetConversation:
+    async def get_conversation(self, id: str, **kwargs: Any) -> Conversation:
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
-            query=GET_CONVERSATION_GQL,
-            operation_name="GetConversation",
+            query=CONVERSATION_GQL,
+            operation_name="Conversation",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
-        return GetConversation.model_validate(data)
+        return Conversation.model_validate(data)
 
     async def prompt_conversation(
         self,
         prompt: str,
         id: Union[Optional[str], UnsetType] = UNSET,
         correlation_id: Union[Optional[str], UnsetType] = UNSET,
         **kwargs: Any
@@ -913,21 +907,21 @@
             operation_name="EnableFeed",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return EnableFeed.model_validate(data)
 
-    async def get_feed(self, id: str, **kwargs: Any) -> GetFeed:
+    async def get_feed(self, id: str, **kwargs: Any) -> Feed:
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
-            query=GET_FEED_GQL, operation_name="GetFeed", variables=variables, **kwargs
+            query=FEED_GQL, operation_name="Feed", variables=variables, **kwargs
         )
         data = self.get_data(response)
-        return GetFeed.model_validate(data)
+        return Feed.model_validate(data)
 
     async def is_feed_done(self, id: str, **kwargs: Any) -> IsFeedDone:
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
             query=IS_FEED_DONE_GQL,
             operation_name="IsFeedDone",
             variables=variables,
@@ -986,15 +980,15 @@
             operation_name="LookupUsage",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return LookupUsage.model_validate(data)
 
-    async def project(self, **kwargs: Any) -> Project:
+    async def get_project(self, **kwargs: Any) -> Project:
         variables: Dict[str, object] = {}
         response = await self.execute(
             query=PROJECT_GQL, operation_name="Project", variables=variables, **kwargs
         )
         data = self.get_data(response)
         return Project.model_validate(data)
 
@@ -1039,24 +1033,24 @@
             operation_name="DeleteSpecification",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteSpecification.model_validate(data)
 
-    async def get_specification(self, id: str, **kwargs: Any) -> GetSpecification:
+    async def get_specification(self, id: str, **kwargs: Any) -> Specification:
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
-            query=GET_SPECIFICATION_GQL,
-            operation_name="GetSpecification",
+            query=SPECIFICATION_GQL,
+            operation_name="Specification",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
-        return GetSpecification.model_validate(data)
+        return Specification.model_validate(data)
 
     async def prompt_specifications(
         self, prompt: str, ids: List[str], **kwargs: Any
     ) -> PromptSpecifications:
         variables: Dict[str, object] = {"prompt": prompt, "ids": ids}
         response = await self.execute(
             query=PROMPT_SPECIFICATIONS_GQL,
@@ -1137,24 +1131,21 @@
             operation_name="DeleteWorkflows",
             variables=variables,
             **kwargs
         )
         data = self.get_data(response)
         return DeleteWorkflows.model_validate(data)
 
-    async def get_workflow(self, id: str, **kwargs: Any) -> GetWorkflow:
+    async def get_workflow(self, id: str, **kwargs: Any) -> Workflow:
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
-            query=GET_WORKFLOW_GQL,
-            operation_name="GetWorkflow",
-            variables=variables,
-            **kwargs
+            query=WORKFLOW_GQL, operation_name="Workflow", variables=variables, **kwargs
         )
         data = self.get_data(response)
-        return GetWorkflow.model_validate(data)
+        return Workflow.model_validate(data)
 
     async def query_workflows(
         self, filter: Union[Optional[WorkflowFilter], UnsetType] = UNSET, **kwargs: Any
     ) -> QueryWorkflows:
         variables: Dict[str, object] = {"filter": filter}
         response = await self.execute(
             query=QUERY_WORKFLOWS_GQL,
```

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/close_conversation.py` & `graphlit_client-1.0.20240420001/graphlit_api/close_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/create_collection.py` & `graphlit_client-1.0.20240420001/graphlit_api/create_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/create_conversation.py` & `graphlit_client-1.0.20240420001/graphlit_api/create_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/create_specification.py` & `graphlit_client-1.0.20240420001/graphlit_api/create_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/create_workflow.py` & `graphlit_client-1.0.20240420001/graphlit_api/create_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/credits.py` & `graphlit_client-1.0.20240420001/graphlit_api/credits.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/delete_all_conversations.py` & `graphlit_client-1.0.20240420001/graphlit_api/delete_all_conversations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/enums.py` & `graphlit_client-1.0.20240420001/graphlit_api/enums.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/exceptions.py` & `graphlit_client-1.0.20240420001/graphlit_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/extract_contents.py` & `graphlit_client-1.0.20240420001/graphlit_api/extract_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/get_content.py` & `graphlit_client-1.0.20240420001/graphlit_api/content.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     MailPriority,
     MailSensitivity,
     ObservableTypes,
     OccurrenceTypes,
 )
 
 
-class GetContent(BaseModel):
-    content: Optional["GetContentContent"]
+class Content(BaseModel):
+    content: Optional["ContentContent"]
 
 
-class GetContentContent(BaseModel):
+class ContentContent(BaseModel):
     id: str
     name: str
     creation_date: Any = Field(alias="creationDate")
-    owner: "GetContentContentOwner"
+    owner: "ContentContentOwner"
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
-    video: Optional["GetContentContentVideo"]
-    audio: Optional["GetContentContentAudio"]
-    image: Optional["GetContentContentImage"]
-    document: Optional["GetContentContentDocument"]
-    email: Optional["GetContentContentEmail"]
-    issue: Optional["GetContentContentIssue"]
-    observations: Optional[List[Optional["GetContentContentObservations"]]]
-    parent: Optional["GetContentContentParent"]
-    children: Optional[List[Optional["GetContentContentChildren"]]]
-    collections: Optional[List[Optional["GetContentContentCollections"]]]
-    feed: Optional["GetContentContentFeed"]
-    workflow: Optional["GetContentContentWorkflow"]
+    video: Optional["ContentContentVideo"]
+    audio: Optional["ContentContentAudio"]
+    image: Optional["ContentContentImage"]
+    document: Optional["ContentContentDocument"]
+    email: Optional["ContentContentEmail"]
+    issue: Optional["ContentContentIssue"]
+    observations: Optional[List[Optional["ContentContentObservations"]]]
+    parent: Optional["ContentContentParent"]
+    children: Optional[List[Optional["ContentContentChildren"]]]
+    collections: Optional[List[Optional["ContentContentCollections"]]]
+    feed: Optional["ContentContentFeed"]
+    workflow: Optional["ContentContentWorkflow"]
     markdown: Optional[str]
-    links: Optional[List["GetContentContentLinks"]]
+    links: Optional[List["ContentContentLinks"]]
     error: Optional[str]
 
 
-class GetContentContentOwner(BaseModel):
+class ContentContentOwner(BaseModel):
     id: str
 
 
-class GetContentContentVideo(BaseModel):
+class ContentContentVideo(BaseModel):
     width: Optional[int]
     height: Optional[int]
     duration: Optional[str]
     software: Optional[str]
     make: Optional[str]
     model: Optional[str]
 
 
-class GetContentContentAudio(BaseModel):
+class ContentContentAudio(BaseModel):
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
 
 
-class GetContentContentImage(BaseModel):
+class ContentContentImage(BaseModel):
     width: Optional[int]
     height: Optional[int]
     description: Optional[str]
     software: Optional[str]
     identifier: Optional[str]
     make: Optional[str]
     model: Optional[str]
 
 
-class GetContentContentDocument(BaseModel):
+class ContentContentDocument(BaseModel):
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
 
 
-class GetContentContentEmail(BaseModel):
+class ContentContentEmail(BaseModel):
     subject: Optional[str]
     identifier: Optional[str]
     sensitivity: Optional[MailSensitivity]
     priority: Optional[MailPriority]
     importance: Optional[MailImportance]
     labels: Optional[List[Optional[str]]]
-    from_: Optional[List[Optional["GetContentContentEmailFrom"]]] = Field(alias="from")
-    to: Optional[List[Optional["GetContentContentEmailTo"]]]
-    cc: Optional[List[Optional["GetContentContentEmailCc"]]]
-    bcc: Optional[List[Optional["GetContentContentEmailBcc"]]]
+    from_: Optional[List[Optional["ContentContentEmailFrom"]]] = Field(alias="from")
+    to: Optional[List[Optional["ContentContentEmailTo"]]]
+    cc: Optional[List[Optional["ContentContentEmailCc"]]]
+    bcc: Optional[List[Optional["ContentContentEmailBcc"]]]
 
 
-class GetContentContentEmailFrom(BaseModel):
+class ContentContentEmailFrom(BaseModel):
     name: Optional[str]
     family_name: Optional[str] = Field(alias="familyName")
     given_name: Optional[str] = Field(alias="givenName")
     email: Optional[str]
 
 
-class GetContentContentEmailTo(BaseModel):
+class ContentContentEmailTo(BaseModel):
     name: Optional[str]
     family_name: Optional[str] = Field(alias="familyName")
     given_name: Optional[str] = Field(alias="givenName")
     email: Optional[str]
 
 
-class GetContentContentEmailCc(BaseModel):
+class ContentContentEmailCc(BaseModel):
     name: Optional[str]
     family_name: Optional[str] = Field(alias="familyName")
     given_name: Optional[str] = Field(alias="givenName")
     email: Optional[str]
 
 
-class GetContentContentEmailBcc(BaseModel):
+class ContentContentEmailBcc(BaseModel):
     name: Optional[str]
     family_name: Optional[str] = Field(alias="familyName")
     given_name: Optional[str] = Field(alias="givenName")
     email: Optional[str]
 
 
-class GetContentContentIssue(BaseModel):
+class ContentContentIssue(BaseModel):
     title: Optional[str]
     project: Optional[str]
     team: Optional[str]
     status: Optional[str]
     priority: Optional[str]
     type: Optional[str]
     identifier: Optional[str]
     labels: Optional[List[Optional[str]]]
 
 
-class GetContentContentObservations(BaseModel):
+class ContentContentObservations(BaseModel):
     type: ObservableTypes
-    observable: "GetContentContentObservationsObservable"
-    occurrences: Optional[List[Optional["GetContentContentObservationsOccurrences"]]]
+    observable: "ContentContentObservationsObservable"
+    occurrences: Optional[List[Optional["ContentContentObservationsOccurrences"]]]
 
 
-class GetContentContentObservationsObservable(BaseModel):
+class ContentContentObservationsObservable(BaseModel):
     id: str
     name: Optional[str]
 
 
-class GetContentContentObservationsOccurrences(BaseModel):
+class ContentContentObservationsOccurrences(BaseModel):
     type: Optional[OccurrenceTypes]
     confidence: Optional[float]
-    bounding_box: Optional["GetContentContentObservationsOccurrencesBoundingBox"] = (
-        Field(alias="boundingBox")
+    bounding_box: Optional["ContentContentObservationsOccurrencesBoundingBox"] = Field(
+        alias="boundingBox"
     )
     page_index: Optional[int] = Field(alias="pageIndex")
     start_time: Optional[Any] = Field(alias="startTime")
     end_time: Optional[Any] = Field(alias="endTime")
 
 
-class GetContentContentObservationsOccurrencesBoundingBox(BaseModel):
+class ContentContentObservationsOccurrencesBoundingBox(BaseModel):
     left: Optional[float]
     top: Optional[float]
     width: Optional[float]
     height: Optional[float]
 
 
-class GetContentContentParent(BaseModel):
+class ContentContentParent(BaseModel):
     id: str
 
 
-class GetContentContentChildren(BaseModel):
+class ContentContentChildren(BaseModel):
     id: str
 
 
-class GetContentContentCollections(BaseModel):
+class ContentContentCollections(BaseModel):
     id: str
 
 
-class GetContentContentFeed(BaseModel):
+class ContentContentFeed(BaseModel):
     id: str
 
 
-class GetContentContentWorkflow(BaseModel):
+class ContentContentWorkflow(BaseModel):
     id: str
 
 
-class GetContentContentLinks(BaseModel):
+class ContentContentLinks(BaseModel):
     uri: Optional[Any]
     link_type: Optional[LinkTypes] = Field(alias="linkType")
 
 
-GetContent.model_rebuild()
-GetContentContent.model_rebuild()
-GetContentContentEmail.model_rebuild()
-GetContentContentObservations.model_rebuild()
-GetContentContentObservationsOccurrences.model_rebuild()
+Content.model_rebuild()
+ContentContent.model_rebuild()
+ContentContentEmail.model_rebuild()
+ContentContentObservations.model_rebuild()
+ContentContentObservationsOccurrences.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/get_conversation.py` & `graphlit_client-1.0.20240420001/graphlit_api/conversation.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,118 +13,118 @@
     EntityState,
     FileTypes,
     ModelServiceTypes,
     ObservableTypes,
 )
 
 
-class GetConversation(BaseModel):
-    conversation: Optional["GetConversationConversation"]
+class Conversation(BaseModel):
+    conversation: Optional["ConversationConversation"]
 
 
-class GetConversationConversation(BaseModel):
+class ConversationConversation(BaseModel):
     id: str
     name: str
     creation_date: Any = Field(alias="creationDate")
-    owner: "GetConversationConversationOwner"
+    owner: "ConversationConversationOwner"
     state: EntityState
     correlation_id: Optional[str] = Field(alias="correlationId")
     type: Optional[ConversationTypes]
-    messages: Optional[List[Optional["GetConversationConversationMessages"]]]
-    specification: Optional["GetConversationConversationSpecification"]
-    filter: Optional["GetConversationConversationFilter"]
+    messages: Optional[List[Optional["ConversationConversationMessages"]]]
+    specification: Optional["ConversationConversationSpecification"]
+    filter: Optional["ConversationConversationFilter"]
 
 
-class GetConversationConversationOwner(BaseModel):
+class ConversationConversationOwner(BaseModel):
     id: str
 
 
-class GetConversationConversationMessages(BaseModel):
+class ConversationConversationMessages(BaseModel):
     role: ConversationRoleTypes
     author: Optional[str]
     message: str
-    citations: Optional[List[Optional["GetConversationConversationMessagesCitations"]]]
+    citations: Optional[List[Optional["ConversationConversationMessagesCitations"]]]
     tokens: int
     throughput: Optional[float]
     completion_time: Optional[Any] = Field(alias="completionTime")
     timestamp: Any
     model_service: Optional[ModelServiceTypes] = Field(alias="modelService")
     model: Optional[str]
 
 
-class GetConversationConversationMessagesCitations(BaseModel):
-    content: Optional["GetConversationConversationMessagesCitationsContent"]
+class ConversationConversationMessagesCitations(BaseModel):
+    content: Optional["ConversationConversationMessagesCitationsContent"]
     index: Optional[int]
     text: Optional[str]
     start_time: Optional[Any] = Field(alias="startTime")
     end_time: Optional[Any] = Field(alias="endTime")
     page_number: Optional[int] = Field(alias="pageNumber")
     frame_number: Optional[int] = Field(alias="frameNumber")
 
 
-class GetConversationConversationMessagesCitationsContent(BaseModel):
+class ConversationConversationMessagesCitationsContent(BaseModel):
     id: str
 
 
-class GetConversationConversationSpecification(BaseModel):
+class ConversationConversationSpecification(BaseModel):
     id: str
     name: str
 
 
-class GetConversationConversationFilter(BaseModel):
-    date_range: Optional["GetConversationConversationFilterDateRange"] = Field(
+class ConversationConversationFilter(BaseModel):
+    date_range: Optional["ConversationConversationFilterDateRange"] = Field(
         alias="dateRange"
     )
-    creation_date_range: Optional[
-        "GetConversationConversationFilterCreationDateRange"
-    ] = Field(alias="creationDateRange")
+    creation_date_range: Optional["ConversationConversationFilterCreationDateRange"] = (
+        Field(alias="creationDateRange")
+    )
     types: Optional[List[ContentTypes]]
     file_types: Optional[List[Optional[FileTypes]]] = Field(alias="fileTypes")
-    contents: Optional[List["GetConversationConversationFilterContents"]]
-    feeds: Optional[List["GetConversationConversationFilterFeeds"]]
-    workflows: Optional[List["GetConversationConversationFilterWorkflows"]]
-    collections: Optional[List["GetConversationConversationFilterCollections"]]
-    observations: Optional[List["GetConversationConversationFilterObservations"]]
+    contents: Optional[List["ConversationConversationFilterContents"]]
+    feeds: Optional[List["ConversationConversationFilterFeeds"]]
+    workflows: Optional[List["ConversationConversationFilterWorkflows"]]
+    collections: Optional[List["ConversationConversationFilterCollections"]]
+    observations: Optional[List["ConversationConversationFilterObservations"]]
 
 
-class GetConversationConversationFilterDateRange(BaseModel):
+class ConversationConversationFilterDateRange(BaseModel):
     from_: Optional[Any] = Field(alias="from")
     to: Optional[Any]
 
 
-class GetConversationConversationFilterCreationDateRange(BaseModel):
+class ConversationConversationFilterCreationDateRange(BaseModel):
     from_: Optional[Any] = Field(alias="from")
     to: Optional[Any]
 
 
-class GetConversationConversationFilterContents(BaseModel):
+class ConversationConversationFilterContents(BaseModel):
     id: str
 
 
-class GetConversationConversationFilterFeeds(BaseModel):
+class ConversationConversationFilterFeeds(BaseModel):
     id: str
 
 
-class GetConversationConversationFilterWorkflows(BaseModel):
+class ConversationConversationFilterWorkflows(BaseModel):
     id: str
 
 
-class GetConversationConversationFilterCollections(BaseModel):
+class ConversationConversationFilterCollections(BaseModel):
     id: str
 
 
-class GetConversationConversationFilterObservations(BaseModel):
+class ConversationConversationFilterObservations(BaseModel):
     type: ObservableTypes
-    observable: "GetConversationConversationFilterObservationsObservable"
+    observable: "ConversationConversationFilterObservationsObservable"
     states: Optional[List[Optional[EntityState]]]
 
 
-class GetConversationConversationFilterObservationsObservable(BaseModel):
+class ConversationConversationFilterObservationsObservable(BaseModel):
     id: str
 
 
-GetConversation.model_rebuild()
-GetConversationConversation.model_rebuild()
-GetConversationConversationMessages.model_rebuild()
-GetConversationConversationMessagesCitations.model_rebuild()
-GetConversationConversationFilter.model_rebuild()
-GetConversationConversationFilterObservations.model_rebuild()
+Conversation.model_rebuild()
+ConversationConversation.model_rebuild()
+ConversationConversationMessages.model_rebuild()
+ConversationConversationMessagesCitations.model_rebuild()
+ConversationConversationFilter.model_rebuild()
+ConversationConversationFilterObservations.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/get_feed.py` & `graphlit_client-1.0.20240420001/graphlit_api/feed.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,215 +16,213 @@
     SharePointAuthenticationTypes,
     SiteTypes,
     TimedPolicyRecurrenceTypes,
     YouTubeTypes,
 )
 
 
-class GetFeed(BaseModel):
-    feed: Optional["GetFeedFeed"]
+class Feed(BaseModel):
+    feed: Optional["FeedFeed"]
 
 
-class GetFeedFeed(BaseModel):
+class FeedFeed(BaseModel):
     id: str
     name: str
     creation_date: Any = Field(alias="creationDate")
-    owner: "GetFeedFeedOwner"
+    owner: "FeedFeedOwner"
     state: EntityState
     correlation_id: Optional[str] = Field(alias="correlationId")
     type: FeedTypes
-    site: Optional["GetFeedFeedSite"]
-    email: Optional["GetFeedFeedEmail"]
-    issue: Optional["GetFeedFeedIssue"]
-    rss: Optional["GetFeedFeedRss"]
-    web: Optional["GetFeedFeedWeb"]
-    reddit: Optional["GetFeedFeedReddit"]
-    notion: Optional["GetFeedFeedNotion"]
-    youtube: Optional["GetFeedFeedYoutube"]
-    slack: Optional["GetFeedFeedSlack"]
-    discord: Optional["GetFeedFeedDiscord"]
+    site: Optional["FeedFeedSite"]
+    email: Optional["FeedFeedEmail"]
+    issue: Optional["FeedFeedIssue"]
+    rss: Optional["FeedFeedRss"]
+    web: Optional["FeedFeedWeb"]
+    reddit: Optional["FeedFeedReddit"]
+    notion: Optional["FeedFeedNotion"]
+    youtube: Optional["FeedFeedYoutube"]
+    slack: Optional["FeedFeedSlack"]
+    discord: Optional["FeedFeedDiscord"]
     error: Optional[str]
     last_post_date: Optional[Any] = Field(alias="lastPostDate")
     last_read_date: Optional[Any] = Field(alias="lastReadDate")
     read_count: Optional[int] = Field(alias="readCount")
-    workflow: Optional["GetFeedFeedWorkflow"]
-    schedule_policy: Optional["GetFeedFeedSchedulePolicy"] = Field(
-        alias="schedulePolicy"
-    )
+    workflow: Optional["FeedFeedWorkflow"]
+    schedule_policy: Optional["FeedFeedSchedulePolicy"] = Field(alias="schedulePolicy")
 
 
-class GetFeedFeedOwner(BaseModel):
+class FeedFeedOwner(BaseModel):
     id: str
 
 
-class GetFeedFeedSite(BaseModel):
+class FeedFeedSite(BaseModel):
     site_type: SiteTypes = Field(alias="siteType")
     type: FeedServiceTypes
     is_recursive: Optional[bool] = Field(alias="isRecursive")
-    s_3: Optional["GetFeedFeedSiteS3"] = Field(alias="s3")
-    azure_blob: Optional["GetFeedFeedSiteAzureBlob"] = Field(alias="azureBlob")
-    azure_file: Optional["GetFeedFeedSiteAzureFile"] = Field(alias="azureFile")
-    google: Optional["GetFeedFeedSiteGoogle"]
-    share_point: Optional["GetFeedFeedSiteSharePoint"] = Field(alias="sharePoint")
-    one_drive: Optional["GetFeedFeedSiteOneDrive"] = Field(alias="oneDrive")
-    google_drive: Optional["GetFeedFeedSiteGoogleDrive"] = Field(alias="googleDrive")
+    s_3: Optional["FeedFeedSiteS3"] = Field(alias="s3")
+    azure_blob: Optional["FeedFeedSiteAzureBlob"] = Field(alias="azureBlob")
+    azure_file: Optional["FeedFeedSiteAzureFile"] = Field(alias="azureFile")
+    google: Optional["FeedFeedSiteGoogle"]
+    share_point: Optional["FeedFeedSiteSharePoint"] = Field(alias="sharePoint")
+    one_drive: Optional["FeedFeedSiteOneDrive"] = Field(alias="oneDrive")
+    google_drive: Optional["FeedFeedSiteGoogleDrive"] = Field(alias="googleDrive")
 
 
-class GetFeedFeedSiteS3(BaseModel):
+class FeedFeedSiteS3(BaseModel):
     access_key: Optional[str] = Field(alias="accessKey")
     secret_access_key: Optional[str] = Field(alias="secretAccessKey")
     bucket_name: Optional[str] = Field(alias="bucketName")
     prefix: Optional[str]
     region: Optional[str]
 
 
-class GetFeedFeedSiteAzureBlob(BaseModel):
+class FeedFeedSiteAzureBlob(BaseModel):
     storage_access_key: Optional[str] = Field(alias="storageAccessKey")
     account_name: Optional[str] = Field(alias="accountName")
     container_name: Optional[str] = Field(alias="containerName")
     prefix: Optional[str]
 
 
-class GetFeedFeedSiteAzureFile(BaseModel):
+class FeedFeedSiteAzureFile(BaseModel):
     storage_access_key: Optional[str] = Field(alias="storageAccessKey")
     account_name: Optional[str] = Field(alias="accountName")
     share_name: Optional[str] = Field(alias="shareName")
     prefix: Optional[str]
 
 
-class GetFeedFeedSiteGoogle(BaseModel):
+class FeedFeedSiteGoogle(BaseModel):
     credentials: Optional[str]
     container_name: Optional[str] = Field(alias="containerName")
     prefix: Optional[str]
 
 
-class GetFeedFeedSiteSharePoint(BaseModel):
+class FeedFeedSiteSharePoint(BaseModel):
     authentication_type: Optional[SharePointAuthenticationTypes] = Field(
         alias="authenticationType"
     )
     account_name: Optional[str] = Field(alias="accountName")
     library_id: Optional[str] = Field(alias="libraryId")
     tenant_id: Optional[str] = Field(alias="tenantId")
     refresh_token: Optional[str] = Field(alias="refreshToken")
 
 
-class GetFeedFeedSiteOneDrive(BaseModel):
+class FeedFeedSiteOneDrive(BaseModel):
     folder_id: Optional[str] = Field(alias="folderId")
     refresh_token: str = Field(alias="refreshToken")
 
 
-class GetFeedFeedSiteGoogleDrive(BaseModel):
+class FeedFeedSiteGoogleDrive(BaseModel):
     folder_id: Optional[str] = Field(alias="folderId")
     refresh_token: str = Field(alias="refreshToken")
 
 
-class GetFeedFeedEmail(BaseModel):
+class FeedFeedEmail(BaseModel):
     type: FeedServiceTypes
     include_attachments: Optional[bool] = Field(alias="includeAttachments")
-    google: Optional["GetFeedFeedEmailGoogle"]
-    microsoft: Optional["GetFeedFeedEmailMicrosoft"]
+    google: Optional["FeedFeedEmailGoogle"]
+    microsoft: Optional["FeedFeedEmailMicrosoft"]
 
 
-class GetFeedFeedEmailGoogle(BaseModel):
+class FeedFeedEmailGoogle(BaseModel):
     type: Optional[EmailListingTypes]
     refresh_token: Optional[str] = Field(alias="refreshToken")
 
 
-class GetFeedFeedEmailMicrosoft(BaseModel):
+class FeedFeedEmailMicrosoft(BaseModel):
     type: Optional[EmailListingTypes]
     tenant_id: Optional[str] = Field(alias="tenantId")
     refresh_token: Optional[str] = Field(alias="refreshToken")
 
 
-class GetFeedFeedIssue(BaseModel):
+class FeedFeedIssue(BaseModel):
     type: FeedServiceTypes
     include_attachments: Optional[bool] = Field(alias="includeAttachments")
-    jira: Optional["GetFeedFeedIssueJira"]
-    linear: Optional["GetFeedFeedIssueLinear"]
-    github: Optional["GetFeedFeedIssueGithub"]
+    jira: Optional["FeedFeedIssueJira"]
+    linear: Optional["FeedFeedIssueLinear"]
+    github: Optional["FeedFeedIssueGithub"]
 
 
-class GetFeedFeedIssueJira(BaseModel):
+class FeedFeedIssueJira(BaseModel):
     uri: Any
     project: str
     email: str
     token: str
 
 
-class GetFeedFeedIssueLinear(BaseModel):
+class FeedFeedIssueLinear(BaseModel):
     key: str
     project: str
 
 
-class GetFeedFeedIssueGithub(BaseModel):
+class FeedFeedIssueGithub(BaseModel):
     uri: Optional[Any]
     repository_owner: str = Field(alias="repositoryOwner")
     repository_name: str = Field(alias="repositoryName")
     refresh_token: Optional[str] = Field(alias="refreshToken")
     personal_access_token: Optional[str] = Field(alias="personalAccessToken")
 
 
-class GetFeedFeedRss(BaseModel):
+class FeedFeedRss(BaseModel):
     read_limit: Optional[int] = Field(alias="readLimit")
     uri: Any
 
 
-class GetFeedFeedWeb(BaseModel):
+class FeedFeedWeb(BaseModel):
     read_limit: Optional[int] = Field(alias="readLimit")
     uri: Any
     include_files: Optional[bool] = Field(alias="includeFiles")
 
 
-class GetFeedFeedReddit(BaseModel):
+class FeedFeedReddit(BaseModel):
     read_limit: Optional[int] = Field(alias="readLimit")
     subreddit_name: str = Field(alias="subredditName")
 
 
-class GetFeedFeedNotion(BaseModel):
+class FeedFeedNotion(BaseModel):
     read_limit: Optional[int] = Field(alias="readLimit")
     token: str
     identifiers: List[str]
     type: NotionTypes
 
 
-class GetFeedFeedYoutube(BaseModel):
+class FeedFeedYoutube(BaseModel):
     read_limit: Optional[int] = Field(alias="readLimit")
     type: YouTubeTypes
     video_name: Optional[str] = Field(alias="videoName")
     video_identifiers: Optional[List[str]] = Field(alias="videoIdentifiers")
     channel_identifier: Optional[str] = Field(alias="channelIdentifier")
     playlist_identifier: Optional[str] = Field(alias="playlistIdentifier")
 
 
-class GetFeedFeedSlack(BaseModel):
+class FeedFeedSlack(BaseModel):
     read_limit: Optional[int] = Field(alias="readLimit")
     type: Optional[FeedListingTypes]
     token: str
     channel: str
     include_attachments: Optional[bool] = Field(alias="includeAttachments")
 
 
-class GetFeedFeedDiscord(BaseModel):
+class FeedFeedDiscord(BaseModel):
     read_limit: Optional[int] = Field(alias="readLimit")
     type: Optional[FeedListingTypes]
     token: str
     channel: str
     include_attachments: Optional[bool] = Field(alias="includeAttachments")
 
 
-class GetFeedFeedWorkflow(BaseModel):
+class FeedFeedWorkflow(BaseModel):
     id: str
     name: str
 
 
-class GetFeedFeedSchedulePolicy(BaseModel):
+class FeedFeedSchedulePolicy(BaseModel):
     recurrence_type: Optional[TimedPolicyRecurrenceTypes] = Field(
         alias="recurrenceType"
     )
     repeat_interval: Optional[Any] = Field(alias="repeatInterval")
 
 
-GetFeed.model_rebuild()
-GetFeedFeed.model_rebuild()
-GetFeedFeedSite.model_rebuild()
-GetFeedFeedEmail.model_rebuild()
-GetFeedFeedIssue.model_rebuild()
+Feed.model_rebuild()
+FeedFeed.model_rebuild()
+FeedFeedSite.model_rebuild()
+FeedFeedEmail.model_rebuild()
+FeedFeedIssue.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/get_specification.py` & `graphlit_client-1.0.20240420001/graphlit_api/specification.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,116 +16,116 @@
     PromptStrategyTypes,
     ReplicateModels,
     RetrievalStrategyTypes,
     SpecificationTypes,
 )
 
 
-class GetSpecification(BaseModel):
-    specification: Optional["GetSpecificationSpecification"]
+class Specification(BaseModel):
+    specification: Optional["SpecificationSpecification"]
 
 
-class GetSpecificationSpecification(BaseModel):
+class SpecificationSpecification(BaseModel):
     id: str
     name: str
     creation_date: Any = Field(alias="creationDate")
-    owner: "GetSpecificationSpecificationOwner"
+    owner: "SpecificationSpecificationOwner"
     state: EntityState
     type: Optional[SpecificationTypes]
     service_type: Optional[ModelServiceTypes] = Field(alias="serviceType")
     system_prompt: Optional[str] = Field(alias="systemPrompt")
     custom_guidance: Optional[str] = Field(alias="customGuidance")
-    strategy: Optional["GetSpecificationSpecificationStrategy"]
-    prompt_strategy: Optional["GetSpecificationSpecificationPromptStrategy"] = Field(
+    strategy: Optional["SpecificationSpecificationStrategy"]
+    prompt_strategy: Optional["SpecificationSpecificationPromptStrategy"] = Field(
         alias="promptStrategy"
     )
-    retrieval_strategy: Optional["GetSpecificationSpecificationRetrievalStrategy"] = (
-        Field(alias="retrievalStrategy")
+    retrieval_strategy: Optional["SpecificationSpecificationRetrievalStrategy"] = Field(
+        alias="retrievalStrategy"
     )
-    reranking_strategy: Optional["GetSpecificationSpecificationRerankingStrategy"] = (
-        Field(alias="rerankingStrategy")
+    reranking_strategy: Optional["SpecificationSpecificationRerankingStrategy"] = Field(
+        alias="rerankingStrategy"
     )
-    open_ai: Optional["GetSpecificationSpecificationOpenAi"] = Field(alias="openAI")
-    azure_open_ai: Optional["GetSpecificationSpecificationAzureOpenAi"] = Field(
+    open_ai: Optional["SpecificationSpecificationOpenAi"] = Field(alias="openAI")
+    azure_open_ai: Optional["SpecificationSpecificationAzureOpenAi"] = Field(
         alias="azureOpenAI"
     )
-    anthropic: Optional["GetSpecificationSpecificationAnthropic"]
-    replicate: Optional["GetSpecificationSpecificationReplicate"]
-    tools: Optional[List["GetSpecificationSpecificationTools"]]
+    anthropic: Optional["SpecificationSpecificationAnthropic"]
+    replicate: Optional["SpecificationSpecificationReplicate"]
+    tools: Optional[List["SpecificationSpecificationTools"]]
 
 
-class GetSpecificationSpecificationOwner(BaseModel):
+class SpecificationSpecificationOwner(BaseModel):
     id: str
 
 
-class GetSpecificationSpecificationStrategy(BaseModel):
-    type: ConversationStrategyTypes
+class SpecificationSpecificationStrategy(BaseModel):
+    type: Optional[ConversationStrategyTypes]
     message_limit: Optional[int] = Field(alias="messageLimit")
     embed_citations: Optional[bool] = Field(alias="embedCitations")
     enable_facets: Optional[bool] = Field(alias="enableFacets")
     messages_weight: Optional[float] = Field(alias="messagesWeight")
     contents_weight: Optional[float] = Field(alias="contentsWeight")
 
 
-class GetSpecificationSpecificationPromptStrategy(BaseModel):
+class SpecificationSpecificationPromptStrategy(BaseModel):
     type: PromptStrategyTypes
 
 
-class GetSpecificationSpecificationRetrievalStrategy(BaseModel):
+class SpecificationSpecificationRetrievalStrategy(BaseModel):
     type: RetrievalStrategyTypes
     content_limit: Optional[int] = Field(alias="contentLimit")
 
 
-class GetSpecificationSpecificationRerankingStrategy(BaseModel):
+class SpecificationSpecificationRerankingStrategy(BaseModel):
     service_type: ModelServiceTypes = Field(alias="serviceType")
 
 
-class GetSpecificationSpecificationOpenAi(BaseModel):
+class SpecificationSpecificationOpenAi(BaseModel):
     token_limit: Optional[int] = Field(alias="tokenLimit")
     completion_token_limit: Optional[int] = Field(alias="completionTokenLimit")
     model: OpenAIModels
     key: Optional[str]
     model_name: Optional[str] = Field(alias="modelName")
     temperature: Optional[float]
     probability: Optional[float]
 
 
-class GetSpecificationSpecificationAzureOpenAi(BaseModel):
+class SpecificationSpecificationAzureOpenAi(BaseModel):
     token_limit: Optional[int] = Field(alias="tokenLimit")
     completion_token_limit: Optional[int] = Field(alias="completionTokenLimit")
     model: AzureOpenAIModels
     key: Optional[str]
     endpoint: Optional[Any]
     deployment_name: Optional[str] = Field(alias="deploymentName")
     temperature: Optional[float]
     probability: Optional[float]
 
 
-class GetSpecificationSpecificationAnthropic(BaseModel):
+class SpecificationSpecificationAnthropic(BaseModel):
     token_limit: Optional[int] = Field(alias="tokenLimit")
     completion_token_limit: Optional[int] = Field(alias="completionTokenLimit")
     model: AnthropicModels
     key: Optional[str]
     model_name: Optional[str] = Field(alias="modelName")
     temperature: Optional[float]
     probability: Optional[float]
 
 
-class GetSpecificationSpecificationReplicate(BaseModel):
+class SpecificationSpecificationReplicate(BaseModel):
     token_limit: Optional[int] = Field(alias="tokenLimit")
     completion_token_limit: Optional[int] = Field(alias="completionTokenLimit")
     model: ReplicateModels
     key: Optional[str]
     model_name: Optional[str] = Field(alias="modelName")
     temperature: Optional[float]
     probability: Optional[float]
 
 
-class GetSpecificationSpecificationTools(BaseModel):
+class SpecificationSpecificationTools(BaseModel):
     name: str
     description: Optional[str]
     schema_: str = Field(alias="schema")
     uri: Optional[Any]
 
 
-GetSpecification.model_rebuild()
-GetSpecificationSpecification.model_rebuild()
+Specification.model_rebuild()
+SpecificationSpecification.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/get_workflow.py` & `graphlit_client-1.0.20240420001/graphlit_api/workflow.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,204 +19,204 @@
     LinkTypes,
     ObservableTypes,
     OpenAIVisionDetailLevels,
     SummarizationTypes,
 )
 
 
-class GetWorkflow(BaseModel):
-    workflow: Optional["GetWorkflowWorkflow"]
+class Workflow(BaseModel):
+    workflow: Optional["WorkflowWorkflow"]
 
 
-class GetWorkflowWorkflow(BaseModel):
+class WorkflowWorkflow(BaseModel):
     id: str
     name: str
     creation_date: Any = Field(alias="creationDate")
-    owner: "GetWorkflowWorkflowOwner"
+    owner: "WorkflowWorkflowOwner"
     state: EntityState
-    ingestion: Optional["GetWorkflowWorkflowIngestion"]
-    preparation: Optional["GetWorkflowWorkflowPreparation"]
-    extraction: Optional["GetWorkflowWorkflowExtraction"]
-    enrichment: Optional["GetWorkflowWorkflowEnrichment"]
-    actions: Optional[List[Optional["GetWorkflowWorkflowActions"]]]
+    ingestion: Optional["WorkflowWorkflowIngestion"]
+    preparation: Optional["WorkflowWorkflowPreparation"]
+    extraction: Optional["WorkflowWorkflowExtraction"]
+    enrichment: Optional["WorkflowWorkflowEnrichment"]
+    actions: Optional[List[Optional["WorkflowWorkflowActions"]]]
 
 
-class GetWorkflowWorkflowOwner(BaseModel):
+class WorkflowWorkflowOwner(BaseModel):
     id: str
 
 
-class GetWorkflowWorkflowIngestion(BaseModel):
-    if_: Optional["GetWorkflowWorkflowIngestionIf"] = Field(alias="if")
-    collections: Optional[List[Optional["GetWorkflowWorkflowIngestionCollections"]]]
+class WorkflowWorkflowIngestion(BaseModel):
+    if_: Optional["WorkflowWorkflowIngestionIf"] = Field(alias="if")
+    collections: Optional[List[Optional["WorkflowWorkflowIngestionCollections"]]]
 
 
-class GetWorkflowWorkflowIngestionIf(BaseModel):
+class WorkflowWorkflowIngestionIf(BaseModel):
     types: Optional[List[Optional[ContentTypes]]]
     file_types: Optional[List[Optional[FileTypes]]] = Field(alias="fileTypes")
 
 
-class GetWorkflowWorkflowIngestionCollections(BaseModel):
+class WorkflowWorkflowIngestionCollections(BaseModel):
     id: str
 
 
-class GetWorkflowWorkflowPreparation(BaseModel):
+class WorkflowWorkflowPreparation(BaseModel):
     disable_smart_capture: Optional[bool] = Field(alias="disableSmartCapture")
     summarizations: Optional[
-        List[Optional["GetWorkflowWorkflowPreparationSummarizations"]]
+        List[Optional["WorkflowWorkflowPreparationSummarizations"]]
     ]
-    jobs: Optional[List[Optional["GetWorkflowWorkflowPreparationJobs"]]]
+    jobs: Optional[List[Optional["WorkflowWorkflowPreparationJobs"]]]
 
 
-class GetWorkflowWorkflowPreparationSummarizations(BaseModel):
+class WorkflowWorkflowPreparationSummarizations(BaseModel):
     type: SummarizationTypes
-    specification: Optional["GetWorkflowWorkflowPreparationSummarizationsSpecification"]
+    specification: Optional["WorkflowWorkflowPreparationSummarizationsSpecification"]
     tokens: Optional[int]
     items: Optional[int]
 
 
-class GetWorkflowWorkflowPreparationSummarizationsSpecification(BaseModel):
+class WorkflowWorkflowPreparationSummarizationsSpecification(BaseModel):
     id: str
 
 
-class GetWorkflowWorkflowPreparationJobs(BaseModel):
-    connector: Optional["GetWorkflowWorkflowPreparationJobsConnector"]
+class WorkflowWorkflowPreparationJobs(BaseModel):
+    connector: Optional["WorkflowWorkflowPreparationJobsConnector"]
 
 
-class GetWorkflowWorkflowPreparationJobsConnector(BaseModel):
+class WorkflowWorkflowPreparationJobsConnector(BaseModel):
     type: FilePreparationServiceTypes
     file_types: Optional[List[FileTypes]] = Field(alias="fileTypes")
     azure_document: Optional[
-        "GetWorkflowWorkflowPreparationJobsConnectorAzureDocument"
+        "WorkflowWorkflowPreparationJobsConnectorAzureDocument"
     ] = Field(alias="azureDocument")
-    deepgram: Optional["GetWorkflowWorkflowPreparationJobsConnectorDeepgram"]
-    document: Optional["GetWorkflowWorkflowPreparationJobsConnectorDocument"]
-    email: Optional["GetWorkflowWorkflowPreparationJobsConnectorEmail"]
+    deepgram: Optional["WorkflowWorkflowPreparationJobsConnectorDeepgram"]
+    document: Optional["WorkflowWorkflowPreparationJobsConnectorDocument"]
+    email: Optional["WorkflowWorkflowPreparationJobsConnectorEmail"]
 
 
-class GetWorkflowWorkflowPreparationJobsConnectorAzureDocument(BaseModel):
+class WorkflowWorkflowPreparationJobsConnectorAzureDocument(BaseModel):
     model: Optional[AzureDocumentIntelligenceModels]
 
 
-class GetWorkflowWorkflowPreparationJobsConnectorDeepgram(BaseModel):
+class WorkflowWorkflowPreparationJobsConnectorDeepgram(BaseModel):
     model: Optional[DeepgramModels]
     key: Optional[str]
     enable_redaction: Optional[bool] = Field(alias="enableRedaction")
     enable_speaker_diarization: Optional[bool] = Field(alias="enableSpeakerDiarization")
 
 
-class GetWorkflowWorkflowPreparationJobsConnectorDocument(BaseModel):
+class WorkflowWorkflowPreparationJobsConnectorDocument(BaseModel):
     include_images: Optional[bool] = Field(alias="includeImages")
 
 
-class GetWorkflowWorkflowPreparationJobsConnectorEmail(BaseModel):
+class WorkflowWorkflowPreparationJobsConnectorEmail(BaseModel):
     include_attachments: Optional[bool] = Field(alias="includeAttachments")
 
 
-class GetWorkflowWorkflowExtraction(BaseModel):
-    jobs: Optional[List[Optional["GetWorkflowWorkflowExtractionJobs"]]]
+class WorkflowWorkflowExtraction(BaseModel):
+    jobs: Optional[List[Optional["WorkflowWorkflowExtractionJobs"]]]
 
 
-class GetWorkflowWorkflowExtractionJobs(BaseModel):
-    connector: Optional["GetWorkflowWorkflowExtractionJobsConnector"]
+class WorkflowWorkflowExtractionJobs(BaseModel):
+    connector: Optional["WorkflowWorkflowExtractionJobsConnector"]
 
 
-class GetWorkflowWorkflowExtractionJobsConnector(BaseModel):
+class WorkflowWorkflowExtractionJobsConnector(BaseModel):
     type: EntityExtractionServiceTypes
     content_types: Optional[List[ContentTypes]] = Field(alias="contentTypes")
     file_types: Optional[List[FileTypes]] = Field(alias="fileTypes")
     extracted_types: Optional[List[ObservableTypes]] = Field(alias="extractedTypes")
-    azure_text: Optional["GetWorkflowWorkflowExtractionJobsConnectorAzureText"] = Field(
+    azure_text: Optional["WorkflowWorkflowExtractionJobsConnectorAzureText"] = Field(
         alias="azureText"
     )
-    azure_image: Optional["GetWorkflowWorkflowExtractionJobsConnectorAzureImage"] = (
-        Field(alias="azureImage")
+    azure_image: Optional["WorkflowWorkflowExtractionJobsConnectorAzureImage"] = Field(
+        alias="azureImage"
     )
-    open_ai_image: Optional["GetWorkflowWorkflowExtractionJobsConnectorOpenAiImage"] = (
+    open_ai_image: Optional["WorkflowWorkflowExtractionJobsConnectorOpenAiImage"] = (
         Field(alias="openAIImage")
     )
-    model_text: Optional["GetWorkflowWorkflowExtractionJobsConnectorModelText"] = Field(
+    model_text: Optional["WorkflowWorkflowExtractionJobsConnectorModelText"] = Field(
         alias="modelText"
     )
 
 
-class GetWorkflowWorkflowExtractionJobsConnectorAzureText(BaseModel):
+class WorkflowWorkflowExtractionJobsConnectorAzureText(BaseModel):
     confidence_threshold: Optional[float] = Field(alias="confidenceThreshold")
     enable_pii: Optional[bool] = Field(alias="enablePII")
 
 
-class GetWorkflowWorkflowExtractionJobsConnectorAzureImage(BaseModel):
+class WorkflowWorkflowExtractionJobsConnectorAzureImage(BaseModel):
     confidence_threshold: Optional[float] = Field(alias="confidenceThreshold")
 
 
-class GetWorkflowWorkflowExtractionJobsConnectorOpenAiImage(BaseModel):
+class WorkflowWorkflowExtractionJobsConnectorOpenAiImage(BaseModel):
     confidence_threshold: Optional[float] = Field(alias="confidenceThreshold")
     detail_level: Optional[OpenAIVisionDetailLevels] = Field(alias="detailLevel")
 
 
-class GetWorkflowWorkflowExtractionJobsConnectorModelText(BaseModel):
+class WorkflowWorkflowExtractionJobsConnectorModelText(BaseModel):
     specification: Optional[
-        "GetWorkflowWorkflowExtractionJobsConnectorModelTextSpecification"
+        "WorkflowWorkflowExtractionJobsConnectorModelTextSpecification"
     ]
 
 
-class GetWorkflowWorkflowExtractionJobsConnectorModelTextSpecification(BaseModel):
+class WorkflowWorkflowExtractionJobsConnectorModelTextSpecification(BaseModel):
     id: str
 
 
-class GetWorkflowWorkflowEnrichment(BaseModel):
-    link: Optional["GetWorkflowWorkflowEnrichmentLink"]
-    jobs: Optional[List[Optional["GetWorkflowWorkflowEnrichmentJobs"]]]
+class WorkflowWorkflowEnrichment(BaseModel):
+    link: Optional["WorkflowWorkflowEnrichmentLink"]
+    jobs: Optional[List[Optional["WorkflowWorkflowEnrichmentJobs"]]]
 
 
-class GetWorkflowWorkflowEnrichmentLink(BaseModel):
+class WorkflowWorkflowEnrichmentLink(BaseModel):
     enable_crawling: Optional[bool] = Field(alias="enableCrawling")
     allowed_domains: Optional[List[str]] = Field(alias="allowedDomains")
     excluded_domains: Optional[List[str]] = Field(alias="excludedDomains")
     allowed_links: Optional[List[LinkTypes]] = Field(alias="allowedLinks")
     excluded_links: Optional[List[LinkTypes]] = Field(alias="excludedLinks")
     allowed_files: Optional[List[FileTypes]] = Field(alias="allowedFiles")
     excluded_files: Optional[List[FileTypes]] = Field(alias="excludedFiles")
     allow_content_domain: Optional[bool] = Field(alias="allowContentDomain")
     maximum_links: Optional[int] = Field(alias="maximumLinks")
 
 
-class GetWorkflowWorkflowEnrichmentJobs(BaseModel):
-    connector: Optional["GetWorkflowWorkflowEnrichmentJobsConnector"]
+class WorkflowWorkflowEnrichmentJobs(BaseModel):
+    connector: Optional["WorkflowWorkflowEnrichmentJobsConnector"]
 
 
-class GetWorkflowWorkflowEnrichmentJobsConnector(BaseModel):
+class WorkflowWorkflowEnrichmentJobsConnector(BaseModel):
     type: Optional[EntityEnrichmentServiceTypes]
     enriched_types: Optional[List[Optional[ObservableTypes]]] = Field(
         alias="enrichedTypes"
     )
 
 
-class GetWorkflowWorkflowActions(BaseModel):
-    connector: Optional["GetWorkflowWorkflowActionsConnector"]
+class WorkflowWorkflowActions(BaseModel):
+    connector: Optional["WorkflowWorkflowActionsConnector"]
 
 
-class GetWorkflowWorkflowActionsConnector(BaseModel):
+class WorkflowWorkflowActionsConnector(BaseModel):
     type: IntegrationServiceTypes
     uri: Optional[str]
-    slack: Optional["GetWorkflowWorkflowActionsConnectorSlack"]
+    slack: Optional["WorkflowWorkflowActionsConnectorSlack"]
 
 
-class GetWorkflowWorkflowActionsConnectorSlack(BaseModel):
+class WorkflowWorkflowActionsConnectorSlack(BaseModel):
     token: str
     channel: str
 
 
-GetWorkflow.model_rebuild()
-GetWorkflowWorkflow.model_rebuild()
-GetWorkflowWorkflowIngestion.model_rebuild()
-GetWorkflowWorkflowPreparation.model_rebuild()
-GetWorkflowWorkflowPreparationSummarizations.model_rebuild()
-GetWorkflowWorkflowPreparationJobs.model_rebuild()
-GetWorkflowWorkflowPreparationJobsConnector.model_rebuild()
-GetWorkflowWorkflowExtraction.model_rebuild()
-GetWorkflowWorkflowExtractionJobs.model_rebuild()
-GetWorkflowWorkflowExtractionJobsConnector.model_rebuild()
-GetWorkflowWorkflowExtractionJobsConnectorModelText.model_rebuild()
-GetWorkflowWorkflowEnrichment.model_rebuild()
-GetWorkflowWorkflowEnrichmentJobs.model_rebuild()
-GetWorkflowWorkflowActions.model_rebuild()
-GetWorkflowWorkflowActionsConnector.model_rebuild()
+Workflow.model_rebuild()
+WorkflowWorkflow.model_rebuild()
+WorkflowWorkflowIngestion.model_rebuild()
+WorkflowWorkflowPreparation.model_rebuild()
+WorkflowWorkflowPreparationSummarizations.model_rebuild()
+WorkflowWorkflowPreparationJobs.model_rebuild()
+WorkflowWorkflowPreparationJobsConnector.model_rebuild()
+WorkflowWorkflowExtraction.model_rebuild()
+WorkflowWorkflowExtractionJobs.model_rebuild()
+WorkflowWorkflowExtractionJobsConnector.model_rebuild()
+WorkflowWorkflowExtractionJobsConnectorModelText.model_rebuild()
+WorkflowWorkflowEnrichment.model_rebuild()
+WorkflowWorkflowEnrichmentJobs.model_rebuild()
+WorkflowWorkflowActions.model_rebuild()
+WorkflowWorkflowActionsConnector.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/ingest_encoded_file.py` & `graphlit_client-1.0.20240420001/graphlit_api/ingest_encoded_file.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/ingest_text.py` & `graphlit_client-1.0.20240420001/graphlit_api/ingest_text.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/ingest_uri.py` & `graphlit_client-1.0.20240420001/graphlit_api/ingest_uri.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/input_types.py` & `graphlit_client-1.0.20240420001/graphlit_api/input_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -634,14 +634,15 @@
     service_type: ModelServiceTypes = Field(alias="serviceType")
     search_type: Optional[ConversationSearchTypes] = Field(
         alias="searchType", default=None
     )
     number_similar: Optional[int] = Field(alias="numberSimilar", default=None)
     system_prompt: Optional[str] = Field(alias="systemPrompt", default=None)
     custom_guidance: Optional[str] = Field(alias="customGuidance", default=None)
+    custom_instructions: Optional[str] = Field(alias="customInstructions", default=None)
     strategy: Optional["ConversationStrategyInput"] = None
     prompt_strategy: Optional["PromptStrategyInput"] = Field(
         alias="promptStrategy", default=None
     )
     retrieval_strategy: Optional["RetrievalStrategyInput"] = Field(
         alias="retrievalStrategy", default=None
     )
@@ -875,14 +876,15 @@
     service_type: ModelServiceTypes = Field(alias="serviceType")
     search_type: Optional[ConversationSearchTypes] = Field(
         alias="searchType", default=None
     )
     number_similar: Optional[int] = Field(alias="numberSimilar", default=None)
     system_prompt: Optional[str] = Field(alias="systemPrompt", default=None)
     custom_guidance: Optional[str] = Field(alias="customGuidance", default=None)
+    custom_instructions: Optional[str] = Field(alias="customInstructions", default=None)
     strategy: Optional["ConversationStrategyUpdateInput"] = None
     prompt_strategy: Optional["PromptStrategyUpdateInput"] = Field(
         alias="promptStrategy", default=None
     )
     retrieval_strategy: Optional["RetrievalStrategyUpdateInput"] = Field(
         alias="retrievalStrategy", default=None
     )
```

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/lookup_credits.py` & `graphlit_client-1.0.20240420001/graphlit_api/lookup_credits.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/lookup_usage.py` & `graphlit_client-1.0.20240420001/graphlit_api/lookup_usage.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/operations.py` & `graphlit_client-1.0.20240420001/graphlit_api/operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Generated by ariadne-codegen
 # Source: ./documents
 
 __all__ = [
     "ADD_CONTENTS_TO_COLLECTIONS_GQL",
+    "ALERT_GQL",
     "CLEAR_CONVERSATION_GQL",
     "CLOSE_CONVERSATION_GQL",
+    "COLLECTION_GQL",
+    "CONTENT_GQL",
+    "CONVERSATION_GQL",
     "CREATE_ALERT_GQL",
     "CREATE_COLLECTION_GQL",
     "CREATE_CONVERSATION_GQL",
     "CREATE_FEED_GQL",
     "CREATE_SPECIFICATION_GQL",
     "CREATE_WORKFLOW_GQL",
     "CREDITS_GQL",
@@ -31,21 +35,15 @@
     "DELETE_WORKFLOWS_GQL",
     "DELETE_WORKFLOW_GQL",
     "DISABLE_ALERT_GQL",
     "DISABLE_FEED_GQL",
     "ENABLE_ALERT_GQL",
     "ENABLE_FEED_GQL",
     "EXTRACT_CONTENTS_GQL",
-    "GET_ALERT_GQL",
-    "GET_COLLECTION_GQL",
-    "GET_CONTENT_GQL",
-    "GET_CONVERSATION_GQL",
-    "GET_FEED_GQL",
-    "GET_SPECIFICATION_GQL",
-    "GET_WORKFLOW_GQL",
+    "FEED_GQL",
     "INGEST_ENCODED_FILE_GQL",
     "INGEST_TEXT_GQL",
     "INGEST_URI_GQL",
     "IS_CONTENT_DONE_GQL",
     "IS_FEED_DONE_GQL",
     "LOOKUP_CREDITS_GQL",
     "LOOKUP_USAGE_GQL",
@@ -59,25 +57,27 @@
     "QUERY_CONTENTS_GQL",
     "QUERY_CONTENT_FACETS_GQL",
     "QUERY_CONVERSATIONS_GQL",
     "QUERY_FEEDS_GQL",
     "QUERY_SPECIFICATIONS_GQL",
     "QUERY_WORKFLOWS_GQL",
     "REMOVE_CONTENTS_FROM_COLLECTION_GQL",
+    "SPECIFICATION_GQL",
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
+    "WORKFLOW_GQL",
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
 
-GET_ALERT_GQL = """
-query GetAlert($id: ID!) {
+ALERT_GQL = """
+query Alert($id: ID!) {
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
 
-GET_COLLECTION_GQL = """
-query GetCollection($id: ID!) {
+COLLECTION_GQL = """
+query Collection($id: ID!) {
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
 
-GET_CONTENT_GQL = """
-query GetContent($id: ID!) {
+CONTENT_GQL = """
+query Content($id: ID!) {
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
 
-GET_CONVERSATION_GQL = """
-query GetConversation($id: ID!) {
+CONVERSATION_GQL = """
+query Conversation($id: ID!) {
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
 
-GET_FEED_GQL = """
-query GetFeed($id: ID!) {
+FEED_GQL = """
+query Feed($id: ID!) {
   feed(id: $id) {
     id
     name
     creationDate
     owner {
       id
     }
@@ -1772,16 +1772,16 @@
   deleteSpecification(id: $id) {
     id
     state
   }
 }
 """
 
-GET_SPECIFICATION_GQL = """
-query GetSpecification($id: ID!) {
+SPECIFICATION_GQL = """
+query Specification($id: ID!) {
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
 
-GET_WORKFLOW_GQL = """
-query GetWorkflow($id: ID!) {
+WORKFLOW_GQL = """
+query Workflow($id: ID!) {
   workflow(id: $id) {
     id
     name
     creationDate
     owner {
       id
     }
```

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/project.py` & `graphlit_client-1.0.20240420001/graphlit_api/project.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/prompt_conversation.py` & `graphlit_client-1.0.20240420001/graphlit_api/prompt_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/prompt_specifications.py` & `graphlit_client-1.0.20240420001/graphlit_api/prompt_specifications.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/publish_contents.py` & `graphlit_client-1.0.20240420001/graphlit_api/publish_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/publish_conversation.py` & `graphlit_client-1.0.20240420001/graphlit_api/publish_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/query_alerts.py` & `graphlit_client-1.0.20240420001/graphlit_api/query_alerts.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/query_collections.py` & `graphlit_client-1.0.20240420001/graphlit_api/query_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/query_content_facets.py` & `graphlit_client-1.0.20240420001/graphlit_api/query_content_facets.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/query_contents.py` & `graphlit_client-1.0.20240420001/graphlit_api/query_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/query_conversations.py` & `graphlit_client-1.0.20240420001/graphlit_api/query_conversations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/query_feeds.py` & `graphlit_client-1.0.20240420001/graphlit_api/query_feeds.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/query_specifications.py` & `graphlit_client-1.0.20240420001/graphlit_api/query_specifications.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 
 class QuerySpecificationsSpecificationsResultsOwner(BaseModel):
     id: str
 
 
 class QuerySpecificationsSpecificationsResultsStrategy(BaseModel):
-    type: ConversationStrategyTypes
+    type: Optional[ConversationStrategyTypes]
     message_limit: Optional[int] = Field(alias="messageLimit")
     embed_citations: Optional[bool] = Field(alias="embedCitations")
     enable_facets: Optional[bool] = Field(alias="enableFacets")
     messages_weight: Optional[float] = Field(alias="messagesWeight")
     contents_weight: Optional[float] = Field(alias="contentsWeight")
```

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/query_workflows.py` & `graphlit_client-1.0.20240420001/graphlit_api/query_workflows.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/remove_contents_from_collection.py` & `graphlit_client-1.0.20240420001/graphlit_api/remove_contents_from_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/summarize_contents.py` & `graphlit_client-1.0.20240420001/graphlit_api/summarize_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/update_collection.py` & `graphlit_client-1.0.20240420001/graphlit_api/update_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/update_content.py` & `graphlit_client-1.0.20240420001/graphlit_api/update_content.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/update_conversation.py` & `graphlit_client-1.0.20240420001/graphlit_api/update_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/update_specification.py` & `graphlit_client-1.0.20240420001/graphlit_api/update_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/update_workflow.py` & `graphlit_client-1.0.20240420001/graphlit_api/update_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_api/usage.py` & `graphlit_client-1.0.20240420001/graphlit_api/usage.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240417002/graphlit_client.egg-info/SOURCES.txt` & `graphlit_client-1.0.20240420001/graphlit_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 README.md
 pyproject.toml
 setup.py
 graphlit/__init__.py
 graphlit/graphlit.py
 graphlit_api/__init__.py
 graphlit_api/add_contents_to_collections.py
+graphlit_api/alert.py
 graphlit_api/async_base_client.py
 graphlit_api/base_model.py
 graphlit_api/clear_conversation.py
 graphlit_api/client.py
 graphlit_api/close_conversation.py
+graphlit_api/collection.py
+graphlit_api/content.py
+graphlit_api/conversation.py
 graphlit_api/create_alert.py
 graphlit_api/create_collection.py
 graphlit_api/create_conversation.py
 graphlit_api/create_feed.py
 graphlit_api/create_specification.py
 graphlit_api/create_workflow.py
 graphlit_api/credits.py
@@ -39,21 +43,15 @@
 graphlit_api/disable_alert.py
 graphlit_api/disable_feed.py
 graphlit_api/enable_alert.py
 graphlit_api/enable_feed.py
 graphlit_api/enums.py
 graphlit_api/exceptions.py
 graphlit_api/extract_contents.py
-graphlit_api/get_alert.py
-graphlit_api/get_collection.py
-graphlit_api/get_content.py
-graphlit_api/get_conversation.py
-graphlit_api/get_feed.py
-graphlit_api/get_specification.py
-graphlit_api/get_workflow.py
+graphlit_api/feed.py
 graphlit_api/ingest_encoded_file.py
 graphlit_api/ingest_text.py
 graphlit_api/ingest_uri.py
 graphlit_api/input_types.py
 graphlit_api/is_content_done.py
 graphlit_api/is_feed_done.py
 graphlit_api/lookup_credits.py
@@ -69,23 +67,25 @@
 graphlit_api/query_content_facets.py
 graphlit_api/query_contents.py
 graphlit_api/query_conversations.py
 graphlit_api/query_feeds.py
 graphlit_api/query_specifications.py
 graphlit_api/query_workflows.py
 graphlit_api/remove_contents_from_collection.py
+graphlit_api/specification.py
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
+graphlit_api/workflow.py
 graphlit_client.egg-info/PKG-INFO
 graphlit_client.egg-info/SOURCES.txt
 graphlit_client.egg-info/dependency_links.txt
 graphlit_client.egg-info/requires.txt
 graphlit_client.egg-info/top_level.txt
```

### Comparing `graphlit_client-1.0.20240417002/setup.py` & `graphlit_client-1.0.20240420001/setup.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from setuptools import setup, find_packages
-import os
-
-# Read the content of your README file
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-version = os.getenv('PACKAGE_VERSION', '1.0.0')
-
-setup(
-    name='graphlit-client',
-    version=version,
-    packages=find_packages(),
-    install_requires=[
-        'httpx',
-        'pydantic>=2.0.0,<3.0.0',
-        'PyJWT',
-        'websockets'
-    ],
-    python_requires='>=3.6',
-    author='Unstruk Data Inc.',
-    author_email='questions@graphlit.com',
-    description='Graphlit API Python Client',
-    url='https://github.com/graphlit/graphlit-client-python',
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-)
+from setuptools import setup, find_packages
+import os
+
+# Read the content of your README file
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+version = os.getenv('PACKAGE_VERSION', '1.0.0')
+
+setup(
+    name='graphlit-client',
+    version=version,
+    packages=find_packages(),
+    install_requires=[
+        'httpx',
+        'pydantic>=2.0.0,<3.0.0',
+        'PyJWT',
+        'websockets'
+    ],
+    python_requires='>=3.6',
+    author='Unstruk Data Inc.',
+    author_email='questions@graphlit.com',
+    description='Graphlit API Python Client',
+    url='https://github.com/graphlit/graphlit-client-python',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+)
```

