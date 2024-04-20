# Comparing `tmp/limits-3.8.0.tar.gz` & `tmp/limits-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limits-3.8.0.tar", last modified: Wed Feb 14 23:52:58 2024, max compression
+gzip compressed data, was "limits-3.9.0.tar", last modified: Sun Feb 18 02:06:52 2024, max compression
```

## Comparing `limits-3.8.0.tar` & `limits-3.9.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 23:52:58.325616 limits-3.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-14 23:52:51.000000 limits-3.8.0/CLASSIFIERS
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-14 23:52:51.000000 limits-3.8.0/CONTRIBUTIONS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-02-14 23:52:51.000000 limits-3.8.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-14 23:52:51.000000 limits-3.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-14 23:52:51.000000 limits-3.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-02-14 23:52:58.325616 limits-3.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-02-14 23:52:51.000000 limits-3.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 23:52:58.309616 limits-3.8.0/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-02-14 23:52:51.000000 limits-3.8.0/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 23:52:58.313616 limits-3.8.0/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 23:52:58.313616 limits-3.8.0/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-14 23:52:51.000000 limits-3.8.0/doc/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-02-14 23:52:51.000000 limits-3.8.0/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-02-14 23:52:51.000000 limits-3.8.0/doc/source/async.rst
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-14 23:52:51.000000 limits-3.8.0/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-02-14 23:52:51.000000 limits-3.8.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-02-14 23:52:51.000000 limits-3.8.0/doc/source/custom-storage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-02-14 23:52:51.000000 limits-3.8.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-02-14 23:52:51.000000 limits-3.8.0/doc/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-02-14 23:52:51.000000 limits-3.8.0/doc/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8575 2024-02-14 23:52:51.000000 limits-3.8.0/doc/source/storage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-02-14 23:52:51.000000 limits-3.8.0/doc/source/strategies.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-02-14 23:52:51.000000 limits-3.8.0/doc/source/theme_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 23:52:58.325616 limits-3.8.0/limits/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-02-14 23:52:51.000000 limits-3.8.0/limits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-14 23:52:58.325616 limits-3.8.0/limits/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 23:52:58.317616 limits-3.8.0/limits/aio/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-14 23:52:51.000000 limits-3.8.0/limits/aio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 23:52:58.317616 limits-3.8.0/limits/aio/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-14 23:52:51.000000 limits-3.8.0/limits/aio/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-02-14 23:52:51.000000 limits-3.8.0/limits/aio/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-02-14 23:52:51.000000 limits-3.8.0/limits/aio/storage/etcd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-02-14 23:52:51.000000 limits-3.8.0/limits/aio/storage/memcached.py
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-02-14 23:52:51.000000 limits-3.8.0/limits/aio/storage/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-02-14 23:52:51.000000 limits-3.8.0/limits/aio/storage/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)    15640 2024-02-14 23:52:51.000000 limits-3.8.0/limits/aio/storage/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-02-14 23:52:51.000000 limits-3.8.0/limits/aio/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-02-14 23:52:51.000000 limits-3.8.0/limits/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-02-14 23:52:51.000000 limits-3.8.0/limits/limits.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 23:52:51.000000 limits-3.8.0/limits/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 23:52:58.309616 limits-3.8.0/limits/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 23:52:58.309616 limits-3.8.0/limits/resources/redis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 23:52:58.317616 limits-3.8.0/limits/resources/redis/lua_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-14 23:52:51.000000 limits-3.8.0/limits/resources/redis/lua_scripts/acquire_moving_window.lua
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-14 23:52:51.000000 limits-3.8.0/limits/resources/redis/lua_scripts/clear_keys.lua
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-14 23:52:51.000000 limits-3.8.0/limits/resources/redis/lua_scripts/incr_expire.lua
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-14 23:52:51.000000 limits-3.8.0/limits/resources/redis/lua_scripts/moving_window.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 23:52:58.321616 limits-3.8.0/limits/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-02-14 23:52:51.000000 limits-3.8.0/limits/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-02-14 23:52:51.000000 limits-3.8.0/limits/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-02-14 23:52:51.000000 limits-3.8.0/limits/storage/etcd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-02-14 23:52:51.000000 limits-3.8.0/limits/storage/memcached.py
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-02-14 23:52:51.000000 limits-3.8.0/limits/storage/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-02-14 23:52:51.000000 limits-3.8.0/limits/storage/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-02-14 23:52:51.000000 limits-3.8.0/limits/storage/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-02-14 23:52:51.000000 limits-3.8.0/limits/storage/redis_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-02-14 23:52:51.000000 limits-3.8.0/limits/storage/redis_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-14 23:52:51.000000 limits-3.8.0/limits/storage/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-02-14 23:52:51.000000 limits-3.8.0/limits/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-02-14 23:52:51.000000 limits-3.8.0/limits/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-02-14 23:52:51.000000 limits-3.8.0/limits/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-14 23:52:51.000000 limits-3.8.0/limits/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 23:52:58.321616 limits-3.8.0/limits.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-02-14 23:52:58.000000 limits-3.8.0/limits.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-02-14 23:52:58.000000 limits-3.8.0/limits.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 23:52:58.000000 limits-3.8.0/limits.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 23:52:58.000000 limits-3.8.0/limits.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-02-14 23:52:58.000000 limits-3.8.0/limits.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-14 23:52:58.000000 limits-3.8.0/limits.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-14 23:52:51.000000 limits-3.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 23:52:58.321616 limits-3.8.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-14 23:52:51.000000 limits-3.8.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-14 23:52:51.000000 limits-3.8.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-14 23:52:51.000000 limits-3.8.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-14 23:52:51.000000 limits-3.8.0/requirements/main.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 23:52:58.321616 limits-3.8.0/requirements/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-14 23:52:51.000000 limits-3.8.0/requirements/storage/async-etcd.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-14 23:52:51.000000 limits-3.8.0/requirements/storage/async-memcached.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-14 23:52:51.000000 limits-3.8.0/requirements/storage/async-mongodb.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-14 23:52:51.000000 limits-3.8.0/requirements/storage/async-redis.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-14 23:52:51.000000 limits-3.8.0/requirements/storage/etcd.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-14 23:52:51.000000 limits-3.8.0/requirements/storage/memcached.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-14 23:52:51.000000 limits-3.8.0/requirements/storage/mongodb.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-14 23:52:51.000000 limits-3.8.0/requirements/storage/redis.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-14 23:52:51.000000 limits-3.8.0/requirements/storage/rediscluster.txt
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-02-14 23:52:51.000000 limits-3.8.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-02-14 23:52:58.325616 limits-3.8.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1928 2024-02-14 23:52:51.000000 limits-3.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 23:52:58.321616 limits-3.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-02-14 23:52:51.000000 limits-3.8.0/tests/test_limit_granularities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-02-14 23:52:51.000000 limits-3.8.0/tests/test_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-02-14 23:52:51.000000 limits-3.8.0/tests/test_ratelimit_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-02-14 23:52:51.000000 limits-3.8.0/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-02-14 23:52:51.000000 limits-3.8.0/tests/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-02-14 23:52:51.000000 limits-3.8.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    81180 2024-02-14 23:52:51.000000 limits-3.8.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 02:06:52.886496 limits-3.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-18 02:06:46.000000 limits-3.9.0/CLASSIFIERS
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-18 02:06:46.000000 limits-3.9.0/CONTRIBUTIONS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-02-18 02:06:46.000000 limits-3.9.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-18 02:06:46.000000 limits-3.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-18 02:06:46.000000 limits-3.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-02-18 02:06:52.886496 limits-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-02-18 02:06:46.000000 limits-3.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 02:06:52.874496 limits-3.9.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-02-18 02:06:46.000000 limits-3.9.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 02:06:52.874496 limits-3.9.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 02:06:52.874496 limits-3.9.0/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-18 02:06:46.000000 limits-3.9.0/doc/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-02-18 02:06:46.000000 limits-3.9.0/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-02-18 02:06:46.000000 limits-3.9.0/doc/source/async.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-18 02:06:46.000000 limits-3.9.0/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-02-18 02:06:46.000000 limits-3.9.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-02-18 02:06:46.000000 limits-3.9.0/doc/source/custom-storage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-02-18 02:06:46.000000 limits-3.9.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-02-18 02:06:46.000000 limits-3.9.0/doc/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-02-18 02:06:46.000000 limits-3.9.0/doc/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8575 2024-02-18 02:06:46.000000 limits-3.9.0/doc/source/storage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-02-18 02:06:46.000000 limits-3.9.0/doc/source/strategies.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-02-18 02:06:46.000000 limits-3.9.0/doc/source/theme_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 02:06:52.886496 limits-3.9.0/limits/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-02-18 02:06:46.000000 limits-3.9.0/limits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-18 02:06:52.886496 limits-3.9.0/limits/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 02:06:52.878497 limits-3.9.0/limits/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-18 02:06:46.000000 limits-3.9.0/limits/aio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 02:06:52.878497 limits-3.9.0/limits/aio/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-18 02:06:46.000000 limits-3.9.0/limits/aio/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-02-18 02:06:46.000000 limits-3.9.0/limits/aio/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-02-18 02:06:46.000000 limits-3.9.0/limits/aio/storage/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-02-18 02:06:46.000000 limits-3.9.0/limits/aio/storage/memcached.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-02-18 02:06:46.000000 limits-3.9.0/limits/aio/storage/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-02-18 02:06:46.000000 limits-3.9.0/limits/aio/storage/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15640 2024-02-18 02:06:46.000000 limits-3.9.0/limits/aio/storage/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-02-18 02:06:46.000000 limits-3.9.0/limits/aio/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-02-18 02:06:46.000000 limits-3.9.0/limits/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-02-18 02:06:46.000000 limits-3.9.0/limits/limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 02:06:46.000000 limits-3.9.0/limits/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 02:06:52.870496 limits-3.9.0/limits/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 02:06:52.870496 limits-3.9.0/limits/resources/redis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 02:06:52.878497 limits-3.9.0/limits/resources/redis/lua_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-18 02:06:46.000000 limits-3.9.0/limits/resources/redis/lua_scripts/acquire_moving_window.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-18 02:06:46.000000 limits-3.9.0/limits/resources/redis/lua_scripts/clear_keys.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-18 02:06:46.000000 limits-3.9.0/limits/resources/redis/lua_scripts/incr_expire.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-18 02:06:46.000000 limits-3.9.0/limits/resources/redis/lua_scripts/moving_window.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 02:06:52.882496 limits-3.9.0/limits/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-02-18 02:06:46.000000 limits-3.9.0/limits/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-02-18 02:06:46.000000 limits-3.9.0/limits/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-02-18 02:06:46.000000 limits-3.9.0/limits/storage/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-02-18 02:06:46.000000 limits-3.9.0/limits/storage/memcached.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-02-18 02:06:46.000000 limits-3.9.0/limits/storage/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-02-18 02:06:46.000000 limits-3.9.0/limits/storage/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-02-18 02:06:46.000000 limits-3.9.0/limits/storage/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-02-18 02:06:46.000000 limits-3.9.0/limits/storage/redis_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-02-18 02:06:46.000000 limits-3.9.0/limits/storage/redis_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-18 02:06:46.000000 limits-3.9.0/limits/storage/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-02-18 02:06:46.000000 limits-3.9.0/limits/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-02-18 02:06:46.000000 limits-3.9.0/limits/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-02-18 02:06:46.000000 limits-3.9.0/limits/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-18 02:06:46.000000 limits-3.9.0/limits/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 02:06:52.882496 limits-3.9.0/limits.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-02-18 02:06:52.000000 limits-3.9.0/limits.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-02-18 02:06:52.000000 limits-3.9.0/limits.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-18 02:06:52.000000 limits-3.9.0/limits.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-18 02:06:52.000000 limits-3.9.0/limits.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-02-18 02:06:52.000000 limits-3.9.0/limits.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-18 02:06:52.000000 limits-3.9.0/limits.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-18 02:06:46.000000 limits-3.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 02:06:52.882496 limits-3.9.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-18 02:06:46.000000 limits-3.9.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-18 02:06:46.000000 limits-3.9.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-18 02:06:46.000000 limits-3.9.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-18 02:06:46.000000 limits-3.9.0/requirements/main.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 02:06:52.882496 limits-3.9.0/requirements/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-18 02:06:46.000000 limits-3.9.0/requirements/storage/async-etcd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-18 02:06:46.000000 limits-3.9.0/requirements/storage/async-memcached.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-18 02:06:46.000000 limits-3.9.0/requirements/storage/async-mongodb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-18 02:06:46.000000 limits-3.9.0/requirements/storage/async-redis.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-18 02:06:46.000000 limits-3.9.0/requirements/storage/etcd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-18 02:06:46.000000 limits-3.9.0/requirements/storage/memcached.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-18 02:06:46.000000 limits-3.9.0/requirements/storage/mongodb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-18 02:06:46.000000 limits-3.9.0/requirements/storage/redis.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-18 02:06:46.000000 limits-3.9.0/requirements/storage/rediscluster.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-02-18 02:06:46.000000 limits-3.9.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-02-18 02:06:52.886496 limits-3.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1928 2024-02-18 02:06:46.000000 limits-3.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 02:06:52.882496 limits-3.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-02-18 02:06:46.000000 limits-3.9.0/tests/test_limit_granularities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-02-18 02:06:46.000000 limits-3.9.0/tests/test_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-02-18 02:06:46.000000 limits-3.9.0/tests/test_ratelimit_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-02-18 02:06:46.000000 limits-3.9.0/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-02-18 02:06:46.000000 limits-3.9.0/tests/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-02-18 02:06:46.000000 limits-3.9.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81180 2024-02-18 02:06:46.000000 limits-3.9.0/versioneer.py
```

### Comparing `limits-3.8.0/HISTORY.rst` & `limits-3.9.0/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 .. :changelog:
 
 Changelog
 =========
 
