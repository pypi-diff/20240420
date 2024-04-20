# Comparing `tmp/dbt-materialize-1.7.6.tar.gz` & `tmp/dbt-materialize-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-materialize-1.7.6.tar", last modified: Thu Apr 18 14:01:05 2024, max compression
+gzip compressed data, was "dbt-materialize-1.7.7.tar", last modified: Sat Apr 20 00:25:53 2024, max compression
```

## Comparing `dbt-materialize-1.7.6.tar` & `dbt-materialize-1.7.7.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/
--rw-r--r--   0 materialize  (2000) materialize   (993)      424 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/MANIFEST.in
--rw-r--r--   0 materialize  (2000) materialize   (993)     6613 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/PKG-INFO
--rw-r--r--   0 materialize  (2000) materialize   (993)     6292 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/README.md
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.357478 dbt-materialize-1.7.6/dbt/
--rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/__init__.py
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.357478 dbt-materialize-1.7.6/dbt/adapters/
--rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/adapters/__init__.py
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.357478 dbt-materialize-1.7.6/dbt/adapters/materialize/
--rw-r--r--   0 materialize  (2000) materialize   (993)     1125 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/adapters/materialize/__init__.py
--rw-r--r--   0 materialize  (2000) materialize   (993)      801 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/adapters/materialize/__version__.py
--rw-r--r--   0 materialize  (2000) materialize   (993)     5553 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/adapters/materialize/connections.py
--rw-r--r--   0 materialize  (2000) materialize   (993)     1598 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/adapters/materialize/exceptions.py
--rw-r--r--   0 materialize  (2000) materialize   (993)    11918 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/adapters/materialize/impl.py
--rw-r--r--   0 materialize  (2000) materialize   (993)     2284 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/adapters/materialize/relation.py
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.357478 dbt-materialize-1.7.6/dbt/include/
--rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/__init__.py
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/dbt/include/materialize/
--rw-r--r--   0 materialize  (2000) materialize   (993)      782 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/__init__.py
--rw-r--r--   0 materialize  (2000) materialize   (993)      808 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/dbt_project.yml
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/dbt/include/materialize/macros/
--rw-r--r--   0 materialize  (2000) materialize   (993)     9472 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/adapters.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     2592 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/catalog.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      979 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/columns.sql
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/
--rw-r--r--   0 materialize  (2000) materialize   (993)     1711 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/deploy_await.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1981 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/deploy_cleanup.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)    12165 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/deploy_init.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     6074 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/deploy_permission_validation.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     5361 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/deploy_promote.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      989 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/freshness.sql
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/
--rw-r--r--   0 materialize  (2000) materialize   (993)     1911 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/incremental.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1922 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/materialized_view.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1224 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/materializedview.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1970 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/sink.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1835 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/source.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1974 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/table.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     2828 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/test.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1883 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/view.sql
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/dbt/include/materialize/macros/tests/
--rw-r--r--   0 materialize  (2000) materialize   (993)     1033 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/tests/helpers.sql
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/
--rw-r--r--   0 materialize  (2000) materialize   (993)     1151 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/await_cluster_ready.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     3245 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/ci_utils.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1986 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/exists.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      887 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/generate_cluster_name.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1285 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/generate_schema_name.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     5211 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/is_cluster_ready.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1016 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/listagg.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1257 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/profile_template.yml
--rw-r--r--   0 materialize  (2000) materialize   (993)     1277 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/materialize/sample_profiles.yml
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/dbt/include/starter_project/
--rw-r--r--   0 materialize  (2000) materialize   (993)      917 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/starter_project/dbt_project.yml
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.357478 dbt-materialize-1.7.6/dbt/include/starter_project/models/
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/dbt/include/starter_project/models/example/
--rw-r--r--   0 materialize  (2000) materialize   (993)      972 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/starter_project/models/example/fraud_activity.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      999 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/starter_project/models/example/funds_movement.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      936 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/starter_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      753 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/starter_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     2822 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/starter_project/models/example/schema.yml
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/dbt/include/starter_project/models/example/sources/
--rw-r--r--   0 materialize  (2000) materialize   (993)      900 2024-04-18 13:58:48.000000 dbt-materialize-1.7.6/dbt/include/starter_project/models/example/sources/auction.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      866 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/starter_project/models/example/sources/sources.yml
--rw-r--r--   0 materialize  (2000) materialize   (993)     1068 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/dbt/include/starter_project/models/example/winning_bids.sql
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/dbt_materialize.egg-info/
--rw-r--r--   0 materialize  (2000) materialize   (993)     6613 2024-04-18 14:01:05.000000 dbt-materialize-1.7.6/dbt_materialize.egg-info/PKG-INFO
--rw-r--r--   0 materialize  (2000) materialize   (993)     2636 2024-04-18 14:01:05.000000 dbt-materialize-1.7.6/dbt_materialize.egg-info/SOURCES.txt
--rw-r--r--   0 materialize  (2000) materialize   (993)        1 2024-04-18 14:01:05.000000 dbt-materialize-1.7.6/dbt_materialize.egg-info/dependency_links.txt
--rw-r--r--   0 materialize  (2000) materialize   (993)       52 2024-04-18 14:01:05.000000 dbt-materialize-1.7.6/dbt_materialize.egg-info/requires.txt
--rw-r--r--   0 materialize  (2000) materialize   (993)        4 2024-04-18 14:01:05.000000 dbt-materialize-1.7.6/dbt_materialize.egg-info/top_level.txt
--rw-r--r--   0 materialize  (2000) materialize   (993)      464 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/pyproject.toml
--rw-r--r--   0 materialize  (2000) materialize   (993)       38 2024-04-18 14:01:05.367478 dbt-materialize-1.7.6/setup.cfg
--rw-r--r--   0 materialize  (2000) materialize   (993)     1814 2024-04-18 13:58:47.000000 dbt-materialize-1.7.6/setup.py
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.288179 dbt-materialize-1.7.7/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      424 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/MANIFEST.in
+-rw-r--r--   0 materialize  (2000) materialize   (993)     6613 2024-04-20 00:25:53.288179 dbt-materialize-1.7.7/PKG-INFO
+-rw-r--r--   0 materialize  (2000) materialize   (993)     6292 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/README.md
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/__init__.py
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/adapters/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/adapters/__init__.py
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/adapters/materialize/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1125 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/adapters/materialize/__init__.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)      801 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/adapters/materialize/__version__.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)     5553 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/adapters/materialize/connections.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1598 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/adapters/materialize/exceptions.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)    11918 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/adapters/materialize/impl.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2284 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/adapters/materialize/relation.py
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/include/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/__init__.py
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/include/materialize/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      782 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/__init__.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)      808 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/dbt_project.yml
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/include/materialize/macros/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     9472 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/adapters.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2592 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/catalog.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      979 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/columns.sql
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1711 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/deploy_await.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1981 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/deploy_cleanup.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)    12165 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/deploy_init.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     6053 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/deploy_permission_validation.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     5361 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/deploy_promote.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      989 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/freshness.sql
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1911 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/incremental.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1922 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/materialized_view.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1224 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/materializedview.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1970 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/sink.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1835 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/source.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1974 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/table.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2828 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/test.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1883 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/view.sql
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/include/materialize/macros/tests/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1033 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/tests/helpers.sql
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1151 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/await_cluster_ready.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     3245 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/ci_utils.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1986 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/exists.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      887 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/generate_cluster_name.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1285 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/generate_schema_name.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     5211 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/is_cluster_ready.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1016 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/listagg.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1257 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/profile_template.yml
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1277 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/sample_profiles.yml
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/include/starter_project/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      917 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/starter_project/dbt_project.yml
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/include/starter_project/models/
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.288179 dbt-materialize-1.7.7/dbt/include/starter_project/models/example/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      972 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/starter_project/models/example/fraud_activity.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      999 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/starter_project/models/example/funds_movement.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      936 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/starter_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      753 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/starter_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2822 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/starter_project/models/example/schema.yml
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.288179 dbt-materialize-1.7.7/dbt/include/starter_project/models/example/sources/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      774 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/starter_project/models/example/sources/auction.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      866 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/starter_project/models/example/sources/sources.yml
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1068 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/starter_project/models/example/winning_bids.sql
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.288179 dbt-materialize-1.7.7/dbt_materialize.egg-info/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     6613 2024-04-20 00:25:53.000000 dbt-materialize-1.7.7/dbt_materialize.egg-info/PKG-INFO
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2636 2024-04-20 00:25:53.000000 dbt-materialize-1.7.7/dbt_materialize.egg-info/SOURCES.txt
+-rw-r--r--   0 materialize  (2000) materialize   (993)        1 2024-04-20 00:25:53.000000 dbt-materialize-1.7.7/dbt_materialize.egg-info/dependency_links.txt
+-rw-r--r--   0 materialize  (2000) materialize   (993)       52 2024-04-20 00:25:53.000000 dbt-materialize-1.7.7/dbt_materialize.egg-info/requires.txt
+-rw-r--r--   0 materialize  (2000) materialize   (993)        4 2024-04-20 00:25:53.000000 dbt-materialize-1.7.7/dbt_materialize.egg-info/top_level.txt
+-rw-r--r--   0 materialize  (2000) materialize   (993)      464 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/pyproject.toml
+-rw-r--r--   0 materialize  (2000) materialize   (993)       38 2024-04-20 00:25:53.288179 dbt-materialize-1.7.7/setup.cfg
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1814 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/setup.py
```

### Comparing `dbt-materialize-1.7.6/PKG-INFO` & `dbt-materialize-1.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-materialize
-Version: 1.7.6
+Version: 1.7.7
 Summary: The Materialize adapter plugin for dbt.
 Home-page: https://github.com/MaterializeInc/materialize/blob/main/misc/dbt-materialize
 Author: Materialize, Inc.
 Author-email: support@materialize.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `dbt-materialize-1.7.6/README.md` & `dbt-materialize-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/__init__.py` & `dbt-materialize-1.7.7/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/adapters/__init__.py` & `dbt-materialize-1.7.7/dbt/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/adapters/materialize/__init__.py` & `dbt-materialize-1.7.7/dbt/adapters/materialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/adapters/materialize/__version__.py` & `dbt-materialize-1.7.7/dbt/adapters/materialize/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # If you bump this version, bump it in setup.py too.
-version = "1.7.6"
+version = "1.7.7"
```

