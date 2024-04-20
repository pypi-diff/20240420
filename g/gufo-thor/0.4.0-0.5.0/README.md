# Comparing `tmp/gufo_thor-0.4.0.tar.gz` & `tmp/gufo_thor-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gufo_thor-0.4.0.tar", last modified: Fri Dec 29 13:57:11 2023, max compression
+gzip compressed data, was "gufo_thor-0.5.0.tar", last modified: Sat Apr 20 08:22:14 2024, max compression
```

## Comparing `gufo_thor-0.4.0.tar` & `gufo_thor-0.5.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:57:11.149056 gufo_thor-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2023-12-29 13:57:11.149056 gufo_thor-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-29 13:57:11.149056 gufo_thor-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:57:11.141056 gufo_thor-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:57:11.137056 gufo_thor-0.4.0/src/gufo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:57:11.141056 gufo_thor-0.4.0/src/gufo/thor/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:57:11.141056 gufo_thor-0.4.0/src/gufo/thor/samples/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/samples/common.yml
--rw-r--r--   0 runner    (1001) docker     (127)      221 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/samples/simple.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:57:11.149056 gufo_thor-0.4.0/src/gufo/thor/services/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/activator.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    17268 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/bh.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/bi.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/card.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/chwriter.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/consul.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/correlator.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/datastream.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/envoy.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/escalator.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/grafanads.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/icqsender.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/kafkasender.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/liftbridge.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/login.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/mailsender.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/metricscollector.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/mib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/migrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/mongo.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/mrt.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/mx.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/nbi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/noc.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/sae.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/selfmon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/static.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/syslogcollector.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/tgsender.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/topo.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/trapcollector.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/web.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/services/zeroconf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:57:11.149056 gufo_thor-0.4.0/src/gufo/thor/targets/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/targets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/targets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/targets/compose.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:57:11.141056 gufo_thor-0.4.0/src/gufo/thor/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:57:11.149056 gufo_thor-0.4.0/src/gufo/thor/templates/envoy/
--rw-r--r--   0 runner    (1001) docker     (127)     7545 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/templates/envoy/envoy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:57:11.149056 gufo_thor-0.4.0/src/gufo/thor/templates/liftbridge/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/templates/liftbridge/liftbridge.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:57:11.149056 gufo_thor-0.4.0/src/gufo/thor/templates/noc/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/templates/noc/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/src/gufo/thor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:57:11.149056 gufo_thor-0.4.0/src/gufo_thor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2023-12-29 13:57:11.000000 gufo_thor-0.4.0/src/gufo_thor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2023-12-29 13:57:11.000000 gufo_thor-0.4.0/src/gufo_thor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-29 13:57:11.000000 gufo_thor-0.4.0/src/gufo_thor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-29 13:57:11.000000 gufo_thor-0.4.0/src/gufo_thor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-29 13:57:11.000000 gufo_thor-0.4.0/src/gufo_thor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-29 13:57:11.000000 gufo_thor-0.4.0/src/gufo_thor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:57:11.149056 gufo_thor-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/tests/test_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)     7111 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/tests/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     6902 2023-12-29 13:56:55.000000 gufo_thor-0.4.0/tests/test_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:22:14.803727 gufo_thor-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-20 08:22:14.803727 gufo_thor-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 08:22:14.803727 gufo_thor-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:22:14.791727 gufo_thor-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:22:14.791727 gufo_thor-0.5.0/src/gufo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:22:14.791727 gufo_thor-0.5.0/src/gufo/thor/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:22:14.791727 gufo_thor-0.5.0/src/gufo/thor/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/samples/common.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/samples/simple.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:22:14.799727 gufo_thor-0.5.0/src/gufo/thor/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/activator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17268 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/bh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/bi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/chwriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/consul.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/correlator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/datastream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/envoy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/escalator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/grafanads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/icqsender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/kafkasender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/liftbridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/mailsender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/metricscollector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/mib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/mrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/mx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/nbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/noc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/sae.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/selfmon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/syslogcollector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/tgsender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/topo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/trapcollector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/web.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/services/zeroconf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:22:14.799727 gufo_thor-0.5.0/src/gufo/thor/targets/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/targets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/targets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/targets/compose.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:22:14.791727 gufo_thor-0.5.0/src/gufo/thor/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:22:14.799727 gufo_thor-0.5.0/src/gufo/thor/templates/envoy/
+-rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/templates/envoy/envoy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:22:14.799727 gufo_thor-0.5.0/src/gufo/thor/templates/liftbridge/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/templates/liftbridge/liftbridge.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:22:14.799727 gufo_thor-0.5.0/src/gufo/thor/templates/noc/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/templates/noc/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/src/gufo/thor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:22:14.803727 gufo_thor-0.5.0/src/gufo_thor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-20 08:22:14.000000 gufo_thor-0.5.0/src/gufo_thor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-20 08:22:14.000000 gufo_thor-0.5.0/src/gufo_thor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 08:22:14.000000 gufo_thor-0.5.0/src/gufo_thor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-20 08:22:14.000000 gufo_thor-0.5.0/src/gufo_thor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-20 08:22:14.000000 gufo_thor-0.5.0/src/gufo_thor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-20 08:22:14.000000 gufo_thor-0.5.0/src/gufo_thor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:22:14.803727 gufo_thor-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/tests/test_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/tests/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-04-20 08:22:07.000000 gufo_thor-0.5.0/tests/test_service.py
```

### Comparing `gufo_thor-0.4.0/LICENSE.md` & `gufo_thor-0.5.0/LICENSE.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 hide:
     - navigation
 ---
