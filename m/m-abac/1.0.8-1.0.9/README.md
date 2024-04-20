# Comparing `tmp/m-abac-1.0.8.tar.gz` & `tmp/m-abac-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-abac-1.0.8.tar", last modified: Fri Oct 13 17:09:31 2023, max compression
+gzip compressed data, was "m-abac-1.0.9.tar", last modified: Mon Oct 16 03:46:50 2023, max compression
```

## Comparing `m-abac-1.0.8.tar` & `m-abac-1.0.9.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 17:09:31.958293 m-abac-1.0.8/
--rw-r--r--   0 root         (0) root         (0)     2114 2023-10-13 17:09:31.957293 m-abac-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      927 2023-10-13 17:05:47.000000 m-abac-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 17:09:31.888291 m-abac-1.0.8/m_abac.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2114 2023-10-13 17:09:31.000000 m-abac-1.0.8/m_abac.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4522 2023-10-13 17:09:31.000000 m-abac-1.0.8/m_abac.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-13 17:09:31.000000 m-abac-1.0.8/m_abac.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      131 2023-10-13 17:09:31.000000 m-abac-1.0.8/m_abac.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-10-13 17:09:31.000000 m-abac-1.0.8/m_abac.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 17:09:31.876290 m-abac-1.0.8/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 17:09:31.876290 m-abac-1.0.8/mobio/libs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 17:09:31.892291 m-abac-1.0.8/mobio/libs/abac/
--rw-r--r--   0 root         (0) root         (0)       70 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 17:09:31.894291 m-abac-1.0.8/mobio/libs/abac/adapter/
--rw-r--r--   0 root         (0) root         (0)      267 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/adapter/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/adapter/adapter.py
--rw-r--r--   0 root         (0) root         (0)    26744 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/adapter/elasticsearch_adapter.py
--rw-r--r--   0 root         (0) root         (0)     7708 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/call_api.py
--rw-r--r--   0 root         (0) root         (0)     4225 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/config.py
--rw-r--r--   0 root         (0) root         (0)    22178 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/pdp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 17:09:31.898291 m-abac-1.0.8/mobio/libs/abac/policy/
--rw-r--r--   0 root         (0) root         (0)       44 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 17:09:31.901291 m-abac-1.0.8/mobio/libs/abac/policy/conditions/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1506 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 17:09:31.903291 m-abac-1.0.8/mobio/libs/abac/policy/conditions/boolean/
--rw-r--r--   0 root         (0) root         (0)       39 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/boolean/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/boolean/base.py
--rw-r--r--   0 root         (0) root         (0)     1110 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/boolean/check_bool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 17:09:31.912291 m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/
--rw-r--r--   0 root         (0) root         (0)      418 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/__init__.py
--rw-r--r--   0 root         (0) root         (0)      680 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/all_in.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/all_not_in.py
--rw-r--r--   0 root         (0) root         (0)      893 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/any_contains.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/any_in.py
--rw-r--r--   0 root         (0) root         (0)      905 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/any_not_contains.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/any_not_in.py
--rw-r--r--   0 root         (0) root         (0)     1773 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/base.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/is_empty.py
--rw-r--r--   0 root         (0) root         (0)      602 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/is_in.py
--rw-r--r--   0 root         (0) root         (0)      921 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
--rw-r--r--   0 root         (0) root         (0)      728 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/is_not_in.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 17:09:31.918292 m-abac-1.0.8/mobio/libs/abac/policy/conditions/date_time/
--rw-r--r--   0 root         (0) root         (0)      243 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/date_time/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2967 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/date_time/base.py
--rw-r--r--   0 root         (0) root         (0)     1714 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_eq.py
--rw-r--r--   0 root         (0) root         (0)     1283 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_gt.py
--rw-r--r--   0 root         (0) root         (0)     1305 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_gte.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_lt.py
--rw-r--r--   0 root         (0) root         (0)     1296 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_lte.py
--rw-r--r--   0 root         (0) root         (0)     1732 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 17:09:31.925292 m-abac-1.0.8/mobio/libs/abac/policy/conditions/day/
--rw-r--r--   0 root         (0) root         (0)      197 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/day/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3129 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/day/base.py
--rw-r--r--   0 root         (0) root         (0)      966 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/day/day_eq.py
--rw-r--r--   0 root         (0) root         (0)     1095 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/day/day_gt.py
--rw-r--r--   0 root         (0) root         (0)     1097 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/day/day_gte.py
--rw-r--r--   0 root         (0) root         (0)     1094 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/day/day_lt.py
--rw-r--r--   0 root         (0) root         (0)     1097 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/day/day_lte.py
--rw-r--r--   0 root         (0) root         (0)      940 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/day/day_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 17:09:31.927292 m-abac-1.0.8/mobio/libs/abac/policy/conditions/ip_address/
--rw-r--r--   0 root         (0) root         (0)       82 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/ip_address/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/ip_address/base.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 17:09:31.935292 m-abac-1.0.8/mobio/libs/abac/policy/conditions/monthday/
--rw-r--r--   0 root         (0) root         (0)      228 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/monthday/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3141 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/monthday/base.py
--rw-r--r--   0 root         (0) root         (0)     1001 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/monthday/day_eq.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/monthday/day_gt.py
--rw-r--r--   0 root         (0) root         (0)     1132 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/monthday/day_gte.py
--rw-r--r--   0 root         (0) root         (0)     1129 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/monthday/day_lt.py
--rw-r--r--   0 root         (0) root         (0)     1132 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/monthday/day_lte.py
--rw-r--r--   0 root         (0) root         (0)      975 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/monthday/day_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 17:09:31.944292 m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/
--rw-r--r--   0 root         (0) root         (0)      328 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1442 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/base.py
--rw-r--r--   0 root         (0) root         (0)     1545 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/base_list.py
--rw-r--r--   0 root         (0) root         (0)      854 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/eq.py
--rw-r--r--   0 root         (0) root         (0)      872 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/gt.py
--rw-r--r--   0 root         (0) root         (0)      895 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/gte.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/list_gt.py
--rw-r--r--   0 root         (0) root         (0)      980 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/list_gte.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/list_lt.py
--rw-r--r--   0 root         (0) root         (0)      980 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/list_lte.py
--rw-r--r--   0 root         (0) root         (0)      863 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/lt.py
--rw-r--r--   0 root         (0) root         (0)      886 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/lte.py
--rw-r--r--   0 root         (0) root         (0)      869 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 17:09:31.947292 m-abac-1.0.8/mobio/libs/abac/policy/conditions/others/
--rw-r--r--   0 root         (0) root         (0)       73 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/others/__init__.py
--rw-r--r--   0 root         (0) root         (0)      963 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/others/base.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/others/exists.py
--rw-r--r--   0 root         (0) root         (0)      702 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/others/not_exists.py
--rw-r--r--   0 root         (0) root         (0)     2746 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 17:09:31.956293 m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/
--rw-r--r--   0 root         (0) root         (0)      401 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2051 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/base.py
--rw-r--r--   0 root         (0) root         (0)     1877 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/contains.py
--rw-r--r--   0 root         (0) root         (0)     1752 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/ends_with.py
--rw-r--r--   0 root         (0) root         (0)     1307 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/equals.py
--rw-r--r--   0 root         (0) root         (0)     1682 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/not_contains.py
--rw-r--r--   0 root         (0) root         (0)     1707 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/not_ends_with.py
--rw-r--r--   0 root         (0) root         (0)     1318 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/not_equals.py
--rw-r--r--   0 root         (0) root         (0)     1726 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/not_starts_with.py
--rw-r--r--   0 root         (0) root         (0)     1956 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/regex_match.py
--rw-r--r--   0 root         (0) root         (0)     1771 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/starts_with.py
--rw-r--r--   0 root         (0) root         (0)     1601 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     7835 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/policy.py
--rw-r--r--   0 root         (0) root         (0)     6467 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/policy/utils.py
--rw-r--r--   0 root         (0) root         (0)     6571 2023-10-13 17:05:47.000000 m-abac-1.0.8/mobio/libs/abac/result_access.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-10-13 17:05:47.000000 m-abac-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-13 17:09:31.958293 m-abac-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9835 2023-10-13 17:09:31.000000 m-abac-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 03:46:50.551328 m-abac-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-10-16 03:46:50.550327 m-abac-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      927 2023-10-13 17:05:47.000000 m-abac-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 03:46:50.479326 m-abac-1.0.9/m_abac.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-10-16 03:46:50.000000 m-abac-1.0.9/m_abac.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4522 2023-10-16 03:46:50.000000 m-abac-1.0.9/m_abac.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 03:46:50.000000 m-abac-1.0.9/m_abac.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      131 2023-10-16 03:46:50.000000 m-abac-1.0.9/m_abac.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-10-16 03:46:50.000000 m-abac-1.0.9/m_abac.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 03:46:50.469325 m-abac-1.0.9/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 03:46:50.469325 m-abac-1.0.9/mobio/libs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 03:46:50.483326 m-abac-1.0.9/mobio/libs/abac/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 03:46:50.486326 m-abac-1.0.9/mobio/libs/abac/adapter/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/adapter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/adapter/adapter.py
+-rw-r--r--   0 root         (0) root         (0)    26744 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/adapter/elasticsearch_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     7708 2023-10-16 03:45:03.000000 m-abac-1.0.9/mobio/libs/abac/call_api.py
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/config.py
+-rw-r--r--   0 root         (0) root         (0)    22178 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/pdp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 03:46:50.490326 m-abac-1.0.9/mobio/libs/abac/policy/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 03:46:50.492326 m-abac-1.0.9/mobio/libs/abac/policy/conditions/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 03:46:50.495326 m-abac-1.0.9/mobio/libs/abac/policy/conditions/boolean/
+-rw-r--r--   0 root         (0) root         (0)       39 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/boolean/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/boolean/base.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/boolean/check_bool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 03:46:50.504326 m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/
+-rw-r--r--   0 root         (0) root         (0)      418 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      680 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/all_in.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/all_not_in.py
+-rw-r--r--   0 root         (0) root         (0)      893 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/any_contains.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/any_in.py
+-rw-r--r--   0 root         (0) root         (0)      905 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/any_not_contains.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/any_not_in.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/base.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/is_empty.py
+-rw-r--r--   0 root         (0) root         (0)      602 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/is_in.py
+-rw-r--r--   0 root         (0) root         (0)      921 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
+-rw-r--r--   0 root         (0) root         (0)      728 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/is_not_in.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 03:46:50.510326 m-abac-1.0.9/mobio/libs/abac/policy/conditions/date_time/
+-rw-r--r--   0 root         (0) root         (0)      243 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/date_time/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/date_time/base.py
+-rw-r--r--   0 root         (0) root         (0)     1714 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_eq.py
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_gt.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_gte.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_lt.py
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_lte.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 03:46:50.517327 m-abac-1.0.9/mobio/libs/abac/policy/conditions/day/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/day/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3129 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/day/base.py
+-rw-r--r--   0 root         (0) root         (0)      966 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/day/day_eq.py
+-rw-r--r--   0 root         (0) root         (0)     1095 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/day/day_gt.py
+-rw-r--r--   0 root         (0) root         (0)     1097 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/day/day_gte.py
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/day/day_lt.py
+-rw-r--r--   0 root         (0) root         (0)     1097 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/day/day_lte.py
+-rw-r--r--   0 root         (0) root         (0)      940 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/day/day_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 03:46:50.521327 m-abac-1.0.9/mobio/libs/abac/policy/conditions/ip_address/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/ip_address/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/ip_address/base.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 03:46:50.527327 m-abac-1.0.9/mobio/libs/abac/policy/conditions/monthday/
+-rw-r--r--   0 root         (0) root         (0)      228 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/monthday/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3141 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/monthday/base.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/monthday/day_eq.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/monthday/day_gt.py
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/monthday/day_gte.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/monthday/day_lt.py
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/monthday/day_lte.py
+-rw-r--r--   0 root         (0) root         (0)      975 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/monthday/day_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 03:46:50.537327 m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/
+-rw-r--r--   0 root         (0) root         (0)      328 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/base.py
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/base_list.py
+-rw-r--r--   0 root         (0) root         (0)      854 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/eq.py
+-rw-r--r--   0 root         (0) root         (0)      872 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/gt.py
+-rw-r--r--   0 root         (0) root         (0)      895 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/gte.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/list_gt.py
+-rw-r--r--   0 root         (0) root         (0)      980 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/list_gte.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/list_lt.py
+-rw-r--r--   0 root         (0) root         (0)      980 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/list_lte.py
+-rw-r--r--   0 root         (0) root         (0)      863 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/lt.py
+-rw-r--r--   0 root         (0) root         (0)      886 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/lte.py
+-rw-r--r--   0 root         (0) root         (0)      869 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 03:46:50.541327 m-abac-1.0.9/mobio/libs/abac/policy/conditions/others/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/others/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      963 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/others/base.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/others/exists.py
+-rw-r--r--   0 root         (0) root         (0)      702 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/others/not_exists.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 03:46:50.549327 m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/
+-rw-r--r--   0 root         (0) root         (0)      401 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/base.py
+-rw-r--r--   0 root         (0) root         (0)     1877 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/contains.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/ends_with.py
+-rw-r--r--   0 root         (0) root         (0)     1307 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/equals.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/not_contains.py
+-rw-r--r--   0 root         (0) root         (0)     1707 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/not_ends_with.py
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/not_equals.py
+-rw-r--r--   0 root         (0) root         (0)     1726 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/not_starts_with.py
+-rw-r--r--   0 root         (0) root         (0)     1956 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/regex_match.py
+-rw-r--r--   0 root         (0) root         (0)     1771 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/starts_with.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     7835 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/policy.py
+-rw-r--r--   0 root         (0) root         (0)     6467 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/policy/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6571 2023-10-13 17:05:47.000000 m-abac-1.0.9/mobio/libs/abac/result_access.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-10-13 17:05:47.000000 m-abac-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-10-16 03:46:50.551328 m-abac-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9835 2023-10-16 03:46:49.000000 m-abac-1.0.9/setup.py
```

### Comparing `m-abac-1.0.8/PKG-INFO` & `m-abac-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac
-Version: 1.0.8
+Version: 1.0.9
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mobio-engine,m-abac
```

### Comparing `m-abac-1.0.8/README.md` & `m-abac-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/m_abac.egg-info/PKG-INFO` & `m-abac-1.0.9/m_abac.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac
-Version: 1.0.8
+Version: 1.0.9
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mobio-engine,m-abac
```

### Comparing `m-abac-1.0.8/m_abac.egg-info/SOURCES.txt` & `m-abac-1.0.9/m_abac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/adapter/elasticsearch_adapter.py` & `m-abac-1.0.9/mobio/libs/abac/adapter/elasticsearch_adapter.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/call_api.py` & `m-abac-1.0.9/mobio/libs/abac/call_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 
-from .config import lru_cache_redis, Mobio
+from .config import lru_redis_cache, Mobio
 
 
 class APIRequest:
     TimeOut = 10
     ADMIN_GET_FULL_INFO_ACCOUNT = "{domain}/adm/api/v2.1/accounts/{account_id}/full-info"
     ADMIN_GET_LIST_ACTION_FOR_MERCHANT = "{domain}/adm/api/v2.1/policies/actions/sdk"
     ADMIN_GET_LIST_STATEMENT = "{domain}/adm/api/v2.1/statements"