### Comparing `dbt-materialize-1.7.6/dbt/adapters/materialize/connections.py` & `dbt-materialize-1.7.7/dbt/adapters/materialize/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/adapters/materialize/exceptions.py` & `dbt-materialize-1.7.7/dbt/adapters/materialize/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/adapters/materialize/impl.py` & `dbt-materialize-1.7.7/dbt/adapters/materialize/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/adapters/materialize/relation.py` & `dbt-materialize-1.7.7/dbt/adapters/materialize/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/__init__.py` & `dbt-materialize-1.7.7/dbt/include/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/__init__.py` & `dbt-materialize-1.7.7/dbt/include/materialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/dbt_project.yml` & `dbt-materialize-1.7.7/dbt/include/materialize/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/adapters.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/catalog.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/columns.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/deploy_await.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/deploy_await.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/deploy_cleanup.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/deploy_cleanup.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/deploy_init.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/deploy_init.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/deploy_permission_validation.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/deploy_permission_validation.sql`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 -- The deployment user must be a superuser OR
 --
 -- Have CREATE and USAGE rights on the database
 -- Have CREATECLUSTER rights
 -- Have OWNERSHIP rights on the production clusters and schemas
 {% macro deploy_validate_permissions(clusters=[], schemas=[]) %}
 
-{% set is_not_super_user %}
-    SELECT mz_is_superuser() IS FALSE;
+{% set is_super_user %}
+    SELECT mz_is_superuser();
 {% endset %}
 