-Copyright &copy; 2023, Gufo Labs.
+Copyright &copy; 2023-2024, Gufo Labs.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
```

### Comparing `gufo_thor-0.4.0/PKG-INFO` & `gufo_thor-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gufo_thor
-Version: 0.4.0
+Version: 0.5.0
 Author: Gufo Labs
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/gufolabs/gufo_thor/issues
 Project-URL: Changelog, https://github.com/gufolabs/gufo_thor/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://docs.gufolabs.com/gufo_thor/
 Project-URL: Homepage, https://github.com/gufolabs/gufo_thor/
 Project-URL: Source Code, https://github.com/gufolabs/gufo_thor/
```

### Comparing `gufo_thor-0.4.0/README.md` & `gufo_thor-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/pyproject.toml` & `gufo_thor-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/cli.py` & `gufo_thor-0.5.0/src/gufo/thor/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,15 +71,18 @@
             "--template",
             default="simple",
             help="Select sample config template",
         )
         # prepare
         subparsers.add_parser("prepare", help="Prepare services configuration")
         # up
-        subparsers.add_parser("up", help="Set up ana launch NOC")
+        up_parser = subparsers.add_parser("up", help="Set up and launch NOC")
+        up_parser.add_argument(
+            "--no-migrate", action="store_true", help="Skip migrations on run"
+        )
         # down
         subparsers.add_parser("stop", help="Stop NOC")
         # shell
         subparsers.add_parser("shell", help="Run shell")
         # Parse arguments
         ns = parser.parse_args(args)
         # Set up logging