+v3.9.0
+------
+Release Date: 2024-02-17
+
+* Bug Fix
+
+  * Remove excessively low defaults for mongodb storage and instead
+    delegate to the underlying dependency (pymongo, motor)
+
+
 v3.8.0
 ------
 Release Date: 2024-02-14
 
 * Features
 
   * Add option to wrap storage errors with a ``StorageError``
@@ -591,14 +601,15 @@
 
 
 
 
 
 
 
+
```

### Comparing `limits-3.8.0/LICENSE.txt` & `limits-3.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/PKG-INFO` & `limits-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limits
-Version: 3.8.0
+Version: 3.9.0
 Summary: Rate limiting utilities
 Home-page: https://limits.readthedocs.org
 Author: Ali-Akber Saifee
 Author-email: ali@indydevs.org
 License: MIT
 Project-URL: Source, https://github.com/alisaifee/limits
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `limits-3.8.0/README.rst` & `limits-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/doc/Makefile` & `limits-3.9.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/doc/source/api.rst` & `limits-3.9.0/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/doc/source/async.rst` & `limits-3.9.0/doc/source/async.rst`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/doc/source/conf.py` & `limits-3.9.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/doc/source/custom-storage.rst` & `limits-3.9.0/doc/source/custom-storage.rst`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/doc/source/index.rst` & `limits-3.9.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/doc/source/installation.rst` & `limits-3.9.0/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/doc/source/quickstart.rst` & `limits-3.9.0/doc/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/doc/source/storage.rst` & `limits-3.9.0/doc/source/storage.rst`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/doc/source/strategies.rst` & `limits-3.9.0/doc/source/strategies.rst`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/doc/source/theme_config.py` & `limits-3.9.0/doc/source/theme_config.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/__init__.py` & `limits-3.9.0/limits/__init__.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/aio/storage/__init__.py` & `limits-3.9.0/limits/aio/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/aio/storage/base.py` & `limits-3.9.0/limits/aio/storage/base.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/aio/storage/etcd.py` & `limits-3.9.0/limits/aio/storage/etcd.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/aio/storage/memcached.py` & `limits-3.9.0/limits/aio/storage/memcached.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/aio/storage/memory.py` & `limits-3.9.0/limits/aio/storage/memory.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/aio/storage/mongodb.py` & `limits-3.9.0/limits/aio/storage/mongodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,20 +25,14 @@
     """
 
     STORAGE_SCHEME = ["async+mongodb", "async+mongodb+srv"]
     """
     The storage scheme for MongoDB for use in an async context
     """
 
-    DEFAULT_OPTIONS: Dict[str, Union[float, str, bool]] = {
-        "serverSelectionTimeoutMS": 1000,
-        "connectTimeoutMS": 1000,
-    }
-    "Default options passed to :class:`~motor.motor_asyncio.AsyncIOMotorClient`"
-
     DEPENDENCIES = ["motor.motor_asyncio", "pymongo"]
 
     def __init__(
         self,
         uri: str,
         database_name: str = "limits",
         wrap_exceptions: bool = False,
@@ -47,32 +41,29 @@
         """
         :param uri: uri of the form ``async+mongodb://[user:password]@host:port?...``,
          This uri is passed directly to :class:`~motor.motor_asyncio.AsyncIOMotorClient`
         :param database_name: The database to use for storing the rate limit
          collections.
         :param wrap_exceptions: Whether to wrap storage exceptions in
          :exc:`limits.errors.StorageError` before raising it.
-        :param options: all remaining keyword arguments are merged with
-         :data:`DEFAULT_OPTIONS` and passed to the constructor of
-         :class:`~motor.motor_asyncio.AsyncIOMotorClient`
+        :param options: all remaining keyword arguments are passed
+         to the constructor of :class:`~motor.motor_asyncio.AsyncIOMotorClient`
         :raise ConfigurationError: when the :pypi:`motor` or :pypi:`pymongo` are
          not available
         """
 
-        mongo_opts = options.copy()
-        [mongo_opts.setdefault(k, v) for k, v in self.DEFAULT_OPTIONS.items()]
         uri = uri.replace("async+mongodb", "mongodb", 1)
 
         super().__init__(uri, wrap_exceptions=wrap_exceptions, **options)
 
         self.dependency = self.dependencies["motor.motor_asyncio"]
         self.proxy_dependency = self.dependencies["pymongo"]
         self.lib_errors, _ = get_dependency("pymongo.errors")
 
-        self.storage = self.dependency.module.AsyncIOMotorClient(uri, **mongo_opts)
+        self.storage = self.dependency.module.AsyncIOMotorClient(uri, **options)
         # TODO: Fix this hack. It was noticed when running a benchmark
         # with FastAPI - however - doesn't appear in unit tests or in an isolated
         # use. Reference: https://jira.mongodb.org/browse/MOTOR-822
         self.storage.get_io_loop = asyncio.get_running_loop
 
         self.__database_name = database_name
         self.__indices_created = False
```