-{% set not_super_user = run_query(is_not_super_user) %}
+{% set super_user = run_query(is_super_user) %}
 {% if execute %}
-    {% if not_super_user.rows[0][0] %}
+    {% if not super_user.rows[0][0] %}
         {{ internal_ensure_database_permission() }}
         {{ internal_ensure_createcluster_permission() }}
         {{ internal_ensure_schema_ownership(schemas) }}
         {{ internal_ensure_cluster_ownership(clusters) }}
     {% endif %}
 {% endif %}
```

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/deploy/deploy_promote.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/deploy_promote.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/freshness.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/incremental.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/materialized_view.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/materializedview.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/materializedview.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/sink.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/sink.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/source.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/source.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/table.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/test.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/materializations/view.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/tests/helpers.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/await_cluster_ready.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/await_cluster_ready.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/ci_utils.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/ci_utils.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/exists.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/exists.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/generate_cluster_name.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/generate_cluster_name.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/generate_schema_name.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/generate_schema_name.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/is_cluster_ready.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/is_cluster_ready.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/macros/utils/listagg.sql` & `dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/profile_template.yml` & `dbt-materialize-1.7.7/dbt/include/materialize/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/materialize/sample_profiles.yml` & `dbt-materialize-1.7.7/dbt/include/materialize/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/starter_project/dbt_project.yml` & `dbt-materialize-1.7.7/dbt/include/starter_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/starter_project/models/example/fraud_activity.sql` & `dbt-materialize-1.7.7/dbt/include/starter_project/models/example/fraud_activity.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/starter_project/models/example/funds_movement.sql` & `dbt-materialize-1.7.7/dbt/include/starter_project/models/example/funds_movement.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/starter_project/models/example/my_first_dbt_model.sql` & `dbt-materialize-1.7.7/dbt/include/starter_project/models/example/my_first_dbt_model.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/starter_project/models/example/my_second_dbt_model.sql` & `dbt-materialize-1.7.7/dbt/include/starter_project/models/example/my_second_dbt_model.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/starter_project/models/example/schema.yml` & `dbt-materialize-1.7.7/dbt/include/starter_project/models/example/schema.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/starter_project/models/example/sources/sources.yml` & `dbt-materialize-1.7.7/dbt/include/starter_project/models/example/sources/sources.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt/include/starter_project/models/example/winning_bids.sql` & `dbt-materialize-1.7.7/dbt/include/starter_project/models/example/winning_bids.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/dbt_materialize.egg-info/PKG-INFO` & `dbt-materialize-1.7.7/dbt_materialize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-materialize
-Version: 1.7.6
+Version: 1.7.7
 Summary: The Materialize adapter plugin for dbt.
 Home-page: https://github.com/MaterializeInc/materialize/blob/main/misc/dbt-materialize
 Author: Materialize, Inc.
 Author-email: support@materialize.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `dbt-materialize-1.7.6/dbt_materialize.egg-info/SOURCES.txt` & `dbt-materialize-1.7.7/dbt_materialize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.6/setup.py` & `dbt-materialize-1.7.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 README = Path(__file__).parent / "README.md"
 
 setup(
     name="dbt-materialize",
     # This adapter's minor version should match the required dbt-postgres version,
     # but patch versions may differ.
     # If you bump this version, bump it in __version__.py too.
-    version="1.7.6",
+    version="1.7.7",
     description="The Materialize adapter plugin for dbt.",
     long_description=(Path(__file__).parent / "README.md").open().read(),
     long_description_content_type="text/markdown",
     author="Materialize, Inc.",
     author_email="support@materialize.com",
     url="https://github.com/MaterializeInc/materialize/blob/main/misc/dbt-materialize",
     packages=find_packages(),
```