@@ -147,15 +150,15 @@
         Returns:
             Config instance.
         """
         path = "thor.yml"
         with open(path) as fp:
             return Config.from_yaml(fp.read())
 
-    def handle_prepare(self: "Cli", _ns: argparse.Namespace) -> ExitCode:
+    def handle_prepare(self: "Cli", ns: argparse.Namespace) -> ExitCode:
         """Prepare NOC configuration."""
         from gufo.thor.targets.base import loader
 
         # Read config
         path = "thor.yml"
         if not os.path.exists(path):
             from gufo.thor.config import get_sample
@@ -182,14 +185,18 @@
         if cfg.expose.port != DEFAULT_HTTPS_PORT:
             parts.append(f":{cfg.expose.port}")
         parts.append("/")
         return "".join(parts)
 
     def handle_up(self: "Cli", ns: argparse.Namespace) -> ExitCode:
         """Prepare NOC configuration and run NOC."""
+        # --no-migrations
+        if ns.no_migrate:
+            self.config.cli.no_migrate = True
+        #
         r = self.handle_prepare(ns)
         if r != ExitCode.OK:
             return r
         if not docker.up():
             return ExitCode.ERR
         # Open UI
         url = self._get_ui_url()
```

### Comparing `gufo_thor-0.4.0/src/gufo/thor/config.py` & `gufo_thor-0.5.0/src/gufo/thor/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,14 +108,29 @@
     @staticmethod
     def default() -> "ServiceConfig":
         """Get default ServiceConfig."""
         return ServiceConfig(tag=None, scale=1)
 
 
 @dataclass
+class CliConfig(object):
+    """
+    Config populated during runtime.
+
+    Should not be set by user. Populated
+    from CLI options.
+
+    Attributes:
+        no_migrations: Skip migrations if true.
+    """
+
+    no_migrate: bool = False
+
+
+@dataclass
 class Config(object):
     """
     The Gufo Thor config.
 
     Attributes:
         project: Optional project name used to prefix
             the services and volumes. If not set - directory
@@ -126,14 +141,15 @@
         services: The `services` section of the config.
     """
 
     project: Optional[str]
     noc: NocConfig
     expose: ExposeConfig
     services: Dict[str, ServiceConfig]
+    cli: CliConfig
 
     @staticmethod
     def from_yaml(data: str) -> "Config":
         """
         Parse YAML file and return an instance of the Config.
 
         Args:
@@ -161,28 +177,33 @@
             msg = f"services must be list or dict, not {type(data_svc)}"
             raise ValueError(msg)
         return Config(
             project=cfg.get("project"),
             noc=noc_cfg,
             expose=expose_cfg,
             services=services,
+            cli=CliConfig(),
         )
 
     @staticmethod
     def default() -> "Config":
         """
         Generate default config.
 
         Returns:
             An Config instance
         """
         noc_cfg = NocConfig()
         expose_cfg = ExposeConfig()
         return Config(
-            project=None, noc=noc_cfg, expose=expose_cfg, services={}
+            project=None,
+            noc=noc_cfg,
+            expose=expose_cfg,
+            services={},
+            cli=CliConfig(),
         )
 
 
 def get_sample(name: str) -> str:
     """
     Get preconfigured config sample by name.
```

### Comparing `gufo_thor-0.4.0/src/gufo/thor/docker.py` & `gufo_thor-0.5.0/src/gufo/thor/docker.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/activator.py` & `gufo_thor-0.5.0/src/gufo/thor/services/activator.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/auth.py` & `gufo_thor-0.5.0/src/gufo/thor/services/auth.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/base.py` & `gufo_thor-0.5.0/src/gufo/thor/services/base.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/bi.py` & `gufo_thor-0.5.0/src/gufo/thor/services/bi.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/card.py` & `gufo_thor-0.5.0/src/gufo/thor/services/card.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/chwriter.py` & `gufo_thor-0.5.0/src/gufo/thor/services/chwriter.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/classifier.py` & `gufo_thor-0.5.0/src/gufo/thor/services/classifier.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/clickhouse.py` & `gufo_thor-0.5.0/src/gufo/thor/services/clickhouse.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/consul.py` & `gufo_thor-0.5.0/src/gufo/thor/services/consul.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/correlator.py` & `gufo_thor-0.5.0/src/gufo/thor/services/correlator.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/datasource.py` & `gufo_thor-0.5.0/src/gufo/thor/services/datasource.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/datastream.py` & `gufo_thor-0.5.0/src/gufo/thor/services/datastream.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/discovery.py` & `gufo_thor-0.5.0/src/gufo/thor/services/discovery.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/envoy.py` & `gufo_thor-0.5.0/src/gufo/thor/services/envoy.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/escalator.py` & `gufo_thor-0.5.0/src/gufo/thor/services/escalator.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/grafanads.py` & `gufo_thor-0.5.0/src/gufo/thor/services/grafanads.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/icqsender.py` & `gufo_thor-0.5.0/src/gufo/thor/services/icqsender.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/kafkasender.py` & `gufo_thor-0.5.0/src/gufo/thor/services/kafkasender.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/liftbridge.py` & `gufo_thor-0.5.0/src/gufo/thor/services/liftbridge.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/login.py` & `gufo_thor-0.5.0/src/gufo/thor/services/login.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/mailsender.py` & `gufo_thor-0.5.0/src/gufo/thor/services/mailsender.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/metrics.py` & `gufo_thor-0.5.0/src/gufo/thor/services/metrics.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/metricscollector.py` & `gufo_thor-0.5.0/src/gufo/thor/services/metricscollector.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/migrate.py` & `gufo_thor-0.5.0/src/gufo/thor/services/migrate.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,26 @@
     """
 
     name = "migrate"
     dependencies = (clickhouse, consul, liftbridge, mongo, postgres)
     compose_depends_condition = ComposeDependsCondition.COMPLETED_SUCCESSFULLY
     compose_command = "./scripts/deploy/migrate.sh"
 