### Comparing `limits-3.8.0/limits/aio/storage/redis.py` & `limits-3.9.0/limits/aio/storage/redis.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/aio/strategies.py` & `limits-3.9.0/limits/aio/strategies.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/errors.py` & `limits-3.9.0/limits/errors.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/limits.py` & `limits-3.9.0/limits/limits.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/storage/__init__.py` & `limits-3.9.0/limits/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/storage/base.py` & `limits-3.9.0/limits/storage/base.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/storage/etcd.py` & `limits-3.9.0/limits/storage/etcd.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/storage/memcached.py` & `limits-3.9.0/limits/storage/memcached.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/storage/memory.py` & `limits-3.9.0/limits/storage/memory.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/storage/mongodb.py` & `limits-3.9.0/limits/storage/mongodb.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,19 +21,14 @@
     """
     Rate limit storage with MongoDB as backend.
 
     Depends on :pypi:`pymongo`.
     """
 
     STORAGE_SCHEME = ["mongodb", "mongodb+srv"]
-    DEFAULT_OPTIONS: Dict[str, Union[int, str, bool]] = {
-        "serverSelectionTimeoutMS": 1000,
-        "connectTimeoutMS": 1000,
-    }
-    "Default options passed to :class:`~pymongo.mongo_client.MongoClient`"
 
     DEPENDENCIES = ["pymongo"]
 
     def __init__(
         self,
         uri: str,
         database_name: str = "limits",
@@ -43,30 +38,26 @@
         """
         :param uri: uri of the form ``mongodb://[user:password]@host:port?...``,
          This uri is passed directly to :class:`~pymongo.mongo_client.MongoClient`
         :param database_name: The database to use for storing the rate limit
          collections.
         :param wrap_exceptions: Whether to wrap storage exceptions in
          :exc:`limits.errors.StorageError` before raising it.
-        :param options: all remaining keyword arguments are merged with
-         :data:`DEFAULT_OPTIONS` and passed to the constructor of
-         :class:`~pymongo.mongo_client.MongoClient`
+        :param options: all remaining keyword arguments are passed to the
+         constructor of :class:`~pymongo.mongo_client.MongoClient`
         :raise ConfigurationError: when the :pypi:`pymongo` library is not available
         """
 
         super().__init__(uri, wrap_exceptions=wrap_exceptions, **options)
 
         self.lib = self.dependencies["pymongo"].module
         self.lib_errors, _ = get_dependency("pymongo.errors")
 
-        mongo_opts = options.copy()
-        [mongo_opts.setdefault(k, v) for k, v in self.DEFAULT_OPTIONS.items()]
-
         self.storage: "pymongo.MongoClient" = self.lib.MongoClient(  # type: ignore[type-arg]
-            uri, **mongo_opts
+            uri, **options
         )
         self.counters = self.storage.get_database(database_name).counters
         self.windows = self.storage.get_database(database_name).windows
         self.__initialize_database()
 
     @property
     def base_exceptions(
```

### Comparing `limits-3.8.0/limits/storage/redis.py` & `limits-3.9.0/limits/storage/redis.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/storage/redis_cluster.py` & `limits-3.9.0/limits/storage/redis_cluster.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/storage/redis_sentinel.py` & `limits-3.9.0/limits/storage/redis_sentinel.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/storage/registry.py` & `limits-3.9.0/limits/storage/registry.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/strategies.py` & `limits-3.9.0/limits/strategies.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/typing.py` & `limits-3.9.0/limits/typing.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits/util.py` & `limits-3.9.0/limits/util.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits.egg-info/PKG-INFO` & `limits-3.9.0/limits.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limits
-Version: 3.8.0
+Version: 3.9.0
 Summary: Rate limiting utilities
 Home-page: https://limits.readthedocs.org
 Author: Ali-Akber Saifee
 Author-email: ali@indydevs.org
 License: MIT
 Project-URL: Source, https://github.com/alisaifee/limits
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `limits-3.8.0/limits.egg-info/SOURCES.txt` & `limits-3.9.0/limits.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/limits.egg-info/requires.txt` & `limits-3.9.0/limits.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/setup.cfg` & `limits-3.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/setup.py` & `limits-3.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/tests/test_limit_granularities.py` & `limits-3.9.0/tests/test_limit_granularities.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/tests/test_limits.py` & `limits-3.9.0/tests/test_limits.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/tests/test_ratelimit_parser.py` & `limits-3.9.0/tests/test_ratelimit_parser.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/tests/test_storage.py` & `limits-3.9.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/tests/test_strategy.py` & `limits-3.9.0/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/tests/test_utils.py` & `limits-3.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `limits-3.8.0/versioneer.py` & `limits-3.9.0/versioneer.py`

 * *Files identical despite different names*