@@ -14,15 +14,15 @@
 # _TIME_CACHE = 60
 
 
 class CallAPI:
 
     # TODO: thay expiration cho production
     @staticmethod
-    @lru_cache_redis.add(expiration=_TIME_CACHE)
+    @lru_redis_cache.add(expiration=_TIME_CACHE)
     def admin_get_account_info(merchant_id, account_id):
         # try:
         url = APIRequest.ADMIN_GET_FULL_INFO_ACCOUNT.format(domain=Mobio.ADMIN_HOST, account_id=account_id)
         authorization = Mobio.MOBIO_TOKEN
         data_res = requests.get(
             url,
             headers={
@@ -38,15 +38,15 @@
         # print("abac_sdk admin_get_account_info: {}".format(data))
         return data
         # except Exception as er:
         #     err_msg = "abac_sdk admin_get_account_info err: {}".format(er)
         #     print(err_msg)
         #     return {}
 
-    @lru_cache_redis.add()
+    @lru_redis_cache.add()
     @staticmethod
     def admin_get_json_action(merchant_id):
         # try:
         url = APIRequest.ADMIN_GET_LIST_ACTION_FOR_MERCHANT.format(domain=Mobio.ADMIN_HOST)
         authorization = Mobio.MOBIO_TOKEN
         data_res = requests.get(
             url,
@@ -68,15 +68,15 @@
         # except Exception as er:
         #     err_msg = "abac_sdk admin_get_json_action err: {}".format(er)
         #     print(err_msg)
         #     return {}
 
     # TODO: thay expiration cho production
     @staticmethod
-    @lru_cache_redis.add(expiration=_TIME_CACHE)
+    @lru_redis_cache.add(expiration=_TIME_CACHE)
     def admin_get_list_statement(merchant_id, account_id, resource, action, service):
         """
         :param merchant_id:
         :param account_id:
         :param resource:
         :param action:
         :return: [{
```

### Comparing `m-abac-1.0.8/mobio/libs/abac/config.py` & `m-abac-1.0.9/mobio/libs/abac/config.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/pdp.py` & `m-abac-1.0.9/mobio/libs/abac/pdp.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/base.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/boolean/base.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/boolean/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/boolean/check_bool.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/boolean/check_bool.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/all_in.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/all_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/all_not_in.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/all_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/any_contains.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/any_contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/any_in.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/any_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/any_not_contains.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/any_not_contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/any_not_in.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/any_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/base.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/is_empty.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/is_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/is_in.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/is_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/is_not_empty.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/is_not_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/collection/is_not_in.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/collection/is_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/date_time/base.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/date_time/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_eq.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_gt.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_gte.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_lt.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_lte.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_neq.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/day/base.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/day/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/day/day_eq.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/day/day_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/day/day_gt.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/day/day_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/day/day_gte.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/day/day_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/day/day_lt.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/day/day_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/day/day_lte.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/day/day_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/day/day_neq.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/day/day_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/ip_address/base.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/ip_address/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/monthday/base.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/monthday/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/monthday/day_eq.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/monthday/day_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/monthday/day_gt.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/monthday/day_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/monthday/day_gte.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/monthday/day_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/monthday/day_lt.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/monthday/day_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/monthday/day_lte.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/monthday/day_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/monthday/day_neq.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/monthday/day_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/base.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/base_list.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/base_list.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/eq.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/gt.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/gte.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/list_gt.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/list_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/list_gte.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/list_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/list_lt.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/list_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/list_lte.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/list_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/lt.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/lte.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/numeric/neq.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/numeric/neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/others/base.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/others/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/others/exists.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/others/exists.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/others/not_exists.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/others/not_exists.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/schema.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/schema.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/base.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/contains.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/ends_with.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/ends_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/equals.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/not_contains.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/not_contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/not_ends_with.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/not_ends_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/not_equals.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/not_equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/not_starts_with.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/not_starts_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/regex_match.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/regex_match.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/conditions/string/starts_with.py` & `m-abac-1.0.9/mobio/libs/abac/policy/conditions/string/starts_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/exceptions.py` & `m-abac-1.0.9/mobio/libs/abac/policy/exceptions.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/policy.py` & `m-abac-1.0.9/mobio/libs/abac/policy/policy.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/policy/utils.py` & `m-abac-1.0.9/mobio/libs/abac/policy/utils.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/mobio/libs/abac/result_access.py` & `m-abac-1.0.9/mobio/libs/abac/result_access.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.8/setup.py` & `m-abac-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         # with open(Requirements.requirements_path) as req_file:
         #     for line in req_file.read().splitlines():
         #         if not line.strip().startswith("#"):
         #             requirements.append(line)
         return requirements
 
 version_dev='1.0.37'
-version_prod='1.0.8'
+version_prod='1.0.9'
 
 run_mode=''
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
@@ -72,15 +72,15 @@
     # options={"bdist_wheel": {"universal": True}},
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.8',  # Required
+    version='1.0.9',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