+    def get_compose_command(
+        self: "MigrateService", config: Config, svc: Optional[ServiceConfig]
+    ) -> Optional[str]:
+        """
+        Get compose command.
+
+        Considers config.cli.no_migrations option.
+        """
+        if config.cli.no_migrate:
+            return "/bin/true"
+        return self.compose_command
+
     def get_compose_volumes(
         self: "MigrateService", config: Config, svc: Optional[ServiceConfig]
     ) -> Optional[List[str]]:
         """
         Get volumes settings for docker compose.
 
         Additionaly map slots configuration.
```

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/mongo.py` & `gufo_thor-0.5.0/src/gufo/thor/services/mongo.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/nbi.py` & `gufo_thor-0.5.0/src/gufo/thor/services/nbi.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/noc.py` & `gufo_thor-0.5.0/src/gufo/thor/services/noc.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/ping.py` & `gufo_thor-0.5.0/src/gufo/thor/services/ping.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/postgres.py` & `gufo_thor-0.5.0/src/gufo/thor/services/postgres.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/runner.py` & `gufo_thor-0.5.0/src/gufo/thor/services/runner.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/sae.py` & `gufo_thor-0.5.0/src/gufo/thor/services/sae.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/scheduler.py` & `gufo_thor-0.5.0/src/gufo/thor/services/scheduler.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/selfmon.py` & `gufo_thor-0.5.0/src/gufo/thor/services/selfmon.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/shell.py` & `gufo_thor-0.5.0/src/gufo/thor/services/shell.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,26 +12,25 @@
 
 # Gufo Thor modules
 from typing import Optional
 
 from gufo.thor.config import Config, ServiceConfig
 
 from .clickhouse import clickhouse
-from .migrate import migrate
 from .mongo import mongo
 from .noc import NocService
 from .postgres import postgres
 from .worker import worker
 
 
 class ShellService(NocService):
     """web service."""
 
     name = "shell"
-    dependencies = (clickhouse, migrate, mongo, postgres, worker)
+    dependencies = (clickhouse, mongo, postgres, worker)
     compose_extra = {"scale": 0}
 
     def get_compose_command(
         self: NocService, config: Config, svc: Optional[ServiceConfig]
     ) -> Optional[str]:
         """Override to bash."""
         return "/bin/bash"
```

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/static.py` & `gufo_thor-0.5.0/src/gufo/thor/services/static.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/syslogcollector.py` & `gufo_thor-0.5.0/src/gufo/thor/services/syslogcollector.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/tgsender.py` & `gufo_thor-0.5.0/src/gufo/thor/services/tgsender.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/topo.py` & `gufo_thor-0.5.0/src/gufo/thor/services/topo.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/trapcollector.py` & `gufo_thor-0.5.0/src/gufo/thor/services/trapcollector.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/ui.py` & `gufo_thor-0.5.0/src/gufo/thor/services/ui.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/web.py` & `gufo_thor-0.5.0/src/gufo/thor/services/web.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/worker.py` & `gufo_thor-0.5.0/src/gufo/thor/services/worker.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/services/zeroconf.py` & `gufo_thor-0.5.0/src/gufo/thor/services/zeroconf.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/targets/base.py` & `gufo_thor-0.5.0/src/gufo/thor/targets/base.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/targets/compose.py` & `gufo_thor-0.5.0/src/gufo/thor/targets/compose.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/templates/envoy/envoy.yaml` & `gufo_thor-0.5.0/src/gufo/thor/templates/envoy/envoy.yaml`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo/thor/utils.py` & `gufo_thor-0.5.0/src/gufo/thor/utils.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/src/gufo_thor.egg-info/PKG-INFO` & `gufo_thor-0.5.0/src/gufo_thor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gufo_thor
-Version: 0.4.0
+Version: 0.5.0
 Author: Gufo Labs
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/gufolabs/gufo_thor/issues
 Project-URL: Changelog, https://github.com/gufolabs/gufo_thor/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://docs.gufolabs.com/gufo_thor/
 Project-URL: Homepage, https://github.com/gufolabs/gufo_thor/
 Project-URL: Source Code, https://github.com/gufolabs/gufo_thor/
```

### Comparing `gufo_thor-0.4.0/src/gufo_thor.egg-info/SOURCES.txt` & `gufo_thor-0.5.0/src/gufo_thor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/tests/test_ci.py` & `gufo_thor-0.5.0/tests/test_ci.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 def _get_root() -> str:
     mod_path = inspect.getfile(sys.modules[__name__])
     rel_root = os.path.dirname(mod_path)
     return os.path.abspath(os.path.join(rel_root, ".."))
 
 
 VERSIONS = [
-    "actions/cache@v3",
-    "actions/checkout@v3",
-    "actions/setup-python@v4",
+    "actions/cache@v4",
+    "actions/checkout@v4",
+    "actions/setup-python@v5",
     "pypa/gh-action-pypi-publish@release/v1",
 ]
 
 
 @dataclass
 class Action(object):
     path: str
```

### Comparing `gufo_thor-0.4.0/tests/test_compose.py` & `gufo_thor-0.5.0/tests/test_compose.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/tests/test_config.py` & `gufo_thor-0.5.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gufo_thor-0.4.0/tests/test_docs.py` & `gufo_thor-0.5.0/tests/test_docs.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 import pytest
 
 _doc_files: Optional[List[str]] = None
 
 rx_link = re.compile(r"\[([^\]]+)\]\[([^\]]+)\]", re.MULTILINE)
 rx_link_def = re.compile(r"^\[([^\]]+)\]:", re.MULTILINE)
 rx_footnote = re.compile(r"[^\]]\[(\^\d+)\][^\[]", re.MULTILINE)
+rx_datatracker_ietf = re.compile(
+    r"https://datatracker\.ietf\.org/doc/[^/]+/(rfc\d+)", re.MULTILINE
+)
 
 
 @lru_cache(maxsize=1)
 def get_docs() -> List[str]:
     doc_files: List[str] = []
     for root, _, files in os.walk("docs"):
         for f in files:
@@ -40,13 +43,21 @@
 def test_links(doc: str) -> None:
     data = get_file(doc)
     links: Set[str] = set()
     defs: Set[str] = set()
     for match in rx_link.finditer(data):
         links.add(match.group(2))
     for match in rx_footnote.finditer(data):
-        print(match.group(1))
         links.add(match.group(1))
     for match in rx_link_def.finditer(data):
         d = match.group(1)
         assert d not in defs, f"Link already defined: {d}"
         assert d in links, f"Unused link definition: {d}"
+
+
+@pytest.mark.parametrize("doc", get_docs())
+def test_rfc_links(doc: str) -> None:
+    data = get_file(doc)
+    match = rx_datatracker_ietf.search(data)
+    assert (
+        not match
+    ), f"{match.group(0)} link used. Must be https://www.rfc-editor.org/rfc/{match.group(1)}.html"
```

### Comparing `gufo_thor-0.4.0/tests/test_project.py` & `gufo_thor-0.5.0/tests/test_project.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # ---------------------------------------------------------------------
 # Gufo Labs: Project structure tests
 # ---------------------------------------------------------------------
-# Copyright (C) 2022-23, Gufo Labs
+# Copyright (C) 2022-24, Gufo Labs
 # See LICENSE.md for details
 # ---------------------------------------------------------------------
 
 # Python modules
 import inspect
 import os
 import sys
+from pathlib import Path
 from typing import Tuple, Union
 
 # Third-party modules
 import pytest
 
 
 def _get_root() -> str:
@@ -26,21 +27,30 @@
     Get project information.
 
     Returns:
         Tuple of (project path, project module)
     """
 
     def explore_dir(*args: str) -> str:
+        def is_not_rust(path: Path) -> bool:
+            if not path.is_dir():
+                return True
+            return not any(path.rglob("*.rs"))
+
+        root = Path(*args)
         d = [
             f
             for f in os.listdir(os.path.join(*args))
             if not f.startswith(".")
             and not f.startswith("_")
             and not f.endswith(".egg-info")
+            and not f.endswith(".rs")
         ]
+        if len(d) > 1:
+            d = [x for x in d if is_not_rust(root / x)]
         assert len(d) == 1
         return d[0]
 
     ns = explore_dir(ROOT, "src")
     if ns == "gufo":
         # gufo.* namespace
         pkg = explore_dir(ROOT, "src", ns)
@@ -66,22 +76,22 @@
     "CODE_OF_CONDUCT.md",
     "CONTRIBUTING.md",
     "Dockerfile",
     "LICENSE.md",
     "README.md",
     "SECURITY.md",
     "docs/assets/logo.png",
-    "docs/codebase.md",
-    "docs/codequality.md",
-    "docs/devcommon.md",
-    "docs/environment.md",
+    "docs/dev/codebase.md",
+    "docs/dev/codequality.md",
+    "docs/dev/common.md",
+    "docs/dev/environment.md",
+    "docs/dev/testing.md",
     "docs/faq.md",
     "docs/index.md",
     ("docs/installation.md", "docs/installation/index.md"),
-    "docs/testing.md",
     "mkdocs.yml",
     "pyproject.toml",
     f"{PROJECT_SRC}/__init__.py",
     f"{PROJECT_SRC}/py.typed",
     "tests/test_docs.py",
     "tests/test_project.py",
 ]
```

### Comparing `gufo_thor-0.4.0/tests/test_service.py` & `gufo_thor-0.5.0/tests/test_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,16 @@
         ), "Not exposes http prefix, must not have `envoy` dependency"
 
 
 @pytest.mark.parametrize("svc", ALL_SERVICES)
 def test_migrate_deps(svc: str) -> None:
     if svc == "migrate":
         pytest.skip("migrate service")
+    if svc == "shell":
+        return
     service = loader[svc]
     deps = set(service.iter_dependencies())
     if mongo in deps:
         assert migrate in deps, "Depends on `mongo`, must depend on `migrate`"
     if postgres in deps:
         assert (
             migrate in deps
@@ -221,15 +223,14 @@
   migrate -> scheduler
   mongo -> scheduler
   postgres -> scheduler
   migrate -> selfmon
   mongo -> selfmon
   postgres -> selfmon
   clickhouse -> shell
-  migrate -> shell
   mongo -> shell
   postgres -> shell
   worker -> shell
   envoy -> static
   datastream -> syslogcollector
   liftbridge -> syslogcollector
   migrate -> syslogcollector
```

